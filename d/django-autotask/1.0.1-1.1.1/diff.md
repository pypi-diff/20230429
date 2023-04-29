# Comparing `tmp/django-autotask-1.0.1.tar.gz` & `tmp/django-autotask-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-autotask-1.0.1.tar", last modified: Fri Apr 28 17:01:45 2023, max compression
+gzip compressed data, was "django-autotask-1.1.1.tar", last modified: Sat Apr 29 00:44:21 2023, max compression
```

## Comparing `django-autotask-1.0.1.tar` & `django-autotask-1.1.1.tar`

### file list

```diff
@@ -1,341 +1,341 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 17:01:45.811685 django-autotask-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-04-28 17:00:53.000000 django-autotask-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-04-28 17:00:53.000000 django-autotask-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-04-28 17:01:45.811685 django-autotask-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      885 2023-04-28 17:00:53.000000 django-autotask-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 17:01:45.775684 django-autotask-1.0.1/django_autotask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-04-28 17:01:45.000000 django-autotask-1.0.1/django_autotask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    18996 2023-04-28 17:01:45.000000 django-autotask-1.0.1/django_autotask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 17:01:45.000000 django-autotask-1.0.1/django_autotask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 17:01:08.000000 django-autotask-1.0.1/django_autotask.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-28 17:01:45.000000 django-autotask-1.0.1/django_autotask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-28 17:01:45.000000 django-autotask-1.0.1/django_autotask.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 17:01:45.775684 django-autotask-1.0.1/djautotask/
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 17:01:45.775684 django-autotask-1.0.1/djautotask/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-28 17:01:08.000000 django-autotask-1.0.1/djautotask/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)    29142 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/__pycache__/api.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-04-28 17:01:17.000000 django-autotask-1.0.1/djautotask/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)    47691 2023-04-28 17:01:17.000000 django-autotask-1.0.1/djautotask/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)    57154 2023-04-28 17:01:26.000000 django-autotask-1.0.1/djautotask/__pycache__/sync.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      370 2023-04-28 17:01:44.000000 django-autotask-1.0.1/djautotask/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-04-28 17:01:44.000000 django-autotask-1.0.1/djautotask/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)    10903 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    31778 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/api.py
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 17:01:45.775684 django-autotask-1.0.1/djautotask/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 17:01:45.775684 django-autotask-1.0.1/djautotask/management/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/management/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 17:01:45.775684 django-autotask-1.0.1/djautotask/management/commands/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 17:01:45.775684 django-autotask-1.0.1/djautotask/management/commands/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-28 17:01:32.000000 django-autotask-1.0.1/djautotask/management/commands/__pycache__/atsync.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     8434 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/management/commands/atsync.py
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/management/commands/clearoldsyncjobs.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/management/commands/list_users.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 17:01:45.791684 django-autotask-1.0.1/djautotask/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     2211 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0002_ticket_ticket_number.py
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0003_auto_20190913_0941.py
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0004_auto_20190913_1425.py
--rw-r--r--   0 runner    (1001) docker     (122)     1517 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0005_auto_20190916_1549.py
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0005_remove_ticketstatus_value.py
--rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0006_auto_20190916_1645.py
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0006_merge_20190920_1450.py
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0007_auto_20190917_1009.py
--rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0008_auto_20190917_1454.py
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0008_merge_20190920_1644.py
--rw-r--r--   0 runner    (1001) docker     (122)     4964 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0009_auto_20190918_1525.py
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0009_auto_20190920_1648.py
--rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0010_auto_20190923_0930.py
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0010_merge_20190923_1155.py
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0011_auto_20190923_1157.py
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0012_merge_20190923_1439.py
--rw-r--r--   0 runner    (1001) docker     (122)      446 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0013_auto_20190923_1439.py
--rw-r--r--   0 runner    (1001) docker     (122)     6182 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0014_auto_20190930_1548.py
--rw-r--r--   0 runner    (1001) docker     (122)     1583 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0015_auto_20191001_0847.py
--rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0016_auto_20191021_0958.py
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0017_auto_20191021_1028.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0018_auto_20191029_1621.py
--rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0018_auto_20191029_1634.py
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0019_auto_20191030_0905.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0020_auto_20191030_0916.py
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0021_merge_20191031_0858.py
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0021_merge_20191031_1259.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0022_merge_20191031_1620.py
--rw-r--r--   0 runner    (1001) docker     (122)      401 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0023_auto_20191119_0923.py
--rw-r--r--   0 runner    (1001) docker     (122)     3582 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0024_auto_20191122_1516.py
--rw-r--r--   0 runner    (1001) docker     (122)      362 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0025_auto_20191125_0939.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0026_auto_20191125_0952.py
--rw-r--r--   0 runner    (1001) docker     (122)      375 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0027_auto_20191125_1103.py
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0028_phase.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0028_task_secondary_resources.py
--rw-r--r--   0 runner    (1001) docker     (122)      398 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0029_phase_last_activity_date.py
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0030_task_phase.py
--rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0031_auto_20191129_1454.py
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0031_merge_20191202_1119.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0032_auto_20191129_1501.py
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0033_merge_20191204_1022.py
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0034_auto_20191210_1518.py
--rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0035_timeentry.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0036_auto_20200127_1157.py
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0037_subissuetype_parent_value.py
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0038_auto_20200130_1218.py
--rw-r--r--   0 runner    (1001) docker     (122)     4027 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0038_notetype_tasknote_ticketnote.py
--rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0039_auto_20200131_1134.py
--rw-r--r--   0 runner    (1001) docker     (122)      290 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0039_merge_20200131_1022.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0040_auto_20200204_1538.py
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0040_merge_20200131_1627.py
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0041_merge_20200204_1546.py
--rw-r--r--   0 runner    (1001) docker     (122)     2395 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0042_auto_20200205_1057.py
--rw-r--r--   0 runner    (1001) docker     (122)     1304 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0042_auto_20200205_1455.py
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0043_department.py
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0043_timeentry_allocation_code.py
--rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0044_merge_20200205_1651.py
--rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0045_resourceroledepartment_resourceservicedeskrole.py
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0046_auto_20200207_1002.py
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0046_ticket_assigned_resource_role.py
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0047_auto_20200207_1126.py
--rw-r--r--   0 runner    (1001) docker     (122)      523 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0047_task_assigned_resource_role.py
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0048_auto_20200211_1037.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0049_merge_20200227_1701.py
--rw-r--r--   0 runner    (1001) docker     (122)      331 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0050_remove_ticket_role.py
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0051_auto_20200315_1819.py
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0051_contract.py
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0052_contract_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0053_timeentry_contract.py
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0054_merge_20200323_1511.py
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0055_auto_20200325_0928.py
--rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0055_auto_20200325_1335.py
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0056_merge_20200327_1045.py
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0057_auto_20200406_1620.py
--rw-r--r--   0 runner    (1001) docker     (122)      717 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0058_auto_20200408_1022.py
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0059_auto_20200414_1242.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0060_auto_20200414_1522.py
--rw-r--r--   0 runner    (1001) docker     (122)      410 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0061_auto_20200416_1241.py
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0062_task_department.py
--rw-r--r--   0 runner    (1001) docker     (122)      822 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0063_accountphysicallocation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0064_auto_20200511_1124.py
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0064_servicecall_location.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0065_auto_20200512_1224.py
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0066_auto_20200512_1420.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0067_auto_20200519_1100.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0067_merge_20200514_1713.py
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0068_merge_20200521_1615.py
--rw-r--r--   0 runner    (1001) docker     (122)      777 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0069_auto_20200602_1419.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0070_auto_20200714_0807.py
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0071_project_status_detail.py
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0072_account_parent_account.py
--rw-r--r--   0 runner    (1001) docker     (122)      401 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0073_syncjob_skipped.py
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0074_auto_20200827_1818.py
--rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0075_taskpredecessor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0076_auto_20200923_0953.py
--rw-r--r--   0 runner    (1001) docker     (122)      982 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0076_auto_20200925_1326.py
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0077_auto_20200924_1512.py
--rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0078_merge_20201001_1657.py
--rw-r--r--   0 runner    (1001) docker     (122)      391 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0079_auto_20201003_1125.py
--rw-r--r--   0 runner    (1001) docker     (122)    14818 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0080_accountphysicallocationtracker_accounttracker_accounttypetracker_allocationcodetracker_contracttrack.py
--rw-r--r--   0 runner    (1001) docker     (122)      590 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0081_project_department.py
--rw-r--r--   0 runner    (1001) docker     (122)     3176 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0082_auto_20201020_1617.py
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0083_ticketudftracker.py
--rw-r--r--   0 runner    (1001) docker     (122)      917 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0084_projectudftracker_taskudftracker.py
--rw-r--r--   0 runner    (1001) docker     (122)      589 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0085_auto_20201022_1822.py
--rw-r--r--   0 runner    (1001) docker     (122)     2105 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0086_auto_20201222_1402.py
--rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0087_auto_20210108_1214.py
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0087_auto_20210108_1307.py
--rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0088_merge_20210113_1743.py
--rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0089_auto_20210125_1649.py
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0090_auto_20210309_1157.py
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0091_auto_20210525_1723.py
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0092_auto_20210629_1124.py
--rw-r--r--   0 runner    (1001) docker     (122)      477 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0093_auto_20210629_1204.py
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0094_auto_20210723_1018.py
--rw-r--r--   0 runner    (1001) docker     (122)      608 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0094_auto_20210727_0940.py
--rw-r--r--   0 runner    (1001) docker     (122)      368 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0095_auto_20210726_1251.py
--rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0096_merge_20210728_1429.py
--rw-r--r--   0 runner    (1001) docker     (122)      707 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0097_auto_20210819_1402.py
--rw-r--r--   0 runner    (1001) docker     (122)      430 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0098_auto_20211029_1641.py
--rw-r--r--   0 runner    (1001) docker     (122)      528 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0099_auto_20211124_1808.py
--rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0100_auto_20211228_1443.py
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0101_auto_20220104_1349.py
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0102_auto_20220104_1655.py
--rw-r--r--   0 runner    (1001) docker     (122)      391 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0103_auto_20220106_1622.py
--rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0104_rename_allocationcode_billingcode_and_more.py
--rw-r--r--   0 runner    (1001) docker     (122)      538 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0105_tasknote_created_by_contact.py
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0106_ticketnote_created_by_contact.py
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0107_contact_extension.py
--rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0108_billingcodetype_billingcodetypetracker.py
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0109_billingcode_billing_code_type.py
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0110_account_phone.py
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0111_alter_phase_estimated_hours.py
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/0112_account_owner_resource.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 17:01:45.807685 django-autotask-1.0.1/djautotask/migrations/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0001_initial.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0002_ticket_ticket_number.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1517 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0003_auto_20190913_0941.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0004_auto_20190913_1425.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0005_auto_20190916_1549.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0005_remove_ticketstatus_value.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0006_auto_20190916_1645.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0006_merge_20190920_1450.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0007_auto_20190917_1009.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0008_auto_20190917_1454.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0008_merge_20190920_1644.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0009_auto_20190918_1525.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0009_auto_20190920_1648.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0010_auto_20190923_0930.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0010_merge_20190923_1155.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      574 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0011_auto_20190923_1157.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0012_merge_20190923_1439.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0013_auto_20190923_1439.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     2594 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0014_auto_20190930_1548.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0015_auto_20191001_0847.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0016_auto_20191021_0958.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0017_auto_20191021_1028.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0018_auto_20191029_1621.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0018_auto_20191029_1634.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      659 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0019_auto_20191030_0905.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0020_auto_20191030_0916.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0021_merge_20191031_0858.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0021_merge_20191031_1259.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0022_merge_20191031_1620.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0023_auto_20191119_0923.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0024_auto_20191122_1516.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0025_auto_20191125_0939.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      580 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0026_auto_20191125_0952.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      580 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0027_auto_20191125_1103.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0028_phase.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      732 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0028_task_secondary_resources.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0029_phase_last_activity_date.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0030_task_phase.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0031_auto_20191129_1454.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0031_merge_20191202_1119.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      755 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0032_auto_20191129_1501.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0033_merge_20191204_1022.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      739 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0034_auto_20191210_1518.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1673 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0035_timeentry.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      860 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0036_auto_20200127_1157.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      755 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0037_subissuetype_parent_value.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0038_auto_20200130_1218.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0038_notetype_tasknote_ticketnote.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1429 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0039_auto_20200131_1134.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0039_merge_20200131_1022.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0040_auto_20200204_1538.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0040_merge_20200131_1627.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0041_merge_20200204_1546.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0042_auto_20200205_1057.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0042_auto_20200205_1455.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0043_department.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0043_timeentry_allocation_code.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0044_merge_20200205_1651.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0045_resourceroledepartment_resourceservicedeskrole.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0046_auto_20200207_1002.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0046_ticket_assigned_resource_role.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      803 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0047_auto_20200207_1126.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0047_task_assigned_resource_role.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0048_auto_20200211_1037.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0049_merge_20200227_1701.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0050_remove_ticket_role.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      816 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0051_auto_20200315_1819.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0051_contract.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0052_contract_status.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0053_timeentry_contract.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0054_merge_20200323_1511.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      794 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0055_auto_20200325_0928.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0055_auto_20200325_1335.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0056_merge_20200327_1045.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0057_auto_20200406_1620.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0058_auto_20200408_1022.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0059_auto_20200414_1242.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0060_auto_20200414_1522.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0061_auto_20200416_1241.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      737 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0062_task_department.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0063_accountphysicallocation.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      942 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0064_auto_20200511_1124.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0064_servicecall_location.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0065_auto_20200512_1224.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0066_auto_20200512_1420.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      880 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0067_auto_20200519_1100.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0067_merge_20200514_1713.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0068_merge_20200521_1615.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      822 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0069_auto_20200602_1419.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0070_auto_20200714_0807.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0071_project_status_detail.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0072_account_parent_account.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0073_syncjob_skipped.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0074_auto_20200827_1818.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1263 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0075_taskpredecessor.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0076_auto_20200923_0953.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0076_auto_20200925_1326.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      814 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0077_auto_20200924_1512.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0078_merge_20201001_1657.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0079_auto_20201003_1125.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     5525 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0080_accountphysicallocationtracker_accounttracker_accounttypetracker_allocationcodetracker_contracttrack.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0081_project_department.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0082_auto_20201020_1617.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0083_ticketudftracker.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      793 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0084_projectudftracker_taskudftracker.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0085_auto_20201022_1822.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0086_auto_20201222_1402.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0087_auto_20210108_1214.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0087_auto_20210108_1307.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0088_merge_20210113_1743.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0089_auto_20210125_1649.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0090_auto_20210309_1157.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      637 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0091_auto_20210525_1723.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0092_auto_20210629_1124.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      717 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0093_auto_20210629_1204.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0094_auto_20210723_1018.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0094_auto_20210727_0940.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0095_auto_20210726_1251.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0096_merge_20210728_1429.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      862 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0097_auto_20210819_1402.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0098_auto_20211029_1641.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0099_auto_20211124_1808.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0100_auto_20211228_1443.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      589 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0101_auto_20220104_1349.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0102_auto_20220104_1655.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0103_auto_20220106_1622.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0104_rename_allocationcode_billingcode_and_more.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      782 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0105_tasknote_created_by_contact.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0106_ticketnote_created_by_contact.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0107_contact_extension.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0108_billingcodetype_billingcodetypetracker.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      790 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0109_billingcode_billing_code_type.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0110_account_phone.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0111_alter_phase_estimated_hours.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/0112_account_owner_resource.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-28 17:01:18.000000 django-autotask-1.0.1/djautotask/migrations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)    44367 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/models.py
--rw-r--r--   0 runner    (1001) docker     (122)    70445 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 17:01:45.807685 django-autotask-1.0.1/djautotask/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/templates/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 17:01:45.811685 django-autotask-1.0.1/djautotask/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 17:01:45.811685 django-autotask-1.0.1/djautotask/tests/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-28 17:01:26.000000 django-autotask-1.0.1/djautotask/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)    14124 2023-04-28 17:01:26.000000 django-autotask-1.0.1/djautotask/tests/__pycache__/fixture_utils.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)    14344 2023-04-28 17:01:26.000000 django-autotask-1.0.1/djautotask/tests/__pycache__/fixtures.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-04-28 17:01:26.000000 django-autotask-1.0.1/djautotask/tests/__pycache__/mocks.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     6805 2023-04-28 17:01:26.000000 django-autotask-1.0.1/djautotask/tests/__pycache__/test_api.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)    29946 2023-04-28 17:01:26.000000 django-autotask-1.0.1/djautotask/tests/__pycache__/test_commands.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-04-28 17:01:26.000000 django-autotask-1.0.1/djautotask/tests/__pycache__/test_model.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)    51638 2023-04-28 17:01:26.000000 django-autotask-1.0.1/djautotask/tests/__pycache__/test_sync.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-28 17:01:26.000000 django-autotask-1.0.1/djautotask/tests/__pycache__/test_views.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      317 2023-04-28 17:01:44.000000 django-autotask-1.0.1/djautotask/tests/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (122)    11695 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/tests/fixture_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    39489 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     8430 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     6592 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    31888 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     3794 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    53083 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     2268 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-04-28 17:00:53.000000 django-autotask-1.0.1/djautotask/views.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-28 17:01:45.811685 django-autotask-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-04-28 17:00:53.000000 django-autotask-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 00:44:21.561198 django-autotask-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-04-29 00:43:30.000000 django-autotask-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-04-29 00:43:30.000000 django-autotask-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-04-29 00:44:21.561198 django-autotask-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-04-29 00:43:30.000000 django-autotask-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 00:44:21.505196 django-autotask-1.1.1/django_autotask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-04-29 00:44:21.000000 django-autotask-1.1.1/django_autotask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    18996 2023-04-29 00:44:21.000000 django-autotask-1.1.1/django_autotask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-29 00:44:21.000000 django-autotask-1.1.1/django_autotask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-29 00:43:45.000000 django-autotask-1.1.1/django_autotask.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-29 00:44:21.000000 django-autotask-1.1.1/django_autotask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-29 00:44:21.000000 django-autotask-1.1.1/django_autotask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 00:44:21.505196 django-autotask-1.1.1/djautotask/
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 00:44:21.509196 django-autotask-1.1.1/djautotask/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-29 00:43:45.000000 django-autotask-1.1.1/djautotask/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    30481 2023-04-29 00:43:53.000000 django-autotask-1.1.1/djautotask/__pycache__/api.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-04-29 00:43:53.000000 django-autotask-1.1.1/djautotask/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    47691 2023-04-29 00:43:53.000000 django-autotask-1.1.1/djautotask/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    58453 2023-04-29 00:44:01.000000 django-autotask-1.1.1/djautotask/__pycache__/sync.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      370 2023-04-29 00:44:20.000000 django-autotask-1.1.1/djautotask/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-04-29 00:44:20.000000 django-autotask-1.1.1/djautotask/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    10903 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33499 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 00:44:21.509196 django-autotask-1.1.1/djautotask/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 00:44:21.509196 django-autotask-1.1.1/djautotask/management/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 00:44:21.509196 django-autotask-1.1.1/djautotask/management/commands/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 00:44:21.509196 django-autotask-1.1.1/djautotask/management/commands/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-29 00:44:08.000000 django-autotask-1.1.1/djautotask/management/commands/__pycache__/atsync.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     8434 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/management/commands/atsync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/management/commands/clearoldsyncjobs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/management/commands/list_users.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 00:44:21.533197 django-autotask-1.1.1/djautotask/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2211 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0002_ticket_ticket_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0003_auto_20190913_0941.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0004_auto_20190913_1425.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1517 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0005_auto_20190916_1549.py
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0005_remove_ticketstatus_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0006_auto_20190916_1645.py
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0006_merge_20190920_1450.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0007_auto_20190917_1009.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0008_auto_20190917_1454.py
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0008_merge_20190920_1644.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4964 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0009_auto_20190918_1525.py
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0009_auto_20190920_1648.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0010_auto_20190923_0930.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0010_merge_20190923_1155.py
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0011_auto_20190923_1157.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0012_merge_20190923_1439.py
+-rw-r--r--   0 runner    (1001) docker     (122)      446 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0013_auto_20190923_1439.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6182 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0014_auto_20190930_1548.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1583 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0015_auto_20191001_0847.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0016_auto_20191021_0958.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0017_auto_20191021_1028.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0018_auto_20191029_1621.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0018_auto_20191029_1634.py
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0019_auto_20191030_0905.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0020_auto_20191030_0916.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0021_merge_20191031_0858.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0021_merge_20191031_1259.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0022_merge_20191031_1620.py
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0023_auto_20191119_0923.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3582 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0024_auto_20191122_1516.py
+-rw-r--r--   0 runner    (1001) docker     (122)      362 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0025_auto_20191125_0939.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0026_auto_20191125_0952.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0027_auto_20191125_1103.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0028_phase.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0028_task_secondary_resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)      398 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0029_phase_last_activity_date.py
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0030_task_phase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0031_auto_20191129_1454.py
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0031_merge_20191202_1119.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0032_auto_20191129_1501.py
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0033_merge_20191204_1022.py
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0034_auto_20191210_1518.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0035_timeentry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0036_auto_20200127_1157.py
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0037_subissuetype_parent_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0038_auto_20200130_1218.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4027 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0038_notetype_tasknote_ticketnote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0039_auto_20200131_1134.py
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0039_merge_20200131_1022.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0040_auto_20200204_1538.py
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0040_merge_20200131_1627.py
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0041_merge_20200204_1546.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2395 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0042_auto_20200205_1057.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1304 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0042_auto_20200205_1455.py
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0043_department.py
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0043_timeentry_allocation_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0044_merge_20200205_1651.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0045_resourceroledepartment_resourceservicedeskrole.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0046_auto_20200207_1002.py
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0046_ticket_assigned_resource_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0047_auto_20200207_1126.py
+-rw-r--r--   0 runner    (1001) docker     (122)      523 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0047_task_assigned_resource_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0048_auto_20200211_1037.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0049_merge_20200227_1701.py
+-rw-r--r--   0 runner    (1001) docker     (122)      331 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0050_remove_ticket_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0051_auto_20200315_1819.py
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0051_contract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0052_contract_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0053_timeentry_contract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0054_merge_20200323_1511.py
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0055_auto_20200325_0928.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0055_auto_20200325_1335.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0056_merge_20200327_1045.py
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0057_auto_20200406_1620.py
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0058_auto_20200408_1022.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0059_auto_20200414_1242.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0060_auto_20200414_1522.py
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0061_auto_20200416_1241.py
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0062_task_department.py
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0063_accountphysicallocation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0064_auto_20200511_1124.py
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0064_servicecall_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0065_auto_20200512_1224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0066_auto_20200512_1420.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0067_auto_20200519_1100.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0067_merge_20200514_1713.py
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0068_merge_20200521_1615.py
+-rw-r--r--   0 runner    (1001) docker     (122)      777 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0069_auto_20200602_1419.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0070_auto_20200714_0807.py
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0071_project_status_detail.py
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0072_account_parent_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0073_syncjob_skipped.py
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0074_auto_20200827_1818.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0075_taskpredecessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0076_auto_20200923_0953.py
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0076_auto_20200925_1326.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0077_auto_20200924_1512.py
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0078_merge_20201001_1657.py
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0079_auto_20201003_1125.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14818 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0080_accountphysicallocationtracker_accounttracker_accounttypetracker_allocationcodetracker_contracttrack.py
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0081_project_department.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3176 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0082_auto_20201020_1617.py
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0083_ticketudftracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      917 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0084_projectudftracker_taskudftracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0085_auto_20201022_1822.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2105 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0086_auto_20201222_1402.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0087_auto_20210108_1214.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0087_auto_20210108_1307.py
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0088_merge_20210113_1743.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0089_auto_20210125_1649.py
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0090_auto_20210309_1157.py
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0091_auto_20210525_1723.py
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0092_auto_20210629_1124.py
+-rw-r--r--   0 runner    (1001) docker     (122)      477 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0093_auto_20210629_1204.py
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0094_auto_20210723_1018.py
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0094_auto_20210727_0940.py
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0095_auto_20210726_1251.py
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0096_merge_20210728_1429.py
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0097_auto_20210819_1402.py
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0098_auto_20211029_1641.py
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0099_auto_20211124_1808.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0100_auto_20211228_1443.py
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0101_auto_20220104_1349.py
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0102_auto_20220104_1655.py
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0103_auto_20220106_1622.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0104_rename_allocationcode_billingcode_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0105_tasknote_created_by_contact.py
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0106_ticketnote_created_by_contact.py
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0107_contact_extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0108_billingcodetype_billingcodetypetracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0109_billingcode_billing_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0110_account_phone.py
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0111_alter_phase_estimated_hours.py
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/0112_account_owner_resource.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 00:44:21.557198 django-autotask-1.1.1/djautotask/migrations/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0001_initial.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0002_ticket_ticket_number.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1517 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0003_auto_20190913_0941.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0004_auto_20190913_1425.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0005_auto_20190916_1549.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0005_remove_ticketstatus_value.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0006_auto_20190916_1645.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0006_merge_20190920_1450.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0007_auto_20190917_1009.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0008_auto_20190917_1454.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0008_merge_20190920_1644.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0009_auto_20190918_1525.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0009_auto_20190920_1648.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0010_auto_20190923_0930.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0010_merge_20190923_1155.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0011_auto_20190923_1157.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0012_merge_20190923_1439.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0013_auto_20190923_1439.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     2594 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0014_auto_20190930_1548.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0015_auto_20191001_0847.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0016_auto_20191021_0958.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0017_auto_20191021_1028.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0018_auto_20191029_1621.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0018_auto_20191029_1634.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      659 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0019_auto_20191030_0905.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0020_auto_20191030_0916.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0021_merge_20191031_0858.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0021_merge_20191031_1259.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0022_merge_20191031_1620.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0023_auto_20191119_0923.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0024_auto_20191122_1516.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0025_auto_20191125_0939.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      580 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0026_auto_20191125_0952.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      580 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0027_auto_20191125_1103.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0028_phase.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0028_task_secondary_resources.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0029_phase_last_activity_date.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0030_task_phase.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0031_auto_20191129_1454.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0031_merge_20191202_1119.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0032_auto_20191129_1501.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0033_merge_20191204_1022.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      739 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0034_auto_20191210_1518.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1673 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0035_timeentry.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      860 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0036_auto_20200127_1157.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0037_subissuetype_parent_value.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0038_auto_20200130_1218.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0038_notetype_tasknote_ticketnote.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1429 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0039_auto_20200131_1134.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0039_merge_20200131_1022.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0040_auto_20200204_1538.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0040_merge_20200131_1627.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0041_merge_20200204_1546.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0042_auto_20200205_1057.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0042_auto_20200205_1455.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0043_department.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0043_timeentry_allocation_code.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0044_merge_20200205_1651.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0045_resourceroledepartment_resourceservicedeskrole.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0046_auto_20200207_1002.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0046_ticket_assigned_resource_role.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      803 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0047_auto_20200207_1126.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0047_task_assigned_resource_role.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0048_auto_20200211_1037.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0049_merge_20200227_1701.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0050_remove_ticket_role.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      816 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0051_auto_20200315_1819.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0051_contract.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0052_contract_status.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0053_timeentry_contract.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0054_merge_20200323_1511.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      794 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0055_auto_20200325_0928.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0055_auto_20200325_1335.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0056_merge_20200327_1045.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0057_auto_20200406_1620.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0058_auto_20200408_1022.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0059_auto_20200414_1242.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0060_auto_20200414_1522.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0061_auto_20200416_1241.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      737 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0062_task_department.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0063_accountphysicallocation.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0064_auto_20200511_1124.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0064_servicecall_location.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0065_auto_20200512_1224.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0066_auto_20200512_1420.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0067_auto_20200519_1100.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0067_merge_20200514_1713.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0068_merge_20200521_1615.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0069_auto_20200602_1419.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0070_auto_20200714_0807.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0071_project_status_detail.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0072_account_parent_account.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0073_syncjob_skipped.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0074_auto_20200827_1818.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1263 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0075_taskpredecessor.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0076_auto_20200923_0953.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0076_auto_20200925_1326.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0077_auto_20200924_1512.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0078_merge_20201001_1657.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0079_auto_20201003_1125.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     5525 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0080_accountphysicallocationtracker_accounttracker_accounttypetracker_allocationcodetracker_contracttrack.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0081_project_department.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0082_auto_20201020_1617.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0083_ticketudftracker.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0084_projectudftracker_taskudftracker.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0085_auto_20201022_1822.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0086_auto_20201222_1402.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0087_auto_20210108_1214.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0087_auto_20210108_1307.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0088_merge_20210113_1743.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0089_auto_20210125_1649.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0090_auto_20210309_1157.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0091_auto_20210525_1723.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0092_auto_20210629_1124.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0093_auto_20210629_1204.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0094_auto_20210723_1018.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0094_auto_20210727_0940.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0095_auto_20210726_1251.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0096_merge_20210728_1429.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0097_auto_20210819_1402.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0098_auto_20211029_1641.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0099_auto_20211124_1808.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0100_auto_20211228_1443.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0101_auto_20220104_1349.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0102_auto_20220104_1655.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0103_auto_20220106_1622.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0104_rename_allocationcode_billingcode_and_more.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      782 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0105_tasknote_created_by_contact.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0106_ticketnote_created_by_contact.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0107_contact_extension.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0108_billingcodetype_billingcodetypetracker.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0109_billingcode_billing_code_type.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0110_account_phone.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0111_alter_phase_estimated_hours.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/0112_account_owner_resource.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-29 00:43:54.000000 django-autotask-1.1.1/djautotask/migrations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    44367 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71799 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 00:44:21.557198 django-autotask-1.1.1/djautotask/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/templates/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 00:44:21.561198 django-autotask-1.1.1/djautotask/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 00:44:21.561198 django-autotask-1.1.1/djautotask/tests/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-29 00:44:01.000000 django-autotask-1.1.1/djautotask/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    14124 2023-04-29 00:44:01.000000 django-autotask-1.1.1/djautotask/tests/__pycache__/fixture_utils.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    14344 2023-04-29 00:44:01.000000 django-autotask-1.1.1/djautotask/tests/__pycache__/fixtures.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-04-29 00:44:01.000000 django-autotask-1.1.1/djautotask/tests/__pycache__/mocks.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     6805 2023-04-29 00:44:01.000000 django-autotask-1.1.1/djautotask/tests/__pycache__/test_api.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    29946 2023-04-29 00:44:01.000000 django-autotask-1.1.1/djautotask/tests/__pycache__/test_commands.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-04-29 00:44:01.000000 django-autotask-1.1.1/djautotask/tests/__pycache__/test_model.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    51638 2023-04-29 00:44:01.000000 django-autotask-1.1.1/djautotask/tests/__pycache__/test_sync.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-29 00:44:01.000000 django-autotask-1.1.1/djautotask/tests/__pycache__/test_views.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      317 2023-04-29 00:44:20.000000 django-autotask-1.1.1/djautotask/tests/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    11695 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/tests/fixture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39489 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8430 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6592 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31888 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3794 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53083 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2268 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-04-29 00:43:30.000000 django-autotask-1.1.1/djautotask/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-29 00:44:21.561198 django-autotask-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-04-29 00:43:30.000000 django-autotask-1.1.1/setup.py
```

### Comparing `django-autotask-1.0.1/LICENSE` & `django-autotask-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/PKG-INFO` & `django-autotask-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-autotask
-Version: 1.0.1
+Version: 1.1.1
 Summary: Django app for working with Autotask. Defines models (tickets, members, companies, etc.) and callbacks.
 Home-page: https://github.com/KerkhoffTechnologies/django-autotask
 Author: Kerkhoff Technologies Inc.
 Author-email: matt@kerkhofftech.ca
 License: MIT
 Description: ## django-autotask
```

### Comparing `django-autotask-1.0.1/README.md` & `django-autotask-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/django_autotask.egg-info/PKG-INFO` & `django-autotask-1.1.1/django_autotask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-autotask
-Version: 1.0.1
+Version: 1.1.1
 Summary: Django app for working with Autotask. Defines models (tickets, members, companies, etc.) and callbacks.
 Home-page: https://github.com/KerkhoffTechnologies/django-autotask
 Author: Kerkhoff Technologies Inc.
 Author-email: matt@kerkhofftech.ca
 License: MIT
 Description: ## django-autotask
```

### Comparing `django-autotask-1.0.1/django_autotask.egg-info/SOURCES.txt` & `django-autotask-1.1.1/django_autotask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/__pycache__/api.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/__pycache__/api.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 31778 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 227c 0000  U.........Kd"|..
+00000000: 550d 0d0a 0000 0000 3268 4c64 db82 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 4404 0000 6400  .....@...sD...d.
+00000020: 0005 0000 0040 0000 0073 5404 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c02 6d04 5a04 0100 6400 6401 6c05  d.l.m.Z...d.d.l.
 00000060: 5a05 6400 6401 6c06 5a06 6400 6403 6c07  Z.d.d.l.Z.d.d.l.
 00000070: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000080: 0100 6400 6405 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
 00000090: 6406 6c0d 6d0e 5a0e 0100 6400 6407 6c0f  d.l.m.Z...d.d.l.
@@ -14,17 +14,17 @@
 000000d0: 6410 8400 6410 651b 8303 5a1c 4700 6411  d...d.e...Z.G.d.
 000000e0: 6412 8400 6412 651c 8303 5a1d 4700 6413  d...d.e...Z.G.d.
 000000f0: 6414 8400 6414 651c 8303 5a1e 4700 6415  d...d.e...Z.G.d.
 00000100: 6416 8400 6416 651d 8303 5a1f 4700 6417  d...d.e...Z.G.d.
 00000110: 6418 8400 6418 651d 8303 5a20 4700 6419  d...d.e...Z G.d.
 00000120: 641a 8400 641a 6520 8303 5a21 641b 641c  d...d.e ..Z!d.d.
 00000130: 8400 5a22 641d 641e 8400 5a23 641f 6420  ..Z"d.d...Z#d.d 
-00000140: 8400 5a24 6421 6422 8400 5a25 648a 6424  ..Z$d!d"..Z%d.d$
-00000150: 6425 8401 5a26 648b 6426 6427 8401 5a27  d%..Z&d.d&d'..Z'
-00000160: 648c 6428 6429 8401 5a28 642a 642b 8400  d.d(d)..Z(d*d+..
+00000140: 8400 5a24 6421 6422 8400 5a25 648c 6424  ..Z$d!d"..Z%d.d$
+00000150: 6425 8401 5a26 648d 6426 6427 8401 5a27  d%..Z&d.d&d'..Z'
+00000160: 648e 6428 6429 8401 5a28 642a 642b 8400  d.d(d)..Z(d*d+..
 00000170: 5a29 4700 642c 642d 8400 642d 8302 5a2a  Z)G.d,d-..d-..Z*
 00000180: 4700 642e 642f 8400 642f 8302 5a2b 4700  G.d.d/..d/..Z+G.
 00000190: 6430 6431 8400 6431 652c 8303 5a2d 4700  d0d1..d1e,..Z-G.
 000001a0: 6432 6433 8400 6433 8302 5a2e 4700 6434  d2d3..d3..Z.G.d4
 000001b0: 6435 8400 6435 652d 8303 5a2f 4700 6436  d5..d5e-..Z/G.d6
 000001c0: 6437 8400 6437 652d 8303 5a30 4700 6438  d7..d7e-..Z0G.d8
 000001d0: 6439 8400 6439 652d 8303 5a31 4700 643a  d9..d9e-..Z1G.d:
@@ -64,1759 +64,1843 @@
 000003f0: 647b 8400 647b 654d 8303 5a52 4700 647c  d{..d{eM..ZRG.d|
 00000400: 647d 8400 647d 654d 8303 5a53 4700 647e  d}..d}eM..ZSG.d~
 00000410: 647f 8400 647f 654d 8303 5a54 4700 6480  d...d.eM..ZTG.d.
 00000420: 6481 8400 6481 654d 8303 5a55 4700 6482  d...d.eM..ZUG.d.
 00000430: 6483 8400 6483 654d 8303 5a56 4700 6484  d...d.eM..ZVG.d.
 00000440: 6485 8400 6485 654d 8303 5a57 4700 6486  d...d.eM..ZWG.d.
 00000450: 6487 8400 6487 654d 8303 5a58 4700 6488  d...d.eM..ZXG.d.
-00000460: 6489 8400 6489 652e 652d 8304 5a59 6401  d...d.e.e-..ZYd.
-00000470: 5300 298d e900 0000 004e 2901 da0f 4a53  S.)......N)...JS
-00000480: 4f4e 4465 636f 6465 4572 726f 7229 01da  ONDecodeError)..
-00000490: 0873 6574 7469 6e67 7329 01da 0563 6163  .settings)...cac
-000004a0: 6865 2901 da06 6d6f 6465 6c73 2901 da12  he)...models)...
-000004b0: 446a 6175 746f 7461 736b 5365 7474 696e  DjautotaskSettin
-000004c0: 6773 2901 da05 7265 7472 7969 e803 0000  gs)...retryi....
-000004d0: 6910 2700 0069 5802 0000 da03 7572 6c5a  i.'..iX.....urlZ
-000004e0: 0677 6562 5572 6c7a 3d54 6865 206c 6f67  .webUrlz=The log
-000004f0: 6765 6420 696e 2052 6573 6f75 7263 6520  ged in Resource 
-00000500: 646f 6573 206e 6f74 2068 6176 6520 7468  does not have th
-00000510: 6520 6164 6571 7561 7465 2070 6572 6d69  e adequate permi
-00000520: 7373 696f 6e73 7a77 4e6f 206d 6573 7361  ssionszwNo messa
-00000530: 6765 2e20 4e6f 206d 6174 6368 696e 6720  ge. No matching 
-00000540: 7265 636f 7264 7320 666f 756e 642e 2054  records found. T
-00000550: 6865 206c 6f67 6765 6420 696e 2052 6573  he logged in Res
-00000560: 6f75 7263 6520 6d61 7920 6e6f 7420 6861  ource may not ha
-00000570: 7665 2074 6865 2072 6571 7569 7265 6420  ve the required 
-00000580: 7065 726d 6973 7369 6f6e 7320 746f 2064  permissions to d
-00000590: 656c 6574 6520 7468 6520 6461 7461 2e63  elete the data.c
-000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005b0: 0100 0000 4000 0000 7310 0000 0065 005a  ....@...s....e.Z
-000005c0: 0164 005a 0264 015a 0364 0253 0029 03da  .d.Z.d.Z.d.S.)..
-000005d0: 1041 7574 6f74 6173 6b41 5049 4572 726f  .AutotaskAPIErro
-000005e0: 727a 2352 6169 7365 2074 6869 732c 206e  rz#Raise this, n
-000005f0: 6f74 2072 6571 7565 7374 2065 7863 6570  ot request excep
-00000600: 7469 6f6e 732e 4ea9 04da 085f 5f6e 616d  tions.N....__nam
-00000610: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000620: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
-00000630: 5f64 6f63 5f5f a900 720f 0000 0072 0f00  _doc__..r....r..
-00000640: 0000 fa43 2f68 6f6d 652f 7275 6e6e 6572  ...C/home/runner
-00000650: 2f77 6f72 6b2f 646a 616e 676f 2d61 7574  /work/django-aut
-00000660: 6f74 6173 6b2f 646a 616e 676f 2d61 7574  otask/django-aut
-00000670: 6f74 6173 6b2f 646a 6175 746f 7461 736b  otask/djautotask
-00000680: 2f61 7069 2e70 7972 0900 0000 1f00 0000  /api.pyr........
-00000690: 7304 0000 0008 0104 0172 0900 0000 6300  s........r....c.
-000006a0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-000006b0: 0000 0040 0000 0073 1000 0000 6500 5a01  ...@...s....e.Z.
-000006c0: 6400 5a02 6401 5a03 6402 5300 2903 da16  d.Z.d.Z.d.S.)...
-000006d0: 4175 746f 7461 736b 4150 4943 6c69 656e  AutotaskAPIClien
-000006e0: 7445 7272 6f72 7a69 0a20 2020 2052 6169  tErrorzi.    Rai
-000006f0: 7365 2074 6869 7320 746f 2069 6e64 6963  se this to indic
-00000700: 6174 6520 616e 7920 6874 7470 2065 7272  ate any http err
-00000710: 6f72 2074 6861 7420 6661 6c6c 7320 7769  or that falls wi
-00000720: 7468 696e 2074 6865 0a20 2020 2034 7878  thin the.    4xx
-00000730: 2063 6c61 7373 206f 6620 6874 7470 2073   class of http s
-00000740: 7461 7475 7320 636f 6465 732e 0a20 2020  tatus codes..   
-00000750: 204e 720a 0000 0072 0f00 0000 720f 0000   Nr....r....r...
-00000760: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
-00000770: 2400 0000 7304 0000 0008 0104 0472 1100  $...s........r..
-00000780: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000790: 0000 0001 0000 0040 0000 0073 1000 0000  .......@...s....
-000007a0: 6500 5a01 6400 5a02 6401 5a03 6402 5300  e.Z.d.Z.d.Z.d.S.
-000007b0: 2903 da16 4175 746f 7461 736b 4150 4953  )...AutotaskAPIS
-000007c0: 6572 7665 7245 7272 6f72 7a53 0a20 2020  erverErrorzS.   
-000007d0: 2052 6169 7365 2074 6869 7320 746f 2069   Raise this to i
-000007e0: 6e64 6963 6174 6520 6120 5365 7276 6572  ndicate a Server
-000007f0: 2045 7272 6f72 0a20 2020 2035 3030 2063   Error.    500 c
-00000800: 6c61 7373 206f 6620 6874 7470 2073 7461  lass of http sta
-00000810: 7475 7320 636f 6465 732e 0a20 2020 204e  tus codes..    N
-00000820: 720a 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00000830: 0f00 0000 7210 0000 0072 1200 0000 2c00  ....r....r....,.
-00000840: 0000 7304 0000 0008 0104 0472 1200 0000  ..s........r....
-00000850: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000860: 0001 0000 0040 0000 0073 1000 0000 6500  .....@...s....e.
-00000870: 5a01 6400 5a02 6401 5a03 6402 5300 2903  Z.d.Z.d.Z.d.S.).
-00000880: da1b 4175 746f 7461 736b 5265 636f 7264  ..AutotaskRecord
-00000890: 4e6f 7446 6f75 6e64 4572 726f 727a 1954  NotFoundErrorz.T
-000008a0: 6865 2072 6563 6f72 6420 7761 7320 6e6f  he record was no
-000008b0: 7420 666f 756e 642e 4e72 0a00 0000 720f  t found.Nr....r.
-000008c0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-000008d0: 0000 7213 0000 0034 0000 0073 0400 0000  ..r....4...s....
-000008e0: 0801 0401 7213 0000 0063 0000 0000 0000  ....r....c......
-000008f0: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-00000900: 0000 7310 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00000910: 015a 0364 0253 0029 03da 2441 7574 6f74  .Z.d.S.)..$Autot
-00000920: 6173 6b53 6563 7572 6974 7950 6572 6d69  askSecurityPermi
-00000930: 7373 696f 6e73 4578 6365 7074 696f 6e7a  ssionsExceptionz
-00000940: 3b54 6865 2041 5049 2063 7265 6465 6e74  ;The API credent
-00000950: 6961 6c73 2068 6176 6520 696e 7375 6666  ials have insuff
-00000960: 6963 6965 6e74 2073 6563 7572 6974 7920  icient security 
-00000970: 7065 726d 6973 7369 6f6e 732e 4e72 0a00  permissions.Nr..
-00000980: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-00000990: 0072 1000 0000 7214 0000 0039 0000 0073  .r....r....9...s
-000009a0: 0400 0000 0801 0401 7214 0000 0063 0000  ........r....c..
-000009b0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-000009c0: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
-000009d0: 005a 0264 015a 0364 0253 0029 03da 2541  .Z.d.Z.d.S.)..%A
-000009e0: 7574 6f74 6173 6b49 6d70 6572 736f 6e61  utotaskImpersona
-000009f0: 7469 6f6e 4c69 6d69 7465 6445 7863 6570  tionLimitedExcep
-00000a00: 7469 6f6e 7a41 5468 6520 696d 7065 7273  tionzAThe impers
-00000a10: 6f6e 6174 696f 6e20 7265 736f 7572 6365  onation resource
-00000a20: 2068 6173 2069 6e73 7566 6669 6369 656e   has insufficien
-00000a30: 7420 7365 6375 7269 7479 2070 6572 6d69  t security permi
-00000a40: 7373 696f 6e73 2e4e 720a 0000 0072 0f00  ssions.Nr....r..
-00000a50: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00000a60: 0072 1500 0000 3e00 0000 7304 0000 0008  .r....>...s.....
-00000a70: 0304 0172 1500 0000 6301 0000 0000 0000  ...r....c.......
-00000a80: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00000a90: 0073 0c00 0000 6401 a000 7c00 6a01 a101  .s....d...|.j...
-00000aa0: 5300 2902 4e7a 022c 2029 02da 046a 6f69  S.).Nz., )...joi
-00000ab0: 6eda 0461 7267 7329 01da 0165 720f 0000  n..args)...er...
-00000ac0: 0072 0f00 0000 7210 0000 00da 1670 6172  .r....r......par
-00000ad0: 7365 5f61 7574 6f74 6173 6b61 7069 6572  se_autotaskapier
-00000ae0: 726f 7245 0000 0073 0200 0000 0001 7219  rorE...s......r.
-00000af0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000b00: 0100 0000 0200 0000 4300 0000 730c 0000  ........C...s...
-00000b10: 0074 007c 0083 0174 016b 0853 0029 017a  .t.|...t.k.S.).z
-00000b20: fc0a 2020 2020 5265 7475 726e 2054 7275  ..    Return Tru
-00000b30: 6520 6966 2077 6520 7368 6f75 6c64 2072  e if we should r
-00000b40: 6574 7279 2028 696e 2074 6869 7320 6361  etry (in this ca
-00000b50: 7365 2077 6865 6e20 6974 2773 2061 6e0a  se when it's an.
-00000b60: 2020 2020 4175 746f 7461 736b 4150 4945      AutotaskAPIE
-00000b70: 7272 6f72 292c 2046 616c 7365 206f 7468  rror), False oth
-00000b80: 6572 7769 7365 2e0a 0a20 2020 2042 6173  erwise...    Bas
-00000b90: 6963 616c 6c79 2c20 646f 6e27 7420 7265  ically, don't re
-00000ba0: 7472 7920 6f6e 2041 7574 6f74 6173 6b41  try on AutotaskA
-00000bb0: 5049 436c 6965 6e74 4572 726f 722c 2062  PIClientError, b
-00000bc0: 6563 6175 7365 2074 686f 7365 2061 7265  ecause those are
-00000bd0: 2074 6865 0a20 2020 2074 7970 6520 6f66   the.    type of
-00000be0: 2065 7863 6570 7469 6f6e 7320 7768 6572   exceptions wher
-00000bf0: 6520 7265 7472 7969 6e67 2077 6f6e 2774  e retrying won't
-00000c00: 2068 656c 7020 2834 3034 732c 2034 3033   help (404s, 403
-00000c10: 732c 2065 7463 292e 0a20 2020 2029 02da  s, etc)..    )..
-00000c20: 0474 7970 6572 0900 0000 2901 da09 6578  .typer....)...ex
-00000c30: 6365 7074 696f 6e72 0f00 0000 720f 0000  ceptionr....r...
-00000c40: 0072 1000 0000 da12 7265 7472 795f 6966  .r......retry_if
-00000c50: 5f61 7069 5f65 7272 6f72 4900 0000 7302  _api_errorI...s.
-00000c60: 0000 0000 0872 1c00 0000 6301 0000 0000  .....r....c.....
-00000c70: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00000c80: 0000 0073 1000 0000 7400 a001 6401 7c00  ...s....t...d.|.
-00000c90: 9b00 9d02 a101 5300 2902 4eda 057a 6f6e  ......S.).N..zon
-00000ca0: 655f 2902 7204 0000 00da 0367 6574 2901  e_).r......get).
-00000cb0: da09 6361 6368 655f 6b65 7972 0f00 0000  ..cache_keyr....
-00000cc0: 720f 0000 0072 1000 0000 da0e 6765 745f  r....r......get_
-00000cd0: 6361 6368 6564 5f75 726c 5400 0000 7302  cached_urlT...s.
-00000ce0: 0000 0000 0172 2000 0000 6301 0000 0000  .....r ...c.....
-00000cf0: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
-00000d00: 0000 0073 3800 0000 7400 6a01 6401 7402  ...s8...t.j.d.t.
-00000d10: 9b00 9d02 7c00 7402 1900 7403 6402 8d03  ....|.t...t.d...
-00000d20: 0100 7400 6a01 6401 7404 9b00 9d02 7c00  ..t.j.d.t.....|.
-00000d30: 7404 1900 7403 6402 8d03 0100 6400 5300  t...t.d.....d.S.
-00000d40: 2903 4e72 1d00 0000 a901 da07 7469 6d65  ).Nr........time
-00000d50: 6f75 7429 0572 0400 0000 da03 7365 74da  out).r......set.
-00000d60: 0a41 545f 5552 4c5f 4b45 59da 0d43 4143  .AT_URL_KEY..CAC
-00000d70: 4845 5f54 494d 454f 5554 da0a 4154 5f57  HE_TIMEOUT..AT_W
-00000d80: 4542 5f4b 4559 2901 da08 6a73 6f6e 5f6f  EB_KEY)...json_o
-00000d90: 626a 720f 0000 0072 0f00 0000 7210 0000  bjr....r....r...
-00000da0: 00da 0c75 7064 6174 655f 6361 6368 6558  ...update_cacheX
-00000db0: 0000 0073 1400 0000 0002 0401 0800 0600  ...s............
-00000dc0: 02ff 0602 0401 0800 0600 02ff 7228 0000  ............r(..
-00000dd0: 0046 6301 0000 0000 0000 0000 0000 0001  .Fc.............
-00000de0: 0000 0003 0000 0043 0000 0073 0a00 0000  .......C...s....
-00000df0: 7400 7401 7c00 8302 5300 a901 4e29 02da  t.t.|...S...N)..
-00000e00: 135f 6765 745f 636f 6e6e 6563 7469 6f6e  ._get_connection
-00000e10: 5f75 726c 7224 0000 00a9 01da 0b66 6f72  _urlr$.......for
-00000e20: 6365 5f66 6574 6368 720f 0000 0072 0f00  ce_fetchr....r..
-00000e30: 0000 7210 0000 00da 1667 6574 5f61 7069  ..r......get_api
-00000e40: 5f63 6f6e 6e65 6374 696f 6e5f 7572 6c60  _connection_url`
-00000e50: 0000 0073 0200 0000 0001 722d 0000 0063  ...s......r-...c
-00000e60: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000e70: 0300 0000 4300 0000 730a 0000 0074 0074  ....C...s....t.t
-00000e80: 017c 0083 0253 0072 2900 0000 2902 722a  .|...S.r)...).r*
-00000e90: 0000 0072 2600 0000 722b 0000 0072 0f00  ...r&...r+...r..
-00000ea0: 0000 720f 0000 0072 1000 0000 da16 6765  ..r....r......ge
-00000eb0: 745f 7765 625f 636f 6e6e 6563 7469 6f6e  t_web_connection
-00000ec0: 5f75 726c 6400 0000 7302 0000 0000 0172  _urld...s......r
-00000ed0: 2e00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000ee0: 0006 0000 000a 0000 0043 0000 0073 6e00  .........C...sn.
-00000ef0: 0000 7400 7c00 8301 7d02 7c02 7210 7c01  ..t.|...}.|.r.|.
-00000f00: 7266 7a22 7401 7402 6a03 6401 1900 8301  rfz"t.t.j.d.....
-00000f10: 7d03 7404 7c03 8301 0100 7c03 7c00 1900  }.t.|.....|.|...
-00000f20: 7d04 5700 716a 0400 7405 6b0a 7262 0100  }.W.qj..t.k.rb..
-00000f30: 7d05 0100 7a12 7405 6402 7c05 9b00 9d02  }...z.t.d.|.....
-00000f40: 8301 8201 5700 3500 6400 7d05 7e05 5800  ....W.5.d.}.~.X.
-00000f50: 5900 716a 5800 6e04 7c02 7d04 7c04 5300  Y.qjX.n.|.}.|.S.
-00000f60: 2903 4eda 0875 7365 726e 616d 657a 1946  ).N..usernamez.F
-00000f70: 6169 6c65 6420 746f 2067 6574 207a 6f6e  ailed to get zon
-00000f80: 6520 696e 666f 3a20 2906 7220 0000 00da  e info: ).r ....
-00000f90: 0d67 6574 5f7a 6f6e 655f 696e 666f 7203  .get_zone_infor.
-00000fa0: 0000 00da 1441 5554 4f54 4153 4b5f 4352  .....AUTOTASK_CR
-00000fb0: 4544 454e 5449 414c 5372 2800 0000 7209  EDENTIALSr(...r.
-00000fc0: 0000 0029 06da 0566 6965 6c64 722c 0000  ...)...fieldr,..
-00000fd0: 005a 1261 7069 5f75 726c 5f66 726f 6d5f  .Z.api_url_from_
-00000fe0: 6361 6368 6572 2700 0000 7208 0000 0072  cacher'...r....r
-00000ff0: 1800 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-00001000: 0000 0072 2a00 0000 6800 0000 7314 0000  ...r*...h...s...
-00001010: 0000 0108 0208 0102 010e 0208 020c 0110  ................
-00001020: 0122 0204 0272 2a00 0000 6301 0000 0000  ."...r*...c.....
-00001030: 0000 0000 0000 0005 0000 000a 0000 0043  ...............C
-00001040: 0000 0073 b600 0000 7400 6a01 6401 1700  ...s....t.j.d...
-00001050: 7c00 1700 7d01 7a6e 7402 a003 6402 a004  |...}.znt...d...
-00001060: 7c01 a101 a101 0100 7405 6a06 7c01 6403  |.......t.j.|.d.
-00001070: 6404 8d02 7d02 6405 7c02 6a07 6b02 7246  d...}.d.|.j.k.rF
-00001080: 7c02 a008 a100 7d03 7c03 5700 5300 6406  |.....}.|.W.S.d.
-00001090: 7c02 6a07 6b02 7270 7c02 a008 a100 7d03  |.j.k.rp|.....}.
-000010a0: 7409 6407 a004 7c01 7408 a00a 7c03 a101  t.d...|.t...|...
-000010b0: a102 8301 8201 6e0a 7409 7c02 6a0b 8301  ......n.t.|.j...
-000010c0: 8201 5700 6e34 0400 7405 6a0c 6b0a 72b0  ..W.n4..t.j.k.r.
-000010d0: 0100 7d04 0100 7a14 7409 6407 a004 7c01  ..}...z.t.d...|.
-000010e0: 7c04 a102 8301 8201 5700 3500 6400 7d04  |.......W.5.d.}.
-000010f0: 7e04 5800 5900 6e02 5800 6400 5300 2908  ~.X.Y.n.X.d.S.).
-00001100: 4e7a 1a76 312e 302f 7a6f 6e65 496e 666f  Nz.v1.0/zoneInfo
-00001110: 726d 6174 696f 6e3f 7573 6572 3d7a 184d  rmation?user=z.M
-00001120: 616b 696e 6720 4745 5420 7265 7175 6573  aking GET reques
-00001130: 7420 746f 207b 7de9 0300 0000 7221 0000  t to {}.....r!..
-00001140: 00e9 c800 0000 e9f4 0100 007a 1a52 6571  ...........z.Req
-00001150: 7565 7374 2066 6169 6c65 643a 2047 4554  uest failed: GET
-00001160: 207b 7d3a 207b 7d29 0d72 0300 0000 da13   {}: {}).r......
-00001170: 4155 544f 5441 534b 5f53 4552 5645 525f  AUTOTASK_SERVER_
-00001180: 5552 4cda 066c 6f67 6765 72da 0564 6562  URL..logger..deb
-00001190: 7567 da06 666f 726d 6174 da08 7265 7175  ug..format..requ
-000011a0: 6573 7473 721e 0000 00da 0b73 7461 7475  estsr......statu
-000011b0: 735f 636f 6465 da04 6a73 6f6e 7209 0000  s_code..jsonr...
-000011c0: 00da 0564 756d 7073 da07 636f 6e74 656e  ...dumps..conten
-000011d0: 74da 1052 6571 7565 7374 4578 6365 7074  t..RequestExcept
-000011e0: 696f 6e29 0572 2f00 0000 da0c 656e 6470  ion).r/.....endp
-000011f0: 6f69 6e74 5f75 726c da08 7265 7370 6f6e  oint_url..respon
-00001200: 7365 5a09 7265 7370 5f6a 736f 6e72 1800  seZ.resp_jsonr..
-00001210: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00001220: 0072 3000 0000 7a00 0000 7332 0000 0000  .r0...z...s2....
-00001230: 0108 0102 ff04 0302 0110 010e 010a 0108  ................
-00001240: 0106 010a 0208 0102 0104 0102 0008 ff02  ................
-00001250: ff06 060e 0112 0102 0104 0102 0002 ff02  ................
-00001260: ff72 3000 0000 6300 0000 0000 0000 0000  .r0...c.........
-00001270: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
-00001280: 2e00 0000 6500 5a01 6400 5a02 6401 6401  ....e.Z.d.Z.d.d.
-00001290: 6401 6402 9c03 6403 6404 8402 5a03 6405  d.d...d.d...Z.d.
-000012a0: 6406 8400 5a04 6407 6408 8400 5a05 6401  d...Z.d.d...Z.d.
-000012b0: 5300 2909 da0c 4170 6943 6f6e 6469 7469  S.)...ApiConditi
-000012c0: 6f6e 4e29 03da 026f 7072 3200 0000 da05  onN)...opr2.....
-000012d0: 7661 6c75 6563 0100 0000 0000 0000 0300  valuec..........
-000012e0: 0000 0600 0000 0500 0000 4700 0000 735a  ..........G...sZ
-000012f0: 0000 0067 007c 005f 007c 017c 005f 017c  ...g.|._.|.|._.|
-00001300: 027c 005f 027c 037c 005f 037c 0164 016b  .|._.|.|._.|.d.k
-00001310: 0672 567c 0444 005d 307d 0574 047c 0583  .rV|.D.]0}.t.|..
-00001320: 017c 006a 056b 0372 4874 0664 02a0 077c  .|.j.k.rHt.d...|
-00001330: 006a 056a 08a1 0183 0182 017c 006a 00a0  .j.j.......|.j..
-00001340: 097c 05a1 0101 0071 2464 0053 0029 034e  .|.....q$d.S.).N
-00001350: 2902 da03 616e 64da 026f 727a 2f47 726f  )...and..orz/Gro
-00001360: 7570 6564 2063 6f6e 6469 7469 6f6e 7320  uped conditions 
-00001370: 6d75 7374 2061 6c73 6f20 6265 2069 6e73  must also be ins
-00001380: 7461 6e63 6573 206f 6620 7b7d 290a da06  tances of {})...
-00001390: 5f69 7465 6d73 7243 0000 0072 3200 0000  _itemsrC...r2...
-000013a0: 7244 0000 0072 1a00 0000 da09 5f5f 636c  rD...r......__cl
-000013b0: 6173 735f 5fda 0954 7970 6545 7272 6f72  ass__..TypeError
-000013c0: 7239 0000 0072 0b00 0000 da06 6170 7065  r9...r......appe
-000013d0: 6e64 2906 da04 7365 6c66 7243 0000 0072  nd)...selfrC...r
-000013e0: 3200 0000 7244 0000 0072 1700 0000 da09  2...rD...r......
-000013f0: 636f 6e64 6974 696f 6e72 0f00 0000 720f  conditionr....r.
-00001400: 0000 0072 1000 0000 da08 5f5f 696e 6974  ...r......__init
-00001410: 5f5f 9800 0000 731a 0000 0000 0106 0106  __....s.........
-00001420: 0106 0106 0208 0208 010e 0102 0104 0106  ................
-00001430: ff02 ff04 047a 1541 7069 436f 6e64 6974  .....z.ApiCondit
-00001440: 696f 6e2e 5f5f 696e 6974 5f5f 6301 0000  ion.__init__c...
-00001450: 0000 0000 0000 0000 0001 0000 0005 0000  ................
-00001460: 0043 0000 0073 2800 0000 7400 7c00 6a01  .C...s(...t.|.j.
-00001470: 8301 7214 7c00 6a01 a002 a100 5300 6401  ..r.|.j.....S.d.
-00001480: a003 7c00 6a04 7c00 6a05 7c00 6a06 a103  ..|.j.|.j.|.j...
-00001490: 5300 2902 4e7a 207b 7b6f 703a 207b 7d2c  S.).Nz {{op: {},
-000014a0: 2066 6965 6c64 3a20 7b7d 2c20 7661 6c75   field: {}, valu
-000014b0: 653a 207b 7d7d 7d29 07da 036c 656e 7247  e: {}}})...lenrG
-000014c0: 0000 00da 085f 5f72 6570 725f 5f72 3900  .....__repr__r9.
-000014d0: 0000 7243 0000 0072 3200 0000 7244 0000  ..rC...r2...rD..
-000014e0: 00a9 0172 4b00 0000 720f 0000 0072 0f00  ...rK...r....r..
-000014f0: 0000 7210 0000 0072 4f00 0000 a800 0000  ..r....rO.......
-00001500: 730e 0000 0000 010a 010a 0104 0104 0104  s...............
-00001510: 0104 fd7a 1541 7069 436f 6e64 6974 696f  ...z.ApiConditio
-00001520: 6e2e 5f5f 7265 7072 5f5f 6301 0000 0000  n.__repr__c.....
-00001530: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00001540: 0000 0073 4600 0000 7400 7c00 6a01 8301  ...sF...t.|.j...
-00001550: 7224 7c00 6a02 6401 6402 8400 7c00 6a01  r$|.j.d.d...|.j.
-00001560: 4400 8301 6403 9c02 7d01 6e1e 7c00 6a02  D...d...}.n.|.j.
-00001570: 7c00 6a03 6404 9c02 7d01 7c00 6a04 7242  |.j.d...}.|.j.rB
-00001580: 7c00 6a04 7c01 6405 3c00 7c01 5300 2906  |.j.|.d.<.|.S.).
-00001590: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
-000015a0: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
-000015b0: 007c 005d 0c7d 017c 01a0 00a1 0091 0271  .|.].}.|.......q
-000015c0: 0453 0072 0f00 0000 2901 da10 666f 726d  .S.r....)...form
-000015d0: 6174 5f63 6f6e 6469 7469 6f6e 2902 da02  at_condition)...
-000015e0: 2e30 5a0d 6170 695f 636f 6e64 6974 696f  .0Z.api_conditio
-000015f0: 6e72 0f00 0000 720f 0000 0072 1000 0000  nr....r....r....
-00001600: da0a 3c6c 6973 7463 6f6d 703e b600 0000  ..<listcomp>....
-00001610: 7304 0000 0006 0202 ff7a 3141 7069 436f  s........z1ApiCo
-00001620: 6e64 6974 696f 6e2e 666f 726d 6174 5f63  ndition.format_c
-00001630: 6f6e 6469 7469 6f6e 2e3c 6c6f 6361 6c73  ondition.<locals
-00001640: 3e2e 3c6c 6973 7463 6f6d 703e 2902 7243  >.<listcomp>).rC
-00001650: 0000 00da 0569 7465 6d73 2902 7243 0000  .....items).rC..
-00001660: 0072 3200 0000 7244 0000 0029 0572 4e00  .r2...rD...).rN.
-00001670: 0000 7247 0000 0072 4300 0000 7232 0000  ..rG...rC...r2..
-00001680: 0072 4400 0000 a902 724b 0000 0072 4c00  .rD.....rK...rL.
-00001690: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-000016a0: 0072 5100 0000 b100 0000 7318 0000 0000  .rQ.......s.....
-000016b0: 010a 0304 0106 0204 fe04 fe08 0904 0104  ................
-000016c0: fe06 0406 020a 027a 1d41 7069 436f 6e64  .......z.ApiCond
-000016d0: 6974 696f 6e2e 666f 726d 6174 5f63 6f6e  ition.format_con
-000016e0: 6469 7469 6f6e 2906 720b 0000 0072 0c00  dition).r....r..
-000016f0: 0000 720d 0000 0072 4d00 0000 724f 0000  ..r....rM...rO..
-00001700: 0072 5100 0000 720f 0000 0072 0f00 0000  .rQ...r....r....
-00001710: 720f 0000 0072 1000 0000 7242 0000 0096  r....r....rB....
-00001720: 0000 0073 0600 0000 0802 1210 0809 7242  ...s..........rB
-00001730: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00001740: 0000 0000 0300 0000 4000 0000 7360 0000  ........@...s`..
-00001750: 0065 005a 0164 005a 0264 0164 0264 039c  .e.Z.d.Z.d.d.d..
-00001760: 025a 0364 0464 0584 005a 0464 0664 0784  .Z.d.d...Z.d.d..
-00001770: 005a 0564 0864 0984 005a 0664 0a64 0b84  .Z.d.d...Z.d.d..
-00001780: 005a 0764 0c64 0d84 005a 0864 0e64 0f84  .Z.d.d...Z.d.d..
-00001790: 005a 0964 1064 1184 005a 0a64 1864 1364  .Z.d.d...Z.d.d.d
-000017a0: 1484 015a 0b64 1564 1684 005a 0c64 1753  ...Z.d.d...Z.d.S
-000017b0: 0029 19da 1041 7069 436f 6e64 6974 696f  .)...ApiConditio
-000017c0: 6e4c 6973 747a 0d71 7565 7279 3f73 6561  nListz.query?sea
-000017d0: 7263 683d da05 7175 6572 7929 0272 1e00  rch=..query).r..
-000017e0: 0000 da04 706f 7374 6301 0000 0000 0000  ....postc.......
-000017f0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00001800: 0073 0c00 0000 7400 8300 7c00 5f01 6400  .s....t...|._.d.
-00001810: 5300 7229 0000 0029 02da 046c 6973 74da  S.r)...)...list.
-00001820: 055f 6c69 7374 7250 0000 0072 0f00 0000  ._listrP...r....
-00001830: 720f 0000 0072 1000 0000 724d 0000 00cd  r....r....rM....
-00001840: 0000 0073 0200 0000 0001 7a19 4170 6943  ...s......z.ApiC
-00001850: 6f6e 6469 7469 6f6e 4c69 7374 2e5f 5f69  onditionList.__i
-00001860: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-00001870: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
-00001880: 0000 007c 006a 00a0 01a1 0053 0072 2900  ...|.j.....S.r).
-00001890: 0000 2902 725a 0000 0072 4f00 0000 7250  ..).rZ...rO...rP
-000018a0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-000018b0: 0000 724f 0000 00d0 0000 0073 0200 0000  ..rO.......s....
-000018c0: 0001 7a19 4170 6943 6f6e 6469 7469 6f6e  ..z.ApiCondition
-000018d0: 4c69 7374 2e5f 5f72 6570 725f 5f63 0100  List.__repr__c..
-000018e0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000018f0: 0000 4300 0000 730a 0000 0074 007c 006a  ..C...s....t.|.j
-00001900: 0183 0153 0072 2900 0000 2902 724e 0000  ...S.r)...).rN..
-00001910: 0072 5a00 0000 7250 0000 0072 0f00 0000  .rZ...rP...r....
-00001920: 720f 0000 0072 1000 0000 da07 5f5f 6c65  r....r......__le
-00001930: 6e5f 5fd3 0000 0073 0200 0000 0001 7a18  n__....s......z.
-00001940: 4170 6943 6f6e 6469 7469 6f6e 4c69 7374  ApiConditionList
-00001950: 2e5f 5f6c 656e 5f5f 6302 0000 0000 0000  .__len__c.......
-00001960: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-00001970: 0073 0a00 0000 7c00 6a00 7c01 1900 5300  .s....|.j.|...S.
-00001980: 7229 0000 00a9 0172 5a00 0000 a902 724b  r).....rZ.....rK
-00001990: 0000 00da 0169 720f 0000 0072 0f00 0000  .....ir....r....
-000019a0: 7210 0000 00da 0b5f 5f67 6574 6974 656d  r......__getitem
-000019b0: 5f5f d600 0000 7302 0000 0000 017a 1c41  __....s......z.A
-000019c0: 7069 436f 6e64 6974 696f 6e4c 6973 742e  piConditionList.
-000019d0: 5f5f 6765 7469 7465 6d5f 5f63 0300 0000  __getitem__c....
-000019e0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-000019f0: 4300 0000 7322 0000 0074 007c 0283 0174  C...s"...t.|...t
-00001a00: 016b 0972 1474 0264 0183 0182 017c 027c  .k.r.t.d.....|.|
-00001a10: 006a 037c 013c 0064 0053 00a9 024e 7a2d  .j.|.<.d.S...Nz-
-00001a20: 436f 6e64 6974 696f 6e73 206d 7573 7420  Conditions must 
-00001a30: 6265 2069 6e73 7461 6e63 6573 206f 6620  be instances of 
-00001a40: 4170 6943 6f6e 6469 7469 6f6e 2e29 0472  ApiCondition.).r
-00001a50: 1a00 0000 7242 0000 0072 4900 0000 725a  ....rB...rI...rZ
-00001a60: 0000 0029 0372 4b00 0000 725e 0000 0072  ...).rK...r^...r
-00001a70: 4400 0000 720f 0000 0072 0f00 0000 7210  D...r....r....r.
-00001a80: 0000 00da 0b5f 5f73 6574 6974 656d 5f5f  .....__setitem__
-00001a90: d900 0000 7306 0000 0000 010c 0108 017a  ....s..........z
-00001aa0: 1c41 7069 436f 6e64 6974 696f 6e4c 6973  .ApiConditionLis
-00001ab0: 742e 5f5f 7365 7469 7465 6d5f 5f63 0200  t.__setitem__c..
-00001ac0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00001ad0: 0000 4300 0000 730c 0000 007c 006a 007c  ..C...s....|.j.|
-00001ae0: 013d 0064 0053 0072 2900 0000 725c 0000  .=.d.S.r)...r\..
-00001af0: 0072 5d00 0000 720f 0000 0072 0f00 0000  .r]...r....r....
-00001b00: 7210 0000 00da 0b5f 5f64 656c 6974 656d  r......__delitem
-00001b10: 5f5f de00 0000 7302 0000 0000 017a 1c41  __....s......z.A
-00001b20: 7069 436f 6e64 6974 696f 6e4c 6973 742e  piConditionList.
-00001b30: 5f5f 6465 6c69 7465 6d5f 5f63 0100 0000  __delitem__c....
-00001b40: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00001b50: 4300 0000 730a 0000 007c 006a 00a0 01a1  C...s....|.j....
-00001b60: 0053 0072 2900 0000 2902 725a 0000 00da  .S.r)...).rZ....
-00001b70: 085f 5f69 7465 725f 5f72 5000 0000 720f  .__iter__rP...r.
-00001b80: 0000 0072 0f00 0000 7210 0000 0072 6300  ...r....r....rc.
-00001b90: 0000 e100 0000 7302 0000 0000 017a 1941  ......s......z.A
-00001ba0: 7069 436f 6e64 6974 696f 6e4c 6973 742e  piConditionList.
-00001bb0: 5f5f 6974 6572 5f5f 721e 0000 0063 0200  __iter__r....c..
-00001bc0: 0000 0000 0000 0000 0000 0600 0000 0500  ................
-00001bd0: 0000 4300 0000 7364 0000 0067 007d 027c  ..C...sd...g.}.|
-00001be0: 006a 0044 005d 127d 037c 02a0 017c 03a0  .j.D.].}.|...|..
-00001bf0: 02a1 00a1 0101 0071 0a7c 006a 037c 0119  .......q.|.j.|..
-00001c00: 007d 0474 04a0 0564 017c 0269 01a1 017d  .}.t...d.|.i...}
-00001c10: 057c 0164 026b 0272 4c7c 047c 0537 007d  .|.d.k.rL|.|.7.}
-00001c20: 0464 007d 056e 107c 0164 036b 0372 5c74  .d.}.n.|.d.k.r\t
-00001c30: 0664 0483 0182 017c 047c 0566 0253 0029  .d.....|.|.f.S.)
-00001c40: 054e da06 6669 6c74 6572 721e 0000 0072  .N..filterr....r
-00001c50: 5800 0000 7a12 556e 7375 7070 6f72 7465  X...z.Unsupporte
-00001c60: 6420 6d65 7468 6f64 2907 725a 0000 0072  d method).rZ...r
-00001c70: 4a00 0000 7251 0000 00da 074d 4554 484f  J...rQ.....METHO
-00001c80: 4453 723c 0000 0072 3d00 0000 7249 0000  DSr<...r=...rI..
-00001c90: 0029 0672 4b00 0000 da06 6d65 7468 6f64  .).rK.....method
-00001ca0: da07 7175 6572 6965 7372 4c00 0000 da08  ..queriesrL.....
-00001cb0: 656e 6470 6f69 6e74 da07 6669 6c74 6572  endpoint..filter
-00001cc0: 7372 0f00 0000 720f 0000 0072 1000 0000  sr....r....r....
-00001cd0: da0b 6275 696c 645f 7175 6572 79e4 0000  ..build_query...
-00001ce0: 0073 1600 0000 0001 0401 0a01 1002 0a01  .s..............
-00001cf0: 0e02 0801 0801 0601 0801 0801 7a1c 4170  ............z.Ap
-00001d00: 6943 6f6e 6469 7469 6f6e 4c69 7374 2e62  iConditionList.b
-00001d10: 7569 6c64 5f71 7565 7279 6302 0000 0000  uild_queryc.....
-00001d20: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00001d30: 0000 0073 2400 0000 7400 7c01 8301 7401  ...s$...t.|...t.
-00001d40: 6b09 7214 7402 6401 8301 8201 7c00 6a03  k.r.t.d.....|.j.
-00001d50: a004 7c01 a101 0100 6400 5300 7260 0000  ..|.....d.S.r`..
-00001d60: 0029 0572 1a00 0000 7242 0000 0072 4900  .).r....rB...rI.
-00001d70: 0000 725a 0000 0072 4a00 0000 7255 0000  ..rZ...rJ...rU..
-00001d80: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00001d90: da03 6164 64f3 0000 0073 0600 0000 0001  ..add....s......
-00001da0: 0c01 0802 7a14 4170 6943 6f6e 6469 7469  ....z.ApiConditi
-00001db0: 6f6e 4c69 7374 2e61 6464 4e29 0172 1e00  onList.addN).r..
-00001dc0: 0000 290d 720b 0000 0072 0c00 0000 720d  ..).r....r....r.
-00001dd0: 0000 0072 6500 0000 724d 0000 0072 4f00  ...re...rM...rO.
-00001de0: 0000 725b 0000 0072 5f00 0000 7261 0000  ..r[...r_...ra..
-00001df0: 0072 6200 0000 7263 0000 0072 6a00 0000  .rb...rc...rj...
-00001e00: 726b 0000 0072 0f00 0000 720f 0000 0072  rk...r....r....r
-00001e10: 0f00 0000 7210 0000 0072 5600 0000 c700  ....r....rV.....
-00001e20: 0000 7318 0000 0008 0202 0102 fe06 0508  ..s.............
-00001e30: 0308 0308 0308 0308 0508 0308 030a 0f72  ...............r
-00001e40: 5600 0000 6300 0000 0000 0000 0000 0000  V...c...........
-00001e50: 0000 0000 0006 0000 0040 0000 0073 da00  .........@...s..
-00001e60: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00001e70: 5a04 6432 6403 6404 8401 5a05 6506 6405  Z.d2d.d...Z.e.d.
-00001e80: 6406 8400 8301 5a07 6433 6407 6408 8401  d.....Z.d3d.d...
-00001e90: 5a08 6409 640a 8400 5a09 640b 640c 8400  Z.d.d...Z.d.d...
-00001ea0: 5a0a 640d 640e 8400 5a0b 640f 6410 8400  Z.d.d...Z.d.d...
-00001eb0: 5a0c 6411 6412 8400 5a0d 6413 6414 8400  Z.d.d...Z.d.d...
-00001ec0: 5a0e 6415 6416 8400 5a0f 6434 6418 6419  Z.d.d...Z.d4d.d.
-00001ed0: 8401 5a10 641a 641b 8400 5a11 641c 641d  ..Z.d.d...Z.d.d.
-00001ee0: 8400 5a12 6435 641e 641f 8401 5a13 6420  ..Z.d5d.d...Z.d 
-00001ef0: 6421 8400 5a14 6422 6423 8400 5a15 6424  d!..Z.d"d#..Z.d$
-00001f00: 6425 8400 5a16 6426 6427 8400 5a17 6428  d%..Z.d&d'..Z.d(
-00001f10: 6429 8400 5a18 642a 642b 8400 5a19 642c  d)..Z.d*d+..Z.d,
-00001f20: 642d 8400 5a1a 642e 642f 8400 5a1b 6436  d-..Z.d.d/..Z.d6
-00001f30: 6430 6431 8401 5a1c 6401 5300 2937 da11  d0d1..Z.d.S.)7..
-00001f40: 4175 746f 7461 736b 4150 4943 6c69 656e  AutotaskAPIClien
-00001f50: 744e e901 0000 0063 0700 0000 0000 0000  tN.....c........
-00001f60: 0000 0000 0700 0000 0200 0000 4300 0000  ............C...
-00001f70: 739e 0000 007c 0173 0e74 006a 0164 0119  s....|.s.t.j.d..
-00001f80: 007d 017c 0273 1c74 006a 0164 0219 007d  .}.|.s.t.j.d...}
-00001f90: 027c 0373 2a74 006a 0164 0319 007d 037c  .|.s*t.j.d...}.|
-00001fa0: 0473 3874 006a 0164 0419 007d 047c 0573  .s8t.j.d...}.|.s
-00001fb0: 4274 0283 007d 057c 006a 0373 5074 0464  Bt...}.|.j.sPt.d
-00001fc0: 0583 0182 017c 017c 005f 057c 027c 005f  .....|.|._.|.|._
-00001fd0: 067c 037c 005f 077c 047c 005f 087c 057c  .|.|._.|.|._.|.|
-00001fe0: 005f 0974 0a83 00a0 0ba1 007c 005f 0c7c  ._.t.......|._.|
-00001ff0: 006a 0c64 0619 007c 005f 0d7c 067c 005f  .j.d...|._.|.|._
-00002000: 0e74 0f83 007c 005f 1064 007c 005f 1164  .t...|._.d.|._.d
-00002010: 0053 0029 074e 722f 0000 00da 0870 6173  .S.).Nr/.....pas
-00002020: 7377 6f72 64da 1069 6e74 6567 7261 7469  sword..integrati
-00002030: 6f6e 5f63 6f64 65da 1072 6573 745f 6170  on_code..rest_ap
-00002040: 695f 7665 7273 696f 6e7a 1141 5049 206e  i_versionz.API n
-00002050: 6f74 2073 7065 6369 6669 6564 7222 0000  ot specifiedr"..
-00002060: 0029 1272 0300 0000 7231 0000 0072 2d00  .).r....r1...r-.
-00002070: 0000 da03 4150 49da 0a56 616c 7565 4572  ....API..ValueEr
-00002080: 726f 7272 2f00 0000 726e 0000 0072 6f00  rorr/...rn...ro.
-00002090: 0000 7270 0000 00da 0a73 6572 7665 725f  ..rp.....server_
-000020a0: 7572 6c72 0600 0000 5a0c 6765 745f 7365  urlr....Z.get_se
-000020b0: 7474 696e 6773 da10 7265 7175 6573 745f  ttings..request_
-000020c0: 7365 7474 696e 6773 7222 0000 00da 1669  settingsr".....i
-000020d0: 6d70 6572 736f 6e61 7469 6f6e 5f72 6573  mpersonation_res
-000020e0: 6f75 7263 6572 5600 0000 da0a 636f 6e64  ourcerV.....cond
-000020f0: 6974 696f 6e73 da0b 6361 6368 6564 5f62  itions..cached_b
-00002100: 6f64 7929 0772 4b00 0000 722f 0000 0072  ody).rK...r/...r
-00002110: 6e00 0000 726f 0000 0072 7000 0000 7273  n...ro...rp...rs
-00002120: 0000 0072 7500 0000 720f 0000 0072 0f00  ...ru...r....r..
-00002130: 0000 7210 0000 0072 4d00 0000 fe00 0000  ..r....rM.......
-00002140: 7334 0000 0000 0904 010a 0104 010a 0104  s4..............
-00002150: 0104 0102 ff04 0304 0104 0102 ff04 0204  ................
-00002160: 0106 0206 0108 0206 0106 0106 0106 0106  ................
-00002170: 020c 010c 0106 0108 027a 1a41 7574 6f74  .........z.Autot
-00002180: 6173 6b41 5049 436c 6965 6e74 2e5f 5f69  askAPIClient.__i
-00002190: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-000021a0: 0000 0100 0000 0500 0000 4300 0000 7314  ..........C...s.
-000021b0: 0000 0064 01a0 007c 006a 0174 026a 0364  ...d...|.j.t.j.d
-000021c0: 0219 00a1 0253 0029 034e 7a08 7b30 7d76  .....S.).Nz.{0}v
-000021d0: 7b31 7d2f 7270 0000 0029 0472 3900 0000  {1}/rp...).r9...
-000021e0: 7273 0000 0072 0300 0000 7231 0000 0072  rs...r....r1...r
-000021f0: 5000 0000 720f 0000 0072 0f00 0000 7210  P...r....r....r.
-00002200: 0000 00da 0c61 7069 5f62 6173 655f 7572  .....api_base_ur
-00002210: 6c25 0100 0073 0800 0000 0002 0401 0401  l%...s..........
-00002220: 08fe 7a1e 4175 746f 7461 736b 4150 4943  ..z.AutotaskAPIC
-00002230: 6c69 656e 742e 6170 695f 6261 7365 5f75  lient.api_base_u
-00002240: 726c 6302 0000 0000 0000 0000 0000 0002  rlc.............
-00002250: 0000 0004 0000 0043 0000 0073 1800 0000  .......C...s....
-00002260: 7c01 730a 7c00 6a00 7d01 6401 a001 7c00  |.s.|.j.}.d...|.
-00002270: 6a02 7c01 a102 5300 2902 4e7a 077b 307d  j.|...S.).Nz.{0}
-00002280: 7b31 7d2f 2903 7271 0000 0072 3900 0000  {1}/).rq...r9...
-00002290: 7278 0000 00a9 0272 4b00 0000 7268 0000  rx.....rK...rh..
-000022a0: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
-000022b0: da0b 6765 745f 6170 695f 7572 6c2c 0100  ..get_api_url,..
-000022c0: 0073 0c00 0000 0001 0401 0602 0401 0401  .s..............
-000022d0: 02fe 7a1d 4175 746f 7461 736b 4150 4943  ..z.AutotaskAPIC
-000022e0: 6c69 656e 742e 6765 745f 6170 695f 7572  lient.get_api_ur
-000022f0: 6c63 0200 0000 0000 0000 0000 0000 0200  lc..............
-00002300: 0000 0700 0000 4300 0000 731e 0000 0074  ......C...s....t
-00002310: 00a0 0164 01a0 027c 016a 037c 016a 047c  ...d...|.j.|.j.|
-00002320: 016a 05a1 03a1 0101 0064 0053 0029 024e  .j.......d.S.).N
-00002330: 7a20 4661 696c 6564 2041 5049 2063 616c  z Failed API cal
-00002340: 6c3a 207b 307d 202d 207b 317d 202d 207b  l: {0} - {1} - {
-00002350: 327d 2906 7237 0000 00da 0565 7272 6f72  2}).r7.....error
-00002360: 7239 0000 0072 0800 0000 723b 0000 0072  r9...r....r;...r
-00002370: 3e00 0000 2902 724b 0000 0072 4100 0000  >...).rK...rA...
-00002380: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
-00002390: 0b5f 6c6f 675f 6661 696c 6564 3501 0000  ._log_failed5...
-000023a0: 730a 0000 0000 0108 0104 0004 0004 ff7a  s..............z
-000023b0: 1d41 7574 6f74 6173 6b41 5049 436c 6965  .AutotaskAPIClie
-000023c0: 6e74 2e5f 6c6f 675f 6661 696c 6564 6302  nt._log_failedc.
-000023d0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-000023e0: 0000 0043 0000 0073 1400 0000 6401 7d02  ...C...s....d.}.
-000023f0: 6402 a000 7c01 7c02 a102 7d01 7c01 5300  d...|.|...}.|.S.
-00002400: 2903 4e7a 8352 6573 6f75 7263 6520 696d  ).Nz.Resource im
-00002410: 7065 7273 6f6e 6174 696f 6e20 6973 2065  personation is e
-00002420: 6e61 626c 6564 2069 6e20 796f 7572 2054  nabled in your T
-00002430: 6f70 4c65 6674 2061 7070 6c69 6361 7469  opLeft applicati
-00002440: 6f6e 2e20 506c 6561 7365 2063 6865 636b  on. Please check
-00002450: 2074 6865 2072 6573 6f75 7263 6520 7365   the resource se
-00002460: 6375 7269 7479 206c 6576 656c 2074 6861  curity level tha
-00002470: 7420 6973 2062 6569 6e67 2069 6d70 6572  t is being imper
-00002480: 736f 6e61 7465 642e fa05 7b7d 207b 7d29  sonated...{} {})
-00002490: 0172 3900 0000 2903 724b 0000 00da 036d  .r9...).rK.....m
-000024a0: 7367 5a17 696d 7065 7273 6f6e 6174 696f  sgZ.impersonatio
-000024b0: 6e5f 6572 726f 725f 6d73 6772 0f00 0000  n_error_msgr....
-000024c0: 720f 0000 0072 1000 0000 da20 5f70 7265  r....r..... _pre
-000024d0: 7061 7265 5f65 7272 6f72 5f66 6f72 5f69  pare_error_for_i
-000024e0: 6d70 6572 736f 6e61 7469 6f6e 3901 0000  mpersonation9...
-000024f0: 7308 0000 0000 0202 ff02 040c 017a 3241  s............z2A
-00002500: 7574 6f74 6173 6b41 5049 436c 6965 6e74  utotaskAPIClient
-00002510: 2e5f 7072 6570 6172 655f 6572 726f 725f  ._prepare_error_
-00002520: 666f 725f 696d 7065 7273 6f6e 6174 696f  for_impersonatio
-00002530: 6e63 0200 0000 0000 0000 0000 0000 0800  nc..............
-00002540: 0000 0800 0000 4300 0000 73e4 0000 007c  ......C...s....|
-00002550: 016a 00a0 0164 01a1 017d 027c 02a0 0264  .j...d...}.|...d
-00002560: 0264 03a1 027d 0267 007d 037a 7c74 03a0  .d...}.g.}.z|t..
-00002570: 047c 02a1 017d 027c 02a0 0564 04a1 0172  .|...}.|...d...r
-00002580: 427c 02a0 0564 04a1 01a0 0664 05a1 016e  B|...d.....d...n
-00002590: 0264 067d 0464 07a0 077c 04a1 017d 057c  .d.}.d...|...}.|
-000025a0: 02a0 0564 08a1 0172 807c 02a0 0564 08a1  ...d...r.|...d..
-000025b0: 0144 005d 1a7d 067c 03a0 0864 07a0 077c  .D.].}.|...d...|
-000025c0: 06a0 0664 05a1 01a1 01a1 0101 0071 6464  ...d.........qdd
-000025d0: 09a0 097c 03a1 017d 0364 0aa0 077c 057c  ...|...}.d...|.|
-000025e0: 03a1 027d 0757 006e 4604 0074 036a 0a6a  ...}.W.nF..t.j.j
-000025f0: 0b6b 0a72 be01 0001 0001 0064 0ba0 077c  .k.r.......d...|
-00002600: 016a 0c7c 02a1 027d 0759 006e 2204 0074  .j.|...}.Y.n"..t
-00002610: 0d6b 0a72 de01 0001 0001 0064 0ba0 077c  .k.r.......d...|
-00002620: 016a 0c7c 02a1 027d 0759 006e 0258 007c  .j.|...}.Y.n.X.|
-00002630: 0753 0029 0c4e 7a05 7574 662d 387a 020d  .S.).Nz.utf-8z..
-00002640: 0ada 00da 076d 6573 7361 6765 da01 2e7a  .....message...z
-00002650: 0a4e 6f20 6d65 7373 6167 657a 037b 7d2e  .No messagez.{}.
-00002660: da06 6572 726f 7273 7a10 2054 6865 2065  ..errorsz. The e
-00002670: 7272 6f72 2077 6173 3a20 727d 0000 007a  rror was: r}...z
-00002680: 1841 6e20 6572 726f 7220 6f63 6375 7272  .An error occurr
-00002690: 6564 3a20 7b7d 207b 7d29 0e72 3e00 0000  ed: {} {}).r>...
-000026a0: da06 6465 636f 6465 da07 7265 706c 6163  ..decode..replac
-000026b0: 6572 3c00 0000 da05 6c6f 6164 7372 1e00  er<.....loadsr..
-000026c0: 0000 da06 7273 7472 6970 7239 0000 0072  ....rstripr9...r
-000026d0: 4a00 0000 7216 0000 00da 0764 6563 6f64  J...r......decod
-000026e0: 6572 7202 0000 0072 3b00 0000 da08 4b65  err....r;.....Ke
-000026f0: 7945 7272 6f72 2908 724b 0000 0072 4100  yError).rK...rA.
-00002700: 0000 727b 0000 00da 086d 6573 7361 6765  ..r{.....message
-00002710: 735a 1073 7472 6970 7065 645f 6d65 7373  sZ.stripped_mess
-00002720: 6167 655a 1170 7269 6d61 7279 5f65 7272  ageZ.primary_err
-00002730: 6f72 5f6d 7367 da0d 6572 726f 725f 6d65  or_msg..error_me
-00002740: 7373 6167 6572 7e00 0000 720f 0000 0072  ssager~...r....r
-00002750: 0f00 0000 7210 0000 00da 175f 7072 6570  ....r......_prep
-00002760: 6172 655f 6572 726f 725f 7265 7370 6f6e  are_error_respon
-00002770: 7365 4101 0000 7334 0000 0000 010c 030c  seA...s4........
-00002780: 0104 0202 010a 0208 ff12 0102 ff02 020a  ................
-00002790: 010a 010e 0104 010e ff06 040a 0210 0212  ................
-000027a0: 0208 0102 ff08 020e 0208 0102 ff0a 027a  ...............z
-000027b0: 2941 7574 6f74 6173 6b41 5049 436c 6965  )AutotaskAPIClie
-000027c0: 6e74 2e5f 7072 6570 6172 655f 6572 726f  nt._prepare_erro
-000027d0: 725f 7265 7370 6f6e 7365 6302 0000 0000  r_responsec.....
-000027e0: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
-000027f0: 0000 0073 7000 0000 6401 6402 6901 7d02  ...sp...d.d.i.}.
-00002800: 7c00 6a00 7218 7c00 6a00 7c02 6403 3c00  |.j.r.|.j.|.d.<.
-00002810: 7c00 6a01 7228 7c00 6a01 7c02 6404 3c00  |.j.r(|.j.|.d.<.
-00002820: 7c00 6a02 7238 7c00 6a02 7c02 6405 3c00  |.j.r8|.j.|.d.<.
-00002830: 7c00 6a03 726c 7c01 a004 a100 6406 6b03  |.j.rl|.....d.k.
-00002840: 726c 7c00 a005 a100 0100 7c00 6a03 7264  rl|.......|.j.rd
-00002850: 7406 7c00 6a03 6a07 8301 6e02 6400 7c02  t.|.j.j...n.d.|.
-00002860: 6407 3c00 7c02 5300 2908 4e7a 0c43 6f6e  d.<.|.S.).Nz.Con
-00002870: 7465 6e74 2d54 7970 657a 1061 7070 6c69  tent-Typez.appli
-00002880: 6361 7469 6f6e 2f6a 736f 6e5a 0855 7365  cation/jsonZ.Use
-00002890: 724e 616d 655a 0653 6563 7265 745a 1241  rNameZ.SecretZ.A
-000028a0: 7069 496e 7465 6772 6174 696f 6e43 6f64  piIntegrationCod
-000028b0: 65da 0347 4554 5a17 496d 7065 7273 6f6e  e..GETZ.Imperson
-000028c0: 6174 696f 6e52 6573 6f75 7263 6549 6429  ationResourceId)
-000028d0: 0872 2f00 0000 726e 0000 0072 6f00 0000  .r/...rn...ro...
-000028e0: 7275 0000 00da 0575 7070 6572 da1f 6368  ru.....upper..ch
-000028f0: 6563 6b5f 696d 7065 7273 6f6e 6174 696f  eck_impersonatio
-00002900: 6e5f 706f 7373 6962 696c 6974 79da 0373  n_possibility..s
-00002910: 7472 da02 6964 2903 724b 0000 0072 6600  tr..id).rK...rf.
-00002920: 0000 da07 6865 6164 6572 7372 0f00 0000  ....headersr....
-00002930: 720f 0000 0072 1000 0000 da0b 6765 745f  r....r......get_
-00002940: 6865 6164 6572 7361 0100 0073 2000 0000  headersa...s ...
-00002950: 0001 0802 0601 0a01 0601 0a01 0601 0a01  ................
-00002960: 1202 0803 04fe 0401 06ff 0402 02fe 0604  ................
-00002970: 7a1d 4175 746f 7461 736b 4150 4943 6c69  z.AutotaskAPICli
-00002980: 656e 742e 6765 745f 6865 6164 6572 7363  ent.get_headersc
-00002990: 0300 0000 0000 0000 0000 0000 0700 0000  ................
-000029a0: 0600 0000 4300 0000 733e 0000 007c 016a  ....C...s>...|.j
-000029b0: 0072 1064 017c 016a 0069 016e 0474 0183  .r.d.|.j.i.n.t..
-000029c0: 007d 037c 02a0 02a1 0044 005d 1a5c 027d  .}.|.....D.].\.}
-000029d0: 047d 057c 047d 067c 00a0 037c 037c 067c  .}.|.}.|...|.|.|
-000029e0: 05a1 037d 0371 1e7c 0353 00a9 024e 7291  ...}.q.|.S...Nr.
-000029f0: 0000 0029 0472 9100 0000 da04 6469 6374  ...).r......dict
-00002a00: 7254 0000 00da 145f 666f 726d 6174 5f72  rT....._format_r
-00002a10: 6571 7565 7374 5f62 6f64 7929 0772 4b00  equest_body).rK.
-00002a20: 0000 da06 7265 636f 7264 da0f 696e 7365  ....record..inse
-00002a30: 7274 6564 5f66 6965 6c64 73da 0462 6f64  rted_fields..bod
-00002a40: 7972 3200 0000 7244 0000 00da 036b 6579  yr2...rD.....key
-00002a50: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
-00002a60: 0e5f 666f 726d 6174 5f66 6965 6c64 7373  ._format_fieldss
-00002a70: 0100 0073 0a00 0000 0001 1602 1001 0401  ...s............
-00002a80: 1002 7a20 4175 746f 7461 736b 4150 4943  ..z AutotaskAPIC
-00002a90: 6c69 656e 742e 5f66 6f72 6d61 745f 6669  lient._format_fi
-00002aa0: 656c 6473 6304 0000 0000 0000 0000 0000  eldsc...........
-00002ab0: 0004 0000 0008 0000 0043 0000 0073 ac00  .........C...s..
-00002ac0: 0000 7400 7c03 7401 6a01 8302 722e 7c01  ..t.|.t.j...r.|.
-00002ad0: a002 7c02 7c03 a003 7404 a005 6401 a101  ..|.|...t...d...
-00002ae0: a101 a006 6402 a101 6901 a101 0100 6e7a  ....d...i.....nz
-00002af0: 7400 7c03 7407 6a08 8302 724c 7c01 a002  t.|.t.j...rL|...
-00002b00: 7c02 7c03 6a09 6901 a101 0100 6e5c 7400  |.|.j.i.....n\t.
-00002b10: 7c03 740a 6a0b 8302 7274 7c01 a002 7c02  |.t.j...rt|...|.
-00002b20: 7c03 726a 740c 7c03 8301 6e02 6403 6901  |.rjt.|...n.d.i.
-00002b30: a101 0100 6e34 7400 7c03 740d 8302 728e  ....n4t.|.t...r.
-00002b40: 7c01 a002 7c02 7c03 6901 a101 0100 6e1a  |...|.|.i.....n.
-00002b50: 7c01 a002 7c02 7c03 72a0 740c 7c03 8301  |...|.|.r.t.|...
-00002b60: 6e02 6404 6901 a101 0100 7c01 5300 2905  n.d.i.....|.S.).
-00002b70: 4eda 0355 5443 7a12 2559 2d25 6d2d 2564  N..UTCz.%Y-%m-%d
-00002b80: 5425 483a 254d 3a25 535a da01 3072 8000  T%H:%M:%SZ..0r..
-00002b90: 0000 290e da0a 6973 696e 7374 616e 6365  ..)...isinstance
-00002ba0: da08 6461 7465 7469 6d65 da06 7570 6461  ..datetime..upda
-00002bb0: 7465 da0a 6173 7469 6d65 7a6f 6e65 da04  te..astimezone..
-00002bc0: 7079 747a da08 7469 6d65 7a6f 6e65 da08  pytz..timezone..
-00002bd0: 7374 7266 7469 6d65 7205 0000 00da 054d  strftimer......M
-00002be0: 6f64 656c 7291 0000 00da 0764 6563 696d  odelr......decim
-00002bf0: 616c da07 4465 6369 6d61 6c72 9000 0000  al..Decimalr....
-00002c00: da04 626f 6f6c 2904 724b 0000 0072 9900  ..bool).rK...r..
-00002c10: 0000 729a 0000 0072 4400 0000 720f 0000  ..r....rD...r...
-00002c20: 0072 0f00 0000 7210 0000 0072 9600 0000  .r....r....r....
-00002c30: 7c01 0000 7334 0000 0000 010c 0104 0102  |...s4..........
-00002c40: 0004 0108 ff04 0202 fe02 ff08 060c 0104  ................
-00002c50: 0102 0004 ff08 040c 0104 0112 ff06 040a  ................
-00002c60: 0104 0106 ff06 0404 0112 ff04 047a 2641  .............z&A
-00002c70: 7574 6f74 6173 6b41 5049 436c 6965 6e74  utotaskAPIClient
-00002c80: 2e5f 666f 726d 6174 5f72 6571 7565 7374  ._format_request
-00002c90: 5f62 6f64 7963 0300 0000 0000 0000 0000  _bodyc..........
-00002ca0: 0000 0700 0000 0600 0000 4300 0000 734e  ..........C...sN
-00002cb0: 0000 007c 016a 0072 1064 017c 016a 0069  ...|.j.r.d.|.j.i
-00002cc0: 016e 0474 0183 007d 037c 02a0 02a1 0044  .n.t...}.|.....D
-00002cd0: 005d 2a5c 027d 047d 057c 047c 016a 036b  .]*\.}.}.|.|.j.k
-00002ce0: 0672 1e7c 016a 037c 0419 007d 067c 00a0  .r.|.j.|...}.|..
-00002cf0: 047c 037c 067c 05a1 037d 0371 1e7c 0353  .|.|.|...}.q.|.S
-00002d00: 0072 9400 0000 2905 7291 0000 0072 9500  .r....).r....r..
-00002d10: 0000 7254 0000 00da 0f41 5554 4f54 4153  ..rT.....AUTOTAS
-00002d20: 4b5f 4649 454c 4453 7296 0000 0029 0772  K_FIELDSr....).r
-00002d30: 4b00 0000 5a0a 6170 695f 656e 7469 7479  K...Z.api_entity
-00002d40: 7298 0000 0072 9900 0000 7232 0000 0072  r....r....r2...r
-00002d50: 4400 0000 729a 0000 0072 0f00 0000 720f  D...r....r....r.
-00002d60: 0000 0072 1000 0000 da15 5f6c 6567 6163  ...r......_legac
-00002d70: 795f 666f 726d 6174 5f66 6965 6c64 7399  y_format_fields.
-00002d80: 0100 0073 0c00 0000 0007 1602 1001 0a01  ...s............
-00002d90: 0a01 1002 7a27 4175 746f 7461 736b 4150  ....z'AutotaskAP
-00002da0: 4943 6c69 656e 742e 5f6c 6567 6163 795f  IClient._legacy_
-00002db0: 666f 726d 6174 5f66 6965 6c64 7372 1e00  format_fieldsr..
-00002dc0: 0000 6304 0000 0000 0000 0000 0000 0009  ..c.............
-00002dd0: 0000 0006 0000 000f 0000 0073 7200 0000  ...........sr...
-00002de0: 7400 8800 6a01 6401 1900 7402 7403 7404  t...j.d...t.t.t.
-00002df0: 6402 8d04 6403 7c03 6403 6603 8700 6601  d...d.|.d.f...f.
-00002e00: 6404 6405 8409 8301 7d06 7c01 7234 7c01  d.d.....}.|.r4|.
-00002e10: 7d07 6e24 8800 6a05 6a06 7c03 6406 8d01  }.n$..j.j.|.d...
-00002e20: 5c02 7d08 8800 5f07 6407 a008 8800 a009  \.}..._.d.......
-00002e30: a100 7c08 a102 7d07 7c06 7c07 6601 7c02  ..|...}.|.|.f.|.
-00002e40: 7c03 8800 6a07 6408 9c03 7c05 9702 8e01  |...j.d...|.....
-00002e50: 5300 2909 7a8d 0a20 2020 2020 2020 2072  S.).z..        r
-00002e60: 6574 7279 5f63 6f75 6e74 6572 2069 7320  etry_counter is 
-00002e70: 6120 6469 6374 2069 6e20 7468 6520 666f  a dict in the fo
-00002e80: 726d 207b 2763 6f75 6e74 273a 2030 7d20  rm {'count': 0} 
-00002e90: 7468 6174 2069 7320 7061 7373 6564 2069  that is passed i
-00002ea0: 6e0a 2020 2020 2020 2020 746f 2076 6572  n.        to ver
-00002eb0: 6966 7920 7468 6520 6e75 6d62 6572 206f  ify the number o
-00002ec0: 6620 6174 7465 6d70 7473 2074 6861 7420  f attempts that 
-00002ed0: 7765 7265 206d 6164 652e 0a20 2020 2020  were made..     
-00002ee0: 2020 205a 0c6d 6178 5f61 7474 656d 7074     Z.max_attempt
-00002ef0: 7329 045a 1773 746f 705f 6d61 785f 6174  s).Z.stop_max_at
-00002f00: 7465 6d70 745f 6e75 6d62 6572 5a1b 7761  tempt_numberZ.wa
-00002f10: 6974 5f65 7870 6f6e 656e 7469 616c 5f6d  it_exponential_m
-00002f20: 756c 7469 706c 6965 725a 1477 6169 745f  ultiplierZ.wait_
-00002f30: 6578 706f 6e65 6e74 6961 6c5f 6d61 785a  exponential_maxZ
-00002f40: 1272 6574 7279 5f6f 6e5f 6578 6365 7074  .retry_on_except
-00002f50: 696f 6e4e 6304 0000 0000 0000 0000 0000  ionNc...........
-00002f60: 0009 0000 000a 0000 001b 0000 0073 1602  .............s..
-00002f70: 0000 7c01 730c 6401 6402 6901 7d01 7c01  ..|.s.d.d.i.}.|.
-00002f80: 6401 0500 1900 6403 3700 0300 3c00 7a2e  d.....d.7...<.z.
-00002f90: 8800 a000 7c00 7c02 7c03 a103 0100 7401  ....|.|.|.....t.
-00002fa0: 6a02 7c02 7c00 7c03 8800 6a03 8800 a004  j.|.|.|...j.....
-00002fb0: 7c02 a101 6404 8d05 7d05 5700 6e4a 0400  |...d...}.W.nJ..
-00002fc0: 7401 6a05 6b0a 7294 0100 7d06 0100 7a2a  t.j.k.r...}...z*
-00002fd0: 7406 a007 6405 a008 7c02 a009 a100 7c00  t...d...|.....|.
-00002fe0: 7c06 a103 a101 0100 740a 6406 a008 7c06  |.......t.d...|.
-00002ff0: a101 8301 8201 5700 3500 6400 7d06 7e06  ......W.5.d.}.~.
-00003000: 5800 5900 6e02 5800 6407 7c05 6a0b 0400  X.Y.n.X.d.|.j...
-00003010: 0300 6b01 72ae 6408 6b00 9001 720c 6e04  ..k.r.d.k...r.n.
-00003020: 0100 6e5a 7a0a 7c05 a00c a100 5700 5300  ..nZz.|.....W.S.
-00003030: 0400 740d 6b0a 9001 7206 0100 7d06 0100  ..t.k...r...}...
-00003040: 7a2a 7406 a007 6409 a008 7c02 a009 a100  z*t...d...|.....
-00003050: 7c00 7c06 a103 a101 0100 740a 6406 a008  |.|.......t.d...
-00003060: 7c06 a101 8301 8201 5700 3500 6400 7d06  |.......W.5.d.}.
-00003070: 7e06 5800 5900 6e02 5800 9001 6e06 7c05  ~.X.Y.n.X...n.|.
-00003080: 6a0b 640a 6b02 9001 7272 640b a008 7c00  j.d.k...rrd...|.
-00003090: a101 7d07 7406 a00e 7c07 a101 0100 7c01  ..}.t...|.....|.
-000030a0: 6401 1900 8800 6a0f 6b01 9001 7268 7410  d.....j.k...rht.
-000030b0: 7411 8301 7d08 7c08 7412 640c 640d 8d01  t...}.|.t.d.d...
-000030c0: 6b03 9001 7268 7406 a013 640e a101 0100  k...rht...d.....
-000030d0: 740a 7c05 6a14 8301 8201 7415 7c07 8301  t.|.j.....t.|...
-000030e0: 8201 6ea0 7c05 6a0b 640f 6b02 9001 729c  ..n.|.j.d.k...r.
-000030f0: 8800 a016 7c05 a101 0100 7417 8800 a018  ....|.....t.....
-00003100: 7c05 a101 7c05 6a0b 8302 8201 6e76 6410  |...|.j.....nvd.
-00003110: 7c05 6a0b 0400 0300 6b01 9001 72b6 6411  |.j.....k...r.d.
-00003120: 6b00 9001 72d4 6e04 0100 6e1a 8800 a016  k...r.n...n.....
-00003130: 7c05 a101 0100 7415 8800 a018 7c05 a101  |.....t.....|...
-00003140: 8301 8201 6e3e 7c05 6a0b 6412 6b02 9001  ....n>|.j.d.k...
-00003150: 72fa 8800 a016 7c05 a101 0100 7419 8800  r.....|.....t...
-00003160: a018 7c05 a101 8301 8201 6e18 8800 a016  ..|.......n.....
-00003170: 7c05 a101 0100 740a 8800 a018 7c05 a101  |.....t.....|...
-00003180: 8301 8201 6400 5300 2913 4eda 0563 6f75  ....d.S.).N..cou
-00003190: 6e74 7201 0000 0072 6d00 0000 2903 da04  ntr....rm...)...
-000031a0: 6461 7461 7222 0000 0072 9200 0000 fa19  datar"...r......
-000031b0: 5265 7175 6573 7420 6661 696c 6564 3a20  Request failed: 
-000031c0: 7b7d 207b 7d3a 207b 7dfa 027b 7d72 3400  {} {}: {}..{}r4.
-000031d0: 0000 e92c 0100 007a 2c52 6571 7565 7374  ...,...z,Request
-000031e0: 2066 6169 6c65 6420 6475 7269 6e67 204a   failed during J
-000031f0: 534f 4e20 6465 636f 6465 3a20 7b7d 207b  SON decode: {} {
-00003200: 7d3a 207b 7d69 9101 0000 7a18 556e 6175  }: {}i....z.Unau
-00003210: 7468 6f72 697a 6564 2072 6571 7565 7374  thorized request
-00003220: 3a20 7b7d 5472 2b00 0000 7a43 5a6f 6e65  : {}Tr+...zCZone
-00003230: 2069 6e66 6f72 6d61 7469 6f6e 2068 6173   information has
-00003240: 2062 6565 6e20 6368 616e 6765 642c 2073   been changed, s
-00003250: 6f20 7468 6973 2072 6571 7565 7374 2077  o this request w
-00003260: 696c 6c20 6265 2072 6574 7269 6564 2ee9  ill be retried..
-00003270: 9301 0000 e990 0100 00e9 f301 0000 7235  ..............r5
-00003280: 0000 0029 1ada 0b6c 6f67 5f6d 6573 7361  ...)...log_messa
-00003290: 6765 723a 0000 00da 0772 6571 7565 7374  ger:.....request
-000032a0: 7222 0000 0072 9300 0000 723f 0000 0072  r"...r....r?...r
-000032b0: 3700 0000 727b 0000 0072 3900 0000 728e  7...r{...r9...r.
-000032c0: 0000 0072 0900 0000 723b 0000 0072 3c00  ...r....r;...r<.
-000032d0: 0000 7202 0000 00da 0777 6172 6e69 6e67  ..r......warning
-000032e0: da10 4d41 585f 3430 315f 4154 5445 4d50  ..MAX_401_ATTEMP
-000032f0: 5453 7220 0000 0072 2400 0000 722d 0000  TSr ...r$...r-..
-00003300: 00da 0469 6e66 6f72 3e00 0000 7211 0000  ...infor>...r...
-00003310: 0072 7c00 0000 7214 0000 0072 8c00 0000  .r|...r....r....
-00003320: 7212 0000 0029 0972 4000 0000 da15 7265  r....).r@.....re
-00003330: 7175 6573 745f 7265 7472 795f 636f 756e  quest_retry_coun
-00003340: 7465 72da 0e72 6571 7565 7374 5f6d 6574  ter..request_met
-00003350: 686f 64da 0c72 6571 7565 7374 5f62 6f64  hod..request_bod
-00003360: 79da 066b 7761 7267 7372 4100 0000 7218  y..kwargsrA...r.
-00003370: 0000 0072 7e00 0000 5a0a 6361 6368 6564  ...r~...Z.cached
-00003380: 5f75 726c 7250 0000 0072 0f00 0000 7210  _urlrP...r....r.
-00003390: 0000 00da 0f5f 6665 7463 685f 7265 736f  ....._fetch_reso
-000033a0: 7572 6365 af01 0000 7378 0000 0000 0704  urce....sx......
-000033b0: 0108 0110 0202 010e 0204 0102 0102 0102  ................
-000033c0: 0104 0108 fb0a 0812 0108 0106 0002 0002  ................
-000033d0: ff06 0220 021c 0102 010a 0112 0104 0104  ... ............
-000033e0: 0106 0002 0002 ff02 ff04 0424 020c 020a  ...........$....
-000033f0: 010a 0110 0108 0110 010a 020a 010a 010c  ................
-00003400: 010a 0102 0108 0104 fe06 031e 010a 0102  ................
-00003410: 0108 ff06 020c 010a 0102 0108 ff06 030a  ................
-00003420: 0102 0108 ff7a 3941 7574 6f74 6173 6b41  .....z9AutotaskA
-00003430: 5049 436c 6965 6e74 2e66 6574 6368 5f72  PIClient.fetch_r
-00003440: 6573 6f75 7263 652e 3c6c 6f63 616c 733e  esource.<locals>
-00003450: 2e5f 6665 7463 685f 7265 736f 7572 6365  ._fetch_resource
-00003460: 2901 7266 0000 00fa 047b 7d7b 7d29 0372  ).rf.....{}{}).r
-00003470: b800 0000 72b9 0000 0072 ba00 0000 290a  ....r....r....).
-00003480: 7207 0000 0072 7400 0000 da22 5245 5452  r....rt...."RETR
-00003490: 595f 5741 4954 5f45 5850 4f4e 454e 5449  Y_WAIT_EXPONENTI
-000034a0: 414c 5f4d 554c 5441 5050 4c49 4552 da1a  AL_MULTAPPLIER..
-000034b0: 5245 5452 595f 5741 4954 5f45 5850 4f4e  RETRY_WAIT_EXPON
-000034c0: 454e 5449 414c 5f4d 4158 721c 0000 0072  ENTIAL_MAXr....r
-000034d0: 7600 0000 726a 0000 0072 7700 0000 7239  v...rj...rw...r9
-000034e0: 0000 0072 7a00 0000 2909 724b 0000 00da  ...rz...).rK....
-000034f0: 086e 6578 745f 7572 6c5a 0d72 6574 7279  .next_urlZ.retry
-00003500: 5f63 6f75 6e74 6572 7266 0000 0072 1700  _counterrf...r..
-00003510: 0000 72bb 0000 0072 bc00 0000 7208 0000  ..r....r....r...
-00003520: 005a 0e71 7565 7279 5f65 6e64 706f 696e  .Z.query_endpoin
-00003530: 7472 0f00 0000 7250 0000 0072 1000 0000  tr....rP...r....
-00003540: da0e 6665 7463 685f 7265 736f 7572 6365  ..fetch_resource
-00003550: a901 0000 732e 0000 0000 060a 0102 0102  ....s...........
-00003560: 0102 fd04 0402 0102 0002 ff10 3e04 0106  ............>...
-00003570: 040c ff08 0210 0202 0102 ff02 0102 0102  ................
-00003580: 0004 fe04 0202 fe7a 2041 7574 6f74 6173  .......z Autotas
-00003590: 6b41 5049 436c 6965 6e74 2e66 6574 6368  kAPIClient.fetch
-000035a0: 5f72 6573 6f75 7263 6563 0400 0000 0000  _resourcec......
-000035b0: 0000 0000 0000 0500 0000 0400 0000 4300  ..............C.
-000035c0: 0000 733e 0000 007c 0372 087c 036e 0264  ..s>...|.r.|.n.d
-000035d0: 017d 0364 02a0 007c 02a0 01a1 007c 01a1  .}.d...|.....|..
-000035e0: 027d 047c 0264 036b 0272 3064 04a0 007c  .}.|.d.k.r0d...|
-000035f0: 047c 03a1 027d 0474 02a0 037c 04a1 0101  .|...}.t...|....
-00003600: 0064 0053 0029 054e 7280 0000 00fa 174d  .d.S.).Nr......M
-00003610: 616b 696e 6720 7b7d 2072 6571 7565 7374  aking {} request
-00003620: 2074 6f20 7b7d 7258 0000 007a 147b 7d2e   to {}rX...z.{}.
-00003630: 2052 6571 7565 7374 2062 6f64 793a 207b   Request body: {
-00003640: 7d29 0472 3900 0000 728e 0000 0072 3700  }).r9...r....r7.
-00003650: 0000 7238 0000 0029 0572 4b00 0000 7268  ..r8...).rK...rh
-00003660: 0000 0072 6600 0000 7299 0000 005a 0e6c  ...rf...r....Z.l
-00003670: 6f67 6765 725f 6d65 7373 6167 6572 0f00  ogger_messager..
-00003680: 0000 720f 0000 0072 1000 0000 72b3 0000  ..r....r....r...
-00003690: 00fd 0100 0073 0e00 0000 0001 0c03 0eff  .....s..........
-000036a0: 0202 0802 0aff 0203 7a1d 4175 746f 7461  ........z.Autota
-000036b0: 736b 4150 4943 6c69 656e 742e 6c6f 675f  skAPIClient.log_
-000036c0: 6d65 7373 6167 6563 0100 0000 0000 0000  messagec........
-000036d0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-000036e0: 7320 0000 007c 006a 0072 1c7c 006a 006a  s ...|.j.r.|.j.j
-000036f0: 01a0 027c 00a1 0173 1c74 0364 0183 0182  ...|...s.t.d....
-00003700: 0164 0053 0029 024e 7a44 596f 7520 646f  .d.S.).NzDYou do
-00003710: 206e 6f74 2068 6176 6520 7468 6520 6164   not have the ad
-00003720: 6571 7561 7465 2070 6572 6d69 7373 696f  equate permissio
-00003730: 6e73 2028 696d 7065 7273 6f6e 6174 696f  ns (impersonatio
-00003740: 6e20 6c69 6d69 7461 7469 6f6e 292e 2904  n limitation).).
-00003750: 7275 0000 00da 0c6c 6963 656e 7365 5f74  ru.....license_t
-00003760: 7970 65da 1168 6173 5f69 6d70 6572 736f  ype..has_imperso
-00003770: 6e61 7469 6f6e 7215 0000 0072 5000 0000  nationr....rP...
-00003780: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00003790: 8f00 0000 0802 0000 730c 0000 0000 010e  ........s.......
-000037a0: 0102 ff04 0202 0102 ff7a 3141 7574 6f74  .........z1Autot
-000037b0: 6173 6b41 5049 436c 6965 6e74 2e63 6865  askAPIClient.che
-000037c0: 636b 5f69 6d70 6572 736f 6e61 7469 6f6e  ck_impersonation
-000037d0: 5f70 6f73 7369 6269 6c69 7479 6304 0000  _possibilityc...
-000037e0: 0000 0000 0000 0000 0008 0000 000a 0000  ................
-000037f0: 0043 0000 0073 ec01 0000 7a32 7400 a001  .C...s....z2t...
-00003800: 6401 a002 7c01 7c02 a102 a101 0100 7403  d...|.|.......t.
-00003810: 6a04 7c01 7c02 7c03 7c00 6a05 7c00 a006  j.|.|.|.|.j.|...
-00003820: 7c01 a101 6402 8d05 7d04 5700 6e7e 0400  |...d...}.W.n~..
-00003830: 7407 6b0a 726c 0100 7d05 0100 7a1c 7400  t.k.rl..}...z.t.
-00003840: a008 6403 a002 7c01 7c02 7c05 a103 a101  ..d...|.|.|.....
-00003850: 0100 7c05 8201 5700 3500 6404 7d05 7e05  ..|...W.5.d.}.~.
-00003860: 5800 5900 6e46 0400 7403 6a09 6b0a 72b0  X.Y.nF..t.j.k.r.
-00003870: 0100 7d05 0100 7a26 7400 a008 6403 a002  ..}...z&t...d...
-00003880: 7c01 7c02 7c05 a103 a101 0100 740a 6405  |.|.|.......t.d.
-00003890: a002 7c05 a101 8301 8201 5700 3500 6404  ..|.......W.5.d.
-000038a0: 7d05 7e05 5800 5900 6e02 5800 7c04 6a0b  }.~.X.Y.n.X.|.j.
-000038b0: 6406 6b02 72c0 6404 5300 6407 7c04 6a0b  d.k.r.d.S.d.|.j.
-000038c0: 0400 0300 6b01 72d6 6408 6b00 72e2 6e04  ....k.r.d.k.r.n.
-000038d0: 0100 6e08 7c04 a00c a100 5300 7c04 6a0b  ..n.|.....S.|.j.
-000038e0: 6409 6b02 9001 720c 7c00 a00d 7c04 a101  d.k...r.|...|...
-000038f0: 0100 740e 7c00 a00f 7c04 a101 7c04 6a0b  ..t.|...|...|.j.
-00003900: 8302 8201 6edc 7c04 6a0b 640a 6b02 9001  ....n.|.j.d.k...
-00003910: 7238 640b a002 7c04 6a10 a101 7d06 7400  r8d...|.j...}.t.
-00003920: a011 7c06 a101 0100 7412 7c06 8301 8201  ..|.....t.|.....
-00003930: 6eb0 640c 7c04 6a0b 0400 0300 6b01 9001  n.d.|.j.....k...
-00003940: 7252 640d 6b00 9001 7270 6e04 0100 6e1a  rRd.k...rpn...n.
-00003950: 7c00 a00d 7c04 a101 0100 7413 7c00 a00f  |...|.....t.|...
-00003960: 7c04 a101 8301 8201 6e78 7c04 6a0b 640e  |.......nx|.j.d.
-00003970: 6b02 9001 72d6 7c00 a00d 7c04 a101 0100  k...r.|...|.....
-00003980: 7c00 a00f 7c04 a101 7d07 7414 7c07 6b06  |...|...}.t.|.k.
-00003990: 9001 72b6 7c00 6a15 9001 72ac 7c00 a016  ..r.|.j...r.|...
-000039a0: 7c07 a101 7d07 740e 7c07 8301 8201 6e1e  |...}.t.|.....n.
-000039b0: 7417 7c07 6b06 9001 72cc 7412 7c07 640a  t.|.k...r.t.|.d.
-000039c0: 8302 8201 6e08 7418 7c07 8301 8201 6e12  ....n.t.|.....n.
-000039d0: 7c00 a00d 7c04 a101 0100 740a 7c04 8301  |...|.....t.|...
-000039e0: 8201 6404 5300 290f 7a51 0a20 2020 2020  ..d.S.).zQ.     
-000039f0: 2020 2049 7373 7565 2074 6865 2067 6976     Issue the giv
-00003a00: 656e 2074 7970 6520 6f66 2072 6571 7565  en type of reque
-00003a10: 7374 2074 6f20 7468 6520 7370 6563 6966  st to the specif
-00003a20: 6965 6420 5245 5354 2065 6e64 706f 696e  ied REST endpoin
-00003a30: 742e 0a20 2020 2020 2020 2072 c200 0000  t..        r....
-00003a40: 2903 723c 0000 0072 2200 0000 7292 0000  ).r<...r"...r...
-00003a50: 0072 ad00 0000 4e72 ae00 0000 e9cc 0000  .r....Nr........
-00003a60: 0072 3400 0000 72af 0000 0072 b000 0000  .r4...r....r....
-00003a70: 6994 0100 00fa 1652 6573 6f75 7263 6520  i......Resource 
-00003a80: 6e6f 7420 666f 756e 643a 207b 7d72 b100  not found: {}r..
-00003a90: 0000 72b2 0000 0072 3500 0000 2919 7237  ..r....r5...).r7
-00003aa0: 0000 0072 3800 0000 7239 0000 0072 3a00  ...r8...r9...r:.
-00003ab0: 0000 72b4 0000 0072 2200 0000 7293 0000  ..r....r"...r...
-00003ac0: 0072 1500 0000 727b 0000 0072 3f00 0000  .r....r{...r?...
-00003ad0: 7209 0000 0072 3b00 0000 723c 0000 0072  r....r;...r<...r
-00003ae0: 7c00 0000 7214 0000 0072 8c00 0000 7208  |...r....r....r.
-00003af0: 0000 0072 b500 0000 7213 0000 0072 1100  ...r....r....r..
-00003b00: 0000 da17 464f 5242 4944 4445 4e5f 4552  ....FORBIDDEN_ER
-00003b10: 524f 525f 4d45 5353 4147 4572 7500 0000  ROR_MESSAGEru...
-00003b20: 727f 0000 00da 174e 4f5f 5245 434f 5244  r......NO_RECORD
-00003b30: 5f45 5252 4f52 5f4d 4553 5341 4745 7212  _ERROR_MESSAGEr.
-00003b40: 0000 0029 0872 4b00 0000 7266 0000 0072  ...).rK...rf...r
-00003b50: 4000 0000 7299 0000 0072 4100 0000 7218  @...r....rA...r.
-00003b60: 0000 0072 7e00 0000 5a0e 7072 6570 6172  ...r~...Z.prepar
-00003b70: 6564 5f65 7272 6f72 720f 0000 0072 0f00  ed_errorr....r..
-00003b80: 0000 7210 0000 0072 b400 0000 0f02 0000  ..r....r........
-00003b90: 736c 0000 0000 0402 0104 010a ff04 0404  sl..............
-00003ba0: 0102 0102 0102 0104 0108 fb0a 0710 0104  ................
-00003bb0: 010c ff04 0314 0112 0104 010c ff04 0320  ............... 
-00003bc0: 020a 0104 011a 0108 010c 010a 0102 0108  ................
-00003bd0: 0004 ff06 020c 010c 010a 010a 011e 010a  ................
-00003be0: 0102 0108 ff06 020c 010a 010a 0a0a 0108  ................
-00003bf0: 0104 0102 ff04 030a 010a 010c 020a 020a  ................
-00003c00: 017a 1941 7574 6f74 6173 6b41 5049 436c  .z.AutotaskAPICl
-00003c10: 6965 6e74 2e72 6571 7565 7374 6302 0000  ient.requestc...
-00003c20: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00003c30: 0043 0000 0073 1a00 0000 7c00 6a00 a001  .C...s....|.j...
-00003c40: 7c01 a101 0100 7402 7c00 6a00 8301 6401  |.....t.|.j...d.
-00003c50: 1800 5300 2902 4e72 6d00 0000 2903 7276  ..S.).Nrm...).rv
-00003c60: 0000 0072 6b00 0000 724e 0000 0072 5500  ...rk...rN...rU.
-00003c70: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00003c80: 00da 0d61 6464 5f63 6f6e 6469 7469 6f6e  ...add_condition
-00003c90: 5402 0000 7304 0000 0000 010c 017a 1f41  T...s........z.A
-00003ca0: 7574 6f74 6173 6b41 5049 436c 6965 6e74  utotaskAPIClient
-00003cb0: 2e61 6464 5f63 6f6e 6469 7469 6f6e 6301  .add_conditionc.
-00003cc0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00003cd0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-00003ce0: 5300 7229 0000 00a9 0172 7600 0000 7250  S.r).....rv...rP
-00003cf0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00003d00: 0000 da0e 6765 745f 636f 6e64 6974 696f  ....get_conditio
-00003d10: 6e73 5802 0000 7302 0000 0000 017a 2041  nsX...s......z A
-00003d20: 7574 6f74 6173 6b41 5049 436c 6965 6e74  utotaskAPIClient
-00003d30: 2e67 6574 5f63 6f6e 6469 7469 6f6e 7363  .get_conditionsc
-00003d40: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00003d50: 0200 0000 4300 0000 730c 0000 007c 006a  ....C...s....|.j
-00003d60: 007c 013d 0064 0053 0072 2900 0000 72ca  .|.=.d.S.r)...r.
-00003d70: 0000 0029 0272 4b00 0000 da05 696e 6465  ...).rK.....inde
-00003d80: 7872 0f00 0000 720f 0000 0072 1000 0000  xr....r....r....
-00003d90: da10 7265 6d6f 7665 5f63 6f6e 6469 7469  ..remove_conditi
-00003da0: 6f6e 5b02 0000 7302 0000 0000 017a 2241  on[...s......z"A
-00003db0: 7574 6f74 6173 6b41 5049 436c 6965 6e74  utotaskAPIClient
-00003dc0: 2e72 656d 6f76 655f 636f 6e64 6974 696f  .remove_conditio
-00003dd0: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
-00003de0: 0000 0200 0000 4300 0000 730c 0000 0074  ......C...s....t
-00003df0: 0083 007c 005f 0164 0053 0072 2900 0000  ...|._.d.S.r)...
-00003e00: 2902 7256 0000 0072 7600 0000 7250 0000  ).rV...rv...rP..
-00003e10: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00003e20: da10 636c 6561 725f 636f 6e64 6974 696f  ..clear_conditio
-00003e30: 6e73 5e02 0000 7302 0000 0000 017a 2241  ns^...s......z"A
-00003e40: 7574 6f74 6173 6b41 5049 436c 6965 6e74  utotaskAPIClient
-00003e50: 2e63 6c65 6172 5f63 6f6e 6469 7469 6f6e  .clear_condition
-00003e60: 7363 0200 0000 0000 0000 0000 0000 0400  sc..............
-00003e70: 0000 0300 0000 4f00 0000 7312 0000 007c  ......O...s....|
-00003e80: 006a 007c 0166 017c 029e 027c 038e 0153  .j.|.f.|...|...S
-00003e90: 0072 2900 0000 a901 72c1 0000 00a9 0472  .r).....r......r
-00003ea0: 4b00 0000 72c0 0000 0072 1700 0000 72bb  K...r....r....r.
-00003eb0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00003ec0: 0000 721e 0000 0061 0200 0073 0200 0000  ..r....a...s....
-00003ed0: 0001 7a15 4175 746f 7461 736b 4150 4943  ..z.AutotaskAPIC
-00003ee0: 6c69 656e 742e 6765 7463 0200 0000 0000  lient.getc......
-00003ef0: 0000 0000 0000 0500 0000 0400 0000 4300  ..............C.
-00003f00: 0000 7342 0000 0064 01a0 007c 00a0 01a1  ..sB...d...|....
-00003f10: 007c 01a1 027d 027c 00a0 027c 02a1 017d  .|...}.|...|...}
-00003f20: 037c 0364 0219 0073 3e64 03a0 007c 02a1  .|.d...s>d...|..
-00003f30: 017d 0474 03a0 047c 04a1 0101 0074 057c  .}.t...|.....t.|
-00003f40: 0483 0182 017c 0353 0029 044e 72bd 0000  .....|.S.).Nr...
-00003f50: 00da 0469 7465 6d72 c600 0000 2906 7239  ...itemr....).r9
-00003f60: 0000 0072 7a00 0000 72c1 0000 0072 3700  ...rz...r....r7.
-00003f70: 0000 72b5 0000 0072 1300 0000 2905 724b  ..r....r....).rK
-00003f80: 0000 005a 0b69 6e73 7461 6e63 655f 6964  ...Z.instance_id
-00003f90: 7240 0000 0072 4100 0000 727e 0000 0072  r@...rA...r~...r
-00003fa0: 0f00 0000 720f 0000 0072 1000 0000 da0a  ....r....r......
-00003fb0: 6765 745f 7369 6e67 6c65 6402 0000 730e  get_singled...s.
-00003fc0: 0000 0000 0110 010a 0108 010a 010a 0108  ................
-00003fd0: 017a 1c41 7574 6f74 6173 6b41 5049 436c  .z.AutotaskAPICl
-00003fe0: 6965 6e74 2e67 6574 5f73 696e 676c 6563  ient.get_singlec
-00003ff0: 0300 0000 0000 0000 0000 0000 0400 0000  ................
-00004000: 0500 0000 4300 0000 731e 0000 007c 00a0  ....C...s....|..
-00004010: 007c 017c 02a1 027d 037c 00a0 0164 017c  .|.|...}.|...d.|
-00004020: 00a0 02a1 007c 03a1 0353 00a9 024e da05  .....|...S...N..
-00004030: 7061 7463 6829 0372 aa00 0000 72b4 0000  patch).r....r...
-00004040: 0072 7a00 0000 a904 724b 0000 00da 0869  .rz.....rK.....i
-00004050: 6e73 7461 6e63 65da 0e63 6861 6e67 6564  nstance..changed
-00004060: 5f66 6965 6c64 7372 9900 0000 720f 0000  _fieldsr....r...
-00004070: 0072 0f00 0000 7210 0000 0072 a000 0000  .r....r....r....
-00004080: 6d02 0000 7304 0000 0000 010c 017a 1841  m...s........z.A
-00004090: 7574 6f74 6173 6b41 5049 436c 6965 6e74  utotaskAPIClient
-000040a0: 2e75 7064 6174 6563 0200 0000 0000 0000  .updatec........
-000040b0: 0000 0000 0500 0000 0500 0000 4b00 0000  ............K...
-000040c0: 7328 0000 007c 00a0 007c 017c 02a1 027d  s(...|...|.|...}
-000040d0: 037c 00a0 0164 017c 00a0 02a1 007c 03a1  .|...d.|.....|..
-000040e0: 037d 047c 04a0 0364 02a1 0153 00a9 034e  .}.|...d...S...N
-000040f0: 7258 0000 00da 0669 7465 6d49 6429 0472  rX.....itemId).r
-00004100: aa00 0000 72b4 0000 0072 7a00 0000 721e  ....r....rz...r.
-00004110: 0000 0029 0572 4b00 0000 72d6 0000 0072  ...).rK...r....r
-00004120: bb00 0000 7299 0000 0072 4100 0000 720f  ....r....rA...r.
-00004130: 0000 0072 0f00 0000 7210 0000 00da 0663  ...r....r......c
-00004140: 7265 6174 6571 0200 0073 0600 0000 0001  reateq...s......
-00004150: 0c02 1201 7a18 4175 746f 7461 736b 4150  ....z.AutotaskAP
-00004160: 4943 6c69 656e 742e 6372 6561 7465 6303  IClient.createc.
-00004170: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00004180: 0000 0043 0000 0073 2800 0000 7c00 a000  ...C...s(...|...
-00004190: a100 7401 7c01 6a02 8301 1700 7d03 7c00  ..t.|.j.....}.|.
-000041a0: a003 6401 7c03 a102 7d04 7c04 a004 6402  ..d.|...}.|...d.
-000041b0: a101 5300 2903 4eda 0664 656c 6574 6572  ..S.).N..deleter
-000041c0: d900 0000 2905 727a 0000 0072 9000 0000  ....).rz...r....
-000041d0: 7291 0000 0072 b400 0000 721e 0000 00a9  r....r....r.....
-000041e0: 0572 4b00 0000 72d6 0000 00da 0670 6172  .rK...r......par
-000041f0: 656e 7472 4000 0000 7241 0000 0072 0f00  entr@...rA...r..
-00004200: 0000 720f 0000 0072 1000 0000 72db 0000  ..r....r....r...
-00004210: 0077 0200 0073 0600 0000 0001 1201 0c02  .w...s..........
-00004220: 7a18 4175 746f 7461 736b 4150 4943 6c69  z.AutotaskAPICli
-00004230: 656e 742e 6465 6c65 7465 2906 4e4e 4e4e  ent.delete).NNNN
-00004240: 4e4e 2901 4e29 034e 4e72 1e00 0000 2901  NN).N).NNr....).
-00004250: 4e29 014e 291d 720b 0000 0072 0c00 0000  N).N).r....r....
-00004260: 720d 0000 0072 7100 0000 72b6 0000 0072  r....rq...r....r
-00004270: 4d00 0000 da08 7072 6f70 6572 7479 7278  M.....propertyrx
-00004280: 0000 0072 7a00 0000 727c 0000 0072 7f00  ...rz...r|...r..
-00004290: 0000 728c 0000 0072 9300 0000 729b 0000  ..r....r....r...
-000042a0: 0072 9600 0000 72aa 0000 0072 c100 0000  .r....r....r....
-000042b0: 72b3 0000 0072 8f00 0000 72b4 0000 0072  r....r....r....r
-000042c0: c900 0000 72cb 0000 0072 cd00 0000 72ce  ....r....r....r.
-000042d0: 0000 0072 1e00 0000 72d2 0000 0072 a000  ...r....r....r..
-000042e0: 0000 72da 0000 0072 db00 0000 720f 0000  ..r....r....r...
-000042f0: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00004300: 726c 0000 00fa 0000 0073 4000 0000 0801  rl.......s@.....
-00004310: 0401 0404 0001 0001 0001 0001 0001 00f9  ................
-00004320: 0a27 0201 0a06 0a09 0804 0808 0820 0812  .'........... ..
-00004330: 0809 081d 0810 0a54 080b 0807 0a45 0804  .......T.....E..
-00004340: 0803 0803 0803 0803 0809 0804 0806 726c  ..............rl
-00004350: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00004360: 0000 0000 0200 0000 4000 0000 733c 0000  ........@...s<..
-00004370: 0065 005a 0164 005a 0264 015a 0364 015a  .e.Z.d.Z.d.Z.d.Z
-00004380: 0464 0264 0384 005a 0564 0464 0584 005a  .d.d...Z.d.d...Z
-00004390: 0664 0664 0784 005a 0764 0864 0984 005a  .d.d...Z.d.d...Z
-000043a0: 0864 0a64 0b84 005a 0964 0153 0029 0cda  .d.d...Z.d.S.)..
-000043b0: 0d43 6869 6c64 4150 494d 6978 696e 4e63  .ChildAPIMixinNc
-000043c0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000043d0: 0600 0000 4300 0000 7316 0000 0064 01a0  ....C...s....d..
-000043e0: 007c 006a 017c 006a 027c 017c 006a 03a1  .|.j.|.j.|.|.j..
-000043f0: 0453 0029 024e 7a0a 7b7d 7b7d 2f7b 7d2f  .S.).Nz.{}{}/{}/
-00004400: 7b7d 2904 7239 0000 0072 7800 0000 da0a  {}).r9...rx.....
-00004410: 5041 5245 4e54 5f41 5049 da09 4348 494c  PARENT_API..CHIL
-00004420: 445f 4150 4929 0272 4b00 0000 5a09 7061  D_API).rK...Z.pa
-00004430: 7265 6e74 5f69 6472 0f00 0000 720f 0000  rent_idr....r...
-00004440: 0072 1000 0000 da0d 6765 745f 6368 696c  .r......get_chil
-00004450: 645f 7572 6c82 0200 0073 0c00 0000 0001  d_url....s......
-00004460: 0401 0401 0401 0201 04fc 7a1b 4368 696c  ..........z.Chil
-00004470: 6441 5049 4d69 7869 6e2e 6765 745f 6368  dAPIMixin.get_ch
-00004480: 696c 645f 7572 6c63 0400 0000 0000 0000  ild_urlc........
-00004490: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
-000044a0: 7326 0000 007c 00a0 007c 026a 01a1 017d  s&...|...|.j...}
-000044b0: 047c 00a0 027c 017c 03a1 027d 057c 00a0  .|...|.|...}.|..
-000044c0: 0364 017c 047c 05a1 0353 0072 d300 0000  .d.|.|...S.r....
-000044d0: 2904 72e2 0000 0072 9100 0000 72aa 0000  ).r....r....r...
-000044e0: 0072 b400 0000 a906 724b 0000 0072 d600  .r......rK...r..
-000044f0: 0000 72dd 0000 0072 d700 0000 7240 0000  ..r....r....r@..
-00004500: 0072 9900 0000 720f 0000 0072 0f00 0000  .r....r....r....
-00004510: 7210 0000 0072 a000 0000 8a02 0000 7306  r....r........s.
-00004520: 0000 0000 020c 010c 017a 1443 6869 6c64  .........z.Child
-00004530: 4150 494d 6978 696e 2e75 7064 6174 6563  APIMixin.updatec
-00004540: 0300 0000 0000 0000 0000 0000 0700 0000  ................
-00004550: 0500 0000 4b00 0000 7330 0000 007c 00a0  ....K...s0...|..
-00004560: 007c 026a 01a1 017d 047c 00a0 027c 017c  .|.j...}.|...|.|
-00004570: 03a1 027d 057c 00a0 0364 017c 047c 05a1  ...}.|...d.|.|..
-00004580: 037d 067c 06a0 0464 02a1 0153 0072 d800  .}.|...d...S.r..
-00004590: 0000 2905 72e2 0000 0072 9100 0000 72aa  ..).r....r....r.
-000045a0: 0000 0072 b400 0000 721e 0000 0029 0772  ...r....r....).r
-000045b0: 4b00 0000 72d6 0000 0072 dd00 0000 72bb  K...r....r....r.
-000045c0: 0000 0072 4000 0000 7299 0000 0072 4100  ...r@...r....rA.
-000045d0: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-000045e0: 0072 da00 0000 9002 0000 7308 0000 0000  .r........s.....
-000045f0: 010c 010c 010e 017a 1443 6869 6c64 4150  .......z.ChildAP
-00004600: 494d 6978 696e 2e63 7265 6174 6563 0300  IMixin.createc..
-00004610: 0000 0000 0000 0000 0000 0500 0000 0500  ................
-00004620: 0000 4300 0000 7330 0000 0064 01a0 007c  ..C...s0...d...|
-00004630: 00a0 017c 026a 02a1 0174 037c 016a 0283  ...|.j...t.|.j..
-00004640: 01a1 027d 037c 00a0 0464 027c 03a1 027d  ...}.|...d.|...}
-00004650: 047c 04a0 0564 03a1 0153 0029 044e fa05  .|...d...S.).N..
-00004660: 7b7d 2f7b 7d72 db00 0000 72d9 0000 0029  {}/{}r....r....)
-00004670: 0672 3900 0000 72e2 0000 0072 9100 0000  .r9...r....r....
-00004680: 7290 0000 0072 b400 0000 721e 0000 0072  r....r....r....r
-00004690: dc00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-000046a0: 0000 0072 db00 0000 9602 0000 730c 0000  ...r........s...
-000046b0: 0000 0104 010a 0108 fe04 040c 027a 1443  .............z.C
-000046c0: 6869 6c64 4150 494d 6978 696e 2e64 656c  hildAPIMixin.del
-000046d0: 6574 6563 0200 0000 0000 0000 0000 0000  etec............
-000046e0: 0400 0000 0400 0000 4f00 0000 731a 0000  ........O...s...
-000046f0: 007c 006a 007c 0166 017c 029e 0264 0164  .|.j.|.f.|...d.d
-00004700: 0269 017c 0397 028e 0153 00a9 034e 7266  .i.|.....S...Nrf
-00004710: 0000 0072 5800 0000 72cf 0000 0072 d000  ...rX...r....r..
-00004720: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00004730: 0072 1e00 0000 a002 0000 7302 0000 0000  .r........s.....
-00004740: 017a 1143 6869 6c64 4150 494d 6978 696e  .z.ChildAPIMixin
-00004750: 2e67 6574 290a 720b 0000 0072 0c00 0000  .get).r....r....
-00004760: 720d 0000 0072 e000 0000 72e1 0000 0072  r....r....r....r
-00004770: e200 0000 72a0 0000 0072 da00 0000 72db  ....r....r....r.
-00004780: 0000 0072 1e00 0000 720f 0000 0072 0f00  ...r....r....r..
-00004790: 0000 720f 0000 0072 1000 0000 72df 0000  ..r....r....r...
-000047a0: 007e 0200 0073 0e00 0000 0801 0401 0402  .~...s..........
-000047b0: 0808 0806 0806 080a 72df 0000 0063 0000  ........r....c..
-000047c0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-000047d0: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
-000047e0: 005a 0264 015a 0364 0253 0029 03da 1143  .Z.d.Z.d.S.)...C
-000047f0: 6f6e 7461 6374 7341 5049 436c 6965 6e74  ontactsAPIClient
-00004800: 5a08 436f 6e74 6163 7473 4ea9 0472 0b00  Z.ContactsN..r..
-00004810: 0000 720c 0000 0072 0d00 0000 7271 0000  ..r....r....rq..
-00004820: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
-00004830: 7210 0000 0072 e600 0000 a402 0000 7302  r....r........s.
-00004840: 0000 0008 0172 e600 0000 6300 0000 0000  .....r....c.....
-00004850: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-00004860: 0000 0073 1000 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00004870: 6401 5a03 6402 5300 2903 da0e 526f 6c65  d.Z.d.S.)...Role
-00004880: 7341 5049 436c 6965 6e74 5a05 526f 6c65  sAPIClientZ.Role
-00004890: 734e 72e7 0000 0072 0f00 0000 720f 0000  sNr....r....r...
-000048a0: 0072 0f00 0000 7210 0000 0072 e800 0000  .r....r....r....
-000048b0: a802 0000 7302 0000 0008 0172 e800 0000  ....s......r....
-000048c0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000048d0: 0001 0000 0040 0000 0073 1000 0000 6500  .....@...s....e.
-000048e0: 5a01 6400 5a02 6401 5a03 6402 5300 2903  Z.d.Z.d.Z.d.S.).
-000048f0: da14 4465 7061 7274 6d65 6e74 7341 5049  ..DepartmentsAPI
-00004900: 436c 6965 6e74 5a0b 4465 7061 7274 6d65  ClientZ.Departme
-00004910: 6e74 734e 72e7 0000 0072 0f00 0000 720f  ntsNr....r....r.
-00004920: 0000 0072 0f00 0000 7210 0000 0072 e900  ...r....r....r..
-00004930: 0000 ac02 0000 7302 0000 0008 0172 e900  ......s......r..
-00004940: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00004950: 0000 0001 0000 0040 0000 0073 1000 0000  .......@...s....
-00004960: 6500 5a01 6400 5a02 6401 5a03 6402 5300  e.Z.d.Z.d.Z.d.S.
-00004970: 2903 da21 5265 736f 7572 6365 5365 7276  )..!ResourceServ
-00004980: 6963 6544 6573 6b52 6f6c 6573 4150 4943  iceDeskRolesAPIC
-00004990: 6c69 656e 745a 1852 6573 6f75 7263 6553  lientZ.ResourceS
-000049a0: 6572 7669 6365 4465 736b 526f 6c65 734e  erviceDeskRolesN
-000049b0: 72e7 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-000049c0: 0f00 0000 7210 0000 0072 ea00 0000 b002  ....r....r......
-000049d0: 0000 7302 0000 0008 0172 ea00 0000 6300  ..s......r....c.
-000049e0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-000049f0: 0000 0040 0000 0073 1000 0000 6500 5a01  ...@...s....e.Z.
-00004a00: 6400 5a02 6401 5a03 6402 5300 2903 da20  d.Z.d.Z.d.S.).. 
-00004a10: 5265 736f 7572 6365 526f 6c65 4465 7061  ResourceRoleDepa
-00004a20: 7274 6d65 6e74 7341 5049 436c 6965 6e74  rtmentsAPIClient
-00004a30: 5a17 5265 736f 7572 6365 526f 6c65 4465  Z.ResourceRoleDe
-00004a40: 7061 7274 6d65 6e74 734e 72e7 0000 0072  partmentsNr....r
-00004a50: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-00004a60: 0000 0072 eb00 0000 b402 0000 7302 0000  ...r........s...
-00004a70: 0008 0172 eb00 0000 6300 0000 0000 0000  ...r....c.......
-00004a80: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-00004a90: 0073 2000 0000 6500 5a01 6400 5a02 6401  .s ...e.Z.d.Z.d.
-00004aa0: 5a03 6402 6403 8400 5a04 6404 6405 8400  Z.d.d...Z.d.d...
-00004ab0: 5a05 6406 5300 2907 da10 5469 636b 6574  Z.d.S.)...Ticket
-00004ac0: 7341 5049 436c 6965 6e74 da07 5469 636b  sAPIClient..Tick
-00004ad0: 6574 7363 0200 0000 0000 0000 0000 0000  etsc............
-00004ae0: 0400 0000 0300 0000 4f00 0000 7312 0000  ........O...s...
-00004af0: 007c 006a 007c 0166 017c 029e 027c 038e  .|.j.|.f.|...|..
-00004b00: 0153 0072 2900 0000 72cf 0000 0072 d000  .S.r)...r....r..
-00004b10: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00004b20: 0072 ab00 0000 bb02 0000 7302 0000 0000  .r........s.....
-00004b30: 027a 1654 6963 6b65 7473 4150 4943 6c69  .z.TicketsAPICli
-00004b40: 656e 742e 636f 756e 7463 0300 0000 0000  ent.countc......
-00004b50: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
-00004b60: 0000 731e 0000 007c 00a0 007c 017c 02a1  ..s....|...|.|..
-00004b70: 027d 037c 00a0 0164 017c 00a0 02a1 007c  .}.|...d.|.....|
-00004b80: 03a1 0353 0072 d300 0000 a903 729b 0000  ...S.r......r...
-00004b90: 0072 b400 0000 727a 0000 0072 d500 0000  .r....rz...r....
-00004ba0: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00004bb0: a000 0000 bf02 0000 7304 0000 0000 030c  ........s.......
-00004bc0: 017a 1754 6963 6b65 7473 4150 4943 6c69  .z.TicketsAPICli
-00004bd0: 656e 742e 7570 6461 7465 4e29 0672 0b00  ent.updateN).r..
-00004be0: 0000 720c 0000 0072 0d00 0000 7271 0000  ..r....r....rq..
-00004bf0: 0072 ab00 0000 72a0 0000 0072 0f00 0000  .r....r....r....
-00004c00: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00004c10: ec00 0000 b802 0000 7306 0000 0008 0104  ........s.......
-00004c20: 0208 0472 ec00 0000 6300 0000 0000 0000  ...r....c.......
-00004c30: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-00004c40: 0073 1000 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00004c50: 5a03 6402 5300 2903 da15 4269 6c6c 696e  Z.d.S.)...Billin
-00004c60: 6743 6f64 6573 4150 4943 6c69 656e 74da  gCodesAPIClient.
-00004c70: 0c42 696c 6c69 6e67 436f 6465 734e 72e7  .BillingCodesNr.
-00004c80: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
-00004c90: 0000 7210 0000 0072 ef00 0000 c602 0000  ..r....r........
-00004ca0: 7302 0000 0008 0172 ef00 0000 6300 0000  s......r....c...
-00004cb0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00004cc0: 0040 0000 0073 1000 0000 6500 5a01 6400  .@...s....e.Z.d.
-00004cd0: 5a02 6401 5a03 6402 5300 2903 da12 436f  Z.d.Z.d.S.)...Co
-00004ce0: 6e74 7261 6374 7341 5049 436c 6965 6e74  ntractsAPIClient
-00004cf0: 5a09 436f 6e74 7261 6374 734e 72e7 0000  Z.ContractsNr...
-00004d00: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
-00004d10: 7210 0000 0072 f100 0000 ca02 0000 7302  r....r........s.
-00004d20: 0000 0008 0172 f100 0000 6300 0000 0000  .....r....c.....
-00004d30: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
-00004d40: 0000 0073 1800 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00004d50: 6401 5a03 6402 6403 8400 5a04 6404 5300  d.Z.d.d...Z.d.S.
-00004d60: 2905 da21 4163 636f 756e 7450 6879 7369  )..!AccountPhysi
-00004d70: 6361 6c4c 6f63 6174 696f 6e73 4150 4943  calLocationsAPIC
-00004d80: 6c69 656e 745a 1043 6f6d 7061 6e79 4c6f  lientZ.CompanyLo
-00004d90: 6361 7469 6f6e 7363 0200 0000 0000 0000  cationsc........
-00004da0: 0000 0000 0400 0000 0400 0000 4f00 0000  ............O...
-00004db0: 731a 0000 007c 006a 007c 0166 017c 029e  s....|.j.|.f.|..
-00004dc0: 0264 0164 0269 017c 0397 028e 0153 0072  .d.d.i.|.....S.r
-00004dd0: e500 0000 72cf 0000 0072 d000 0000 720f  ....r....r....r.
-00004de0: 0000 0072 0f00 0000 7210 0000 0072 1e00  ...r....r....r..
-00004df0: 0000 d202 0000 7302 0000 0000 017a 2541  ......s......z%A
-00004e00: 6363 6f75 6e74 5068 7973 6963 616c 4c6f  ccountPhysicalLo
-00004e10: 6361 7469 6f6e 7341 5049 436c 6965 6e74  cationsAPIClient
-00004e20: 2e67 6574 4ea9 0572 0b00 0000 720c 0000  .getN..r....r...
-00004e30: 0072 0d00 0000 7271 0000 0072 1e00 0000  .r....rq...r....
-00004e40: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00004e50: 1000 0000 72f2 0000 00ce 0200 0073 0400  ....r........s..
-00004e60: 0000 0801 0403 72f2 0000 0063 0000 0000  ......r....c....
-00004e70: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00004e80: 4000 0000 7320 0000 0065 005a 0164 005a  @...s ...e.Z.d.Z
-00004e90: 0264 015a 0364 025a 0465 035a 0564 0364  .d.Z.d.Z.e.Z.d.d
-00004ea0: 0484 005a 0664 0553 0029 06da 0e54 6173  ...Z.d.S.)...Tas
-00004eb0: 6b73 4150 4943 6c69 656e 74da 0554 6173  ksAPIClient..Tas
-00004ec0: 6b73 da08 5072 6f6a 6563 7473 6304 0000  ks..Projectsc...
-00004ed0: 0000 0000 0000 0000 0006 0000 0005 0000  ................
-00004ee0: 0043 0000 0073 2600 0000 7c00 a000 7c02  .C...s&...|...|.
-00004ef0: 6a01 a101 7d04 7c00 a002 7c01 7c03 a102  j...}.|...|.|...
-00004f00: 7d05 7c00 a003 6401 7c04 7c05 a103 5300  }.|...d.|.|...S.
-00004f10: 72d3 0000 0029 0472 e200 0000 7291 0000  r....).r....r...
-00004f20: 0072 9b00 0000 72b4 0000 0072 e300 0000  .r....r....r....
-00004f30: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00004f40: a000 0000 dc02 0000 7306 0000 0000 030c  ........s.......
-00004f50: 010c 017a 1554 6173 6b73 4150 4943 6c69  ...z.TasksAPICli
-00004f60: 656e 742e 7570 6461 7465 4e29 0772 0b00  ent.updateN).r..
-00004f70: 0000 720c 0000 0072 0d00 0000 7271 0000  ..r....r....rq..
-00004f80: 0072 e000 0000 72e1 0000 0072 a000 0000  .r....r....r....
-00004f90: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00004fa0: 1000 0000 72f4 0000 00d6 0200 0073 0800  ....r........s..
-00004fb0: 0000 0801 0401 0401 0403 72f4 0000 0063  ..........r....c
-00004fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004fd0: 0300 0000 0000 0000 7328 0000 0065 005a  ........s(...e.Z
-00004fe0: 0164 005a 0264 015a 0364 025a 0464 035a  .d.Z.d.Z.d.Z.d.Z
-00004ff0: 0587 0066 0164 0464 0584 085a 0687 0004  ...f.d.d...Z....
-00005000: 005a 0753 0029 06da 1454 6963 6b65 744e  .Z.S.)...TicketN
-00005010: 6f74 6573 4150 4943 6c69 656e 74da 0b54  otesAPIClient..T
-00005020: 6963 6b65 744e 6f74 6573 72ed 0000 005a  icketNotesr....Z
-00005030: 054e 6f74 6573 6302 0000 0000 0000 0000  .Notesc.........
-00005040: 0000 0004 0000 0003 0000 000b 0000 0073  ...............s
-00005050: 1c00 0000 7c02 a000 6401 a101 7d03 7401  ....|...d...}.t.
-00005060: 8300 6a02 7c01 7c03 6602 7c02 8e01 5300  ..j.|.|.f.|...S.
-00005070: a902 4eda 0674 6963 6b65 74a9 03da 0370  ..N..ticket....p
-00005080: 6f70 da05 7375 7065 7272 da00 0000 a904  op..superr......
-00005090: 724b 0000 0072 d600 0000 72bb 0000 0072  rK...r....r....r
-000050a0: dd00 0000 a901 7248 0000 0072 0f00 0000  ......rH...r....
-000050b0: 7210 0000 0072 da00 0000 e902 0000 7304  r....r........s.
-000050c0: 0000 0000 010a 017a 1b54 6963 6b65 744e  .......z.TicketN
-000050d0: 6f74 6573 4150 4943 6c69 656e 742e 6372  otesAPIClient.cr
-000050e0: 6561 7465 a908 720b 0000 0072 0c00 0000  eate..r....r....
-000050f0: 720d 0000 0072 7100 0000 72e0 0000 0072  r....rq...r....r
-00005100: e100 0000 72da 0000 00da 0d5f 5f63 6c61  ....r......__cla
-00005110: 7373 6365 6c6c 5f5f 720f 0000 0072 0f00  sscell__r....r..
-00005120: 0000 72ff 0000 0072 1000 0000 72f7 0000  ..r....r....r...
-00005130: 00e4 0200 0073 0800 0000 0801 0401 0401  .....s..........
-00005140: 0402 72f7 0000 0063 0000 0000 0000 0000  ..r....c........
-00005150: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-00005160: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00005170: 0364 0264 0384 005a 0464 0453 0029 05da  .d.d...Z.d.S.)..
-00005180: 1254 6173 6b4e 6f74 6573 4150 4943 6c69  .TaskNotesAPICli
-00005190: 656e 745a 0954 6173 6b4e 6f74 6573 6302  entZ.TaskNotesc.
-000051a0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-000051b0: 0000 004f 0000 0073 1a00 0000 7c00 6a00  ...O...s....|.j.
-000051c0: 7c01 6601 7c02 9e02 6401 6402 6901 7c03  |.f.|...d.d.i.|.
-000051d0: 9702 8e01 5300 72e5 0000 0072 cf00 0000  ....S.r....r....
-000051e0: 72d0 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-000051f0: 1000 0000 721e 0000 00f2 0200 0073 0200  ....r........s..
-00005200: 0000 0001 7a16 5461 736b 4e6f 7465 7341  ....z.TaskNotesA
-00005210: 5049 436c 6965 6e74 2e67 6574 4e72 f300  PIClient.getNr..
-00005220: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-00005230: 0072 1000 0000 7202 0100 00ee 0200 0073  .r....r........s
-00005240: 0400 0000 0801 0403 7202 0100 0063 0000  ........r....c..
-00005250: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00005260: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
-00005270: 005a 0264 015a 0364 0264 0384 005a 0464  .Z.d.Z.d.d...Z.d
-00005280: 0453 0029 05da 1454 696d 6545 6e74 7269  .S.)...TimeEntri
-00005290: 6573 4150 4943 6c69 656e 74da 0b54 696d  esAPIClient..Tim
-000052a0: 6545 6e74 7269 6573 6302 0000 0000 0000  eEntriesc.......
-000052b0: 0000 0000 0004 0000 0004 0000 004f 0000  .............O..
-000052c0: 0073 1a00 0000 7c00 6a00 7c01 6601 7c02  .s....|.j.|.f.|.
-000052d0: 9e02 6401 6402 6901 7c03 9702 8e01 5300  ..d.d.i.|.....S.
-000052e0: 72e5 0000 0072 cf00 0000 72d0 0000 0072  r....r....r....r
-000052f0: 0f00 0000 720f 0000 0072 1000 0000 721e  ....r....r....r.
-00005300: 0000 00fa 0200 0073 0200 0000 0001 7a18  .......s......z.
-00005310: 5469 6d65 456e 7472 6965 7341 5049 436c  TimeEntriesAPICl
-00005320: 6965 6e74 2e67 6574 4e72 f300 0000 720f  ient.getNr....r.
-00005330: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00005340: 0000 7203 0100 00f6 0200 0073 0400 0000  ..r........s....
-00005350: 0801 0403 7203 0100 0063 0000 0000 0000  ....r....c......
-00005360: 0000 0000 0000 0000 0000 0300 0000 0000  ................
-00005370: 0000 7328 0000 0065 005a 0164 005a 0264  ..s(...e.Z.d.Z.d
-00005380: 015a 0364 025a 0464 035a 0587 0066 0164  .Z.d.Z.d.Z...f.d
-00005390: 0464 0584 085a 0687 0004 005a 0753 0029  .d...Z.....Z.S.)
-000053a0: 06da 2154 6963 6b65 7453 6563 6f6e 6461  ..!TicketSeconda
-000053b0: 7279 5265 736f 7572 6365 7341 5049 436c  ryResourcesAPICl
-000053c0: 6965 6e74 5a18 5469 636b 6574 5365 636f  ientZ.TicketSeco
-000053d0: 6e64 6172 7952 6573 6f75 7263 6573 72ed  ndaryResourcesr.
-000053e0: 0000 00da 1253 6563 6f6e 6461 7279 5265  .....SecondaryRe
-000053f0: 736f 7572 6365 7363 0200 0000 0000 0000  sourcesc........
-00005400: 0000 0000 0400 0000 0300 0000 0b00 0000  ................
-00005410: 731c 0000 007c 02a0 0064 01a1 017d 0374  s....|...d...}.t
-00005420: 0183 006a 027c 017c 0366 027c 028e 0153  ...j.|.|.f.|...S
-00005430: 0072 f900 0000 72fb 0000 0072 fe00 0000  .r....r....r....
-00005440: 72ff 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00005450: da00 0000 0303 0000 7304 0000 0000 010a  ........s.......
-00005460: 017a 2854 6963 6b65 7453 6563 6f6e 6461  .z(TicketSeconda
-00005470: 7279 5265 736f 7572 6365 7341 5049 436c  ryResourcesAPICl
-00005480: 6965 6e74 2e63 7265 6174 6572 0001 0000  ient.creater....
-00005490: 720f 0000 0072 0f00 0000 72ff 0000 0072  r....r....r....r
-000054a0: 1000 0000 7205 0100 00fe 0200 0073 0800  ....r........s..
-000054b0: 0000 0801 0401 0401 0402 7205 0100 0063  ..........r....c
-000054c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000054d0: 0300 0000 0000 0000 7328 0000 0065 005a  ........s(...e.Z
-000054e0: 0164 005a 0264 015a 0364 025a 0464 035a  .d.Z.d.Z.d.Z.d.Z
-000054f0: 0587 0066 0164 0464 0584 085a 0687 0004  ...f.d.d...Z....
-00005500: 005a 0753 0029 06da 1f54 6173 6b53 6563  .Z.S.)...TaskSec
-00005510: 6f6e 6461 7279 5265 736f 7572 6365 7341  ondaryResourcesA
-00005520: 5049 436c 6965 6e74 5a16 5461 736b 5365  PIClientZ.TaskSe
-00005530: 636f 6e64 6172 7952 6573 6f75 7263 6573  condaryResources
-00005540: 72f5 0000 0072 0601 0000 6302 0000 0000  r....r....c.....
-00005550: 0000 0000 0000 0004 0000 0003 0000 000b  ................
-00005560: 0000 0073 1c00 0000 7c02 a000 6401 a101  ...s....|...d...
-00005570: 7d03 7401 8300 6a02 7c01 7c03 6602 7c02  }.t...j.|.|.f.|.
-00005580: 8e01 5300 2902 4eda 0474 6173 6b72 fb00  ..S.).N..taskr..
-00005590: 0000 72fe 0000 0072 ff00 0000 720f 0000  ..r....r....r...
-000055a0: 0072 1000 0000 72da 0000 000d 0300 0073  .r....r........s
-000055b0: 0400 0000 0001 0a01 7a26 5461 736b 5365  ........z&TaskSe
-000055c0: 636f 6e64 6172 7952 6573 6f75 7263 6573  condaryResources
-000055d0: 4150 4943 6c69 656e 742e 6372 6561 7465  APIClient.create
-000055e0: 7200 0100 0072 0f00 0000 720f 0000 0072  r....r....r....r
-000055f0: ff00 0000 7210 0000 0072 0701 0000 0803  ....r....r......
-00005600: 0000 7308 0000 0008 0104 0104 0104 0272  ..s............r
-00005610: 0701 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00005620: 0000 0000 0002 0000 0040 0000 0073 2000  .........@...s .
-00005630: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00005640: 6403 8400 5a04 6404 6405 8400 5a05 6406  d...Z.d.d...Z.d.
-00005650: 5300 2907 da11 5072 6f6a 6563 7473 4150  S.)...ProjectsAP
-00005660: 4943 6c69 656e 7472 f600 0000 6302 0000  IClientr....c...
-00005670: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00005680: 004f 0000 0073 1a00 0000 7c00 6a00 7c01  .O...s....|.j.|.
-00005690: 6601 7c02 9e02 6401 6402 6901 7c03 9702  f.|...d.d.i.|...
-000056a0: 8e01 5300 72e5 0000 0072 cf00 0000 72d0  ..S.r....r....r.
-000056b0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-000056c0: 0000 721e 0000 0016 0300 0073 0200 0000  ..r........s....
-000056d0: 0001 7a15 5072 6f6a 6563 7473 4150 4943  ..z.ProjectsAPIC
-000056e0: 6c69 656e 742e 6765 7463 0300 0000 0000  lient.getc......
-000056f0: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
-00005700: 0000 731e 0000 007c 00a0 007c 017c 02a1  ..s....|...|.|..
-00005710: 027d 037c 00a0 0164 017c 00a0 02a1 007c  .}.|...d.|.....|
-00005720: 03a1 0353 0072 d300 0000 72ee 0000 0072  ...S.r....r....r
-00005730: d500 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-00005740: 0000 0072 a000 0000 1903 0000 7304 0000  ...r........s...
-00005750: 0000 030c 017a 1850 726f 6a65 6374 7341  .....z.ProjectsA
-00005760: 5049 436c 6965 6e74 2e75 7064 6174 654e  PIClient.updateN
-00005770: 2906 720b 0000 0072 0c00 0000 720d 0000  ).r....r....r...
-00005780: 0072 7100 0000 721e 0000 0072 a000 0000  .rq...r....r....
-00005790: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-000057a0: 1000 0000 7209 0100 0012 0300 0073 0600  ....r........s..
-000057b0: 0000 0801 0403 0803 7209 0100 0063 0000  ........r....c..
-000057c0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-000057d0: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
-000057e0: 005a 0264 015a 0364 0253 0029 03da 1954  .Z.d.Z.d.S.)...T
-000057f0: 6963 6b65 7443 6174 6567 6f72 6965 7341  icketCategoriesA
-00005800: 5049 436c 6965 6e74 da10 5469 636b 6574  PIClient..Ticket
-00005810: 4361 7465 676f 7269 6573 4e72 e700 0000  CategoriesNr....
-00005820: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00005830: 1000 0000 720a 0100 0020 0300 0073 0200  ....r.... ...s..
-00005840: 0000 0801 720a 0100 0063 0000 0000 0000  ....r....c......
-00005850: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00005860: 0000 7318 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00005870: 015a 0364 0264 0384 005a 0464 0453 0029  .Z.d.d...Z.d.S.)
-00005880: 05da 1954 6173 6b50 7265 6465 6365 7373  ...TaskPredecess
-00005890: 6f72 7341 5049 436c 6965 6e74 5a10 5461  orsAPIClientZ.Ta
-000058a0: 736b 5072 6564 6563 6573 736f 7273 6302  skPredecessorsc.
-000058b0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-000058c0: 0000 004f 0000 0073 1a00 0000 7c00 6a00  ...O...s....|.j.
-000058d0: 7c01 6601 7c02 9e02 6401 6402 6901 7c03  |.f.|...d.d.i.|.
-000058e0: 9702 8e01 5300 72e5 0000 0072 cf00 0000  ....S.r....r....
-000058f0: 72d0 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00005900: 1000 0000 721e 0000 0028 0300 0073 0200  ....r....(...s..
-00005910: 0000 0001 7a1d 5461 736b 5072 6564 6563  ....z.TaskPredec
-00005920: 6573 736f 7273 4150 4943 6c69 656e 742e  essorsAPIClient.
-00005930: 6765 744e 72f3 0000 0072 0f00 0000 720f  getNr....r....r.
-00005940: 0000 0072 0f00 0000 7210 0000 0072 0c01  ...r....r....r..
-00005950: 0000 2403 0000 7304 0000 0008 0104 0372  ..$...s........r
-00005960: 0c01 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00005970: 0000 0000 0002 0000 0040 0000 0073 1800  .........@...s..
-00005980: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00005990: 6403 8400 5a04 6404 5300 2905 da15 5365  d...Z.d.S.)...Se
-000059a0: 7276 6963 6543 616c 6c73 4150 4943 6c69  rviceCallsAPICli
-000059b0: 656e 74da 0c53 6572 7669 6365 4361 6c6c  ent..ServiceCall
-000059c0: 7363 0200 0000 0000 0000 0000 0000 0400  sc..............
-000059d0: 0000 0400 0000 4f00 0000 731a 0000 007c  ......O...s....|
-000059e0: 006a 007c 0166 017c 029e 0264 0164 0269  .j.|.f.|...d.d.i
-000059f0: 017c 0397 028e 0153 0072 e500 0000 72cf  .|.....S.r....r.
-00005a00: 0000 0072 d000 0000 720f 0000 0072 0f00  ...r....r....r..
-00005a10: 0000 7210 0000 0072 1e00 0000 3003 0000  ..r....r....0...
-00005a20: 7302 0000 0000 017a 1953 6572 7669 6365  s......z.Service
-00005a30: 4361 6c6c 7341 5049 436c 6965 6e74 2e67  CallsAPIClient.g
-00005a40: 6574 4e72 f300 0000 720f 0000 0072 0f00  etNr....r....r..
-00005a50: 0000 720f 0000 0072 1000 0000 720d 0100  ..r....r....r...
-00005a60: 002c 0300 0073 0400 0000 0801 0403 720d  .,...s........r.
-00005a70: 0100 0063 0000 0000 0000 0000 0000 0000  ...c............
-00005a80: 0000 0000 0300 0000 0000 0000 7328 0000  ............s(..
-00005a90: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
-00005aa0: 0464 035a 0587 0066 0164 0464 0584 085a  .d.Z...f.d.d...Z
-00005ab0: 0687 0004 005a 0753 0029 06da 1b53 6572  .....Z.S.)...Ser
-00005ac0: 7669 6365 4361 6c6c 5469 636b 6574 7341  viceCallTicketsA
-00005ad0: 5049 436c 6965 6e74 da12 5365 7276 6963  PIClient..Servic
-00005ae0: 6543 616c 6c54 6963 6b65 7473 720e 0100  eCallTicketsr...
-00005af0: 0072 ed00 0000 6302 0000 0000 0000 0000  .r....c.........
-00005b00: 0000 0004 0000 0003 0000 000b 0000 0073  ...............s
-00005b10: 1c00 0000 7c02 a000 6401 a101 7d03 7401  ....|...d...}.t.
-00005b20: 8300 6a02 7c01 7c03 6602 7c02 8e01 5300  ..j.|.|.f.|...S.
-00005b30: a902 4eda 0c73 6572 7669 6365 5f63 616c  ..N..service_cal
-00005b40: 6c72 fb00 0000 72fe 0000 0072 ff00 0000  lr....r....r....
-00005b50: 720f 0000 0072 1000 0000 72da 0000 0039  r....r....r....9
-00005b60: 0300 0073 0400 0000 0001 0a01 7a22 5365  ...s........z"Se
-00005b70: 7276 6963 6543 616c 6c54 6963 6b65 7473  rviceCallTickets
-00005b80: 4150 4943 6c69 656e 742e 6372 6561 7465  APIClient.create
-00005b90: 7200 0100 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00005ba0: ff00 0000 7210 0000 0072 0f01 0000 3403  ....r....r....4.
-00005bb0: 0000 7308 0000 0008 0104 0104 0104 0272  ..s............r
-00005bc0: 0f01 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00005bd0: 0000 0000 0003 0000 0000 0000 0073 2800  .............s(.
-00005be0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00005bf0: 5a04 6403 5a05 8700 6601 6404 6405 8408  Z.d.Z...f.d.d...
-00005c00: 5a06 8700 0400 5a07 5300 2906 da23 5365  Z.....Z.S.)..#Se
-00005c10: 7276 6963 6543 616c 6c54 6963 6b65 7452  rviceCallTicketR
-00005c20: 6573 6f75 7263 6573 4150 4943 6c69 656e  esourcesAPIClien
-00005c30: 745a 1a53 6572 7669 6365 4361 6c6c 5469  tZ.ServiceCallTi
-00005c40: 636b 6574 5265 736f 7572 6365 7372 1001  cketResourcesr..
-00005c50: 0000 da09 5265 736f 7572 6365 7363 0200  ....Resourcesc..
-00005c60: 0000 0000 0000 0000 0000 0400 0000 0300  ................
-00005c70: 0000 0b00 0000 731c 0000 007c 02a0 0064  ......s....|...d
-00005c80: 01a1 017d 0374 0183 006a 027c 017c 0366  ...}.t...j.|.|.f
-00005c90: 027c 028e 0153 0029 024e da13 7365 7276  .|...S.).N..serv
-00005ca0: 6963 655f 6361 6c6c 5f74 6963 6b65 7472  ice_call_ticketr
-00005cb0: fb00 0000 72fe 0000 0072 ff00 0000 720f  ....r....r....r.
-00005cc0: 0000 0072 1000 0000 72da 0000 0043 0300  ...r....r....C..
-00005cd0: 0073 0400 0000 0001 0a01 7a2a 5365 7276  .s........z*Serv
-00005ce0: 6963 6543 616c 6c54 6963 6b65 7452 6573  iceCallTicketRes
-00005cf0: 6f75 7263 6573 4150 4943 6c69 656e 742e  ourcesAPIClient.
-00005d00: 6372 6561 7465 7200 0100 0072 0f00 0000  creater....r....
-00005d10: 720f 0000 0072 ff00 0000 7210 0000 0072  r....r....r....r
-00005d20: 1301 0000 3e03 0000 7308 0000 0008 0104  ....>...s.......
-00005d30: 0104 0104 0272 1301 0000 6300 0000 0000  .....r....c.....
-00005d40: 0000 0000 0000 0000 0000 0003 0000 0000  ................
-00005d50: 0000 0073 2800 0000 6500 5a01 6400 5a02  ...s(...e.Z.d.Z.
-00005d60: 6401 5a03 6402 5a04 6403 5a05 8700 6601  d.Z.d.Z.d.Z...f.
-00005d70: 6404 6405 8408 5a06 8700 0400 5a07 5300  d.d...Z.....Z.S.
-00005d80: 2906 da19 5365 7276 6963 6543 616c 6c54  )...ServiceCallT
-00005d90: 6173 6b73 4150 4943 6c69 656e 74da 1053  asksAPIClient..S
-00005da0: 6572 7669 6365 4361 6c6c 5461 736b 7372  erviceCallTasksr
-00005db0: 0e01 0000 72f5 0000 0063 0200 0000 0000  ....r....c......
-00005dc0: 0000 0000 0000 0400 0000 0300 0000 0b00  ................
-00005dd0: 0000 731c 0000 007c 02a0 0064 01a1 017d  ..s....|...d...}
-00005de0: 0374 0183 006a 027c 017c 0366 027c 028e  .t...j.|.|.f.|..
-00005df0: 0153 0072 1101 0000 72fb 0000 0072 fe00  .S.r....r....r..
-00005e00: 0000 72ff 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00005e10: 0072 da00 0000 4d03 0000 7304 0000 0000  .r....M...s.....
-00005e20: 010a 017a 2053 6572 7669 6365 4361 6c6c  ...z ServiceCall
-00005e30: 5461 736b 7341 5049 436c 6965 6e74 2e63  TasksAPIClient.c
-00005e40: 7265 6174 6572 0001 0000 720f 0000 0072  reater....r....r
-00005e50: 0f00 0000 72ff 0000 0072 1000 0000 7216  ....r....r....r.
-00005e60: 0100 0048 0300 0073 0800 0000 0801 0401  ...H...s........
-00005e70: 0401 0402 7216 0100 0063 0000 0000 0000  ....r....c......
-00005e80: 0000 0000 0000 0000 0000 0300 0000 0000  ................
-00005e90: 0000 7328 0000 0065 005a 0164 005a 0264  ..s(...e.Z.d.Z.d
-00005ea0: 015a 0364 025a 0464 035a 0587 0066 0164  .Z.d.Z.d.Z...f.d
-00005eb0: 0464 0584 085a 0687 0004 005a 0753 0029  .d...Z.....Z.S.)
-00005ec0: 06da 2153 6572 7669 6365 4361 6c6c 5461  ..!ServiceCallTa
-00005ed0: 736b 5265 736f 7572 6365 7341 5049 436c  skResourcesAPICl
-00005ee0: 6965 6e74 5a18 5365 7276 6963 6543 616c  ientZ.ServiceCal
-00005ef0: 6c54 6173 6b52 6573 6f75 7263 6573 7217  lTaskResourcesr.
-00005f00: 0100 0072 1401 0000 6302 0000 0000 0000  ...r....c.......
-00005f10: 0000 0000 0004 0000 0003 0000 000b 0000  ................
-00005f20: 0073 1c00 0000 7c02 a000 6401 a101 7d03  .s....|...d...}.
-00005f30: 7401 8300 6a02 7c01 7c03 6602 7c02 8e01  t...j.|.|.f.|...
-00005f40: 5300 2902 4eda 1173 6572 7669 6365 5f63  S.).N..service_c
-00005f50: 616c 6c5f 7461 736b 72fb 0000 0072 fe00  all_taskr....r..
-00005f60: 0000 72ff 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00005f70: 0072 da00 0000 5703 0000 7304 0000 0000  .r....W...s.....
-00005f80: 010a 017a 2853 6572 7669 6365 4361 6c6c  ...z(ServiceCall
-00005f90: 5461 736b 5265 736f 7572 6365 7341 5049  TaskResourcesAPI
-00005fa0: 436c 6965 6e74 2e63 7265 6174 6572 0001  Client.creater..
-00005fb0: 0000 720f 0000 0072 0f00 0000 72ff 0000  ..r....r....r...
-00005fc0: 0072 1000 0000 7218 0100 0052 0300 0073  .r....r....R...s
-00005fd0: 0800 0000 0801 0401 0401 0402 7218 0100  ............r...
-00005fe0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00005ff0: 0000 0100 0000 4000 0000 7310 0000 0065  ......@...s....e
-00006000: 005a 0164 005a 0264 015a 0364 0253 0029  .Z.d.Z.d.Z.d.S.)
-00006010: 03da 1252 6573 6f75 7263 6573 4150 4943  ...ResourcesAPIC
-00006020: 6c69 656e 7472 1401 0000 4e72 e700 0000  lientr....Nr....
-00006030: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00006040: 1000 0000 721a 0100 005c 0300 0073 0200  ....r....\...s..
-00006050: 0000 0801 721a 0100 0063 0000 0000 0000  ....r....c......
-00006060: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-00006070: 0000 7310 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00006080: 015a 0364 0253 0029 03da 1141 6363 6f75  .Z.d.S.)...Accou
-00006090: 6e74 7341 5049 436c 6965 6e74 da09 436f  ntsAPIClient..Co
-000060a0: 6d70 616e 6965 734e 72e7 0000 0072 0f00  mpaniesNr....r..
-000060b0: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-000060c0: 0072 1b01 0000 6003 0000 7302 0000 0008  .r....`...s.....
-000060d0: 0172 1b01 0000 6300 0000 0000 0000 0000  .r....c.........
-000060e0: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
-000060f0: 1000 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-00006100: 6402 5300 2903 da0f 5068 6173 6573 4150  d.S.)...PhasesAP
-00006110: 4943 6c69 656e 745a 0650 6861 7365 734e  IClientZ.PhasesN
-00006120: 72e7 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00006130: 0f00 0000 7210 0000 0072 1d01 0000 6403  ....r....r....d.
-00006140: 0000 7302 0000 0008 0172 1d01 0000 6300  ..s......r....c.
-00006150: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00006160: 0000 0040 0000 0073 1600 0000 6500 5a01  ...@...s....e.Z.
-00006170: 6400 5a02 6404 6402 6403 8401 5a03 6401  d.Z.d.d.d...Z.d.
-00006180: 5300 2905 da0c 5544 4641 5049 436c 6965  S.)...UDFAPIClie
-00006190: 6e74 4e63 0200 0000 0000 0000 0000 0000  ntNc............
-000061a0: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
-000061b0: 0064 01a0 007c 006a 017c 006a 02a1 0253  .d...|.j.|.j...S
-000061c0: 0029 024e 7a2a 7b30 7d7b 317d 2f65 6e74  .).Nz*{0}{1}/ent
-000061d0: 6974 7949 6e66 6f72 6d61 7469 6f6e 2f75  ityInformation/u
-000061e0: 7365 7244 6566 696e 6564 4669 656c 6473  serDefinedFields
-000061f0: 2903 7239 0000 0072 7800 0000 7271 0000  ).r9...rx...rq..
-00006200: 0072 7900 0000 720f 0000 0072 0f00 0000  .ry...r....r....
-00006210: 7210 0000 0072 7a00 0000 6a03 0000 7308  r....rz...j...s.
-00006220: 0000 0000 0104 0104 0104 fe7a 1855 4446  ...........z.UDF
-00006230: 4150 4943 6c69 656e 742e 6765 745f 6170  APIClient.get_ap
-00006240: 695f 7572 6c29 014e 2904 720b 0000 0072  i_url).N).r....r
-00006250: 0c00 0000 720d 0000 0072 7a00 0000 720f  ....r....rz...r.
-00006260: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00006270: 0000 721e 0100 0068 0300 0073 0200 0000  ..r....h...s....
-00006280: 0802 721e 0100 0063 0000 0000 0000 0000  ..r....c........
-00006290: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-000062a0: 7310 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-000062b0: 0364 0253 0029 03da 1354 6963 6b65 7473  .d.S.)...Tickets
-000062c0: 5544 4641 5049 436c 6965 6e74 72ed 0000  UDFAPIClientr...
-000062d0: 004e 72e7 0000 0072 0f00 0000 720f 0000  .Nr....r....r...
-000062e0: 0072 0f00 0000 7210 0000 0072 1f01 0000  .r....r....r....
-000062f0: 7103 0000 7302 0000 0008 0172 1f01 0000  q...s......r....
-00006300: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00006310: 0001 0000 0040 0000 0073 1000 0000 6500  .....@...s....e.
-00006320: 5a01 6400 5a02 6401 5a03 6402 5300 2903  Z.d.Z.d.Z.d.S.).
-00006330: da11 5461 736b 7355 4446 4150 4943 6c69  ..TasksUDFAPICli
-00006340: 656e 7472 f500 0000 4e72 e700 0000 720f  entr....Nr....r.
-00006350: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00006360: 0000 7220 0100 0075 0300 0073 0200 0000  ..r ...u...s....
-00006370: 0801 7220 0100 0063 0000 0000 0000 0000  ..r ...c........
-00006380: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00006390: 7310 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-000063a0: 0364 0253 0029 03da 1450 726f 6a65 6374  .d.S.)...Project
-000063b0: 7355 4446 4150 4943 6c69 656e 7472 f600  sUDFAPIClientr..
-000063c0: 0000 4e72 e700 0000 720f 0000 0072 0f00  ..Nr....r....r..
-000063d0: 0000 720f 0000 0072 1000 0000 7221 0100  ..r....r....r!..
-000063e0: 0079 0300 0073 0200 0000 0801 7221 0100  .y...s......r!..
-000063f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00006400: 0000 0300 0000 0000 0000 7324 0000 0065  ..........s$...e
-00006410: 005a 0164 005a 0287 0066 0164 0164 0284  .Z.d.Z...f.d.d..
-00006420: 085a 0364 0364 0484 005a 0487 0004 005a  .Z.d.d...Z.....Z
-00006430: 0553 0029 05da 1941 7574 6f74 6173 6b50  .S.)...AutotaskP
-00006440: 6963 6b6c 6973 7441 5049 436c 6965 6e74  icklistAPIClient
-00006450: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00006460: 0003 0000 000b 0000 0073 2000 0000 6401  .........s ...d.
-00006470: a000 7c00 6a01 a101 7c00 5f02 7403 8300  ..|.j...|._.t...
-00006480: 6a04 6600 7c01 8e01 0100 6400 5300 2902  j.f.|.....d.S.).
-00006490: 4e7a 1b7b 7d2f 656e 7469 7479 496e 666f  Nz.{}/entityInfo
-000064a0: 726d 6174 696f 6e2f 6669 656c 6473 2905  rmation/fields).
-000064b0: 7239 0000 00da 0a41 5049 5f45 4e54 4954  r9.....API_ENTIT
-000064c0: 5972 7100 0000 72fd 0000 0072 4d00 0000  Yrq...r....rM...
-000064d0: 2902 724b 0000 0072 bb00 0000 72ff 0000  ).rK...r....r...
-000064e0: 0072 0f00 0000 7210 0000 0072 4d00 0000  .r....r....rM...
-000064f0: 7f03 0000 7304 0000 0000 010e 017a 2241  ....s........z"A
-00006500: 7574 6f74 6173 6b50 6963 6b6c 6973 7441  utotaskPicklistA
-00006510: 5049 436c 6965 6e74 2e5f 5f69 6e69 745f  PIClient.__init_
-00006520: 5f63 0200 0000 0000 0000 0000 0000 0400  _c..............
-00006530: 0000 0300 0000 4f00 0000 731a 0000 007c  ......O...s....|
-00006540: 006a 007c 0170 0e7c 00a0 01a1 0066 017c  .j.|.p.|.....f.|
-00006550: 029e 027c 038e 0153 0072 2900 0000 2902  ...|...S.r)...).
-00006560: 72c1 0000 0072 7a00 0000 72d0 0000 0072  r....rz...r....r
-00006570: 0f00 0000 720f 0000 0072 1000 0000 721e  ....r....r....r.
-00006580: 0000 0083 0300 0073 0e00 0000 0003 0401  .......s........
-00006590: 0aff 0201 02ff 0201 02ff 7a1d 4175 746f  ..........z.Auto
-000065a0: 7461 736b 5069 636b 6c69 7374 4150 4943  taskPicklistAPIC
-000065b0: 6c69 656e 742e 6765 7429 0672 0b00 0000  lient.get).r....
-000065c0: 720c 0000 0072 0d00 0000 724d 0000 0072  r....r....rM...r
-000065d0: 1e00 0000 7201 0100 0072 0f00 0000 720f  ....r....r....r.
-000065e0: 0000 0072 ff00 0000 7210 0000 0072 2201  ...r....r....r".
-000065f0: 0000 7d03 0000 7304 0000 0008 020c 0472  ..}...s........r
-00006600: 2201 0000 6300 0000 0000 0000 0000 0000  "...c...........
-00006610: 0000 0000 0001 0000 0040 0000 0073 1000  .........@...s..
-00006620: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00006630: 5300 2903 da12 4e6f 7465 5479 7065 7341  S.)...NoteTypesA
-00006640: 5049 436c 6965 6e74 72f8 0000 004e a904  PIClientr....N..
-00006650: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-00006660: 2301 0000 720f 0000 0072 0f00 0000 720f  #...r....r....r.
-00006670: 0000 0072 1000 0000 7224 0100 008a 0300  ...r....r$......
-00006680: 0073 0200 0000 0801 7224 0100 0063 0000  .s......r$...c..
-00006690: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-000066a0: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
-000066b0: 005a 0264 015a 0364 0253 0029 03da 154c  .Z.d.Z.d.S.)...L
-000066c0: 6963 656e 7365 5479 7065 7341 5049 436c  icenseTypesAPICl
-000066d0: 6965 6e74 7214 0100 004e 7225 0100 0072  ientr....Nr%...r
-000066e0: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-000066f0: 0000 0072 2601 0000 8e03 0000 7302 0000  ...r&.......s...
-00006700: 0008 0172 2601 0000 6300 0000 0000 0000  ...r&...c.......
-00006710: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-00006720: 0073 1000 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00006730: 5a03 6402 5300 2903 da11 5573 6554 7970  Z.d.S.)...UseTyp
-00006740: 6573 4150 4943 6c69 656e 7472 f000 0000  esAPIClientr....
-00006750: 4e72 2501 0000 720f 0000 0072 0f00 0000  Nr%...r....r....
-00006760: 720f 0000 0072 1000 0000 7227 0100 0092  r....r....r'....
-00006770: 0300 0073 0200 0000 0801 7227 0100 0063  ...s......r'...c
-00006780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006790: 0100 0000 4000 0000 7310 0000 0065 005a  ....@...s....e.Z
-000067a0: 0164 005a 0264 015a 0364 0253 0029 03da  .d.Z.d.Z.d.S.)..
-000067b0: 1842 696c 6c69 6e67 436f 6465 5479 7065  .BillingCodeType
-000067c0: 4150 4943 6c69 656e 7472 f000 0000 4e72  APIClientr....Nr
-000067d0: 2501 0000 720f 0000 0072 0f00 0000 720f  %...r....r....r.
-000067e0: 0000 0072 1000 0000 7228 0100 0096 0300  ...r....r(......
-000067f0: 0073 0200 0000 0801 7228 0100 0063 0000  .s......r(...c..
-00006800: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-00006810: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
-00006820: 005a 0264 015a 0364 0253 0029 03da 1654  .Z.d.Z.d.S.)...T
-00006830: 6173 6b54 7970 654c 696e 6b73 4150 4943  askTypeLinksAPIC
-00006840: 6c69 656e 7472 0401 0000 4e72 2501 0000  lientr....Nr%...
-00006850: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00006860: 1000 0000 7229 0100 009a 0300 0073 0200  ....r).......s..
-00006870: 0000 0801 7229 0100 0063 0000 0000 0000  ....r)...c......
-00006880: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-00006890: 0000 7310 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-000068a0: 015a 0364 0253 0029 03da 1541 6363 6f75  .Z.d.S.)...Accou
-000068b0: 6e74 5479 7065 7341 5049 436c 6965 6e74  ntTypesAPIClient
-000068c0: 721c 0100 004e 7225 0100 0072 0f00 0000  r....Nr%...r....
-000068d0: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-000068e0: 2a01 0000 9e03 0000 7302 0000 0008 0172  *.......s......r
-000068f0: 2a01 0000 6300 0000 0000 0000 0000 0000  *...c...........
-00006900: 0000 0000 0001 0000 0040 0000 0073 1000  .........@...s..
-00006910: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00006920: 5300 2903 da1f 5469 636b 6574 4361 7465  S.)...TicketCate
-00006930: 676f 7279 5069 636b 6c69 7374 4150 4943  goryPicklistAPIC
-00006940: 6c69 656e 7472 0b01 0000 4e72 2501 0000  lientr....Nr%...
-00006950: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00006960: 1000 0000 722b 0100 00a2 0300 0073 0200  ....r+.......s..
-00006970: 0000 0801 722b 0100 0063 0000 0000 0000  ....r+...c......
-00006980: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-00006990: 0000 7310 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-000069a0: 015a 0364 0253 0029 03da 2253 6572 7669  .Z.d.S.).."Servi
-000069b0: 6365 4361 6c6c 5374 6174 7573 5069 636b  ceCallStatusPick
-000069c0: 6c69 7374 4150 4943 6c69 656e 7472 0e01  listAPIClientr..
-000069d0: 0000 4e72 2501 0000 720f 0000 0072 0f00  ..Nr%...r....r..
-000069e0: 0000 720f 0000 0072 1000 0000 722c 0100  ..r....r....r,..
-000069f0: 00a6 0300 0073 0200 0000 0801 722c 0100  .....s......r,..
-00006a00: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00006a10: 0000 0100 0000 4000 0000 7310 0000 0065  ......@...s....e
-00006a20: 005a 0164 005a 0264 015a 0364 0253 0029  .Z.d.Z.d.Z.d.S.)
-00006a30: 03da 1754 6963 6b65 7450 6963 6b6c 6973  ...TicketPicklis
-00006a40: 7441 5049 436c 6965 6e74 72ed 0000 004e  tAPIClientr....N
-00006a50: 7225 0100 0072 0f00 0000 720f 0000 0072  r%...r....r....r
-00006a60: 0f00 0000 7210 0000 0072 2d01 0000 aa03  ....r....r-.....
-00006a70: 0000 7302 0000 0008 0172 2d01 0000 6300  ..s......r-...c.
-00006a80: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00006a90: 0000 0040 0000 0073 1000 0000 6500 5a01  ...@...s....e.Z.
-00006aa0: 6400 5a02 6401 5a03 6402 5300 2903 da15  d.Z.d.Z.d.S.)...
-00006ab0: 5461 736b 5069 636b 6c69 7374 4150 4943  TaskPicklistAPIC
-00006ac0: 6c69 656e 7472 f500 0000 4e72 2501 0000  lientr....Nr%...
-00006ad0: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00006ae0: 1000 0000 722e 0100 00ae 0300 0073 0200  ....r........s..
-00006af0: 0000 0801 722e 0100 0063 0000 0000 0000  ....r....c......
-00006b00: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-00006b10: 0000 7310 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00006b20: 015a 0364 0253 0029 03da 1850 726f 6a65  .Z.d.S.)...Proje
-00006b30: 6374 5069 636b 6c69 7374 4150 4943 6c69  ctPicklistAPICli
-00006b40: 656e 7472 f600 0000 4e72 2501 0000 720f  entr....Nr%...r.
-00006b50: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00006b60: 0000 722f 0100 00b2 0300 0073 0200 0000  ..r/.......s....
-00006b70: 0801 722f 0100 0063 0000 0000 0000 0000  ..r/...c........
-00006b80: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-00006b90: 7338 0000 0065 005a 0164 005a 0264 015a  s8...e.Z.d.Z.d.Z
-00006ba0: 0364 025a 0464 035a 0564 0464 0584 005a  .d.Z.d.Z.d.d...Z
-00006bb0: 0664 0664 0784 005a 0764 0864 0984 005a  .d.d...Z.d.d...Z
-00006bc0: 0864 0a64 0b84 005a 0964 0c53 0029 0dda  .d.d...Z.d.S.)..
-00006bd0: 1d54 6963 6b65 7443 6865 636b 6c69 7374  .TicketChecklist
-00006be0: 4974 656d 7341 5049 436c 6965 6e74 5a14  ItemsAPIClientZ.
-00006bf0: 5469 636b 6574 4368 6563 6b6c 6973 7449  TicketChecklistI
-00006c00: 7465 6d73 72ed 0000 005a 0e43 6865 636b  temsr....Z.Check
-00006c10: 6c69 7374 4974 656d 7363 0200 0000 0000  listItemsc......
-00006c20: 0000 0000 0000 0400 0000 0300 0000 4f00  ..............O.
-00006c30: 0000 7312 0000 007c 006a 007c 0166 017c  ..s....|.j.|.f.|
-00006c40: 029e 027c 038e 0153 0072 2900 0000 72cf  ...|...S.r)...r.
-00006c50: 0000 0072 d000 0000 720f 0000 0072 0f00  ...r....r....r..
-00006c60: 0000 7210 0000 0072 1e00 0000 bb03 0000  ..r....r........
-00006c70: 7302 0000 0000 017a 2154 6963 6b65 7443  s......z!TicketC
-00006c80: 6865 636b 6c69 7374 4974 656d 7341 5049  hecklistItemsAPI
-00006c90: 436c 6965 6e74 2e67 6574 6302 0000 0000  Client.getc.....
-00006ca0: 0000 0000 0000 0004 0000 0005 0000 004b  ...............K
-00006cb0: 0000 0073 1800 0000 7c00 a000 7c01 a101  ...s....|...|...
-00006cc0: 7d03 7c00 a001 6401 7c03 7c02 a103 5300  }.|...d.|.|...S.
-00006cd0: 72d3 0000 00a9 0272 e200 0000 72b4 0000  r......r....r...
-00006ce0: 00a9 0472 4b00 0000 72dd 0000 0072 bb00  ...rK...r....r..
-00006cf0: 0000 7240 0000 0072 0f00 0000 720f 0000  ..r@...r....r...
-00006d00: 0072 1000 0000 72a0 0000 00be 0300 0073  .r....r........s
-00006d10: 0400 0000 0001 0a01 7a24 5469 636b 6574  ........z$Ticket
-00006d20: 4368 6563 6b6c 6973 7449 7465 6d73 4150  ChecklistItemsAP
-00006d30: 4943 6c69 656e 742e 7570 6461 7465 6302  IClient.updatec.
-00006d40: 0000 0000 0000 0000 0000 0004 0000 0005  ................
-00006d50: 0000 004b 0000 0073 1800 0000 7c00 a000  ...K...s....|...
-00006d60: 7c01 a101 7d03 7c00 a001 6401 7c03 7c02  |...}.|...d.|.|.
-00006d70: a103 5300 2902 4e72 5800 0000 7231 0100  ..S.).NrX...r1..
-00006d80: 0072 3201 0000 720f 0000 0072 0f00 0000  .r2...r....r....
-00006d90: 7210 0000 0072 da00 0000 c203 0000 7304  r....r........s.
-00006da0: 0000 0000 010a 017a 2454 6963 6b65 7443  .......z$TicketC
-00006db0: 6865 636b 6c69 7374 4974 656d 7341 5049  hecklistItemsAPI
-00006dc0: 436c 6965 6e74 2e63 7265 6174 6563 0200  Client.createc..
-00006dd0: 0000 0000 0000 0000 0000 0400 0000 0600  ................
-00006de0: 0000 4b00 0000 7324 0000 0064 01a0 007c  ..K...s$...d...|
-00006df0: 00a0 017c 01a1 017c 02a0 0264 02a1 01a1  ...|...|...d....
-00006e00: 027d 037c 00a0 0364 037c 03a1 0253 0029  .}.|...d.|...S.)
-00006e10: 044e 72e4 0000 0072 9100 0000 72db 0000  .Nr....r....r...
-00006e20: 0029 0472 3900 0000 72e2 0000 0072 1e00  .).r9...r....r..
-00006e30: 0000 72b4 0000 0072 3201 0000 720f 0000  ..r....r2...r...
-00006e40: 0072 0f00 0000 7210 0000 0072 db00 0000  .r....r....r....
-00006e50: c603 0000 730a 0000 0000 0104 0108 0108  ....s...........
-00006e60: fe04 047a 2454 6963 6b65 7443 6865 636b  ...z$TicketCheck
-00006e70: 6c69 7374 4974 656d 7341 5049 436c 6965  listItemsAPIClie
-00006e80: 6e74 2e64 656c 6574 654e 290a 720b 0000  nt.deleteN).r...
-00006e90: 0072 0c00 0000 720d 0000 0072 7100 0000  .r....r....rq...
-00006ea0: 72e0 0000 0072 e100 0000 721e 0000 0072  r....r....r....r
-00006eb0: a000 0000 72da 0000 0072 db00 0000 720f  ....r....r....r.
-00006ec0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00006ed0: 0000 7230 0100 00b6 0300 0073 0e00 0000  ..r0.......s....
-00006ee0: 0801 0401 0401 0402 0803 0804 0804 7230  ..............r0
-00006ef0: 0100 0029 0146 2901 4629 0146 295a 729f  ...).F).F).F)Zr.
-00006f00: 0000 0072 a600 0000 723c 0000 00da 076c  ...r....r<.....l
-00006f10: 6f67 6769 6e67 7202 0000 0072 a200 0000  oggingr....r....
-00006f20: 723a 0000 00da 0b64 6a61 6e67 6f2e 636f  r:.....django.co
-00006f30: 6e66 7203 0000 00da 1164 6a61 6e67 6f2e  nfr......django.
-00006f40: 636f 7265 2e63 6163 6865 7204 0000 00da  core.cacher.....
-00006f50: 0964 6a61 6e67 6f2e 6462 7205 0000 005a  .django.dbr....Z
-00006f60: 1064 6a61 7574 6f74 6173 6b2e 7574 696c  .djautotask.util
-00006f70: 7372 0600 0000 da08 7265 7472 7969 6e67  sr......retrying
-00006f80: 7207 0000 0072 be00 0000 72bf 0000 0072  r....r....r....r
-00006f90: 2500 0000 7224 0000 0072 2600 0000 72c7  %...r$...r&...r.
-00006fa0: 0000 0072 c800 0000 da09 6765 744c 6f67  ...r......getLog
-00006fb0: 6765 7272 0b00 0000 7237 0000 00da 0945  gerr....r7.....E
-00006fc0: 7863 6570 7469 6f6e 7209 0000 0072 1100  xceptionr....r..
-00006fd0: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00006fe0: 0072 1500 0000 7219 0000 0072 1c00 0000  .r....r....r....
-00006ff0: 7220 0000 0072 2800 0000 722d 0000 0072  r ...r(...r-...r
-00007000: 2e00 0000 722a 0000 0072 3000 0000 7242  ....r*...r0...rB
-00007010: 0000 0072 5600 0000 da06 6f62 6a65 6374  ...rV.....object
-00007020: 726c 0000 0072 df00 0000 72e6 0000 0072  rl...r....r....r
-00007030: e800 0000 72e9 0000 0072 ea00 0000 72eb  ....r....r....r.
-00007040: 0000 0072 ec00 0000 72ef 0000 0072 f100  ...r....r....r..
-00007050: 0000 72f2 0000 0072 f400 0000 72f7 0000  ..r....r....r...
-00007060: 0072 0201 0000 7203 0100 0072 0501 0000  .r....r....r....
-00007070: 7207 0100 0072 0901 0000 720a 0100 0072  r....r....r....r
-00007080: 0c01 0000 720d 0100 0072 0f01 0000 7213  ....r....r....r.
-00007090: 0100 0072 1601 0000 7218 0100 0072 1a01  ...r....r....r..
-000070a0: 0000 721b 0100 0072 1d01 0000 721e 0100  ..r....r....r...
-000070b0: 0072 1f01 0000 7220 0100 0072 2101 0000  .r....r ...r!...
-000070c0: 7222 0100 0072 2401 0000 7226 0100 0072  r"...r$...r&...r
-000070d0: 2701 0000 7228 0100 0072 2901 0000 722a  '...r(...r)...r*
-000070e0: 0100 0072 2b01 0000 722c 0100 0072 2d01  ...r+...r,...r-.
-000070f0: 0000 722e 0100 0072 2f01 0000 7230 0100  ..r....r/...r0..
-00007100: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
-00007110: 7210 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00007120: 0000 0073 ae00 0000 0801 0801 0801 0801  ...s............
-00007130: 0c02 0801 0802 0c01 0c01 0c01 0c01 0c02  ................
-00007140: 0402 0401 0401 0401 0402 02ff 0203 02ff  ................
-00007150: 0204 0a03 1005 1008 1008 1005 1005 0a01  ................
-00007160: 02ff 0407 0804 080b 0804 0808 0a04 0a04  ................
-00007170: 0a12 081c 0e31 0e33 107f 007f 007f 0007  .....1.3........
-00007180: 0e26 1004 1004 1004 1004 1004 100e 1004  .&..............
-00007190: 1004 1008 120e 120a 1008 1008 120a 120a  ................
-000071a0: 100e 1004 1008 1008 120a 120a 120a 120a  ................
-000071b0: 1004 1004 1004 1009 1004 1004 1004 100d  ................
-000071c0: 1004 1004 1004 1004 1004 1004 1004 1004  ................
-000071d0: 1004 1004 1004                           ......
+00000460: 6489 8400 6489 652e 652d 8304 5a59 4700  d...d.e.e-..ZYG.
+00000470: 648a 648b 8400 648b 652d 8303 5a5a 6401  d.d...d.e-..ZZd.
+00000480: 5300 298f e900 0000 004e 2901 da0f 4a53  S.)......N)...JS
+00000490: 4f4e 4465 636f 6465 4572 726f 7229 01da  ONDecodeError)..
+000004a0: 0873 6574 7469 6e67 7329 01da 0563 6163  .settings)...cac
+000004b0: 6865 2901 da06 6d6f 6465 6c73 2901 da12  he)...models)...
+000004c0: 446a 6175 746f 7461 736b 5365 7474 696e  DjautotaskSettin
+000004d0: 6773 2901 da05 7265 7472 7969 e803 0000  gs)...retryi....
+000004e0: 6910 2700 0069 5802 0000 da03 7572 6c5a  i.'..iX.....urlZ
+000004f0: 0677 6562 5572 6c7a 3d54 6865 206c 6f67  .webUrlz=The log
+00000500: 6765 6420 696e 2052 6573 6f75 7263 6520  ged in Resource 
+00000510: 646f 6573 206e 6f74 2068 6176 6520 7468  does not have th
+00000520: 6520 6164 6571 7561 7465 2070 6572 6d69  e adequate permi
+00000530: 7373 696f 6e73 7a77 4e6f 206d 6573 7361  ssionszwNo messa
+00000540: 6765 2e20 4e6f 206d 6174 6368 696e 6720  ge. No matching 
+00000550: 7265 636f 7264 7320 666f 756e 642e 2054  records found. T
+00000560: 6865 206c 6f67 6765 6420 696e 2052 6573  he logged in Res
+00000570: 6f75 7263 6520 6d61 7920 6e6f 7420 6861  ource may not ha
+00000580: 7665 2074 6865 2072 6571 7569 7265 6420  ve the required 
+00000590: 7065 726d 6973 7369 6f6e 7320 746f 2064  permissions to d
+000005a0: 656c 6574 6520 7468 6520 6461 7461 2e63  elete the data.c
+000005b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005c0: 0100 0000 4000 0000 7310 0000 0065 005a  ....@...s....e.Z
+000005d0: 0164 005a 0264 015a 0364 0253 0029 03da  .d.Z.d.Z.d.S.)..
+000005e0: 1041 7574 6f74 6173 6b41 5049 4572 726f  .AutotaskAPIErro
+000005f0: 727a 2352 6169 7365 2074 6869 732c 206e  rz#Raise this, n
+00000600: 6f74 2072 6571 7565 7374 2065 7863 6570  ot request excep
+00000610: 7469 6f6e 732e 4ea9 04da 085f 5f6e 616d  tions.N....__nam
+00000620: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000630: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
+00000640: 5f64 6f63 5f5f a900 720f 0000 0072 0f00  _doc__..r....r..
+00000650: 0000 fa43 2f68 6f6d 652f 7275 6e6e 6572  ...C/home/runner
+00000660: 2f77 6f72 6b2f 646a 616e 676f 2d61 7574  /work/django-aut
+00000670: 6f74 6173 6b2f 646a 616e 676f 2d61 7574  otask/django-aut
+00000680: 6f74 6173 6b2f 646a 6175 746f 7461 736b  otask/djautotask
+00000690: 2f61 7069 2e70 7972 0900 0000 1f00 0000  /api.pyr........
+000006a0: 7304 0000 0008 0104 0172 0900 0000 6300  s........r....c.
+000006b0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+000006c0: 0000 0040 0000 0073 1000 0000 6500 5a01  ...@...s....e.Z.
+000006d0: 6400 5a02 6401 5a03 6402 5300 2903 da16  d.Z.d.Z.d.S.)...
+000006e0: 4175 746f 7461 736b 4150 4943 6c69 656e  AutotaskAPIClien
+000006f0: 7445 7272 6f72 7a69 0a20 2020 2052 6169  tErrorzi.    Rai
+00000700: 7365 2074 6869 7320 746f 2069 6e64 6963  se this to indic
+00000710: 6174 6520 616e 7920 6874 7470 2065 7272  ate any http err
+00000720: 6f72 2074 6861 7420 6661 6c6c 7320 7769  or that falls wi
+00000730: 7468 696e 2074 6865 0a20 2020 2034 7878  thin the.    4xx
+00000740: 2063 6c61 7373 206f 6620 6874 7470 2073   class of http s
+00000750: 7461 7475 7320 636f 6465 732e 0a20 2020  tatus codes..   
+00000760: 204e 720a 0000 0072 0f00 0000 720f 0000   Nr....r....r...
+00000770: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
+00000780: 2400 0000 7304 0000 0008 0104 0472 1100  $...s........r..
+00000790: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000007a0: 0000 0001 0000 0040 0000 0073 1000 0000  .......@...s....
+000007b0: 6500 5a01 6400 5a02 6401 5a03 6402 5300  e.Z.d.Z.d.Z.d.S.
+000007c0: 2903 da16 4175 746f 7461 736b 4150 4953  )...AutotaskAPIS
+000007d0: 6572 7665 7245 7272 6f72 7a53 0a20 2020  erverErrorzS.   
+000007e0: 2052 6169 7365 2074 6869 7320 746f 2069   Raise this to i
+000007f0: 6e64 6963 6174 6520 6120 5365 7276 6572  ndicate a Server
+00000800: 2045 7272 6f72 0a20 2020 2035 3030 2063   Error.    500 c
+00000810: 6c61 7373 206f 6620 6874 7470 2073 7461  lass of http sta
+00000820: 7475 7320 636f 6465 732e 0a20 2020 204e  tus codes..    N
+00000830: 720a 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+00000840: 0f00 0000 7210 0000 0072 1200 0000 2c00  ....r....r....,.
+00000850: 0000 7304 0000 0008 0104 0472 1200 0000  ..s........r....
+00000860: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000870: 0001 0000 0040 0000 0073 1000 0000 6500  .....@...s....e.
+00000880: 5a01 6400 5a02 6401 5a03 6402 5300 2903  Z.d.Z.d.Z.d.S.).
+00000890: da1b 4175 746f 7461 736b 5265 636f 7264  ..AutotaskRecord
+000008a0: 4e6f 7446 6f75 6e64 4572 726f 727a 1954  NotFoundErrorz.T
+000008b0: 6865 2072 6563 6f72 6420 7761 7320 6e6f  he record was no
+000008c0: 7420 666f 756e 642e 4e72 0a00 0000 720f  t found.Nr....r.
+000008d0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+000008e0: 0000 7213 0000 0034 0000 0073 0400 0000  ..r....4...s....
+000008f0: 0801 0401 7213 0000 0063 0000 0000 0000  ....r....c......
+00000900: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+00000910: 0000 7310 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00000920: 015a 0364 0253 0029 03da 2441 7574 6f74  .Z.d.S.)..$Autot
+00000930: 6173 6b53 6563 7572 6974 7950 6572 6d69  askSecurityPermi
+00000940: 7373 696f 6e73 4578 6365 7074 696f 6e7a  ssionsExceptionz
+00000950: 3b54 6865 2041 5049 2063 7265 6465 6e74  ;The API credent
+00000960: 6961 6c73 2068 6176 6520 696e 7375 6666  ials have insuff
+00000970: 6963 6965 6e74 2073 6563 7572 6974 7920  icient security 
+00000980: 7065 726d 6973 7369 6f6e 732e 4e72 0a00  permissions.Nr..
+00000990: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+000009a0: 0072 1000 0000 7214 0000 0039 0000 0073  .r....r....9...s
+000009b0: 0400 0000 0801 0401 7214 0000 0063 0000  ........r....c..
+000009c0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+000009d0: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
+000009e0: 005a 0264 015a 0364 0253 0029 03da 2541  .Z.d.Z.d.S.)..%A
+000009f0: 7574 6f74 6173 6b49 6d70 6572 736f 6e61  utotaskImpersona
+00000a00: 7469 6f6e 4c69 6d69 7465 6445 7863 6570  tionLimitedExcep
+00000a10: 7469 6f6e 7a41 5468 6520 696d 7065 7273  tionzAThe impers
+00000a20: 6f6e 6174 696f 6e20 7265 736f 7572 6365  onation resource
+00000a30: 2068 6173 2069 6e73 7566 6669 6369 656e   has insufficien
+00000a40: 7420 7365 6375 7269 7479 2070 6572 6d69  t security permi
+00000a50: 7373 696f 6e73 2e4e 720a 0000 0072 0f00  ssions.Nr....r..
+00000a60: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00000a70: 0072 1500 0000 3e00 0000 7304 0000 0008  .r....>...s.....
+00000a80: 0304 0172 1500 0000 6301 0000 0000 0000  ...r....c.......
+00000a90: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00000aa0: 0073 0c00 0000 6401 a000 7c00 6a01 a101  .s....d...|.j...
+00000ab0: 5300 2902 4e7a 022c 2029 02da 046a 6f69  S.).Nz., )...joi
+00000ac0: 6eda 0461 7267 7329 01da 0165 720f 0000  n..args)...er...
+00000ad0: 0072 0f00 0000 7210 0000 00da 1670 6172  .r....r......par
+00000ae0: 7365 5f61 7574 6f74 6173 6b61 7069 6572  se_autotaskapier
+00000af0: 726f 7245 0000 0073 0200 0000 0001 7219  rorE...s......r.
+00000b00: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000b10: 0100 0000 0200 0000 4300 0000 730c 0000  ........C...s...
+00000b20: 0074 007c 0083 0174 016b 0853 0029 017a  .t.|...t.k.S.).z
+00000b30: fc0a 2020 2020 5265 7475 726e 2054 7275  ..    Return Tru
+00000b40: 6520 6966 2077 6520 7368 6f75 6c64 2072  e if we should r
+00000b50: 6574 7279 2028 696e 2074 6869 7320 6361  etry (in this ca
+00000b60: 7365 2077 6865 6e20 6974 2773 2061 6e0a  se when it's an.
+00000b70: 2020 2020 4175 746f 7461 736b 4150 4945      AutotaskAPIE
+00000b80: 7272 6f72 292c 2046 616c 7365 206f 7468  rror), False oth
+00000b90: 6572 7769 7365 2e0a 0a20 2020 2042 6173  erwise...    Bas
+00000ba0: 6963 616c 6c79 2c20 646f 6e27 7420 7265  ically, don't re
+00000bb0: 7472 7920 6f6e 2041 7574 6f74 6173 6b41  try on AutotaskA
+00000bc0: 5049 436c 6965 6e74 4572 726f 722c 2062  PIClientError, b
+00000bd0: 6563 6175 7365 2074 686f 7365 2061 7265  ecause those are
+00000be0: 2074 6865 0a20 2020 2074 7970 6520 6f66   the.    type of
+00000bf0: 2065 7863 6570 7469 6f6e 7320 7768 6572   exceptions wher
+00000c00: 6520 7265 7472 7969 6e67 2077 6f6e 2774  e retrying won't
+00000c10: 2068 656c 7020 2834 3034 732c 2034 3033   help (404s, 403
+00000c20: 732c 2065 7463 292e 0a20 2020 2029 02da  s, etc)..    )..
+00000c30: 0474 7970 6572 0900 0000 2901 da09 6578  .typer....)...ex
+00000c40: 6365 7074 696f 6e72 0f00 0000 720f 0000  ceptionr....r...
+00000c50: 0072 1000 0000 da12 7265 7472 795f 6966  .r......retry_if
+00000c60: 5f61 7069 5f65 7272 6f72 4900 0000 7302  _api_errorI...s.
+00000c70: 0000 0000 0872 1c00 0000 6301 0000 0000  .....r....c.....
+00000c80: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
+00000c90: 0000 0073 1000 0000 7400 a001 6401 7c00  ...s....t...d.|.
+00000ca0: 9b00 9d02 a101 5300 2902 4eda 057a 6f6e  ......S.).N..zon
+00000cb0: 655f 2902 7204 0000 00da 0367 6574 2901  e_).r......get).
+00000cc0: da09 6361 6368 655f 6b65 7972 0f00 0000  ..cache_keyr....
+00000cd0: 720f 0000 0072 1000 0000 da0e 6765 745f  r....r......get_
+00000ce0: 6361 6368 6564 5f75 726c 5400 0000 7302  cached_urlT...s.
+00000cf0: 0000 0000 0172 2000 0000 6301 0000 0000  .....r ...c.....
+00000d00: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
+00000d10: 0000 0073 3800 0000 7400 6a01 6401 7402  ...s8...t.j.d.t.
+00000d20: 9b00 9d02 7c00 7402 1900 7403 6402 8d03  ....|.t...t.d...
+00000d30: 0100 7400 6a01 6401 7404 9b00 9d02 7c00  ..t.j.d.t.....|.
+00000d40: 7404 1900 7403 6402 8d03 0100 6400 5300  t...t.d.....d.S.
+00000d50: 2903 4e72 1d00 0000 a901 da07 7469 6d65  ).Nr........time
+00000d60: 6f75 7429 0572 0400 0000 da03 7365 74da  out).r......set.
+00000d70: 0a41 545f 5552 4c5f 4b45 59da 0d43 4143  .AT_URL_KEY..CAC
+00000d80: 4845 5f54 494d 454f 5554 da0a 4154 5f57  HE_TIMEOUT..AT_W
+00000d90: 4542 5f4b 4559 2901 da08 6a73 6f6e 5f6f  EB_KEY)...json_o
+00000da0: 626a 720f 0000 0072 0f00 0000 7210 0000  bjr....r....r...
+00000db0: 00da 0c75 7064 6174 655f 6361 6368 6558  ...update_cacheX
+00000dc0: 0000 0073 1400 0000 0002 0401 0800 0600  ...s............
+00000dd0: 02ff 0602 0401 0800 0600 02ff 7228 0000  ............r(..
+00000de0: 0046 6301 0000 0000 0000 0000 0000 0001  .Fc.............
+00000df0: 0000 0003 0000 0043 0000 0073 0a00 0000  .......C...s....
+00000e00: 7400 7401 7c00 8302 5300 a901 4e29 02da  t.t.|...S...N)..
+00000e10: 135f 6765 745f 636f 6e6e 6563 7469 6f6e  ._get_connection
+00000e20: 5f75 726c 7224 0000 00a9 01da 0b66 6f72  _urlr$.......for
+00000e30: 6365 5f66 6574 6368 720f 0000 0072 0f00  ce_fetchr....r..
+00000e40: 0000 7210 0000 00da 1667 6574 5f61 7069  ..r......get_api
+00000e50: 5f63 6f6e 6e65 6374 696f 6e5f 7572 6c60  _connection_url`
+00000e60: 0000 0073 0200 0000 0001 722d 0000 0063  ...s......r-...c
+00000e70: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000e80: 0300 0000 4300 0000 730a 0000 0074 0074  ....C...s....t.t
+00000e90: 017c 0083 0253 0072 2900 0000 2902 722a  .|...S.r)...).r*
+00000ea0: 0000 0072 2600 0000 722b 0000 0072 0f00  ...r&...r+...r..
+00000eb0: 0000 720f 0000 0072 1000 0000 da16 6765  ..r....r......ge
+00000ec0: 745f 7765 625f 636f 6e6e 6563 7469 6f6e  t_web_connection
+00000ed0: 5f75 726c 6400 0000 7302 0000 0000 0172  _urld...s......r
+00000ee0: 2e00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00000ef0: 0006 0000 000a 0000 0043 0000 0073 6e00  .........C...sn.
+00000f00: 0000 7400 7c00 8301 7d02 7c02 7210 7c01  ..t.|...}.|.r.|.
+00000f10: 7266 7a22 7401 7402 6a03 6401 1900 8301  rfz"t.t.j.d.....
+00000f20: 7d03 7404 7c03 8301 0100 7c03 7c00 1900  }.t.|.....|.|...
+00000f30: 7d04 5700 716a 0400 7405 6b0a 7262 0100  }.W.qj..t.k.rb..
+00000f40: 7d05 0100 7a12 7405 6402 7c05 9b00 9d02  }...z.t.d.|.....
+00000f50: 8301 8201 5700 3500 6400 7d05 7e05 5800  ....W.5.d.}.~.X.
+00000f60: 5900 716a 5800 6e04 7c02 7d04 7c04 5300  Y.qjX.n.|.}.|.S.
+00000f70: 2903 4eda 0875 7365 726e 616d 657a 1946  ).N..usernamez.F
+00000f80: 6169 6c65 6420 746f 2067 6574 207a 6f6e  ailed to get zon
+00000f90: 6520 696e 666f 3a20 2906 7220 0000 00da  e info: ).r ....
+00000fa0: 0d67 6574 5f7a 6f6e 655f 696e 666f 7203  .get_zone_infor.
+00000fb0: 0000 00da 1441 5554 4f54 4153 4b5f 4352  .....AUTOTASK_CR
+00000fc0: 4544 454e 5449 414c 5372 2800 0000 7209  EDENTIALSr(...r.
+00000fd0: 0000 0029 06da 0566 6965 6c64 722c 0000  ...)...fieldr,..
+00000fe0: 005a 1261 7069 5f75 726c 5f66 726f 6d5f  .Z.api_url_from_
+00000ff0: 6361 6368 6572 2700 0000 7208 0000 0072  cacher'...r....r
+00001000: 1800 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+00001010: 0000 0072 2a00 0000 6800 0000 7314 0000  ...r*...h...s...
+00001020: 0000 0108 0208 0102 010e 0208 020c 0110  ................
+00001030: 0122 0204 0272 2a00 0000 6301 0000 0000  ."...r*...c.....
+00001040: 0000 0000 0000 0005 0000 000a 0000 0043  ...............C
+00001050: 0000 0073 b600 0000 7400 6a01 6401 1700  ...s....t.j.d...
+00001060: 7c00 1700 7d01 7a6e 7402 a003 6402 a004  |...}.znt...d...
+00001070: 7c01 a101 a101 0100 7405 6a06 7c01 6403  |.......t.j.|.d.
+00001080: 6404 8d02 7d02 6405 7c02 6a07 6b02 7246  d...}.d.|.j.k.rF
+00001090: 7c02 a008 a100 7d03 7c03 5700 5300 6406  |.....}.|.W.S.d.
+000010a0: 7c02 6a07 6b02 7270 7c02 a008 a100 7d03  |.j.k.rp|.....}.
+000010b0: 7409 6407 a004 7c01 7408 a00a 7c03 a101  t.d...|.t...|...
+000010c0: a102 8301 8201 6e0a 7409 7c02 6a0b 8301  ......n.t.|.j...
+000010d0: 8201 5700 6e34 0400 7405 6a0c 6b0a 72b0  ..W.n4..t.j.k.r.
+000010e0: 0100 7d04 0100 7a14 7409 6407 a004 7c01  ..}...z.t.d...|.
+000010f0: 7c04 a102 8301 8201 5700 3500 6400 7d04  |.......W.5.d.}.
+00001100: 7e04 5800 5900 6e02 5800 6400 5300 2908  ~.X.Y.n.X.d.S.).
+00001110: 4e7a 1a76 312e 302f 7a6f 6e65 496e 666f  Nz.v1.0/zoneInfo
+00001120: 726d 6174 696f 6e3f 7573 6572 3dfa 184d  rmation?user=..M
+00001130: 616b 696e 6720 4745 5420 7265 7175 6573  aking GET reques
+00001140: 7420 746f 207b 7de9 0300 0000 7221 0000  t to {}.....r!..
+00001150: 00e9 c800 0000 e9f4 0100 00fa 1a52 6571  .............Req
+00001160: 7565 7374 2066 6169 6c65 643a 2047 4554  uest failed: GET
+00001170: 207b 7d3a 207b 7d29 0d72 0300 0000 da13   {}: {}).r......
+00001180: 4155 544f 5441 534b 5f53 4552 5645 525f  AUTOTASK_SERVER_
+00001190: 5552 4cda 066c 6f67 6765 72da 0564 6562  URL..logger..deb
+000011a0: 7567 da06 666f 726d 6174 da08 7265 7175  ug..format..requ
+000011b0: 6573 7473 721e 0000 00da 0b73 7461 7475  estsr......statu
+000011c0: 735f 636f 6465 da04 6a73 6f6e 7209 0000  s_code..jsonr...
+000011d0: 00da 0564 756d 7073 da07 636f 6e74 656e  ...dumps..conten
+000011e0: 74da 1052 6571 7565 7374 4578 6365 7074  t..RequestExcept
+000011f0: 696f 6e29 0572 2f00 0000 da0c 656e 6470  ion).r/.....endp
+00001200: 6f69 6e74 5f75 726c da08 7265 7370 6f6e  oint_url..respon
+00001210: 7365 5a09 7265 7370 5f6a 736f 6e72 1800  seZ.resp_jsonr..
+00001220: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00001230: 0072 3000 0000 7a00 0000 7332 0000 0000  .r0...z...s2....
+00001240: 0108 0102 ff04 0302 0110 010e 010a 0108  ................
+00001250: 0106 010a 0208 0102 0104 0102 0008 ff02  ................
+00001260: ff06 060e 0112 0102 0104 0102 0002 ff02  ................
+00001270: ff72 3000 0000 6300 0000 0000 0000 0000  .r0...c.........
+00001280: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
+00001290: 2e00 0000 6500 5a01 6400 5a02 6401 6401  ....e.Z.d.Z.d.d.
+000012a0: 6401 6402 9c03 6403 6404 8402 5a03 6405  d.d...d.d...Z.d.
+000012b0: 6406 8400 5a04 6407 6408 8400 5a05 6401  d...Z.d.d...Z.d.
+000012c0: 5300 2909 da0c 4170 6943 6f6e 6469 7469  S.)...ApiConditi
+000012d0: 6f6e 4e29 03da 026f 7072 3200 0000 da05  onN)...opr2.....
+000012e0: 7661 6c75 6563 0100 0000 0000 0000 0300  valuec..........
+000012f0: 0000 0600 0000 0500 0000 4700 0000 735a  ..........G...sZ
+00001300: 0000 0067 007c 005f 007c 017c 005f 017c  ...g.|._.|.|._.|
+00001310: 027c 005f 027c 037c 005f 037c 0164 016b  .|._.|.|._.|.d.k
+00001320: 0672 567c 0444 005d 307d 0574 047c 0583  .rV|.D.]0}.t.|..
+00001330: 017c 006a 056b 0372 4874 0664 02a0 077c  .|.j.k.rHt.d...|
+00001340: 006a 056a 08a1 0183 0182 017c 006a 00a0  .j.j.......|.j..
+00001350: 097c 05a1 0101 0071 2464 0053 0029 034e  .|.....q$d.S.).N
+00001360: 2902 da03 616e 64da 026f 727a 2f47 726f  )...and..orz/Gro
+00001370: 7570 6564 2063 6f6e 6469 7469 6f6e 7320  uped conditions 
+00001380: 6d75 7374 2061 6c73 6f20 6265 2069 6e73  must also be ins
+00001390: 7461 6e63 6573 206f 6620 7b7d 290a da06  tances of {})...
+000013a0: 5f69 7465 6d73 7245 0000 0072 3200 0000  _itemsrE...r2...
+000013b0: 7246 0000 0072 1a00 0000 da09 5f5f 636c  rF...r......__cl
+000013c0: 6173 735f 5fda 0954 7970 6545 7272 6f72  ass__..TypeError
+000013d0: 723b 0000 0072 0b00 0000 da06 6170 7065  r;...r......appe
+000013e0: 6e64 2906 da04 7365 6c66 7245 0000 0072  nd)...selfrE...r
+000013f0: 3200 0000 7246 0000 0072 1700 0000 da09  2...rF...r......
+00001400: 636f 6e64 6974 696f 6e72 0f00 0000 720f  conditionr....r.
+00001410: 0000 0072 1000 0000 da08 5f5f 696e 6974  ...r......__init
+00001420: 5f5f 9800 0000 731a 0000 0000 0106 0106  __....s.........
+00001430: 0106 0106 0208 0208 010e 0102 0104 0106  ................
+00001440: ff02 ff04 047a 1541 7069 436f 6e64 6974  .....z.ApiCondit
+00001450: 696f 6e2e 5f5f 696e 6974 5f5f 6301 0000  ion.__init__c...
+00001460: 0000 0000 0000 0000 0001 0000 0005 0000  ................
+00001470: 0043 0000 0073 2800 0000 7400 7c00 6a01  .C...s(...t.|.j.
+00001480: 8301 7214 7c00 6a01 a002 a100 5300 6401  ..r.|.j.....S.d.
+00001490: a003 7c00 6a04 7c00 6a05 7c00 6a06 a103  ..|.j.|.j.|.j...
+000014a0: 5300 2902 4e7a 207b 7b6f 703a 207b 7d2c  S.).Nz {{op: {},
+000014b0: 2066 6965 6c64 3a20 7b7d 2c20 7661 6c75   field: {}, valu
+000014c0: 653a 207b 7d7d 7d29 07da 036c 656e 7249  e: {}}})...lenrI
+000014d0: 0000 00da 085f 5f72 6570 725f 5f72 3b00  .....__repr__r;.
+000014e0: 0000 7245 0000 0072 3200 0000 7246 0000  ..rE...r2...rF..
+000014f0: 00a9 0172 4d00 0000 720f 0000 0072 0f00  ...rM...r....r..
+00001500: 0000 7210 0000 0072 5100 0000 a800 0000  ..r....rQ.......
+00001510: 730e 0000 0000 010a 010a 0104 0104 0104  s...............
+00001520: 0104 fd7a 1541 7069 436f 6e64 6974 696f  ...z.ApiConditio
+00001530: 6e2e 5f5f 7265 7072 5f5f 6301 0000 0000  n.__repr__c.....
+00001540: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00001550: 0000 0073 4600 0000 7400 7c00 6a01 8301  ...sF...t.|.j...
+00001560: 7224 7c00 6a02 6401 6402 8400 7c00 6a01  r$|.j.d.d...|.j.
+00001570: 4400 8301 6403 9c02 7d01 6e1e 7c00 6a02  D...d...}.n.|.j.
+00001580: 7c00 6a03 6404 9c02 7d01 7c00 6a04 7242  |.j.d...}.|.j.rB
+00001590: 7c00 6a04 7c01 6405 3c00 7c01 5300 2906  |.j.|.d.<.|.S.).
+000015a0: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
+000015b0: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
+000015c0: 007c 005d 0c7d 017c 01a0 00a1 0091 0271  .|.].}.|.......q
+000015d0: 0453 0072 0f00 0000 2901 da10 666f 726d  .S.r....)...form
+000015e0: 6174 5f63 6f6e 6469 7469 6f6e 2902 da02  at_condition)...
+000015f0: 2e30 5a0d 6170 695f 636f 6e64 6974 696f  .0Z.api_conditio
+00001600: 6e72 0f00 0000 720f 0000 0072 1000 0000  nr....r....r....
+00001610: da0a 3c6c 6973 7463 6f6d 703e b600 0000  ..<listcomp>....
+00001620: 7304 0000 0006 0202 ff7a 3141 7069 436f  s........z1ApiCo
+00001630: 6e64 6974 696f 6e2e 666f 726d 6174 5f63  ndition.format_c
+00001640: 6f6e 6469 7469 6f6e 2e3c 6c6f 6361 6c73  ondition.<locals
+00001650: 3e2e 3c6c 6973 7463 6f6d 703e 2902 7245  >.<listcomp>).rE
+00001660: 0000 00da 0569 7465 6d73 2902 7245 0000  .....items).rE..
+00001670: 0072 3200 0000 7246 0000 0029 0572 5000  .r2...rF...).rP.
+00001680: 0000 7249 0000 0072 4500 0000 7232 0000  ..rI...rE...r2..
+00001690: 0072 4600 0000 a902 724d 0000 0072 4e00  .rF.....rM...rN.
+000016a0: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+000016b0: 0072 5300 0000 b100 0000 7318 0000 0000  .rS.......s.....
+000016c0: 010a 0304 0106 0204 fe04 fe08 0904 0104  ................
+000016d0: fe06 0406 020a 027a 1d41 7069 436f 6e64  .......z.ApiCond
+000016e0: 6974 696f 6e2e 666f 726d 6174 5f63 6f6e  ition.format_con
+000016f0: 6469 7469 6f6e 2906 720b 0000 0072 0c00  dition).r....r..
+00001700: 0000 720d 0000 0072 4f00 0000 7251 0000  ..r....rO...rQ..
+00001710: 0072 5300 0000 720f 0000 0072 0f00 0000  .rS...r....r....
+00001720: 720f 0000 0072 1000 0000 7244 0000 0096  r....r....rD....
+00001730: 0000 0073 0600 0000 0802 1210 0809 7244  ...s..........rD
+00001740: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001750: 0000 0000 0300 0000 4000 0000 7360 0000  ........@...s`..
+00001760: 0065 005a 0164 005a 0264 0164 0264 039c  .e.Z.d.Z.d.d.d..
+00001770: 025a 0364 0464 0584 005a 0464 0664 0784  .Z.d.d...Z.d.d..
+00001780: 005a 0564 0864 0984 005a 0664 0a64 0b84  .Z.d.d...Z.d.d..
+00001790: 005a 0764 0c64 0d84 005a 0864 0e64 0f84  .Z.d.d...Z.d.d..
+000017a0: 005a 0964 1064 1184 005a 0a64 1864 1364  .Z.d.d...Z.d.d.d
+000017b0: 1484 015a 0b64 1564 1684 005a 0c64 1753  ...Z.d.d...Z.d.S
+000017c0: 0029 19da 1041 7069 436f 6e64 6974 696f  .)...ApiConditio
+000017d0: 6e4c 6973 747a 0d71 7565 7279 3f73 6561  nListz.query?sea
+000017e0: 7263 683d da05 7175 6572 7929 0272 1e00  rch=..query).r..
+000017f0: 0000 da04 706f 7374 6301 0000 0000 0000  ....postc.......
+00001800: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00001810: 0073 0c00 0000 7400 8300 7c00 5f01 6400  .s....t...|._.d.
+00001820: 5300 7229 0000 0029 02da 046c 6973 74da  S.r)...)...list.
+00001830: 055f 6c69 7374 7252 0000 0072 0f00 0000  ._listrR...r....
+00001840: 720f 0000 0072 1000 0000 724f 0000 00cd  r....r....rO....
+00001850: 0000 0073 0200 0000 0001 7a19 4170 6943  ...s......z.ApiC
+00001860: 6f6e 6469 7469 6f6e 4c69 7374 2e5f 5f69  onditionList.__i
+00001870: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00001880: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
+00001890: 0000 007c 006a 00a0 01a1 0053 0072 2900  ...|.j.....S.r).
+000018a0: 0000 2902 725c 0000 0072 5100 0000 7252  ..).r\...rQ...rR
+000018b0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+000018c0: 0000 7251 0000 00d0 0000 0073 0200 0000  ..rQ.......s....
+000018d0: 0001 7a19 4170 6943 6f6e 6469 7469 6f6e  ..z.ApiCondition
+000018e0: 4c69 7374 2e5f 5f72 6570 725f 5f63 0100  List.__repr__c..
+000018f0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00001900: 0000 4300 0000 730a 0000 0074 007c 006a  ..C...s....t.|.j
+00001910: 0183 0153 0072 2900 0000 2902 7250 0000  ...S.r)...).rP..
+00001920: 0072 5c00 0000 7252 0000 0072 0f00 0000  .r\...rR...r....
+00001930: 720f 0000 0072 1000 0000 da07 5f5f 6c65  r....r......__le
+00001940: 6e5f 5fd3 0000 0073 0200 0000 0001 7a18  n__....s......z.
+00001950: 4170 6943 6f6e 6469 7469 6f6e 4c69 7374  ApiConditionList
+00001960: 2e5f 5f6c 656e 5f5f 6302 0000 0000 0000  .__len__c.......
+00001970: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00001980: 0073 0a00 0000 7c00 6a00 7c01 1900 5300  .s....|.j.|...S.
+00001990: 7229 0000 00a9 0172 5c00 0000 a902 724d  r).....r\.....rM
+000019a0: 0000 00da 0169 720f 0000 0072 0f00 0000  .....ir....r....
+000019b0: 7210 0000 00da 0b5f 5f67 6574 6974 656d  r......__getitem
+000019c0: 5f5f d600 0000 7302 0000 0000 017a 1c41  __....s......z.A
+000019d0: 7069 436f 6e64 6974 696f 6e4c 6973 742e  piConditionList.
+000019e0: 5f5f 6765 7469 7465 6d5f 5f63 0300 0000  __getitem__c....
+000019f0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00001a00: 4300 0000 7322 0000 0074 007c 0283 0174  C...s"...t.|...t
+00001a10: 016b 0972 1474 0264 0183 0182 017c 027c  .k.r.t.d.....|.|
+00001a20: 006a 037c 013c 0064 0053 00a9 024e 7a2d  .j.|.<.d.S...Nz-
+00001a30: 436f 6e64 6974 696f 6e73 206d 7573 7420  Conditions must 
+00001a40: 6265 2069 6e73 7461 6e63 6573 206f 6620  be instances of 
+00001a50: 4170 6943 6f6e 6469 7469 6f6e 2e29 0472  ApiCondition.).r
+00001a60: 1a00 0000 7244 0000 0072 4b00 0000 725c  ....rD...rK...r\
+00001a70: 0000 0029 0372 4d00 0000 7260 0000 0072  ...).rM...r`...r
+00001a80: 4600 0000 720f 0000 0072 0f00 0000 7210  F...r....r....r.
+00001a90: 0000 00da 0b5f 5f73 6574 6974 656d 5f5f  .....__setitem__
+00001aa0: d900 0000 7306 0000 0000 010c 0108 017a  ....s..........z
+00001ab0: 1c41 7069 436f 6e64 6974 696f 6e4c 6973  .ApiConditionLis
+00001ac0: 742e 5f5f 7365 7469 7465 6d5f 5f63 0200  t.__setitem__c..
+00001ad0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00001ae0: 0000 4300 0000 730c 0000 007c 006a 007c  ..C...s....|.j.|
+00001af0: 013d 0064 0053 0072 2900 0000 725e 0000  .=.d.S.r)...r^..
+00001b00: 0072 5f00 0000 720f 0000 0072 0f00 0000  .r_...r....r....
+00001b10: 7210 0000 00da 0b5f 5f64 656c 6974 656d  r......__delitem
+00001b20: 5f5f de00 0000 7302 0000 0000 017a 1c41  __....s......z.A
+00001b30: 7069 436f 6e64 6974 696f 6e4c 6973 742e  piConditionList.
+00001b40: 5f5f 6465 6c69 7465 6d5f 5f63 0100 0000  __delitem__c....
+00001b50: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00001b60: 4300 0000 730a 0000 007c 006a 00a0 01a1  C...s....|.j....
+00001b70: 0053 0072 2900 0000 2902 725c 0000 00da  .S.r)...).r\....
+00001b80: 085f 5f69 7465 725f 5f72 5200 0000 720f  .__iter__rR...r.
+00001b90: 0000 0072 0f00 0000 7210 0000 0072 6500  ...r....r....re.
+00001ba0: 0000 e100 0000 7302 0000 0000 017a 1941  ......s......z.A
+00001bb0: 7069 436f 6e64 6974 696f 6e4c 6973 742e  piConditionList.
+00001bc0: 5f5f 6974 6572 5f5f 721e 0000 0063 0200  __iter__r....c..
+00001bd0: 0000 0000 0000 0000 0000 0a00 0000 0500  ................
+00001be0: 0000 4b00 0000 739e 0000 0067 007d 037c  ..K...s....g.}.|
+00001bf0: 006a 0044 005d 127d 047c 03a0 017c 04a0  .j.D.].}.|...|..
+00001c00: 02a1 00a1 0101 0071 0a64 017c 0369 017d  .......q.d.|.i.}
+00001c10: 057c 02a0 0364 02a1 017d 067c 0672 427c  .|...d...}.|.rB|
+00001c20: 05a0 0464 037c 0669 01a1 0101 007c 006a  ...d.|.i.....|.j
+00001c30: 057c 0119 007d 0774 06a0 077c 05a1 017d  .|...}.t...|...}
+00001c40: 087c 0164 046b 0272 867c 02a0 0364 05a1  .|.d.k.r.|...d..
+00001c50: 017d 097c 0972 7864 067c 089b 009d 027d  .}.|.rxd.|.....}
+00001c60: 076e 087c 077c 0837 007d 0764 007d 086e  .n.|.|.7.}.d.}.n
+00001c70: 107c 0164 076b 0372 9674 0864 0883 0182  .|.d.k.r.t.d....
+00001c80: 017c 077c 0866 0253 0029 094e da06 6669  .|.|.f.S.).N..fi
+00001c90: 6c74 6572 da09 7061 6765 5f73 697a 655a  lter..page_sizeZ
+00001ca0: 0a4d 6178 5265 636f 7264 7372 1e00 0000  .MaxRecordsr....
+00001cb0: da0c 7265 636f 7264 5f63 6f75 6e74 7a13  ..record_countz.
+00001cc0: 7175 6572 792f 636f 756e 743f 7365 6172  query/count?sear
+00001cd0: 6368 3d72 5a00 0000 7a12 556e 7375 7070  ch=rZ...z.Unsupp
+00001ce0: 6f72 7465 6420 6d65 7468 6f64 2909 725c  orted method).r\
+00001cf0: 0000 0072 4c00 0000 7253 0000 0072 1e00  ...rL...rS...r..
+00001d00: 0000 da06 7570 6461 7465 da07 4d45 5448  ....update..METH
+00001d10: 4f44 5372 3e00 0000 723f 0000 0072 4b00  ODSr>...r?...rK.
+00001d20: 0000 290a 724d 0000 00da 066d 6574 686f  ..).rM.....metho
+00001d30: 64da 066b 7761 7267 73da 0771 7565 7269  d..kwargs..queri
+00001d40: 6573 724e 0000 005a 1163 6f6e 6469 7469  esrN...Z.conditi
+00001d50: 6f6e 5f66 696c 7465 7273 5a0b 6d61 785f  on_filtersZ.max_
+00001d60: 7265 636f 7264 73da 0865 6e64 706f 696e  records..endpoin
+00001d70: 74da 0766 696c 7465 7273 da05 636f 756e  t..filters..coun
+00001d80: 7472 0f00 0000 720f 0000 0072 1000 0000  tr....r....r....
+00001d90: da0b 6275 696c 645f 7175 6572 79e4 0000  ..build_query...
+00001da0: 0073 2e00 0000 0001 0401 0a01 1003 0200  .s..............
+00001db0: 02ff 0404 0a01 0401 0401 0200 02ff 0604  ................
+00001dc0: 0a01 0a02 0802 0a01 0401 0c02 0802 0601  ................
+00001dd0: 0801 0802 7a1c 4170 6943 6f6e 6469 7469  ....z.ApiConditi
+00001de0: 6f6e 4c69 7374 2e62 7569 6c64 5f71 7565  onList.build_que
+00001df0: 7279 6302 0000 0000 0000 0000 0000 0002  ryc.............
+00001e00: 0000 0003 0000 0043 0000 0073 2400 0000  .......C...s$...
+00001e10: 7400 7c01 8301 7401 6b09 7214 7402 6401  t.|...t.k.r.t.d.
+00001e20: 8301 8201 7c00 6a03 a004 7c01 a101 0100  ....|.j...|.....
+00001e30: 6400 5300 7262 0000 0029 0572 1a00 0000  d.S.rb...).r....
+00001e40: 7244 0000 0072 4b00 0000 725c 0000 0072  rD...rK...r\...r
+00001e50: 4c00 0000 7257 0000 0072 0f00 0000 720f  L...rW...r....r.
+00001e60: 0000 0072 1000 0000 da03 6164 6404 0100  ...r......add...
+00001e70: 0073 0600 0000 0001 0c01 0802 7a14 4170  .s..........z.Ap
+00001e80: 6943 6f6e 6469 7469 6f6e 4c69 7374 2e61  iConditionList.a
+00001e90: 6464 4e29 0172 1e00 0000 290d 720b 0000  ddN).r....).r...
+00001ea0: 0072 0c00 0000 720d 0000 0072 6a00 0000  .r....r....rj...
+00001eb0: 724f 0000 0072 5100 0000 725d 0000 0072  rO...rQ...r]...r
+00001ec0: 6100 0000 7263 0000 0072 6400 0000 7265  a...rc...rd...re
+00001ed0: 0000 0072 7100 0000 7272 0000 0072 0f00  ...rq...rr...r..
+00001ee0: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00001ef0: 0072 5800 0000 c700 0000 7318 0000 0008  .rX.......s.....
+00001f00: 0202 0102 fe06 0508 0308 0308 0308 0308  ................
+00001f10: 0508 0308 030a 2072 5800 0000 6300 0000  ...... rX...c...
+00001f20: 0000 0000 0000 0000 0000 0000 0006 0000  ................
+00001f30: 0040 0000 0073 da00 0000 6500 5a01 6400  .@...s....e.Z.d.
+00001f40: 5a02 6401 5a03 6402 5a04 6432 6403 6404  Z.d.Z.d.Z.d2d.d.
+00001f50: 8401 5a05 6506 6405 6406 8400 8301 5a07  ..Z.e.d.d.....Z.
+00001f60: 6433 6407 6408 8401 5a08 6409 640a 8400  d3d.d...Z.d.d...
+00001f70: 5a09 640b 640c 8400 5a0a 640d 640e 8400  Z.d.d...Z.d.d...
+00001f80: 5a0b 640f 6410 8400 5a0c 6411 6412 8400  Z.d.d...Z.d.d...
+00001f90: 5a0d 6413 6414 8400 5a0e 6415 6416 8400  Z.d.d...Z.d.d...
+00001fa0: 5a0f 6434 6418 6419 8401 5a10 641a 641b  Z.d4d.d...Z.d.d.
+00001fb0: 8400 5a11 641c 641d 8400 5a12 6435 641e  ..Z.d.d...Z.d5d.
+00001fc0: 641f 8401 5a13 6420 6421 8400 5a14 6422  d...Z.d d!..Z.d"
+00001fd0: 6423 8400 5a15 6424 6425 8400 5a16 6426  d#..Z.d$d%..Z.d&
+00001fe0: 6427 8400 5a17 6428 6429 8400 5a18 642a  d'..Z.d(d)..Z.d*
+00001ff0: 642b 8400 5a19 642c 642d 8400 5a1a 642e  d+..Z.d,d-..Z.d.
+00002000: 642f 8400 5a1b 6436 6430 6431 8401 5a1c  d/..Z.d6d0d1..Z.
+00002010: 6401 5300 2937 da11 4175 746f 7461 736b  d.S.)7..Autotask
+00002020: 4150 4943 6c69 656e 744e e901 0000 0063  APIClientN.....c
+00002030: 0700 0000 0000 0000 0000 0000 0700 0000  ................
+00002040: 0200 0000 4300 0000 739e 0000 007c 0173  ....C...s....|.s
+00002050: 0e74 006a 0164 0119 007d 017c 0273 1c74  .t.j.d...}.|.s.t
+00002060: 006a 0164 0219 007d 027c 0373 2a74 006a  .j.d...}.|.s*t.j
+00002070: 0164 0319 007d 037c 0473 3874 006a 0164  .d...}.|.s8t.j.d
+00002080: 0419 007d 047c 0573 4274 0283 007d 057c  ...}.|.sBt...}.|
+00002090: 006a 0373 5074 0464 0583 0182 017c 017c  .j.sPt.d.....|.|
+000020a0: 005f 057c 027c 005f 067c 037c 005f 077c  ._.|.|._.|.|._.|
+000020b0: 047c 005f 087c 057c 005f 0974 0a83 00a0  .|._.|.|._.t....
+000020c0: 0ba1 007c 005f 0c7c 006a 0c64 0619 007c  ...|._.|.j.d...|
+000020d0: 005f 0d7c 067c 005f 0e74 0f83 007c 005f  ._.|.|._.t...|._
+000020e0: 1064 007c 005f 1164 0053 0029 074e 722f  .d.|._.d.S.).Nr/
+000020f0: 0000 00da 0870 6173 7377 6f72 64da 1069  .....password..i
+00002100: 6e74 6567 7261 7469 6f6e 5f63 6f64 65da  ntegration_code.
+00002110: 1072 6573 745f 6170 695f 7665 7273 696f  .rest_api_versio
+00002120: 6e7a 1141 5049 206e 6f74 2073 7065 6369  nz.API not speci
+00002130: 6669 6564 7222 0000 0029 1272 0300 0000  fiedr"...).r....
+00002140: 7231 0000 0072 2d00 0000 da03 4150 49da  r1...r-.....API.
+00002150: 0a56 616c 7565 4572 726f 7272 2f00 0000  .ValueErrorr/...
+00002160: 7275 0000 0072 7600 0000 7277 0000 00da  ru...rv...rw....
+00002170: 0a73 6572 7665 725f 7572 6c72 0600 0000  .server_urlr....
+00002180: 5a0c 6765 745f 7365 7474 696e 6773 da10  Z.get_settings..
+00002190: 7265 7175 6573 745f 7365 7474 696e 6773  request_settings
+000021a0: 7222 0000 00da 1669 6d70 6572 736f 6e61  r".....impersona
+000021b0: 7469 6f6e 5f72 6573 6f75 7263 6572 5800  tion_resourcerX.
+000021c0: 0000 da0a 636f 6e64 6974 696f 6e73 da0b  ....conditions..
+000021d0: 6361 6368 6564 5f62 6f64 7929 0772 4d00  cached_body).rM.
+000021e0: 0000 722f 0000 0072 7500 0000 7276 0000  ..r/...ru...rv..
+000021f0: 0072 7700 0000 727a 0000 0072 7c00 0000  .rw...rz...r|...
+00002200: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00002210: 4f00 0000 0f01 0000 7334 0000 0000 0904  O.......s4......
+00002220: 010a 0104 010a 0104 0104 0102 ff04 0304  ................
+00002230: 0104 0102 ff04 0204 0106 0206 0108 0206  ................
+00002240: 0106 0106 0106 0106 020c 010c 0106 0108  ................
+00002250: 027a 1a41 7574 6f74 6173 6b41 5049 436c  .z.AutotaskAPICl
+00002260: 6965 6e74 2e5f 5f69 6e69 745f 5f63 0100  ient.__init__c..
+00002270: 0000 0000 0000 0000 0000 0100 0000 0500  ................
+00002280: 0000 4300 0000 7314 0000 0064 01a0 007c  ..C...s....d...|
+00002290: 006a 0174 026a 0364 0219 00a1 0253 0029  .j.t.j.d.....S.)
+000022a0: 034e 7a08 7b30 7d76 7b31 7d2f 7277 0000  .Nz.{0}v{1}/rw..
+000022b0: 0029 0472 3b00 0000 727a 0000 0072 0300  .).r;...rz...r..
+000022c0: 0000 7231 0000 0072 5200 0000 720f 0000  ..r1...rR...r...
+000022d0: 0072 0f00 0000 7210 0000 00da 0c61 7069  .r....r......api
+000022e0: 5f62 6173 655f 7572 6c36 0100 0073 0800  _base_url6...s..
+000022f0: 0000 0002 0401 0401 08fe 7a1e 4175 746f  ..........z.Auto
+00002300: 7461 736b 4150 4943 6c69 656e 742e 6170  taskAPIClient.ap
+00002310: 695f 6261 7365 5f75 726c 6302 0000 0000  i_base_urlc.....
+00002320: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00002330: 0000 0073 1800 0000 7c01 730a 7c00 6a00  ...s....|.s.|.j.
+00002340: 7d01 6401 a001 7c00 6a02 7c01 a102 5300  }.d...|.j.|...S.
+00002350: 2902 4e7a 077b 307d 7b31 7d2f 2903 7278  ).Nz.{0}{1}/).rx
+00002360: 0000 0072 3b00 0000 727f 0000 00a9 0272  ...r;...r......r
+00002370: 4d00 0000 726e 0000 0072 0f00 0000 720f  M...rn...r....r.
+00002380: 0000 0072 1000 0000 da0b 6765 745f 6170  ...r......get_ap
+00002390: 695f 7572 6c3d 0100 0073 0c00 0000 0001  i_url=...s......
+000023a0: 0401 0602 0401 0401 02fe 7a1d 4175 746f  ..........z.Auto
+000023b0: 7461 736b 4150 4943 6c69 656e 742e 6765  taskAPIClient.ge
+000023c0: 745f 6170 695f 7572 6c63 0200 0000 0000  t_api_urlc......
+000023d0: 0000 0000 0000 0200 0000 0700 0000 4300  ..............C.
+000023e0: 0000 731e 0000 0074 00a0 0164 01a0 027c  ..s....t...d...|
+000023f0: 016a 037c 016a 047c 016a 05a1 03a1 0101  .j.|.j.|.j......
+00002400: 0064 0053 0029 024e 7a20 4661 696c 6564  .d.S.).Nz Failed
+00002410: 2041 5049 2063 616c 6c3a 207b 307d 202d   API call: {0} -
+00002420: 207b 317d 202d 207b 327d 2906 7239 0000   {1} - {2}).r9..
+00002430: 00da 0565 7272 6f72 723b 0000 0072 0800  ...errorr;...r..
+00002440: 0000 723d 0000 0072 4000 0000 2902 724d  ..r=...r@...).rM
+00002450: 0000 0072 4300 0000 720f 0000 0072 0f00  ...rC...r....r..
+00002460: 0000 7210 0000 00da 0b5f 6c6f 675f 6661  ..r......_log_fa
+00002470: 696c 6564 4601 0000 730a 0000 0000 0108  iledF...s.......
+00002480: 0104 0004 0004 ff7a 1d41 7574 6f74 6173  .......z.Autotas
+00002490: 6b41 5049 436c 6965 6e74 2e5f 6c6f 675f  kAPIClient._log_
+000024a0: 6661 696c 6564 6302 0000 0000 0000 0000  failedc.........
+000024b0: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
+000024c0: 1400 0000 6401 7d02 6402 a000 7c01 7c02  ....d.}.d...|.|.
+000024d0: a102 7d01 7c01 5300 2903 4e7a 8352 6573  ..}.|.S.).Nz.Res
+000024e0: 6f75 7263 6520 696d 7065 7273 6f6e 6174  ource impersonat
+000024f0: 696f 6e20 6973 2065 6e61 626c 6564 2069  ion is enabled i
+00002500: 6e20 796f 7572 2054 6f70 4c65 6674 2061  n your TopLeft a
+00002510: 7070 6c69 6361 7469 6f6e 2e20 506c 6561  pplication. Plea
+00002520: 7365 2063 6865 636b 2074 6865 2072 6573  se check the res
+00002530: 6f75 7263 6520 7365 6375 7269 7479 206c  ource security l
+00002540: 6576 656c 2074 6861 7420 6973 2062 6569  evel that is bei
+00002550: 6e67 2069 6d70 6572 736f 6e61 7465 642e  ng impersonated.
+00002560: fa05 7b7d 207b 7d29 0172 3b00 0000 2903  ..{} {}).r;...).
+00002570: 724d 0000 00da 036d 7367 5a17 696d 7065  rM.....msgZ.impe
+00002580: 7273 6f6e 6174 696f 6e5f 6572 726f 725f  rsonation_error_
+00002590: 6d73 6772 0f00 0000 720f 0000 0072 1000  msgr....r....r..
+000025a0: 0000 da20 5f70 7265 7061 7265 5f65 7272  ... _prepare_err
+000025b0: 6f72 5f66 6f72 5f69 6d70 6572 736f 6e61  or_for_impersona
+000025c0: 7469 6f6e 4a01 0000 7308 0000 0000 0202  tionJ...s.......
+000025d0: ff02 040c 017a 3241 7574 6f74 6173 6b41  .....z2AutotaskA
+000025e0: 5049 436c 6965 6e74 2e5f 7072 6570 6172  PIClient._prepar
+000025f0: 655f 6572 726f 725f 666f 725f 696d 7065  e_error_for_impe
+00002600: 7273 6f6e 6174 696f 6e63 0200 0000 0000  rsonationc......
+00002610: 0000 0000 0000 0800 0000 0800 0000 4300  ..............C.
+00002620: 0000 73e4 0000 007c 016a 00a0 0164 01a1  ..s....|.j...d..
+00002630: 017d 027c 02a0 0264 0264 03a1 027d 0267  .}.|...d.d...}.g
+00002640: 007d 037a 7c74 03a0 047c 02a1 017d 027c  .}.z|t...|...}.|
+00002650: 02a0 0564 04a1 0172 427c 02a0 0564 04a1  ...d...rB|...d..
+00002660: 01a0 0664 05a1 016e 0264 067d 0464 07a0  ...d...n.d.}.d..
+00002670: 077c 04a1 017d 057c 02a0 0564 08a1 0172  .|...}.|...d...r
+00002680: 807c 02a0 0564 08a1 0144 005d 1a7d 067c  .|...d...D.].}.|
+00002690: 03a0 0864 07a0 077c 06a0 0664 05a1 01a1  ...d...|...d....
+000026a0: 01a1 0101 0071 6464 09a0 097c 03a1 017d  .....qdd...|...}
+000026b0: 0364 0aa0 077c 057c 03a1 027d 0757 006e  .d...|.|...}.W.n
+000026c0: 4604 0074 036a 0a6a 0b6b 0a72 be01 0001  F..t.j.j.k.r....
+000026d0: 0001 0064 0ba0 077c 016a 0c7c 02a1 027d  ...d...|.j.|...}
+000026e0: 0759 006e 2204 0074 0d6b 0a72 de01 0001  .Y.n"..t.k.r....
+000026f0: 0001 0064 0ba0 077c 016a 0c7c 02a1 027d  ...d...|.j.|...}
+00002700: 0759 006e 0258 007c 0753 0029 0c4e 7a05  .Y.n.X.|.S.).Nz.
+00002710: 7574 662d 387a 020d 0ada 00da 076d 6573  utf-8z.......mes
+00002720: 7361 6765 da01 2e7a 0a4e 6f20 6d65 7373  sage...z.No mess
+00002730: 6167 657a 037b 7d2e da06 6572 726f 7273  agez.{}...errors
+00002740: 7a10 2054 6865 2065 7272 6f72 2077 6173  z. The error was
+00002750: 3a20 7284 0000 007a 1841 6e20 6572 726f  : r....z.An erro
+00002760: 7220 6f63 6375 7272 6564 3a20 7b7d 207b  r occurred: {} {
+00002770: 7d29 0e72 4000 0000 da06 6465 636f 6465  }).r@.....decode
+00002780: da07 7265 706c 6163 6572 3e00 0000 da05  ..replacer>.....
+00002790: 6c6f 6164 7372 1e00 0000 da06 7273 7472  loadsr......rstr
+000027a0: 6970 723b 0000 0072 4c00 0000 7216 0000  ipr;...rL...r...
+000027b0: 00da 0764 6563 6f64 6572 7202 0000 0072  ...decoderr....r
+000027c0: 3d00 0000 da08 4b65 7945 7272 6f72 2908  =.....KeyError).
+000027d0: 724d 0000 0072 4300 0000 7282 0000 00da  rM...rC...r.....
+000027e0: 086d 6573 7361 6765 735a 1073 7472 6970  .messagesZ.strip
+000027f0: 7065 645f 6d65 7373 6167 655a 1170 7269  ped_messageZ.pri
+00002800: 6d61 7279 5f65 7272 6f72 5f6d 7367 da0d  mary_error_msg..
+00002810: 6572 726f 725f 6d65 7373 6167 6572 8500  error_messager..
+00002820: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00002830: 00da 175f 7072 6570 6172 655f 6572 726f  ..._prepare_erro
+00002840: 725f 7265 7370 6f6e 7365 5201 0000 7334  r_responseR...s4
+00002850: 0000 0000 010c 030c 0104 0202 010a 0208  ................
+00002860: ff12 0102 ff02 020a 010a 010e 0104 010e  ................
+00002870: ff06 040a 0210 0212 0208 0102 ff08 020e  ................
+00002880: 0208 0102 ff0a 027a 2941 7574 6f74 6173  .......z)Autotas
+00002890: 6b41 5049 436c 6965 6e74 2e5f 7072 6570  kAPIClient._prep
+000028a0: 6172 655f 6572 726f 725f 7265 7370 6f6e  are_error_respon
+000028b0: 7365 6302 0000 0000 0000 0000 0000 0003  sec.............
+000028c0: 0000 0003 0000 0043 0000 0073 7000 0000  .......C...sp...
+000028d0: 6401 6402 6901 7d02 7c00 6a00 7218 7c00  d.d.i.}.|.j.r.|.
+000028e0: 6a00 7c02 6403 3c00 7c00 6a01 7228 7c00  j.|.d.<.|.j.r(|.
+000028f0: 6a01 7c02 6404 3c00 7c00 6a02 7238 7c00  j.|.d.<.|.j.r8|.
+00002900: 6a02 7c02 6405 3c00 7c00 6a03 726c 7c01  j.|.d.<.|.j.rl|.
+00002910: a004 a100 6406 6b03 726c 7c00 a005 a100  ....d.k.rl|.....
+00002920: 0100 7c00 6a03 7264 7406 7c00 6a03 6a07  ..|.j.rdt.|.j.j.
+00002930: 8301 6e02 6400 7c02 6407 3c00 7c02 5300  ..n.d.|.d.<.|.S.
+00002940: 2908 4e7a 0c43 6f6e 7465 6e74 2d54 7970  ).Nz.Content-Typ
+00002950: 657a 1061 7070 6c69 6361 7469 6f6e 2f6a  ez.application/j
+00002960: 736f 6e5a 0855 7365 724e 616d 655a 0653  sonZ.UserNameZ.S
+00002970: 6563 7265 745a 1241 7069 496e 7465 6772  ecretZ.ApiIntegr
+00002980: 6174 696f 6e43 6f64 65da 0347 4554 5a17  ationCode..GETZ.
+00002990: 496d 7065 7273 6f6e 6174 696f 6e52 6573  ImpersonationRes
+000029a0: 6f75 7263 6549 6429 0872 2f00 0000 7275  ourceId).r/...ru
+000029b0: 0000 0072 7600 0000 727c 0000 00da 0575  ...rv...r|.....u
+000029c0: 7070 6572 da1f 6368 6563 6b5f 696d 7065  pper..check_impe
+000029d0: 7273 6f6e 6174 696f 6e5f 706f 7373 6962  rsonation_possib
+000029e0: 696c 6974 79da 0373 7472 da02 6964 2903  ility..str..id).
+000029f0: 724d 0000 0072 6b00 0000 da07 6865 6164  rM...rk.....head
+00002a00: 6572 7372 0f00 0000 720f 0000 0072 1000  ersr....r....r..
+00002a10: 0000 da0b 6765 745f 6865 6164 6572 7372  ....get_headersr
+00002a20: 0100 0073 2000 0000 0001 0802 0601 0a01  ...s ...........
+00002a30: 0601 0a01 0601 0a01 1202 0803 04fe 0401  ................
+00002a40: 06ff 0402 02fe 0604 7a1d 4175 746f 7461  ........z.Autota
+00002a50: 736b 4150 4943 6c69 656e 742e 6765 745f  skAPIClient.get_
+00002a60: 6865 6164 6572 7363 0300 0000 0000 0000  headersc........
+00002a70: 0000 0000 0700 0000 0600 0000 4300 0000  ............C...
+00002a80: 733e 0000 007c 016a 0072 1064 017c 016a  s>...|.j.r.d.|.j
+00002a90: 0069 016e 0474 0183 007d 037c 02a0 02a1  .i.n.t...}.|....
+00002aa0: 0044 005d 1a5c 027d 047d 057c 047d 067c  .D.].\.}.}.|.}.|
+00002ab0: 00a0 037c 037c 067c 05a1 037d 0371 1e7c  ...|.|.|...}.q.|
+00002ac0: 0353 00a9 024e 7298 0000 0029 0472 9800  .S...Nr....).r..
+00002ad0: 0000 da04 6469 6374 7256 0000 00da 145f  ....dictrV....._
+00002ae0: 666f 726d 6174 5f72 6571 7565 7374 5f62  format_request_b
+00002af0: 6f64 7929 0772 4d00 0000 da06 7265 636f  ody).rM.....reco
+00002b00: 7264 da0f 696e 7365 7274 6564 5f66 6965  rd..inserted_fie
+00002b10: 6c64 73da 0462 6f64 7972 3200 0000 7246  lds..bodyr2...rF
+00002b20: 0000 00da 036b 6579 720f 0000 0072 0f00  .....keyr....r..
+00002b30: 0000 7210 0000 00da 0e5f 666f 726d 6174  ..r......_format
+00002b40: 5f66 6965 6c64 7384 0100 0073 0a00 0000  _fields....s....
+00002b50: 0001 1602 1001 0401 1002 7a20 4175 746f  ..........z Auto
+00002b60: 7461 736b 4150 4943 6c69 656e 742e 5f66  taskAPIClient._f
+00002b70: 6f72 6d61 745f 6669 656c 6473 6304 0000  ormat_fieldsc...
+00002b80: 0000 0000 0000 0000 0004 0000 0008 0000  ................
+00002b90: 0043 0000 0073 ac00 0000 7400 7c03 7401  .C...s....t.|.t.
+00002ba0: 6a01 8302 722e 7c01 a002 7c02 7c03 a003  j...r.|...|.|...
+00002bb0: 7404 a005 6401 a101 a101 a006 6402 a101  t...d.......d...
+00002bc0: 6901 a101 0100 6e7a 7400 7c03 7407 6a08  i.....nzt.|.t.j.
+00002bd0: 8302 724c 7c01 a002 7c02 7c03 6a09 6901  ..rL|...|.|.j.i.
+00002be0: a101 0100 6e5c 7400 7c03 740a 6a0b 8302  ....n\t.|.t.j...
+00002bf0: 7274 7c01 a002 7c02 7c03 726a 740c 7c03  rt|...|.|.rjt.|.
+00002c00: 8301 6e02 6403 6901 a101 0100 6e34 7400  ..n.d.i.....n4t.
+00002c10: 7c03 740d 8302 728e 7c01 a002 7c02 7c03  |.t...r.|...|.|.
+00002c20: 6901 a101 0100 6e1a 7c01 a002 7c02 7c03  i.....n.|...|.|.
+00002c30: 72a0 740c 7c03 8301 6e02 6404 6901 a101  r.t.|...n.d.i...
+00002c40: 0100 7c01 5300 2905 4eda 0355 5443 7a12  ..|.S.).N..UTCz.
+00002c50: 2559 2d25 6d2d 2564 5425 483a 254d 3a25  %Y-%m-%dT%H:%M:%
+00002c60: 535a da01 3072 8700 0000 290e da0a 6973  SZ..0r....)...is
+00002c70: 696e 7374 616e 6365 da08 6461 7465 7469  instance..dateti
+00002c80: 6d65 7269 0000 00da 0a61 7374 696d 657a  meri.....astimez
+00002c90: 6f6e 65da 0470 7974 7ada 0874 696d 657a  one..pytz..timez
+00002ca0: 6f6e 65da 0873 7472 6674 696d 6572 0500  one..strftimer..
+00002cb0: 0000 da05 4d6f 6465 6c72 9800 0000 da07  ....Modelr......
+00002cc0: 6465 6369 6d61 6cda 0744 6563 696d 616c  decimal..Decimal
+00002cd0: 7297 0000 00da 0462 6f6f 6c29 0472 4d00  r......bool).rM.
+00002ce0: 0000 72a0 0000 0072 a100 0000 7246 0000  ..r....r....rF..
+00002cf0: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
+00002d00: 729d 0000 008d 0100 0073 3400 0000 0001  r........s4.....
+00002d10: 0c01 0401 0200 0401 08ff 0402 02fe 02ff  ................
+00002d20: 0806 0c01 0401 0200 04ff 0804 0c01 0401  ................
+00002d30: 12ff 0604 0a01 0401 06ff 0604 0401 12ff  ................
+00002d40: 0404 7a26 4175 746f 7461 736b 4150 4943  ..z&AutotaskAPIC
+00002d50: 6c69 656e 742e 5f66 6f72 6d61 745f 7265  lient._format_re
+00002d60: 7175 6573 745f 626f 6479 6303 0000 0000  quest_bodyc.....
+00002d70: 0000 0000 0000 0007 0000 0006 0000 0043  ...............C
+00002d80: 0000 0073 4e00 0000 7c01 6a00 7210 6401  ...sN...|.j.r.d.
+00002d90: 7c01 6a00 6901 6e04 7401 8300 7d03 7c02  |.j.i.n.t...}.|.
+00002da0: a002 a100 4400 5d2a 5c02 7d04 7d05 7c04  ....D.]*\.}.}.|.
+00002db0: 7c01 6a03 6b06 721e 7c01 6a03 7c04 1900  |.j.k.r.|.j.|...
+00002dc0: 7d06 7c00 a004 7c03 7c06 7c05 a103 7d03  }.|...|.|.|...}.
+00002dd0: 711e 7c03 5300 729b 0000 0029 0572 9800  q.|.S.r....).r..
+00002de0: 0000 729c 0000 0072 5600 0000 da0f 4155  ..r....rV.....AU
+00002df0: 544f 5441 534b 5f46 4945 4c44 5372 9d00  TOTASK_FIELDSr..
+00002e00: 0000 2907 724d 0000 005a 0a61 7069 5f65  ..).rM...Z.api_e
+00002e10: 6e74 6974 7972 9f00 0000 72a0 0000 0072  ntityr....r....r
+00002e20: 3200 0000 7246 0000 0072 a100 0000 720f  2...rF...r....r.
+00002e30: 0000 0072 0f00 0000 7210 0000 00da 155f  ...r....r......_
+00002e40: 6c65 6761 6379 5f66 6f72 6d61 745f 6669  legacy_format_fi
+00002e50: 656c 6473 aa01 0000 730c 0000 0000 0716  elds....s.......
+00002e60: 0210 010a 010a 0110 027a 2741 7574 6f74  .........z'Autot
+00002e70: 6173 6b41 5049 436c 6965 6e74 2e5f 6c65  askAPIClient._le
+00002e80: 6761 6379 5f66 6f72 6d61 745f 6669 656c  gacy_format_fiel
+00002e90: 6473 721e 0000 0063 0400 0000 0000 0000  dsr....c........
+00002ea0: 0000 0000 0900 0000 0600 0000 0f00 0000  ................
+00002eb0: 737a 0000 0074 0088 006a 0164 0119 0074  sz...t...j.d...t
+00002ec0: 0274 0374 0464 028d 0464 037c 0364 0366  .t.t.d...d.|.d.f
+00002ed0: 0387 0066 0164 0464 0584 0983 017d 067c  ...f.d.d.....}.|
+00002ee0: 0172 347c 017d 076e 2c88 006a 056a 0666  .r4|.}.n,..j.j.f
+00002ef0: 0064 067c 0369 017c 0597 028e 015c 027d  .d.|.i.|.....\.}
+00002f00: 0888 005f 0764 07a0 0888 00a0 09a1 007c  ..._.d.........|
+00002f10: 08a1 027d 077c 067c 0766 017c 027c 0388  ...}.|.|.f.|.|..
+00002f20: 006a 0764 089c 037c 0597 028e 0153 0029  .j.d...|.....S.)
+00002f30: 097a 8d0a 2020 2020 2020 2020 7265 7472  .z..        retr
+00002f40: 795f 636f 756e 7465 7220 6973 2061 2064  y_counter is a d
+00002f50: 6963 7420 696e 2074 6865 2066 6f72 6d20  ict in the form 
+00002f60: 7b27 636f 756e 7427 3a20 307d 2074 6861  {'count': 0} tha
+00002f70: 7420 6973 2070 6173 7365 6420 696e 0a20  t is passed in. 
+00002f80: 2020 2020 2020 2074 6f20 7665 7269 6679         to verify
+00002f90: 2074 6865 206e 756d 6265 7220 6f66 2061   the number of a
+00002fa0: 7474 656d 7074 7320 7468 6174 2077 6572  ttempts that wer
+00002fb0: 6520 6d61 6465 2e0a 2020 2020 2020 2020  e made..        
+00002fc0: 5a0c 6d61 785f 6174 7465 6d70 7473 2904  Z.max_attempts).
+00002fd0: 5a17 7374 6f70 5f6d 6178 5f61 7474 656d  Z.stop_max_attem
+00002fe0: 7074 5f6e 756d 6265 725a 1b77 6169 745f  pt_numberZ.wait_
+00002ff0: 6578 706f 6e65 6e74 6961 6c5f 6d75 6c74  exponential_mult
+00003000: 6970 6c69 6572 5a14 7761 6974 5f65 7870  iplierZ.wait_exp
+00003010: 6f6e 656e 7469 616c 5f6d 6178 5a12 7265  onential_maxZ.re
+00003020: 7472 795f 6f6e 5f65 7863 6570 7469 6f6e  try_on_exception
+00003030: 4e63 0400 0000 0000 0000 0000 0000 0900  Nc..............
+00003040: 0000 0a00 0000 1b00 0000 7316 0200 007c  ..........s....|
+00003050: 0173 0c64 0164 0269 017d 017c 0164 0105  .s.d.d.i.}.|.d..
+00003060: 0019 0064 0337 0003 003c 007a 2e88 00a0  ...d.7...<.z....
+00003070: 007c 007c 027c 03a1 0301 0074 016a 027c  .|.|.|.....t.j.|
+00003080: 027c 007c 0388 006a 0388 00a0 047c 02a1  .|.|...j.....|..
+00003090: 0164 048d 057d 0557 006e 4a04 0074 016a  .d...}.W.nJ..t.j
+000030a0: 056b 0a72 9401 007d 0601 007a 2a74 06a0  .k.r...}...z*t..
+000030b0: 0764 05a0 087c 02a0 09a1 007c 007c 06a1  .d...|.....|.|..
+000030c0: 03a1 0101 0074 0a64 06a0 087c 06a1 0183  .....t.d...|....
+000030d0: 0182 0157 0035 0064 007d 067e 0658 0059  ...W.5.d.}.~.X.Y
+000030e0: 006e 0258 0064 077c 056a 0b04 0003 006b  .n.X.d.|.j.....k
+000030f0: 0172 ae64 086b 0090 0172 0c6e 0401 006e  .r.d.k...r.n...n
+00003100: 5a7a 0a7c 05a0 0ca1 0057 0053 0004 0074  Zz.|.....W.S...t
+00003110: 0d6b 0a90 0172 0601 007d 0601 007a 2a74  .k...r...}...z*t
+00003120: 06a0 0764 09a0 087c 02a0 09a1 007c 007c  ...d...|.....|.|
+00003130: 06a1 03a1 0101 0074 0a64 06a0 087c 06a1  .......t.d...|..
+00003140: 0183 0182 0157 0035 0064 007d 067e 0658  .....W.5.d.}.~.X
+00003150: 0059 006e 0258 0090 016e 067c 056a 0b64  .Y.n.X...n.|.j.d
+00003160: 0a6b 0290 0172 7264 0ba0 087c 00a1 017d  .k...rrd...|...}
+00003170: 0774 06a0 0e7c 07a1 0101 007c 0164 0119  .t...|.....|.d..
+00003180: 0088 006a 0f6b 0190 0172 6874 1074 1183  ...j.k...rht.t..
+00003190: 017d 087c 0874 1264 0c64 0d8d 016b 0390  .}.|.t.d.d...k..
+000031a0: 0172 6874 06a0 1364 0ea1 0101 0074 0a7c  .rht...d.....t.|
+000031b0: 056a 1483 0182 0174 157c 0783 0182 016e  .j.....t.|.....n
+000031c0: a07c 056a 0b64 0f6b 0290 0172 9c88 00a0  .|.j.d.k...r....
+000031d0: 167c 05a1 0101 0074 1788 00a0 187c 05a1  .|.....t.....|..
+000031e0: 017c 056a 0b83 0282 016e 7664 107c 056a  .|.j.....nvd.|.j
+000031f0: 0b04 0003 006b 0190 0172 b664 116b 0090  .....k...r.d.k..
+00003200: 0172 d46e 0401 006e 1a88 00a0 167c 05a1  .r.n...n.....|..
+00003210: 0101 0074 1588 00a0 187c 05a1 0183 0182  ...t.....|......
+00003220: 016e 3e7c 056a 0b64 126b 0290 0172 fa88  .n>|.j.d.k...r..
+00003230: 00a0 167c 05a1 0101 0074 1988 00a0 187c  ...|.....t.....|
+00003240: 05a1 0183 0182 016e 1888 00a0 167c 05a1  .......n.....|..
+00003250: 0101 0074 0a88 00a0 187c 05a1 0183 0182  ...t.....|......
+00003260: 0164 0053 0029 134e 7270 0000 0072 0100  .d.S.).Nrp...r..
+00003270: 0000 7274 0000 0029 03da 0464 6174 6172  ..rt...)...datar
+00003280: 2200 0000 7299 0000 00fa 1952 6571 7565  "...r......Reque
+00003290: 7374 2066 6169 6c65 643a 207b 7d20 7b7d  st failed: {} {}
+000032a0: 3a20 7b7d fa02 7b7d 7235 0000 00e9 2c01  : {}..{}r5....,.
+000032b0: 0000 7a2c 5265 7175 6573 7420 6661 696c  ..z,Request fail
+000032c0: 6564 2064 7572 696e 6720 4a53 4f4e 2064  ed during JSON d
+000032d0: 6563 6f64 653a 207b 7d20 7b7d 3a20 7b7d  ecode: {} {}: {}
+000032e0: 6991 0100 007a 1855 6e61 7574 686f 7269  i....z.Unauthori
+000032f0: 7a65 6420 7265 7175 6573 743a 207b 7d54  zed request: {}T
+00003300: 722b 0000 007a 435a 6f6e 6520 696e 666f  r+...zCZone info
+00003310: 726d 6174 696f 6e20 6861 7320 6265 656e  rmation has been
+00003320: 2063 6861 6e67 6564 2c20 736f 2074 6869   changed, so thi
+00003330: 7320 7265 7175 6573 7420 7769 6c6c 2062  s request will b
+00003340: 6520 7265 7472 6965 642e e993 0100 00e9  e retried.......
+00003350: 9001 0000 e9f3 0100 0072 3600 0000 291a  .........r6...).
+00003360: da0b 6c6f 675f 6d65 7373 6167 6572 3c00  ..log_messager<.
+00003370: 0000 da07 7265 7175 6573 7472 2200 0000  ....requestr"...
+00003380: 729a 0000 0072 4100 0000 7239 0000 0072  r....rA...r9...r
+00003390: 8200 0000 723b 0000 0072 9500 0000 7209  ....r;...r....r.
+000033a0: 0000 0072 3d00 0000 723e 0000 0072 0200  ...r=...r>...r..
+000033b0: 0000 da07 7761 726e 696e 67da 104d 4158  ....warning..MAX
+000033c0: 5f34 3031 5f41 5454 454d 5054 5372 2000  _401_ATTEMPTSr .
+000033d0: 0000 7224 0000 0072 2d00 0000 da04 696e  ..r$...r-.....in
+000033e0: 666f 7240 0000 0072 1100 0000 7283 0000  for@...r....r...
+000033f0: 0072 1400 0000 7293 0000 0072 1200 0000  .r....r....r....
+00003400: 2909 7242 0000 00da 1572 6571 7565 7374  ).rB.....request
+00003410: 5f72 6574 7279 5f63 6f75 6e74 6572 da0e  _retry_counter..
+00003420: 7265 7175 6573 745f 6d65 7468 6f64 da0c  request_method..
+00003430: 7265 7175 6573 745f 626f 6479 726c 0000  request_bodyrl..
+00003440: 0072 4300 0000 7218 0000 0072 8500 0000  .rC...r....r....
+00003450: 5a0a 6361 6368 6564 5f75 726c 7252 0000  Z.cached_urlrR..
+00003460: 0072 0f00 0000 7210 0000 00da 0f5f 6665  .r....r......_fe
+00003470: 7463 685f 7265 736f 7572 6365 c001 0000  tch_resource....
+00003480: 7378 0000 0000 0704 0108 0110 0202 010e  sx..............
+00003490: 0204 0102 0102 0102 0104 0108 fb0a 0812  ................
+000034a0: 0108 0106 0002 0002 ff06 0220 021c 0102  ........... ....
+000034b0: 010a 0112 0104 0104 0106 0002 0002 ff02  ................
+000034c0: ff04 0424 020c 020a 010a 0110 0108 0110  ...$............
+000034d0: 010a 020a 010a 010c 010a 0102 0108 0104  ................
+000034e0: fe06 031e 010a 0102 0108 ff06 020c 010a  ................
+000034f0: 0102 0108 ff06 030a 0102 0108 ff7a 3941  .............z9A
+00003500: 7574 6f74 6173 6b41 5049 436c 6965 6e74  utotaskAPIClient
+00003510: 2e66 6574 6368 5f72 6573 6f75 7263 652e  .fetch_resource.
+00003520: 3c6c 6f63 616c 733e 2e5f 6665 7463 685f  <locals>._fetch_
+00003530: 7265 736f 7572 6365 726b 0000 00fa 047b  resourcerk.....{
+00003540: 7d7b 7d29 0372 bd00 0000 72be 0000 0072  }{}).r....r....r
+00003550: bf00 0000 290a 7207 0000 0072 7b00 0000  ....).r....r{...
+00003560: da22 5245 5452 595f 5741 4954 5f45 5850  ."RETRY_WAIT_EXP
+00003570: 4f4e 454e 5449 414c 5f4d 554c 5441 5050  ONENTIAL_MULTAPP
+00003580: 4c49 4552 da1a 5245 5452 595f 5741 4954  LIER..RETRY_WAIT
+00003590: 5f45 5850 4f4e 454e 5449 414c 5f4d 4158  _EXPONENTIAL_MAX
+000035a0: 721c 0000 0072 7d00 0000 7271 0000 0072  r....r}...rq...r
+000035b0: 7e00 0000 723b 0000 0072 8100 0000 2909  ~...r;...r....).
+000035c0: 724d 0000 00da 086e 6578 745f 7572 6c5a  rM.....next_urlZ
+000035d0: 0d72 6574 7279 5f63 6f75 6e74 6572 726b  .retry_counterrk
+000035e0: 0000 0072 1700 0000 726c 0000 0072 c000  ...r....rl...r..
+000035f0: 0000 7208 0000 005a 0e71 7565 7279 5f65  ..r....Z.query_e
+00003600: 6e64 706f 696e 7472 0f00 0000 7252 0000  ndpointr....rR..
+00003610: 0072 1000 0000 da0e 6665 7463 685f 7265  .r......fetch_re
+00003620: 736f 7572 6365 ba01 0000 732e 0000 0000  source....s.....
+00003630: 060a 0102 0102 0102 fd04 0402 0102 0002  ................
+00003640: ff10 3e04 0106 0414 ff08 0210 0202 0102  ..>.............
+00003650: ff02 0102 0102 0004 fe04 0202 fe7a 2041  .............z A
+00003660: 7574 6f74 6173 6b41 5049 436c 6965 6e74  utotaskAPIClient
+00003670: 2e66 6574 6368 5f72 6573 6f75 7263 6563  .fetch_resourcec
+00003680: 0400 0000 0000 0000 0000 0000 0500 0000  ................
+00003690: 0400 0000 4300 0000 733e 0000 007c 0372  ....C...s>...|.r
+000036a0: 087c 036e 0264 017d 0364 02a0 007c 02a0  .|.n.d.}.d...|..
+000036b0: 01a1 007c 01a1 027d 047c 0264 036b 0272  ...|...}.|.d.k.r
+000036c0: 3064 04a0 007c 047c 03a1 027d 0474 02a0  0d...|.|...}.t..
+000036d0: 037c 04a1 0101 0064 0053 0029 054e 7287  .|.....d.S.).Nr.
+000036e0: 0000 00fa 174d 616b 696e 6720 7b7d 2072  .....Making {} r
+000036f0: 6571 7565 7374 2074 6f20 7b7d 725a 0000  equest to {}rZ..
+00003700: 007a 147b 7d2e 2052 6571 7565 7374 2062  .z.{}. Request b
+00003710: 6f64 793a 207b 7d29 0472 3b00 0000 7295  ody: {}).r;...r.
+00003720: 0000 0072 3900 0000 723a 0000 0029 0572  ...r9...r:...).r
+00003730: 4d00 0000 726e 0000 0072 6b00 0000 72a0  M...rn...rk...r.
+00003740: 0000 005a 0e6c 6f67 6765 725f 6d65 7373  ...Z.logger_mess
+00003750: 6167 6572 0f00 0000 720f 0000 0072 1000  ager....r....r..
+00003760: 0000 72b8 0000 000e 0200 0073 0e00 0000  ..r........s....
+00003770: 0001 0c03 0eff 0202 0802 0aff 0203 7a1d  ..............z.
+00003780: 4175 746f 7461 736b 4150 4943 6c69 656e  AutotaskAPIClien
+00003790: 742e 6c6f 675f 6d65 7373 6167 6563 0100  t.log_messagec..
+000037a0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000037b0: 0000 4300 0000 7320 0000 007c 006a 0072  ..C...s ...|.j.r
+000037c0: 1c7c 006a 006a 01a0 027c 00a1 0173 1c74  .|.j.j...|...s.t
+000037d0: 0364 0183 0182 0164 0053 0029 024e 7a44  .d.....d.S.).NzD
+000037e0: 596f 7520 646f 206e 6f74 2068 6176 6520  You do not have 
+000037f0: 7468 6520 6164 6571 7561 7465 2070 6572  the adequate per
+00003800: 6d69 7373 696f 6e73 2028 696d 7065 7273  missions (impers
+00003810: 6f6e 6174 696f 6e20 6c69 6d69 7461 7469  onation limitati
+00003820: 6f6e 292e 2904 727c 0000 00da 0c6c 6963  on).).r|.....lic
+00003830: 656e 7365 5f74 7970 65da 1168 6173 5f69  ense_type..has_i
+00003840: 6d70 6572 736f 6e61 7469 6f6e 7215 0000  mpersonationr...
+00003850: 0072 5200 0000 720f 0000 0072 0f00 0000  .rR...r....r....
+00003860: 7210 0000 0072 9600 0000 1902 0000 730c  r....r........s.
+00003870: 0000 0000 010e 0102 ff04 0202 0102 ff7a  ...............z
+00003880: 3141 7574 6f74 6173 6b41 5049 436c 6965  1AutotaskAPIClie
+00003890: 6e74 2e63 6865 636b 5f69 6d70 6572 736f  nt.check_imperso
+000038a0: 6e61 7469 6f6e 5f70 6f73 7369 6269 6c69  nation_possibili
+000038b0: 7479 6304 0000 0000 0000 0000 0000 0008  tyc.............
+000038c0: 0000 000a 0000 0043 0000 0073 ec01 0000  .......C...s....
+000038d0: 7a32 7400 a001 6401 a002 7c01 7c02 a102  z2t...d...|.|...
+000038e0: a101 0100 7403 6a04 7c01 7c02 7c03 7c00  ....t.j.|.|.|.|.
+000038f0: 6a05 7c00 a006 7c01 a101 6402 8d05 7d04  j.|...|...d...}.
+00003900: 5700 6e7e 0400 7407 6b0a 726c 0100 7d05  W.n~..t.k.rl..}.
+00003910: 0100 7a1c 7400 a008 6403 a002 7c01 7c02  ..z.t...d...|.|.
+00003920: 7c05 a103 a101 0100 7c05 8201 5700 3500  |.......|...W.5.
+00003930: 6404 7d05 7e05 5800 5900 6e46 0400 7403  d.}.~.X.Y.nF..t.
+00003940: 6a09 6b0a 72b0 0100 7d05 0100 7a26 7400  j.k.r...}...z&t.
+00003950: a008 6403 a002 7c01 7c02 7c05 a103 a101  ..d...|.|.|.....
+00003960: 0100 740a 6405 a002 7c05 a101 8301 8201  ..t.d...|.......
+00003970: 5700 3500 6404 7d05 7e05 5800 5900 6e02  W.5.d.}.~.X.Y.n.
+00003980: 5800 7c04 6a0b 6406 6b02 72c0 6404 5300  X.|.j.d.k.r.d.S.
+00003990: 6407 7c04 6a0b 0400 0300 6b01 72d6 6408  d.|.j.....k.r.d.
+000039a0: 6b00 72e2 6e04 0100 6e08 7c04 a00c a100  k.r.n...n.|.....
+000039b0: 5300 7c04 6a0b 6409 6b02 9001 720c 7c00  S.|.j.d.k...r.|.
+000039c0: a00d 7c04 a101 0100 740e 7c00 a00f 7c04  ..|.....t.|...|.
+000039d0: a101 7c04 6a0b 8302 8201 6edc 7c04 6a0b  ..|.j.....n.|.j.
+000039e0: 640a 6b02 9001 7238 640b a002 7c04 6a10  d.k...r8d...|.j.
+000039f0: a101 7d06 7400 a011 7c06 a101 0100 7412  ..}.t...|.....t.
+00003a00: 7c06 8301 8201 6eb0 640c 7c04 6a0b 0400  |.....n.d.|.j...
+00003a10: 0300 6b01 9001 7252 640d 6b00 9001 7270  ..k...rRd.k...rp
+00003a20: 6e04 0100 6e1a 7c00 a00d 7c04 a101 0100  n...n.|...|.....
+00003a30: 7413 7c00 a00f 7c04 a101 8301 8201 6e78  t.|...|.......nx
+00003a40: 7c04 6a0b 640e 6b02 9001 72d6 7c00 a00d  |.j.d.k...r.|...
+00003a50: 7c04 a101 0100 7c00 a00f 7c04 a101 7d07  |.....|...|...}.
+00003a60: 7414 7c07 6b06 9001 72b6 7c00 6a15 9001  t.|.k...r.|.j...
+00003a70: 72ac 7c00 a016 7c07 a101 7d07 740e 7c07  r.|...|...}.t.|.
+00003a80: 8301 8201 6e1e 7417 7c07 6b06 9001 72cc  ....n.t.|.k...r.
+00003a90: 7412 7c07 640a 8302 8201 6e08 7418 7c07  t.|.d.....n.t.|.
+00003aa0: 8301 8201 6e12 7c00 a00d 7c04 a101 0100  ....n.|...|.....
+00003ab0: 740a 7c04 8301 8201 6404 5300 290f 7a51  t.|.....d.S.).zQ
+00003ac0: 0a20 2020 2020 2020 2049 7373 7565 2074  .        Issue t
+00003ad0: 6865 2067 6976 656e 2074 7970 6520 6f66  he given type of
+00003ae0: 2072 6571 7565 7374 2074 6f20 7468 6520   request to the 
+00003af0: 7370 6563 6966 6965 6420 5245 5354 2065  specified REST e
+00003b00: 6e64 706f 696e 742e 0a20 2020 2020 2020  ndpoint..       
+00003b10: 2072 c600 0000 2903 723e 0000 0072 2200   r....).r>...r".
+00003b20: 0000 7299 0000 0072 b200 0000 4e72 b300  ..r....r....Nr..
+00003b30: 0000 e9cc 0000 0072 3500 0000 72b4 0000  .......r5...r...
+00003b40: 0072 b500 0000 6994 0100 00fa 1652 6573  .r....i......Res
+00003b50: 6f75 7263 6520 6e6f 7420 666f 756e 643a  ource not found:
+00003b60: 207b 7d72 b600 0000 72b7 0000 0072 3600   {}r....r....r6.
+00003b70: 0000 2919 7239 0000 0072 3a00 0000 723b  ..).r9...r:...r;
+00003b80: 0000 0072 3c00 0000 72b9 0000 0072 2200  ...r<...r....r".
+00003b90: 0000 729a 0000 0072 1500 0000 7282 0000  ..r....r....r...
+00003ba0: 0072 4100 0000 7209 0000 0072 3d00 0000  .rA...r....r=...
+00003bb0: 723e 0000 0072 8300 0000 7214 0000 0072  r>...r....r....r
+00003bc0: 9300 0000 7208 0000 0072 ba00 0000 7213  ....r....r....r.
+00003bd0: 0000 0072 1100 0000 da17 464f 5242 4944  ...r......FORBID
+00003be0: 4445 4e5f 4552 524f 525f 4d45 5353 4147  DEN_ERROR_MESSAG
+00003bf0: 4572 7c00 0000 7286 0000 00da 174e 4f5f  Er|...r......NO_
+00003c00: 5245 434f 5244 5f45 5252 4f52 5f4d 4553  RECORD_ERROR_MES
+00003c10: 5341 4745 7212 0000 0029 0872 4d00 0000  SAGEr....).rM...
+00003c20: 726b 0000 0072 4200 0000 72a0 0000 0072  rk...rB...r....r
+00003c30: 4300 0000 7218 0000 0072 8500 0000 5a0e  C...r....r....Z.
+00003c40: 7072 6570 6172 6564 5f65 7272 6f72 720f  prepared_errorr.
+00003c50: 0000 0072 0f00 0000 7210 0000 0072 b900  ...r....r....r..
+00003c60: 0000 2002 0000 736c 0000 0000 0402 0104  .. ...sl........
+00003c70: 010a ff04 0404 0102 0102 0102 0104 0108  ................
+00003c80: fb0a 0710 0104 010c ff04 0314 0112 0104  ................
+00003c90: 010c ff04 0320 020a 0104 011a 0108 010c  ..... ..........
+00003ca0: 010a 0102 0108 0004 ff06 020c 010c 010a  ................
+00003cb0: 010a 011e 010a 0102 0108 ff06 020c 010a  ................
+00003cc0: 010a 0a0a 0108 0104 0102 ff04 030a 010a  ................
+00003cd0: 010c 020a 020a 017a 1941 7574 6f74 6173  .......z.Autotas
+00003ce0: 6b41 5049 436c 6965 6e74 2e72 6571 7565  kAPIClient.reque
+00003cf0: 7374 6302 0000 0000 0000 0000 0000 0002  stc.............
+00003d00: 0000 0003 0000 0043 0000 0073 1a00 0000  .......C...s....
+00003d10: 7c00 6a00 a001 7c01 a101 0100 7402 7c00  |.j...|.....t.|.
+00003d20: 6a00 8301 6401 1800 5300 2902 4e72 7400  j...d...S.).Nrt.
+00003d30: 0000 2903 727d 0000 0072 7200 0000 7250  ..).r}...rr...rP
+00003d40: 0000 0072 5700 0000 720f 0000 0072 0f00  ...rW...r....r..
+00003d50: 0000 7210 0000 00da 0d61 6464 5f63 6f6e  ..r......add_con
+00003d60: 6469 7469 6f6e 6502 0000 7304 0000 0000  ditione...s.....
+00003d70: 010c 017a 1f41 7574 6f74 6173 6b41 5049  ...z.AutotaskAPI
+00003d80: 436c 6965 6e74 2e61 6464 5f63 6f6e 6469  Client.add_condi
+00003d90: 7469 6f6e 6301 0000 0000 0000 0000 0000  tionc...........
+00003da0: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
+00003db0: 0000 7c00 6a00 5300 7229 0000 00a9 0172  ..|.j.S.r).....r
+00003dc0: 7d00 0000 7252 0000 0072 0f00 0000 720f  }...rR...r....r.
+00003dd0: 0000 0072 1000 0000 da0e 6765 745f 636f  ...r......get_co
+00003de0: 6e64 6974 696f 6e73 6902 0000 7302 0000  nditionsi...s...
+00003df0: 0000 017a 2041 7574 6f74 6173 6b41 5049  ...z AutotaskAPI
+00003e00: 436c 6965 6e74 2e67 6574 5f63 6f6e 6469  Client.get_condi
+00003e10: 7469 6f6e 7363 0200 0000 0000 0000 0000  tionsc..........
+00003e20: 0000 0200 0000 0200 0000 4300 0000 730c  ..........C...s.
+00003e30: 0000 007c 006a 007c 013d 0064 0053 0072  ...|.j.|.=.d.S.r
+00003e40: 2900 0000 72ce 0000 0029 0272 4d00 0000  )...r....).rM...
+00003e50: da05 696e 6465 7872 0f00 0000 720f 0000  ..indexr....r...
+00003e60: 0072 1000 0000 da10 7265 6d6f 7665 5f63  .r......remove_c
+00003e70: 6f6e 6469 7469 6f6e 6c02 0000 7302 0000  onditionl...s...
+00003e80: 0000 017a 2241 7574 6f74 6173 6b41 5049  ...z"AutotaskAPI
+00003e90: 436c 6965 6e74 2e72 656d 6f76 655f 636f  Client.remove_co
+00003ea0: 6e64 6974 696f 6e63 0100 0000 0000 0000  nditionc........
+00003eb0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00003ec0: 730c 0000 0074 0083 007c 005f 0164 0053  s....t...|._.d.S
+00003ed0: 0072 2900 0000 2902 7258 0000 0072 7d00  .r)...).rX...r}.
+00003ee0: 0000 7252 0000 0072 0f00 0000 720f 0000  ..rR...r....r...
+00003ef0: 0072 1000 0000 da10 636c 6561 725f 636f  .r......clear_co
+00003f00: 6e64 6974 696f 6e73 6f02 0000 7302 0000  nditionso...s...
+00003f10: 0000 017a 2241 7574 6f74 6173 6b41 5049  ...z"AutotaskAPI
+00003f20: 436c 6965 6e74 2e63 6c65 6172 5f63 6f6e  Client.clear_con
+00003f30: 6469 7469 6f6e 7363 0200 0000 0000 0000  ditionsc........
+00003f40: 0000 0000 0400 0000 0300 0000 4f00 0000  ............O...
+00003f50: 7312 0000 007c 006a 007c 0166 017c 029e  s....|.j.|.f.|..
+00003f60: 027c 038e 0153 0072 2900 0000 a901 72c5  .|...S.r).....r.
+00003f70: 0000 00a9 0472 4d00 0000 72c4 0000 0072  .....rM...r....r
+00003f80: 1700 0000 726c 0000 0072 0f00 0000 720f  ....rl...r....r.
+00003f90: 0000 0072 1000 0000 721e 0000 0072 0200  ...r....r....r..
+00003fa0: 0073 0200 0000 0001 7a15 4175 746f 7461  .s......z.Autota
+00003fb0: 736b 4150 4943 6c69 656e 742e 6765 7463  skAPIClient.getc
+00003fc0: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+00003fd0: 0400 0000 4300 0000 7342 0000 0064 01a0  ....C...sB...d..
+00003fe0: 007c 00a0 01a1 007c 01a1 027d 027c 00a0  .|.....|...}.|..
+00003ff0: 027c 02a1 017d 037c 0364 0219 0073 3e64  .|...}.|.d...s>d
+00004000: 03a0 007c 02a1 017d 0474 03a0 047c 04a1  ...|...}.t...|..
+00004010: 0101 0074 057c 0483 0182 017c 0353 0029  ...t.|.....|.S.)
+00004020: 044e 72c1 0000 00da 0469 7465 6d72 ca00  .Nr......itemr..
+00004030: 0000 2906 723b 0000 0072 8100 0000 72c5  ..).r;...r....r.
+00004040: 0000 0072 3900 0000 72ba 0000 0072 1300  ...r9...r....r..
+00004050: 0000 2905 724d 0000 005a 0b69 6e73 7461  ..).rM...Z.insta
+00004060: 6e63 655f 6964 7242 0000 0072 4300 0000  nce_idrB...rC...
+00004070: 7285 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+00004080: 1000 0000 da0a 6765 745f 7369 6e67 6c65  ......get_single
+00004090: 7502 0000 730e 0000 0000 0110 010a 0108  u...s...........
+000040a0: 010a 010a 0108 017a 1c41 7574 6f74 6173  .......z.Autotas
+000040b0: 6b41 5049 436c 6965 6e74 2e67 6574 5f73  kAPIClient.get_s
+000040c0: 696e 676c 6563 0300 0000 0000 0000 0000  inglec..........
+000040d0: 0000 0400 0000 0500 0000 4300 0000 731e  ..........C...s.
+000040e0: 0000 007c 00a0 007c 017c 02a1 027d 037c  ...|...|.|...}.|
+000040f0: 00a0 0164 017c 00a0 02a1 007c 03a1 0353  ...d.|.....|...S
+00004100: 00a9 024e da05 7061 7463 6829 0372 b000  ...N..patch).r..
+00004110: 0000 72b9 0000 0072 8100 0000 a904 724d  ..r....r......rM
+00004120: 0000 00da 0869 6e73 7461 6e63 65da 0e63  .....instance..c
+00004130: 6861 6e67 6564 5f66 6965 6c64 7372 a000  hanged_fieldsr..
+00004140: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00004150: 0072 6900 0000 7e02 0000 7304 0000 0000  .ri...~...s.....
+00004160: 010c 017a 1841 7574 6f74 6173 6b41 5049  ...z.AutotaskAPI
+00004170: 436c 6965 6e74 2e75 7064 6174 6563 0200  Client.updatec..
+00004180: 0000 0000 0000 0000 0000 0500 0000 0500  ................
+00004190: 0000 4b00 0000 7328 0000 007c 00a0 007c  ..K...s(...|...|
+000041a0: 017c 02a1 027d 037c 00a0 0164 017c 00a0  .|...}.|...d.|..
+000041b0: 02a1 007c 03a1 037d 047c 04a0 0364 02a1  ...|...}.|...d..
+000041c0: 0153 00a9 034e 725a 0000 00da 0669 7465  .S...NrZ.....ite
+000041d0: 6d49 6429 0472 b000 0000 72b9 0000 0072  mId).r....r....r
+000041e0: 8100 0000 721e 0000 0029 0572 4d00 0000  ....r....).rM...
+000041f0: 72da 0000 0072 6c00 0000 72a0 0000 0072  r....rl...r....r
+00004200: 4300 0000 720f 0000 0072 0f00 0000 7210  C...r....r....r.
+00004210: 0000 00da 0663 7265 6174 6582 0200 0073  .....create....s
+00004220: 0600 0000 0001 0c02 1201 7a18 4175 746f  ..........z.Auto
+00004230: 7461 736b 4150 4943 6c69 656e 742e 6372  taskAPIClient.cr
+00004240: 6561 7465 6303 0000 0000 0000 0000 0000  eatec...........
+00004250: 0005 0000 0004 0000 0043 0000 0073 2800  .........C...s(.
+00004260: 0000 7c00 a000 a100 7401 7c01 6a02 8301  ..|.....t.|.j...
+00004270: 1700 7d03 7c00 a003 6401 7c03 a102 7d04  ..}.|...d.|...}.
+00004280: 7c04 a004 6402 a101 5300 2903 4eda 0664  |...d...S.).N..d
+00004290: 656c 6574 6572 dd00 0000 2905 7281 0000  eleter....).r...
+000042a0: 0072 9700 0000 7298 0000 0072 b900 0000  .r....r....r....
+000042b0: 721e 0000 00a9 0572 4d00 0000 72da 0000  r......rM...r...
+000042c0: 00da 0670 6172 656e 7472 4200 0000 7243  ...parentrB...rC
+000042d0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+000042e0: 0000 72df 0000 0088 0200 0073 0600 0000  ..r........s....
+000042f0: 0001 1201 0c02 7a18 4175 746f 7461 736b  ......z.Autotask
+00004300: 4150 4943 6c69 656e 742e 6465 6c65 7465  APIClient.delete
+00004310: 2906 4e4e 4e4e 4e4e 2901 4e29 034e 4e72  ).NNNNNN).N).NNr
+00004320: 1e00 0000 2901 4e29 014e 291d 720b 0000  ....).N).N).r...
+00004330: 0072 0c00 0000 720d 0000 0072 7800 0000  .r....r....rx...
+00004340: 72bb 0000 0072 4f00 0000 da08 7072 6f70  r....rO.....prop
+00004350: 6572 7479 727f 0000 0072 8100 0000 7283  ertyr....r....r.
+00004360: 0000 0072 8600 0000 7293 0000 0072 9a00  ...r....r....r..
+00004370: 0000 72a2 0000 0072 9d00 0000 72b0 0000  ..r....r....r...
+00004380: 0072 c500 0000 72b8 0000 0072 9600 0000  .r....r....r....
+00004390: 72b9 0000 0072 cd00 0000 72cf 0000 0072  r....r....r....r
+000043a0: d100 0000 72d2 0000 0072 1e00 0000 72d6  ....r....r....r.
+000043b0: 0000 0072 6900 0000 72de 0000 0072 df00  ...ri...r....r..
+000043c0: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+000043d0: 0072 1000 0000 7273 0000 000b 0100 0073  .r....rs.......s
+000043e0: 4000 0000 0801 0401 0404 0001 0001 0001  @...............
+000043f0: 0001 0001 00f9 0a27 0201 0a06 0a09 0804  .......'........
+00004400: 0808 0820 0812 0809 081d 0810 0a54 080b  ... .........T..
+00004410: 0807 0a45 0804 0803 0803 0803 0803 0809  ...E............
+00004420: 0804 0806 7273 0000 0063 0000 0000 0000  ....rs...c......
+00004430: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00004440: 0000 733c 0000 0065 005a 0164 005a 0264  ..s<...e.Z.d.Z.d
+00004450: 015a 0364 015a 0464 0264 0384 005a 0564  .Z.d.Z.d.d...Z.d
+00004460: 0464 0584 005a 0664 0664 0784 005a 0764  .d...Z.d.d...Z.d
+00004470: 0864 0984 005a 0864 0a64 0b84 005a 0964  .d...Z.d.d...Z.d
+00004480: 0153 0029 0cda 0d43 6869 6c64 4150 494d  .S.)...ChildAPIM
+00004490: 6978 696e 4e63 0200 0000 0000 0000 0000  ixinNc..........
+000044a0: 0000 0200 0000 0600 0000 4300 0000 7316  ..........C...s.
+000044b0: 0000 0064 01a0 007c 006a 017c 006a 027c  ...d...|.j.|.j.|
+000044c0: 017c 006a 03a1 0453 0029 024e 7a0a 7b7d  .|.j...S.).Nz.{}
+000044d0: 7b7d 2f7b 7d2f 7b7d 2904 723b 0000 0072  {}/{}/{}).r;...r
+000044e0: 7f00 0000 da0a 5041 5245 4e54 5f41 5049  ......PARENT_API
+000044f0: da09 4348 494c 445f 4150 4929 0272 4d00  ..CHILD_API).rM.
+00004500: 0000 5a09 7061 7265 6e74 5f69 6472 0f00  ..Z.parent_idr..
+00004510: 0000 720f 0000 0072 1000 0000 da0d 6765  ..r....r......ge
+00004520: 745f 6368 696c 645f 7572 6c93 0200 0073  t_child_url....s
+00004530: 0c00 0000 0001 0401 0401 0401 0201 04fc  ................
+00004540: 7a1b 4368 696c 6441 5049 4d69 7869 6e2e  z.ChildAPIMixin.
+00004550: 6765 745f 6368 696c 645f 7572 6c63 0400  get_child_urlc..
+00004560: 0000 0000 0000 0000 0000 0600 0000 0500  ................
+00004570: 0000 4300 0000 7326 0000 007c 00a0 007c  ..C...s&...|...|
+00004580: 026a 01a1 017d 047c 00a0 027c 017c 03a1  .j...}.|...|.|..
+00004590: 027d 057c 00a0 0364 017c 047c 05a1 0353  .}.|...d.|.|...S
+000045a0: 0072 d700 0000 2904 72e6 0000 0072 9800  .r....).r....r..
+000045b0: 0000 72b0 0000 0072 b900 0000 a906 724d  ..r....r......rM
+000045c0: 0000 0072 da00 0000 72e1 0000 0072 db00  ...r....r....r..
+000045d0: 0000 7242 0000 0072 a000 0000 720f 0000  ..rB...r....r...
+000045e0: 0072 0f00 0000 7210 0000 0072 6900 0000  .r....r....ri...
+000045f0: 9b02 0000 7306 0000 0000 020c 010c 017a  ....s..........z
+00004600: 1443 6869 6c64 4150 494d 6978 696e 2e75  .ChildAPIMixin.u
+00004610: 7064 6174 6563 0300 0000 0000 0000 0000  pdatec..........
+00004620: 0000 0700 0000 0500 0000 4b00 0000 7330  ..........K...s0
+00004630: 0000 007c 00a0 007c 026a 01a1 017d 047c  ...|...|.j...}.|
+00004640: 00a0 027c 017c 03a1 027d 057c 00a0 0364  ...|.|...}.|...d
+00004650: 017c 047c 05a1 037d 067c 06a0 0464 02a1  .|.|...}.|...d..
+00004660: 0153 0072 dc00 0000 2905 72e6 0000 0072  .S.r....).r....r
+00004670: 9800 0000 72b0 0000 0072 b900 0000 721e  ....r....r....r.
+00004680: 0000 0029 0772 4d00 0000 72da 0000 0072  ...).rM...r....r
+00004690: e100 0000 726c 0000 0072 4200 0000 72a0  ....rl...rB...r.
+000046a0: 0000 0072 4300 0000 720f 0000 0072 0f00  ...rC...r....r..
+000046b0: 0000 7210 0000 0072 de00 0000 a102 0000  ..r....r........
+000046c0: 7308 0000 0000 010c 010c 010e 017a 1443  s............z.C
+000046d0: 6869 6c64 4150 494d 6978 696e 2e63 7265  hildAPIMixin.cre
+000046e0: 6174 6563 0300 0000 0000 0000 0000 0000  atec............
+000046f0: 0500 0000 0500 0000 4300 0000 7330 0000  ........C...s0..
+00004700: 0064 01a0 007c 00a0 017c 026a 02a1 0174  .d...|...|.j...t
+00004710: 037c 016a 0283 01a1 027d 037c 00a0 0464  .|.j.....}.|...d
+00004720: 027c 03a1 027d 047c 04a0 0564 03a1 0153  .|...}.|...d...S
+00004730: 0029 044e fa05 7b7d 2f7b 7d72 df00 0000  .).N..{}/{}r....
+00004740: 72dd 0000 0029 0672 3b00 0000 72e6 0000  r....).r;...r...
+00004750: 0072 9800 0000 7297 0000 0072 b900 0000  .r....r....r....
+00004760: 721e 0000 0072 e000 0000 720f 0000 0072  r....r....r....r
+00004770: 0f00 0000 7210 0000 0072 df00 0000 a702  ....r....r......
+00004780: 0000 730c 0000 0000 0104 010a 0108 fe04  ..s.............
+00004790: 040c 027a 1443 6869 6c64 4150 494d 6978  ...z.ChildAPIMix
+000047a0: 696e 2e64 656c 6574 6563 0200 0000 0000  in.deletec......
+000047b0: 0000 0000 0000 0400 0000 0400 0000 4f00  ..............O.
+000047c0: 0000 731a 0000 007c 006a 007c 0166 017c  ..s....|.j.|.f.|
+000047d0: 029e 0264 0164 0269 017c 0397 028e 0153  ...d.d.i.|.....S
+000047e0: 00a9 034e 726b 0000 0072 5a00 0000 72d3  ...Nrk...rZ...r.
+000047f0: 0000 0072 d400 0000 720f 0000 0072 0f00  ...r....r....r..
+00004800: 0000 7210 0000 0072 1e00 0000 b102 0000  ..r....r........
+00004810: 7302 0000 0000 017a 1143 6869 6c64 4150  s......z.ChildAP
+00004820: 494d 6978 696e 2e67 6574 290a 720b 0000  IMixin.get).r...
+00004830: 0072 0c00 0000 720d 0000 0072 e400 0000  .r....r....r....
+00004840: 72e5 0000 0072 e600 0000 7269 0000 0072  r....r....ri...r
+00004850: de00 0000 72df 0000 0072 1e00 0000 720f  ....r....r....r.
+00004860: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+00004870: 0000 72e3 0000 008f 0200 0073 0e00 0000  ..r........s....
+00004880: 0801 0401 0402 0808 0806 0806 080a 72e3  ..............r.
+00004890: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000048a0: 0000 0000 0100 0000 4000 0000 7310 0000  ........@...s...
+000048b0: 0065 005a 0164 005a 0264 015a 0364 0253  .e.Z.d.Z.d.Z.d.S
+000048c0: 0029 03da 1143 6f6e 7461 6374 7341 5049  .)...ContactsAPI
+000048d0: 436c 6965 6e74 5a08 436f 6e74 6163 7473  ClientZ.Contacts
+000048e0: 4ea9 0472 0b00 0000 720c 0000 0072 0d00  N..r....r....r..
+000048f0: 0000 7278 0000 0072 0f00 0000 720f 0000  ..rx...r....r...
+00004900: 0072 0f00 0000 7210 0000 0072 ea00 0000  .r....r....r....
+00004910: b502 0000 7302 0000 0008 0172 ea00 0000  ....s......r....
+00004920: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00004930: 0001 0000 0040 0000 0073 1000 0000 6500  .....@...s....e.
+00004940: 5a01 6400 5a02 6401 5a03 6402 5300 2903  Z.d.Z.d.Z.d.S.).
+00004950: da0e 526f 6c65 7341 5049 436c 6965 6e74  ..RolesAPIClient
+00004960: 5a05 526f 6c65 734e 72eb 0000 0072 0f00  Z.RolesNr....r..
+00004970: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00004980: 0072 ec00 0000 b902 0000 7302 0000 0008  .r........s.....
+00004990: 0172 ec00 0000 6300 0000 0000 0000 0000  .r....c.........
+000049a0: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
+000049b0: 1000 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+000049c0: 6402 5300 2903 da14 4465 7061 7274 6d65  d.S.)...Departme
+000049d0: 6e74 7341 5049 436c 6965 6e74 5a0b 4465  ntsAPIClientZ.De
+000049e0: 7061 7274 6d65 6e74 734e 72eb 0000 0072  partmentsNr....r
+000049f0: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+00004a00: 0000 0072 ed00 0000 bd02 0000 7302 0000  ...r........s...
+00004a10: 0008 0172 ed00 0000 6300 0000 0000 0000  ...r....c.......
+00004a20: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+00004a30: 0073 1000 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00004a40: 5a03 6402 5300 2903 da21 5265 736f 7572  Z.d.S.)..!Resour
+00004a50: 6365 5365 7276 6963 6544 6573 6b52 6f6c  ceServiceDeskRol
+00004a60: 6573 4150 4943 6c69 656e 745a 1852 6573  esAPIClientZ.Res
+00004a70: 6f75 7263 6553 6572 7669 6365 4465 736b  ourceServiceDesk
+00004a80: 526f 6c65 734e 72eb 0000 0072 0f00 0000  RolesNr....r....
+00004a90: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00004aa0: ee00 0000 c102 0000 7302 0000 0008 0172  ........s......r
+00004ab0: ee00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00004ac0: 0000 0000 0001 0000 0040 0000 0073 1000  .........@...s..
+00004ad0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00004ae0: 5300 2903 da20 5265 736f 7572 6365 526f  S.).. ResourceRo
+00004af0: 6c65 4465 7061 7274 6d65 6e74 7341 5049  leDepartmentsAPI
+00004b00: 436c 6965 6e74 5a17 5265 736f 7572 6365  ClientZ.Resource
+00004b10: 526f 6c65 4465 7061 7274 6d65 6e74 734e  RoleDepartmentsN
+00004b20: 72eb 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+00004b30: 0f00 0000 7210 0000 0072 ef00 0000 c502  ....r....r......
+00004b40: 0000 7302 0000 0008 0172 ef00 0000 6300  ..s......r....c.
+00004b50: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00004b60: 0000 0040 0000 0073 2000 0000 6500 5a01  ...@...s ...e.Z.
+00004b70: 6400 5a02 6401 5a03 6402 6403 8400 5a04  d.Z.d.Z.d.d...Z.
+00004b80: 6404 6405 8400 5a05 6406 5300 2907 da10  d.d...Z.d.S.)...
+00004b90: 5469 636b 6574 7341 5049 436c 6965 6e74  TicketsAPIClient
+00004ba0: da07 5469 636b 6574 7363 0200 0000 0000  ..Ticketsc......
+00004bb0: 0000 0000 0000 0400 0000 0300 0000 4f00  ..............O.
+00004bc0: 0000 7312 0000 007c 006a 007c 0166 017c  ..s....|.j.|.f.|
+00004bd0: 029e 027c 038e 0153 0072 2900 0000 72d3  ...|...S.r)...r.
+00004be0: 0000 0072 d400 0000 720f 0000 0072 0f00  ...r....r....r..
+00004bf0: 0000 7210 0000 0072 7000 0000 cc02 0000  ..r....rp.......
+00004c00: 7302 0000 0000 027a 1654 6963 6b65 7473  s......z.Tickets
+00004c10: 4150 4943 6c69 656e 742e 636f 756e 7463  APIClient.countc
+00004c20: 0300 0000 0000 0000 0000 0000 0400 0000  ................
+00004c30: 0500 0000 4300 0000 731e 0000 007c 00a0  ....C...s....|..
+00004c40: 007c 017c 02a1 027d 037c 00a0 0164 017c  .|.|...}.|...d.|
+00004c50: 00a0 02a1 007c 03a1 0353 0072 d700 0000  .....|...S.r....
+00004c60: a903 72a2 0000 0072 b900 0000 7281 0000  ..r....r....r...
+00004c70: 0072 d900 0000 720f 0000 0072 0f00 0000  .r....r....r....
+00004c80: 7210 0000 0072 6900 0000 d002 0000 7304  r....ri.......s.
+00004c90: 0000 0000 030c 017a 1754 6963 6b65 7473  .......z.Tickets
+00004ca0: 4150 4943 6c69 656e 742e 7570 6461 7465  APIClient.update
+00004cb0: 4e29 0672 0b00 0000 720c 0000 0072 0d00  N).r....r....r..
+00004cc0: 0000 7278 0000 0072 7000 0000 7269 0000  ..rx...rp...ri..
+00004cd0: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
+00004ce0: 7210 0000 0072 f000 0000 c902 0000 7306  r....r........s.
+00004cf0: 0000 0008 0104 0208 0472 f000 0000 6300  .........r....c.
+00004d00: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00004d10: 0000 0040 0000 0073 1000 0000 6500 5a01  ...@...s....e.Z.
+00004d20: 6400 5a02 6401 5a03 6402 5300 2903 da15  d.Z.d.Z.d.S.)...
+00004d30: 4269 6c6c 696e 6743 6f64 6573 4150 4943  BillingCodesAPIC
+00004d40: 6c69 656e 74da 0c42 696c 6c69 6e67 436f  lient..BillingCo
+00004d50: 6465 734e 72eb 0000 0072 0f00 0000 720f  desNr....r....r.
+00004d60: 0000 0072 0f00 0000 7210 0000 0072 f300  ...r....r....r..
+00004d70: 0000 d702 0000 7302 0000 0008 0172 f300  ......s......r..
+00004d80: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00004d90: 0000 0001 0000 0040 0000 0073 1000 0000  .......@...s....
+00004da0: 6500 5a01 6400 5a02 6401 5a03 6402 5300  e.Z.d.Z.d.Z.d.S.
+00004db0: 2903 da12 436f 6e74 7261 6374 7341 5049  )...ContractsAPI
+00004dc0: 436c 6965 6e74 5a09 436f 6e74 7261 6374  ClientZ.Contract
+00004dd0: 734e 72eb 0000 0072 0f00 0000 720f 0000  sNr....r....r...
+00004de0: 0072 0f00 0000 7210 0000 0072 f500 0000  .r....r....r....
+00004df0: db02 0000 7302 0000 0008 0172 f500 0000  ....s......r....
+00004e00: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00004e10: 0002 0000 0040 0000 0073 1800 0000 6500  .....@...s....e.
+00004e20: 5a01 6400 5a02 6401 5a03 6402 6403 8400  Z.d.Z.d.Z.d.d...
+00004e30: 5a04 6404 5300 2905 da21 4163 636f 756e  Z.d.S.)..!Accoun
+00004e40: 7450 6879 7369 6361 6c4c 6f63 6174 696f  tPhysicalLocatio
+00004e50: 6e73 4150 4943 6c69 656e 745a 1043 6f6d  nsAPIClientZ.Com
+00004e60: 7061 6e79 4c6f 6361 7469 6f6e 7363 0200  panyLocationsc..
+00004e70: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+00004e80: 0000 4f00 0000 731a 0000 007c 006a 007c  ..O...s....|.j.|
+00004e90: 0166 017c 029e 0264 0164 0269 017c 0397  .f.|...d.d.i.|..
+00004ea0: 028e 0153 0072 e900 0000 72d3 0000 0072  ...S.r....r....r
+00004eb0: d400 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+00004ec0: 0000 0072 1e00 0000 e302 0000 7302 0000  ...r........s...
+00004ed0: 0000 017a 2541 6363 6f75 6e74 5068 7973  ...z%AccountPhys
+00004ee0: 6963 616c 4c6f 6361 7469 6f6e 7341 5049  icalLocationsAPI
+00004ef0: 436c 6965 6e74 2e67 6574 4ea9 0572 0b00  Client.getN..r..
+00004f00: 0000 720c 0000 0072 0d00 0000 7278 0000  ..r....r....rx..
+00004f10: 0072 1e00 0000 720f 0000 0072 0f00 0000  .r....r....r....
+00004f20: 720f 0000 0072 1000 0000 72f6 0000 00df  r....r....r.....
+00004f30: 0200 0073 0400 0000 0801 0403 72f6 0000  ...s........r...
+00004f40: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00004f50: 0000 0200 0000 4000 0000 7320 0000 0065  ......@...s ...e
+00004f60: 005a 0164 005a 0264 015a 0364 025a 0465  .Z.d.Z.d.Z.d.Z.e
+00004f70: 035a 0564 0364 0484 005a 0664 0553 0029  .Z.d.d...Z.d.S.)
+00004f80: 06da 0e54 6173 6b73 4150 4943 6c69 656e  ...TasksAPIClien
+00004f90: 74da 0554 6173 6b73 da08 5072 6f6a 6563  t..Tasks..Projec
+00004fa0: 7473 6304 0000 0000 0000 0000 0000 0006  tsc.............
+00004fb0: 0000 0005 0000 0043 0000 0073 2600 0000  .......C...s&...
+00004fc0: 7c00 a000 7c02 6a01 a101 7d04 7c00 a002  |...|.j...}.|...
+00004fd0: 7c01 7c03 a102 7d05 7c00 a003 6401 7c04  |.|...}.|...d.|.
+00004fe0: 7c05 a103 5300 72d7 0000 0029 0472 e600  |...S.r....).r..
+00004ff0: 0000 7298 0000 0072 a200 0000 72b9 0000  ..r....r....r...
+00005000: 0072 e700 0000 720f 0000 0072 0f00 0000  .r....r....r....
+00005010: 7210 0000 0072 6900 0000 ed02 0000 7306  r....ri.......s.
+00005020: 0000 0000 030c 010c 017a 1554 6173 6b73  .........z.Tasks
+00005030: 4150 4943 6c69 656e 742e 7570 6461 7465  APIClient.update
+00005040: 4e29 0772 0b00 0000 720c 0000 0072 0d00  N).r....r....r..
+00005050: 0000 7278 0000 0072 e400 0000 72e5 0000  ..rx...r....r...
+00005060: 0072 6900 0000 720f 0000 0072 0f00 0000  .ri...r....r....
+00005070: 720f 0000 0072 1000 0000 72f8 0000 00e7  r....r....r.....
+00005080: 0200 0073 0800 0000 0801 0401 0401 0403  ...s............
+00005090: 72f8 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000050a0: 0000 0000 0000 0300 0000 0000 0000 7328  ..............s(
+000050b0: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+000050c0: 025a 0464 035a 0587 0066 0164 0464 0584  .Z.d.Z...f.d.d..
+000050d0: 085a 0687 0004 005a 0753 0029 06da 1454  .Z.....Z.S.)...T
+000050e0: 6963 6b65 744e 6f74 6573 4150 4943 6c69  icketNotesAPICli
+000050f0: 656e 74da 0b54 6963 6b65 744e 6f74 6573  ent..TicketNotes
+00005100: 72f1 0000 005a 054e 6f74 6573 6302 0000  r....Z.Notesc...
+00005110: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+00005120: 000b 0000 0073 1c00 0000 7c02 a000 6401  .....s....|...d.
+00005130: a101 7d03 7401 8300 6a02 7c01 7c03 6602  ..}.t...j.|.|.f.
+00005140: 7c02 8e01 5300 a902 4eda 0674 6963 6b65  |...S...N..ticke
+00005150: 74a9 03da 0370 6f70 da05 7375 7065 7272  t....pop..superr
+00005160: de00 0000 a904 724d 0000 0072 da00 0000  ......rM...r....
+00005170: 726c 0000 0072 e100 0000 a901 724a 0000  rl...r......rJ..
+00005180: 0072 0f00 0000 7210 0000 0072 de00 0000  .r....r....r....
+00005190: fa02 0000 7304 0000 0000 010a 017a 1b54  ....s........z.T
+000051a0: 6963 6b65 744e 6f74 6573 4150 4943 6c69  icketNotesAPICli
+000051b0: 656e 742e 6372 6561 7465 a908 720b 0000  ent.create..r...
+000051c0: 0072 0c00 0000 720d 0000 0072 7800 0000  .r....r....rx...
+000051d0: 72e4 0000 0072 e500 0000 72de 0000 00da  r....r....r.....
+000051e0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 720f  .__classcell__r.
+000051f0: 0000 0072 0f00 0000 7203 0100 0072 1000  ...r....r....r..
+00005200: 0000 72fb 0000 00f5 0200 0073 0800 0000  ..r........s....
+00005210: 0801 0401 0401 0402 72fb 0000 0063 0000  ........r....c..
+00005220: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+00005230: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
+00005240: 005a 0264 015a 0364 0264 0384 005a 0464  .Z.d.Z.d.d...Z.d
+00005250: 0453 0029 05da 1254 6173 6b4e 6f74 6573  .S.)...TaskNotes
+00005260: 4150 4943 6c69 656e 745a 0954 6173 6b4e  APIClientZ.TaskN
+00005270: 6f74 6573 6302 0000 0000 0000 0000 0000  otesc...........
+00005280: 0004 0000 0004 0000 004f 0000 0073 1a00  .........O...s..
+00005290: 0000 7c00 6a00 7c01 6601 7c02 9e02 6401  ..|.j.|.f.|...d.
+000052a0: 6402 6901 7c03 9702 8e01 5300 72e9 0000  d.i.|.....S.r...
+000052b0: 0072 d300 0000 72d4 0000 0072 0f00 0000  .r....r....r....
+000052c0: 720f 0000 0072 1000 0000 721e 0000 0003  r....r....r.....
+000052d0: 0300 0073 0200 0000 0001 7a16 5461 736b  ...s......z.Task
+000052e0: 4e6f 7465 7341 5049 436c 6965 6e74 2e67  NotesAPIClient.g
+000052f0: 6574 4e72 f700 0000 720f 0000 0072 0f00  etNr....r....r..
+00005300: 0000 720f 0000 0072 1000 0000 7206 0100  ..r....r....r...
+00005310: 00ff 0200 0073 0400 0000 0801 0403 7206  .....s........r.
+00005320: 0100 0063 0000 0000 0000 0000 0000 0000  ...c............
+00005330: 0000 0000 0200 0000 4000 0000 7318 0000  ........@...s...
+00005340: 0065 005a 0164 005a 0264 015a 0364 0264  .e.Z.d.Z.d.Z.d.d
+00005350: 0384 005a 0464 0453 0029 05da 1454 696d  ...Z.d.S.)...Tim
+00005360: 6545 6e74 7269 6573 4150 4943 6c69 656e  eEntriesAPIClien
+00005370: 74da 0b54 696d 6545 6e74 7269 6573 6302  t..TimeEntriesc.
+00005380: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00005390: 0000 004f 0000 0073 1a00 0000 7c00 6a00  ...O...s....|.j.
+000053a0: 7c01 6601 7c02 9e02 6401 6402 6901 7c03  |.f.|...d.d.i.|.
+000053b0: 9702 8e01 5300 72e9 0000 0072 d300 0000  ....S.r....r....
+000053c0: 72d4 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+000053d0: 1000 0000 721e 0000 000b 0300 0073 0200  ....r........s..
+000053e0: 0000 0001 7a18 5469 6d65 456e 7472 6965  ....z.TimeEntrie
+000053f0: 7341 5049 436c 6965 6e74 2e67 6574 4e72  sAPIClient.getNr
+00005400: f700 0000 720f 0000 0072 0f00 0000 720f  ....r....r....r.
+00005410: 0000 0072 1000 0000 7207 0100 0007 0300  ...r....r.......
+00005420: 0073 0400 0000 0801 0403 7207 0100 0063  .s........r....c
+00005430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005440: 0300 0000 0000 0000 7328 0000 0065 005a  ........s(...e.Z
+00005450: 0164 005a 0264 015a 0364 025a 0464 035a  .d.Z.d.Z.d.Z.d.Z
+00005460: 0587 0066 0164 0464 0584 085a 0687 0004  ...f.d.d...Z....
+00005470: 005a 0753 0029 06da 2154 6963 6b65 7453  .Z.S.)..!TicketS
+00005480: 6563 6f6e 6461 7279 5265 736f 7572 6365  econdaryResource
+00005490: 7341 5049 436c 6965 6e74 5a18 5469 636b  sAPIClientZ.Tick
+000054a0: 6574 5365 636f 6e64 6172 7952 6573 6f75  etSecondaryResou
+000054b0: 7263 6573 72f1 0000 00da 1253 6563 6f6e  rcesr......Secon
+000054c0: 6461 7279 5265 736f 7572 6365 7363 0200  daryResourcesc..
+000054d0: 0000 0000 0000 0000 0000 0400 0000 0300  ................
+000054e0: 0000 0b00 0000 731c 0000 007c 02a0 0064  ......s....|...d
+000054f0: 01a1 017d 0374 0183 006a 027c 017c 0366  ...}.t...j.|.|.f
+00005500: 027c 028e 0153 0072 fd00 0000 72ff 0000  .|...S.r....r...
+00005510: 0072 0201 0000 7203 0100 0072 0f00 0000  .r....r....r....
+00005520: 7210 0000 0072 de00 0000 1403 0000 7304  r....r........s.
+00005530: 0000 0000 010a 017a 2854 6963 6b65 7453  .......z(TicketS
+00005540: 6563 6f6e 6461 7279 5265 736f 7572 6365  econdaryResource
+00005550: 7341 5049 436c 6965 6e74 2e63 7265 6174  sAPIClient.creat
+00005560: 6572 0401 0000 720f 0000 0072 0f00 0000  er....r....r....
+00005570: 7203 0100 0072 1000 0000 7209 0100 000f  r....r....r.....
+00005580: 0300 0073 0800 0000 0801 0401 0401 0402  ...s............
+00005590: 7209 0100 0063 0000 0000 0000 0000 0000  r....c..........
+000055a0: 0000 0000 0000 0300 0000 0000 0000 7328  ..............s(
+000055b0: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+000055c0: 025a 0464 035a 0587 0066 0164 0464 0584  .Z.d.Z...f.d.d..
+000055d0: 085a 0687 0004 005a 0753 0029 06da 1f54  .Z.....Z.S.)...T
+000055e0: 6173 6b53 6563 6f6e 6461 7279 5265 736f  askSecondaryReso
+000055f0: 7572 6365 7341 5049 436c 6965 6e74 5a16  urcesAPIClientZ.
+00005600: 5461 736b 5365 636f 6e64 6172 7952 6573  TaskSecondaryRes
+00005610: 6f75 7263 6573 72f9 0000 0072 0a01 0000  ourcesr....r....
+00005620: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+00005630: 0003 0000 000b 0000 0073 1c00 0000 7c02  .........s....|.
+00005640: a000 6401 a101 7d03 7401 8300 6a02 7c01  ..d...}.t...j.|.
+00005650: 7c03 6602 7c02 8e01 5300 2902 4eda 0474  |.f.|...S.).N..t
+00005660: 6173 6b72 ff00 0000 7202 0100 0072 0301  askr....r....r..
+00005670: 0000 720f 0000 0072 1000 0000 72de 0000  ..r....r....r...
+00005680: 001e 0300 0073 0400 0000 0001 0a01 7a26  .....s........z&
+00005690: 5461 736b 5365 636f 6e64 6172 7952 6573  TaskSecondaryRes
+000056a0: 6f75 7263 6573 4150 4943 6c69 656e 742e  ourcesAPIClient.
+000056b0: 6372 6561 7465 7204 0100 0072 0f00 0000  creater....r....
+000056c0: 720f 0000 0072 0301 0000 7210 0000 0072  r....r....r....r
+000056d0: 0b01 0000 1903 0000 7308 0000 0008 0104  ........s.......
+000056e0: 0104 0104 0272 0b01 0000 6300 0000 0000  .....r....c.....
+000056f0: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
+00005700: 0000 0073 2000 0000 6500 5a01 6400 5a02  ...s ...e.Z.d.Z.
+00005710: 6401 5a03 6402 6403 8400 5a04 6404 6405  d.Z.d.d...Z.d.d.
+00005720: 8400 5a05 6406 5300 2907 da11 5072 6f6a  ..Z.d.S.)...Proj
+00005730: 6563 7473 4150 4943 6c69 656e 7472 fa00  ectsAPIClientr..
+00005740: 0000 6302 0000 0000 0000 0000 0000 0004  ..c.............
+00005750: 0000 0004 0000 004f 0000 0073 1a00 0000  .......O...s....
+00005760: 7c00 6a00 7c01 6601 7c02 9e02 6401 6402  |.j.|.f.|...d.d.
+00005770: 6901 7c03 9702 8e01 5300 72e9 0000 0072  i.|.....S.r....r
+00005780: d300 0000 72d4 0000 0072 0f00 0000 720f  ....r....r....r.
+00005790: 0000 0072 1000 0000 721e 0000 0027 0300  ...r....r....'..
+000057a0: 0073 0200 0000 0001 7a15 5072 6f6a 6563  .s......z.Projec
+000057b0: 7473 4150 4943 6c69 656e 742e 6765 7463  tsAPIClient.getc
+000057c0: 0300 0000 0000 0000 0000 0000 0400 0000  ................
+000057d0: 0500 0000 4300 0000 731e 0000 007c 00a0  ....C...s....|..
+000057e0: 007c 017c 02a1 027d 037c 00a0 0164 017c  .|.|...}.|...d.|
+000057f0: 00a0 02a1 007c 03a1 0353 0072 d700 0000  .....|...S.r....
+00005800: 72f2 0000 0072 d900 0000 720f 0000 0072  r....r....r....r
+00005810: 0f00 0000 7210 0000 0072 6900 0000 2a03  ....r....ri...*.
+00005820: 0000 7304 0000 0000 030c 017a 1850 726f  ..s........z.Pro
+00005830: 6a65 6374 7341 5049 436c 6965 6e74 2e75  jectsAPIClient.u
+00005840: 7064 6174 654e 2906 720b 0000 0072 0c00  pdateN).r....r..
+00005850: 0000 720d 0000 0072 7800 0000 721e 0000  ..r....rx...r...
+00005860: 0072 6900 0000 720f 0000 0072 0f00 0000  .ri...r....r....
+00005870: 720f 0000 0072 1000 0000 720d 0100 0023  r....r....r....#
+00005880: 0300 0073 0600 0000 0801 0403 0803 720d  ...s..........r.
+00005890: 0100 0063 0000 0000 0000 0000 0000 0000  ...c............
+000058a0: 0000 0000 0100 0000 4000 0000 7310 0000  ........@...s...
+000058b0: 0065 005a 0164 005a 0264 015a 0364 0253  .e.Z.d.Z.d.Z.d.S
+000058c0: 0029 03da 1954 6963 6b65 7443 6174 6567  .)...TicketCateg
+000058d0: 6f72 6965 7341 5049 436c 6965 6e74 da10  oriesAPIClient..
+000058e0: 5469 636b 6574 4361 7465 676f 7269 6573  TicketCategories
+000058f0: 4e72 eb00 0000 720f 0000 0072 0f00 0000  Nr....r....r....
+00005900: 720f 0000 0072 1000 0000 720e 0100 0031  r....r....r....1
+00005910: 0300 0073 0200 0000 0801 720e 0100 0063  ...s......r....c
+00005920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005930: 0200 0000 4000 0000 7318 0000 0065 005a  ....@...s....e.Z
+00005940: 0164 005a 0264 015a 0364 0264 0384 005a  .d.Z.d.Z.d.d...Z
+00005950: 0464 0453 0029 05da 1954 6173 6b50 7265  .d.S.)...TaskPre
+00005960: 6465 6365 7373 6f72 7341 5049 436c 6965  decessorsAPIClie
+00005970: 6e74 5a10 5461 736b 5072 6564 6563 6573  ntZ.TaskPredeces
+00005980: 736f 7273 6302 0000 0000 0000 0000 0000  sorsc...........
+00005990: 0004 0000 0004 0000 004f 0000 0073 1a00  .........O...s..
+000059a0: 0000 7c00 6a00 7c01 6601 7c02 9e02 6401  ..|.j.|.f.|...d.
+000059b0: 6402 6901 7c03 9702 8e01 5300 72e9 0000  d.i.|.....S.r...
+000059c0: 0072 d300 0000 72d4 0000 0072 0f00 0000  .r....r....r....
+000059d0: 720f 0000 0072 1000 0000 721e 0000 0039  r....r....r....9
+000059e0: 0300 0073 0200 0000 0001 7a1d 5461 736b  ...s......z.Task
+000059f0: 5072 6564 6563 6573 736f 7273 4150 4943  PredecessorsAPIC
+00005a00: 6c69 656e 742e 6765 744e 72f7 0000 0072  lient.getNr....r
+00005a10: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+00005a20: 0000 0072 1001 0000 3503 0000 7304 0000  ...r....5...s...
+00005a30: 0008 0104 0372 1001 0000 6300 0000 0000  .....r....c.....
+00005a40: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
+00005a50: 0000 0073 1800 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00005a60: 6401 5a03 6402 6403 8400 5a04 6404 5300  d.Z.d.d...Z.d.S.
+00005a70: 2905 da15 5365 7276 6963 6543 616c 6c73  )...ServiceCalls
+00005a80: 4150 4943 6c69 656e 74da 0c53 6572 7669  APIClient..Servi
+00005a90: 6365 4361 6c6c 7363 0200 0000 0000 0000  ceCallsc........
+00005aa0: 0000 0000 0400 0000 0400 0000 4f00 0000  ............O...
+00005ab0: 731a 0000 007c 006a 007c 0166 017c 029e  s....|.j.|.f.|..
+00005ac0: 0264 0164 0269 017c 0397 028e 0153 0072  .d.d.i.|.....S.r
+00005ad0: e900 0000 72d3 0000 0072 d400 0000 720f  ....r....r....r.
+00005ae0: 0000 0072 0f00 0000 7210 0000 0072 1e00  ...r....r....r..
+00005af0: 0000 4103 0000 7302 0000 0000 017a 1953  ..A...s......z.S
+00005b00: 6572 7669 6365 4361 6c6c 7341 5049 436c  erviceCallsAPICl
+00005b10: 6965 6e74 2e67 6574 4e72 f700 0000 720f  ient.getNr....r.
+00005b20: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+00005b30: 0000 7211 0100 003d 0300 0073 0400 0000  ..r....=...s....
+00005b40: 0801 0403 7211 0100 0063 0000 0000 0000  ....r....c......
+00005b50: 0000 0000 0000 0000 0000 0300 0000 0000  ................
+00005b60: 0000 7328 0000 0065 005a 0164 005a 0264  ..s(...e.Z.d.Z.d
+00005b70: 015a 0364 025a 0464 035a 0587 0066 0164  .Z.d.Z.d.Z...f.d
+00005b80: 0464 0584 085a 0687 0004 005a 0753 0029  .d...Z.....Z.S.)
+00005b90: 06da 1b53 6572 7669 6365 4361 6c6c 5469  ...ServiceCallTi
+00005ba0: 636b 6574 7341 5049 436c 6965 6e74 da12  cketsAPIClient..
+00005bb0: 5365 7276 6963 6543 616c 6c54 6963 6b65  ServiceCallTicke
+00005bc0: 7473 7212 0100 0072 f100 0000 6302 0000  tsr....r....c...
+00005bd0: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+00005be0: 000b 0000 0073 1c00 0000 7c02 a000 6401  .....s....|...d.
+00005bf0: a101 7d03 7401 8300 6a02 7c01 7c03 6602  ..}.t...j.|.|.f.
+00005c00: 7c02 8e01 5300 a902 4eda 0c73 6572 7669  |...S...N..servi
+00005c10: 6365 5f63 616c 6c72 ff00 0000 7202 0100  ce_callr....r...
+00005c20: 0072 0301 0000 720f 0000 0072 1000 0000  .r....r....r....
+00005c30: 72de 0000 004a 0300 0073 0400 0000 0001  r....J...s......
+00005c40: 0a01 7a22 5365 7276 6963 6543 616c 6c54  ..z"ServiceCallT
+00005c50: 6963 6b65 7473 4150 4943 6c69 656e 742e  icketsAPIClient.
+00005c60: 6372 6561 7465 7204 0100 0072 0f00 0000  creater....r....
+00005c70: 720f 0000 0072 0301 0000 7210 0000 0072  r....r....r....r
+00005c80: 1301 0000 4503 0000 7308 0000 0008 0104  ....E...s.......
+00005c90: 0104 0104 0272 1301 0000 6300 0000 0000  .....r....c.....
+00005ca0: 0000 0000 0000 0000 0000 0003 0000 0000  ................
+00005cb0: 0000 0073 2800 0000 6500 5a01 6400 5a02  ...s(...e.Z.d.Z.
+00005cc0: 6401 5a03 6402 5a04 6403 5a05 8700 6601  d.Z.d.Z.d.Z...f.
+00005cd0: 6404 6405 8408 5a06 8700 0400 5a07 5300  d.d...Z.....Z.S.
+00005ce0: 2906 da23 5365 7276 6963 6543 616c 6c54  )..#ServiceCallT
+00005cf0: 6963 6b65 7452 6573 6f75 7263 6573 4150  icketResourcesAP
+00005d00: 4943 6c69 656e 745a 1a53 6572 7669 6365  IClientZ.Service
+00005d10: 4361 6c6c 5469 636b 6574 5265 736f 7572  CallTicketResour
+00005d20: 6365 7372 1401 0000 da09 5265 736f 7572  cesr......Resour
+00005d30: 6365 7363 0200 0000 0000 0000 0000 0000  cesc............
+00005d40: 0400 0000 0300 0000 0b00 0000 731c 0000  ............s...
+00005d50: 007c 02a0 0064 01a1 017d 0374 0183 006a  .|...d...}.t...j
+00005d60: 027c 017c 0366 027c 028e 0153 0029 024e  .|.|.f.|...S.).N
+00005d70: da13 7365 7276 6963 655f 6361 6c6c 5f74  ..service_call_t
+00005d80: 6963 6b65 7472 ff00 0000 7202 0100 0072  icketr....r....r
+00005d90: 0301 0000 720f 0000 0072 1000 0000 72de  ....r....r....r.
+00005da0: 0000 0054 0300 0073 0400 0000 0001 0a01  ...T...s........
+00005db0: 7a2a 5365 7276 6963 6543 616c 6c54 6963  z*ServiceCallTic
+00005dc0: 6b65 7452 6573 6f75 7263 6573 4150 4943  ketResourcesAPIC
+00005dd0: 6c69 656e 742e 6372 6561 7465 7204 0100  lient.creater...
+00005de0: 0072 0f00 0000 720f 0000 0072 0301 0000  .r....r....r....
+00005df0: 7210 0000 0072 1701 0000 4f03 0000 7308  r....r....O...s.
+00005e00: 0000 0008 0104 0104 0104 0272 1701 0000  ...........r....
+00005e10: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00005e20: 0003 0000 0000 0000 0073 2800 0000 6500  .........s(...e.
+00005e30: 5a01 6400 5a02 6401 5a03 6402 5a04 6403  Z.d.Z.d.Z.d.Z.d.
+00005e40: 5a05 8700 6601 6404 6405 8408 5a06 8700  Z...f.d.d...Z...
+00005e50: 0400 5a07 5300 2906 da19 5365 7276 6963  ..Z.S.)...Servic
+00005e60: 6543 616c 6c54 6173 6b73 4150 4943 6c69  eCallTasksAPICli
+00005e70: 656e 74da 1053 6572 7669 6365 4361 6c6c  ent..ServiceCall
+00005e80: 5461 736b 7372 1201 0000 72f9 0000 0063  Tasksr....r....c
+00005e90: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+00005ea0: 0300 0000 0b00 0000 731c 0000 007c 02a0  ........s....|..
+00005eb0: 0064 01a1 017d 0374 0183 006a 027c 017c  .d...}.t...j.|.|
+00005ec0: 0366 027c 028e 0153 0072 1501 0000 72ff  .f.|...S.r....r.
+00005ed0: 0000 0072 0201 0000 7203 0100 0072 0f00  ...r....r....r..
+00005ee0: 0000 7210 0000 0072 de00 0000 5e03 0000  ..r....r....^...
+00005ef0: 7304 0000 0000 010a 017a 2053 6572 7669  s........z Servi
+00005f00: 6365 4361 6c6c 5461 736b 7341 5049 436c  ceCallTasksAPICl
+00005f10: 6965 6e74 2e63 7265 6174 6572 0401 0000  ient.creater....
+00005f20: 720f 0000 0072 0f00 0000 7203 0100 0072  r....r....r....r
+00005f30: 1000 0000 721a 0100 0059 0300 0073 0800  ....r....Y...s..
+00005f40: 0000 0801 0401 0401 0402 721a 0100 0063  ..........r....c
+00005f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005f60: 0300 0000 0000 0000 7328 0000 0065 005a  ........s(...e.Z
+00005f70: 0164 005a 0264 015a 0364 025a 0464 035a  .d.Z.d.Z.d.Z.d.Z
+00005f80: 0587 0066 0164 0464 0584 085a 0687 0004  ...f.d.d...Z....
+00005f90: 005a 0753 0029 06da 2153 6572 7669 6365  .Z.S.)..!Service
+00005fa0: 4361 6c6c 5461 736b 5265 736f 7572 6365  CallTaskResource
+00005fb0: 7341 5049 436c 6965 6e74 5a18 5365 7276  sAPIClientZ.Serv
+00005fc0: 6963 6543 616c 6c54 6173 6b52 6573 6f75  iceCallTaskResou
+00005fd0: 7263 6573 721b 0100 0072 1801 0000 6302  rcesr....r....c.
+00005fe0: 0000 0000 0000 0000 0000 0004 0000 0003  ................
+00005ff0: 0000 000b 0000 0073 1c00 0000 7c02 a000  .......s....|...
+00006000: 6401 a101 7d03 7401 8300 6a02 7c01 7c03  d...}.t...j.|.|.
+00006010: 6602 7c02 8e01 5300 2902 4eda 1173 6572  f.|...S.).N..ser
+00006020: 7669 6365 5f63 616c 6c5f 7461 736b 72ff  vice_call_taskr.
+00006030: 0000 0072 0201 0000 7203 0100 0072 0f00  ...r....r....r..
+00006040: 0000 7210 0000 0072 de00 0000 6803 0000  ..r....r....h...
+00006050: 7304 0000 0000 010a 017a 2853 6572 7669  s........z(Servi
+00006060: 6365 4361 6c6c 5461 736b 5265 736f 7572  ceCallTaskResour
+00006070: 6365 7341 5049 436c 6965 6e74 2e63 7265  cesAPIClient.cre
+00006080: 6174 6572 0401 0000 720f 0000 0072 0f00  ater....r....r..
+00006090: 0000 7203 0100 0072 1000 0000 721c 0100  ..r....r....r...
+000060a0: 0063 0300 0073 0800 0000 0801 0401 0401  .c...s..........
+000060b0: 0402 721c 0100 0063 0000 0000 0000 0000  ..r....c........
+000060c0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
+000060d0: 7310 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+000060e0: 0364 0253 0029 03da 1252 6573 6f75 7263  .d.S.)...Resourc
+000060f0: 6573 4150 4943 6c69 656e 7472 1801 0000  esAPIClientr....
+00006100: 4e72 eb00 0000 720f 0000 0072 0f00 0000  Nr....r....r....
+00006110: 720f 0000 0072 1000 0000 721e 0100 006d  r....r....r....m
+00006120: 0300 0073 0200 0000 0801 721e 0100 0063  ...s......r....c
+00006130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006140: 0100 0000 4000 0000 7310 0000 0065 005a  ....@...s....e.Z
+00006150: 0164 005a 0264 015a 0364 0253 0029 03da  .d.Z.d.Z.d.S.)..
+00006160: 1141 6363 6f75 6e74 7341 5049 436c 6965  .AccountsAPIClie
+00006170: 6e74 da09 436f 6d70 616e 6965 734e 72eb  nt..CompaniesNr.
+00006180: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
+00006190: 0000 7210 0000 0072 1f01 0000 7103 0000  ..r....r....q...
+000061a0: 7302 0000 0008 0172 1f01 0000 6300 0000  s......r....c...
+000061b0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+000061c0: 0040 0000 0073 1000 0000 6500 5a01 6400  .@...s....e.Z.d.
+000061d0: 5a02 6401 5a03 6402 5300 2903 da0f 5068  Z.d.Z.d.S.)...Ph
+000061e0: 6173 6573 4150 4943 6c69 656e 745a 0650  asesAPIClientZ.P
+000061f0: 6861 7365 734e 72eb 0000 0072 0f00 0000  hasesNr....r....
+00006200: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00006210: 2101 0000 7503 0000 7302 0000 0008 0172  !...u...s......r
+00006220: 2101 0000 6300 0000 0000 0000 0000 0000  !...c...........
+00006230: 0000 0000 0003 0000 0040 0000 0073 1600  .........@...s..
+00006240: 0000 6500 5a01 6400 5a02 6404 6402 6403  ..e.Z.d.Z.d.d.d.
+00006250: 8401 5a03 6401 5300 2905 da0c 5544 4641  ..Z.d.S.)...UDFA
+00006260: 5049 436c 6965 6e74 4e63 0200 0000 0000  PIClientNc......
+00006270: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+00006280: 0000 7310 0000 0064 01a0 007c 006a 017c  ..s....d...|.j.|
+00006290: 006a 02a1 0253 0029 024e 7a2a 7b30 7d7b  .j...S.).Nz*{0}{
+000062a0: 317d 2f65 6e74 6974 7949 6e66 6f72 6d61  1}/entityInforma
+000062b0: 7469 6f6e 2f75 7365 7244 6566 696e 6564  tion/userDefined
+000062c0: 4669 656c 6473 2903 723b 0000 0072 7f00  Fields).r;...r..
+000062d0: 0000 7278 0000 0072 8000 0000 720f 0000  ..rx...r....r...
+000062e0: 0072 0f00 0000 7210 0000 0072 8100 0000  .r....r....r....
+000062f0: 7b03 0000 7308 0000 0000 0104 0104 0104  {...s...........
+00006300: fe7a 1855 4446 4150 4943 6c69 656e 742e  .z.UDFAPIClient.
+00006310: 6765 745f 6170 695f 7572 6c29 014e 2904  get_api_url).N).
+00006320: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00006330: 8100 0000 720f 0000 0072 0f00 0000 720f  ....r....r....r.
+00006340: 0000 0072 1000 0000 7222 0100 0079 0300  ...r....r"...y..
+00006350: 0073 0200 0000 0802 7222 0100 0063 0000  .s......r"...c..
+00006360: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00006370: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
+00006380: 005a 0264 015a 0364 0253 0029 03da 1354  .Z.d.Z.d.S.)...T
+00006390: 6963 6b65 7473 5544 4641 5049 436c 6965  icketsUDFAPIClie
+000063a0: 6e74 72f1 0000 004e 72eb 0000 0072 0f00  ntr....Nr....r..
+000063b0: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+000063c0: 0072 2301 0000 8203 0000 7302 0000 0008  .r#.......s.....
+000063d0: 0172 2301 0000 6300 0000 0000 0000 0000  .r#...c.........
+000063e0: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
+000063f0: 1000 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+00006400: 6402 5300 2903 da11 5461 736b 7355 4446  d.S.)...TasksUDF
+00006410: 4150 4943 6c69 656e 7472 f900 0000 4e72  APIClientr....Nr
+00006420: eb00 0000 720f 0000 0072 0f00 0000 720f  ....r....r....r.
+00006430: 0000 0072 1000 0000 7224 0100 0086 0300  ...r....r$......
+00006440: 0073 0200 0000 0801 7224 0100 0063 0000  .s......r$...c..
+00006450: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00006460: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
+00006470: 005a 0264 015a 0364 0253 0029 03da 1450  .Z.d.Z.d.S.)...P
+00006480: 726f 6a65 6374 7355 4446 4150 4943 6c69  rojectsUDFAPICli
+00006490: 656e 7472 fa00 0000 4e72 eb00 0000 720f  entr....Nr....r.
+000064a0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+000064b0: 0000 7225 0100 008a 0300 0073 0200 0000  ..r%.......s....
+000064c0: 0801 7225 0100 0063 0000 0000 0000 0000  ..r%...c........
+000064d0: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+000064e0: 7324 0000 0065 005a 0164 005a 0287 0066  s$...e.Z.d.Z...f
+000064f0: 0164 0164 0284 085a 0364 0364 0484 005a  .d.d...Z.d.d...Z
+00006500: 0487 0004 005a 0553 0029 05da 1941 7574  .....Z.S.)...Aut
+00006510: 6f74 6173 6b50 6963 6b6c 6973 7441 5049  otaskPicklistAPI
+00006520: 436c 6965 6e74 6301 0000 0000 0000 0000  Clientc.........
+00006530: 0000 0002 0000 0003 0000 000b 0000 0073  ...............s
+00006540: 2000 0000 6401 a000 7c00 6a01 a101 7c00   ...d...|.j...|.
+00006550: 5f02 7403 8300 6a04 6600 7c01 8e01 0100  _.t...j.f.|.....
+00006560: 6400 5300 2902 4e7a 1b7b 7d2f 656e 7469  d.S.).Nz.{}/enti
+00006570: 7479 496e 666f 726d 6174 696f 6e2f 6669  tyInformation/fi
+00006580: 656c 6473 2905 723b 0000 00da 0a41 5049  elds).r;.....API
+00006590: 5f45 4e54 4954 5972 7800 0000 7201 0100  _ENTITYrx...r...
+000065a0: 0072 4f00 0000 2902 724d 0000 0072 6c00  .rO...).rM...rl.
+000065b0: 0000 7203 0100 0072 0f00 0000 7210 0000  ..r....r....r...
+000065c0: 0072 4f00 0000 9003 0000 7304 0000 0000  .rO.......s.....
+000065d0: 010e 017a 2241 7574 6f74 6173 6b50 6963  ...z"AutotaskPic
+000065e0: 6b6c 6973 7441 5049 436c 6965 6e74 2e5f  klistAPIClient._
+000065f0: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
+00006600: 0000 0000 0400 0000 0300 0000 4f00 0000  ............O...
+00006610: 731a 0000 007c 006a 007c 0170 0e7c 00a0  s....|.j.|.p.|..
+00006620: 01a1 0066 017c 029e 027c 038e 0153 0072  ...f.|...|...S.r
+00006630: 2900 0000 2902 72c5 0000 0072 8100 0000  )...).r....r....
+00006640: 72d4 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+00006650: 1000 0000 721e 0000 0094 0300 0073 0e00  ....r........s..
+00006660: 0000 0003 0401 0aff 0201 02ff 0201 02ff  ................
+00006670: 7a1d 4175 746f 7461 736b 5069 636b 6c69  z.AutotaskPickli
+00006680: 7374 4150 4943 6c69 656e 742e 6765 7429  stAPIClient.get)
+00006690: 0672 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+000066a0: 724f 0000 0072 1e00 0000 7205 0100 0072  rO...r....r....r
+000066b0: 0f00 0000 720f 0000 0072 0301 0000 7210  ....r....r....r.
+000066c0: 0000 0072 2601 0000 8e03 0000 7304 0000  ...r&.......s...
+000066d0: 0008 020c 0472 2601 0000 6300 0000 0000  .....r&...c.....
+000066e0: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+000066f0: 0000 0073 1000 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00006700: 6401 5a03 6402 5300 2903 da12 4e6f 7465  d.Z.d.S.)...Note
+00006710: 5479 7065 7341 5049 436c 6965 6e74 72fc  TypesAPIClientr.
+00006720: 0000 004e a904 720b 0000 0072 0c00 0000  ...N..r....r....
+00006730: 720d 0000 0072 2701 0000 720f 0000 0072  r....r'...r....r
+00006740: 0f00 0000 720f 0000 0072 1000 0000 7228  ....r....r....r(
+00006750: 0100 009b 0300 0073 0200 0000 0801 7228  .......s......r(
+00006760: 0100 0063 0000 0000 0000 0000 0000 0000  ...c............
+00006770: 0000 0000 0100 0000 4000 0000 7310 0000  ........@...s...
+00006780: 0065 005a 0164 005a 0264 015a 0364 0253  .e.Z.d.Z.d.Z.d.S
+00006790: 0029 03da 154c 6963 656e 7365 5479 7065  .)...LicenseType
+000067a0: 7341 5049 436c 6965 6e74 7218 0100 004e  sAPIClientr....N
+000067b0: 7229 0100 0072 0f00 0000 720f 0000 0072  r)...r....r....r
+000067c0: 0f00 0000 7210 0000 0072 2a01 0000 9f03  ....r....r*.....
+000067d0: 0000 7302 0000 0008 0172 2a01 0000 6300  ..s......r*...c.
+000067e0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+000067f0: 0000 0040 0000 0073 1000 0000 6500 5a01  ...@...s....e.Z.
+00006800: 6400 5a02 6401 5a03 6402 5300 2903 da11  d.Z.d.Z.d.S.)...
+00006810: 5573 6554 7970 6573 4150 4943 6c69 656e  UseTypesAPIClien
+00006820: 7472 f400 0000 4e72 2901 0000 720f 0000  tr....Nr)...r...
+00006830: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
+00006840: 722b 0100 00a3 0300 0073 0200 0000 0801  r+.......s......
+00006850: 722b 0100 0063 0000 0000 0000 0000 0000  r+...c..........
+00006860: 0000 0000 0000 0100 0000 4000 0000 7310  ..........@...s.
+00006870: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00006880: 0253 0029 03da 1842 696c 6c69 6e67 436f  .S.)...BillingCo
+00006890: 6465 5479 7065 4150 4943 6c69 656e 7472  deTypeAPIClientr
+000068a0: f400 0000 4e72 2901 0000 720f 0000 0072  ....Nr)...r....r
+000068b0: 0f00 0000 720f 0000 0072 1000 0000 722c  ....r....r....r,
+000068c0: 0100 00a7 0300 0073 0200 0000 0801 722c  .......s......r,
+000068d0: 0100 0063 0000 0000 0000 0000 0000 0000  ...c............
+000068e0: 0000 0000 0100 0000 4000 0000 7310 0000  ........@...s...
+000068f0: 0065 005a 0164 005a 0264 015a 0364 0253  .e.Z.d.Z.d.Z.d.S
+00006900: 0029 03da 1654 6173 6b54 7970 654c 696e  .)...TaskTypeLin
+00006910: 6b73 4150 4943 6c69 656e 7472 0801 0000  ksAPIClientr....
+00006920: 4e72 2901 0000 720f 0000 0072 0f00 0000  Nr)...r....r....
+00006930: 720f 0000 0072 1000 0000 722d 0100 00ab  r....r....r-....
+00006940: 0300 0073 0200 0000 0801 722d 0100 0063  ...s......r-...c
+00006950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006960: 0100 0000 4000 0000 7310 0000 0065 005a  ....@...s....e.Z
+00006970: 0164 005a 0264 015a 0364 0253 0029 03da  .d.Z.d.Z.d.S.)..
+00006980: 1541 6363 6f75 6e74 5479 7065 7341 5049  .AccountTypesAPI
+00006990: 436c 6965 6e74 7220 0100 004e 7229 0100  Clientr ...Nr)..
+000069a0: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
+000069b0: 7210 0000 0072 2e01 0000 af03 0000 7302  r....r........s.
+000069c0: 0000 0008 0172 2e01 0000 6300 0000 0000  .....r....c.....
+000069d0: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+000069e0: 0000 0073 1000 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+000069f0: 6401 5a03 6402 5300 2903 da1f 5469 636b  d.Z.d.S.)...Tick
+00006a00: 6574 4361 7465 676f 7279 5069 636b 6c69  etCategoryPickli
+00006a10: 7374 4150 4943 6c69 656e 7472 0f01 0000  stAPIClientr....
+00006a20: 4e72 2901 0000 720f 0000 0072 0f00 0000  Nr)...r....r....
+00006a30: 720f 0000 0072 1000 0000 722f 0100 00b3  r....r....r/....
+00006a40: 0300 0073 0200 0000 0801 722f 0100 0063  ...s......r/...c
+00006a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006a60: 0100 0000 4000 0000 7310 0000 0065 005a  ....@...s....e.Z
+00006a70: 0164 005a 0264 015a 0364 0253 0029 03da  .d.Z.d.Z.d.S.)..
+00006a80: 2253 6572 7669 6365 4361 6c6c 5374 6174  "ServiceCallStat
+00006a90: 7573 5069 636b 6c69 7374 4150 4943 6c69  usPicklistAPICli
+00006aa0: 656e 7472 1201 0000 4e72 2901 0000 720f  entr....Nr)...r.
+00006ab0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+00006ac0: 0000 7230 0100 00b7 0300 0073 0200 0000  ..r0.......s....
+00006ad0: 0801 7230 0100 0063 0000 0000 0000 0000  ..r0...c........
+00006ae0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
+00006af0: 7310 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+00006b00: 0364 0253 0029 03da 1754 6963 6b65 7450  .d.S.)...TicketP
+00006b10: 6963 6b6c 6973 7441 5049 436c 6965 6e74  icklistAPIClient
+00006b20: 72f1 0000 004e 7229 0100 0072 0f00 0000  r....Nr)...r....
+00006b30: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00006b40: 3101 0000 bb03 0000 7302 0000 0008 0172  1.......s......r
+00006b50: 3101 0000 6300 0000 0000 0000 0000 0000  1...c...........
+00006b60: 0000 0000 0001 0000 0040 0000 0073 1000  .........@...s..
+00006b70: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00006b80: 5300 2903 da15 5461 736b 5069 636b 6c69  S.)...TaskPickli
+00006b90: 7374 4150 4943 6c69 656e 7472 f900 0000  stAPIClientr....
+00006ba0: 4e72 2901 0000 720f 0000 0072 0f00 0000  Nr)...r....r....
+00006bb0: 720f 0000 0072 1000 0000 7232 0100 00bf  r....r....r2....
+00006bc0: 0300 0073 0200 0000 0801 7232 0100 0063  ...s......r2...c
+00006bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006be0: 0100 0000 4000 0000 7310 0000 0065 005a  ....@...s....e.Z
+00006bf0: 0164 005a 0264 015a 0364 0253 0029 03da  .d.Z.d.Z.d.S.)..
+00006c00: 1850 726f 6a65 6374 5069 636b 6c69 7374  .ProjectPicklist
+00006c10: 4150 4943 6c69 656e 7472 fa00 0000 4e72  APIClientr....Nr
+00006c20: 2901 0000 720f 0000 0072 0f00 0000 720f  )...r....r....r.
+00006c30: 0000 0072 1000 0000 7233 0100 00c3 0300  ...r....r3......
+00006c40: 0073 0200 0000 0801 7233 0100 0063 0000  .s......r3...c..
+00006c50: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+00006c60: 0000 4000 0000 7338 0000 0065 005a 0164  ..@...s8...e.Z.d
+00006c70: 005a 0264 015a 0364 025a 0464 035a 0564  .Z.d.Z.d.Z.d.Z.d
+00006c80: 0464 0584 005a 0664 0664 0784 005a 0764  .d...Z.d.d...Z.d
+00006c90: 0864 0984 005a 0864 0a64 0b84 005a 0964  .d...Z.d.d...Z.d
+00006ca0: 0c53 0029 0dda 1d54 6963 6b65 7443 6865  .S.)...TicketChe
+00006cb0: 636b 6c69 7374 4974 656d 7341 5049 436c  cklistItemsAPICl
+00006cc0: 6965 6e74 5a14 5469 636b 6574 4368 6563  ientZ.TicketChec
+00006cd0: 6b6c 6973 7449 7465 6d73 72f1 0000 005a  klistItemsr....Z
+00006ce0: 0e43 6865 636b 6c69 7374 4974 656d 7363  .ChecklistItemsc
+00006cf0: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+00006d00: 0300 0000 4f00 0000 7312 0000 007c 006a  ....O...s....|.j
+00006d10: 007c 0166 017c 029e 027c 038e 0153 0072  .|.f.|...|...S.r
+00006d20: 2900 0000 72d3 0000 0072 d400 0000 720f  )...r....r....r.
+00006d30: 0000 0072 0f00 0000 7210 0000 0072 1e00  ...r....r....r..
+00006d40: 0000 cc03 0000 7302 0000 0000 017a 2154  ......s......z!T
+00006d50: 6963 6b65 7443 6865 636b 6c69 7374 4974  icketChecklistIt
+00006d60: 656d 7341 5049 436c 6965 6e74 2e67 6574  emsAPIClient.get
+00006d70: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+00006d80: 0005 0000 004b 0000 0073 1800 0000 7c00  .....K...s....|.
+00006d90: a000 7c01 a101 7d03 7c00 a001 6401 7c03  ..|...}.|...d.|.
+00006da0: 7c02 a103 5300 72d7 0000 00a9 0272 e600  |...S.r......r..
+00006db0: 0000 72b9 0000 00a9 0472 4d00 0000 72e1  ..r......rM...r.
+00006dc0: 0000 0072 6c00 0000 7242 0000 0072 0f00  ...rl...rB...r..
+00006dd0: 0000 720f 0000 0072 1000 0000 7269 0000  ..r....r....ri..
+00006de0: 00cf 0300 0073 0400 0000 0001 0a01 7a24  .....s........z$
+00006df0: 5469 636b 6574 4368 6563 6b6c 6973 7449  TicketChecklistI
+00006e00: 7465 6d73 4150 4943 6c69 656e 742e 7570  temsAPIClient.up
+00006e10: 6461 7465 6302 0000 0000 0000 0000 0000  datec...........
+00006e20: 0004 0000 0005 0000 004b 0000 0073 1800  .........K...s..
+00006e30: 0000 7c00 a000 7c01 a101 7d03 7c00 a001  ..|...|...}.|...
+00006e40: 6401 7c03 7c02 a103 5300 2902 4e72 5a00  d.|.|...S.).NrZ.
+00006e50: 0000 7235 0100 0072 3601 0000 720f 0000  ..r5...r6...r...
+00006e60: 0072 0f00 0000 7210 0000 0072 de00 0000  .r....r....r....
+00006e70: d303 0000 7304 0000 0000 010a 017a 2454  ....s........z$T
+00006e80: 6963 6b65 7443 6865 636b 6c69 7374 4974  icketChecklistIt
+00006e90: 656d 7341 5049 436c 6965 6e74 2e63 7265  emsAPIClient.cre
+00006ea0: 6174 6563 0200 0000 0000 0000 0000 0000  atec............
+00006eb0: 0400 0000 0600 0000 4b00 0000 7324 0000  ........K...s$..
+00006ec0: 0064 01a0 007c 00a0 017c 01a1 017c 02a0  .d...|...|...|..
+00006ed0: 0264 02a1 01a1 027d 037c 00a0 0364 037c  .d.....}.|...d.|
+00006ee0: 03a1 0253 0029 044e 72e8 0000 0072 9800  ...S.).Nr....r..
+00006ef0: 0000 72df 0000 0029 0472 3b00 0000 72e6  ..r....).r;...r.
+00006f00: 0000 0072 1e00 0000 72b9 0000 0072 3601  ...r....r....r6.
+00006f10: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00006f20: 0072 df00 0000 d703 0000 730a 0000 0000  .r........s.....
+00006f30: 0104 0108 0108 fe04 047a 2454 6963 6b65  .........z$Ticke
+00006f40: 7443 6865 636b 6c69 7374 4974 656d 7341  tChecklistItemsA
+00006f50: 5049 436c 6965 6e74 2e64 656c 6574 654e  PIClient.deleteN
+00006f60: 290a 720b 0000 0072 0c00 0000 720d 0000  ).r....r....r...
+00006f70: 0072 7800 0000 72e4 0000 0072 e500 0000  .rx...r....r....
+00006f80: 721e 0000 0072 6900 0000 72de 0000 0072  r....ri...r....r
+00006f90: df00 0000 720f 0000 0072 0f00 0000 720f  ....r....r....r.
+00006fa0: 0000 0072 1000 0000 7234 0100 00c7 0300  ...r....r4......
+00006fb0: 0073 0e00 0000 0801 0401 0401 0402 0803  .s..............
+00006fc0: 0804 0804 7234 0100 0063 0000 0000 0000  ....r4...c......
+00006fd0: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00006fe0: 0000 7328 0000 0065 005a 0164 005a 0264  ..s(...e.Z.d.Z.d
+00006ff0: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
+00007000: 005a 0564 0664 0784 005a 0664 0853 0029  .Z.d.d...Z.d.S.)
+00007010: 09da 1741 7474 6163 686d 656e 7449 6e66  ...AttachmentInf
+00007020: 6f41 5049 436c 6965 6e74 5a0e 4174 7461  oAPIClientZ.Atta
+00007030: 6368 6d65 6e74 496e 666f 6304 0000 0000  chmentInfoc.....
+00007040: 0000 0000 0000 0008 0000 000a 0000 0043  ...............C
+00007050: 0000 0073 e600 0000 7c03 9b00 6401 7c01  ...s....|...d.|.
+00007060: 9b00 6402 7c02 9b00 9d05 7d04 7c00 6a00  ..d.|.....}.|.j.
+00007070: 9b00 6401 7c04 9b00 9d03 7d05 7a2c 7401  ..d.|.....}.z,t.
+00007080: a002 6403 a003 7c05 a101 a101 0100 7404  ..d...|.......t.
+00007090: 6a05 7c05 7c00 6a06 7c00 a007 6404 a101  j.|.|.j.|...d...
+000070a0: 6405 8d03 7d06 5700 6e44 0400 7404 6a08  d...}.W.nD..t.j.
+000070b0: 6b0a 7294 0100 7d07 0100 7a24 7401 a009  k.r...}...z$t...
+000070c0: 6406 a003 7c05 7c07 a102 a101 0100 740a  d...|.|.......t.
+000070d0: 6407 a003 7c07 a101 8301 8201 5700 3500  d...|.......W.5.
+000070e0: 6400 7d07 7e07 5800 5900 6e02 5800 6408  d.}.~.X.Y.n.X.d.
+000070f0: 7c06 6a0b 0400 0300 6b01 72ac 6409 6b00  |.j.....k.r.d.k.
+00007100: 72d4 6e04 0100 6e24 7c06 a00c a100 a005  r.n...n$|.......
+00007110: 640a a101 72d0 7c06 a00c a100 a005 640a  d...r.|.......d.
+00007120: a101 640b 1900 7d06 7c06 5300 7c00 a00d  ..d...}.|.S.|...
+00007130: 7c06 a101 0100 6400 5300 6400 5300 290c  |.....d.S.d.S.).
+00007140: 4efa 012f 7a0d 2f41 7474 6163 686d 656e  N../z./Attachmen
+00007150: 7473 2f72 3300 0000 7294 0000 0029 0272  ts/r3...r....).r
+00007160: 2200 0000 7299 0000 0072 3700 0000 72b3  "...r....r7...r.
+00007170: 0000 0072 3500 0000 72b4 0000 0072 5600  ...r5...r....rV.
+00007180: 0000 7201 0000 0029 0e72 7f00 0000 7239  ..r....).r....r9
+00007190: 0000 0072 3a00 0000 723b 0000 0072 3c00  ...r:...r;...r<.
+000071a0: 0000 721e 0000 0072 2200 0000 729a 0000  ..r....r"...r...
+000071b0: 0072 4100 0000 7282 0000 0072 0900 0000  .rA...r....r....
+000071c0: 723d 0000 0072 3e00 0000 7283 0000 0029  r=...r>...r....)
+000071d0: 0872 4d00 0000 da09 6f62 6a65 6374 5f69  .rM.....object_i
+000071e0: 64da 0b64 6f63 756d 656e 745f 6964 da0b  d..document_id..
+000071f0: 7265 636f 7264 5f74 7970 655a 1b45 4e44  record_typeZ.END
+00007200: 504f 494e 545f 444f 4355 4d45 4e54 535f  POINT_DOCUMENTS_
+00007210: 444f 574e 4c4f 4144 726e 0000 0072 4300  DOWNLOADrn...rC.
+00007220: 0000 7218 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+00007230: 0072 1000 0000 da11 646f 6375 6d65 6e74  .r......document
+00007240: 5f64 6f77 6e6c 6f61 64e2 0300 0073 2400  _download....s$.
+00007250: 0000 0001 1403 1002 0201 1001 0401 0201  ................
+00007260: 0401 08fd 0a05 1201 1201 2002 1a01 0e01  .......... .....
+00007270: 1202 0402 0a01 7a29 4174 7461 6368 6d65  ......z)Attachme
+00007280: 6e74 496e 666f 4150 4943 6c69 656e 742e  ntInfoAPIClient.
+00007290: 646f 6375 6d65 6e74 5f64 6f77 6e6c 6f61  document_downloa
+000072a0: 6463 0400 0000 0000 0000 0000 0000 0400  dc..............
+000072b0: 0000 0500 0000 4300 0000 730e 0000 007c  ......C...s....|
+000072c0: 00a0 007c 017c 027c 03a1 0353 0072 2900  ...|.|.|...S.r).
+000072d0: 0000 2901 723c 0100 0029 0472 4d00 0000  ..).r<...).rM...
+000072e0: 7239 0100 0072 3a01 0000 723b 0100 0072  r9...r:...r;...r
+000072f0: 0f00 0000 720f 0000 0072 1000 0000 da0e  ....r....r......
+00007300: 6765 745f 6174 7461 6368 6d65 6e74 fc03  get_attachment..
+00007310: 0000 7302 0000 0000 017a 2641 7474 6163  ..s......z&Attac
+00007320: 686d 656e 7449 6e66 6f41 5049 436c 6965  hmentInfoAPIClie
+00007330: 6e74 2e67 6574 5f61 7474 6163 686d 656e  nt.get_attachmen
+00007340: 7463 0100 0000 0000 0000 0000 0000 0300  tc..............
+00007350: 0000 0300 0000 4f00 0000 7314 0000 0064  ......O...s....d
+00007360: 017c 0264 023c 007c 006a 007c 017c 028e  .|.d.<.|.j.|.|..
+00007370: 0153 0029 034e 5472 6800 0000 72d3 0000  .S.).NTrh...r...
+00007380: 0029 0372 4d00 0000 7217 0000 0072 6c00  .).rM...r....rl.
+00007390: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+000073a0: 0072 7000 0000 ff03 0000 7304 0000 0000  .rp.......s.....
+000073b0: 0108 027a 1d41 7474 6163 686d 656e 7449  ...z.AttachmentI
+000073c0: 6e66 6f41 5049 436c 6965 6e74 2e63 6f75  nfoAPIClient.cou
+000073d0: 6e74 4e29 0772 0b00 0000 720c 0000 0072  ntN).r....r....r
+000073e0: 0d00 0000 7278 0000 0072 3c01 0000 723d  ....rx...r<...r=
+000073f0: 0100 0072 7000 0000 720f 0000 0072 0f00  ...rp...r....r..
+00007400: 0000 720f 0000 0072 1000 0000 7237 0100  ..r....r....r7..
+00007410: 00df 0300 0073 0800 0000 0801 0402 081a  .....s..........
+00007420: 0803 7237 0100 0029 0146 2901 4629 0146  ..r7...).F).F).F
+00007430: 295b 72a6 0000 0072 ac00 0000 723e 0000  )[r....r....r>..
+00007440: 00da 076c 6f67 6769 6e67 7202 0000 0072  ...loggingr....r
+00007450: a800 0000 723c 0000 00da 0b64 6a61 6e67  ....r<.....djang
+00007460: 6f2e 636f 6e66 7203 0000 00da 1164 6a61  o.confr......dja
+00007470: 6e67 6f2e 636f 7265 2e63 6163 6865 7204  ngo.core.cacher.
+00007480: 0000 00da 0964 6a61 6e67 6f2e 6462 7205  .....django.dbr.
+00007490: 0000 005a 1064 6a61 7574 6f74 6173 6b2e  ...Z.djautotask.
+000074a0: 7574 696c 7372 0600 0000 da08 7265 7472  utilsr......retr
+000074b0: 7969 6e67 7207 0000 0072 c200 0000 72c3  yingr....r....r.
+000074c0: 0000 0072 2500 0000 7224 0000 0072 2600  ...r%...r$...r&.
+000074d0: 0000 72cb 0000 0072 cc00 0000 da09 6765  ..r....r......ge
+000074e0: 744c 6f67 6765 7272 0b00 0000 7239 0000  tLoggerr....r9..
+000074f0: 00da 0945 7863 6570 7469 6f6e 7209 0000  ...Exceptionr...
+00007500: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00007510: 7214 0000 0072 1500 0000 7219 0000 0072  r....r....r....r
+00007520: 1c00 0000 7220 0000 0072 2800 0000 722d  ....r ...r(...r-
+00007530: 0000 0072 2e00 0000 722a 0000 0072 3000  ...r....r*...r0.
+00007540: 0000 7244 0000 0072 5800 0000 da06 6f62  ..rD...rX.....ob
+00007550: 6a65 6374 7273 0000 0072 e300 0000 72ea  jectrs...r....r.
+00007560: 0000 0072 ec00 0000 72ed 0000 0072 ee00  ...r....r....r..
+00007570: 0000 72ef 0000 0072 f000 0000 72f3 0000  ..r....r....r...
+00007580: 0072 f500 0000 72f6 0000 0072 f800 0000  .r....r....r....
+00007590: 72fb 0000 0072 0601 0000 7207 0100 0072  r....r....r....r
+000075a0: 0901 0000 720b 0100 0072 0d01 0000 720e  ....r....r....r.
+000075b0: 0100 0072 1001 0000 7211 0100 0072 1301  ...r....r....r..
+000075c0: 0000 7217 0100 0072 1a01 0000 721c 0100  ..r....r....r...
+000075d0: 0072 1e01 0000 721f 0100 0072 2101 0000  .r....r....r!...
+000075e0: 7222 0100 0072 2301 0000 7224 0100 0072  r"...r#...r$...r
+000075f0: 2501 0000 7226 0100 0072 2801 0000 722a  %...r&...r(...r*
+00007600: 0100 0072 2b01 0000 722c 0100 0072 2d01  ...r+...r,...r-.
+00007610: 0000 722e 0100 0072 2f01 0000 7230 0100  ..r....r/...r0..
+00007620: 0072 3101 0000 7232 0100 0072 3301 0000  .r1...r2...r3...
+00007630: 7234 0100 0072 3701 0000 720f 0000 0072  r4...r7...r....r
+00007640: 0f00 0000 720f 0000 0072 1000 0000 da08  ....r....r......
+00007650: 3c6d 6f64 756c 653e 0100 0000 73b0 0000  <module>....s...
+00007660: 0008 0108 0108 0108 010c 0208 0108 020c  ................
+00007670: 010c 010c 010c 010c 0204 0204 0104 0104  ................
+00007680: 0104 0202 ff02 0302 ff02 040a 0310 0510  ................
+00007690: 0810 0810 0510 050a 0102 ff04 0708 0408  ................
+000076a0: 0b08 0408 080a 040a 040a 1208 1c0e 310e  ..............1.
+000076b0: 4410 7f00 7f00 7f00 070e 2610 0410 0410  D.........&.....
+000076c0: 0410 0410 0410 0e10 0410 0410 0812 0e12  ................
+000076d0: 0a10 0810 0812 0a12 0a10 0e10 0410 0810  ................
+000076e0: 0812 0a12 0a12 0a12 0a10 0410 0410 0410  ................
+000076f0: 0910 0410 0410 0410 0d10 0410 0410 0410  ................
+00007700: 0410 0410 0410 0410 0410 0410 0410 0412  ................
+00007710: 18                                       .
```

### Comparing `django-autotask-1.0.1/djautotask/__pycache__/models.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/__pycache__/models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 44367 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 4fad 0000  U.........KdO...
+00000000: 550d 0d0a 0000 0000 3268 4c64 4fad 0000  U.......2hLdO...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 f206 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6407 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `django-autotask-1.0.1/djautotask/__pycache__/utils.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/__pycache__/utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 497 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 f101 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 f101 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 8302 5a02 6404 5300 2905 e900  ..d...Z.d.S.)...
 00000050: 0000 0029 01da 0873 6574 7469 6e67 7363  ...)...settingsc
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0200 0000 4000 0000 7314 0000 0065 005a  ....@...s....e.Z
```

### Comparing `django-autotask-1.0.1/djautotask/__pycache__/views.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/__pycache__/views.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 2213 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 a508 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 a508 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6400 6406 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
```

### Comparing `django-autotask-1.0.1/djautotask/admin.py` & `django-autotask-1.1.1/djautotask/admin.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/api.py` & `django-autotask-1.1.1/djautotask/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,27 +221,44 @@
 
     def __delitem__(self, i):
         del self._list[i]
 
     def __iter__(self):
         return self._list.__iter__()
 
-    def build_query(self, method="get"):
+    def build_query(self, method="get", **kwargs):
         queries = []
         for condition in self._list:
             queries.append(condition.format_condition())
 
+        condition_filters = {
+            'filter': queries,
+        }
+
+        max_records = kwargs.get('page_size')
+        if max_records:
+            condition_filters.update({
+                'MaxRecords': max_records
+            })
+
         endpoint = self.METHODS[method]
-        filters = json.dumps({'filter': queries})
+        filters = json.dumps(condition_filters)
 
         if method == "get":
-            endpoint += filters
+
+            count = kwargs.get('record_count')
+            if count:
+                endpoint = f'query/count?search={filters}'
+            else:
+                endpoint += filters
+
             filters = None
         elif method != "post":
             raise TypeError("Unsupported method")
+
         return endpoint, filters
 
     def add(self, condition):
         if type(condition) is not ApiCondition:
             raise TypeError("Conditions must be instances of ApiCondition.")
 
         self._list.append(condition)
@@ -495,15 +512,15 @@
                     self._prepare_error_response(response))
 
         if next_url:
             url = next_url
         else:
             # Query endpoint is different between GET and POST
             query_endpoint, self.cached_body = \
-                self.conditions.build_query(method=method)
+                self.conditions.build_query(method=method, **kwargs)
             url = "{}{}".format(self.get_api_url(), query_endpoint)
 
         return _fetch_resource(
             url, request_retry_counter=retry_counter,
             request_method=method, request_body=self.cached_body, **kwargs)
 
     def log_message(self, endpoint, method, body):
@@ -965,7 +982,45 @@
 
     def delete(self, parent, **kwargs):
         endpoint_url = '{}/{}'.format(
             self.get_child_url(parent),
             kwargs.get("id")
         )
         return self.request('delete', endpoint_url)
+
+
+class AttachmentInfoAPIClient(AutotaskAPIClient):
+    API = 'AttachmentInfo'
+
+    def document_download(self, object_id, document_id, record_type):
+        ENDPOINT_DOCUMENTS_DOWNLOAD = f'{record_type}/{object_id}' \
+                                      f'/Attachments/{document_id}'
+
+        endpoint = f'{self.api_base_url}/{ENDPOINT_DOCUMENTS_DOWNLOAD}'
+
+        try:
+            logger.debug('Making GET request to {}'.format(endpoint))
+            response = requests.get(
+                endpoint,
+                timeout=self.timeout,
+                headers=self.get_headers('GET'),
+            )
+        except requests.RequestException as e:
+            logger.error('Request failed: GET {}: {}'.format(endpoint, e))
+            raise AutotaskAPIError('{}'.format(e))
+
+        if 200 <= response.status_code < 300:
+            if response.json().get('items'):
+                response = response.json().get('items')[0]
+
+            return response
+        else:
+            self._log_failed(response)
+            return None
+
+    def get_attachment(self, object_id, document_id, record_type):
+        return self.document_download(object_id, document_id, record_type)
+
+    def count(self, *args, **kwargs):
+        kwargs['record_count'] = True
+
+        return self.fetch_resource(*args, **kwargs)
```

### Comparing `django-autotask-1.0.1/djautotask/management/commands/__pycache__/atsync.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/management/commands/__pycache__/atsync.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 8434 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 f220 0000  U.........Kd. ..
+00000000: 550d 0d0a 0000 0000 3268 4c64 f220 0000  U.......2hLd. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6400 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d0a 5a0a 0100 6406  ..d.d.l.m.Z...d.
 00000070: 5a0b 6407 5a0c 4700 6408 6409 8400 6409  Z.d.Z.G.d.d...d.
```

### Comparing `django-autotask-1.0.1/djautotask/management/commands/atsync.py` & `django-autotask-1.1.1/djautotask/management/commands/atsync.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/management/commands/clearoldsyncjobs.py` & `django-autotask-1.1.1/djautotask/management/commands/clearoldsyncjobs.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0001_initial.py` & `django-autotask-1.1.1/djautotask/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0003_auto_20190913_0941.py` & `django-autotask-1.1.1/djautotask/migrations/0003_auto_20190913_0941.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0004_auto_20190913_1425.py` & `django-autotask-1.1.1/djautotask/migrations/0004_auto_20190913_1425.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0005_auto_20190916_1549.py` & `django-autotask-1.1.1/djautotask/migrations/0005_auto_20190916_1549.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0006_auto_20190916_1645.py` & `django-autotask-1.1.1/djautotask/migrations/0006_auto_20190916_1645.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0007_auto_20190917_1009.py` & `django-autotask-1.1.1/djautotask/migrations/0007_auto_20190917_1009.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0008_auto_20190917_1454.py` & `django-autotask-1.1.1/djautotask/migrations/0008_auto_20190917_1454.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0009_auto_20190918_1525.py` & `django-autotask-1.1.1/djautotask/migrations/0009_auto_20190918_1525.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0010_auto_20190923_0930.py` & `django-autotask-1.1.1/djautotask/migrations/0010_auto_20190923_0930.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0014_auto_20190930_1548.py` & `django-autotask-1.1.1/djautotask/migrations/0014_auto_20190930_1548.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0015_auto_20191001_0847.py` & `django-autotask-1.1.1/djautotask/migrations/0015_auto_20191001_0847.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0016_auto_20191021_0958.py` & `django-autotask-1.1.1/djautotask/migrations/0016_auto_20191021_0958.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0017_auto_20191021_1028.py` & `django-autotask-1.1.1/djautotask/migrations/0017_auto_20191021_1028.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0018_auto_20191029_1621.py` & `django-autotask-1.1.1/djautotask/migrations/0018_auto_20191029_1621.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0018_auto_20191029_1634.py` & `django-autotask-1.1.1/djautotask/migrations/0018_auto_20191029_1634.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0024_auto_20191122_1516.py` & `django-autotask-1.1.1/djautotask/migrations/0024_auto_20191122_1516.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0028_phase.py` & `django-autotask-1.1.1/djautotask/migrations/0028_phase.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0031_auto_20191129_1454.py` & `django-autotask-1.1.1/djautotask/migrations/0031_auto_20191129_1454.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0032_auto_20191129_1501.py` & `django-autotask-1.1.1/djautotask/migrations/0032_auto_20191129_1501.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0035_timeentry.py` & `django-autotask-1.1.1/djautotask/migrations/0035_timeentry.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0036_auto_20200127_1157.py` & `django-autotask-1.1.1/djautotask/migrations/0036_auto_20200127_1157.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0037_subissuetype_parent_value.py` & `django-autotask-1.1.1/djautotask/migrations/0037_subissuetype_parent_value.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0038_notetype_tasknote_ticketnote.py` & `django-autotask-1.1.1/djautotask/migrations/0038_notetype_tasknote_ticketnote.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0039_auto_20200131_1134.py` & `django-autotask-1.1.1/djautotask/migrations/0039_auto_20200131_1134.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0040_auto_20200204_1538.py` & `django-autotask-1.1.1/djautotask/migrations/0040_auto_20200204_1538.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0042_auto_20200205_1057.py` & `django-autotask-1.1.1/djautotask/migrations/0042_auto_20200205_1057.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0042_auto_20200205_1455.py` & `django-autotask-1.1.1/djautotask/migrations/0042_auto_20200205_1455.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0043_department.py` & `django-autotask-1.1.1/djautotask/migrations/0043_department.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0043_timeentry_allocation_code.py` & `django-autotask-1.1.1/djautotask/migrations/0043_timeentry_allocation_code.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0045_resourceroledepartment_resourceservicedeskrole.py` & `django-autotask-1.1.1/djautotask/migrations/0045_resourceroledepartment_resourceservicedeskrole.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0046_auto_20200207_1002.py` & `django-autotask-1.1.1/djautotask/migrations/0046_auto_20200207_1002.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0046_ticket_assigned_resource_role.py` & `django-autotask-1.1.1/djautotask/migrations/0046_ticket_assigned_resource_role.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0047_auto_20200207_1126.py` & `django-autotask-1.1.1/djautotask/migrations/0047_auto_20200207_1126.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0047_task_assigned_resource_role.py` & `django-autotask-1.1.1/djautotask/migrations/0047_task_assigned_resource_role.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0048_auto_20200211_1037.py` & `django-autotask-1.1.1/djautotask/migrations/0048_auto_20200211_1037.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0051_auto_20200315_1819.py` & `django-autotask-1.1.1/djautotask/migrations/0051_auto_20200315_1819.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0051_contract.py` & `django-autotask-1.1.1/djautotask/migrations/0051_contract.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0055_auto_20200325_0928.py` & `django-autotask-1.1.1/djautotask/migrations/0055_auto_20200325_0928.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0055_auto_20200325_1335.py` & `django-autotask-1.1.1/djautotask/migrations/0055_auto_20200325_1335.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0057_auto_20200406_1620.py` & `django-autotask-1.1.1/djautotask/migrations/0057_auto_20200406_1620.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0058_auto_20200408_1022.py` & `django-autotask-1.1.1/djautotask/migrations/0058_auto_20200408_1022.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0059_auto_20200414_1242.py` & `django-autotask-1.1.1/djautotask/migrations/0059_auto_20200414_1242.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0060_auto_20200414_1522.py` & `django-autotask-1.1.1/djautotask/migrations/0060_auto_20200414_1522.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0063_accountphysicallocation.py` & `django-autotask-1.1.1/djautotask/migrations/0063_accountphysicallocation.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0064_auto_20200511_1124.py` & `django-autotask-1.1.1/djautotask/migrations/0064_auto_20200511_1124.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0064_servicecall_location.py` & `django-autotask-1.1.1/djautotask/migrations/0064_servicecall_location.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0065_auto_20200512_1224.py` & `django-autotask-1.1.1/djautotask/migrations/0065_auto_20200512_1224.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0067_auto_20200519_1100.py` & `django-autotask-1.1.1/djautotask/migrations/0067_auto_20200519_1100.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0069_auto_20200602_1419.py` & `django-autotask-1.1.1/djautotask/migrations/0069_auto_20200602_1419.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0072_account_parent_account.py` & `django-autotask-1.1.1/djautotask/migrations/0072_account_parent_account.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0075_taskpredecessor.py` & `django-autotask-1.1.1/djautotask/migrations/0075_taskpredecessor.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0076_auto_20200923_0953.py` & `django-autotask-1.1.1/djautotask/migrations/0076_auto_20200923_0953.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0076_auto_20200925_1326.py` & `django-autotask-1.1.1/djautotask/migrations/0076_auto_20200925_1326.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0077_auto_20200924_1512.py` & `django-autotask-1.1.1/djautotask/migrations/0077_auto_20200924_1512.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0080_accountphysicallocationtracker_accounttracker_accounttypetracker_allocationcodetracker_contracttrack.py` & `django-autotask-1.1.1/djautotask/migrations/0080_accountphysicallocationtracker_accounttracker_accounttypetracker_allocationcodetracker_contracttrack.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0081_project_department.py` & `django-autotask-1.1.1/djautotask/migrations/0081_project_department.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0082_auto_20201020_1617.py` & `django-autotask-1.1.1/djautotask/migrations/0082_auto_20201020_1617.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0083_ticketudftracker.py` & `django-autotask-1.1.1/djautotask/migrations/0083_ticketudftracker.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0084_projectudftracker_taskudftracker.py` & `django-autotask-1.1.1/djautotask/migrations/0084_projectudftracker_taskudftracker.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0085_auto_20201022_1822.py` & `django-autotask-1.1.1/djautotask/migrations/0085_auto_20201022_1822.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0086_auto_20201222_1402.py` & `django-autotask-1.1.1/djautotask/migrations/0086_auto_20201222_1402.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0087_auto_20210108_1214.py` & `django-autotask-1.1.1/djautotask/migrations/0087_auto_20210108_1214.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0087_auto_20210108_1307.py` & `django-autotask-1.1.1/djautotask/migrations/0087_auto_20210108_1307.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0089_auto_20210125_1649.py` & `django-autotask-1.1.1/djautotask/migrations/0089_auto_20210125_1649.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0092_auto_20210629_1124.py` & `django-autotask-1.1.1/djautotask/migrations/0092_auto_20210629_1124.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0094_auto_20210723_1018.py` & `django-autotask-1.1.1/djautotask/migrations/0094_auto_20210723_1018.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0094_auto_20210727_0940.py` & `django-autotask-1.1.1/djautotask/migrations/0094_auto_20210727_0940.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0097_auto_20210819_1402.py` & `django-autotask-1.1.1/djautotask/migrations/0097_auto_20210819_1402.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0099_auto_20211124_1808.py` & `django-autotask-1.1.1/djautotask/migrations/0099_auto_20211124_1808.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0100_auto_20211228_1443.py` & `django-autotask-1.1.1/djautotask/migrations/0100_auto_20211228_1443.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0104_rename_allocationcode_billingcode_and_more.py` & `django-autotask-1.1.1/djautotask/migrations/0104_rename_allocationcode_billingcode_and_more.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0105_tasknote_created_by_contact.py` & `django-autotask-1.1.1/djautotask/migrations/0105_tasknote_created_by_contact.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0106_ticketnote_created_by_contact.py` & `django-autotask-1.1.1/djautotask/migrations/0106_ticketnote_created_by_contact.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0108_billingcodetype_billingcodetypetracker.py` & `django-autotask-1.1.1/djautotask/migrations/0108_billingcodetype_billingcodetypetracker.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0109_billingcode_billing_code_type.py` & `django-autotask-1.1.1/djautotask/migrations/0109_billingcode_billing_code_type.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/0112_account_owner_resource.py` & `django-autotask-1.1.1/djautotask/migrations/0112_account_owner_resource.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0001_initial.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0001_initial.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 2211 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 a308 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 a308 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0002_ticket_ticket_number.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0002_ticket_ticket_number.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 407 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 9701 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 9701 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0003_auto_20190913_0941.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0003_auto_20190913_0941.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1715 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 b306 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 b306 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0004_auto_20190913_1425.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0004_auto_20190913_1425.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1430 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 9605 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 9605 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
@@ -18,68 +18,68 @@
 00000110: 6a0d 6410 640e 8d01 6602 6412 6506 6a0d  j.d.d...f.d.e.j.
 00000120: 6410 640e 8d01 6602 6413 6506 6a0e 6405  d.d...f.d.e.j.d.
 00000130: 6414 8d01 6602 6708 6415 6416 6901 6417  d...f.g.d.d.i.d.
 00000140: 8d03 6504 6a0f 6418 6419 6506 6a10 6404  ..e.j.d.d.e.j.d.
 00000150: 6404 6511 6a09 6a06 6a12 6a13 641a 641b  d.e.j.j.j.j.d.d.
 00000160: 8d04 641c 8d03 6702 5a14 641d 5300 291e  ..d...g.Z.d.S.).
 00000170: da09 4d69 6772 6174 696f 6e29 02da 0a64  ..Migration)...d
-00000180: 6a61 7574 6f74 6173 6bda 1730 3030 335f  jautotask..0003_
+00000180: 6a61 7574 6f74 6173 6b5a 1730 3030 335f  jautotaskZ.0003_
 00000190: 6175 746f 5f32 3031 3930 3931 335f 3039  auto_20190913_09
 000001a0: 3431 da08 5265 736f 7572 6365 da02 6964  41..Resource..id
 000001b0: 5446 da02 4944 2904 da0c 6175 746f 5f63  TF..ID)...auto_c
 000001c0: 7265 6174 6564 da0b 7072 696d 6172 795f  reated..primary_
 000001d0: 6b65 79da 0973 6572 6961 6c69 7a65 da0c  key..serialize..
 000001e0: 7665 7262 6f73 655f 6e61 6d65 da07 6372  verbose_name..cr
 000001f0: 6561 7465 6429 02da 0c61 7574 6f5f 6e6f  eated)...auto_no
-00000200: 775f 6164 6472 0d00 0000 da08 6d6f 6469  w_addr......modi
+00000200: 775f 6164 6472 0c00 0000 da08 6d6f 6469  w_addr......modi
 00000210: 6669 6564 2902 da08 6175 746f 5f6e 6f77  fied)...auto_now
-00000220: 720d 0000 00da 0975 7365 725f 6e61 6d65  r......user_name
+00000220: 720c 0000 00da 0975 7365 725f 6e61 6d65  r......user_name
 00000230: e920 0000 0029 01da 0a6d 6178 5f6c 656e  . ...)...max_len
 00000240: 6774 68da 0565 6d61 696c e932 0000 00da  gth..email.2....
 00000250: 0a66 6972 7374 5f6e 616d 65da 096c 6173  .first_name..las
 00000260: 745f 6e61 6d65 da06 6163 7469 7665 2901  t_name..active).
 00000270: da07 6465 6661 756c 74da 086f 7264 6572  ..default..order
-00000280: 696e 6729 0272 1700 0000 7218 0000 0029  ing).r....r....)
+00000280: 696e 6729 0272 1600 0000 7217 0000 0029  ing).r....r....)
 00000290: 03da 046e 616d 65da 0666 6965 6c64 73da  ...name..fields.
 000002a0: 076f 7074 696f 6e73 da06 7469 636b 6574  .options..ticket
 000002b0: da11 6173 7369 676e 6564 5f72 6573 6f75  ..assigned_resou
 000002c0: 7263 657a 1364 6a61 7574 6f74 6173 6b2e  rcez.djautotask.
 000002d0: 5265 736f 7572 6365 2904 da05 626c 616e  Resource)...blan
 000002e0: 6bda 046e 756c 6cda 096f 6e5f 6465 6c65  k..null..on_dele
 000002f0: 7465 da02 746f 2903 da0a 6d6f 6465 6c5f  te..to)...model_
-00000300: 6e61 6d65 721c 0000 00da 0566 6965 6c64  namer......field
+00000300: 6e61 6d65 721b 0000 00da 0566 6965 6c64  namer......field
 00000310: 4e29 15da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
 00000320: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 00000330: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
 00000340: 6e63 6965 7372 0200 0000 da0b 4372 6561  nciesr......Crea
 00000350: 7465 4d6f 6465 6c72 0300 0000 da09 4175  teModelr......Au
 00000360: 746f 4669 656c 64da 1164 6a61 6e67 6f5f  toField..django_
-00000370: 6578 7465 6e73 696f 6e73 da02 6462 721d  extensions..dbr.
+00000370: 6578 7465 6e73 696f 6e73 da02 6462 721c  extensions..dbr.
 00000380: 0000 00da 1543 7265 6174 696f 6e44 6174  .....CreationDat
 00000390: 6554 696d 6546 6965 6c64 da19 4d6f 6469  eTimeField..Modi
 000003a0: 6669 6361 7469 6f6e 4461 7465 5469 6d65  ficationDateTime
 000003b0: 4669 656c 64da 0943 6861 7246 6965 6c64  Field..CharField
 000003c0: da0c 426f 6f6c 6561 6e46 6965 6c64 da08  ..BooleanField..
 000003d0: 4164 6446 6965 6c64 da0a 466f 7265 6967  AddField..Foreig
 000003e0: 6e4b 6579 da06 646a 616e 676f da08 6465  nKey..django..de
 000003f0: 6c65 7469 6f6e da08 5345 545f 4e55 4c4c  letion..SET_NULL
-00000400: da0a 6f70 6572 6174 696f 6e73 a900 7239  ..operations..r9
-00000410: 0000 0072 3900 0000 fa62 2f68 6f6d 652f  ...r9....b/home/
+00000400: da0a 6f70 6572 6174 696f 6e73 a900 7238  ..operations..r8
+00000410: 0000 0072 3800 0000 fa62 2f68 6f6d 652f  ...r8....b/home/
 00000420: 7275 6e6e 6572 2f77 6f72 6b2f 646a 616e  runner/work/djan
 00000430: 676f 2d61 7574 6f74 6173 6b2f 646a 616e  go-autotask/djan
 00000440: 676f 2d61 7574 6f74 6173 6b2f 646a 6175  go-autotask/djau
 00000450: 746f 7461 736b 2f6d 6967 7261 7469 6f6e  totask/migration
 00000460: 732f 3030 3034 5f61 7574 6f5f 3230 3139  s/0004_auto_2019
 00000470: 3039 3133 5f31 3432 352e 7079 7204 0000  0913_1425.pyr...
 00000480: 0008 0000 0073 2e00 0000 0803 02ff 0405  .....s..........
 00000490: 0401 0202 1401 1401 1401 0e01 0e01 0e01  ................
 000004a0: 0e01 0ef8 020b 0200 02ff 02f4 0410 0401  ................
 000004b0: 0201 0201 18fd 04ef 7204 0000 0029 08da  ........r....)..
 000004c0: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
 000004d0: 0300 0000 da19 646a 616e 676f 2e64 622e  ......django.db.
 000004e0: 6d6f 6465 6c73 2e64 656c 6574 696f 6e72  models.deletionr
-000004f0: 3500 0000 da1b 646a 616e 676f 5f65 7874  5.....django_ext
+000004f0: 3400 0000 da1b 646a 616e 676f 5f65 7874  4.....django_ext
 00000500: 656e 7369 6f6e 732e 6462 2e66 6965 6c64  ensions.db.field
-00000510: 7372 2d00 0000 7204 0000 0072 3900 0000  sr-...r....r9...
-00000520: 7239 0000 0072 3900 0000 723a 0000 00da  r9...r9...r:....
+00000510: 7372 2c00 0000 7204 0000 0072 3800 0000  sr,...r....r8...
+00000520: 7238 0000 0072 3800 0000 7239 0000 00da  r8...r8...r9....
 00000530: 083c 6d6f 6475 6c65 3e03 0000 0073 0600  .<module>....s..
 00000540: 0000 1001 0801 0803                      ........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0005_auto_20190916_1549.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0005_auto_20190916_1549.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1517 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 ed05 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 ed05 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0005_remove_ticketstatus_value.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0005_remove_ticketstatus_value.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 337 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 5101 0000  U.........KdQ...
+00000000: 550d 0d0a 0000 0000 3268 4c64 5101 0000  U.......2hLdQ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0400 0000 4000 0000 7322  ..........@...s"
 00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
 00000090: 0365 046a 0564 0264 0364 048d 0267 015a  .e.j.d.d.d...g.Z
 000000a0: 0664 0553 0029 06da 094d 6967 7261 7469  .d.S.)...Migrati
 000000b0: 6f6e 2902 da0a 646a 6175 746f 7461 736b  on)...djautotask
-000000c0: 5a17 3030 3034 5f61 7574 6f5f 3230 3139  Z.0004_auto_2019
-000000d0: 3039 3133 5f31 3432 35da 0c74 6963 6b65  0913_1425..ticke
+000000c0: da17 3030 3034 5f61 7574 6f5f 3230 3139  ..0004_auto_2019
+000000d0: 3039 3133 5f31 3432 355a 0c74 6963 6b65  0913_1425Z.ticke
 000000e0: 7473 7461 7475 73da 0576 616c 7565 2902  tstatus..value).
 000000f0: da0a 6d6f 6465 6c5f 6e61 6d65 da04 6e61  ..model_name..na
 00000100: 6d65 4e29 07da 085f 5f6e 616d 655f 5fda  meN)...__name__.
 00000110: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
 00000120: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
 00000130: 6465 6e63 6965 7372 0200 0000 da0b 5265  denciesr......Re
 00000140: 6d6f 7665 4669 656c 64da 0a6f 7065 7261  moveField..opera
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0006_auto_20190916_1645.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0006_auto_20190916_1645.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1723 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 bb06 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 bb06 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
@@ -21,76 +21,76 @@
 00000140: 8d03 6602 6416 6506 6a0e 6405 6411 8d01  ..f.d.e.j.d.d...
 00000150: 6602 6417 6506 6a0e 6405 6411 8d01 6602  f.d.e.j.d.d...f.
 00000160: 670a 6418 6419 641a 9c02 641b 8d03 6504  g.d.d.d...d...e.
 00000170: 6a10 641c 641d 6506 6a11 6404 6404 6512  j.d.d.e.j.d.d.e.
 00000180: 6a09 6a06 6a13 6a14 641e 641f 8d04 6420  j.j.j.j.d.d...d 
 00000190: 8d03 6702 5a15 6421 5300 2922 da09 4d69  ..g.Z.d!S.)"..Mi
 000001a0: 6772 6174 696f 6e29 02da 0a64 6a61 7574  gration)...djaut
-000001b0: 6f74 6173 6b5a 1730 3030 355f 6175 746f  otaskZ.0005_auto
-000001c0: 5f32 3031 3930 3931 365f 3135 3439 5a0e  _20190916_1549Z.
+000001b0: 6f74 6173 6bda 1730 3030 355f 6175 746f  otask..0005_auto
+000001c0: 5f32 3031 3930 3931 365f 3135 3439 da0e  _20190916_1549..
 000001d0: 5469 636b 6574 5072 696f 7269 7479 da02  TicketPriority..
 000001e0: 6964 5446 da02 4944 2904 da0c 6175 746f  idTF..ID)...auto
 000001f0: 5f63 7265 6174 6564 da0b 7072 696d 6172  _created..primar
 00000200: 795f 6b65 79da 0973 6572 6961 6c69 7a65  y_key..serialize
 00000210: da0c 7665 7262 6f73 655f 6e61 6d65 da07  ..verbose_name..
 00000220: 6372 6561 7465 6429 02da 0c61 7574 6f5f  created)...auto_
-00000230: 6e6f 775f 6164 6472 0b00 0000 da08 6d6f  now_addr......mo
+00000230: 6e6f 775f 6164 6472 0d00 0000 da08 6d6f  now_addr......mo
 00000240: 6469 6669 6564 2902 da08 6175 746f 5f6e  dified)...auto_n
-00000250: 6f77 720b 0000 00da 0576 616c 7565 e932  owr......value.2
+00000250: 6f77 720d 0000 00da 0576 616c 7565 e932  owr......value.2
 00000260: 0000 0029 03da 0562 6c61 6e6b da0a 6d61  ...)...blank..ma
 00000270: 785f 6c65 6e67 7468 da04 6e75 6c6c da05  x_length..null..
 00000280: 6c61 6265 6cda 1069 735f 6465 6661 756c  label..is_defaul
 00000290: 745f 7661 6c75 6529 01da 0764 6566 6175  t_value)...defau
 000002a0: 6c74 da0a 736f 7274 5f6f 7264 6572 2902  lt..sort_order).
-000002b0: 7212 0000 0072 1400 0000 da0c 7061 7265  r....r......pare
+000002b0: 7214 0000 0072 1600 0000 da0c 7061 7265  r....r......pare
 000002c0: 6e74 5f76 616c 7565 e914 0000 00da 0969  nt_value.......i
 000002d0: 735f 6163 7469 7665 da09 6973 5f73 7973  s_active..is_sys
 000002e0: 7465 6d7a 0f54 6963 6b65 7420 7072 696f  temz.Ticket prio
 000002f0: 7269 7479 7a11 5469 636b 6574 2070 7269  rityz.Ticket pri
-00000300: 6f72 6974 6965 7329 0272 0b00 0000 da13  orities).r......
+00000300: 6f72 6974 6965 7329 0272 0d00 0000 da13  orities).r......
 00000310: 7665 7262 6f73 655f 6e61 6d65 5f70 6c75  verbose_name_plu
 00000320: 7261 6c29 03da 046e 616d 65da 0666 6965  ral)...name..fie
 00000330: 6c64 73da 076f 7074 696f 6e73 da06 7469  lds..options..ti
 00000340: 636b 6574 da08 7072 696f 7269 7479 7a19  cket..priorityz.
 00000350: 646a 6175 746f 7461 736b 2e54 6963 6b65  djautotask.Ticke
-00000360: 7450 7269 6f72 6974 7929 0472 1200 0000  tPriority).r....
-00000370: 7214 0000 00da 096f 6e5f 6465 6c65 7465  r......on_delete
+00000360: 7450 7269 6f72 6974 7929 0472 1400 0000  tPriority).r....
+00000370: 7216 0000 00da 096f 6e5f 6465 6c65 7465  r......on_delete
 00000380: da02 746f 2903 da0a 6d6f 6465 6c5f 6e61  ..to)...model_na
-00000390: 6d65 721e 0000 00da 0566 6965 6c64 4e29  mer......fieldN)
+00000390: 6d65 7220 0000 00da 0566 6965 6c64 4e29  mer .....fieldN)
 000003a0: 16da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
 000003b0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
 000003c0: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
 000003d0: 6965 7372 0200 0000 da0b 4372 6561 7465  iesr......Create
 000003e0: 4d6f 6465 6c72 0300 0000 da09 4175 746f  Modelr......Auto
 000003f0: 4669 656c 64da 1164 6a61 6e67 6f5f 6578  Field..django_ex
-00000400: 7465 6e73 696f 6e73 da02 6462 721f 0000  tensions..dbr...
+00000400: 7465 6e73 696f 6e73 da02 6462 7221 0000  tensions..dbr!..
 00000410: 00da 1543 7265 6174 696f 6e44 6174 6554  ...CreationDateT
 00000420: 696d 6546 6965 6c64 da19 4d6f 6469 6669  imeField..Modifi
 00000430: 6361 7469 6f6e 4461 7465 5469 6d65 4669  cationDateTimeFi
 00000440: 656c 64da 0943 6861 7246 6965 6c64 da0c  eld..CharField..
 00000450: 426f 6f6c 6561 6e46 6965 6c64 da19 506f  BooleanField..Po
 00000460: 7369 7469 7665 536d 616c 6c49 6e74 6567  sitiveSmallInteg
 00000470: 6572 4669 656c 64da 0841 6464 4669 656c  erField..AddFiel
 00000480: 64da 0a46 6f72 6569 676e 4b65 79da 0664  d..ForeignKey..d
 00000490: 6a61 6e67 6fda 0864 656c 6574 696f 6eda  jango..deletion.
 000004a0: 0853 4554 5f4e 554c 4cda 0a6f 7065 7261  .SET_NULL..opera
-000004b0: 7469 6f6e 73a9 0072 3a00 0000 723a 0000  tions..r:...r:..
+000004b0: 7469 6f6e 73a9 0072 3c00 0000 723c 0000  tions..r<...r<..
 000004c0: 00fa 622f 686f 6d65 2f72 756e 6e65 722f  ..b/home/runner/
 000004d0: 776f 726b 2f64 6a61 6e67 6f2d 6175 746f  work/django-auto
 000004e0: 7461 736b 2f64 6a61 6e67 6f2d 6175 746f  task/django-auto
 000004f0: 7461 736b 2f64 6a61 7574 6f74 6173 6b2f  task/djautotask/
 00000500: 6d69 6772 6174 696f 6e73 2f30 3030 365f  migrations/0006_
 00000510: 6175 746f 5f32 3031 3930 3931 365f 3136  auto_20190916_16
 00000520: 3435 2e70 7972 0400 0000 0800 0000 7332  45.pyr........s2
 00000530: 0000 0008 0302 ff04 0504 0102 0214 0114  ................
 00000540: 0114 0112 0112 010e 0110 0112 010e 010e  ................
 00000550: f602 0d02 0102 fe04 f204 1304 0102 0102  ................
 00000560: 0118 fd04 ec72 0400 0000 2908 da09 646a  .....r....)...dj
 00000570: 616e 676f 2e64 6272 0200 0000 7203 0000  ango.dbr....r...
 00000580: 00da 1964 6a61 6e67 6f2e 6462 2e6d 6f64  ...django.db.mod
-00000590: 656c 732e 6465 6c65 7469 6f6e 7236 0000  els.deletionr6..
+00000590: 656c 732e 6465 6c65 7469 6f6e 7238 0000  els.deletionr8..
 000005a0: 00da 1b64 6a61 6e67 6f5f 6578 7465 6e73  ...django_extens
-000005b0: 696f 6e73 2e64 622e 6669 656c 6473 722d  ions.db.fieldsr-
-000005c0: 0000 0072 0400 0000 723a 0000 0072 3a00  ...r....r:...r:.
-000005d0: 0000 723a 0000 0072 3b00 0000 da08 3c6d  ..r:...r;.....<m
+000005b0: 696f 6e73 2e64 622e 6669 656c 6473 722f  ions.db.fieldsr/
+000005c0: 0000 0072 0400 0000 723c 0000 0072 3c00  ...r....r<...r<.
+000005d0: 0000 723c 0000 0072 3d00 0000 da08 3c6d  ..r<...r=.....<m
 000005e0: 6f64 756c 653e 0300 0000 7306 0000 0010  odule>....s.....
 000005f0: 0108 0108 03                             .....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0006_merge_20190920_1450.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0006_merge_20190920_1450.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 287 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 1f01 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 1f01 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0200 0000 4000 0000 7318  ..........@...s.
 00000080: 0000 0065 005a 0164 005a 0264 0164 0267  ...e.Z.d.Z.d.d.g
 00000090: 025a 0367 005a 0464 0353 0029 04da 094d  .Z.g.Z.d.S.)...M
 000000a0: 6967 7261 7469 6f6e 2902 da0a 646a 6175  igration)...djau
-000000b0: 746f 7461 736b da17 3030 3035 5f61 7574  totask..0005_aut
+000000b0: 746f 7461 736b 5a17 3030 3035 5f61 7574  totaskZ.0005_aut
 000000c0: 6f5f 3230 3139 3039 3136 5f31 3534 3929  o_20190916_1549)
-000000d0: 0272 0400 0000 da1e 3030 3035 5f72 656d  .r......0005_rem
+000000d0: 0272 0400 0000 5a1e 3030 3035 5f72 656d  .r....Z.0005_rem
 000000e0: 6f76 655f 7469 636b 6574 7374 6174 7573  ove_ticketstatus
 000000f0: 5f76 616c 7565 4e29 05da 085f 5f6e 616d  _valueN)...__nam
 00000100: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
 00000110: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
 00000120: 6570 656e 6465 6e63 6965 73da 0a6f 7065  ependencies..ope
-00000130: 7261 7469 6f6e 73a9 0072 0c00 0000 720c  rations..r....r.
+00000130: 7261 7469 6f6e 73a9 0072 0a00 0000 720a  rations..r....r.
 00000140: 0000 00fa 632f 686f 6d65 2f72 756e 6e65  ....c/home/runne
 00000150: 722f 776f 726b 2f64 6a61 6e67 6f2d 6175  r/work/django-au
 00000160: 746f 7461 736b 2f64 6a61 6e67 6f2d 6175  totask/django-au
 00000170: 746f 7461 736b 2f64 6a61 7574 6f74 6173  totask/djautotas
 00000180: 6b2f 6d69 6772 6174 696f 6e73 2f30 3030  k/migrations/000
 00000190: 365f 6d65 7267 655f 3230 3139 3039 3230  6_merge_20190920
 000001a0: 5f31 3435 302e 7079 7203 0000 0006 0000  _1450.pyr.......
 000001b0: 0073 0800 0000 0803 0201 02fe 0405 7203  .s............r.
 000001c0: 0000 004e 2903 da09 646a 616e 676f 2e64  ...N)...django.d
-000001d0: 6272 0200 0000 7203 0000 0072 0c00 0000  br....r....r....
-000001e0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+000001d0: 6272 0200 0000 7203 0000 0072 0a00 0000  br....r....r....
+000001e0: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
 000001f0: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
 00000200: 0000 0c03                                ....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0007_auto_20190917_1009.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0007_auto_20190917_1009.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1640 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 6806 0000  U.........Kdh...
+00000000: 550d 0d0a 0000 0000 3268 4c64 6806 0000  U.......2hLdh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
@@ -21,72 +21,72 @@
 00000140: 8d03 6602 6416 6506 6a0e 6405 6411 8d01  ..f.d.e.j.d.d...
 00000150: 6602 6417 6506 6a0e 6405 6411 8d01 6602  f.d.e.j.d.d...f.
 00000160: 670a 6418 6419 6901 641a 8d03 6504 6a10  g.d.d.i.d...e.j.
 00000170: 641b 641c 6506 6a11 6404 6404 6512 6a09  d.d.e.j.d.d.e.j.
 00000180: 6a06 6a13 6a14 641d 641e 8d04 641f 8d03  j.j.j.d.d...d...
 00000190: 6702 5a15 6420 5300 2921 da09 4d69 6772  g.Z.d S.)!..Migr
 000001a0: 6174 696f 6e29 02da 0a64 6a61 7574 6f74  ation)...djautot
-000001b0: 6173 6bda 1730 3030 365f 6175 746f 5f32  ask..0006_auto_2
+000001b0: 6173 6b5a 1730 3030 365f 6175 746f 5f32  askZ.0006_auto_2
 000001c0: 3031 3930 3931 365f 3136 3435 da05 5175  0190916_1645..Qu
 000001d0: 6575 65da 0269 6454 46da 0249 4429 04da  eue..idTF..ID)..
 000001e0: 0c61 7574 6f5f 6372 6561 7465 64da 0b70  .auto_created..p
 000001f0: 7269 6d61 7279 5f6b 6579 da09 7365 7269  rimary_key..seri
 00000200: 616c 697a 65da 0c76 6572 626f 7365 5f6e  alize..verbose_n
 00000210: 616d 65da 0763 7265 6174 6564 2902 da0c  ame..created)...
-00000220: 6175 746f 5f6e 6f77 5f61 6464 720d 0000  auto_now_addr...
+00000220: 6175 746f 5f6e 6f77 5f61 6464 720c 0000  auto_now_addr...
 00000230: 00da 086d 6f64 6966 6965 6429 02da 0861  ...modified)...a
-00000240: 7574 6f5f 6e6f 7772 0d00 0000 da05 7661  uto_nowr......va
+00000240: 7574 6f5f 6e6f 7772 0c00 0000 da05 7661  uto_nowr......va
 00000250: 6c75 65e9 3200 0000 2903 da05 626c 616e  lue.2...)...blan
 00000260: 6bda 0a6d 6178 5f6c 656e 6774 68da 046e  k..max_length..n
 00000270: 756c 6cda 056c 6162 656c da10 6973 5f64  ull..label..is_d
 00000280: 6566 6175 6c74 5f76 616c 7565 2901 da07  efault_value)...
 00000290: 6465 6661 756c 74da 0a73 6f72 745f 6f72  default..sort_or
-000002a0: 6465 7229 0272 1400 0000 7216 0000 00da  der).r....r.....
+000002a0: 6465 7229 0272 1300 0000 7215 0000 00da  der).r....r.....
 000002b0: 0c70 6172 656e 745f 7661 6c75 65e9 1400  .parent_value...
 000002c0: 0000 da09 6973 5f61 6374 6976 65da 0969  ....is_active..i
 000002d0: 735f 7379 7374 656d da13 7665 7262 6f73  s_system..verbos
 000002e0: 655f 6e61 6d65 5f70 6c75 7261 6cda 0651  e_name_plural..Q
 000002f0: 7565 7565 7329 03da 046e 616d 65da 0666  ueues)...name..f
 00000300: 6965 6c64 73da 076f 7074 696f 6e73 da06  ields..options..
 00000310: 7469 636b 6574 da05 7175 6575 657a 1064  ticket..queuez.d
 00000320: 6a61 7574 6f74 6173 6b2e 5175 6575 6529  jautotask.Queue)
-00000330: 0472 1400 0000 7216 0000 00da 096f 6e5f  .r....r......on_
+00000330: 0472 1300 0000 7215 0000 00da 096f 6e5f  .r....r......on_
 00000340: 6465 6c65 7465 da02 746f 2903 da0a 6d6f  delete..to)...mo
-00000350: 6465 6c5f 6e61 6d65 7221 0000 00da 0566  del_namer!.....f
+00000350: 6465 6c5f 6e61 6d65 7220 0000 00da 0566  del_namer .....f
 00000360: 6965 6c64 4e29 16da 085f 5f6e 616d 655f  ieldN)...__name_
 00000370: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 00000380: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
 00000390: 656e 6465 6e63 6965 7372 0200 0000 da0b  endenciesr......
 000003a0: 4372 6561 7465 4d6f 6465 6c72 0300 0000  CreateModelr....
 000003b0: da09 4175 746f 4669 656c 64da 1164 6a61  ..AutoField..dja
 000003c0: 6e67 6f5f 6578 7465 6e73 696f 6e73 da02  ngo_extensions..
-000003d0: 6462 7222 0000 00da 1543 7265 6174 696f  dbr".....Creatio
+000003d0: 6462 7221 0000 00da 1543 7265 6174 696f  dbr!.....Creatio
 000003e0: 6e44 6174 6554 696d 6546 6965 6c64 da19  nDateTimeField..
 000003f0: 4d6f 6469 6669 6361 7469 6f6e 4461 7465  ModificationDate
 00000400: 5469 6d65 4669 656c 64da 0943 6861 7246  TimeField..CharF
 00000410: 6965 6c64 da0c 426f 6f6c 6561 6e46 6965  ield..BooleanFie
 00000420: 6c64 da19 506f 7369 7469 7665 536d 616c  ld..PositiveSmal
 00000430: 6c49 6e74 6567 6572 4669 656c 64da 0841  lIntegerField..A
 00000440: 6464 4669 656c 64da 0a46 6f72 6569 676e  ddField..Foreign
 00000450: 4b65 79da 0664 6a61 6e67 6fda 0864 656c  Key..django..del
 00000460: 6574 696f 6eda 0853 4554 5f4e 554c 4cda  etion..SET_NULL.
-00000470: 0a6f 7065 7261 7469 6f6e 73a9 0072 3d00  .operations..r=.
-00000480: 0000 723d 0000 00fa 622f 686f 6d65 2f72  ..r=....b/home/r
+00000470: 0a6f 7065 7261 7469 6f6e 73a9 0072 3c00  .operations..r<.
+00000480: 0000 723c 0000 00fa 622f 686f 6d65 2f72  ..r<....b/home/r
 00000490: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
 000004a0: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
 000004b0: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
 000004c0: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
 000004d0: 2f30 3030 375f 6175 746f 5f32 3031 3930  /0007_auto_20190
 000004e0: 3931 375f 3130 3039 2e70 7972 0400 0000  917_1009.pyr....
 000004f0: 0800 0000 7332 0000 0008 0302 ff04 0504  ....s2..........
 00000500: 0102 0214 0114 0114 0112 0112 010e 0110  ................
 00000510: 0112 010e 010e f602 0d02 0002 ff02 f204  ................
 00000520: 1204 0102 0102 0118 fd04 ed72 0400 0000  ...........r....
 00000530: 2908 da09 646a 616e 676f 2e64 6272 0200  )...django.dbr..
 00000540: 0000 7203 0000 00da 1964 6a61 6e67 6f2e  ..r......django.
 00000550: 6462 2e6d 6f64 656c 732e 6465 6c65 7469  db.models.deleti
-00000560: 6f6e 7239 0000 00da 1b64 6a61 6e67 6f5f  onr9.....django_
+00000560: 6f6e 7238 0000 00da 1b64 6a61 6e67 6f5f  onr8.....django_
 00000570: 6578 7465 6e73 696f 6e73 2e64 622e 6669  extensions.db.fi
-00000580: 656c 6473 7230 0000 0072 0400 0000 723d  eldsr0...r....r=
-00000590: 0000 0072 3d00 0000 723d 0000 0072 3e00  ...r=...r=...r>.
+00000580: 656c 6473 722f 0000 0072 0400 0000 723c  eldsr/...r....r<
+00000590: 0000 0072 3c00 0000 723c 0000 0072 3d00  ...r<...r<...r=.
 000005a0: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
 000005b0: 7306 0000 0010 0108 0108 03              s..........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0008_auto_20190917_1454.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0008_auto_20190917_1454.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1843 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 3307 0000  U.........Kd3...
+00000000: 550d 0d0a 0000 0000 3268 4c64 3307 0000  U.......2hLd3...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
@@ -42,15 +42,15 @@
 00000290: 5f64 6174 6529 02da 0562 6c61 6e6b da04  _date)...blank..
 000002a0: 6e75 6c6c 2902 7a09 2d6d 6f64 6966 6965  null).z.-modifie
 000002b0: 647a 082d 6372 6561 7465 6429 03da 086f  dz.-created)...o
 000002c0: 7264 6572 696e 67da 0d67 6574 5f6c 6174  rdering..get_lat
 000002d0: 6573 745f 6279 da08 6162 7374 7261 6374  est_by..abstract
 000002e0: 2903 7212 0000 00da 0666 6965 6c64 73da  ).r......fields.
 000002f0: 076f 7074 696f 6e73 da05 7175 6575 6529  .options..queue)
-00000300: 0272 1200 0000 7220 0000 00da 0e74 6963  .r....r .....tic
+00000300: 0272 1200 0000 7220 0000 005a 0e74 6963  .r....r ...Z.tic
 00000310: 6b65 7470 7269 6f72 6974 79da 1376 6572  ketpriority..ver
 00000320: 626f 7365 5f6e 616d 655f 706c 7572 616c  bose_name_plural
 00000330: 7a11 5469 636b 6574 2070 7269 6f72 6974  z.Ticket priorit
 00000340: 6965 73da 0c74 6963 6b65 7473 7461 7475  ies..ticketstatu
 00000350: 737a 0f54 6963 6b65 7420 7374 6174 7573  sz.Ticket status
 00000360: 6573 da06 7469 636b 6574 da07 6163 636f  es..ticket..acco
 00000370: 756e 747a 1264 6a61 7574 6f74 6173 6b2e  untz.djautotask.
@@ -71,29 +71,29 @@
 00000460: 64da 0943 6861 7246 6965 6c64 da0c 426f  d..CharField..Bo
 00000470: 6f6c 6561 6e46 6965 6c64 da0d 4461 7465  oleanField..Date
 00000480: 5469 6d65 4669 656c 64da 1141 6c74 6572  TimeField..Alter
 00000490: 4d6f 6465 6c4f 7074 696f 6e73 da08 4164  ModelOptions..Ad
 000004a0: 6446 6965 6c64 da0a 466f 7265 6967 6e4b  dField..ForeignK
 000004b0: 6579 da06 646a 616e 676f da08 6465 6c65  ey..django..dele
 000004c0: 7469 6f6e da08 5345 545f 4e55 4c4c da0a  tion..SET_NULL..
-000004d0: 6f70 6572 6174 696f 6e73 a900 723f 0000  operations..r?..
-000004e0: 0072 3f00 0000 fa62 2f68 6f6d 652f 7275  .r?....b/home/ru
+000004d0: 6f70 6572 6174 696f 6e73 a900 723e 0000  operations..r>..
+000004e0: 0072 3e00 0000 fa62 2f68 6f6d 652f 7275  .r>....b/home/ru
 000004f0: 6e6e 6572 2f77 6f72 6b2f 646a 616e 676f  nner/work/django
 00000500: 2d61 7574 6f74 6173 6b2f 646a 616e 676f  -autotask/django
 00000510: 2d61 7574 6f74 6173 6b2f 646a 6175 746f  -autotask/djauto
 00000520: 7461 736b 2f6d 6967 7261 7469 6f6e 732f  task/migrations/
 00000530: 3030 3038 5f61 7574 6f5f 3230 3139 3039  0008_auto_201909
 00000540: 3137 5f31 3435 342e 7079 7204 0000 0008  17_1454.pyr.....
 00000550: 0000 0073 4600 0000 0803 02ff 0405 0401  ...sF...........
 00000560: 0202 1401 1401 1401 0e01 0e01 0e01 10f9  ................
 00000570: 020a 0201 0201 02fd 04f5 0411 0401 0201  ................
 00000580: 02fe 0404 0401 0201 06fe 0404 0401 0201  ................
 00000590: 06fe 0404 0401 0201 0201 18fd 04e2 7204  ..............r.
 000005a0: 0000 0029 08da 0964 6a61 6e67 6f2e 6462  ...)...django.db
 000005b0: 7202 0000 0072 0300 0000 da19 646a 616e  r....r......djan
 000005c0: 676f 2e64 622e 6d6f 6465 6c73 2e64 656c  go.db.models.del
-000005d0: 6574 696f 6e72 3b00 0000 da1b 646a 616e  etionr;.....djan
+000005d0: 6574 696f 6e72 3a00 0000 da1b 646a 616e  etionr:.....djan
 000005e0: 676f 5f65 7874 656e 7369 6f6e 732e 6462  go_extensions.db
-000005f0: 2e66 6965 6c64 7372 3100 0000 7204 0000  .fieldsr1...r...
-00000600: 0072 3f00 0000 723f 0000 0072 3f00 0000  .r?...r?...r?...
-00000610: 7240 0000 00da 083c 6d6f 6475 6c65 3e03  r@.....<module>.
+000005f0: 2e66 6965 6c64 7372 3000 0000 7204 0000  .fieldsr0...r...
+00000600: 0072 3e00 0000 723e 0000 0072 3e00 0000  .r>...r>...r>...
+00000610: 723f 0000 00da 083c 6d6f 6475 6c65 3e03  r?.....<module>.
 00000620: 0000 0073 0600 0000 1001 0801 0803       ...s..........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0009_auto_20190918_1525.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0009_auto_20190918_1525.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 4964 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 6413 0000  U.........Kdd...
+00000000: 550d 0d0a 0000 0000 3268 4c64 6413 0000  U.......2hLdd...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
@@ -73,15 +73,15 @@
 00000480: 0000 0029 01da 0a6d 6178 5f6c 656e 6774  ...)...max_lengt
 00000490: 68da 066e 756d 6265 72e9 3200 0000 2902  h..number.2...).
 000004a0: 7214 0000 00da 046e 756c 6cda 0b64 6573  r......null..des
 000004b0: 6372 6970 7469 6f6e 69d0 0700 00da 0c61  criptioni......a
 000004c0: 6374 7561 6c5f 686f 7572 73e9 0200 0000  ctual_hours.....
 000004d0: e909 0000 0029 03da 0e64 6563 696d 616c  .....)...decimal
 000004e0: 5f70 6c61 6365 73da 0a6d 6178 5f64 6967  _places..max_dig
-000004f0: 6974 7372 1700 0000 da13 636f 6d70 6c65  itsr......comple
+000004f0: 6974 7372 1700 0000 5a13 636f 6d70 6c65  itsr....Z.comple
 00000500: 7465 645f 6461 7465 5f74 696d 6529 0172  ted_date_time).r
 00000510: 1700 0000 da14 636f 6d70 6c65 7465 645f  ......completed_
 00000520: 7065 7263 656e 7461 6765 7201 0000 0029  percentager....)
 00000530: 01da 0764 6566 6175 6c74 da08 6475 7261  ...default..dura
 00000540: 7469 6f6e da0f 7374 6172 745f 6461 7465  tion..start_date
 00000550: 5f74 696d 65da 0d65 6e64 5f64 6174 655f  _time..end_date_
 00000560: 7469 6d65 da0e 6573 7469 6d61 7465 645f  time..estimated_
@@ -99,49 +99,49 @@
 00000620: 6162 7374 7261 6374 2903 7212 0000 00da  abstract).r.....
 00000630: 0666 6965 6c64 73da 076f 7074 696f 6e73  .fields..options
 00000640: da0d 5072 6f6a 6563 7453 7461 7475 73da  ..ProjectStatus.
 00000650: 0576 616c 7565 2903 da05 626c 616e 6b72  .value)...blankr
 00000660: 1400 0000 7217 0000 00da 056c 6162 656c  ....r......label
 00000670: da10 6973 5f64 6566 6175 6c74 5f76 616c  ..is_default_val
 00000680: 7565 da0a 736f 7274 5f6f 7264 6572 2902  ue..sort_order).
-00000690: 7231 0000 0072 1700 0000 da0c 7061 7265  r1...r......pare
+00000690: 7230 0000 0072 1700 0000 da0c 7061 7265  r0...r......pare
 000006a0: 6e74 5f76 616c 7565 e914 0000 00da 0969  nt_value.......i
 000006b0: 735f 6163 7469 7665 da09 6973 5f73 7973  s_active..is_sys
 000006c0: 7465 6dda 1376 6572 626f 7365 5f6e 616d  tem..verbose_nam
 000006d0: 655f 706c 7572 616c 7a10 5072 6f6a 6563  e_pluralz.Projec
 000006e0: 7420 7374 6174 7573 6573 da0b 5072 6f6a  t statuses..Proj
-000006f0: 6563 7454 7970 6572 2c00 0000 da07 7072  ectTyper,.....pr
+000006f0: 6563 7454 7970 6572 2b00 0000 da07 7072  ectTyper+.....pr
 00000700: 6f6a 6563 74da 0673 7461 7475 737a 1864  oject..statusz.d
 00000710: 6a61 7574 6f74 6173 6b2e 5072 6f6a 6563  jautotask.Projec
 00000720: 7453 7461 7475 7329 03da 0a6d 6f64 656c  tStatus)...model
 00000730: 5f6e 616d 6572 1200 0000 da05 6669 656c  _namer......fiel
 00000740: 64da 0474 7970 657a 1664 6a61 7574 6f74  d..typez.djautot
 00000750: 6173 6b2e 5072 6f6a 6563 7454 7970 65da  ask.ProjectType.
 00000760: 0674 6963 6b65 747a 1264 6a61 7574 6f74  .ticketz.djautot
 00000770: 6173 6b2e 5072 6f6a 6563 744e 2918 da08  ask.ProjectN)...
 00000780: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
 00000790: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
 000007a0: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
 000007b0: 7202 0000 00da 0b43 7265 6174 654d 6f64  r......CreateMod
 000007c0: 656c 7203 0000 00da 0941 7574 6f46 6965  elr......AutoFie
 000007d0: 6c64 da11 646a 616e 676f 5f65 7874 656e  ld..django_exten
-000007e0: 7369 6f6e 73da 0264 6272 2d00 0000 da15  sions..dbr-.....
+000007e0: 7369 6f6e 73da 0264 6272 2c00 0000 da15  sions..dbr,.....
 000007f0: 4372 6561 7469 6f6e 4461 7465 5469 6d65  CreationDateTime
 00000800: 4669 656c 64da 194d 6f64 6966 6963 6174  Field..Modificat
 00000810: 696f 6e44 6174 6554 696d 6546 6965 6c64  ionDateTimeField
 00000820: da09 4368 6172 4669 656c 64da 0c44 6563  ..CharField..Dec
 00000830: 696d 616c 4669 656c 64da 0d44 6174 6554  imalField..DateT
 00000840: 696d 6546 6965 6c64 da19 506f 7369 7469  imeField..Positi
 00000850: 7665 536d 616c 6c49 6e74 6567 6572 4669  veSmallIntegerFi
 00000860: 656c 64da 0a46 6f72 6569 676e 4b65 79da  eld..ForeignKey.
 00000870: 0664 6a61 6e67 6fda 0864 656c 6574 696f  .django..deletio
 00000880: 6eda 0853 4554 5f4e 554c 4cda 0c42 6f6f  n..SET_NULL..Boo
 00000890: 6c65 616e 4669 656c 64da 0841 6464 4669  leanField..AddFi
 000008a0: 656c 64da 0a6f 7065 7261 7469 6f6e 73a9  eld..operations.
-000008b0: 0072 5600 0000 7256 0000 00fa 622f 686f  .rV...rV....b/ho
+000008b0: 0072 5500 0000 7255 0000 00fa 622f 686f  .rU...rU....b/ho
 000008c0: 6d65 2f72 756e 6e65 722f 776f 726b 2f64  me/runner/work/d
 000008d0: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
 000008e0: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
 000008f0: 6a61 7574 6f74 6173 6b2f 6d69 6772 6174  jautotask/migrat
 00000900: 696f 6e73 2f30 3030 395f 6175 746f 5f32  ions/0009_auto_2
 00000910: 3031 3930 3931 385f 3135 3235 2e70 7972  0190918_1525.pyr
 00000920: 0400 0000 0800 0000 7398 0000 0008 0302  ........s.......
@@ -153,14 +153,14 @@
 00000980: ff02 f204 1204 0102 0214 0114 0114 0112  ................
 00000990: 0112 010e 0110 0112 010e 010e f602 0d02  ................
 000009a0: 0002 ff02 f204 1204 0102 0102 0116 fd04  ................
 000009b0: 0504 0102 0102 0116 fd04 0504 0102 0102  ................
 000009c0: 0116 fd04 b772 0400 0000 2908 da09 646a  .....r....)...dj
 000009d0: 616e 676f 2e64 6272 0200 0000 7203 0000  ango.dbr....r...
 000009e0: 00da 1964 6a61 6e67 6f2e 6462 2e6d 6f64  ...django.db.mod
-000009f0: 656c 732e 6465 6c65 7469 6f6e 7250 0000  els.deletionrP..
+000009f0: 656c 732e 6465 6c65 7469 6f6e 724f 0000  els.deletionrO..
 00000a00: 00da 1b64 6a61 6e67 6f5f 6578 7465 6e73  ...django_extens
-00000a10: 696f 6e73 2e64 622e 6669 656c 6473 7247  ions.db.fieldsrG
-00000a20: 0000 0072 0400 0000 7256 0000 0072 5600  ...r....rV...rV.
-00000a30: 0000 7256 0000 0072 5700 0000 da08 3c6d  ..rV...rW.....<m
+00000a10: 696f 6e73 2e64 622e 6669 656c 6473 7246  ions.db.fieldsrF
+00000a20: 0000 0072 0400 0000 7255 0000 0072 5500  ...r....rU...rU.
+00000a30: 0000 7255 0000 0072 5600 0000 da08 3c6d  ..rU...rV.....<m
 00000a40: 6f64 756c 653e 0300 0000 7306 0000 0010  odule>....s.....
 00000a50: 0108 0108 03                             .....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0009_auto_20190920_1648.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0009_auto_20190920_1648.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 441 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 b901 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 b901 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0500 0000 4000 0000 732e  ..........@...s.
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0010_auto_20190923_0930.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0034_auto_20191210_1518.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1036 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,47 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 0c04 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 f901 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
-00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
-00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
-00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
-00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00000080: 0000 0b00 0000 4000 0000 737c 0000 0065  ......@...s|...e
-00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
-000000a0: 0564 0264 0364 048d 0265 046a 0564 0264  .d.d.d...e.j.d.d
-000000b0: 0564 048d 0265 046a 0564 0264 0664 048d  .d...e.j.d.d.d..
-000000c0: 0265 046a 0664 0264 0765 076a 0864 0864  .e.j.d.d.e.j.d.d
-000000d0: 098d 0164 0a8d 0365 046a 0664 0264 0b65  ...d...e.j.d.d.e
-000000e0: 076a 0864 0864 098d 0164 0a8d 0365 046a  .j.d.d...d...e.j
-000000f0: 0664 0264 0c65 076a 0864 0864 098d 0164  .d.d.e.j.d.d...d
-00000100: 0a8d 0367 065a 0964 0d53 0029 0eda 094d  ...g.Z.d.S.)...M
-00000110: 6967 7261 7469 6f6e 2902 da0a 646a 6175  igration)...djau
-00000120: 746f 7461 736b 5a17 3030 3039 5f61 7574  totaskZ.0009_aut
-00000130: 6f5f 3230 3139 3039 3138 5f31 3532 35da  o_20190918_1525.
-00000140: 0770 726f 6a65 6374 5a13 636f 6d70 6c65  .projectZ.comple
-00000150: 7465 645f 6461 7465 5f74 696d 6529 02da  ted_date_time)..
-00000160: 0a6d 6f64 656c 5f6e 616d 65da 046e 616d  .model_name..nam
-00000170: 65da 0d65 6e64 5f64 6174 655f 7469 6d65  e..end_date_time
-00000180: da0f 7374 6172 745f 6461 7465 5f74 696d  ..start_date_tim
-00000190: 65da 0e63 6f6d 706c 6574 6564 5f64 6174  e..completed_dat
-000001a0: 6554 2901 da04 6e75 6c6c 2903 7207 0000  eT)...null).r...
-000001b0: 0072 0800 0000 da05 6669 656c 64da 0865  .r......field..e
-000001c0: 6e64 5f64 6174 65da 0a73 7461 7274 5f64  nd_date..start_d
-000001d0: 6174 654e 290a da08 5f5f 6e61 6d65 5f5f  ateN)...__name__
-000001e0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000001f0: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
-00000200: 6e64 656e 6369 6573 7202 0000 00da 0b52  ndenciesr......R
-00000210: 656d 6f76 6546 6965 6c64 da08 4164 6446  emoveField..AddF
-00000220: 6965 6c64 7203 0000 00da 0944 6174 6546  ieldr......DateF
-00000230: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
-00000240: a900 7218 0000 0072 1800 0000 fa62 2f68  ..r....r.....b/h
-00000250: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
-00000260: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
-00000270: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
-00000280: 646a 6175 746f 7461 736b 2f6d 6967 7261  djautotask/migra
-00000290: 7469 6f6e 732f 3030 3130 5f61 7574 6f5f  tions/0010_auto_
-000002a0: 3230 3139 3039 3233 5f30 3933 302e 7079  20190923_0930.py
-000002b0: 7204 0000 0006 0000 0073 3c00 0000 0803  r........s<.....
-000002c0: 02ff 0405 0401 0201 02fe 0404 0401 0201  ................
-000002d0: 02fe 0404 0401 0201 02fe 0404 0401 0201  ................
-000002e0: 0201 0afd 0405 0401 0201 0201 0afd 0405  ................
-000002f0: 0401 0201 0201 0afd 04e9 7204 0000 004e  ..........r....N
-00000300: 2904 da09 646a 616e 676f 2e64 6272 0200  )...django.dbr..
-00000310: 0000 7203 0000 0072 0400 0000 7218 0000  ..r....r....r...
-00000320: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000330: da08 3c6d 6f64 756c 653e 0300 0000 7302  ..<module>....s.
-00000340: 0000 0010 03                             .....
+00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
+00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
+00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
+00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
+00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
+00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
+000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
+000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
+000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
+000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
+000000e0: 02da 0a64 6a61 7574 6f74 6173 6bda 1830  ...djautotask..0
+000000f0: 3033 335f 6d65 7267 655f 3230 3139 3132  033_merge_201912
+00000100: 3034 5f31 3032 32da 0474 6173 6bda 0870  04_1022..task..p
+00000110: 7269 6f72 6974 7954 7a13 646a 6175 746f  riorityTz.djauto
+00000120: 7461 736b 2e50 7269 6f72 6974 7929 04da  task.Priority)..
+00000130: 0562 6c61 6e6b da04 6e75 6c6c da09 6f6e  .blank..null..on
+00000140: 5f64 656c 6574 65da 0274 6f29 03da 0a6d  _delete..to)...m
+00000150: 6f64 656c 5f6e 616d 65da 046e 616d 65da  odel_name..name.
+00000160: 0566 6965 6c64 4e29 0dda 085f 5f6e 616d  .fieldN)...__nam
+00000170: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000180: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
+00000190: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
+000001a0: da0a 416c 7465 7246 6965 6c64 7203 0000  ..AlterFieldr...
+000001b0: 00da 0a46 6f72 6569 676e 4b65 79da 0664  ...ForeignKey..d
+000001c0: 6a61 6e67 6fda 0264 62da 0864 656c 6574  jango..db..delet
+000001d0: 696f 6eda 0853 4554 5f4e 554c 4cda 0a6f  ion..SET_NULL..o
+000001e0: 7065 7261 7469 6f6e 73a9 0072 1b00 0000  perations..r....
+000001f0: 721b 0000 00fa 622f 686f 6d65 2f72 756e  r.....b/home/run
+00000200: 6e65 722f 776f 726b 2f64 6a61 6e67 6f2d  ner/work/django-
+00000210: 6175 746f 7461 736b 2f64 6a61 6e67 6f2d  autotask/django-
+00000220: 6175 746f 7461 736b 2f64 6a61 7574 6f74  autotask/djautot
+00000230: 6173 6b2f 6d69 6772 6174 696f 6e73 2f30  ask/migrations/0
+00000240: 3033 345f 6175 746f 5f32 3031 3931 3231  034_auto_2019121
+00000250: 305f 3135 3138 2e70 7972 0400 0000 0700  0_1518.pyr......
+00000260: 0000 7310 0000 0008 0302 ff04 0504 0102  ..s.............
+00000270: 0102 0118 fd04 ff72 0400 0000 2906 da09  .......r....)...
+00000280: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
+00000290: 0000 00da 1964 6a61 6e67 6f2e 6462 2e6d  .....django.db.m
+000002a0: 6f64 656c 732e 6465 6c65 7469 6f6e 7216  odels.deletionr.
+000002b0: 0000 0072 0400 0000 721b 0000 0072 1b00  ...r....r....r..
+000002c0: 0000 721b 0000 0072 1c00 0000 da08 3c6d  ..r....r......<m
+000002d0: 6f64 756c 653e 0300 0000 7304 0000 0010  odule>....s.....
+000002e0: 0108 03                                  ...
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0011_auto_20190923_1157.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0011_auto_20190923_1157.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 360 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 6801 0000  U.........Kdh...
+00000000: 550d 0d0a 0000 0000 3268 4c64 6801 0000  U.......2hLdh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0400 0000 4000 0000 7326  ..........@...s&
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0013_auto_20190923_1439.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0058_auto_20200408_1022.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 446 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,48 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 be01 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 cd02 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
-00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
-00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
-00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
-00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
-00000070: 0000 0000 0000 0500 0000 4000 0000 732e  ..........@...s.
-00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
-00000090: 0365 046a 0564 0264 0364 048d 0265 046a  .e.j.d.d.d...e.j
-000000a0: 0564 0564 0364 048d 0267 025a 0664 0653  .d.d.d...g.Z.d.S
-000000b0: 0029 07da 094d 6967 7261 7469 6f6e 2902  .)...Migration).
-000000c0: da0a 646a 6175 746f 7461 736b 5a18 3030  ..djautotaskZ.00
-000000d0: 3132 5f6d 6572 6765 5f32 3031 3930 3932  12_merge_2019092
-000000e0: 335f 3134 3339 da0d 7072 6f6a 6563 7473  3_1439..projects
-000000f0: 7461 7475 73da 0576 616c 7565 2902 da0a  tatus..value)...
-00000100: 6d6f 6465 6c5f 6e61 6d65 da04 6e61 6d65  model_name..name
-00000110: da0b 7072 6f6a 6563 7474 7970 654e 2907  ..projecttypeN).
-00000120: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000130: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000140: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
-00000150: 6573 7202 0000 00da 0b52 656d 6f76 6546  esr......RemoveF
-00000160: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
-00000170: a900 7210 0000 0072 1000 0000 fa62 2f68  ..r....r.....b/h
-00000180: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
-00000190: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
-000001a0: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
-000001b0: 646a 6175 746f 7461 736b 2f6d 6967 7261  djautotask/migra
-000001c0: 7469 6f6e 732f 3030 3133 5f61 7574 6f5f  tions/0013_auto_
-000001d0: 3230 3139 3039 3233 5f31 3433 392e 7079  20190923_1439.py
-000001e0: 7203 0000 0006 0000 0073 1600 0000 0803  r........s......
-000001f0: 02ff 0405 0401 0201 02fe 0404 0401 0201  ................
-00000200: 02fe 04fb 7203 0000 004e 2903 da09 646a  ....r....N)...dj
-00000210: 616e 676f 2e64 6272 0200 0000 7203 0000  ango.dbr....r...
-00000220: 0072 1000 0000 7210 0000 0072 1000 0000  .r....r....r....
-00000230: 7211 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
-00000240: 0000 0073 0200 0000 0c03                 ...s......
+00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
+00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
+00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
+00000080: 0000 0a00 0000 4000 0000 7356 0000 0065  ......@...sV...e
+00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
+000000a0: 0564 0264 0365 066a 0764 0464 0564 0667  .d.d.e.j.d.d.d.g
+000000b0: 0264 0764 0464 088d 0464 098d 0365 046a  .d.d.d...d...e.j
+000000c0: 0564 0a64 0365 066a 0764 0464 0564 0667  .d.d.e.j.d.d.d.g
+000000d0: 0264 0764 0464 088d 0464 098d 0367 025a  .d.d.d...d...g.Z
+000000e0: 0864 0b53 0029 0cda 094d 6967 7261 7469  .d.S.)...Migrati
+000000f0: 6f6e 2902 da0a 646a 6175 746f 7461 736b  on)...djautotask
+00000100: 5a17 3030 3537 5f61 7574 6f5f 3230 3230  Z.0057_auto_2020
+00000110: 3034 3036 5f31 3632 305a 0874 6173 6b6e  0406_1620Z.taskn
+00000120: 6f74 65da 0770 7562 6c69 7368 5429 02e9  ote..publishT)..
+00000130: 0100 0000 7a12 416c 6c20 4175 746f 7461  ....z.All Autota
+00000140: 736b 2055 7365 7273 2902 e902 0000 007a  sk Users)......z
+00000150: 0e49 6e74 6572 6e61 6c20 5573 6572 73e9  .Internal Users.
+00000160: 1400 0000 2904 da05 626c 616e 6bda 0763  ....)...blank..c
+00000170: 686f 6963 6573 da0a 6d61 785f 6c65 6e67  hoices..max_leng
+00000180: 7468 da04 6e75 6c6c 2903 da0a 6d6f 6465  th..null)...mode
+00000190: 6c5f 6e61 6d65 da04 6e61 6d65 da05 6669  l_name..name..fi
+000001a0: 656c 645a 0a74 6963 6b65 746e 6f74 654e  eldZ.ticketnoteN
+000001b0: 2909 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000001c0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000001d0: 6e61 6d65 5f5f da0c 6465 7065 6e64 656e  name__..dependen
+000001e0: 6369 6573 7202 0000 00da 0a41 6c74 6572  ciesr......Alter
+000001f0: 4669 656c 6472 0300 0000 da09 4368 6172  Fieldr......Char
+00000200: 4669 656c 64da 0a6f 7065 7261 7469 6f6e  Field..operation
+00000210: 73a9 0072 1800 0000 7218 0000 00fa 622f  s..r....r.....b/
+00000220: 686f 6d65 2f72 756e 6e65 722f 776f 726b  home/runner/work
+00000230: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
+00000240: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
+00000250: 2f64 6a61 7574 6f74 6173 6b2f 6d69 6772  /djautotask/migr
+00000260: 6174 696f 6e73 2f30 3035 385f 6175 746f  ations/0058_auto
+00000270: 5f32 3032 3030 3430 385f 3130 3232 2e70  _20200408_1022.p
+00000280: 7972 0400 0000 0600 0000 731a 0000 0008  yr........s.....
+00000290: 0302 ff04 0504 0102 0102 0114 fd04 0504  ................
+000002a0: 0102 0102 0114 fd04 fa72 0400 0000 4e29  .........r....N)
+000002b0: 04da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
+000002c0: 0072 0300 0000 7204 0000 0072 1800 0000  .r....r....r....
+000002d0: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
+000002e0: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
+000002f0: 0000 1003                                ....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0014_auto_20190930_1548.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0014_auto_20190930_1548.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 6182 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 2618 0000  U.........Kd&...
+00000000: 550d 0d0a 0000 0000 3268 4c64 2618 0000  U.......2hLd&...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
@@ -67,47 +67,47 @@
 00000420: 6a13 6a14 642b 6426 8d03 6427 8d03 6504  j.j.d+d&..d'..e.
 00000430: 6a10 6423 642c 6506 6a11 6404 6512 6a09  j.d#d,e.j.d.e.j.
 00000440: 6a06 6a13 6a14 642d 6426 8d03 6427 8d03  j.j.j.d-d&..d'..
 00000450: 6504 6a10 6423 642e 6506 6a11 6404 6512  e.j.d#d.e.j.d.e.
 00000460: 6a09 6a06 6a13 6a14 642f 6426 8d03 6427  j.j.j.j.d/d&..d'
 00000470: 8d03 670a 5a15 6430 5300 2931 da09 4d69  ..g.Z.d0S.)1..Mi
 00000480: 6772 6174 696f 6e29 02da 0a64 6a61 7574  gration)...djaut
-00000490: 6f74 6173 6bda 1730 3031 335f 6175 746f  otask..0013_auto
+00000490: 6f74 6173 6b5a 1730 3031 335f 6175 746f  otaskZ.0013_auto
 000004a0: 5f32 3031 3930 3932 335f 3134 3339 da09  _20190923_1439..
 000004b0: 4973 7375 6554 7970 65da 0269 6454 46da  IssueType..idTF.
 000004c0: 0249 4429 04da 0c61 7574 6f5f 6372 6561  .ID)...auto_crea
 000004d0: 7465 64da 0b70 7269 6d61 7279 5f6b 6579  ted..primary_key
 000004e0: da09 7365 7269 616c 697a 65da 0c76 6572  ..serialize..ver
 000004f0: 626f 7365 5f6e 616d 65da 0763 7265 6174  bose_name..creat
 00000500: 6564 2902 da0c 6175 746f 5f6e 6f77 5f61  ed)...auto_now_a
-00000510: 6464 720d 0000 00da 086d 6f64 6966 6965  ddr......modifie
-00000520: 6429 02da 0861 7574 6f5f 6e6f 7772 0d00  d)...auto_nowr..
+00000510: 6464 720c 0000 00da 086d 6f64 6966 6965  ddr......modifie
+00000520: 6429 02da 0861 7574 6f5f 6e6f 7772 0c00  d)...auto_nowr..
 00000530: 0000 da05 6c61 6265 6ce9 3200 0000 2903  ....label.2...).
 00000540: da05 626c 616e 6bda 0a6d 6178 5f6c 656e  ..blank..max_len
 00000550: 6774 68da 046e 756c 6cda 1069 735f 6465  gth..null..is_de
 00000560: 6661 756c 745f 7661 6c75 6529 01da 0764  fault_value)...d
 00000570: 6566 6175 6c74 da0a 736f 7274 5f6f 7264  efault..sort_ord
-00000580: 6572 2902 7214 0000 0072 1600 0000 da0c  er).r....r......
+00000580: 6572 2902 7213 0000 0072 1500 0000 da0c  er).r....r......
 00000590: 7061 7265 6e74 5f76 616c 7565 e914 0000  parent_value....
 000005a0: 00da 0969 735f 6163 7469 7665 da09 6973  ...is_active..is
 000005b0: 5f73 7973 7465 6dda 0861 6273 7472 6163  _system..abstrac
 000005c0: 7429 03da 046e 616d 65da 0666 6965 6c64  t)...name..field
 000005d0: 73da 076f 7074 696f 6e73 da06 536f 7572  s..options..Sour
 000005e0: 6365 da0c 5375 6249 7373 7565 5479 7065  ce..SubIssueType
 000005f0: da0e 5469 636b 6574 4361 7465 676f 7279  ..TicketCategory
-00000600: 721f 0000 00e9 1e00 0000 2901 7215 0000  r.........).r...
+00000600: 721e 0000 00e9 1e00 0000 2901 7214 0000  r.........).r...
 00000610: 00da 0661 6374 6976 65da 1376 6572 626f  ...active..verbo
 00000620: 7365 5f6e 616d 655f 706c 7572 616c 7a11  se_name_pluralz.
 00000630: 5469 636b 6574 2063 6174 6567 6f72 6965  Ticket categorie
 00000640: 73da 0a54 6963 6b65 7454 7970 65da 0674  s..TicketType..t
 00000650: 6963 6b65 74da 0863 6174 6567 6f72 797a  icket..categoryz
 00000660: 1964 6a61 7574 6f74 6173 6b2e 5469 636b  .djautotask.Tick
-00000670: 6574 4361 7465 676f 7279 2903 7216 0000  etCategory).r...
+00000670: 6574 4361 7465 676f 7279 2903 7215 0000  etCategory).r...
 00000680: 00da 096f 6e5f 6465 6c65 7465 da02 746f  ...on_delete..to
-00000690: 2903 da0a 6d6f 6465 6c5f 6e61 6d65 721f  )...model_namer.
+00000690: 2903 da0a 6d6f 6465 6c5f 6e61 6d65 721e  )...model_namer.
 000006a0: 0000 00da 0566 6965 6c64 da0a 6973 7375  .....field..issu
 000006b0: 655f 7479 7065 7a14 646a 6175 746f 7461  e_typez.djautota
 000006c0: 736b 2e49 7373 7565 5479 7065 da06 736f  sk.IssueType..so
 000006d0: 7572 6365 7a11 646a 6175 746f 7461 736b  urcez.djautotask
 000006e0: 2e53 6f75 7263 65da 0e73 7562 5f69 7373  .Source..sub_iss
 000006f0: 7565 5f74 7970 657a 1764 6a61 7574 6f74  ue_typez.djautot
 00000700: 6173 6b2e 5375 6249 7373 7565 5479 7065  ask.SubIssueType
@@ -115,26 +115,26 @@
 00000720: 736b 2e54 6963 6b65 7454 7970 654e 2916  sk.TicketTypeN).
 00000730: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
 00000740: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
 00000750: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
 00000760: 6573 7202 0000 00da 0b43 7265 6174 654d  esr......CreateM
 00000770: 6f64 656c 7203 0000 00da 0941 7574 6f46  odelr......AutoF
 00000780: 6965 6c64 da11 646a 616e 676f 5f65 7874  ield..django_ext
-00000790: 656e 7369 6f6e 73da 0264 6272 2000 0000  ensions..dbr ...
+00000790: 656e 7369 6f6e 73da 0264 6272 1f00 0000  ensions..dbr....
 000007a0: da15 4372 6561 7469 6f6e 4461 7465 5469  ..CreationDateTi
 000007b0: 6d65 4669 656c 64da 194d 6f64 6966 6963  meField..Modific
 000007c0: 6174 696f 6e44 6174 6554 696d 6546 6965  ationDateTimeFie
 000007d0: 6c64 da09 4368 6172 4669 656c 64da 0c42  ld..CharField..B
 000007e0: 6f6f 6c65 616e 4669 656c 64da 1950 6f73  ooleanField..Pos
 000007f0: 6974 6976 6553 6d61 6c6c 496e 7465 6765  itiveSmallIntege
 00000800: 7246 6965 6c64 da08 4164 6446 6965 6c64  rField..AddField
 00000810: da0a 466f 7265 6967 6e4b 6579 da06 646a  ..ForeignKey..dj
 00000820: 616e 676f da08 6465 6c65 7469 6f6e da08  ango..deletion..
 00000830: 5345 545f 4e55 4c4c da0a 6f70 6572 6174  SET_NULL..operat
-00000840: 696f 6e73 a900 7246 0000 0072 4600 0000  ions..rF...rF...
+00000840: 696f 6e73 a900 7245 0000 0072 4500 0000  ions..rE...rE...
 00000850: fa62 2f68 6f6d 652f 7275 6e6e 6572 2f77  .b/home/runner/w
 00000860: 6f72 6b2f 646a 616e 676f 2d61 7574 6f74  ork/django-autot
 00000870: 6173 6b2f 646a 616e 676f 2d61 7574 6f74  ask/django-autot
 00000880: 6173 6b2f 646a 6175 746f 7461 736b 2f6d  ask/djautotask/m
 00000890: 6967 7261 7469 6f6e 732f 3030 3134 5f61  igrations/0014_a
 000008a0: 7574 6f5f 3230 3139 3039 3330 5f31 3534  uto_20190930_154
 000008b0: 382e 7079 7204 0000 0008 0000 0073 d000  8.pyr........s..
@@ -150,14 +150,14 @@
 00000950: 1201 0e01 0ef7 020c 0200 02ff 02f3 0411  ................
 00000960: 0401 0201 0201 16fd 0405 0401 0201 0201  ................
 00000970: 16fd 0405 0401 0201 0201 16fd 0405 0401  ................
 00000980: 0201 0201 16fd 0405 0401 0201 0201 16fd  ................
 00000990: 049a 7204 0000 0029 08da 0964 6a61 6e67  ..r....)...djang
 000009a0: 6f2e 6462 7202 0000 0072 0300 0000 da19  o.dbr....r......
 000009b0: 646a 616e 676f 2e64 622e 6d6f 6465 6c73  django.db.models
-000009c0: 2e64 656c 6574 696f 6e72 4200 0000 da1b  .deletionrB.....
+000009c0: 2e64 656c 6574 696f 6e72 4100 0000 da1b  .deletionrA.....
 000009d0: 646a 616e 676f 5f65 7874 656e 7369 6f6e  django_extension
-000009e0: 732e 6462 2e66 6965 6c64 7372 3900 0000  s.db.fieldsr9...
-000009f0: 7204 0000 0072 4600 0000 7246 0000 0072  r....rF...rF...r
-00000a00: 4600 0000 7247 0000 00da 083c 6d6f 6475  F...rG.....<modu
+000009e0: 732e 6462 2e66 6965 6c64 7372 3800 0000  s.db.fieldsr8...
+000009f0: 7204 0000 0072 4500 0000 7245 0000 0072  r....rE...rE...r
+00000a00: 4500 0000 7246 0000 00da 083c 6d6f 6475  E...rF.....<modu
 00000a10: 6c65 3e03 0000 0073 0600 0000 1001 0801  le>....s........
 00000a20: 0803                                     ..
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0015_auto_20191001_0847.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0015_auto_20191001_0847.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1583 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 2f06 0000  U.........Kd/...
+00000000: 550d 0d0a 0000 0000 3268 4c64 2f06 0000  U.......2hLd/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
@@ -19,74 +19,74 @@
 00000120: 6413 6506 6a0d 6404 6414 6404 640e 8d03  d.e.j.d.d.d.d...
 00000130: 6602 6415 6506 6a0e 6405 6410 8d01 6602  f.d.e.j.d.d...f.
 00000140: 6416 6506 6a0e 6405 6410 8d01 6602 6709  d.e.j.d.d...f.g.
 00000150: 6417 6418 6901 6419 8d03 6504 6a10 641a  d.d.i.d...e.j.d.
 00000160: 641b 6506 6a11 6404 6512 6a09 6a06 6a13  d.e.j.d.e.j.j.j.
 00000170: 6a14 641c 641d 8d03 641e 8d03 6702 5a15  j.d.d...d...g.Z.
 00000180: 641f 5300 2920 da09 4d69 6772 6174 696f  d.S.) ..Migratio
-00000190: 6e29 02da 0a64 6a61 7574 6f74 6173 6b5a  n)...djautotaskZ
+00000190: 6e29 02da 0a64 6a61 7574 6f74 6173 6bda  n)...djautotask.
 000001a0: 1730 3031 345f 6175 746f 5f32 3031 3930  .0014_auto_20190
 000001b0: 3933 305f 3135 3438 da0c 4469 7370 6c61  930_1548..Displa
 000001c0: 7943 6f6c 6f72 da02 6964 5446 da02 4944  yColor..idTF..ID
 000001d0: 2904 da0c 6175 746f 5f63 7265 6174 6564  )...auto_created
 000001e0: da0b 7072 696d 6172 795f 6b65 79da 0973  ..primary_key..s
 000001f0: 6572 6961 6c69 7a65 da0c 7665 7262 6f73  erialize..verbos
 00000200: 655f 6e61 6d65 da07 6372 6561 7465 6429  e_name..created)
 00000210: 02da 0c61 7574 6f5f 6e6f 775f 6164 6472  ...auto_now_addr
-00000220: 0c00 0000 da08 6d6f 6469 6669 6564 2902  ......modified).
-00000230: da08 6175 746f 5f6e 6f77 720c 0000 00da  ..auto_nowr.....
+00000220: 0d00 0000 da08 6d6f 6469 6669 6564 2902  ......modified).
+00000230: da08 6175 746f 5f6e 6f77 720d 0000 00da  ..auto_nowr.....
 00000240: 056c 6162 656c e932 0000 0029 03da 0562  .label.2...)...b
 00000250: 6c61 6e6b da0a 6d61 785f 6c65 6e67 7468  lank..max_length
 00000260: da04 6e75 6c6c da10 6973 5f64 6566 6175  ..null..is_defau
 00000270: 6c74 5f76 616c 7565 2901 da07 6465 6661  lt_value)...defa
 00000280: 756c 74da 0a73 6f72 745f 6f72 6465 7229  ult..sort_order)
-00000290: 0272 1300 0000 7215 0000 00da 0c70 6172  .r....r......par
+00000290: 0272 1400 0000 7216 0000 00da 0c70 6172  .r....r......par
 000002a0: 656e 745f 7661 6c75 65e9 1400 0000 da09  ent_value.......
 000002b0: 6973 5f61 6374 6976 65da 0969 735f 7379  is_active..is_sy
 000002c0: 7374 656d da13 7665 7262 6f73 655f 6e61  stem..verbose_na
 000002d0: 6d65 5f70 6c75 7261 6c7a 0e44 6973 706c  me_pluralz.Displ
 000002e0: 6179 2063 6f6c 6f72 7329 03da 046e 616d  ay colors)...nam
 000002f0: 65da 0666 6965 6c64 73da 076f 7074 696f  e..fields..optio
 00000300: 6e73 da0e 7469 636b 6574 6361 7465 676f  ns..ticketcatego
 00000310: 7279 da0d 6469 7370 6c61 795f 636f 6c6f  ry..display_colo
 00000320: 727a 1764 6a61 7574 6f74 6173 6b2e 4469  rz.djautotask.Di
-00000330: 7370 6c61 7943 6f6c 6f72 2903 7215 0000  splayColor).r...
+00000330: 7370 6c61 7943 6f6c 6f72 2903 7216 0000  splayColor).r...
 00000340: 00da 096f 6e5f 6465 6c65 7465 da02 746f  ...on_delete..to
-00000350: 2903 da0a 6d6f 6465 6c5f 6e61 6d65 721e  )...model_namer.
+00000350: 2903 da0a 6d6f 6465 6c5f 6e61 6d65 721f  )...model_namer.
 00000360: 0000 00da 0566 6965 6c64 4e29 16da 085f  .....fieldN)..._
 00000370: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 00000380: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
 00000390: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
 000003a0: 0200 0000 da0b 4372 6561 7465 4d6f 6465  ......CreateMode
 000003b0: 6c72 0300 0000 da09 4175 746f 4669 656c  lr......AutoFiel
 000003c0: 64da 1164 6a61 6e67 6f5f 6578 7465 6e73  d..django_extens
-000003d0: 696f 6e73 da02 6462 721f 0000 00da 1543  ions..dbr......C
+000003d0: 696f 6e73 da02 6462 7220 0000 00da 1543  ions..dbr .....C
 000003e0: 7265 6174 696f 6e44 6174 6554 696d 6546  reationDateTimeF
 000003f0: 6965 6c64 da19 4d6f 6469 6669 6361 7469  ield..Modificati
 00000400: 6f6e 4461 7465 5469 6d65 4669 656c 64da  onDateTimeField.
 00000410: 0943 6861 7246 6965 6c64 da0c 426f 6f6c  .CharField..Bool
 00000420: 6561 6e46 6965 6c64 da19 506f 7369 7469  eanField..Positi
 00000430: 7665 536d 616c 6c49 6e74 6567 6572 4669  veSmallIntegerFi
 00000440: 656c 64da 0841 6464 4669 656c 64da 0a46  eld..AddField..F
 00000450: 6f72 6569 676e 4b65 79da 0664 6a61 6e67  oreignKey..djang
 00000460: 6fda 0864 656c 6574 696f 6eda 0853 4554  o..deletion..SET
 00000470: 5f4e 554c 4cda 0a6f 7065 7261 7469 6f6e  _NULL..operation
-00000480: 73a9 0072 3a00 0000 723a 0000 00fa 622f  s..r:...r:....b/
+00000480: 73a9 0072 3b00 0000 723b 0000 00fa 622f  s..r;...r;....b/
 00000490: 686f 6d65 2f72 756e 6e65 722f 776f 726b  home/runner/work
 000004a0: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
 000004b0: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
 000004c0: 2f64 6a61 7574 6f74 6173 6b2f 6d69 6772  /djautotask/migr
 000004d0: 6174 696f 6e73 2f30 3031 355f 6175 746f  ations/0015_auto
 000004e0: 5f32 3031 3931 3030 315f 3038 3437 2e70  _20191001_0847.p
 000004f0: 7972 0400 0000 0800 0000 7330 0000 0008  yr........s0....
 00000500: 0302 ff04 0504 0102 0214 0114 0114 0112  ................
 00000510: 010e 0110 0112 010e 010e f702 0c02 0002  ................
 00000520: ff02 f304 1104 0102 0102 0116 fd04 ee72  ...............r
 00000530: 0400 0000 2908 da09 646a 616e 676f 2e64  ....)...django.d
 00000540: 6272 0200 0000 7203 0000 00da 1964 6a61  br....r......dja
 00000550: 6e67 6f2e 6462 2e6d 6f64 656c 732e 6465  ngo.db.models.de
-00000560: 6c65 7469 6f6e 7236 0000 00da 1b64 6a61  letionr6.....dja
+00000560: 6c65 7469 6f6e 7237 0000 00da 1b64 6a61  letionr7.....dja
 00000570: 6e67 6f5f 6578 7465 6e73 696f 6e73 2e64  ngo_extensions.d
-00000580: 622e 6669 656c 6473 722d 0000 0072 0400  b.fieldsr-...r..
-00000590: 0000 723a 0000 0072 3a00 0000 723a 0000  ..r:...r:...r:..
-000005a0: 0072 3b00 0000 da08 3c6d 6f64 756c 653e  .r;.....<module>
+00000580: 622e 6669 656c 6473 722e 0000 0072 0400  b.fieldsr....r..
+00000590: 0000 723b 0000 0072 3b00 0000 723b 0000  ..r;...r;...r;..
+000005a0: 0072 3c00 0000 da08 3c6d 6f64 756c 653e  .r<.....<module>
 000005b0: 0300 0000 7306 0000 0010 0108 0108 03    ....s..........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0016_auto_20191021_0958.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0016_auto_20191021_0958.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 2205 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 9d08 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 9d08 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a03 4700 6403 6404 8400 6404 6501 6a04  Z.G.d.d...d.e.j.
 00000050: 8303 5a04 6402 5300 2905 e900 0000 0029  ..Z.d.S.)......)
 00000060: 01da 0a6d 6967 7261 7469 6f6e 734e 6300  ...migrationsNc.
 00000070: 0000 0000 0000 0000 0000 0000 0000 000e  ................
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0017_auto_20191021_1028.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0017_auto_20191021_1028.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1423 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 8f05 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 8f05 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0d00 0000 4000 0000 738e  ..........@...s.
@@ -12,42 +12,42 @@
 000000b0: 0064 038d 0265 046a 0564 0667 0064 038d  .d...e.j.d.g.d..
 000000c0: 0265 046a 0564 0767 0064 038d 0265 046a  .e.j.d.g.d...e.j
 000000d0: 0564 0867 0064 038d 0265 046a 0564 0967  .d.g.d...e.j.d.g
 000000e0: 0064 038d 0265 046a 0564 0a67 0064 038d  .d...e.j.d.g.d..
 000000f0: 0265 046a 0564 0b67 0064 038d 0265 046a  .e.j.d.g.d...e.j
 00000100: 0564 0c67 0064 038d 0267 0a5a 0664 0d53  .d.g.d...g.Z.d.S
 00000110: 0029 0eda 094d 6967 7261 7469 6f6e 2902  .)...Migration).
-00000120: da0a 646a 6175 746f 7461 736b 5a17 3030  ..djautotaskZ.00
+00000120: da0a 646a 6175 746f 7461 736b da17 3030  ..djautotask..00
 00000130: 3136 5f61 7574 6f5f 3230 3139 3130 3231  16_auto_20191021
 00000140: 5f30 3935 38da 0c64 6973 706c 6179 636f  _0958..displayco
 00000150: 6c6f 7229 02da 046e 616d 65da 086d 616e  lor)...name..man
 00000160: 6167 6572 73da 0969 7373 7565 7479 7065  agers..issuetype
 00000170: da0d 7072 6f6a 6563 7473 7461 7475 73da  ..projectstatus.
 00000180: 0b70 726f 6a65 6374 7479 7065 da05 7175  .projecttype..qu
 00000190: 6575 65da 0673 6f75 7263 65da 0c73 7562  eue..source..sub
-000001a0: 6973 7375 6574 7970 655a 0e74 6963 6b65  issuetypeZ.ticke
-000001b0: 7470 7269 6f72 6974 795a 0c74 6963 6b65  tpriorityZ.ticke
+000001a0: 6973 7375 6574 7970 65da 0e74 6963 6b65  issuetype..ticke
+000001b0: 7470 7269 6f72 6974 79da 0c74 6963 6b65  tpriority..ticke
 000001c0: 7473 7461 7475 73da 0a74 6963 6b65 7474  tstatus..tickett
 000001d0: 7970 654e 2907 da08 5f5f 6e61 6d65 5f5f  ypeN)...__name__
 000001e0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 000001f0: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
 00000200: 6e64 656e 6369 6573 7202 0000 00da 1241  ndenciesr......A
 00000210: 6c74 6572 4d6f 6465 6c4d 616e 6167 6572  lterModelManager
 00000220: 73da 0a6f 7065 7261 7469 6f6e 73a9 0072  s..operations..r
-00000230: 1500 0000 7215 0000 00fa 622f 686f 6d65  ....r.....b/home
+00000230: 1800 0000 7218 0000 00fa 622f 686f 6d65  ....r.....b/home
 00000240: 2f72 756e 6e65 722f 776f 726b 2f64 6a61  /runner/work/dja
 00000250: 6e67 6f2d 6175 746f 7461 736b 2f64 6a61  ngo-autotask/dja
 00000260: 6e67 6f2d 6175 746f 7461 736b 2f64 6a61  ngo-autotask/dja
 00000270: 7574 6f74 6173 6b2f 6d69 6772 6174 696f  utotask/migratio
 00000280: 6e73 2f30 3031 375f 6175 746f 5f32 3031  ns/0017_auto_201
 00000290: 3931 3032 315f 3130 3238 2e70 7972 0300  91021_1028.pyr..
 000002a0: 0000 0600 0000 7356 0000 0008 0302 ff04  ......sV........
 000002b0: 0504 0102 0102 fe04 0504 0102 0102 fe04  ................
 000002c0: 0504 0102 0102 fe04 0504 0102 0102 fe04  ................
 000002d0: 0504 0102 0102 fe04 0504 0102 0102 fe04  ................
 000002e0: 0504 0102 0102 fe04 0504 0102 0102 fe04  ................
 000002f0: 0504 0102 0102 fe04 0504 0102 0102 fe04  ................
 00000300: d272 0300 0000 4e29 03da 0964 6a61 6e67  .r....N)...djang
-00000310: 6f2e 6462 7202 0000 0072 0300 0000 7215  o.dbr....r....r.
-00000320: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00000310: 6f2e 6462 7202 0000 0072 0300 0000 7218  o.dbr....r....r.
+00000320: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
 00000330: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
 00000340: 7302 0000 000c 03                        s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0018_auto_20191029_1621.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0018_auto_20191029_1621.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1697 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 a106 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 a106 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0018_auto_20191029_1634.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0018_auto_20191029_1634.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1552 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 1006 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 1006 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0019_auto_20191030_0905.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0019_auto_20191030_0905.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 451 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 c301 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 c301 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a03 4700 6403 6404 8400 6404 6501 6a04  Z.G.d.d...d.e.j.
 00000050: 8303 5a04 6402 5300 2905 e900 0000 0029  ..Z.d.S.)......)
 00000060: 01da 0a6d 6967 7261 7469 6f6e 734e 6300  ...migrationsNc.
 00000070: 0000 0000 0000 0000 0000 0000 0000 0005  ................
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0020_auto_20191030_0916.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0020_auto_20191030_0916.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 346 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 5a01 0000  U.........KdZ...
+00000000: 550d 0d0a 0000 0000 3268 4c64 5a01 0000  U.......2hLdZ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0400 0000 4000 0000 7322  ..........@...s"
 00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
 00000090: 0365 046a 0564 0267 0064 038d 0267 015a  .e.j.d.g.d...g.Z
 000000a0: 0664 0453 0029 05da 094d 6967 7261 7469  .d.S.)...Migrati
 000000b0: 6f6e 2902 da0a 646a 6175 746f 7461 736b  on)...djautotask
-000000c0: 5a17 3030 3139 5f61 7574 6f5f 3230 3139  Z.0019_auto_2019
+000000c0: da17 3030 3139 5f61 7574 6f5f 3230 3139  ..0019_auto_2019
 000000d0: 3130 3330 5f30 3930 35da 0872 6573 6f75  1030_0905..resou
 000000e0: 7263 6529 02da 046e 616d 65da 086d 616e  rce)...name..man
 000000f0: 6167 6572 734e 2907 da08 5f5f 6e61 6d65  agersN)...__name
 00000100: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
 00000110: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
 00000120: 7065 6e64 656e 6369 6573 7202 0000 00da  pendenciesr.....
 00000130: 1241 6c74 6572 4d6f 6465 6c4d 616e 6167  .AlterModelManag
 00000140: 6572 73da 0a6f 7065 7261 7469 6f6e 73a9  ers..operations.
-00000150: 0072 0e00 0000 720e 0000 00fa 622f 686f  .r....r.....b/ho
+00000150: 0072 0f00 0000 720f 0000 00fa 622f 686f  .r....r.....b/ho
 00000160: 6d65 2f72 756e 6e65 722f 776f 726b 2f64  me/runner/work/d
 00000170: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
 00000180: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
 00000190: 6a61 7574 6f74 6173 6b2f 6d69 6772 6174  jautotask/migrat
 000001a0: 696f 6e73 2f30 3032 305f 6175 746f 5f32  ions/0020_auto_2
 000001b0: 3031 3931 3033 305f 3039 3136 2e70 7972  0191030_0916.pyr
 000001c0: 0300 0000 0600 0000 730e 0000 0008 0302  ........s.......
 000001d0: ff04 0504 0102 0102 fe04 ff72 0300 0000  ...........r....
 000001e0: 4e29 03da 0964 6a61 6e67 6f2e 6462 7202  N)...django.dbr.
-000001f0: 0000 0072 0300 0000 720e 0000 0072 0e00  ...r....r....r..
-00000200: 0000 720e 0000 0072 0f00 0000 da08 3c6d  ..r....r......<m
+000001f0: 0000 0072 0300 0000 720f 0000 0072 0f00  ...r....r....r..
+00000200: 0000 720f 0000 0072 1000 0000 da08 3c6d  ..r....r......<m
 00000210: 6f64 756c 653e 0300 0000 7302 0000 000c  odule>....s.....
 00000220: 03                                       .
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0023_auto_20191119_0923.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0079_auto_20201003_1125.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 401 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 9101 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 8701 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
 00000080: 0000 0600 0000 4000 0000 732c 0000 0065  ......@...s,...e
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
 000000a0: 0564 0264 0365 066a 0764 0464 058d 0164  .d.d.e.j.d.d...d
 000000b0: 068d 0367 015a 0864 0753 0029 08da 094d  ...g.Z.d.S.)...M
 000000c0: 6967 7261 7469 6f6e 2902 da0a 646a 6175  igration)...djau
-000000d0: 746f 7461 736b 5a18 3030 3232 5f6d 6572  totaskZ.0022_mer
-000000e0: 6765 5f32 3031 3931 3033 315f 3136 3230  ge_20191031_1620
-000000f0: da07 7072 6f6a 6563 74da 0864 7572 6174  ..project..durat
-00000100: 696f 6e72 0100 0000 2901 da07 6465 6661  ionr....)...defa
-00000110: 756c 7429 03da 0a6d 6f64 656c 5f6e 616d  ult)...model_nam
-00000120: 65da 046e 616d 65da 0566 6965 6c64 4e29  e..name..fieldN)
-00000130: 09da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000140: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000150: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
-00000160: 6965 7372 0200 0000 da0a 416c 7465 7246  iesr......AlterF
-00000170: 6965 6c64 7203 0000 00da 1450 6f73 6974  ieldr......Posit
-00000180: 6976 6549 6e74 6567 6572 4669 656c 64da  iveIntegerField.
-00000190: 0a6f 7065 7261 7469 6f6e 73a9 0072 1300  .operations..r..
-000001a0: 0000 7213 0000 00fa 622f 686f 6d65 2f72  ..r.....b/home/r
-000001b0: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
-000001c0: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
-000001d0: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
-000001e0: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
-000001f0: 2f30 3032 335f 6175 746f 5f32 3031 3931  /0023_auto_20191
-00000200: 3131 395f 3039 3233 2e70 7972 0400 0000  119_0923.pyr....
-00000210: 0600 0000 7310 0000 0008 0302 ff04 0504  ....s...........
-00000220: 0102 0102 010a fd04 ff72 0400 0000 4e29  .........r....N)
-00000230: 04da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
-00000240: 0072 0300 0000 7204 0000 0072 1300 0000  .r....r....r....
-00000250: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-00000260: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
-00000270: 0000 1003                                ....
+000000d0: 746f 7461 736b 5a18 3030 3738 5f6d 6572  totaskZ.0078_mer
+000000e0: 6765 5f32 3032 3031 3030 315f 3136 3537  ge_20201001_1657
+000000f0: 5a07 7379 6e63 6a6f 62da 0773 7563 6365  Z.syncjob..succe
+00000100: 7373 5429 01da 046e 756c 6c29 03da 0a6d  ssT)...null)...m
+00000110: 6f64 656c 5f6e 616d 65da 046e 616d 65da  odel_name..name.
+00000120: 0566 6965 6c64 4e29 09da 085f 5f6e 616d  .fieldN)...__nam
+00000130: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000140: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
+00000150: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
+00000160: da0a 416c 7465 7246 6965 6c64 7203 0000  ..AlterFieldr...
+00000170: 00da 0c42 6f6f 6c65 616e 4669 656c 64da  ...BooleanField.
+00000180: 0a6f 7065 7261 7469 6f6e 73a9 0072 1200  .operations..r..
+00000190: 0000 7212 0000 00fa 622f 686f 6d65 2f72  ..r.....b/home/r
+000001a0: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
+000001b0: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
+000001c0: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
+000001d0: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
+000001e0: 2f30 3037 395f 6175 746f 5f32 3032 3031  /0079_auto_20201
+000001f0: 3030 335f 3131 3235 2e70 7972 0400 0000  003_1125.pyr....
+00000200: 0600 0000 7310 0000 0008 0302 ff04 0504  ....s...........
+00000210: 0102 0102 010a fd04 ff72 0400 0000 4e29  .........r....N)
+00000220: 04da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
+00000230: 0072 0300 0000 7204 0000 0072 1200 0000  .r....r....r....
+00000240: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+00000250: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
+00000260: 0000 1003                                ....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0024_auto_20191122_1516.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0024_auto_20191122_1516.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 3582 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 fe0d 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 fe0d 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
@@ -72,15 +72,15 @@
 00000470: 7372 0100 0000 2901 da07 6465 6661 756c  sr....)...defaul
 00000480: 74da 0f72 656d 6169 6e69 6e67 5f68 6f75  t..remaining_hou
 00000490: 7273 da12 6c61 7374 5f61 6374 6976 6974  rs..last_activit
 000004a0: 795f 6461 7465 da11 6173 7369 676e 6564  y_date..assigned
 000004b0: 5f72 6573 6f75 7263 657a 1364 6a61 7574  _resourcez.djaut
 000004c0: 6f74 6173 6b2e 5265 736f 7572 6365 2903  otask.Resource).
 000004d0: 721e 0000 00da 096f 6e5f 6465 6c65 7465  r......on_delete
-000004e0: da02 746f 5a0e 7072 696f 7269 7479 5f6c  ..toZ.priority_l
+000004e0: da02 746f da0e 7072 696f 7269 7479 5f6c  ..to..priority_l
 000004f0: 6162 656c 7a19 646a 6175 746f 7461 736b  abelz.djautotask
 00000500: 2e54 6963 6b65 7450 7269 6f72 6974 79da  .TicketPriority.
 00000510: 0770 726f 6a65 6374 7a12 646a 6175 746f  .projectz.djauto
 00000520: 7461 736b 2e50 726f 6a65 6374 2902 7a09  task.Project).z.
 00000530: 2d6d 6f64 6966 6965 647a 082d 6372 6561  -modifiedz.-crea
 00000540: 7465 6429 03da 086f 7264 6572 696e 67da  ted)...ordering.
 00000550: 0d67 6574 5f6c 6174 6573 745f 6279 da08  .get_latest_by..
@@ -98,26 +98,26 @@
 00000610: da0c 5f5f 7175 616c 6e61 6d65 5f5f da06  ..__qualname__..
 00000620: 6174 6f6d 6963 da0c 6465 7065 6e64 656e  atomic..dependen
 00000630: 6369 6573 7202 0000 00da 0b52 656e 616d  ciesr......Renam
 00000640: 654d 6f64 656c da11 416c 7465 724d 6f64  eModel..AlterMod
 00000650: 656c 4f70 7469 6f6e 73da 0b43 7265 6174  elOptions..Creat
 00000660: 654d 6f64 656c 7203 0000 00da 0941 7574  eModelr......Aut
 00000670: 6f46 6965 6c64 da11 646a 616e 676f 5f65  oField..django_e
-00000680: 7874 656e 7369 6f6e 73da 0264 6272 3100  xtensions..dbr1.
+00000680: 7874 656e 7369 6f6e 73da 0264 6272 3200  xtensions..dbr2.
 00000690: 0000 da15 4372 6561 7469 6f6e 4461 7465  ....CreationDate
 000006a0: 5469 6d65 4669 656c 64da 194d 6f64 6966  TimeField..Modif
 000006b0: 6963 6174 696f 6e44 6174 6554 696d 6546  icationDateTimeF
 000006c0: 6965 6c64 da09 4368 6172 4669 656c 64da  ield..CharField.
 000006d0: 0d44 6174 6554 696d 6546 6965 6c64 da14  .DateTimeField..
 000006e0: 506f 7369 7469 7665 496e 7465 6765 7246  PositiveIntegerF
 000006f0: 6965 6c64 da0a 466f 7265 6967 6e4b 6579  ield..ForeignKey
 00000700: da06 646a 616e 676f da08 6465 6c65 7469  ..django..deleti
 00000710: 6f6e da08 5345 545f 4e55 4c4c da08 4164  on..SET_NULL..Ad
 00000720: 6446 6965 6c64 da0a 6f70 6572 6174 696f  dField..operatio
-00000730: 6e73 a900 724d 0000 0072 4d00 0000 fa62  ns..rM...rM....b
+00000730: 6e73 a900 724e 0000 0072 4e00 0000 fa62  ns..rN...rN....b
 00000740: 2f68 6f6d 652f 7275 6e6e 6572 2f77 6f72  /home/runner/wor
 00000750: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
 00000760: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
 00000770: 6b2f 646a 6175 746f 7461 736b 2f6d 6967  k/djautotask/mig
 00000780: 7261 7469 6f6e 732f 3030 3234 5f61 7574  rations/0024_aut
 00000790: 6f5f 3230 3139 3131 3232 5f31 3531 362e  o_20191122_1516.
 000007a0: 7079 7204 0000 0008 0000 0073 6c00 0000  pyr........sl...
@@ -127,13 +127,13 @@
 000007e0: 0e01 0e01 1001 1a01 1a01 1af0 0213 0201  ................
 000007f0: 0201 02fd 04ec 041a 0401 0202 1401 1401  ................
 00000800: 1401 1c01 1cfb 0208 0201 0201 02fd 04f7  ................
 00000810: 040f 0401 0201 0201 16fd 04ce 7204 0000  ............r...
 00000820: 0029 08da 0964 6a61 6e67 6f2e 6462 7202  .)...django.dbr.
 00000830: 0000 0072 0300 0000 da19 646a 616e 676f  ...r......django
 00000840: 2e64 622e 6d6f 6465 6c73 2e64 656c 6574  .db.models.delet
-00000850: 696f 6e72 4800 0000 da1b 646a 616e 676f  ionrH.....django
+00000850: 696f 6e72 4900 0000 da1b 646a 616e 676f  ionrI.....django
 00000860: 5f65 7874 656e 7369 6f6e 732e 6462 2e66  _extensions.db.f
-00000870: 6965 6c64 7372 4000 0000 7204 0000 0072  ieldsr@...r....r
-00000880: 4d00 0000 724d 0000 0072 4d00 0000 724e  M...rM...rM...rN
+00000870: 6965 6c64 7372 4100 0000 7204 0000 0072  ieldsrA...r....r
+00000880: 4e00 0000 724e 0000 0072 4e00 0000 724f  N...rN...rN...rO
 00000890: 0000 00da 083c 6d6f 6475 6c65 3e03 0000  .....<module>...
 000008a0: 0073 0600 0000 1001 0801 0803            .s..........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0025_auto_20191125_0939.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0026_auto_20191125_0952.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 362 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 6a01 0000  U.........Kdj...
+00000000: 550d 0d0a 0000 0000 3268 4c64 6e01 0000  U.......2hLdn...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0400 0000 4000 0000 7326  ..........@...s&
-00000080: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
-00000090: 0267 015a 0465 056a 0664 0364 0464 058d  .g.Z.e.j.d.d.d..
-000000a0: 0267 015a 0764 0653 0029 07da 094d 6967  .g.Z.d.S.)...Mig
-000000b0: 7261 7469 6f6e 4629 02da 0a64 6a61 7574  rationF)...djaut
-000000c0: 6f74 6173 6bda 1730 3032 345f 6175 746f  otask..0024_auto
-000000d0: 5f32 3031 3931 3132 325f 3135 3136 da0e  _20191122_1516..
-000000e0: 5469 636b 6574 5072 696f 7269 7479 da08  TicketPriority..
-000000f0: 5072 696f 7269 7479 2902 da08 6f6c 645f  Priority)...old_
-00000100: 6e61 6d65 da08 6e65 775f 6e61 6d65 4e29  name..new_nameN)
-00000110: 08da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000120: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000130: 616d 655f 5fda 0661 746f 6d69 63da 0c64  ame__..atomic..d
-00000140: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
-00000150: da0b 5265 6e61 6d65 4d6f 6465 6cda 0a6f  ..RenameModel..o
-00000160: 7065 7261 7469 6f6e 73a9 0072 1100 0000  perations..r....
-00000170: 7211 0000 00fa 622f 686f 6d65 2f72 756e  r.....b/home/run
-00000180: 6e65 722f 776f 726b 2f64 6a61 6e67 6f2d  ner/work/django-
-00000190: 6175 746f 7461 736b 2f64 6a61 6e67 6f2d  autotask/django-
-000001a0: 6175 746f 7461 736b 2f64 6a61 7574 6f74  autotask/djautot
-000001b0: 6173 6b2f 6d69 6772 6174 696f 6e73 2f30  ask/migrations/0
-000001c0: 3032 355f 6175 746f 5f32 3031 3931 3132  025_auto_2019112
-000001d0: 355f 3039 3339 2e70 7972 0300 0000 0600  5_0939.pyr......
-000001e0: 0000 7310 0000 0008 0104 0202 ff04 0504  ..s.............
-000001f0: 0102 0102 fe04 ff72 0300 0000 4e29 03da  .......r....N)..
-00000200: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
-00000210: 0300 0000 7211 0000 0072 1100 0000 7211  ....r....r....r.
-00000220: 0000 0072 1200 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000230: 653e 0300 0000 7302 0000 000c 03         e>....s......
+00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0264 0364 0469 0164 058d  .e.j.d.d.d.i.d..
+000000a0: 0267 015a 0664 0653 0029 07da 094d 6967  .g.Z.d.S.)...Mig
+000000b0: 7261 7469 6f6e 2902 da0a 646a 6175 746f  ration)...djauto
+000000c0: 7461 736b 5a17 3030 3235 5f61 7574 6f5f  taskZ.0025_auto_
+000000d0: 3230 3139 3131 3235 5f30 3933 39da 0870  20191125_0939..p
+000000e0: 7269 6f72 6974 79da 1376 6572 626f 7365  riority..verbose
+000000f0: 5f6e 616d 655f 706c 7572 616c da0a 5072  _name_plural..Pr
+00000100: 696f 7269 7469 6573 2902 da04 6e61 6d65  iorities)...name
+00000110: da07 6f70 7469 6f6e 734e 2907 da08 5f5f  ..optionsN)...__
+00000120: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000130: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000140: da0c 6465 7065 6e64 656e 6369 6573 7202  ..dependenciesr.
+00000150: 0000 00da 1141 6c74 6572 4d6f 6465 6c4f  .....AlterModelO
+00000160: 7074 696f 6e73 da0a 6f70 6572 6174 696f  ptions..operatio
+00000170: 6e73 a900 7210 0000 0072 1000 0000 fa62  ns..r....r.....b
+00000180: 2f68 6f6d 652f 7275 6e6e 6572 2f77 6f72  /home/runner/wor
+00000190: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
+000001a0: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
+000001b0: 6b2f 646a 6175 746f 7461 736b 2f6d 6967  k/djautotask/mig
+000001c0: 7261 7469 6f6e 732f 3030 3236 5f61 7574  rations/0026_aut
+000001d0: 6f5f 3230 3139 3131 3235 5f30 3935 322e  o_20191125_0952.
+000001e0: 7079 7203 0000 0006 0000 0073 0e00 0000  pyr........s....
+000001f0: 0803 02ff 0405 0401 0201 06fe 04ff 7203  ..............r.
+00000200: 0000 004e 2903 da09 646a 616e 676f 2e64  ...N)...django.d
+00000210: 6272 0200 0000 7203 0000 0072 1000 0000  br....r....r....
+00000220: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
+00000230: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
+00000240: 0000 0c03                                ....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0026_auto_20191125_0952.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0027_auto_20191125_1103.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 366 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 6e01 0000  U.........Kdn...
+00000000: 550d 0d0a 0000 0000 3268 4c64 7701 0000  U.......2hLdw...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
-00000070: 0000 0000 0000 0400 0000 4000 0000 7326  ..........@...s&
+00000070: 0000 0000 0000 0500 0000 4000 0000 7324  ..........@...s$
 00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
-00000090: 0365 046a 0564 0264 0364 0469 0164 058d  .e.j.d.d.d.i.d..
-000000a0: 0267 015a 0664 0653 0029 07da 094d 6967  .g.Z.d.S.)...Mig
-000000b0: 7261 7469 6f6e 2902 da0a 646a 6175 746f  ration)...djauto
-000000c0: 7461 736b 5a17 3030 3235 5f61 7574 6f5f  taskZ.0025_auto_
-000000d0: 3230 3139 3131 3235 5f30 3933 39da 0870  20191125_0939..p
-000000e0: 7269 6f72 6974 79da 1376 6572 626f 7365  riority..verbose
-000000f0: 5f6e 616d 655f 706c 7572 616c da0a 5072  _name_plural..Pr
-00000100: 696f 7269 7469 6573 2902 da04 6e61 6d65  iorities)...name
-00000110: da07 6f70 7469 6f6e 734e 2907 da08 5f5f  ..optionsN)...__
-00000120: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000130: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000140: da0c 6465 7065 6e64 656e 6369 6573 7202  ..dependenciesr.
-00000150: 0000 00da 1141 6c74 6572 4d6f 6465 6c4f  .....AlterModelO
-00000160: 7074 696f 6e73 da0a 6f70 6572 6174 696f  ptions..operatio
-00000170: 6e73 a900 7210 0000 0072 1000 0000 fa62  ns..r....r.....b
-00000180: 2f68 6f6d 652f 7275 6e6e 6572 2f77 6f72  /home/runner/wor
-00000190: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
-000001a0: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
-000001b0: 6b2f 646a 6175 746f 7461 736b 2f6d 6967  k/djautotask/mig
-000001c0: 7261 7469 6f6e 732f 3030 3236 5f61 7574  rations/0026_aut
-000001d0: 6f5f 3230 3139 3131 3235 5f30 3935 322e  o_20191125_0952.
-000001e0: 7079 7203 0000 0006 0000 0073 0e00 0000  pyr........s....
-000001f0: 0803 02ff 0405 0401 0201 06fe 04ff 7203  ..............r.
+00000090: 0365 046a 0564 0264 0364 0464 058d 0367  .e.j.d.d.d.d...g
+000000a0: 015a 0664 0653 0029 07da 094d 6967 7261  .Z.d.S.)...Migra
+000000b0: 7469 6f6e 2902 da0a 646a 6175 746f 7461  tion)...djautota
+000000c0: 736b 5a17 3030 3236 5f61 7574 6f5f 3230  skZ.0026_auto_20
+000000d0: 3139 3131 3235 5f30 3935 32da 0474 6173  191125_0952..tas
+000000e0: 6b5a 0e70 7269 6f72 6974 795f 6c61 6265  kZ.priority_labe
+000000f0: 6cda 0870 7269 6f72 6974 7929 03da 0a6d  l..priority)...m
+00000100: 6f64 656c 5f6e 616d 65da 086f 6c64 5f6e  odel_name..old_n
+00000110: 616d 65da 086e 6577 5f6e 616d 654e 2907  ame..new_nameN).
+00000120: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000130: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000140: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
+00000150: 6573 7202 0000 00da 0b52 656e 616d 6546  esr......RenameF
+00000160: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
+00000170: a900 7210 0000 0072 1000 0000 fa62 2f68  ..r....r.....b/h
+00000180: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
+00000190: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
+000001a0: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
+000001b0: 646a 6175 746f 7461 736b 2f6d 6967 7261  djautotask/migra
+000001c0: 7469 6f6e 732f 3030 3237 5f61 7574 6f5f  tions/0027_auto_
+000001d0: 3230 3139 3131 3235 5f31 3130 332e 7079  20191125_1103.py
+000001e0: 7203 0000 0006 0000 0073 1000 0000 0803  r........s......
+000001f0: 02ff 0405 0401 0201 0201 02fd 04ff 7203  ..............r.
 00000200: 0000 004e 2903 da09 646a 616e 676f 2e64  ...N)...django.d
 00000210: 6272 0200 0000 7203 0000 0072 1000 0000  br....r....r....
 00000220: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
 00000230: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
 00000240: 0000 0c03                                ....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0027_auto_20191125_1103.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0043_timeentry_allocation_code.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 375 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,48 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 7701 0000  U.........Kdw...
+00000000: 550d 0d0a 0000 0000 3268 4c64 0802 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
-00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
-00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
-00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
-00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
-00000070: 0000 0000 0000 0500 0000 4000 0000 7324  ..........@...s$
-00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
-00000090: 0365 046a 0564 0264 0364 0464 058d 0367  .e.j.d.d.d.d...g
-000000a0: 015a 0664 0653 0029 07da 094d 6967 7261  .Z.d.S.)...Migra
-000000b0: 7469 6f6e 2902 da0a 646a 6175 746f 7461  tion)...djautota
-000000c0: 736b da17 3030 3236 5f61 7574 6f5f 3230  sk..0026_auto_20
-000000d0: 3139 3131 3235 5f30 3935 32da 0474 6173  191125_0952..tas
-000000e0: 6bda 0e70 7269 6f72 6974 795f 6c61 6265  k..priority_labe
-000000f0: 6cda 0870 7269 6f72 6974 7929 03da 0a6d  l..priority)...m
-00000100: 6f64 656c 5f6e 616d 65da 086f 6c64 5f6e  odel_name..old_n
-00000110: 616d 65da 086e 6577 5f6e 616d 654e 2907  ame..new_nameN).
-00000120: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000130: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000140: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
-00000150: 6573 7202 0000 00da 0b52 656e 616d 6546  esr......RenameF
-00000160: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
-00000170: a900 7212 0000 0072 1200 0000 fa62 2f68  ..r....r.....b/h
-00000180: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
-00000190: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
-000001a0: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
-000001b0: 646a 6175 746f 7461 736b 2f6d 6967 7261  djautotask/migra
-000001c0: 7469 6f6e 732f 3030 3237 5f61 7574 6f5f  tions/0027_auto_
-000001d0: 3230 3139 3131 3235 5f31 3130 332e 7079  20191125_1103.py
-000001e0: 7203 0000 0006 0000 0073 1000 0000 0803  r........s......
-000001f0: 02ff 0405 0401 0201 0201 02fd 04ff 7203  ..............r.
-00000200: 0000 004e 2903 da09 646a 616e 676f 2e64  ...N)...django.d
-00000210: 6272 0200 0000 7203 0000 0072 1200 0000  br....r....r....
-00000220: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00000230: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
-00000240: 0000 0c03                                ....
+00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
+00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
+00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
+00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
+00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
+00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
+000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
+000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
+000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
+000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
+000000e0: 02da 0a64 6a61 7574 6f74 6173 6b5a 1730  ...djautotaskZ.0
+000000f0: 3034 325f 6175 746f 5f32 3032 3030 3230  042_auto_2020020
+00000100: 355f 3130 3537 5a09 7469 6d65 656e 7472  5_1057Z.timeentr
+00000110: 795a 0f61 6c6c 6f63 6174 696f 6e5f 636f  yZ.allocation_co
+00000120: 6465 547a 1964 6a61 7574 6f74 6173 6b2e  deTz.djautotask.
+00000130: 416c 6c6f 6361 7469 6f6e 436f 6465 2904  AllocationCode).
+00000140: da05 626c 616e 6bda 046e 756c 6cda 096f  ..blank..null..o
+00000150: 6e5f 6465 6c65 7465 da02 746f 2903 da0a  n_delete..to)...
+00000160: 6d6f 6465 6c5f 6e61 6d65 da04 6e61 6d65  model_name..name
+00000170: da05 6669 656c 644e 290d da08 5f5f 6e61  ..fieldN)...__na
+00000180: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000190: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
+000001a0: 6465 7065 6e64 656e 6369 6573 7202 0000  dependenciesr...
+000001b0: 00da 0841 6464 4669 656c 6472 0300 0000  ...AddFieldr....
+000001c0: da0a 466f 7265 6967 6e4b 6579 da06 646a  ..ForeignKey..dj
+000001d0: 616e 676f da02 6462 da08 6465 6c65 7469  ango..db..deleti
+000001e0: 6f6e da08 5345 545f 4e55 4c4c da0a 6f70  on..SET_NULL..op
+000001f0: 6572 6174 696f 6e73 a900 7218 0000 0072  erations..r....r
+00000200: 1800 0000 fa69 2f68 6f6d 652f 7275 6e6e  .....i/home/runn
+00000210: 6572 2f77 6f72 6b2f 646a 616e 676f 2d61  er/work/django-a
+00000220: 7574 6f74 6173 6b2f 646a 616e 676f 2d61  utotask/django-a
+00000230: 7574 6f74 6173 6b2f 646a 6175 746f 7461  utotask/djautota
+00000240: 736b 2f6d 6967 7261 7469 6f6e 732f 3030  sk/migrations/00
+00000250: 3433 5f74 696d 6565 6e74 7279 5f61 6c6c  43_timeentry_all
+00000260: 6f63 6174 696f 6e5f 636f 6465 2e70 7972  ocation_code.pyr
+00000270: 0400 0000 0700 0000 7310 0000 0008 0302  ........s.......
+00000280: ff04 0504 0102 0102 0118 fd04 ff72 0400  .............r..
+00000290: 0000 2906 da09 646a 616e 676f 2e64 6272  ..)...django.dbr
+000002a0: 0200 0000 7203 0000 00da 1964 6a61 6e67  ....r......djang
+000002b0: 6f2e 6462 2e6d 6f64 656c 732e 6465 6c65  o.db.models.dele
+000002c0: 7469 6f6e 7213 0000 0072 0400 0000 7218  tionr....r....r.
+000002d0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+000002e0: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
+000002f0: 7304 0000 0010 0108 03                   s........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0028_phase.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0028_phase.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1763 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 e306 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 e306 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0028_task_secondary_resources.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0028_task_secondary_resources.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 501 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 f501 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 f501 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
 00000080: 0000 0800 0000 4000 0000 7330 0000 0065  ......@...s0...e
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
 000000a0: 0564 0264 0365 066a 0764 0464 0564 0664  .d.d.e.j.d.d.d.d
 000000b0: 078d 0364 088d 0367 015a 0864 0953 0029  ...d...g.Z.d.S.)
 000000c0: 0ada 094d 6967 7261 7469 6f6e 2902 da0a  ...Migration)...
-000000d0: 646a 6175 746f 7461 736b 5a17 3030 3237  djautotaskZ.0027
+000000d0: 646a 6175 746f 7461 736b da17 3030 3237  djautotask..0027
 000000e0: 5f61 7574 6f5f 3230 3139 3131 3235 5f31  _auto_20191125_1
 000000f0: 3130 33da 0474 6173 6bda 1373 6563 6f6e  103..task..secon
 00000100: 6461 7279 5f72 6573 6f75 7263 6573 da18  dary_resources..
 00000110: 7365 636f 6e64 6172 795f 7265 736f 7572  secondary_resour
 00000120: 6365 5f74 6173 6b73 7a20 646a 6175 746f  ce_tasksz djauto
 00000130: 7461 736b 2e54 6173 6b53 6563 6f6e 6461  task.TaskSeconda
 00000140: 7279 5265 736f 7572 6365 7a13 646a 6175  ryResourcez.djau
@@ -26,21 +26,21 @@
 00000190: da05 6669 656c 644e 2909 da08 5f5f 6e61  ..fieldN)...__na
 000001a0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 000001b0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
 000001c0: 6465 7065 6e64 656e 6369 6573 7202 0000  dependenciesr...
 000001d0: 00da 0841 6464 4669 656c 6472 0300 0000  ...AddFieldr....
 000001e0: da0f 4d61 6e79 546f 4d61 6e79 4669 656c  ..ManyToManyFiel
 000001f0: 64da 0a6f 7065 7261 7469 6f6e 73a9 0072  d..operations..r
-00000200: 1600 0000 7216 0000 00fa 682f 686f 6d65  ....r.....h/home
+00000200: 1700 0000 7217 0000 00fa 682f 686f 6d65  ....r.....h/home
 00000210: 2f72 756e 6e65 722f 776f 726b 2f64 6a61  /runner/work/dja
 00000220: 6e67 6f2d 6175 746f 7461 736b 2f64 6a61  ngo-autotask/dja
 00000230: 6e67 6f2d 6175 746f 7461 736b 2f64 6a61  ngo-autotask/dja
 00000240: 7574 6f74 6173 6b2f 6d69 6772 6174 696f  utotask/migratio
 00000250: 6e73 2f30 3032 385f 7461 736b 5f73 6563  ns/0028_task_sec
 00000260: 6f6e 6461 7279 5f72 6573 6f75 7263 6573  ondary_resources
 00000270: 2e70 7972 0400 0000 0600 0000 7310 0000  .pyr........s...
 00000280: 0008 0302 ff04 0504 0102 0102 010e fd04  ................
 00000290: ff72 0400 0000 4e29 04da 0964 6a61 6e67  .r....N)...djang
 000002a0: 6f2e 6462 7202 0000 0072 0300 0000 7204  o.dbr....r....r.
-000002b0: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
-000002c0: 0000 7217 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000002b0: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
+000002c0: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
 000002d0: 3e03 0000 0073 0200 0000 1003            >....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0029_phase_last_activity_date.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0073_syncjob_skipped.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 398 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 8e01 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 9101 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00000080: 0000 0700 0000 4000 0000 732e 0000 0065  ......@...s....e
+00000080: 0000 0600 0000 4000 0000 732c 0000 0065  ......@...s,...e
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
-000000a0: 0564 0264 0365 066a 0764 0464 0464 058d  .d.d.e.j.d.d.d..
-000000b0: 0264 068d 0367 015a 0864 0753 0029 08da  .d...g.Z.d.S.)..
-000000c0: 094d 6967 7261 7469 6f6e 2902 da0a 646a  .Migration)...dj
-000000d0: 6175 746f 7461 736b 5a0a 3030 3238 5f70  autotaskZ.0028_p
-000000e0: 6861 7365 da05 7068 6173 65da 126c 6173  hase..phase..las
-000000f0: 745f 6163 7469 7669 7479 5f64 6174 6554  t_activity_dateT
-00000100: 2902 da05 626c 616e 6bda 046e 756c 6c29  )...blank..null)
-00000110: 03da 0a6d 6f64 656c 5f6e 616d 65da 046e  ...model_name..n
-00000120: 616d 65da 0566 6965 6c64 4e29 09da 085f  ame..fieldN)..._
-00000130: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000140: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000150: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
-00000160: 0200 0000 da08 4164 6446 6965 6c64 7203  ......AddFieldr.
-00000170: 0000 00da 0d44 6174 6554 696d 6546 6965  .....DateTimeFie
-00000180: 6c64 da0a 6f70 6572 6174 696f 6e73 a900  ld..operations..
-00000190: 7214 0000 0072 1400 0000 fa68 2f68 6f6d  r....r.....h/hom
-000001a0: 652f 7275 6e6e 6572 2f77 6f72 6b2f 646a  e/runner/work/dj
-000001b0: 616e 676f 2d61 7574 6f74 6173 6b2f 646a  ango-autotask/dj
-000001c0: 616e 676f 2d61 7574 6f74 6173 6b2f 646a  ango-autotask/dj
-000001d0: 6175 746f 7461 736b 2f6d 6967 7261 7469  autotask/migrati
-000001e0: 6f6e 732f 3030 3239 5f70 6861 7365 5f6c  ons/0029_phase_l
-000001f0: 6173 745f 6163 7469 7669 7479 5f64 6174  ast_activity_dat
-00000200: 652e 7079 7204 0000 0006 0000 0073 1000  e.pyr........s..
-00000210: 0000 0803 02ff 0405 0401 0201 0201 0cfd  ................
-00000220: 04ff 7204 0000 004e 2904 da09 646a 616e  ..r....N)...djan
-00000230: 676f 2e64 6272 0200 0000 7203 0000 0072  go.dbr....r....r
-00000240: 0400 0000 7214 0000 0072 1400 0000 7214  ....r....r....r.
-00000250: 0000 0072 1500 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000260: 653e 0300 0000 7302 0000 0010 03         e>....s......
+000000a0: 0564 0264 0365 066a 0764 0464 058d 0164  .d.d.e.j.d.d...d
+000000b0: 068d 0367 015a 0864 0753 0029 08da 094d  ...g.Z.d.S.)...M
+000000c0: 6967 7261 7469 6f6e 2902 da0a 646a 6175  igration)...djau
+000000d0: 746f 7461 736b da1b 3030 3732 5f61 6363  totask..0072_acc
+000000e0: 6f75 6e74 5f70 6172 656e 745f 6163 636f  ount_parent_acco
+000000f0: 756e 74da 0773 796e 636a 6f62 da07 736b  unt..syncjob..sk
+00000100: 6970 7065 6454 2901 da04 6e75 6c6c 2903  ippedT)...null).
+00000110: da0a 6d6f 6465 6c5f 6e61 6d65 da04 6e61  ..model_name..na
+00000120: 6d65 da05 6669 656c 644e 2909 da08 5f5f  me..fieldN)...__
+00000130: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000140: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000150: da0c 6465 7065 6e64 656e 6369 6573 7202  ..dependenciesr.
+00000160: 0000 00da 0841 6464 4669 656c 6472 0300  .....AddFieldr..
+00000170: 0000 da14 506f 7369 7469 7665 496e 7465  ....PositiveInte
+00000180: 6765 7246 6965 6c64 da0a 6f70 6572 6174  gerField..operat
+00000190: 696f 6e73 a900 7214 0000 0072 1400 0000  ions..r....r....
+000001a0: fa5f 2f68 6f6d 652f 7275 6e6e 6572 2f77  ._/home/runner/w
+000001b0: 6f72 6b2f 646a 616e 676f 2d61 7574 6f74  ork/django-autot
+000001c0: 6173 6b2f 646a 616e 676f 2d61 7574 6f74  ask/django-autot
+000001d0: 6173 6b2f 646a 6175 746f 7461 736b 2f6d  ask/djautotask/m
+000001e0: 6967 7261 7469 6f6e 732f 3030 3733 5f73  igrations/0073_s
+000001f0: 796e 636a 6f62 5f73 6b69 7070 6564 2e70  yncjob_skipped.p
+00000200: 7972 0400 0000 0600 0000 7310 0000 0008  yr........s.....
+00000210: 0302 ff04 0504 0102 0102 010a fd04 ff72  ...............r
+00000220: 0400 0000 4e29 04da 0964 6a61 6e67 6f2e  ....N)...django.
+00000230: 6462 7202 0000 0072 0300 0000 7204 0000  dbr....r....r...
+00000240: 0072 1400 0000 7214 0000 0072 1400 0000  .r....r....r....
+00000250: 7215 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
+00000260: 0000 0073 0200 0000 1003                 ...s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0030_task_phase.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0030_task_phase.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 490 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 ea01 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 ea01 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
 00000080: 0000 0000 0000 0000 0000 0008 0000 0040  ...............@
 00000090: 0000 0073 3800 0000 6500 5a01 6400 5a02  ...s8...e.Z.d.Z.
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6404 6508 6a09 6a06 6a0a 6a0b 6405  j.d.e.j.j.j.j.d.
 000000c0: 6406 8d03 6407 8d03 6701 5a0c 6408 5300  d...d...g.Z.d.S.
 000000d0: 2909 da09 4d69 6772 6174 696f 6e29 02da  )...Migration)..
-000000e0: 0a64 6a61 7574 6f74 6173 6bda 1d30 3032  .djautotask..002
+000000e0: 0a64 6a61 7574 6f74 6173 6b5a 1d30 3032  .djautotaskZ.002
 000000f0: 395f 7068 6173 655f 6c61 7374 5f61 6374  9_phase_last_act
 00000100: 6976 6974 795f 6461 7465 da04 7461 736b  ivity_date..task
 00000110: da05 7068 6173 6554 7a10 646a 6175 746f  ..phaseTz.djauto
 00000120: 7461 736b 2e50 6861 7365 2903 da04 6e75  task.Phase)...nu
 00000130: 6c6c da09 6f6e 5f64 656c 6574 65da 0274  ll..on_delete..t
 00000140: 6f29 03da 0a6d 6f64 656c 5f6e 616d 65da  o)...model_name.
 00000150: 046e 616d 65da 0566 6965 6c64 4e29 0dda  .name..fieldN)..
@@ -24,22 +24,22 @@
 00000170: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
 00000180: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
 00000190: 7372 0200 0000 da08 4164 6446 6965 6c64  sr......AddField
 000001a0: 7203 0000 00da 0a46 6f72 6569 676e 4b65  r......ForeignKe
 000001b0: 79da 0664 6a61 6e67 6fda 0264 62da 0864  y..django..db..d
 000001c0: 656c 6574 696f 6eda 0853 4554 5f4e 554c  eletion..SET_NUL
 000001d0: 4cda 0a6f 7065 7261 7469 6f6e 73a9 0072  L..operations..r
-000001e0: 1a00 0000 721a 0000 00fa 5a2f 686f 6d65  ....r.....Z/home
+000001e0: 1900 0000 7219 0000 00fa 5a2f 686f 6d65  ....r.....Z/home
 000001f0: 2f72 756e 6e65 722f 776f 726b 2f64 6a61  /runner/work/dja
 00000200: 6e67 6f2d 6175 746f 7461 736b 2f64 6a61  ngo-autotask/dja
 00000210: 6e67 6f2d 6175 746f 7461 736b 2f64 6a61  ngo-autotask/dja
 00000220: 7574 6f74 6173 6b2f 6d69 6772 6174 696f  utotask/migratio
 00000230: 6e73 2f30 3033 305f 7461 736b 5f70 6861  ns/0030_task_pha
 00000240: 7365 2e70 7972 0400 0000 0700 0000 7310  se.pyr........s.
 00000250: 0000 0008 0302 ff04 0504 0102 0102 0116  ................
 00000260: fd04 ff72 0400 0000 2906 da09 646a 616e  ...r....)...djan
 00000270: 676f 2e64 6272 0200 0000 7203 0000 00da  go.dbr....r.....
 00000280: 1964 6a61 6e67 6f2e 6462 2e6d 6f64 656c  .django.db.model
-00000290: 732e 6465 6c65 7469 6f6e 7215 0000 0072  s.deletionr....r
-000002a0: 0400 0000 721a 0000 0072 1a00 0000 721a  ....r....r....r.
-000002b0: 0000 0072 1b00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000290: 732e 6465 6c65 7469 6f6e 7214 0000 0072  s.deletionr....r
+000002a0: 0400 0000 7219 0000 0072 1900 0000 7219  ....r....r....r.
+000002b0: 0000 0072 1a00 0000 da08 3c6d 6f64 756c  ...r......<modul
 000002c0: 653e 0300 0000 7304 0000 0010 0108 03    e>....s........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0031_auto_20191129_1454.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0031_auto_20191129_1454.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1680 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 9006 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 9006 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0e00 0000 4000 0000 73ca  ..........@...s.
@@ -20,44 +20,44 @@
 00000130: 0264 058d 0265 046a 0564 1564 0364 0769  .d...e.j.d.d.d.i
 00000140: 0164 058d 0267 0b5a 0664 1653 0029 17da  .d...g.Z.d.S.)..
 00000150: 094d 6967 7261 7469 6f6e 2902 da0a 646a  .Migration)...dj
 00000160: 6175 746f 7461 736b 5a0f 3030 3330 5f74  autotaskZ.0030_t
 00000170: 6173 6b5f 7068 6173 65da 0761 6363 6f75  ask_phase..accou
 00000180: 6e74 da08 6f72 6465 7269 6e67 2901 da04  nt..ordering)...
 00000190: 6e61 6d65 2902 7207 0000 00da 076f 7074  name).r......opt
-000001a0: 696f 6e73 5a09 6973 7375 6574 7970 6529  ionsZ.issuetype)
-000001b0: 01da 056c 6162 656c 5a0b 6c69 6365 6e73  ...labelZ.licens
+000001a0: 696f 6e73 da09 6973 7375 6574 7970 6529  ions..issuetype)
+000001b0: 01da 056c 6162 656c da0b 6c69 6365 6e73  ...label..licens
 000001c0: 6574 7970 65da 0570 6861 7365 2901 da05  etype..phase)...
 000001d0: 7469 746c 65da 0870 7269 6f72 6974 7929  title..priority)
 000001e0: 01da 0a73 6f72 745f 6f72 6465 72da 0a50  ...sort_order..P
 000001f0: 7269 6f72 6974 6965 7329 0272 0600 0000  riorities).r....
 00000200: da13 7665 7262 6f73 655f 6e61 6d65 5f70  ..verbose_name_p
-00000210: 6c75 7261 6cda 0770 726f 6a65 6374 5a0b  lural..projectZ.
+00000210: 6c75 7261 6cda 0770 726f 6a65 6374 da0b  lural..project..
 00000220: 7072 6f6a 6563 7474 7970 65da 0673 6f75  projecttype..sou
-00000230: 7263 655a 0c73 7562 6973 7375 6574 7970  rceZ.subissuetyp
+00000230: 7263 65da 0c73 7562 6973 7375 6574 7970  rce..subissuetyp
 00000240: 655a 0e74 6963 6b65 7463 6174 6567 6f72  eZ.ticketcategor
 00000250: 797a 1154 6963 6b65 7420 6361 7465 676f  yz.Ticket catego
-00000260: 7269 6573 5a0a 7469 636b 6574 7479 7065  riesZ.tickettype
+00000260: 7269 6573 da0a 7469 636b 6574 7479 7065  ries..tickettype
 00000270: 4e29 07da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
 00000280: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 00000290: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
 000002a0: 6e63 6965 7372 0200 0000 da11 416c 7465  nciesr......Alte
 000002b0: 724d 6f64 656c 4f70 7469 6f6e 73da 0a6f  rModelOptions..o
-000002c0: 7065 7261 7469 6f6e 73a9 0072 1800 0000  perations..r....
-000002d0: 7218 0000 00fa 622f 686f 6d65 2f72 756e  r.....b/home/run
+000002c0: 7065 7261 7469 6f6e 73a9 0072 1d00 0000  perations..r....
+000002d0: 721d 0000 00fa 622f 686f 6d65 2f72 756e  r.....b/home/run
 000002e0: 6e65 722f 776f 726b 2f64 6a61 6e67 6f2d  ner/work/django-
 000002f0: 6175 746f 7461 736b 2f64 6a61 6e67 6f2d  autotask/django-
 00000300: 6175 746f 7461 736b 2f64 6a61 7574 6f74  autotask/djautot
 00000310: 6173 6b2f 6d69 6772 6174 696f 6e73 2f30  ask/migrations/0
 00000320: 3033 315f 6175 746f 5f32 3031 3931 3132  031_auto_2019112
 00000330: 395f 3134 3534 2e70 7972 0300 0000 0600  9_1454.pyr......
 00000340: 0000 735e 0000 0008 0302 ff04 0504 0102  ..s^............
 00000350: 0106 fe04 0404 0102 0106 fe04 0404 0102  ................
 00000360: 0106 fe04 0404 0102 0106 fe04 0404 0102  ................
 00000370: 0108 fe04 0404 0102 0106 fe04 0404 0102  ................
 00000380: 0106 fe04 0404 0102 0106 fe04 0404 0102  ................
 00000390: 0106 fe04 0404 0102 0108 fe04 0404 0102  ................
 000003a0: 0106 fe04 d772 0300 0000 4e29 03da 0964  .....r....N)...d
 000003b0: 6a61 6e67 6f2e 6462 7202 0000 0072 0300  jango.dbr....r..
-000003c0: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
-000003d0: 0072 1900 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000003c0: 0000 721d 0000 0072 1d00 0000 721d 0000  ..r....r....r...
+000003d0: 0072 1e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
 000003e0: 0300 0000 7302 0000 000c 03              ....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0032_auto_20191129_1501.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0032_auto_20191129_1501.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 881 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 7103 0000  U.........Kdq...
+00000000: 550d 0d0a 0000 0000 3268 4c64 7103 0000  U.......2hLdq...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0800 0000 4000 0000 735e  ..........@...s^
@@ -11,38 +11,38 @@
 000000a0: 068d 0265 046a 0564 0764 0364 0864 059c  ...e.j.d.d.d.d..
 000000b0: 0264 068d 0265 046a 0564 0964 0364 0a64  .d...e.j.d.d.d.d
 000000c0: 059c 0264 068d 0265 046a 0564 0b64 0364  ...d...e.j.d.d.d
 000000d0: 0c64 059c 0264 068d 0267 045a 0664 0d53  .d...d...g.Z.d.S
 000000e0: 0029 0eda 094d 6967 7261 7469 6f6e 2902  .)...Migration).
 000000f0: da0a 646a 6175 746f 7461 736b da17 3030  ..djautotask..00
 00000100: 3331 5f61 7574 6f5f 3230 3139 3131 3239  31_auto_20191129
-00000110: 5f31 3435 345a 0c64 6973 706c 6179 636f  _1454Z.displayco
+00000110: 5f31 3435 34da 0c64 6973 706c 6179 636f  _1454..displayco
 00000120: 6c6f 7229 01da 056c 6162 656c 7a0e 4469  lor)...labelz.Di
 00000130: 7370 6c61 7920 636f 6c6f 7273 2902 da08  splay colors)...
 00000140: 6f72 6465 7269 6e67 da13 7665 7262 6f73  ordering..verbos
 00000150: 655f 6e61 6d65 5f70 6c75 7261 6c29 02da  e_name_plural)..
-00000160: 046e 616d 65da 076f 7074 696f 6e73 5a0d  .name..optionsZ.
+00000160: 046e 616d 65da 076f 7074 696f 6e73 da0d  .name..options..
 00000170: 7072 6f6a 6563 7473 7461 7475 737a 1050  projectstatusz.P
 00000180: 726f 6a65 6374 2073 7461 7475 7365 73da  roject statuses.
 00000190: 0571 7565 7565 da06 5175 6575 6573 da06  .queue..Queues..
 000001a0: 7374 6174 7573 da08 5374 6174 7573 6573  status..Statuses
 000001b0: 4e29 07da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
 000001c0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 000001d0: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
 000001e0: 6e63 6965 7372 0200 0000 da11 416c 7465  nciesr......Alte
 000001f0: 724d 6f64 656c 4f70 7469 6f6e 73da 0a6f  rModelOptions..o
-00000200: 7065 7261 7469 6f6e 73a9 0072 1500 0000  perations..r....
-00000210: 7215 0000 00fa 622f 686f 6d65 2f72 756e  r.....b/home/run
+00000200: 7065 7261 7469 6f6e 73a9 0072 1700 0000  perations..r....
+00000210: 7217 0000 00fa 622f 686f 6d65 2f72 756e  r.....b/home/run
 00000220: 6e65 722f 776f 726b 2f64 6a61 6e67 6f2d  ner/work/django-
 00000230: 6175 746f 7461 736b 2f64 6a61 6e67 6f2d  autotask/django-
 00000240: 6175 746f 7461 736b 2f64 6a61 7574 6f74  autotask/djautot
 00000250: 6173 6b2f 6d69 6772 6174 696f 6e73 2f30  ask/migrations/0
 00000260: 3033 325f 6175 746f 5f32 3031 3931 3132  032_auto_2019112
 00000270: 395f 3135 3031 2e70 7972 0300 0000 0600  9_1501.pyr......
 00000280: 0000 7326 0000 0008 0302 ff04 0504 0102  ..s&............
 00000290: 0108 fe04 0404 0102 0108 fe04 0404 0102  ................
 000002a0: 0108 fe04 0404 0102 0108 fe04 f372 0300  .............r..
 000002b0: 0000 4e29 03da 0964 6a61 6e67 6f2e 6462  ..N)...django.db
-000002c0: 7202 0000 0072 0300 0000 7215 0000 0072  r....r....r....r
-000002d0: 1500 0000 7215 0000 0072 1600 0000 da08  ....r....r......
+000002c0: 7202 0000 0072 0300 0000 7217 0000 0072  r....r....r....r
+000002d0: 1700 0000 7217 0000 0072 1800 0000 da08  ....r....r......
 000002e0: 3c6d 6f64 756c 653e 0300 0000 7302 0000  <module>....s...
 000002f0: 000c 03                                  ...
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0034_auto_20191210_1518.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0112_account_owner_resource.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 505 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 f901 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 0702 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
 00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
 00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
 000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
 000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
-000000e0: 02da 0a64 6a61 7574 6f74 6173 6bda 1830  ...djautotask..0
-000000f0: 3033 335f 6d65 7267 655f 3230 3139 3132  033_merge_201912
-00000100: 3034 5f31 3032 32da 0474 6173 6bda 0870  04_1022..task..p
-00000110: 7269 6f72 6974 7954 7a13 646a 6175 746f  riorityTz.djauto
-00000120: 7461 736b 2e50 7269 6f72 6974 7929 04da  task.Priority)..
-00000130: 0562 6c61 6e6b da04 6e75 6c6c da09 6f6e  .blank..null..on
-00000140: 5f64 656c 6574 65da 0274 6f29 03da 0a6d  _delete..to)...m
-00000150: 6f64 656c 5f6e 616d 65da 046e 616d 65da  odel_name..name.
-00000160: 0566 6965 6c64 4e29 0dda 085f 5f6e 616d  .fieldN)...__nam
-00000170: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000180: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
-00000190: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
-000001a0: da0a 416c 7465 7246 6965 6c64 7203 0000  ..AlterFieldr...
-000001b0: 00da 0a46 6f72 6569 676e 4b65 79da 0664  ...ForeignKey..d
-000001c0: 6a61 6e67 6fda 0264 62da 0864 656c 6574  jango..db..delet
-000001d0: 696f 6eda 0853 4554 5f4e 554c 4cda 0a6f  ion..SET_NULL..o
-000001e0: 7065 7261 7469 6f6e 73a9 0072 1b00 0000  perations..r....
-000001f0: 721b 0000 00fa 622f 686f 6d65 2f72 756e  r.....b/home/run
-00000200: 6e65 722f 776f 726b 2f64 6a61 6e67 6f2d  ner/work/django-
-00000210: 6175 746f 7461 736b 2f64 6a61 6e67 6f2d  autotask/django-
-00000220: 6175 746f 7461 736b 2f64 6a61 7574 6f74  autotask/djautot
-00000230: 6173 6b2f 6d69 6772 6174 696f 6e73 2f30  ask/migrations/0
-00000240: 3033 345f 6175 746f 5f32 3031 3931 3231  034_auto_2019121
-00000250: 305f 3135 3138 2e70 7972 0400 0000 0700  0_1518.pyr......
-00000260: 0000 7310 0000 0008 0302 ff04 0504 0102  ..s.............
-00000270: 0102 0118 fd04 ff72 0400 0000 2906 da09  .......r....)...
-00000280: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
-00000290: 0000 00da 1964 6a61 6e67 6f2e 6462 2e6d  .....django.db.m
-000002a0: 6f64 656c 732e 6465 6c65 7469 6f6e 7216  odels.deletionr.
-000002b0: 0000 0072 0400 0000 721b 0000 0072 1b00  ...r....r....r..
-000002c0: 0000 721b 0000 0072 1c00 0000 da08 3c6d  ..r....r......<m
-000002d0: 6f64 756c 653e 0300 0000 7304 0000 0010  odule>....s.....
-000002e0: 0108 03                                  ...
+000000e0: 02da 0a64 6a61 7574 6f74 6173 6bda 2030  ...djautotask. 0
+000000f0: 3131 315f 616c 7465 725f 7068 6173 655f  111_alter_phase_
+00000100: 6573 7469 6d61 7465 645f 686f 7572 73da  estimated_hours.
+00000110: 0761 6363 6f75 6e74 da0e 6f77 6e65 725f  .account..owner_
+00000120: 7265 736f 7572 6365 547a 1364 6a61 7574  resourceTz.djaut
+00000130: 6f74 6173 6b2e 7265 736f 7572 6365 2904  otask.resource).
+00000140: da05 626c 616e 6bda 046e 756c 6cda 096f  ..blank..null..o
+00000150: 6e5f 6465 6c65 7465 da02 746f 2903 da0a  n_delete..to)...
+00000160: 6d6f 6465 6c5f 6e61 6d65 da04 6e61 6d65  model_name..name
+00000170: da05 6669 656c 644e 290d da08 5f5f 6e61  ..fieldN)...__na
+00000180: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000190: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
+000001a0: 6465 7065 6e64 656e 6369 6573 7202 0000  dependenciesr...
+000001b0: 00da 0841 6464 4669 656c 6472 0300 0000  ...AddFieldr....
+000001c0: da0a 466f 7265 6967 6e4b 6579 da06 646a  ..ForeignKey..dj
+000001d0: 616e 676f da02 6462 da08 6465 6c65 7469  ango..db..deleti
+000001e0: 6f6e da08 5345 545f 4e55 4c4c da0a 6f70  on..SET_NULL..op
+000001f0: 6572 6174 696f 6e73 a900 721b 0000 0072  erations..r....r
+00000200: 1b00 0000 fa66 2f68 6f6d 652f 7275 6e6e  .....f/home/runn
+00000210: 6572 2f77 6f72 6b2f 646a 616e 676f 2d61  er/work/django-a
+00000220: 7574 6f74 6173 6b2f 646a 616e 676f 2d61  utotask/django-a
+00000230: 7574 6f74 6173 6b2f 646a 6175 746f 7461  utotask/djautota
+00000240: 736b 2f6d 6967 7261 7469 6f6e 732f 3031  sk/migrations/01
+00000250: 3132 5f61 6363 6f75 6e74 5f6f 776e 6572  12_account_owner
+00000260: 5f72 6573 6f75 7263 652e 7079 7204 0000  _resource.pyr...
+00000270: 0007 0000 0073 1000 0000 0803 02ff 0405  .....s..........
+00000280: 0401 0201 0201 18fd 04ff 7204 0000 0029  ..........r....)
+00000290: 06da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
+000002a0: 0072 0300 0000 da19 646a 616e 676f 2e64  .r......django.d
+000002b0: 622e 6d6f 6465 6c73 2e64 656c 6574 696f  b.models.deletio
+000002c0: 6e72 1600 0000 7204 0000 0072 1b00 0000  nr....r....r....
+000002d0: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+000002e0: 083c 6d6f 6475 6c65 3e03 0000 0073 0400  .<module>....s..
+000002f0: 0000 1001 0803                           ......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0035_timeentry.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0035_timeentry.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 2114 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 4208 0000  U.........KdB...
+00000000: 550d 0d0a 0000 0000 3268 4c64 4208 0000  U.......2hLdB...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0036_auto_20200127_1157.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0036_auto_20200127_1157.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1456 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 b005 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 b005 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0e00 0000 4000 0000 739a  ..........@...s.
@@ -14,41 +14,41 @@
 000000d0: 0564 0964 0364 048d 0265 046a 0564 0a64  .d.d.d...e.j.d.d
 000000e0: 0364 048d 0265 046a 0564 0b64 0364 048d  .d...e.j.d.d.d..
 000000f0: 0265 046a 0564 0c64 0364 048d 0265 046a  .e.j.d.d.d...e.j
 00000100: 0564 0d64 0364 048d 0265 046a 0564 0e64  .d.d.d...e.j.d.d
 00000110: 0364 048d 0267 0b5a 0664 0f53 0029 10da  .d...g.Z.d.S.)..
 00000120: 094d 6967 7261 7469 6f6e 2902 da0a 646a  .Migration)...dj
 00000130: 6175 746f 7461 736b 5a0e 3030 3335 5f74  autotaskZ.0035_t
-00000140: 696d 6565 6e74 7279 da0c 6469 7370 6c61  imeentry..displa
+00000140: 696d 6565 6e74 7279 5a0c 6469 7370 6c61  imeentryZ.displa
 00000150: 7963 6f6c 6f72 da0c 7061 7265 6e74 5f76  ycolor..parent_v
 00000160: 616c 7565 2902 da0a 6d6f 6465 6c5f 6e61  alue)...model_na
-00000170: 6d65 da04 6e61 6d65 da09 6973 7375 6574  me..name..issuet
-00000180: 7970 65da 0b6c 6963 656e 7365 7479 7065  ype..licensetype
-00000190: da08 7072 696f 7269 7479 da0d 7072 6f6a  ..priority..proj
-000001a0: 6563 7473 7461 7475 73da 0b70 726f 6a65  ectstatus..proje
+00000170: 6d65 da04 6e61 6d65 5a09 6973 7375 6574  me..nameZ.issuet
+00000180: 7970 655a 0b6c 6963 656e 7365 7479 7065  ypeZ.licensetype
+00000190: da08 7072 696f 7269 7479 5a0d 7072 6f6a  ..priorityZ.proj
+000001a0: 6563 7473 7461 7475 735a 0b70 726f 6a65  ectstatusZ.proje
 000001b0: 6374 7479 7065 da05 7175 6575 65da 0673  cttype..queue..s
-000001c0: 6f75 7263 65da 0673 7461 7475 73da 0c73  ource..status..s
-000001d0: 7562 6973 7375 6574 7970 65da 0a74 6963  ubissuetype..tic
+000001c0: 6f75 7263 65da 0673 7461 7475 735a 0c73  ource..statusZ.s
+000001d0: 7562 6973 7375 6574 7970 655a 0a74 6963  ubissuetypeZ.tic
 000001e0: 6b65 7474 7970 654e 2907 da08 5f5f 6e61  kettypeN)...__na
 000001f0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 00000200: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
 00000210: 6465 7065 6e64 656e 6369 6573 7202 0000  dependenciesr...
 00000220: 00da 0b52 656d 6f76 6546 6965 6c64 da0a  ...RemoveField..
-00000230: 6f70 6572 6174 696f 6e73 a900 7219 0000  operations..r...
-00000240: 0072 1900 0000 fa62 2f68 6f6d 652f 7275  .r.....b/home/ru
+00000230: 6f70 6572 6174 696f 6e73 a900 7212 0000  operations..r...
+00000240: 0072 1200 0000 fa62 2f68 6f6d 652f 7275  .r.....b/home/ru
 00000250: 6e6e 6572 2f77 6f72 6b2f 646a 616e 676f  nner/work/django
 00000260: 2d61 7574 6f74 6173 6b2f 646a 616e 676f  -autotask/django
 00000270: 2d61 7574 6f74 6173 6b2f 646a 6175 746f  -autotask/djauto
 00000280: 7461 736b 2f6d 6967 7261 7469 6f6e 732f  task/migrations/
 00000290: 3030 3336 5f61 7574 6f5f 3230 3230 3031  0036_auto_202001
 000002a0: 3237 5f31 3135 372e 7079 7203 0000 0006  27_1157.pyr.....
 000002b0: 0000 0073 5e00 0000 0803 02ff 0405 0401  ...s^...........
 000002c0: 0201 02fe 0404 0401 0201 02fe 0404 0401  ................
 000002d0: 0201 02fe 0404 0401 0201 02fe 0404 0401  ................
 000002e0: 0201 02fe 0404 0401 0201 02fe 0404 0401  ................
 000002f0: 0201 02fe 0404 0401 0201 02fe 0404 0401  ................
 00000300: 0201 02fe 0404 0401 0201 02fe 0404 0401  ................
 00000310: 0201 02fe 04d7 7203 0000 004e 2903 da09  ......r....N)...
 00000320: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
-00000330: 0000 0072 1900 0000 7219 0000 0072 1900  ...r....r....r..
-00000340: 0000 721a 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000330: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
+00000340: 0000 7213 0000 00da 083c 6d6f 6475 6c65  ..r......<module
 00000350: 3e03 0000 0073 0200 0000 0c03            >....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0037_subissuetype_parent_value.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0037_subissuetype_parent_value.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 514 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 0202 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 0202 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
 00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
 00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
 000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
 000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
-000000e0: 02da 0a64 6a61 7574 6f74 6173 6b5a 1730  ...djautotaskZ.0
+000000e0: 02da 0a64 6a61 7574 6f74 6173 6bda 1730  ...djautotask..0
 000000f0: 3033 365f 6175 746f 5f32 3032 3030 3132  036_auto_2020012
 00000100: 375f 3131 3537 da0c 7375 6269 7373 7565  7_1157..subissue
 00000110: 7479 7065 da0c 7061 7265 6e74 5f76 616c  type..parent_val
 00000120: 7565 547a 1464 6a61 7574 6f74 6173 6b2e  ueTz.djautotask.
 00000130: 4973 7375 6554 7970 6529 04da 0562 6c61  IssueType)...bla
 00000140: 6e6b da04 6e75 6c6c da09 6f6e 5f64 656c  nk..null..on_del
 00000150: 6574 65da 0274 6f29 03da 0a6d 6f64 656c  ete..to)...model
@@ -25,24 +25,24 @@
 00000180: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
 00000190: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
 000001a0: 6465 6e63 6965 7372 0200 0000 da08 4164  denciesr......Ad
 000001b0: 6446 6965 6c64 7203 0000 00da 0a46 6f72  dFieldr......For
 000001c0: 6569 676e 4b65 79da 0664 6a61 6e67 6fda  eignKey..django.
 000001d0: 0264 62da 0864 656c 6574 696f 6eda 0743  .db..deletion..C
 000001e0: 4153 4341 4445 da0a 6f70 6572 6174 696f  ASCADE..operatio
-000001f0: 6e73 a900 721a 0000 0072 1a00 0000 fa69  ns..r....r.....i
+000001f0: 6e73 a900 721b 0000 0072 1b00 0000 fa69  ns..r....r.....i
 00000200: 2f68 6f6d 652f 7275 6e6e 6572 2f77 6f72  /home/runner/wor
 00000210: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
 00000220: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
 00000230: 6b2f 646a 6175 746f 7461 736b 2f6d 6967  k/djautotask/mig
 00000240: 7261 7469 6f6e 732f 3030 3337 5f73 7562  rations/0037_sub
 00000250: 6973 7375 6574 7970 655f 7061 7265 6e74  issuetype_parent
 00000260: 5f76 616c 7565 2e70 7972 0400 0000 0700  _value.pyr......
 00000270: 0000 7310 0000 0008 0302 ff04 0504 0102  ..s.............
 00000280: 0102 0118 fd04 ff72 0400 0000 2906 da09  .......r....)...
 00000290: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
 000002a0: 0000 00da 1964 6a61 6e67 6f2e 6462 2e6d  .....django.db.m
-000002b0: 6f64 656c 732e 6465 6c65 7469 6f6e 7215  odels.deletionr.
-000002c0: 0000 0072 0400 0000 721a 0000 0072 1a00  ...r....r....r..
-000002d0: 0000 721a 0000 0072 1b00 0000 da08 3c6d  ..r....r......<m
+000002b0: 6f64 656c 732e 6465 6c65 7469 6f6e 7216  odels.deletionr.
+000002c0: 0000 0072 0400 0000 721b 0000 0072 1b00  ...r....r....r..
+000002d0: 0000 721b 0000 0072 1c00 0000 da08 3c6d  ..r....r......<m
 000002e0: 6f64 756c 653e 0300 0000 7304 0000 0010  odule>....s.....
 000002f0: 0108 03                                  ...
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0038_auto_20200130_1218.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0038_auto_20200130_1218.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 416 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 a001 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 a001 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0500 0000 4000 0000 7328  ..........@...s(
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0038_notetype_tasknote_ticketnote.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0038_notetype_tasknote_ticketnote.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 4027 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 bb0f 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 bb0f 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0039_auto_20200131_1134.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0039_auto_20200131_1134.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1519 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 ef05 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 ef05 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0039_merge_20200131_1022.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0039_merge_20200131_1022.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 290 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 2201 0000  U.........Kd"...
+00000000: 550d 0d0a 0000 0000 3268 4c64 2201 0000  U.......2hLd"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0200 0000 4000 0000 7318  ..........@...s.
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0040_auto_20200204_1538.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0048_auto_20200211_1037.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 644 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 8402 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 5503 0000  U.......2hLdU...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00000080: 0000 0a00 0000 4000 0000 734e 0000 0065  ......@...sN...e
+00000080: 0000 0b00 0000 4000 0000 736a 0000 0065  ......@...sj...e
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
 000000a0: 0564 0264 0365 066a 0764 0464 0564 0664  .d.d.e.j.d.d.d.d
 000000b0: 0464 078d 0464 088d 0365 046a 0564 0264  .d...d...e.j.d.d
 000000c0: 0965 066a 0764 0464 0564 0664 0464 078d  .e.j.d.d.d.d.d..
-000000d0: 0464 088d 0367 025a 0864 0a53 0029 0bda  .d...g.Z.d.S.)..
-000000e0: 094d 6967 7261 7469 6f6e 2902 da0a 646a  .Migration)...dj
-000000f0: 6175 746f 7461 736b da18 3030 3339 5f6d  autotask..0039_m
-00000100: 6572 6765 5f32 3032 3030 3133 315f 3130  erge_20200131_10
-00000110: 3232 da04 7461 736b da0f 6573 7469 6d61  22..task..estima
-00000120: 7465 645f 686f 7572 7354 e902 0000 00e9  ted_hoursT......
-00000130: 0600 0000 2904 da05 626c 616e 6bda 0e64  ....)...blank..d
-00000140: 6563 696d 616c 5f70 6c61 6365 73da 0a6d  ecimal_places..m
-00000150: 6178 5f64 6967 6974 73da 046e 756c 6c29  ax_digits..null)
-00000160: 03da 0a6d 6f64 656c 5f6e 616d 65da 046e  ...model_name..n
-00000170: 616d 65da 0566 6965 6c64 da0f 7265 6d61  ame..field..rema
-00000180: 696e 696e 675f 686f 7572 734e 2909 da08  ining_hoursN)...
-00000190: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000001a0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000001b0: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
-000001c0: 7202 0000 00da 0a41 6c74 6572 4669 656c  r......AlterFiel
-000001d0: 6472 0300 0000 da0c 4465 6369 6d61 6c46  dr......DecimalF
-000001e0: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
-000001f0: a900 721a 0000 0072 1a00 0000 fa62 2f68  ..r....r.....b/h
-00000200: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
-00000210: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
-00000220: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
-00000230: 646a 6175 746f 7461 736b 2f6d 6967 7261  djautotask/migra
-00000240: 7469 6f6e 732f 3030 3430 5f61 7574 6f5f  tions/0040_auto_
-00000250: 3230 3230 3032 3034 5f31 3533 382e 7079  20200204_1538.py
-00000260: 7204 0000 0006 0000 0073 1a00 0000 0803  r........s......
-00000270: 02ff 0405 0401 0201 0201 10fd 0405 0401  ................
-00000280: 0201 0201 10fd 04fa 7204 0000 004e 2904  ........r....N).
-00000290: da09 646a 616e 676f 2e64 6272 0200 0000  ..django.dbr....
-000002a0: 7203 0000 0072 0400 0000 721a 0000 0072  r....r....r....r
-000002b0: 1a00 0000 721a 0000 0072 1b00 0000 da08  ....r....r......
-000002c0: 3c6d 6f64 756c 653e 0300 0000 7302 0000  <module>....s...
-000002d0: 0010 03                                  ...
+000000d0: 0464 088d 0365 046a 0564 0264 0a65 066a  .d...e.j.d.d.e.j
+000000e0: 0764 0464 0564 0664 0464 078d 0464 088d  .d.d.d.d.d...d..
+000000f0: 0367 035a 0864 0b53 0029 0cda 094d 6967  .g.Z.d.S.)...Mig
+00000100: 7261 7469 6f6e 2902 da0a 646a 6175 746f  ration)...djauto
+00000110: 7461 736b 5a17 3030 3437 5f61 7574 6f5f  taskZ.0047_auto_
+00000120: 3230 3230 3032 3037 5f31 3132 36da 0974  20200207_1126..t
+00000130: 696d 6565 6e74 7279 da0d 686f 7572 735f  imeentry..hours_
+00000140: 746f 5f62 696c 6c54 e904 0000 00e9 0900  to_billT........
+00000150: 0000 2904 da05 626c 616e 6bda 0e64 6563  ..)...blank..dec
+00000160: 696d 616c 5f70 6c61 6365 73da 0a6d 6178  imal_places..max
+00000170: 5f64 6967 6974 73da 046e 756c 6c29 03da  _digits..null)..
+00000180: 0a6d 6f64 656c 5f6e 616d 65da 046e 616d  .model_name..nam
+00000190: 65da 0566 6965 6c64 da0c 686f 7572 735f  e..field..hours_
+000001a0: 776f 726b 6564 da0c 6f66 6673 6574 5f68  worked..offset_h
+000001b0: 6f75 7273 4e29 09da 085f 5f6e 616d 655f  oursN)...__name_
+000001c0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+000001d0: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
+000001e0: 656e 6465 6e63 6965 7372 0200 0000 da0a  endenciesr......
+000001f0: 416c 7465 7246 6965 6c64 7203 0000 00da  AlterFieldr.....
+00000200: 0c44 6563 696d 616c 4669 656c 64da 0a6f  .DecimalField..o
+00000210: 7065 7261 7469 6f6e 73a9 0072 1a00 0000  perations..r....
+00000220: 721a 0000 00fa 622f 686f 6d65 2f72 756e  r.....b/home/run
+00000230: 6e65 722f 776f 726b 2f64 6a61 6e67 6f2d  ner/work/django-
+00000240: 6175 746f 7461 736b 2f64 6a61 6e67 6f2d  autotask/django-
+00000250: 6175 746f 7461 736b 2f64 6a61 7574 6f74  autotask/djautot
+00000260: 6173 6b2f 6d69 6772 6174 696f 6e73 2f30  ask/migrations/0
+00000270: 3034 385f 6175 746f 5f32 3032 3030 3231  048_auto_2020021
+00000280: 315f 3130 3337 2e70 7972 0400 0000 0600  1_1037.pyr......
+00000290: 0000 7324 0000 0008 0302 ff04 0504 0102  ..s$............
+000002a0: 0102 0110 fd04 0504 0102 0102 0110 fd04  ................
+000002b0: 0504 0102 0102 0110 fd04 f572 0400 0000  ...........r....
+000002c0: 4e29 04da 0964 6a61 6e67 6f2e 6462 7202  N)...django.dbr.
+000002d0: 0000 0072 0300 0000 7204 0000 0072 1a00  ...r....r....r..
+000002e0: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+000002f0: 00da 083c 6d6f 6475 6c65 3e03 0000 0073  ...<module>....s
+00000300: 0200 0000 1003                           ......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0042_auto_20200205_1057.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0042_auto_20200205_1057.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 2395 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 5b09 0000  U.........Kd[...
+00000000: 550d 0d0a 0000 0000 3268 4c64 5b09 0000  U.......2hLd[...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
@@ -28,79 +28,79 @@
 000001b0: 6602 641d 6506 6a0e 6405 6412 8d01 6602  f.d.e.j.d.d...f.
 000001c0: 6708 641e 6405 641f 9c02 6415 8d03 6504  g.d.d.d...d...e.
 000001d0: 6a10 6420 6421 6506 6a11 6404 6404 6512  j.d d!e.j.d.d.e.
 000001e0: 6a09 6a06 6a13 6a14 6422 6423 8d04 6424  j.j.j.j.d"d#..d$
 000001f0: 8d03 6703 5a15 6425 5300 2926 da09 4d69  ..g.Z.d%S.)&..Mi
 00000200: 6772 6174 696f 6e29 02da 0a64 6a61 7574  gration)...djaut
 00000210: 6f74 6173 6bda 1830 3034 315f 6d65 7267  otask..0041_merg
-00000220: 655f 3230 3230 3032 3034 5f31 3534 36da  e_20200204_1546.
+00000220: 655f 3230 3230 3032 3034 5f31 3534 365a  e_20200204_1546Z
 00000230: 0e41 6c6c 6f63 6174 696f 6e43 6f64 65da  .AllocationCode.
 00000240: 0269 6454 46da 0249 4429 04da 0c61 7574  .idTF..ID)...aut
 00000250: 6f5f 6372 6561 7465 64da 0b70 7269 6d61  o_created..prima
 00000260: 7279 5f6b 6579 da09 7365 7269 616c 697a  ry_key..serializ
 00000270: 65da 0c76 6572 626f 7365 5f6e 616d 65da  e..verbose_name.
 00000280: 0763 7265 6174 6564 2902 da0c 6175 746f  .created)...auto
-00000290: 5f6e 6f77 5f61 6464 720d 0000 00da 086d  _now_addr......m
+00000290: 5f6e 6f77 5f61 6464 720c 0000 00da 086d  _now_addr......m
 000002a0: 6f64 6966 6965 6429 02da 0861 7574 6f5f  odified)...auto_
-000002b0: 6e6f 7772 0d00 0000 da04 6e61 6d65 e9c8  nowr......name..
+000002b0: 6e6f 7772 0c00 0000 da04 6e61 6d65 e9c8  nowr......name..
 000002c0: 0000 0029 03da 0562 6c61 6e6b da0a 6d61  ...)...blank..ma
 000002d0: 785f 6c65 6e67 7468 da04 6e75 6c6c da0b  x_length..null..
 000002e0: 6465 7363 7269 7074 696f 6e69 f401 0000  descriptioni....
 000002f0: da06 6163 7469 7665 2901 da07 6465 6661  ..active)...defa
 00000300: 756c 7429 027a 092d 6d6f 6469 6669 6564  ult).z.-modified
 00000310: 7a08 2d63 7265 6174 6564 2903 da08 6f72  z.-created)...or
 00000320: 6465 7269 6e67 da0d 6765 745f 6c61 7465  dering..get_late
 00000330: 7374 5f62 79da 0861 6273 7472 6163 7429  st_by..abstract)
-00000340: 0372 1200 0000 da06 6669 656c 6473 da07  .r......fields..
+00000340: 0372 1100 0000 da06 6669 656c 6473 da07  .r......fields..
 00000350: 6f70 7469 6f6e 73da 0755 7365 5479 7065  options..UseType
 00000360: da05 6c61 6265 6ce9 3200 0000 da10 6973  ..label.2.....is
 00000370: 5f64 6566 6175 6c74 5f76 616c 7565 da0a  _default_value..
-00000380: 736f 7274 5f6f 7264 6572 2902 7214 0000  sort_order).r...
-00000390: 0072 1600 0000 da09 6973 5f61 6374 6976  .r......is_activ
-000003a0: 65da 0969 735f 7379 7374 656d 2901 7220  e..is_system).r 
-000003b0: 0000 0029 0272 1a00 0000 721c 0000 00da  ...).r....r.....
+00000380: 736f 7274 5f6f 7264 6572 2902 7213 0000  sort_order).r...
+00000390: 0072 1500 0000 da09 6973 5f61 6374 6976  .r......is_activ
+000003a0: 65da 0969 735f 7379 7374 656d 2901 721f  e..is_system).r.
+000003b0: 0000 0029 0272 1900 0000 721b 0000 00da  ...).r....r.....
 000003c0: 0e61 6c6c 6f63 6174 696f 6e63 6f64 65da  .allocationcode.
 000003d0: 0875 7365 5f74 7970 657a 1264 6a61 7574  .use_typez.djaut
 000003e0: 6f74 6173 6b2e 5573 6554 7970 6529 0472  otask.UseType).r
-000003f0: 1400 0000 7216 0000 00da 096f 6e5f 6465  ....r......on_de
+000003f0: 1300 0000 7215 0000 00da 096f 6e5f 6465  ....r......on_de
 00000400: 6c65 7465 da02 746f 2903 da0a 6d6f 6465  lete..to)...mode
-00000410: 6c5f 6e61 6d65 7212 0000 00da 0566 6965  l_namer......fie
+00000410: 6c5f 6e61 6d65 7211 0000 00da 0566 6965  l_namer......fie
 00000420: 6c64 4e29 16da 085f 5f6e 616d 655f 5fda  ldN)...__name__.
 00000430: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
 00000440: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
 00000450: 6465 6e63 6965 7372 0200 0000 da0b 4372  denciesr......Cr
 00000460: 6561 7465 4d6f 6465 6c72 0300 0000 da09  eateModelr......
 00000470: 4175 746f 4669 656c 64da 1164 6a61 6e67  AutoField..djang
 00000480: 6f5f 6578 7465 6e73 696f 6e73 da02 6462  o_extensions..db
-00000490: 721d 0000 00da 1543 7265 6174 696f 6e44  r......CreationD
+00000490: 721c 0000 00da 1543 7265 6174 696f 6e44  r......CreationD
 000004a0: 6174 6554 696d 6546 6965 6c64 da19 4d6f  ateTimeField..Mo
 000004b0: 6469 6669 6361 7469 6f6e 4461 7465 5469  dificationDateTi
 000004c0: 6d65 4669 656c 64da 0943 6861 7246 6965  meField..CharFie
 000004d0: 6c64 da0c 426f 6f6c 6561 6e46 6965 6c64  ld..BooleanField
 000004e0: da19 506f 7369 7469 7665 536d 616c 6c49  ..PositiveSmallI
 000004f0: 6e74 6567 6572 4669 656c 64da 0841 6464  ntegerField..Add
 00000500: 4669 656c 64da 0a46 6f72 6569 676e 4b65  Field..ForeignKe
 00000510: 79da 0664 6a61 6e67 6fda 0864 656c 6574  y..django..delet
 00000520: 696f 6eda 0853 4554 5f4e 554c 4cda 0a6f  ion..SET_NULL..o
-00000530: 7065 7261 7469 6f6e 73a9 0072 3f00 0000  perations..r?...
-00000540: 723f 0000 00fa 622f 686f 6d65 2f72 756e  r?....b/home/run
+00000530: 7065 7261 7469 6f6e 73a9 0072 3e00 0000  perations..r>...
+00000540: 723e 0000 00fa 622f 686f 6d65 2f72 756e  r>....b/home/run
 00000550: 6e65 722f 776f 726b 2f64 6a61 6e67 6f2d  ner/work/django-
 00000560: 6175 746f 7461 736b 2f64 6a61 6e67 6f2d  autotask/django-
 00000570: 6175 746f 7461 736b 2f64 6a61 7574 6f74  autotask/djautot
 00000580: 6173 6b2f 6d69 6772 6174 696f 6e73 2f30  ask/migrations/0
 00000590: 3034 325f 6175 746f 5f32 3032 3030 3230  042_auto_2020020
 000005a0: 355f 3130 3537 2e70 7972 0400 0000 0800  5_1057.pyr......
 000005b0: 0000 734a 0000 0008 0302 ff04 0504 0102  ..sJ............
 000005c0: 0214 0114 0114 0112 0112 010e fa02 0902  ................
 000005d0: 0102 0102 fd04 f604 1004 0102 0214 0114  ................
 000005e0: 0114 0112 010e 0110 010e 010e f802 0b02  ................
 000005f0: 0102 fe04 f404 1104 0102 0102 0118 fd04  ................
 00000600: de72 0400 0000 2908 da09 646a 616e 676f  .r....)...django
 00000610: 2e64 6272 0200 0000 7203 0000 00da 1964  .dbr....r......d
 00000620: 6a61 6e67 6f2e 6462 2e6d 6f64 656c 732e  jango.db.models.
-00000630: 6465 6c65 7469 6f6e 723b 0000 00da 1b64  deletionr;.....d
+00000630: 6465 6c65 7469 6f6e 723a 0000 00da 1b64  deletionr:.....d
 00000640: 6a61 6e67 6f5f 6578 7465 6e73 696f 6e73  jango_extensions
-00000650: 2e64 622e 6669 656c 6473 7232 0000 0072  .db.fieldsr2...r
-00000660: 0400 0000 723f 0000 0072 3f00 0000 723f  ....r?...r?...r?
-00000670: 0000 0072 4000 0000 da08 3c6d 6f64 756c  ...r@.....<modul
+00000650: 2e64 622e 6669 656c 6473 7231 0000 0072  .db.fieldsr1...r
+00000660: 0400 0000 723e 0000 0072 3e00 0000 723e  ....r>...r>...r>
+00000670: 0000 0072 3f00 0000 da08 3c6d 6f64 756c  ...r?.....<modul
 00000680: 653e 0300 0000 7306 0000 0010 0108 0108  e>....s.........
 00000690: 03                                       .
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0042_auto_20200205_1455.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0042_auto_20200205_1455.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1304 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 1805 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 1805 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
@@ -36,15 +36,15 @@
 00000230: 686f 7572 6c79 5f66 6163 746f 72e9 0200  hourly_factor...
 00000240: 0000 e909 0000 0029 0472 1300 0000 da0e  .......).r......
 00000250: 6465 6369 6d61 6c5f 706c 6163 6573 da0a  decimal_places..
 00000260: 6d61 785f 6469 6769 7473 7214 0000 00da  max_digitsr.....
 00000270: 0b68 6f75 726c 795f 7261 7465 da09 726f  .hourly_rate..ro
 00000280: 6c65 5f74 7970 6529 0272 1300 0000 7214  le_type).r....r.
 00000290: 0000 00da 0b73 7973 7465 6d5f 726f 6c65  .....system_role
-000002a0: 2902 720d 0000 00da 0666 6965 6c64 735a  ).r......fieldsZ
+000002a0: 2902 720d 0000 00da 0666 6965 6c64 73da  ).r......fields.
 000002b0: 0974 696d 6565 6e74 7279 da04 726f 6c65  .timeentry..role
 000002c0: 7a0f 646a 6175 746f 7461 736b 2e52 6f6c  z.djautotask.Rol
 000002d0: 6529 0472 1300 0000 7214 0000 00da 096f  e).r....r......o
 000002e0: 6e5f 6465 6c65 7465 da02 746f 2903 da0a  n_delete..to)...
 000002f0: 6d6f 6465 6c5f 6e61 6d65 720d 0000 00da  model_namer.....
 00000300: 0566 6965 6c64 4e29 13da 085f 5f6e 616d  .fieldN)...__nam
 00000310: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
@@ -55,25 +55,25 @@
 00000360: 6861 7246 6965 6c64 da0c 426f 6f6c 6561  harField..Boolea
 00000370: 6e46 6965 6c64 da0c 4465 6369 6d61 6c46  nField..DecimalF
 00000380: 6965 6c64 da14 506f 7369 7469 7665 496e  ield..PositiveIn
 00000390: 7465 6765 7246 6965 6c64 da08 4164 6446  tegerField..AddF
 000003a0: 6965 6c64 da0a 466f 7265 6967 6e4b 6579  ield..ForeignKey
 000003b0: da06 646a 616e 676f da02 6462 da08 6465  ..django..db..de
 000003c0: 6c65 7469 6f6e da08 5345 545f 4e55 4c4c  letion..SET_NULL
-000003d0: da0a 6f70 6572 6174 696f 6e73 a900 7234  ..operations..r4
-000003e0: 0000 0072 3400 0000 fa62 2f68 6f6d 652f  ...r4....b/home/
+000003d0: da0a 6f70 6572 6174 696f 6e73 a900 7235  ..operations..r5
+000003e0: 0000 0072 3500 0000 fa62 2f68 6f6d 652f  ...r5....b/home/
 000003f0: 7275 6e6e 6572 2f77 6f72 6b2f 646a 616e  runner/work/djan
 00000400: 676f 2d61 7574 6f74 6173 6b2f 646a 616e  go-autotask/djan
 00000410: 676f 2d61 7574 6f74 6173 6b2f 646a 6175  go-autotask/djau
 00000420: 746f 7461 736b 2f6d 6967 7261 7469 6f6e  totask/migration
 00000430: 732f 3030 3432 5f61 7574 6f5f 3230 3230  s/0042_auto_2020
 00000440: 3032 3035 5f31 3435 352e 7079 7204 0000  0205_1455.pyr...
 00000450: 0007 0000 0073 2800 0000 0803 02ff 0405  .....s(.........
 00000460: 0401 0202 1401 0e01 0e01 1201 1401 1401  ................
 00000470: 1001 0ef8 02fe 040d 0401 0201 0201 18fd  ................
 00000480: 04f2 7204 0000 0029 06da 0964 6a61 6e67  ..r....)...djang
 00000490: 6f2e 6462 7202 0000 0072 0300 0000 da19  o.dbr....r......
 000004a0: 646a 616e 676f 2e64 622e 6d6f 6465 6c73  django.db.models
-000004b0: 2e64 656c 6574 696f 6e72 2f00 0000 7204  .deletionr/...r.
-000004c0: 0000 0072 3400 0000 7234 0000 0072 3400  ...r4...r4...r4.
-000004d0: 0000 7235 0000 00da 083c 6d6f 6475 6c65  ..r5.....<module
+000004b0: 2e64 656c 6574 696f 6e72 3000 0000 7204  .deletionr0...r.
+000004c0: 0000 0072 3500 0000 7235 0000 0072 3500  ...r5...r5...r5.
+000004d0: 0000 7236 0000 00da 083c 6d6f 6475 6c65  ..r6.....<module
 000004e0: 3e03 0000 0073 0400 0000 1001 0803       >....s........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0043_department.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0043_department.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 697 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 b902 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 b902 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
@@ -11,41 +11,41 @@
 000000a0: 0564 0264 0365 066a 0764 0464 0464 0564  .d.d.e.j.d.d.d.d
 000000b0: 0664 078d 0466 0264 0865 066a 0864 0964  .d...f.d.e.j.d.d
 000000c0: 0a8d 0166 0264 0b65 066a 0964 0464 0c64  ...f.d.e.j.d.d.d
 000000d0: 0464 0d8d 0366 0264 0e65 066a 0864 0464  .d...f.d.e.j.d.d
 000000e0: 0f64 0464 0d8d 0366 0267 0464 108d 0267  .d.d...f.g.d...g
 000000f0: 015a 0a64 1153 0029 12da 094d 6967 7261  .Z.d.S.)...Migra
 00000100: 7469 6f6e 2902 da0a 646a 6175 746f 7461  tion)...djautota
-00000110: 736b da17 3030 3432 5f61 7574 6f5f 3230  sk..0042_auto_20
+00000110: 736b 5a17 3030 3432 5f61 7574 6f5f 3230  skZ.0042_auto_20
 00000120: 3230 3032 3035 5f31 3435 35da 0a44 6570  200205_1455..Dep
 00000130: 6172 746d 656e 74da 0269 6454 46da 0249  artment..idTF..I
 00000140: 4429 04da 0c61 7574 6f5f 6372 6561 7465  D)...auto_create
 00000150: 64da 0b70 7269 6d61 7279 5f6b 6579 da09  d..primary_key..
 00000160: 7365 7269 616c 697a 65da 0c76 6572 626f  serialize..verbo
 00000170: 7365 5f6e 616d 65da 046e 616d 65e9 6400  se_name..name.d.
 00000180: 0000 2901 da0a 6d61 785f 6c65 6e67 7468  ..)...max_length
 00000190: da0b 6465 7363 7269 7074 696f 6e69 e803  ..descriptioni..
-000001a0: 0000 2903 da05 626c 616e 6b72 1000 0000  ..)...blankr....
+000001a0: 0000 2903 da05 626c 616e 6b72 0f00 0000  ..)...blankr....
 000001b0: da04 6e75 6c6c da06 6e75 6d62 6572 e932  ..null..number.2
-000001c0: 0000 0029 0272 0e00 0000 da06 6669 656c  ...).r......fiel
+000001c0: 0000 0029 0272 0d00 0000 da06 6669 656c  ...).r......fiel
 000001d0: 6473 4e29 0bda 085f 5f6e 616d 655f 5fda  dsN)...__name__.
 000001e0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
 000001f0: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
 00000200: 6465 6e63 6965 7372 0200 0000 da0b 4372  denciesr......Cr
 00000210: 6561 7465 4d6f 6465 6c72 0300 0000 da09  eateModelr......
 00000220: 4175 746f 4669 656c 64da 0943 6861 7246  AutoField..CharF
 00000230: 6965 6c64 da09 5465 7874 4669 656c 64da  ield..TextField.
-00000240: 0a6f 7065 7261 7469 6f6e 73a9 0072 2000  .operations..r .
-00000250: 0000 7220 0000 00fa 5a2f 686f 6d65 2f72  ..r ....Z/home/r
+00000240: 0a6f 7065 7261 7469 6f6e 73a9 0072 1f00  .operations..r..
+00000250: 0000 721f 0000 00fa 5a2f 686f 6d65 2f72  ..r.....Z/home/r
 00000260: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
 00000270: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
 00000280: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
 00000290: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
 000002a0: 2f30 3034 335f 6465 7061 7274 6d65 6e74  /0043_department
 000002b0: 2e70 7972 0400 0000 0600 0000 7316 0000  .pyr........s...
 000002c0: 0008 0302 ff04 0504 0102 0214 010e 0112  ................
 000002d0: 0112 fc02 fe04 ff72 0400 0000 4e29 04da  .......r....N)..
 000002e0: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
-000002f0: 0300 0000 7204 0000 0072 2000 0000 7220  ....r....r ...r 
-00000300: 0000 0072 2000 0000 7221 0000 00da 083c  ...r ...r!.....<
+000002f0: 0300 0000 7204 0000 0072 1f00 0000 721f  ....r....r....r.
+00000300: 0000 0072 1f00 0000 7220 0000 00da 083c  ...r....r .....<
 00000310: 6d6f 6475 6c65 3e03 0000 0073 0200 0000  module>....s....
 00000320: 1003                                     ..
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0043_timeentry_allocation_code.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0105_tasknote_created_by_contact.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 520 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,49 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 0802 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 1a02 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
 00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
 00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
 000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
 000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
-000000e0: 02da 0a64 6a61 7574 6f74 6173 6b5a 1730  ...djautotaskZ.0
-000000f0: 3034 325f 6175 746f 5f32 3032 3030 3230  042_auto_2020020
-00000100: 355f 3130 3537 da09 7469 6d65 656e 7472  5_1057..timeentr
-00000110: 795a 0f61 6c6c 6f63 6174 696f 6e5f 636f  yZ.allocation_co
-00000120: 6465 547a 1964 6a61 7574 6f74 6173 6b2e  deTz.djautotask.
-00000130: 416c 6c6f 6361 7469 6f6e 436f 6465 2904  AllocationCode).
-00000140: da05 626c 616e 6bda 046e 756c 6cda 096f  ..blank..null..o
-00000150: 6e5f 6465 6c65 7465 da02 746f 2903 da0a  n_delete..to)...
-00000160: 6d6f 6465 6c5f 6e61 6d65 da04 6e61 6d65  model_name..name
-00000170: da05 6669 656c 644e 290d da08 5f5f 6e61  ..fieldN)...__na
-00000180: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000190: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
-000001a0: 6465 7065 6e64 656e 6369 6573 7202 0000  dependenciesr...
-000001b0: 00da 0841 6464 4669 656c 6472 0300 0000  ...AddFieldr....
-000001c0: da0a 466f 7265 6967 6e4b 6579 da06 646a  ..ForeignKey..dj
-000001d0: 616e 676f da02 6462 da08 6465 6c65 7469  ango..db..deleti
-000001e0: 6f6e da08 5345 545f 4e55 4c4c da0a 6f70  on..SET_NULL..op
-000001f0: 6572 6174 696f 6e73 a900 7219 0000 0072  erations..r....r
-00000200: 1900 0000 fa69 2f68 6f6d 652f 7275 6e6e  .....i/home/runn
-00000210: 6572 2f77 6f72 6b2f 646a 616e 676f 2d61  er/work/django-a
-00000220: 7574 6f74 6173 6b2f 646a 616e 676f 2d61  utotask/django-a
-00000230: 7574 6f74 6173 6b2f 646a 6175 746f 7461  utotask/djautota
-00000240: 736b 2f6d 6967 7261 7469 6f6e 732f 3030  sk/migrations/00
-00000250: 3433 5f74 696d 6565 6e74 7279 5f61 6c6c  43_timeentry_all
-00000260: 6f63 6174 696f 6e5f 636f 6465 2e70 7972  ocation_code.pyr
-00000270: 0400 0000 0700 0000 7310 0000 0008 0302  ........s.......
-00000280: ff04 0504 0102 0102 0118 fd04 ff72 0400  .............r..
-00000290: 0000 2906 da09 646a 616e 676f 2e64 6272  ..)...django.dbr
-000002a0: 0200 0000 7203 0000 00da 1964 6a61 6e67  ....r......djang
-000002b0: 6f2e 6462 2e6d 6f64 656c 732e 6465 6c65  o.db.models.dele
-000002c0: 7469 6f6e 7214 0000 0072 0400 0000 7219  tionr....r....r.
-000002d0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-000002e0: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
-000002f0: 7304 0000 0010 0108 03                   s........
+000000e0: 02da 0a64 6a61 7574 6f74 6173 6b5a 2f30  ...djautotaskZ/0
+000000f0: 3130 345f 7265 6e61 6d65 5f61 6c6c 6f63  104_rename_alloc
+00000100: 6174 696f 6e63 6f64 655f 6269 6c6c 696e  ationcode_billin
+00000110: 6763 6f64 655f 616e 645f 6d6f 7265 da08  gcode_and_more..
+00000120: 7461 736b 6e6f 7465 da12 6372 6561 7465  tasknote..create
+00000130: 645f 6279 5f63 6f6e 7461 6374 547a 1264  d_by_contactTz.d
+00000140: 6a61 7574 6f74 6173 6b2e 636f 6e74 6163  jautotask.contac
+00000150: 7429 04da 0562 6c61 6e6b da04 6e75 6c6c  t)...blank..null
+00000160: da09 6f6e 5f64 656c 6574 65da 0274 6f29  ..on_delete..to)
+00000170: 03da 0a6d 6f64 656c 5f6e 616d 65da 046e  ...model_name..n
+00000180: 616d 65da 0566 6965 6c64 4e29 0dda 085f  ame..fieldN)..._
+00000190: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+000001a0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000001b0: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
+000001c0: 0200 0000 da08 4164 6446 6965 6c64 7203  ......AddFieldr.
+000001d0: 0000 00da 0a46 6f72 6569 676e 4b65 79da  .....ForeignKey.
+000001e0: 0664 6a61 6e67 6fda 0264 62da 0864 656c  .django..db..del
+000001f0: 6574 696f 6eda 0853 4554 5f4e 554c 4cda  etion..SET_NULL.
+00000200: 0a6f 7065 7261 7469 6f6e 73a9 0072 1a00  .operations..r..
+00000210: 0000 721a 0000 00fa 6b2f 686f 6d65 2f72  ..r.....k/home/r
+00000220: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
+00000230: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
+00000240: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
+00000250: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
+00000260: 2f30 3130 355f 7461 736b 6e6f 7465 5f63  /0105_tasknote_c
+00000270: 7265 6174 6564 5f62 795f 636f 6e74 6163  reated_by_contac
+00000280: 742e 7079 7204 0000 0007 0000 0073 1000  t.pyr........s..
+00000290: 0000 0803 02ff 0405 0401 0201 0201 18fd  ................
+000002a0: 04ff 7204 0000 0029 06da 0964 6a61 6e67  ..r....)...djang
+000002b0: 6f2e 6462 7202 0000 0072 0300 0000 da19  o.dbr....r......
+000002c0: 646a 616e 676f 2e64 622e 6d6f 6465 6c73  django.db.models
+000002d0: 2e64 656c 6574 696f 6e72 1500 0000 7204  .deletionr....r.
+000002e0: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+000002f0: 0000 721b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000300: 3e03 0000 0073 0400 0000 1001 0803       >....s........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0045_resourceroledepartment_resourceservicedeskrole.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0045_resourceroledepartment_resourceservicedeskrole.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1647 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 6f06 0000  U.........Kdo...
+00000000: 550d 0d0a 0000 0000 3268 4c64 6f06 0000  U.......2hLdo...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0046_auto_20200207_1002.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0046_auto_20200207_1002.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 773 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 0503 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 0503 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0046_ticket_assigned_resource_role.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0047_task_assigned_resource_role.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 542 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,48 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 1e02 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 0b02 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
 00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
 00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
 000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
 000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
-000000e0: 02da 0a64 6a61 7574 6f74 6173 6b5a 3330  ...djautotaskZ30
-000000f0: 3034 355f 7265 736f 7572 6365 726f 6c65  045_resourcerole
-00000100: 6465 7061 7274 6d65 6e74 5f72 6573 6f75  department_resou
-00000110: 7263 6573 6572 7669 6365 6465 736b 726f  rceservicedeskro
-00000120: 6c65 da06 7469 636b 6574 da16 6173 7369  le..ticket..assi
-00000130: 676e 6564 5f72 6573 6f75 7263 655f 726f  gned_resource_ro
-00000140: 6c65 547a 0f64 6a61 7574 6f74 6173 6b2e  leTz.djautotask.
-00000150: 526f 6c65 2904 da05 626c 616e 6bda 046e  Role)...blank..n
-00000160: 756c 6cda 096f 6e5f 6465 6c65 7465 da02  ull..on_delete..
-00000170: 746f 2903 da0a 6d6f 6465 6c5f 6e61 6d65  to)...model_name
-00000180: da04 6e61 6d65 da05 6669 656c 644e 290d  ..name..fieldN).
-00000190: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000001a0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000001b0: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
-000001c0: 6573 7202 0000 00da 0841 6464 4669 656c  esr......AddFiel
-000001d0: 6472 0300 0000 da0a 466f 7265 6967 6e4b  dr......ForeignK
-000001e0: 6579 da06 646a 616e 676f da02 6462 da08  ey..django..db..
-000001f0: 6465 6c65 7469 6f6e da08 5345 545f 4e55  deletion..SET_NU
-00000200: 4c4c da0a 6f70 6572 6174 696f 6e73 a900  LL..operations..
-00000210: 721a 0000 0072 1a00 0000 fa6d 2f68 6f6d  r....r.....m/hom
-00000220: 652f 7275 6e6e 6572 2f77 6f72 6b2f 646a  e/runner/work/dj
-00000230: 616e 676f 2d61 7574 6f74 6173 6b2f 646a  ango-autotask/dj
-00000240: 616e 676f 2d61 7574 6f74 6173 6b2f 646a  ango-autotask/dj
-00000250: 6175 746f 7461 736b 2f6d 6967 7261 7469  autotask/migrati
-00000260: 6f6e 732f 3030 3436 5f74 6963 6b65 745f  ons/0046_ticket_
-00000270: 6173 7369 676e 6564 5f72 6573 6f75 7263  assigned_resourc
-00000280: 655f 726f 6c65 2e70 7972 0400 0000 0700  e_role.pyr......
-00000290: 0000 7310 0000 0008 0302 ff04 0504 0102  ..s.............
-000002a0: 0102 0118 fd04 ff72 0400 0000 2906 da09  .......r....)...
-000002b0: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
-000002c0: 0000 00da 1964 6a61 6e67 6f2e 6462 2e6d  .....django.db.m
-000002d0: 6f64 656c 732e 6465 6c65 7469 6f6e 7215  odels.deletionr.
-000002e0: 0000 0072 0400 0000 721a 0000 0072 1a00  ...r....r....r..
-000002f0: 0000 721a 0000 0072 1b00 0000 da08 3c6d  ..r....r......<m
-00000300: 6f64 756c 653e 0300 0000 7304 0000 0010  odule>....s.....
-00000310: 0108 03                                  ...
+000000e0: 02da 0a64 6a61 7574 6f74 6173 6b5a 2230  ...djautotaskZ"0
+000000f0: 3034 365f 7469 636b 6574 5f61 7373 6967  046_ticket_assig
+00000100: 6e65 645f 7265 736f 7572 6365 5f72 6f6c  ned_resource_rol
+00000110: 65da 0474 6173 6bda 1661 7373 6967 6e65  e..task..assigne
+00000120: 645f 7265 736f 7572 6365 5f72 6f6c 6554  d_resource_roleT
+00000130: 7a0f 646a 6175 746f 7461 736b 2e52 6f6c  z.djautotask.Rol
+00000140: 6529 04da 0562 6c61 6e6b da04 6e75 6c6c  e)...blank..null
+00000150: da09 6f6e 5f64 656c 6574 65da 0274 6f29  ..on_delete..to)
+00000160: 03da 0a6d 6f64 656c 5f6e 616d 65da 046e  ...model_name..n
+00000170: 616d 65da 0566 6965 6c64 4e29 0dda 085f  ame..fieldN)..._
+00000180: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000190: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000001a0: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
+000001b0: 0200 0000 da08 4164 6446 6965 6c64 7203  ......AddFieldr.
+000001c0: 0000 00da 0a46 6f72 6569 676e 4b65 79da  .....ForeignKey.
+000001d0: 0664 6a61 6e67 6fda 0264 62da 0864 656c  .django..db..del
+000001e0: 6574 696f 6eda 0853 4554 5f4e 554c 4cda  etion..SET_NULL.
+000001f0: 0a6f 7065 7261 7469 6f6e 73a9 0072 1a00  .operations..r..
+00000200: 0000 721a 0000 00fa 6b2f 686f 6d65 2f72  ..r.....k/home/r
+00000210: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
+00000220: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
+00000230: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
+00000240: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
+00000250: 2f30 3034 375f 7461 736b 5f61 7373 6967  /0047_task_assig
+00000260: 6e65 645f 7265 736f 7572 6365 5f72 6f6c  ned_resource_rol
+00000270: 652e 7079 7204 0000 0007 0000 0073 1000  e.pyr........s..
+00000280: 0000 0803 02ff 0405 0401 0201 0201 18fd  ................
+00000290: 04ff 7204 0000 0029 06da 0964 6a61 6e67  ..r....)...djang
+000002a0: 6f2e 6462 7202 0000 0072 0300 0000 da19  o.dbr....r......
+000002b0: 646a 616e 676f 2e64 622e 6d6f 6465 6c73  django.db.models
+000002c0: 2e64 656c 6574 696f 6e72 1500 0000 7204  .deletionr....r.
+000002d0: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+000002e0: 0000 721b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000002f0: 3e03 0000 0073 0400 0000 1001 0803       >....s........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0047_auto_20200207_1126.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0085_auto_20201022_1822.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 762 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,43 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 fa02 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 4d02 0000  U.......2hLdM...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
-00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
-00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
-00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
-00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
-00000080: 0000 0000 0000 0000 0000 000a 0000 0040  ...............@
-00000090: 0000 0073 5e00 0000 6500 5a01 6400 5a02  ...s^...e.Z.d.Z.
-000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
-000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
-000000c0: 6405 6406 8d04 6407 8d03 6504 6a05 6408  d.d...d...e.j.d.
-000000d0: 6403 6506 6a07 6404 6404 6508 6a09 6a06  d.e.j.d.d.e.j.j.
-000000e0: 6a0a 6a0b 6405 6406 8d04 6407 8d03 6702  j.j.d.d...d...g.
-000000f0: 5a0c 6409 5300 290a da09 4d69 6772 6174  Z.d.S.)...Migrat
-00000100: 696f 6e29 02da 0a64 6a61 7574 6f74 6173  ion)...djautotas
-00000110: 6bda 1730 3034 365f 6175 746f 5f32 3032  k..0046_auto_202
-00000120: 3030 3230 375f 3130 3032 da04 7461 736b  00207_1002..task
-00000130: da0f 616c 6c6f 6361 7469 6f6e 5f63 6f64  ..allocation_cod
-00000140: 6554 7a19 646a 6175 746f 7461 736b 2e41  eTz.djautotask.A
-00000150: 6c6c 6f63 6174 696f 6e43 6f64 6529 04da  llocationCode)..
-00000160: 0562 6c61 6e6b da04 6e75 6c6c da09 6f6e  .blank..null..on
-00000170: 5f64 656c 6574 65da 0274 6f29 03da 0a6d  _delete..to)...m
-00000180: 6f64 656c 5f6e 616d 65da 046e 616d 65da  odel_name..name.
-00000190: 0566 6965 6c64 da06 7469 636b 6574 4e29  .field..ticketN)
-000001a0: 0dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000001b0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000001c0: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
-000001d0: 6965 7372 0200 0000 da08 4164 6446 6965  iesr......AddFie
-000001e0: 6c64 7203 0000 00da 0a46 6f72 6569 676e  ldr......Foreign
-000001f0: 4b65 79da 0664 6a61 6e67 6fda 0264 62da  Key..django..db.
-00000200: 0864 656c 6574 696f 6eda 0853 4554 5f4e  .deletion..SET_N
-00000210: 554c 4cda 0a6f 7065 7261 7469 6f6e 73a9  ULL..operations.
-00000220: 0072 1c00 0000 721c 0000 00fa 622f 686f  .r....r.....b/ho
-00000230: 6d65 2f72 756e 6e65 722f 776f 726b 2f64  me/runner/work/d
-00000240: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
-00000250: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
-00000260: 6a61 7574 6f74 6173 6b2f 6d69 6772 6174  jautotask/migrat
-00000270: 696f 6e73 2f30 3034 375f 6175 746f 5f32  ions/0047_auto_2
-00000280: 3032 3030 3230 375f 3131 3236 2e70 7972  0200207_1126.pyr
-00000290: 0400 0000 0700 0000 731a 0000 0008 0302  ........s.......
-000002a0: ff04 0504 0102 0102 0118 fd04 0504 0102  ................
-000002b0: 0102 0118 fd04 fa72 0400 0000 2906 da09  .......r....)...
-000002c0: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
-000002d0: 0000 00da 1964 6a61 6e67 6f2e 6462 2e6d  .....django.db.m
-000002e0: 6f64 656c 732e 6465 6c65 7469 6f6e 7217  odels.deletionr.
-000002f0: 0000 0072 0400 0000 721c 0000 0072 1c00  ...r....r....r..
-00000300: 0000 721c 0000 0072 1d00 0000 da08 3c6d  ..r....r......<m
-00000310: 6f64 756c 653e 0300 0000 7304 0000 0010  odule>....s.....
-00000320: 0108 03                                  ...
+00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
+00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
+00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
+00000080: 0000 0900 0000 4000 0000 734a 0000 0065  ......@...sJ...e
+00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
+000000a0: 0564 0264 0365 066a 0764 0465 0864 0464  .d.d.e.j.d.e.d.d
+000000b0: 058d 0364 068d 0365 046a 0564 0764 0365  ...d...e.j.d.d.e
+000000c0: 066a 0764 0465 0864 0464 058d 0364 068d  .j.d.e.d.d...d..
+000000d0: 0367 025a 0964 0853 0029 09da 094d 6967  .g.Z.d.S.)...Mig
+000000e0: 7261 7469 6f6e 2902 da0a 646a 6175 746f  ration)...djauto
+000000f0: 7461 736b 5a25 3030 3834 5f70 726f 6a65  taskZ%0084_proje
+00000100: 6374 7564 6674 7261 636b 6572 5f74 6173  ctudftracker_tas
+00000110: 6b75 6466 7472 6163 6b65 72da 0770 726f  kudftracker..pro
+00000120: 6a65 6374 da03 7564 6654 2903 da05 626c  ject..udfT)...bl
+00000130: 616e 6bda 0764 6566 6175 6c74 da04 6e75  ank..default..nu
+00000140: 6c6c 2903 da0a 6d6f 6465 6c5f 6e61 6d65  ll)...model_name
+00000150: da04 6e61 6d65 da05 6669 656c 64da 0474  ..name..field..t
+00000160: 6173 6b4e 290a da08 5f5f 6e61 6d65 5f5f  askN)...__name__
+00000170: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000180: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
+00000190: 6e64 656e 6369 6573 7202 0000 00da 0841  ndenciesr......A
+000001a0: 6464 4669 656c 6472 0300 0000 da09 4a53  ddFieldr......JS
+000001b0: 4f4e 4669 656c 64da 0464 6963 74da 0a6f  ONField..dict..o
+000001c0: 7065 7261 7469 6f6e 73a9 0072 1700 0000  perations..r....
+000001d0: 7217 0000 00fa 622f 686f 6d65 2f72 756e  r.....b/home/run
+000001e0: 6e65 722f 776f 726b 2f64 6a61 6e67 6f2d  ner/work/django-
+000001f0: 6175 746f 7461 736b 2f64 6a61 6e67 6f2d  autotask/django-
+00000200: 6175 746f 7461 736b 2f64 6a61 7574 6f74  autotask/djautot
+00000210: 6173 6b2f 6d69 6772 6174 696f 6e73 2f30  ask/migrations/0
+00000220: 3038 355f 6175 746f 5f32 3032 3031 3032  085_auto_2020102
+00000230: 325f 3138 3232 2e70 7972 0400 0000 0600  2_1822.pyr......
+00000240: 0000 731a 0000 0008 0302 ff04 0504 0102  ..s.............
+00000250: 0102 010e fd04 0504 0102 0102 010e fd04  ................
+00000260: fa72 0400 0000 4e29 04da 0964 6a61 6e67  .r....N)...djang
+00000270: 6f2e 6462 7202 0000 0072 0300 0000 7204  o.dbr....r....r.
+00000280: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
+00000290: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000002a0: 3e03 0000 0073 0200 0000 1003            >....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0047_task_assigned_resource_role.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0046_ticket_assigned_resource_role.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 523 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 0b02 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 1e02 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
 00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
 00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
 000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
 000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
-000000e0: 02da 0a64 6a61 7574 6f74 6173 6bda 2230  ...djautotask."0
-000000f0: 3034 365f 7469 636b 6574 5f61 7373 6967  046_ticket_assig
-00000100: 6e65 645f 7265 736f 7572 6365 5f72 6f6c  ned_resource_rol
-00000110: 65da 0474 6173 6bda 1661 7373 6967 6e65  e..task..assigne
-00000120: 645f 7265 736f 7572 6365 5f72 6f6c 6554  d_resource_roleT
-00000130: 7a0f 646a 6175 746f 7461 736b 2e52 6f6c  z.djautotask.Rol
-00000140: 6529 04da 0562 6c61 6e6b da04 6e75 6c6c  e)...blank..null
-00000150: da09 6f6e 5f64 656c 6574 65da 0274 6f29  ..on_delete..to)
-00000160: 03da 0a6d 6f64 656c 5f6e 616d 65da 046e  ...model_name..n
-00000170: 616d 65da 0566 6965 6c64 4e29 0dda 085f  ame..fieldN)..._
-00000180: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000190: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000001a0: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
-000001b0: 0200 0000 da08 4164 6446 6965 6c64 7203  ......AddFieldr.
-000001c0: 0000 00da 0a46 6f72 6569 676e 4b65 79da  .....ForeignKey.
-000001d0: 0664 6a61 6e67 6fda 0264 62da 0864 656c  .django..db..del
-000001e0: 6574 696f 6eda 0853 4554 5f4e 554c 4cda  etion..SET_NULL.
-000001f0: 0a6f 7065 7261 7469 6f6e 73a9 0072 1b00  .operations..r..
-00000200: 0000 721b 0000 00fa 6b2f 686f 6d65 2f72  ..r.....k/home/r
-00000210: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
-00000220: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
-00000230: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
-00000240: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
-00000250: 2f30 3034 375f 7461 736b 5f61 7373 6967  /0047_task_assig
-00000260: 6e65 645f 7265 736f 7572 6365 5f72 6f6c  ned_resource_rol
-00000270: 652e 7079 7204 0000 0007 0000 0073 1000  e.pyr........s..
-00000280: 0000 0803 02ff 0405 0401 0201 0201 18fd  ................
-00000290: 04ff 7204 0000 0029 06da 0964 6a61 6e67  ..r....)...djang
-000002a0: 6f2e 6462 7202 0000 0072 0300 0000 da19  o.dbr....r......
-000002b0: 646a 616e 676f 2e64 622e 6d6f 6465 6c73  django.db.models
-000002c0: 2e64 656c 6574 696f 6e72 1600 0000 7204  .deletionr....r.
-000002d0: 0000 0072 1b00 0000 721b 0000 0072 1b00  ...r....r....r..
-000002e0: 0000 721c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000002f0: 3e03 0000 0073 0400 0000 1001 0803       >....s........
+000000e0: 02da 0a64 6a61 7574 6f74 6173 6bda 3330  ...djautotask.30
+000000f0: 3034 355f 7265 736f 7572 6365 726f 6c65  045_resourcerole
+00000100: 6465 7061 7274 6d65 6e74 5f72 6573 6f75  department_resou
+00000110: 7263 6573 6572 7669 6365 6465 736b 726f  rceservicedeskro
+00000120: 6c65 da06 7469 636b 6574 da16 6173 7369  le..ticket..assi
+00000130: 676e 6564 5f72 6573 6f75 7263 655f 726f  gned_resource_ro
+00000140: 6c65 547a 0f64 6a61 7574 6f74 6173 6b2e  leTz.djautotask.
+00000150: 526f 6c65 2904 da05 626c 616e 6bda 046e  Role)...blank..n
+00000160: 756c 6cda 096f 6e5f 6465 6c65 7465 da02  ull..on_delete..
+00000170: 746f 2903 da0a 6d6f 6465 6c5f 6e61 6d65  to)...model_name
+00000180: da04 6e61 6d65 da05 6669 656c 644e 290d  ..name..fieldN).
+00000190: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+000001a0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+000001b0: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
+000001c0: 6573 7202 0000 00da 0841 6464 4669 656c  esr......AddFiel
+000001d0: 6472 0300 0000 da0a 466f 7265 6967 6e4b  dr......ForeignK
+000001e0: 6579 da06 646a 616e 676f da02 6462 da08  ey..django..db..
+000001f0: 6465 6c65 7469 6f6e da08 5345 545f 4e55  deletion..SET_NU
+00000200: 4c4c da0a 6f70 6572 6174 696f 6e73 a900  LL..operations..
+00000210: 721b 0000 0072 1b00 0000 fa6d 2f68 6f6d  r....r.....m/hom
+00000220: 652f 7275 6e6e 6572 2f77 6f72 6b2f 646a  e/runner/work/dj
+00000230: 616e 676f 2d61 7574 6f74 6173 6b2f 646a  ango-autotask/dj
+00000240: 616e 676f 2d61 7574 6f74 6173 6b2f 646a  ango-autotask/dj
+00000250: 6175 746f 7461 736b 2f6d 6967 7261 7469  autotask/migrati
+00000260: 6f6e 732f 3030 3436 5f74 6963 6b65 745f  ons/0046_ticket_
+00000270: 6173 7369 676e 6564 5f72 6573 6f75 7263  assigned_resourc
+00000280: 655f 726f 6c65 2e70 7972 0400 0000 0700  e_role.pyr......
+00000290: 0000 7310 0000 0008 0302 ff04 0504 0102  ..s.............
+000002a0: 0102 0118 fd04 ff72 0400 0000 2906 da09  .......r....)...
+000002b0: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
+000002c0: 0000 00da 1964 6a61 6e67 6f2e 6462 2e6d  .....django.db.m
+000002d0: 6f64 656c 732e 6465 6c65 7469 6f6e 7216  odels.deletionr.
+000002e0: 0000 0072 0400 0000 721b 0000 0072 1b00  ...r....r....r..
+000002f0: 0000 721b 0000 0072 1c00 0000 da08 3c6d  ..r....r......<m
+00000300: 6f64 756c 653e 0300 0000 7304 0000 0010  odule>....s.....
+00000310: 0108 03                                  ...
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0048_auto_20200211_1037.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0040_auto_20200204_1538.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 853 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,46 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 5503 0000  U.........KdU...
+00000000: 550d 0d0a 0000 0000 3268 4c64 8402 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00000080: 0000 0b00 0000 4000 0000 736a 0000 0065  ......@...sj...e
+00000080: 0000 0a00 0000 4000 0000 734e 0000 0065  ......@...sN...e
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
 000000a0: 0564 0264 0365 066a 0764 0464 0564 0664  .d.d.e.j.d.d.d.d
 000000b0: 0464 078d 0464 088d 0365 046a 0564 0264  .d...d...e.j.d.d
 000000c0: 0965 066a 0764 0464 0564 0664 0464 078d  .e.j.d.d.d.d.d..
-000000d0: 0464 088d 0365 046a 0564 0264 0a65 066a  .d...e.j.d.d.e.j
-000000e0: 0764 0464 0564 0664 0464 078d 0464 088d  .d.d.d.d.d...d..
-000000f0: 0367 035a 0864 0b53 0029 0cda 094d 6967  .g.Z.d.S.)...Mig
-00000100: 7261 7469 6f6e 2902 da0a 646a 6175 746f  ration)...djauto
-00000110: 7461 736b 5a17 3030 3437 5f61 7574 6f5f  taskZ.0047_auto_
-00000120: 3230 3230 3032 3037 5f31 3132 36da 0974  20200207_1126..t
-00000130: 696d 6565 6e74 7279 da0d 686f 7572 735f  imeentry..hours_
-00000140: 746f 5f62 696c 6c54 e904 0000 00e9 0900  to_billT........
-00000150: 0000 2904 da05 626c 616e 6bda 0e64 6563  ..)...blank..dec
-00000160: 696d 616c 5f70 6c61 6365 73da 0a6d 6178  imal_places..max
-00000170: 5f64 6967 6974 73da 046e 756c 6c29 03da  _digits..null)..
-00000180: 0a6d 6f64 656c 5f6e 616d 65da 046e 616d  .model_name..nam
-00000190: 65da 0566 6965 6c64 da0c 686f 7572 735f  e..field..hours_
-000001a0: 776f 726b 6564 da0c 6f66 6673 6574 5f68  worked..offset_h
-000001b0: 6f75 7273 4e29 09da 085f 5f6e 616d 655f  oursN)...__name_
-000001c0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000001d0: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
-000001e0: 656e 6465 6e63 6965 7372 0200 0000 da0a  endenciesr......
-000001f0: 416c 7465 7246 6965 6c64 7203 0000 00da  AlterFieldr.....
-00000200: 0c44 6563 696d 616c 4669 656c 64da 0a6f  .DecimalField..o
-00000210: 7065 7261 7469 6f6e 73a9 0072 1a00 0000  perations..r....
-00000220: 721a 0000 00fa 622f 686f 6d65 2f72 756e  r.....b/home/run
-00000230: 6e65 722f 776f 726b 2f64 6a61 6e67 6f2d  ner/work/django-
-00000240: 6175 746f 7461 736b 2f64 6a61 6e67 6f2d  autotask/django-
-00000250: 6175 746f 7461 736b 2f64 6a61 7574 6f74  autotask/djautot
-00000260: 6173 6b2f 6d69 6772 6174 696f 6e73 2f30  ask/migrations/0
-00000270: 3034 385f 6175 746f 5f32 3032 3030 3231  048_auto_2020021
-00000280: 315f 3130 3337 2e70 7972 0400 0000 0600  1_1037.pyr......
-00000290: 0000 7324 0000 0008 0302 ff04 0504 0102  ..s$............
-000002a0: 0102 0110 fd04 0504 0102 0102 0110 fd04  ................
-000002b0: 0504 0102 0102 0110 fd04 f572 0400 0000  ...........r....
-000002c0: 4e29 04da 0964 6a61 6e67 6f2e 6462 7202  N)...django.dbr.
-000002d0: 0000 0072 0300 0000 7204 0000 0072 1a00  ...r....r....r..
-000002e0: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-000002f0: 00da 083c 6d6f 6475 6c65 3e03 0000 0073  ...<module>....s
-00000300: 0200 0000 1003                           ......
+000000d0: 0464 088d 0367 025a 0864 0a53 0029 0bda  .d...g.Z.d.S.)..
+000000e0: 094d 6967 7261 7469 6f6e 2902 da0a 646a  .Migration)...dj
+000000f0: 6175 746f 7461 736b da18 3030 3339 5f6d  autotask..0039_m
+00000100: 6572 6765 5f32 3032 3030 3133 315f 3130  erge_20200131_10
+00000110: 3232 da04 7461 736b da0f 6573 7469 6d61  22..task..estima
+00000120: 7465 645f 686f 7572 7354 e902 0000 00e9  ted_hoursT......
+00000130: 0600 0000 2904 da05 626c 616e 6bda 0e64  ....)...blank..d
+00000140: 6563 696d 616c 5f70 6c61 6365 73da 0a6d  ecimal_places..m
+00000150: 6178 5f64 6967 6974 73da 046e 756c 6c29  ax_digits..null)
+00000160: 03da 0a6d 6f64 656c 5f6e 616d 65da 046e  ...model_name..n
+00000170: 616d 65da 0566 6965 6c64 da0f 7265 6d61  ame..field..rema
+00000180: 696e 696e 675f 686f 7572 734e 2909 da08  ining_hoursN)...
+00000190: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000001a0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000001b0: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
+000001c0: 7202 0000 00da 0a41 6c74 6572 4669 656c  r......AlterFiel
+000001d0: 6472 0300 0000 da0c 4465 6369 6d61 6c46  dr......DecimalF
+000001e0: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
+000001f0: a900 721a 0000 0072 1a00 0000 fa62 2f68  ..r....r.....b/h
+00000200: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
+00000210: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
+00000220: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
+00000230: 646a 6175 746f 7461 736b 2f6d 6967 7261  djautotask/migra
+00000240: 7469 6f6e 732f 3030 3430 5f61 7574 6f5f  tions/0040_auto_
+00000250: 3230 3230 3032 3034 5f31 3533 382e 7079  20200204_1538.py
+00000260: 7204 0000 0006 0000 0073 1a00 0000 0803  r........s......
+00000270: 02ff 0405 0401 0201 0201 10fd 0405 0401  ................
+00000280: 0201 0201 10fd 04fa 7204 0000 004e 2904  ........r....N).
+00000290: da09 646a 616e 676f 2e64 6272 0200 0000  ..django.dbr....
+000002a0: 7203 0000 0072 0400 0000 721a 0000 0072  r....r....r....r
+000002b0: 1a00 0000 721a 0000 0072 1b00 0000 da08  ....r....r......
+000002c0: 3c6d 6f64 756c 653e 0300 0000 7302 0000  <module>....s...
+000002d0: 0010 03                                  ...
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0049_merge_20200227_1701.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0049_merge_20200227_1701.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 289 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 2101 0000  U.........Kd!...
+00000000: 550d 0d0a 0000 0000 3268 4c64 2101 0000  U.......2hLd!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0200 0000 4000 0000 7318  ..........@...s.
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0050_remove_ticket_role.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0050_remove_ticket_role.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 331 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 4b01 0000  U.........KdK...
+00000000: 550d 0d0a 0000 0000 3268 4c64 4b01 0000  U.......2hLdK...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0400 0000 4000 0000 7322  ..........@...s"
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0051_auto_20200315_1819.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0051_auto_20200315_1819.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 754 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 f202 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 f202 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
@@ -11,15 +11,15 @@
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
 000000c0: 6405 6406 8d04 6407 8d03 6504 6a05 6408  d.d...d...e.j.d.
 000000d0: 6403 6506 6a07 6404 6404 6508 6a09 6a06  d.e.j.d.d.e.j.j.
 000000e0: 6a0a 6a0b 6405 6406 8d04 6407 8d03 6702  j.j.d.d...d...g.
 000000f0: 5a0c 6409 5300 290a da09 4d69 6772 6174  Z.d.S.)...Migrat
 00000100: 696f 6e29 02da 0a64 6a61 7574 6f74 6173  ion)...djautotas
-00000110: 6b5a 1730 3035 305f 7265 6d6f 7665 5f74  kZ.0050_remove_t
+00000110: 6bda 1730 3035 305f 7265 6d6f 7665 5f74  k..0050_remove_t
 00000120: 6963 6b65 745f 726f 6c65 5a15 7461 736b  icket_roleZ.task
 00000130: 7365 636f 6e64 6172 7972 6573 6f75 7263  secondaryresourc
 00000140: 65da 0472 6f6c 6554 7a0f 646a 6175 746f  e..roleTz.djauto
 00000150: 7461 736b 2e52 6f6c 6529 04da 0562 6c61  task.Role)...bla
 00000160: 6e6b da04 6e75 6c6c da09 6f6e 5f64 656c  nk..null..on_del
 00000170: 6574 65da 0274 6f29 03da 0a6d 6f64 656c  ete..to)...model
 00000180: 5f6e 616d 65da 046e 616d 65da 0566 6965  _name..name..fie
@@ -28,24 +28,24 @@
 000001b0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
 000001c0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
 000001d0: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
 000001e0: 7202 0000 00da 0841 6464 4669 656c 6472  r......AddFieldr
 000001f0: 0300 0000 da0a 466f 7265 6967 6e4b 6579  ......ForeignKey
 00000200: da06 646a 616e 676f da02 6462 da08 6465  ..django..db..de
 00000210: 6c65 7469 6f6e da08 5345 545f 4e55 4c4c  letion..SET_NULL
-00000220: da0a 6f70 6572 6174 696f 6e73 a900 7219  ..operations..r.
-00000230: 0000 0072 1900 0000 fa62 2f68 6f6d 652f  ...r.....b/home/
+00000220: da0a 6f70 6572 6174 696f 6e73 a900 721a  ..operations..r.
+00000230: 0000 0072 1a00 0000 fa62 2f68 6f6d 652f  ...r.....b/home/
 00000240: 7275 6e6e 6572 2f77 6f72 6b2f 646a 616e  runner/work/djan
 00000250: 676f 2d61 7574 6f74 6173 6b2f 646a 616e  go-autotask/djan
 00000260: 676f 2d61 7574 6f74 6173 6b2f 646a 6175  go-autotask/djau
 00000270: 746f 7461 736b 2f6d 6967 7261 7469 6f6e  totask/migration
 00000280: 732f 3030 3531 5f61 7574 6f5f 3230 3230  s/0051_auto_2020
 00000290: 3033 3135 5f31 3831 392e 7079 7204 0000  0315_1819.pyr...
 000002a0: 0007 0000 0073 1a00 0000 0803 02ff 0405  .....s..........
 000002b0: 0401 0201 0201 18fd 0405 0401 0201 0201  ................
 000002c0: 18fd 04fa 7204 0000 0029 06da 0964 6a61  ....r....)...dja
 000002d0: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
 000002e0: da19 646a 616e 676f 2e64 622e 6d6f 6465  ..django.db.mode
-000002f0: 6c73 2e64 656c 6574 696f 6e72 1400 0000  ls.deletionr....
-00000300: 7204 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00000310: 1900 0000 721a 0000 00da 083c 6d6f 6475  ....r......<modu
+000002f0: 6c73 2e64 656c 6574 696f 6e72 1500 0000  ls.deletionr....
+00000300: 7204 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00000310: 1a00 0000 721b 0000 00da 083c 6d6f 6475  ....r......<modu
 00000320: 6c65 3e03 0000 0073 0400 0000 1001 0803  le>....s........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0051_contract.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0051_contract.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 779 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 0b03 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 0b03 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
@@ -12,47 +12,47 @@
 000000b0: 6a07 6404 6404 6405 6406 6407 8d04 6602  j.d.d.d.d.d...f.
 000000c0: 6408 6506 6a08 6409 640a 8d01 6602 640b  d.e.j.d.d...f.d.
 000000d0: 6506 6a08 6404 640c 6404 640d 8d03 6602  e.j.d.d.d.d...f.
 000000e0: 640e 6506 6a09 6404 6404 650a 6a0b 6a06  d.e.j.d.d.e.j.j.
 000000f0: 6a0c 6a0d 640f 6410 8d04 6602 6704 6411  j.j.d.d...f.g.d.
 00000100: 8d02 6701 5a0e 6412 5300 2913 da09 4d69  ..g.Z.d.S.)...Mi
 00000110: 6772 6174 696f 6e29 02da 0a64 6a61 7574  gration)...djaut
-00000120: 6f74 6173 6bda 1730 3035 305f 7265 6d6f  otask..0050_remo
+00000120: 6f74 6173 6b5a 1730 3035 305f 7265 6d6f  otaskZ.0050_remo
 00000130: 7665 5f74 6963 6b65 745f 726f 6c65 da08  ve_ticket_role..
 00000140: 436f 6e74 7261 6374 da02 6964 5446 da02  Contract..idTF..
 00000150: 4944 2904 da0c 6175 746f 5f63 7265 6174  ID)...auto_creat
 00000160: 6564 da0b 7072 696d 6172 795f 6b65 79da  ed..primary_key.
 00000170: 0973 6572 6961 6c69 7a65 da0c 7665 7262  .serialize..verb
 00000180: 6f73 655f 6e61 6d65 da04 6e61 6d65 e9fa  ose_name..name..
 00000190: 0000 0029 01da 0a6d 6178 5f6c 656e 6774  ...)...max_lengt
 000001a0: 68da 066e 756d 6265 72e9 3200 0000 2903  h..number.2...).
-000001b0: da05 626c 616e 6b72 1000 0000 da04 6e75  ..blankr......nu
+000001b0: da05 626c 616e 6b72 0f00 0000 da04 6e75  ..blankr......nu
 000001c0: 6c6c da07 6163 636f 756e 747a 1264 6a61  ll..accountz.dja
 000001d0: 7574 6f74 6173 6b2e 4163 636f 756e 7429  utotask.Account)
-000001e0: 0472 1300 0000 7214 0000 00da 096f 6e5f  .r....r......on_
-000001f0: 6465 6c65 7465 da02 746f 2902 720e 0000  delete..to).r...
+000001e0: 0472 1200 0000 7213 0000 00da 096f 6e5f  .r....r......on_
+000001f0: 6465 6c65 7465 da02 746f 2902 720d 0000  delete..to).r...
 00000200: 00da 0666 6965 6c64 734e 290f da08 5f5f  ...fieldsN)...__
 00000210: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
 00000220: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
 00000230: da0c 6465 7065 6e64 656e 6369 6573 7202  ..dependenciesr.
 00000240: 0000 00da 0b43 7265 6174 654d 6f64 656c  .....CreateModel
 00000250: 7203 0000 00da 0941 7574 6f46 6965 6c64  r......AutoField
 00000260: da09 4368 6172 4669 656c 64da 0a46 6f72  ..CharField..For
 00000270: 6569 676e 4b65 79da 0664 6a61 6e67 6fda  eignKey..django.
 00000280: 0264 62da 0864 656c 6574 696f 6eda 0853  .db..deletion..S
 00000290: 4554 5f4e 554c 4cda 0a6f 7065 7261 7469  ET_NULL..operati
-000002a0: 6f6e 73a9 0072 2600 0000 7226 0000 00fa  ons..r&...r&....
+000002a0: 6f6e 73a9 0072 2500 0000 7225 0000 00fa  ons..r%...r%....
 000002b0: 582f 686f 6d65 2f72 756e 6e65 722f 776f  X/home/runner/wo
 000002c0: 726b 2f64 6a61 6e67 6f2d 6175 746f 7461  rk/django-autota
 000002d0: 736b 2f64 6a61 6e67 6f2d 6175 746f 7461  sk/django-autota
 000002e0: 736b 2f64 6a61 7574 6f74 6173 6b2f 6d69  sk/djautotask/mi
 000002f0: 6772 6174 696f 6e73 2f30 3035 315f 636f  grations/0051_co
 00000300: 6e74 7261 6374 2e70 7972 0400 0000 0700  ntract.pyr......
 00000310: 0000 7316 0000 0008 0302 ff04 0504 0102  ..s.............
 00000320: 0214 010e 0112 011c fc02 fe04 ff72 0400  .............r..
 00000330: 0000 2906 da09 646a 616e 676f 2e64 6272  ..)...django.dbr
 00000340: 0200 0000 7203 0000 00da 1964 6a61 6e67  ....r......djang
 00000350: 6f2e 6462 2e6d 6f64 656c 732e 6465 6c65  o.db.models.dele
-00000360: 7469 6f6e 7221 0000 0072 0400 0000 7226  tionr!...r....r&
-00000370: 0000 0072 2600 0000 7226 0000 0072 2700  ...r&...r&...r'.
+00000360: 7469 6f6e 7220 0000 0072 0400 0000 7225  tionr ...r....r%
+00000370: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
 00000380: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
 00000390: 7304 0000 0010 0108 03                   s........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0052_contract_status.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0052_contract_status.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 445 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 bd01 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 bd01 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0053_timeentry_contract.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0106_ticketnote_created_by_contact.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 504 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 f801 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 0d02 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
 00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
 00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
 000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
 000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
-000000e0: 02da 0a64 6a61 7574 6f74 6173 6b5a 1430  ...djautotaskZ.0
-000000f0: 3035 325f 636f 6e74 7261 6374 5f73 7461  052_contract_sta
-00000100: 7475 73da 0974 696d 6565 6e74 7279 da08  tus..timeentry..
-00000110: 636f 6e74 7261 6374 547a 1364 6a61 7574  contractTz.djaut
-00000120: 6f74 6173 6b2e 436f 6e74 7261 6374 2904  otask.Contract).
-00000130: da05 626c 616e 6bda 046e 756c 6cda 096f  ..blank..null..o
-00000140: 6e5f 6465 6c65 7465 da02 746f 2903 da0a  n_delete..to)...
-00000150: 6d6f 6465 6c5f 6e61 6d65 da04 6e61 6d65  model_name..name
-00000160: da05 6669 656c 644e 290d da08 5f5f 6e61  ..fieldN)...__na
-00000170: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000180: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
-00000190: 6465 7065 6e64 656e 6369 6573 7202 0000  dependenciesr...
-000001a0: 00da 0841 6464 4669 656c 6472 0300 0000  ...AddFieldr....
-000001b0: da0a 466f 7265 6967 6e4b 6579 da06 646a  ..ForeignKey..dj
-000001c0: 616e 676f da02 6462 da08 6465 6c65 7469  ango..db..deleti
-000001d0: 6f6e da08 5345 545f 4e55 4c4c da0a 6f70  on..SET_NULL..op
-000001e0: 6572 6174 696f 6e73 a900 721a 0000 0072  erations..r....r
-000001f0: 1a00 0000 fa62 2f68 6f6d 652f 7275 6e6e  .....b/home/runn
-00000200: 6572 2f77 6f72 6b2f 646a 616e 676f 2d61  er/work/django-a
-00000210: 7574 6f74 6173 6b2f 646a 616e 676f 2d61  utotask/django-a
-00000220: 7574 6f74 6173 6b2f 646a 6175 746f 7461  utotask/djautota
-00000230: 736b 2f6d 6967 7261 7469 6f6e 732f 3030  sk/migrations/00
-00000240: 3533 5f74 696d 6565 6e74 7279 5f63 6f6e  53_timeentry_con
-00000250: 7472 6163 742e 7079 7204 0000 0007 0000  tract.pyr.......
-00000260: 0073 1000 0000 0803 02ff 0405 0401 0201  .s..............
-00000270: 0201 18fd 04ff 7204 0000 0029 06da 0964  ......r....)...d
-00000280: 6a61 6e67 6f2e 6462 7202 0000 0072 0300  jango.dbr....r..
-00000290: 0000 da19 646a 616e 676f 2e64 622e 6d6f  ....django.db.mo
-000002a0: 6465 6c73 2e64 656c 6574 696f 6e72 1500  dels.deletionr..
-000002b0: 0000 7204 0000 0072 1a00 0000 721a 0000  ..r....r....r...
-000002c0: 0072 1a00 0000 721b 0000 00da 083c 6d6f  .r....r......<mo
-000002d0: 6475 6c65 3e03 0000 0073 0400 0000 1001  dule>....s......
-000002e0: 0803                                     ..
+000000e0: 02da 0a64 6a61 7574 6f74 6173 6b5a 2030  ...djautotaskZ 0
+000000f0: 3130 355f 7461 736b 6e6f 7465 5f63 7265  105_tasknote_cre
+00000100: 6174 6564 5f62 795f 636f 6e74 6163 74da  ated_by_contact.
+00000110: 0a74 6963 6b65 746e 6f74 65da 1263 7265  .ticketnote..cre
+00000120: 6174 6564 5f62 795f 636f 6e74 6163 7454  ated_by_contactT
+00000130: 7a12 646a 6175 746f 7461 736b 2e63 6f6e  z.djautotask.con
+00000140: 7461 6374 2904 da05 626c 616e 6bda 046e  tact)...blank..n
+00000150: 756c 6cda 096f 6e5f 6465 6c65 7465 da02  ull..on_delete..
+00000160: 746f 2903 da0a 6d6f 6465 6c5f 6e61 6d65  to)...model_name
+00000170: da04 6e61 6d65 da05 6669 656c 644e 290d  ..name..fieldN).
+00000180: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000190: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+000001a0: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
+000001b0: 6573 7202 0000 00da 0841 6464 4669 656c  esr......AddFiel
+000001c0: 6472 0300 0000 da0a 466f 7265 6967 6e4b  dr......ForeignK
+000001d0: 6579 da06 646a 616e 676f da02 6462 da08  ey..django..db..
+000001e0: 6465 6c65 7469 6f6e da08 5345 545f 4e55  deletion..SET_NU
+000001f0: 4c4c da0a 6f70 6572 6174 696f 6e73 a900  LL..operations..
+00000200: 721a 0000 0072 1a00 0000 fa6d 2f68 6f6d  r....r.....m/hom
+00000210: 652f 7275 6e6e 6572 2f77 6f72 6b2f 646a  e/runner/work/dj
+00000220: 616e 676f 2d61 7574 6f74 6173 6b2f 646a  ango-autotask/dj
+00000230: 616e 676f 2d61 7574 6f74 6173 6b2f 646a  ango-autotask/dj
+00000240: 6175 746f 7461 736b 2f6d 6967 7261 7469  autotask/migrati
+00000250: 6f6e 732f 3031 3036 5f74 6963 6b65 746e  ons/0106_ticketn
+00000260: 6f74 655f 6372 6561 7465 645f 6279 5f63  ote_created_by_c
+00000270: 6f6e 7461 6374 2e70 7972 0400 0000 0700  ontact.pyr......
+00000280: 0000 7310 0000 0008 0302 ff04 0504 0102  ..s.............
+00000290: 0102 0118 fd04 ff72 0400 0000 2906 da09  .......r....)...
+000002a0: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
+000002b0: 0000 00da 1964 6a61 6e67 6f2e 6462 2e6d  .....django.db.m
+000002c0: 6f64 656c 732e 6465 6c65 7469 6f6e 7215  odels.deletionr.
+000002d0: 0000 0072 0400 0000 721a 0000 0072 1a00  ...r....r....r..
+000002e0: 0000 721a 0000 0072 1b00 0000 da08 3c6d  ..r....r......<m
+000002f0: 6f64 756c 653e 0300 0000 7304 0000 0010  odule>....s.....
+00000300: 0108 03                                  ...
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0055_auto_20200325_0928.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0055_auto_20200325_0928.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 740 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 e402 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 e402 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0055_auto_20200325_1335.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0055_auto_20200325_1335.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1506 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 e205 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 e205 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
@@ -19,71 +19,71 @@
 00000120: 6413 6506 6a0e 6405 6410 8d01 6602 6414  d.e.j.d.d...f.d.
 00000130: 6506 6a0e 6405 6410 8d01 6602 6708 6405  e.j.d.d...f.g.d.
 00000140: 6415 6416 9c02 6417 8d03 6504 6a10 6418  d.d...d...e.j.d.
 00000150: 6419 6506 6a11 6404 6404 6512 6a09 6a06  d.e.j.d.d.e.j.j.
 00000160: 6a13 6a14 641a 641b 8d04 641c 8d03 6702  j.j.d.d...d...g.
 00000170: 5a15 641d 5300 291e da09 4d69 6772 6174  Z.d.S.)...Migrat
 00000180: 696f 6e29 02da 0a64 6a61 7574 6f74 6173  ion)...djautotas
-00000190: 6b5a 1830 3035 345f 6d65 7267 655f 3230  kZ.0054_merge_20
+00000190: 6bda 1830 3035 345f 6d65 7267 655f 3230  k..0054_merge_20
 000001a0: 3230 3033 3233 5f31 3531 31da 0b41 6363  200323_1511..Acc
 000001b0: 6f75 6e74 5479 7065 da02 6964 5446 da02  ountType..idTF..
 000001c0: 4944 2904 da0c 6175 746f 5f63 7265 6174  ID)...auto_creat
 000001d0: 6564 da0b 7072 696d 6172 795f 6b65 79da  ed..primary_key.
 000001e0: 0973 6572 6961 6c69 7a65 da0c 7665 7262  .serialize..verb
 000001f0: 6f73 655f 6e61 6d65 da07 6372 6561 7465  ose_name..create
 00000200: 6429 02da 0c61 7574 6f5f 6e6f 775f 6164  d)...auto_now_ad
-00000210: 6472 0c00 0000 da08 6d6f 6469 6669 6564  dr......modified
-00000220: 2902 da08 6175 746f 5f6e 6f77 720c 0000  )...auto_nowr...
+00000210: 6472 0d00 0000 da08 6d6f 6469 6669 6564  dr......modified
+00000220: 2902 da08 6175 746f 5f6e 6f77 720d 0000  )...auto_nowr...
 00000230: 00da 056c 6162 656c e932 0000 0029 03da  ...label.2...)..
 00000240: 0562 6c61 6e6b da0a 6d61 785f 6c65 6e67  .blank..max_leng
 00000250: 7468 da04 6e75 6c6c da10 6973 5f64 6566  th..null..is_def
 00000260: 6175 6c74 5f76 616c 7565 2901 da07 6465  ault_value)...de
 00000270: 6661 756c 74da 0a73 6f72 745f 6f72 6465  fault..sort_orde
-00000280: 7229 0272 1300 0000 7215 0000 00da 0969  r).r....r......i
+00000280: 7229 0272 1400 0000 7216 0000 00da 0969  r).r....r......i
 00000290: 735f 6163 7469 7665 da09 6973 5f73 7973  s_active..is_sys
-000002a0: 7465 6d29 0172 1100 0000 2902 da08 6162  tem).r....)...ab
+000002a0: 7465 6d29 0172 1200 0000 2902 da08 6162  tem).r....)...ab
 000002b0: 7374 7261 6374 da08 6f72 6465 7269 6e67  stract..ordering
 000002c0: 2903 da04 6e61 6d65 da06 6669 656c 6473  )...name..fields
 000002d0: da07 6f70 7469 6f6e 73da 0761 6363 6f75  ..options..accou
 000002e0: 6e74 da04 7479 7065 7a16 646a 6175 746f  nt..typez.djauto
 000002f0: 7461 736b 2e41 6363 6f75 6e74 5479 7065  task.AccountType
-00000300: 2904 7213 0000 0072 1500 0000 da09 6f6e  ).r....r......on
+00000300: 2904 7214 0000 0072 1600 0000 da09 6f6e  ).r....r......on
 00000310: 5f64 656c 6574 65da 0274 6f29 03da 0a6d  _delete..to)...m
-00000320: 6f64 656c 5f6e 616d 6572 1d00 0000 da05  odel_namer......
+00000320: 6f64 656c 5f6e 616d 6572 1e00 0000 da05  odel_namer......
 00000330: 6669 656c 644e 2916 da08 5f5f 6e61 6d65  fieldN)...__name
 00000340: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
 00000350: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
 00000360: 7065 6e64 656e 6369 6573 7202 0000 00da  pendenciesr.....
 00000370: 0b43 7265 6174 654d 6f64 656c 7203 0000  .CreateModelr...
 00000380: 00da 0941 7574 6f46 6965 6c64 da11 646a  ...AutoField..dj
 00000390: 616e 676f 5f65 7874 656e 7369 6f6e 73da  ango_extensions.
-000003a0: 0264 6272 1e00 0000 da15 4372 6561 7469  .dbr......Creati
+000003a0: 0264 6272 1f00 0000 da15 4372 6561 7469  .dbr......Creati
 000003b0: 6f6e 4461 7465 5469 6d65 4669 656c 64da  onDateTimeField.
 000003c0: 194d 6f64 6966 6963 6174 696f 6e44 6174  .ModificationDat
 000003d0: 6554 696d 6546 6965 6c64 da09 4368 6172  eTimeField..Char
 000003e0: 4669 656c 64da 0c42 6f6f 6c65 616e 4669  Field..BooleanFi
 000003f0: 656c 64da 1950 6f73 6974 6976 6553 6d61  eld..PositiveSma
 00000400: 6c6c 496e 7465 6765 7246 6965 6c64 da08  llIntegerField..
 00000410: 4164 6446 6965 6c64 da0a 466f 7265 6967  AddField..Foreig
 00000420: 6e4b 6579 da06 646a 616e 676f da08 6465  nKey..django..de
 00000430: 6c65 7469 6f6e da08 5345 545f 4e55 4c4c  letion..SET_NULL
-00000440: da0a 6f70 6572 6174 696f 6e73 a900 7239  ..operations..r9
-00000450: 0000 0072 3900 0000 fa62 2f68 6f6d 652f  ...r9....b/home/
+00000440: da0a 6f70 6572 6174 696f 6e73 a900 723a  ..operations..r:
+00000450: 0000 0072 3a00 0000 fa62 2f68 6f6d 652f  ...r:....b/home/
 00000460: 7275 6e6e 6572 2f77 6f72 6b2f 646a 616e  runner/work/djan
 00000470: 676f 2d61 7574 6f74 6173 6b2f 646a 616e  go-autotask/djan
 00000480: 676f 2d61 7574 6f74 6173 6b2f 646a 6175  go-autotask/djau
 00000490: 746f 7461 736b 2f6d 6967 7261 7469 6f6e  totask/migration
 000004a0: 732f 3030 3535 5f61 7574 6f5f 3230 3230  s/0055_auto_2020
 000004b0: 3033 3235 5f31 3333 352e 7079 7204 0000  0325_1335.pyr...
 000004c0: 0008 0000 0073 2e00 0000 0803 02ff 0405  .....s..........
 000004d0: 0401 0202 1401 1401 1401 1201 0e01 1001  ................
 000004e0: 0e01 0ef8 020b 0201 02fe 04f4 0411 0401  ................
 000004f0: 0201 0201 18fd 04ee 7204 0000 0029 08da  ........r....)..
 00000500: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
 00000510: 0300 0000 da19 646a 616e 676f 2e64 622e  ......django.db.
 00000520: 6d6f 6465 6c73 2e64 656c 6574 696f 6e72  models.deletionr
-00000530: 3500 0000 da1b 646a 616e 676f 5f65 7874  5.....django_ext
+00000530: 3600 0000 da1b 646a 616e 676f 5f65 7874  6.....django_ext
 00000540: 656e 7369 6f6e 732e 6462 2e66 6965 6c64  ensions.db.field
-00000550: 7372 2c00 0000 7204 0000 0072 3900 0000  sr,...r....r9...
-00000560: 7239 0000 0072 3900 0000 723a 0000 00da  r9...r9...r:....
+00000550: 7372 2d00 0000 7204 0000 0072 3a00 0000  sr-...r....r:...
+00000560: 723a 0000 0072 3a00 0000 723b 0000 00da  r:...r:...r;....
 00000570: 083c 6d6f 6475 6c65 3e03 0000 0073 0600  .<module>....s..
 00000580: 0000 1001 0801 0803                      ........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0057_auto_20200406_1620.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0057_auto_20200406_1620.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 728 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 d802 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 d802 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
@@ -10,39 +10,39 @@
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
 000000a0: 0564 0264 0365 066a 0764 0464 0564 0667  .d.d.e.j.d.d.d.g
 000000b0: 0264 0764 0464 088d 0464 098d 0365 046a  .d.d.d...d...e.j
 000000c0: 0564 0a64 0365 066a 0764 0464 0564 0667  .d.d.e.j.d.d.d.g
 000000d0: 0264 0764 0464 088d 0464 098d 0367 025a  .d.d.d...d...g.Z
 000000e0: 0864 0b53 0029 0cda 094d 6967 7261 7469  .d.S.)...Migrati
 000000f0: 6f6e 2902 da0a 646a 6175 746f 7461 736b  on)...djautotask
-00000100: 5a18 3030 3536 5f6d 6572 6765 5f32 3032  Z.0056_merge_202
-00000110: 3030 3332 375f 3130 3435 5a08 7461 736b  00327_1045Z.task
+00000100: da18 3030 3536 5f6d 6572 6765 5f32 3032  ..0056_merge_202
+00000110: 3030 3332 375f 3130 3435 da08 7461 736b  00327_1045..task
 00000120: 6e6f 7465 da07 7075 626c 6973 6854 2902  note..publishT).
 00000130: e901 0000 007a 1241 6c6c 2041 7574 6f74  .....z.All Autot
 00000140: 6173 6b20 5573 6572 7329 02e9 0200 0000  ask Users)......
 00000150: 7a15 496e 7465 726e 616c 2050 726f 6a65  z.Internal Proje
 00000160: 6374 2054 6561 6de9 1400 0000 2904 da05  ct Team.....)...
 00000170: 626c 616e 6bda 0763 686f 6963 6573 da0a  blank..choices..
 00000180: 6d61 785f 6c65 6e67 7468 da04 6e75 6c6c  max_length..null
 00000190: 2903 da0a 6d6f 6465 6c5f 6e61 6d65 da04  )...model_name..
-000001a0: 6e61 6d65 da05 6669 656c 645a 0a74 6963  name..fieldZ.tic
+000001a0: 6e61 6d65 da05 6669 656c 64da 0a74 6963  name..field..tic
 000001b0: 6b65 746e 6f74 654e 2909 da08 5f5f 6e61  ketnoteN)...__na
 000001c0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 000001d0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
 000001e0: 6465 7065 6e64 656e 6369 6573 7202 0000  dependenciesr...
 000001f0: 00da 0841 6464 4669 656c 6472 0300 0000  ...AddFieldr....
 00000200: da09 4368 6172 4669 656c 64da 0a6f 7065  ..CharField..ope
-00000210: 7261 7469 6f6e 73a9 0072 1800 0000 7218  rations..r....r.
+00000210: 7261 7469 6f6e 73a9 0072 1b00 0000 721b  rations..r....r.
 00000220: 0000 00fa 622f 686f 6d65 2f72 756e 6e65  ....b/home/runne
 00000230: 722f 776f 726b 2f64 6a61 6e67 6f2d 6175  r/work/django-au
 00000240: 746f 7461 736b 2f64 6a61 6e67 6f2d 6175  totask/django-au
 00000250: 746f 7461 736b 2f64 6a61 7574 6f74 6173  totask/djautotas
 00000260: 6b2f 6d69 6772 6174 696f 6e73 2f30 3035  k/migrations/005
 00000270: 375f 6175 746f 5f32 3032 3030 3430 365f  7_auto_20200406_
 00000280: 3136 3230 2e70 7972 0400 0000 0600 0000  1620.pyr........
 00000290: 731a 0000 0008 0302 ff04 0504 0102 0102  s...............
 000002a0: 0114 fd04 0504 0102 0102 0114 fd04 fa72  ...............r
 000002b0: 0400 0000 4e29 04da 0964 6a61 6e67 6f2e  ....N)...django.
 000002c0: 6462 7202 0000 0072 0300 0000 7204 0000  dbr....r....r...
-000002d0: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
-000002e0: 7219 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
+000002d0: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
+000002e0: 721c 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
 000002f0: 0000 0073 0200 0000 1003                 ...s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0058_auto_20200408_1022.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0081_project_department.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 717 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,52 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 cd02 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 4e02 0000  U.......2hLdN...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
-00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
-00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
-00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
-00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00000080: 0000 0a00 0000 4000 0000 7356 0000 0065  ......@...sV...e
-00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
-000000a0: 0564 0264 0365 066a 0764 0464 0564 0667  .d.d.e.j.d.d.d.g
-000000b0: 0264 0764 0464 088d 0464 098d 0365 046a  .d.d.d...d...e.j
-000000c0: 0564 0a64 0365 066a 0764 0464 0564 0667  .d.d.e.j.d.d.d.g
-000000d0: 0264 0764 0464 088d 0464 098d 0367 025a  .d.d.d...d...g.Z
-000000e0: 0864 0b53 0029 0cda 094d 6967 7261 7469  .d.S.)...Migrati
-000000f0: 6f6e 2902 da0a 646a 6175 746f 7461 736b  on)...djautotask
-00000100: da17 3030 3537 5f61 7574 6f5f 3230 3230  ..0057_auto_2020
-00000110: 3034 3036 5f31 3632 30da 0874 6173 6b6e  0406_1620..taskn
-00000120: 6f74 65da 0770 7562 6c69 7368 5429 02e9  ote..publishT)..
-00000130: 0100 0000 7a12 416c 6c20 4175 746f 7461  ....z.All Autota
-00000140: 736b 2055 7365 7273 2902 e902 0000 007a  sk Users)......z
-00000150: 0e49 6e74 6572 6e61 6c20 5573 6572 73e9  .Internal Users.
-00000160: 1400 0000 2904 da05 626c 616e 6bda 0763  ....)...blank..c
-00000170: 686f 6963 6573 da0a 6d61 785f 6c65 6e67  hoices..max_leng
-00000180: 7468 da04 6e75 6c6c 2903 da0a 6d6f 6465  th..null)...mode
-00000190: 6c5f 6e61 6d65 da04 6e61 6d65 da05 6669  l_name..name..fi
-000001a0: 656c 64da 0a74 6963 6b65 746e 6f74 654e  eld..ticketnoteN
-000001b0: 2909 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000001c0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000001d0: 6e61 6d65 5f5f da0c 6465 7065 6e64 656e  name__..dependen
-000001e0: 6369 6573 7202 0000 00da 0a41 6c74 6572  ciesr......Alter
-000001f0: 4669 656c 6472 0300 0000 da09 4368 6172  Fieldr......Char
-00000200: 4669 656c 64da 0a6f 7065 7261 7469 6f6e  Field..operation
-00000210: 73a9 0072 1b00 0000 721b 0000 00fa 622f  s..r....r.....b/
-00000220: 686f 6d65 2f72 756e 6e65 722f 776f 726b  home/runner/work
-00000230: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
-00000240: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
-00000250: 2f64 6a61 7574 6f74 6173 6b2f 6d69 6772  /djautotask/migr
-00000260: 6174 696f 6e73 2f30 3035 385f 6175 746f  ations/0058_auto
-00000270: 5f32 3032 3030 3430 385f 3130 3232 2e70  _20200408_1022.p
-00000280: 7972 0400 0000 0600 0000 731a 0000 0008  yr........s.....
-00000290: 0302 ff04 0504 0102 0102 0114 fd04 0504  ................
-000002a0: 0102 0102 0114 fd04 fa72 0400 0000 4e29  .........r....N)
-000002b0: 04da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
-000002c0: 0072 0300 0000 7204 0000 0072 1b00 0000  .r....r....r....
-000002d0: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
-000002e0: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
-000002f0: 0000 1003                                ....
+00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
+00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
+00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
+00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
+00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
+00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
+000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
+000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
+000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
+000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
+000000e0: 02da 0a64 6a61 7574 6f74 6173 6bda 6930  ...djautotask.i0
+000000f0: 3038 305f 6163 636f 756e 7470 6879 7369  080_accountphysi
+00000100: 6361 6c6c 6f63 6174 696f 6e74 7261 636b  callocationtrack
+00000110: 6572 5f61 6363 6f75 6e74 7472 6163 6b65  er_accounttracke
+00000120: 725f 6163 636f 756e 7474 7970 6574 7261  r_accounttypetra
+00000130: 636b 6572 5f61 6c6c 6f63 6174 696f 6e63  cker_allocationc
+00000140: 6f64 6574 7261 636b 6572 5f63 6f6e 7472  odetracker_contr
+00000150: 6163 7474 7261 636b da07 7072 6f6a 6563  acttrack..projec
+00000160: 74da 0a64 6570 6172 746d 656e 7454 7a15  t..departmentTz.
+00000170: 646a 6175 746f 7461 736b 2e64 6570 6172  djautotask.depar
+00000180: 746d 656e 7429 04da 0562 6c61 6e6b da04  tment)...blank..
+00000190: 6e75 6c6c da09 6f6e 5f64 656c 6574 65da  null..on_delete.
+000001a0: 0274 6f29 03da 0a6d 6f64 656c 5f6e 616d  .to)...model_nam
+000001b0: 65da 046e 616d 65da 0566 6965 6c64 4e29  e..name..fieldN)
+000001c0: 0dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000001d0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000001e0: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
+000001f0: 6965 7372 0200 0000 da08 4164 6446 6965  iesr......AddFie
+00000200: 6c64 7203 0000 00da 0a46 6f72 6569 676e  ldr......Foreign
+00000210: 4b65 79da 0664 6a61 6e67 6fda 0264 62da  Key..django..db.
+00000220: 0864 656c 6574 696f 6eda 0853 4554 5f4e  .deletion..SET_N
+00000230: 554c 4cda 0a6f 7065 7261 7469 6f6e 73a9  ULL..operations.
+00000240: 0072 1b00 0000 721b 0000 00fa 622f 686f  .r....r.....b/ho
+00000250: 6d65 2f72 756e 6e65 722f 776f 726b 2f64  me/runner/work/d
+00000260: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
+00000270: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
+00000280: 6a61 7574 6f74 6173 6b2f 6d69 6772 6174  jautotask/migrat
+00000290: 696f 6e73 2f30 3038 315f 7072 6f6a 6563  ions/0081_projec
+000002a0: 745f 6465 7061 7274 6d65 6e74 2e70 7972  t_department.pyr
+000002b0: 0400 0000 0700 0000 7310 0000 0008 0302  ........s.......
+000002c0: ff04 0504 0102 0102 0118 fd04 ff72 0400  .............r..
+000002d0: 0000 2906 da09 646a 616e 676f 2e64 6272  ..)...django.dbr
+000002e0: 0200 0000 7203 0000 00da 1964 6a61 6e67  ....r......djang
+000002f0: 6f2e 6462 2e6d 6f64 656c 732e 6465 6c65  o.db.models.dele
+00000300: 7469 6f6e 7216 0000 0072 0400 0000 721b  tionr....r....r.
+00000310: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
+00000320: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
+00000330: 7304 0000 0010 0108 03                   s........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0059_auto_20200414_1242.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0059_auto_20200414_1242.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 8223 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 1f20 0000  U.........Kd. ..
+00000000: 550d 0d0a 0000 0000 3268 4c64 1f20 0000  U.......2hLd. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0060_auto_20200414_1522.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0060_auto_20200414_1522.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 850 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 5203 0000  U.........KdR...
+00000000: 550d 0d0a 0000 0000 3268 4c64 5203 0000  U.......2hLdR...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
@@ -11,16 +11,16 @@
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
 000000c0: 6405 6406 6407 8d05 6408 8d03 6504 6a05  d.d.d...d...e.j.
 000000d0: 6402 6409 6506 6a07 6404 6404 6508 6a09  d.d.e.j.d.d.e.j.
 000000e0: 6a06 6a0a 6a0b 640a 6406 6407 8d05 6408  j.j.j.d.d.d...d.
 000000f0: 8d03 6702 5a0c 640b 5300 290c da09 4d69  ..g.Z.d.S.)...Mi
 00000100: 6772 6174 696f 6e29 02da 0a64 6a61 7574  gration)...djaut
-00000110: 6f74 6173 6b5a 1730 3035 395f 6175 746f  otaskZ.0059_auto
-00000120: 5f32 3032 3030 3431 345f 3132 3432 5a0b  _20200414_1242Z.
+00000110: 6f74 6173 6bda 1730 3035 395f 6175 746f  otask..0059_auto
+00000120: 5f32 3032 3030 3431 345f 3132 3432 da0b  _20200414_1242..
 00000130: 7365 7276 6963 6563 616c 6cda 1463 616e  servicecall..can
 00000140: 6365 6c65 645f 6279 5f72 6573 6f75 7263  celed_by_resourc
 00000150: 6554 da17 6361 6e63 656c 6c65 645f 7365  eT..cancelled_se
 00000160: 7276 6963 655f 6361 6c6c 737a 1364 6a61  rvice_callsz.dja
 00000170: 7574 6f74 6173 6b2e 5265 736f 7572 6365  utotask.Resource
 00000180: 2905 da05 626c 616e 6bda 046e 756c 6cda  )...blank..null.
 00000190: 096f 6e5f 6465 6c65 7465 da0c 7265 6c61  .on_delete..rela
@@ -33,24 +33,24 @@
 00000200: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 00000210: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
 00000220: 6e63 6965 7372 0200 0000 da0a 416c 7465  nciesr......Alte
 00000230: 7246 6965 6c64 7203 0000 00da 0a46 6f72  rFieldr......For
 00000240: 6569 676e 4b65 79da 0664 6a61 6e67 6fda  eignKey..django.
 00000250: 0264 62da 0864 656c 6574 696f 6eda 0853  .db..deletion..S
 00000260: 4554 5f4e 554c 4cda 0a6f 7065 7261 7469  ET_NULL..operati
-00000270: 6f6e 73a9 0072 1d00 0000 721d 0000 00fa  ons..r....r.....
+00000270: 6f6e 73a9 0072 1f00 0000 721f 0000 00fa  ons..r....r.....
 00000280: 622f 686f 6d65 2f72 756e 6e65 722f 776f  b/home/runner/wo
 00000290: 726b 2f64 6a61 6e67 6f2d 6175 746f 7461  rk/django-autota
 000002a0: 736b 2f64 6a61 6e67 6f2d 6175 746f 7461  sk/django-autota
 000002b0: 736b 2f64 6a61 7574 6f74 6173 6b2f 6d69  sk/djautotask/mi
 000002c0: 6772 6174 696f 6e73 2f30 3036 305f 6175  grations/0060_au
 000002d0: 746f 5f32 3032 3030 3431 345f 3135 3232  to_20200414_1522
 000002e0: 2e70 7972 0400 0000 0700 0000 731a 0000  .pyr........s...
 000002f0: 0008 0302 ff04 0504 0102 0102 011a fd04  ................
 00000300: 0504 0102 0102 011a fd04 fa72 0400 0000  ...........r....
 00000310: 2906 da09 646a 616e 676f 2e64 6272 0200  )...django.dbr..
 00000320: 0000 7203 0000 00da 1964 6a61 6e67 6f2e  ..r......django.
 00000330: 6462 2e6d 6f64 656c 732e 6465 6c65 7469  db.models.deleti
-00000340: 6f6e 7218 0000 0072 0400 0000 721d 0000  onr....r....r...
-00000350: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00000340: 6f6e 721a 0000 0072 0400 0000 721f 0000  onr....r....r...
+00000350: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
 00000360: da08 3c6d 6f64 756c 653e 0300 0000 7304  ..<module>....s.
 00000370: 0000 0010 0108 03                        .......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0061_auto_20200416_1241.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0061_auto_20200416_1241.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 410 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 9a01 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 9a01 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0500 0000 4000 0000 7328  ..........@...s(
 00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
 00000090: 0365 046a 0564 0264 0364 0464 059c 0264  .e.j.d.d.d.d...d
 000000a0: 068d 0267 015a 0664 0753 0029 08da 094d  ...g.Z.d.S.)...M
 000000b0: 6967 7261 7469 6f6e 2902 da0a 646a 6175  igration)...djau
-000000c0: 746f 7461 736b da17 3030 3630 5f61 7574  totask..0060_aut
+000000c0: 746f 7461 736b 5a17 3030 3630 5f61 7574  totaskZ.0060_aut
 000000d0: 6f5f 3230 3230 3034 3134 5f31 3532 32da  o_20200414_1522.
 000000e0: 1173 6572 7669 6365 6361 6c6c 7374 6174  .servicecallstat
 000000f0: 7573 2901 da05 6c61 6265 6c7a 1553 6572  us)...labelz.Ser
 00000100: 7669 6365 2063 616c 6c20 7374 6174 7573  vice call status
 00000110: 6573 2902 da08 6f72 6465 7269 6e67 da13  es)...ordering..
 00000120: 7665 7262 6f73 655f 6e61 6d65 5f70 6c75  verbose_name_plu
 00000130: 7261 6c29 02da 046e 616d 65da 076f 7074  ral)...name..opt
 00000140: 696f 6e73 4e29 07da 085f 5f6e 616d 655f  ionsN)...__name_
 00000150: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 00000160: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
 00000170: 656e 6465 6e63 6965 7372 0200 0000 da11  endenciesr......
 00000180: 416c 7465 724d 6f64 656c 4f70 7469 6f6e  AlterModelOption
 00000190: 73da 0a6f 7065 7261 7469 6f6e 73a9 0072  s..operations..r
-000001a0: 1200 0000 7212 0000 00fa 622f 686f 6d65  ....r.....b/home
+000001a0: 1100 0000 7211 0000 00fa 622f 686f 6d65  ....r.....b/home
 000001b0: 2f72 756e 6e65 722f 776f 726b 2f64 6a61  /runner/work/dja
 000001c0: 6e67 6f2d 6175 746f 7461 736b 2f64 6a61  ngo-autotask/dja
 000001d0: 6e67 6f2d 6175 746f 7461 736b 2f64 6a61  ngo-autotask/dja
 000001e0: 7574 6f74 6173 6b2f 6d69 6772 6174 696f  utotask/migratio
 000001f0: 6e73 2f30 3036 315f 6175 746f 5f32 3032  ns/0061_auto_202
 00000200: 3030 3431 365f 3132 3431 2e70 7972 0300  00416_1241.pyr..
 00000210: 0000 0600 0000 730e 0000 0008 0302 ff04  ......s.........
 00000220: 0504 0102 0108 fe04 ff72 0300 0000 4e29  .........r....N)
 00000230: 03da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
-00000240: 0072 0300 0000 7212 0000 0072 1200 0000  .r....r....r....
-00000250: 7212 0000 0072 1300 0000 da08 3c6d 6f64  r....r......<mod
+00000240: 0072 0300 0000 7211 0000 0072 1100 0000  .r....r....r....
+00000250: 7211 0000 0072 1200 0000 da08 3c6d 6f64  r....r......<mod
 00000260: 756c 653e 0300 0000 7302 0000 000c 03    ule>....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0062_task_department.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0062_task_department.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 506 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 fa01 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 fa01 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0063_accountphysicallocation.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0063_accountphysicallocation.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 822 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 3603 0000  U.........Kd6...
+00000000: 550d 0d0a 0000 0000 3268 4c64 3603 0000  U.......2hLd6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0064_auto_20200511_1124.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0064_auto_20200511_1124.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1330 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 3205 0000  U.........Kd2...
+00000000: 550d 0d0a 0000 0000 3268 4c64 3205 0000  U.......2hLd2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0064_servicecall_location.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0064_servicecall_location.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 529 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 1102 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 1102 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
 00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
 00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
 000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
 000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
-000000e0: 02da 0a64 6a61 7574 6f74 6173 6bda 1c30  ...djautotask..0
+000000e0: 02da 0a64 6a61 7574 6f74 6173 6b5a 1c30  ...djautotaskZ.0
 000000f0: 3036 335f 6163 636f 756e 7470 6879 7369  063_accountphysi
 00000100: 6361 6c6c 6f63 6174 696f 6eda 0b73 6572  callocation..ser
 00000110: 7669 6365 6361 6c6c da08 6c6f 6361 7469  vicecall..locati
 00000120: 6f6e 547a 2264 6a61 7574 6f74 6173 6b2e  onTz"djautotask.
 00000130: 4163 636f 756e 7450 6879 7369 6361 6c4c  AccountPhysicalL
 00000140: 6f63 6174 696f 6e29 04da 0562 6c61 6e6b  ocation)...blank
 00000150: da04 6e75 6c6c da09 6f6e 5f64 656c 6574  ..null..on_delet
@@ -26,23 +26,23 @@
 00000190: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 000001a0: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
 000001b0: 6e63 6965 7372 0200 0000 da08 4164 6446  nciesr......AddF
 000001c0: 6965 6c64 7203 0000 00da 0a46 6f72 6569  ieldr......Forei
 000001d0: 676e 4b65 79da 0664 6a61 6e67 6fda 0264  gnKey..django..d
 000001e0: 62da 0864 656c 6574 696f 6eda 0853 4554  b..deletion..SET
 000001f0: 5f4e 554c 4cda 0a6f 7065 7261 7469 6f6e  _NULL..operation
-00000200: 73a9 0072 1b00 0000 721b 0000 00fa 642f  s..r....r.....d/
+00000200: 73a9 0072 1a00 0000 721a 0000 00fa 642f  s..r....r.....d/
 00000210: 686f 6d65 2f72 756e 6e65 722f 776f 726b  home/runner/work
 00000220: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
 00000230: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
 00000240: 2f64 6a61 7574 6f74 6173 6b2f 6d69 6772  /djautotask/migr
 00000250: 6174 696f 6e73 2f30 3036 345f 7365 7276  ations/0064_serv
 00000260: 6963 6563 616c 6c5f 6c6f 6361 7469 6f6e  icecall_location
 00000270: 2e70 7972 0400 0000 0700 0000 7310 0000  .pyr........s...
 00000280: 0008 0302 ff04 0504 0102 0102 0118 fd04  ................
 00000290: ff72 0400 0000 2906 da09 646a 616e 676f  .r....)...django
 000002a0: 2e64 6272 0200 0000 7203 0000 00da 1964  .dbr....r......d
 000002b0: 6a61 6e67 6f2e 6462 2e6d 6f64 656c 732e  jango.db.models.
-000002c0: 6465 6c65 7469 6f6e 7216 0000 0072 0400  deletionr....r..
-000002d0: 0000 721b 0000 0072 1b00 0000 721b 0000  ..r....r....r...
-000002e0: 0072 1c00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000002c0: 6465 6c65 7469 6f6e 7215 0000 0072 0400  deletionr....r..
+000002d0: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+000002e0: 0072 1b00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
 000002f0: 0300 0000 7304 0000 0010 0108 03         ....s........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0065_auto_20200512_1224.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0065_auto_20200512_1224.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 643 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 8302 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 8302 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0066_auto_20200512_1420.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0066_auto_20200512_1420.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 442 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 ba01 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 ba01 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
 00000080: 0000 0900 0000 4000 0000 7332 0000 0065  ......@...s2...e
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
 000000a0: 0564 0264 0365 066a 0764 0464 0564 0664  .d.d.e.j.d.d.d.d
 000000b0: 0464 078d 0464 088d 0367 015a 0864 0953  .d...d...g.Z.d.S
 000000c0: 0029 0ada 094d 6967 7261 7469 6f6e 2902  .)...Migration).
-000000d0: da0a 646a 6175 746f 7461 736b 5a17 3030  ..djautotaskZ.00
+000000d0: da0a 646a 6175 746f 7461 736b da17 3030  ..djautotask..00
 000000e0: 3635 5f61 7574 6f5f 3230 3230 3035 3132  65_auto_20200512
 000000f0: 5f31 3232 34da 0674 6963 6b65 74da 0f65  _1224..ticket..e
 00000100: 7374 696d 6174 6564 5f68 6f75 7273 54e9  stimated_hoursT.
 00000110: 0200 0000 e909 0000 0029 04da 0562 6c61  .........)...bla
 00000120: 6e6b da0e 6465 6369 6d61 6c5f 706c 6163  nk..decimal_plac
 00000130: 6573 da0a 6d61 785f 6469 6769 7473 da04  es..max_digits..
 00000140: 6e75 6c6c 2903 da0a 6d6f 6465 6c5f 6e61  null)...model_na
 00000150: 6d65 da04 6e61 6d65 da05 6669 656c 644e  me..name..fieldN
 00000160: 2909 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 00000170: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000180: 6e61 6d65 5f5f da0c 6465 7065 6e64 656e  name__..dependen
 00000190: 6369 6573 7202 0000 00da 0a41 6c74 6572  ciesr......Alter
 000001a0: 4669 656c 6472 0300 0000 da0c 4465 6369  Fieldr......Deci
 000001b0: 6d61 6c46 6965 6c64 da0a 6f70 6572 6174  malField..operat
-000001c0: 696f 6e73 a900 7218 0000 0072 1800 0000  ions..r....r....
+000001c0: 696f 6e73 a900 7219 0000 0072 1900 0000  ions..r....r....
 000001d0: fa62 2f68 6f6d 652f 7275 6e6e 6572 2f77  .b/home/runner/w
 000001e0: 6f72 6b2f 646a 616e 676f 2d61 7574 6f74  ork/django-autot
 000001f0: 6173 6b2f 646a 616e 676f 2d61 7574 6f74  ask/django-autot
 00000200: 6173 6b2f 646a 6175 746f 7461 736b 2f6d  ask/djautotask/m
 00000210: 6967 7261 7469 6f6e 732f 3030 3636 5f61  igrations/0066_a
 00000220: 7574 6f5f 3230 3230 3035 3132 5f31 3432  uto_20200512_142
 00000230: 302e 7079 7204 0000 0006 0000 0073 1000  0.pyr........s..
 00000240: 0000 0803 02ff 0405 0401 0201 0201 10fd  ................
 00000250: 04ff 7204 0000 004e 2904 da09 646a 616e  ..r....N)...djan
 00000260: 676f 2e64 6272 0200 0000 7203 0000 0072  go.dbr....r....r
-00000270: 0400 0000 7218 0000 0072 1800 0000 7218  ....r....r....r.
-00000280: 0000 0072 1900 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000270: 0400 0000 7219 0000 0072 1900 0000 7219  ....r....r....r.
+00000280: 0000 0072 1a00 0000 da08 3c6d 6f64 756c  ...r......<modul
 00000290: 653e 0300 0000 7302 0000 0010 03         e>....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0067_auto_20200519_1100.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0067_auto_20200519_1100.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 835 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 4303 0000  U.........KdC...
+00000000: 550d 0d0a 0000 0000 3268 4c64 4303 0000  U.......2hLdC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
@@ -10,46 +10,46 @@
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
 000000a0: 0564 0264 0365 066a 0764 0464 0464 058d  .d.d.e.j.d.d.d..
 000000b0: 0264 068d 0365 046a 0564 0264 0765 066a  .d...e.j.d.d.e.j
 000000c0: 0864 0864 098d 0164 068d 0365 046a 0564  .d.d...d...e.j.d
 000000d0: 0264 0a65 066a 0964 0464 0b64 0c64 0464  .d.e.j.d.d.d.d.d
 000000e0: 0d8d 0464 068d 0367 035a 0a64 0e53 0029  ...d...g.Z.d.S.)
 000000f0: 0fda 094d 6967 7261 7469 6f6e 2902 da0a  ...Migration)...
-00000100: 646a 6175 746f 7461 736b 5a17 3030 3636  djautotaskZ.0066
+00000100: 646a 6175 746f 7461 736b da17 3030 3636  djautotask..0066
 00000110: 5f61 7574 6f5f 3230 3230 3035 3132 5f31  _auto_20200512_1
 00000120: 3432 30da 0674 6963 6b65 74da 1773 6572  420..ticket..ser
 00000130: 7669 6365 5f6c 6576 656c 5f61 6772 6565  vice_level_agree
 00000140: 6d65 6e74 5429 02da 0562 6c61 6e6b da04  mentT)...blank..
 00000150: 6e75 6c6c 2903 da0a 6d6f 6465 6c5f 6e61  null)...model_na
 00000160: 6d65 da04 6e61 6d65 da05 6669 656c 64da  me..name..field.
 00000170: 2473 6572 7669 6365 5f6c 6576 656c 5f61  $service_level_a
 00000180: 6772 6565 6d65 6e74 5f68 6173 5f62 6565  greement_has_bee
 00000190: 6e5f 6d65 7446 2901 da07 6465 6661 756c  n_metF)...defaul
 000001a0: 74da 2f73 6572 7669 6365 5f6c 6576 656c  t./service_level
 000001b0: 5f61 6772 6565 6d65 6e74 5f70 6175 7365  _agreement_pause
 000001c0: 645f 6e65 7874 5f65 7665 6e74 5f68 6f75  d_next_event_hou
-000001d0: 7273 e902 0000 00e9 0900 0000 2904 7208  rs..........).r.
+000001d0: 7273 e902 0000 00e9 0900 0000 2904 7209  rs..........).r.
 000001e0: 0000 00da 0e64 6563 696d 616c 5f70 6c61  .....decimal_pla
 000001f0: 6365 73da 0a6d 6178 5f64 6967 6974 7372  ces..max_digitsr
-00000200: 0900 0000 4e29 0bda 085f 5f6e 616d 655f  ....N)...__name_
+00000200: 0a00 0000 4e29 0bda 085f 5f6e 616d 655f  ....N)...__name_
 00000210: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 00000220: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
 00000230: 656e 6465 6e63 6965 7372 0200 0000 da08  endenciesr......
 00000240: 4164 6446 6965 6c64 7203 0000 00da 0c49  AddFieldr......I
 00000250: 6e74 6567 6572 4669 656c 64da 0c42 6f6f  ntegerField..Boo
 00000260: 6c65 616e 4669 656c 64da 0c44 6563 696d  leanField..Decim
 00000270: 616c 4669 656c 64da 0a6f 7065 7261 7469  alField..operati
-00000280: 6f6e 73a9 0072 1d00 0000 721d 0000 00fa  ons..r....r.....
+00000280: 6f6e 73a9 0072 1e00 0000 721e 0000 00fa  ons..r....r.....
 00000290: 622f 686f 6d65 2f72 756e 6e65 722f 776f  b/home/runner/wo
 000002a0: 726b 2f64 6a61 6e67 6f2d 6175 746f 7461  rk/django-autota
 000002b0: 736b 2f64 6a61 6e67 6f2d 6175 746f 7461  sk/django-autota
 000002c0: 736b 2f64 6a61 7574 6f74 6173 6b2f 6d69  sk/djautotask/mi
 000002d0: 6772 6174 696f 6e73 2f30 3036 375f 6175  grations/0067_au
 000002e0: 746f 5f32 3032 3030 3531 395f 3131 3030  to_20200519_1100
 000002f0: 2e70 7972 0400 0000 0600 0000 7324 0000  .pyr........s$..
 00000300: 0008 0302 ff04 0504 0102 0102 010c fd04  ................
 00000310: 0504 0102 0102 010a fd04 0504 0102 0102  ................
 00000320: 0110 fd04 f572 0400 0000 4e29 04da 0964  .....r....N)...d
 00000330: 6a61 6e67 6f2e 6462 7202 0000 0072 0300  jango.dbr....r..
-00000340: 0000 7204 0000 0072 1d00 0000 721d 0000  ..r....r....r...
-00000350: 0072 1d00 0000 721e 0000 00da 083c 6d6f  .r....r......<mo
+00000340: 0000 7204 0000 0072 1e00 0000 721e 0000  ..r....r....r...
+00000350: 0072 1e00 0000 721f 0000 00da 083c 6d6f  .r....r......<mo
 00000360: 6475 6c65 3e03 0000 0073 0200 0000 1003  dule>....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0069_auto_20200602_1419.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0069_auto_20200602_1419.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 777 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 0903 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 0903 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
@@ -12,41 +12,41 @@
 000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
 000000c0: 6405 6406 8d04 6407 8d03 6504 6a05 6408  d.d...d...e.j.d.
 000000d0: 6403 6506 6a07 6404 6404 6508 6a09 6a06  d.e.j.d.d.e.j.j.
 000000e0: 6a0a 6a0b 6405 6406 8d04 6407 8d03 6702  j.j.d.d...d...g.
 000000f0: 5a0c 6409 5300 290a da09 4d69 6772 6174  Z.d.S.)...Migrat
 00000100: 696f 6e29 02da 0a64 6a61 7574 6f74 6173  ion)...djautotas
 00000110: 6bda 1830 3036 385f 6d65 7267 655f 3230  k..0068_merge_20
-00000120: 3230 3035 3231 5f31 3631 355a 0f73 6572  200521_1615Z.ser
+00000120: 3230 3035 3231 5f31 3631 35da 0f73 6572  200521_1615..ser
 00000130: 7669 6365 6361 6c6c 7461 736b da0c 7365  vicecalltask..se
 00000140: 7276 6963 655f 6361 6c6c 547a 1664 6a61  rvice_callTz.dja
 00000150: 7574 6f74 6173 6b2e 5365 7276 6963 6543  utotask.ServiceC
 00000160: 616c 6c29 04da 0562 6c61 6e6b da04 6e75  all)...blank..nu
 00000170: 6c6c da09 6f6e 5f64 656c 6574 65da 0274  ll..on_delete..t
 00000180: 6f29 03da 0a6d 6f64 656c 5f6e 616d 65da  o)...model_name.
-00000190: 046e 616d 65da 0566 6965 6c64 5a11 7365  .name..fieldZ.se
+00000190: 046e 616d 65da 0566 6965 6c64 da11 7365  .name..field..se
 000001a0: 7276 6963 6563 616c 6c74 6963 6b65 744e  rvicecallticketN
 000001b0: 290d da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 000001c0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 000001d0: 6e61 6d65 5f5f da0c 6465 7065 6e64 656e  name__..dependen
 000001e0: 6369 6573 7202 0000 00da 0a41 6c74 6572  ciesr......Alter
 000001f0: 4669 656c 6472 0300 0000 da0a 466f 7265  Fieldr......Fore
 00000200: 6967 6e4b 6579 da06 646a 616e 676f da02  ignKey..django..
 00000210: 6462 da08 6465 6c65 7469 6f6e da08 5345  db..deletion..SE
 00000220: 545f 4e55 4c4c da0a 6f70 6572 6174 696f  T_NULL..operatio
-00000230: 6e73 a900 721a 0000 0072 1a00 0000 fa62  ns..r....r.....b
+00000230: 6e73 a900 721c 0000 0072 1c00 0000 fa62  ns..r....r.....b
 00000240: 2f68 6f6d 652f 7275 6e6e 6572 2f77 6f72  /home/runner/wor
 00000250: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
 00000260: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
 00000270: 6b2f 646a 6175 746f 7461 736b 2f6d 6967  k/djautotask/mig
 00000280: 7261 7469 6f6e 732f 3030 3639 5f61 7574  rations/0069_aut
 00000290: 6f5f 3230 3230 3036 3032 5f31 3431 392e  o_20200602_1419.
 000002a0: 7079 7204 0000 0007 0000 0073 1a00 0000  pyr........s....
 000002b0: 0803 02ff 0405 0401 0201 0201 18fd 0405  ................
 000002c0: 0401 0201 0201 18fd 04fa 7204 0000 0029  ..........r....)
 000002d0: 06da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
 000002e0: 0072 0300 0000 da19 646a 616e 676f 2e64  .r......django.d
 000002f0: 622e 6d6f 6465 6c73 2e64 656c 6574 696f  b.models.deletio
-00000300: 6e72 1500 0000 7204 0000 0072 1a00 0000  nr....r....r....
-00000310: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
+00000300: 6e72 1700 0000 7204 0000 0072 1c00 0000  nr....r....r....
+00000310: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
 00000320: 083c 6d6f 6475 6c65 3e03 0000 0073 0400  .<module>....s..
 00000330: 0000 1001 0803                           ......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0070_auto_20200714_0807.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0070_auto_20200714_0807.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 412 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 9c01 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 9c01 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0071_project_status_detail.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0071_project_status_detail.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 421 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 a501 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 a501 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
 00000080: 0000 0800 0000 4000 0000 7330 0000 0065  ......@...s0...e
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
 000000a0: 0564 0264 0365 066a 0764 0464 0564 0464  .d.d.e.j.d.d.d.d
 000000b0: 068d 0364 078d 0367 015a 0864 0853 0029  ...d...g.Z.d.S.)
 000000c0: 09da 094d 6967 7261 7469 6f6e 2902 da0a  ...Migration)...
-000000d0: 646a 6175 746f 7461 736b 5a17 3030 3730  djautotaskZ.0070
+000000d0: 646a 6175 746f 7461 736b da17 3030 3730  djautotask..0070
 000000e0: 5f61 7574 6f5f 3230 3230 3037 3134 5f30  _auto_20200714_0
 000000f0: 3830 37da 0770 726f 6a65 6374 da0d 7374  807..project..st
 00000100: 6174 7573 5f64 6574 6169 6c54 69d0 0700  atus_detailTi...
 00000110: 0029 03da 0562 6c61 6e6b da0a 6d61 785f  .)...blank..max_
 00000120: 6c65 6e67 7468 da04 6e75 6c6c 2903 da0a  length..null)...
 00000130: 6d6f 6465 6c5f 6e61 6d65 da04 6e61 6d65  model_name..name
 00000140: da05 6669 656c 644e 2909 da08 5f5f 6e61  ..fieldN)...__na
 00000150: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 00000160: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
 00000170: 6465 7065 6e64 656e 6369 6573 7202 0000  dependenciesr...
 00000180: 00da 0841 6464 4669 656c 6472 0300 0000  ...AddFieldr....
 00000190: da09 4368 6172 4669 656c 64da 0a6f 7065  ..CharField..ope
-000001a0: 7261 7469 6f6e 73a9 0072 1500 0000 7215  rations..r....r.
+000001a0: 7261 7469 6f6e 73a9 0072 1600 0000 7216  rations..r....r.
 000001b0: 0000 00fa 652f 686f 6d65 2f72 756e 6e65  ....e/home/runne
 000001c0: 722f 776f 726b 2f64 6a61 6e67 6f2d 6175  r/work/django-au
 000001d0: 746f 7461 736b 2f64 6a61 6e67 6f2d 6175  totask/django-au
 000001e0: 746f 7461 736b 2f64 6a61 7574 6f74 6173  totask/djautotas
 000001f0: 6b2f 6d69 6772 6174 696f 6e73 2f30 3037  k/migrations/007
 00000200: 315f 7072 6f6a 6563 745f 7374 6174 7573  1_project_status
 00000210: 5f64 6574 6169 6c2e 7079 7204 0000 0006  _detail.pyr.....
 00000220: 0000 0073 1000 0000 0803 02ff 0405 0401  ...s............
 00000230: 0201 0201 0efd 04ff 7204 0000 004e 2904  ........r....N).
 00000240: da09 646a 616e 676f 2e64 6272 0200 0000  ..django.dbr....
-00000250: 7203 0000 0072 0400 0000 7215 0000 0072  r....r....r....r
-00000260: 1500 0000 7215 0000 0072 1600 0000 da08  ....r....r......
+00000250: 7203 0000 0072 0400 0000 7216 0000 0072  r....r....r....r
+00000260: 1600 0000 7216 0000 0072 1700 0000 da08  ....r....r......
 00000270: 3c6d 6f64 756c 653e 0300 0000 7302 0000  <module>....s...
 00000280: 0010 03                                  ...
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0072_account_parent_account.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0072_account_parent_account.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 513 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 0102 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 0102 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
 00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
 00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
 000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
 000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
-000000e0: 02da 0a64 6a61 7574 6f74 6173 6bda 1a30  ...djautotask..0
+000000e0: 02da 0a64 6a61 7574 6f74 6173 6b5a 1a30  ...djautotaskZ.0
 000000f0: 3037 315f 7072 6f6a 6563 745f 7374 6174  071_project_stat
 00000100: 7573 5f64 6574 6169 6cda 0761 6363 6f75  us_detail..accou
 00000110: 6e74 da0e 7061 7265 6e74 5f61 6363 6f75  nt..parent_accou
 00000120: 6e74 547a 1264 6a61 7574 6f74 6173 6b2e  ntTz.djautotask.
 00000130: 4163 636f 756e 7429 04da 0562 6c61 6e6b  Account)...blank
 00000140: da04 6e75 6c6c da09 6f6e 5f64 656c 6574  ..null..on_delet
 00000150: 65da 0274 6f29 03da 0a6d 6f64 656c 5f6e  e..to)...model_n
@@ -25,23 +25,23 @@
 00000180: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 00000190: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
 000001a0: 6e63 6965 7372 0200 0000 da08 4164 6446  nciesr......AddF
 000001b0: 6965 6c64 7203 0000 00da 0a46 6f72 6569  ieldr......Forei
 000001c0: 676e 4b65 79da 0664 6a61 6e67 6fda 0264  gnKey..django..d
 000001d0: 62da 0864 656c 6574 696f 6eda 0853 4554  b..deletion..SET
 000001e0: 5f4e 554c 4cda 0a6f 7065 7261 7469 6f6e  _NULL..operation
-000001f0: 73a9 0072 1b00 0000 721b 0000 00fa 662f  s..r....r.....f/
+000001f0: 73a9 0072 1a00 0000 721a 0000 00fa 662f  s..r....r.....f/
 00000200: 686f 6d65 2f72 756e 6e65 722f 776f 726b  home/runner/work
 00000210: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
 00000220: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
 00000230: 2f64 6a61 7574 6f74 6173 6b2f 6d69 6772  /djautotask/migr
 00000240: 6174 696f 6e73 2f30 3037 325f 6163 636f  ations/0072_acco
 00000250: 756e 745f 7061 7265 6e74 5f61 6363 6f75  unt_parent_accou
 00000260: 6e74 2e70 7972 0400 0000 0700 0000 7310  nt.pyr........s.
 00000270: 0000 0008 0302 ff04 0504 0102 0102 0118  ................
 00000280: fd04 ff72 0400 0000 2906 da09 646a 616e  ...r....)...djan
 00000290: 676f 2e64 6272 0200 0000 7203 0000 00da  go.dbr....r.....
 000002a0: 1964 6a61 6e67 6f2e 6462 2e6d 6f64 656c  .django.db.model
-000002b0: 732e 6465 6c65 7469 6f6e 7216 0000 0072  s.deletionr....r
-000002c0: 0400 0000 721b 0000 0072 1b00 0000 721b  ....r....r....r.
-000002d0: 0000 0072 1c00 0000 da08 3c6d 6f64 756c  ...r......<modul
+000002b0: 732e 6465 6c65 7469 6f6e 7215 0000 0072  s.deletionr....r
+000002c0: 0400 0000 721a 0000 0072 1a00 0000 721a  ....r....r....r.
+000002d0: 0000 0072 1b00 0000 da08 3c6d 6f64 756c  ...r......<modul
 000002e0: 653e 0300 0000 7304 0000 0010 0108 03    e>....s........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0073_syncjob_skipped.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0103_auto_20220106_1622.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 401 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 9101 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 8701 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
 00000080: 0000 0600 0000 4000 0000 732c 0000 0065  ......@...s,...e
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
 000000a0: 0564 0264 0365 066a 0764 0464 058d 0164  .d.d.e.j.d.d...d
 000000b0: 068d 0367 015a 0864 0753 0029 08da 094d  ...g.Z.d.S.)...M
 000000c0: 6967 7261 7469 6f6e 2902 da0a 646a 6175  igration)...djau
-000000d0: 746f 7461 736b 5a1b 3030 3732 5f61 6363  totaskZ.0072_acc
-000000e0: 6f75 6e74 5f70 6172 656e 745f 6163 636f  ount_parent_acco
-000000f0: 756e 745a 0773 796e 636a 6f62 da07 736b  untZ.syncjob..sk
-00000100: 6970 7065 6454 2901 da04 6e75 6c6c 2903  ippedT)...null).
-00000110: da0a 6d6f 6465 6c5f 6e61 6d65 da04 6e61  ..model_name..na
-00000120: 6d65 da05 6669 656c 644e 2909 da08 5f5f  me..fieldN)...__
-00000130: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000140: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000150: da0c 6465 7065 6e64 656e 6369 6573 7202  ..dependenciesr.
-00000160: 0000 00da 0841 6464 4669 656c 6472 0300  .....AddFieldr..
-00000170: 0000 da14 506f 7369 7469 7665 496e 7465  ....PositiveInte
-00000180: 6765 7246 6965 6c64 da0a 6f70 6572 6174  gerField..operat
-00000190: 696f 6e73 a900 7212 0000 0072 1200 0000  ions..r....r....
-000001a0: fa5f 2f68 6f6d 652f 7275 6e6e 6572 2f77  ._/home/runner/w
-000001b0: 6f72 6b2f 646a 616e 676f 2d61 7574 6f74  ork/django-autot
-000001c0: 6173 6b2f 646a 616e 676f 2d61 7574 6f74  ask/django-autot
-000001d0: 6173 6b2f 646a 6175 746f 7461 736b 2f6d  ask/djautotask/m
-000001e0: 6967 7261 7469 6f6e 732f 3030 3733 5f73  igrations/0073_s
-000001f0: 796e 636a 6f62 5f73 6b69 7070 6564 2e70  yncjob_skipped.p
-00000200: 7972 0400 0000 0600 0000 7310 0000 0008  yr........s.....
-00000210: 0302 ff04 0504 0102 0102 010a fd04 ff72  ...............r
-00000220: 0400 0000 4e29 04da 0964 6a61 6e67 6f2e  ....N)...django.
-00000230: 6462 7202 0000 0072 0300 0000 7204 0000  dbr....r....r...
-00000240: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
-00000250: 7213 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
-00000260: 0000 0073 0200 0000 1003                 ...s......
+000000d0: 746f 7461 736b da17 3031 3032 5f61 7574  totask..0102_aut
+000000e0: 6f5f 3230 3232 3031 3034 5f31 3635 35da  o_20220104_1655.
+000000f0: 0872 6573 6f75 7263 65da 0565 6d61 696c  .resource..email
+00000100: e9fa 0000 0029 01da 0a6d 6178 5f6c 656e  .....)...max_len
+00000110: 6774 6829 03da 0a6d 6f64 656c 5f6e 616d  gth)...model_nam
+00000120: 65da 046e 616d 65da 0566 6965 6c64 4e29  e..name..fieldN)
+00000130: 09da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000140: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000150: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
+00000160: 6965 7372 0200 0000 da0a 416c 7465 7246  iesr......AlterF
+00000170: 6965 6c64 7203 0000 00da 0943 6861 7246  ieldr......CharF
+00000180: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
+00000190: a900 7215 0000 0072 1500 0000 fa62 2f68  ..r....r.....b/h
+000001a0: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
+000001b0: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
+000001c0: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
+000001d0: 646a 6175 746f 7461 736b 2f6d 6967 7261  djautotask/migra
+000001e0: 7469 6f6e 732f 3031 3033 5f61 7574 6f5f  tions/0103_auto_
+000001f0: 3230 3232 3031 3036 5f31 3632 322e 7079  20220106_1622.py
+00000200: 7204 0000 0006 0000 0073 1000 0000 0803  r........s......
+00000210: 02ff 0405 0401 0201 0201 0afd 04ff 7204  ..............r.
+00000220: 0000 004e 2904 da09 646a 616e 676f 2e64  ...N)...django.d
+00000230: 6272 0200 0000 7203 0000 0072 0400 0000  br....r....r....
+00000240: 7215 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
+00000250: 1600 0000 da08 3c6d 6f64 756c 653e 0300  ......<module>..
+00000260: 0000 7302 0000 0010 03                   ..s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0074_auto_20200827_1818.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0098_auto_20211029_1641.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 437 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 b501 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 ae01 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00000080: 0000 0900 0000 4000 0000 7332 0000 0065  ......@...s2...e
+00000080: 0000 0800 0000 4000 0000 7330 0000 0065  ......@...s0...e
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
 000000a0: 0564 0264 0365 066a 0764 0464 0564 0664  .d.d.e.j.d.d.d.d
-000000b0: 0464 078d 0464 088d 0367 015a 0864 0953  .d...d...g.Z.d.S
-000000c0: 0029 0ada 094d 6967 7261 7469 6f6e 2902  .)...Migration).
-000000d0: da0a 646a 6175 746f 7461 736b da14 3030  ..djautotask..00
-000000e0: 3733 5f73 796e 636a 6f62 5f73 6b69 7070  73_syncjob_skipp
-000000f0: 6564 da0b 7365 7276 6963 6563 616c 6cda  ed..servicecall.
-00000100: 0864 7572 6174 696f 6e54 e904 0000 00e9  .durationT......
-00000110: 0900 0000 2904 da05 626c 616e 6bda 0e64  ....)...blank..d
-00000120: 6563 696d 616c 5f70 6c61 6365 73da 0a6d  ecimal_places..m
-00000130: 6178 5f64 6967 6974 73da 046e 756c 6c29  ax_digits..null)
-00000140: 03da 0a6d 6f64 656c 5f6e 616d 65da 046e  ...model_name..n
-00000150: 616d 65da 0566 6965 6c64 4e29 09da 085f  ame..fieldN)..._
-00000160: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000170: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000180: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
-00000190: 0200 0000 da0a 416c 7465 7246 6965 6c64  ......AlterField
-000001a0: 7203 0000 00da 0c44 6563 696d 616c 4669  r......DecimalFi
-000001b0: 656c 64da 0a6f 7065 7261 7469 6f6e 73a9  eld..operations.
-000001c0: 0072 1900 0000 7219 0000 00fa 622f 686f  .r....r.....b/ho
-000001d0: 6d65 2f72 756e 6e65 722f 776f 726b 2f64  me/runner/work/d
-000001e0: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
-000001f0: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
-00000200: 6a61 7574 6f74 6173 6b2f 6d69 6772 6174  jautotask/migrat
-00000210: 696f 6e73 2f30 3037 345f 6175 746f 5f32  ions/0074_auto_2
-00000220: 3032 3030 3832 375f 3138 3138 2e70 7972  0200827_1818.pyr
-00000230: 0400 0000 0600 0000 7310 0000 0008 0302  ........s.......
-00000240: ff04 0504 0102 0102 0110 fd04 ff72 0400  .............r..
-00000250: 0000 4e29 04da 0964 6a61 6e67 6f2e 6462  ..N)...django.db
-00000260: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
-00000270: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
-00000280: 0000 00da 083c 6d6f 6475 6c65 3e03 0000  .....<module>...
-00000290: 0073 0200 0000 1003                      .s......
+000000b0: 078d 0364 088d 0367 015a 0864 0953 0029  ...d...g.Z.d.S.)
+000000c0: 0ada 094d 6967 7261 7469 6f6e 2902 da0a  ...Migration)...
+000000d0: 646a 6175 746f 7461 736b da17 3030 3937  djautotask..0097
+000000e0: 5f61 7574 6f5f 3230 3231 3038 3139 5f31  _auto_20210819_1
+000000f0: 3430 32da 0570 6861 7365 da0f 6573 7469  402..phase..esti
+00000100: 6d61 7465 645f 686f 7572 73e9 0200 0000  mated_hours.....
+00000110: 6700 0000 0000 0000 00e9 0600 0000 2903  g.............).
+00000120: da0e 6465 6369 6d61 6c5f 706c 6163 6573  ..decimal_places
+00000130: da07 6465 6661 756c 74da 0a6d 6178 5f64  ..default..max_d
+00000140: 6967 6974 7329 03da 0a6d 6f64 656c 5f6e  igits)...model_n
+00000150: 616d 65da 046e 616d 65da 0566 6965 6c64  ame..name..field
+00000160: 4e29 09da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000170: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000180: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
+00000190: 6e63 6965 7372 0200 0000 da0a 416c 7465  nciesr......Alte
+000001a0: 7246 6965 6c64 7203 0000 00da 0c44 6563  rFieldr......Dec
+000001b0: 696d 616c 4669 656c 64da 0a6f 7065 7261  imalField..opera
+000001c0: 7469 6f6e 73a9 0072 1800 0000 7218 0000  tions..r....r...
+000001d0: 00fa 622f 686f 6d65 2f72 756e 6e65 722f  ..b/home/runner/
+000001e0: 776f 726b 2f64 6a61 6e67 6f2d 6175 746f  work/django-auto
+000001f0: 7461 736b 2f64 6a61 6e67 6f2d 6175 746f  task/django-auto
+00000200: 7461 736b 2f64 6a61 7574 6f74 6173 6b2f  task/djautotask/
+00000210: 6d69 6772 6174 696f 6e73 2f30 3039 385f  migrations/0098_
+00000220: 6175 746f 5f32 3032 3131 3032 395f 3136  auto_20211029_16
+00000230: 3431 2e70 7972 0400 0000 0600 0000 7310  41.pyr........s.
+00000240: 0000 0008 0302 ff04 0504 0102 0102 010e  ................
+00000250: fd04 ff72 0400 0000 4e29 04da 0964 6a61  ...r....N)...dja
+00000260: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
+00000270: 7204 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
+00000280: 1800 0000 7219 0000 00da 083c 6d6f 6475  ....r......<modu
+00000290: 6c65 3e03 0000 0073 0200 0000 1003       le>....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0075_taskpredecessor.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0075_taskpredecessor.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1385 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 6905 0000  U.........Kdi...
+00000000: 550d 0d0a 0000 0000 3268 4c64 6905 0000  U.......2hLdi...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
@@ -16,64 +16,64 @@
 000000f0: 640c 6506 6a0d 6404 6404 640d 8d02 6602  d.e.j.d.d.d...f.
 00000100: 640e 6506 6a0e 6404 6404 650f 6a09 6a06  d.e.j.d.d.e.j.j.
 00000110: 6a10 6a11 640e 640f 6410 8d05 6602 6411  j.j.d.d.d...f.d.
 00000120: 6506 6a0e 6404 6404 650f 6a09 6a06 6a10  e.j.d.d.e.j.j.j.
 00000130: 6a11 6411 640f 6410 8d05 6602 6706 6412  j.d.d.d...f.g.d.
 00000140: 640a 6405 6413 9c03 6414 8d03 6701 5a12  d.d.d...d...g.Z.
 00000150: 6415 5300 2916 da09 4d69 6772 6174 696f  d.S.)...Migratio
-00000160: 6e29 02da 0a64 6a61 7574 6f74 6173 6b5a  n)...djautotaskZ
+00000160: 6e29 02da 0a64 6a61 7574 6f74 6173 6bda  n)...djautotask.
 00000170: 1730 3037 345f 6175 746f 5f32 3032 3030  .0074_auto_20200
 00000180: 3832 375f 3138 3138 da0f 5461 736b 5072  827_1818..TaskPr
 00000190: 6564 6563 6573 736f 72da 0269 6454 46da  edecessor..idTF.
 000001a0: 0249 4429 04da 0c61 7574 6f5f 6372 6561  .ID)...auto_crea
 000001b0: 7465 64da 0b70 7269 6d61 7279 5f6b 6579  ted..primary_key
 000001c0: da09 7365 7269 616c 697a 65da 0c76 6572  ..serialize..ver
 000001d0: 626f 7365 5f6e 616d 65da 0763 7265 6174  bose_name..creat
 000001e0: 6564 2902 da0c 6175 746f 5f6e 6f77 5f61  ed)...auto_now_a
-000001f0: 6464 720c 0000 00da 086d 6f64 6966 6965  ddr......modifie
-00000200: 6429 02da 0861 7574 6f5f 6e6f 7772 0c00  d)...auto_nowr..
+000001f0: 6464 720d 0000 00da 086d 6f64 6966 6965  ddr......modifie
+00000200: 6429 02da 0861 7574 6f5f 6e6f 7772 0d00  d)...auto_nowr..
 00000210: 0000 da08 6c61 675f 6461 7973 2902 da05  ....lag_days)...
 00000220: 626c 616e 6bda 046e 756c 6cda 1070 7265  blank..null..pre
 00000230: 6465 6365 7373 6f72 5f74 6173 6b7a 0f64  decessor_taskz.d
 00000240: 6a61 7574 6f74 6173 6b2e 5461 736b 2905  jautotask.Task).
-00000250: 7212 0000 0072 1300 0000 da09 6f6e 5f64  r....r......on_d
+00000250: 7213 0000 0072 1400 0000 da09 6f6e 5f64  r....r......on_d
 00000260: 656c 6574 65da 0c72 656c 6174 6564 5f6e  elete..related_n
 00000270: 616d 65da 0274 6fda 0e73 7563 6365 7373  ame..to..success
 00000280: 6f72 5f74 6173 6b29 027a 092d 6d6f 6469  or_task).z.-modi
 00000290: 6669 6564 7a08 2d63 7265 6174 6564 2903  fiedz.-created).
 000002a0: da08 6f72 6465 7269 6e67 da0d 6765 745f  ..ordering..get_
 000002b0: 6c61 7465 7374 5f62 79da 0861 6273 7472  latest_by..abstr
 000002c0: 6163 7429 03da 046e 616d 65da 0666 6965  act)...name..fie
 000002d0: 6c64 73da 076f 7074 696f 6e73 4e29 13da  lds..optionsN)..
 000002e0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
 000002f0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
 00000300: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
 00000310: 7372 0200 0000 da0b 4372 6561 7465 4d6f  sr......CreateMo
 00000320: 6465 6c72 0300 0000 da09 4175 746f 4669  delr......AutoFi
 00000330: 656c 64da 1164 6a61 6e67 6f5f 6578 7465  eld..django_exte
-00000340: 6e73 696f 6e73 da02 6462 721d 0000 00da  nsions..dbr.....
+00000340: 6e73 696f 6e73 da02 6462 721e 0000 00da  nsions..dbr.....
 00000350: 1543 7265 6174 696f 6e44 6174 6554 696d  .CreationDateTim
 00000360: 6546 6965 6c64 da19 4d6f 6469 6669 6361  eField..Modifica
 00000370: 7469 6f6e 4461 7465 5469 6d65 4669 656c  tionDateTimeFiel
 00000380: 64da 0c49 6e74 6567 6572 4669 656c 64da  d..IntegerField.
 00000390: 0a46 6f72 6569 676e 4b65 79da 0664 6a61  .ForeignKey..dja
 000003a0: 6e67 6fda 0864 656c 6574 696f 6eda 0743  ngo..deletion..C
 000003b0: 4153 4341 4445 da0a 6f70 6572 6174 696f  ASCADE..operatio
-000003c0: 6e73 a900 722f 0000 0072 2f00 0000 fa5f  ns..r/...r/...._
+000003c0: 6e73 a900 7230 0000 0072 3000 0000 fa5f  ns..r0...r0...._
 000003d0: 2f68 6f6d 652f 7275 6e6e 6572 2f77 6f72  /home/runner/wor
 000003e0: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
 000003f0: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
 00000400: 6b2f 646a 6175 746f 7461 736b 2f6d 6967  k/djautotask/mig
 00000410: 7261 7469 6f6e 732f 3030 3735 5f74 6173  rations/0075_tas
 00000420: 6b70 7265 6465 6365 7373 6f72 2e70 7972  kpredecessor.pyr
 00000430: 0400 0000 0800 0000 7322 0000 0008 0302  ........s"......
 00000440: ff04 0504 0102 0214 0114 0114 0110 011e  ................
 00000450: 011e fa02 0902 0102 0102 fd04 f604 ff72  ...............r
 00000460: 0400 0000 2908 da09 646a 616e 676f 2e64  ....)...django.d
 00000470: 6272 0200 0000 7203 0000 00da 1964 6a61  br....r......dja
 00000480: 6e67 6f2e 6462 2e6d 6f64 656c 732e 6465  ngo.db.models.de
-00000490: 6c65 7469 6f6e 722b 0000 00da 1b64 6a61  letionr+.....dja
+00000490: 6c65 7469 6f6e 722c 0000 00da 1b64 6a61  letionr,.....dja
 000004a0: 6e67 6f5f 6578 7465 6e73 696f 6e73 2e64  ngo_extensions.d
-000004b0: 622e 6669 656c 6473 7225 0000 0072 0400  b.fieldsr%...r..
-000004c0: 0000 722f 0000 0072 2f00 0000 722f 0000  ..r/...r/...r/..
-000004d0: 0072 3000 0000 da08 3c6d 6f64 756c 653e  .r0.....<module>
+000004b0: 622e 6669 656c 6473 7226 0000 0072 0400  b.fieldsr&...r..
+000004c0: 0000 7230 0000 0072 3000 0000 7230 0000  ..r0...r0...r0..
+000004d0: 0072 3100 0000 da08 3c6d 6f64 756c 653e  .r1.....<module>
 000004e0: 0300 0000 7306 0000 0010 0108 0108 03    ....s..........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0076_auto_20200923_0953.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0076_auto_20200923_0953.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1861 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 4507 0000  U.........KdE...
+00000000: 550d 0d0a 0000 0000 3268 4c64 4507 0000  U.......2hLdE...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0f00 0000 4000 0000 73d6  ..........@...s.
@@ -17,38 +17,38 @@
 00000100: 0265 046a 0564 0c64 0364 0469 0164 058d  .e.j.d.d.d.i.d..
 00000110: 0265 046a 0564 0d64 0364 0469 0164 058d  .e.j.d.d.d.i.d..
 00000120: 0265 046a 0564 0e64 0364 0469 0164 058d  .e.j.d.d.d.i.d..
 00000130: 0265 046a 0564 0f64 0364 0469 0164 058d  .e.j.d.d.d.i.d..
 00000140: 0265 046a 0564 1064 0364 0469 0164 058d  .e.j.d.d.d.i.d..
 00000150: 0267 0c5a 0664 1153 0029 12da 094d 6967  .g.Z.d.S.)...Mig
 00000160: 7261 7469 6f6e 2902 da0a 646a 6175 746f  ration)...djauto
-00000170: 7461 736b da14 3030 3735 5f74 6173 6b70  task..0075_taskp
+00000170: 7461 736b 5a14 3030 3735 5f74 6173 6b70  taskZ.0075_taskp
 00000180: 7265 6465 6365 7373 6f72 5a0e 616c 6c6f  redecessorZ.allo
 00000190: 6361 7469 6f6e 636f 6465 da0d 6765 745f  cationcode..get_
 000001a0: 6c61 7465 7374 5f62 79da 086d 6f64 6966  latest_by..modif
 000001b0: 6965 6429 02da 046e 616d 65da 076f 7074  ied)...name..opt
 000001c0: 696f 6e73 da0b 7365 7276 6963 6563 616c  ions..servicecal
-000001d0: 6cda 0f73 6572 7669 6365 6361 6c6c 7461  l..servicecallta
+000001d0: 6c5a 0f73 6572 7669 6365 6361 6c6c 7461  lZ.servicecallta
 000001e0: 736b 5a17 7365 7276 6963 6563 616c 6c74  skZ.servicecallt
-000001f0: 6173 6b72 6573 6f75 7263 65da 1173 6572  askresource..ser
+000001f0: 6173 6b72 6573 6f75 7263 655a 1173 6572  askresourceZ.ser
 00000200: 7669 6365 6361 6c6c 7469 636b 6574 5a19  vicecallticketZ.
 00000210: 7365 7276 6963 6563 616c 6c74 6963 6b65  servicecallticke
 00000220: 7472 6573 6f75 7263 65da 0474 6173 6bda  tresource..task.
-00000230: 0874 6173 6b6e 6f74 65da 0f74 6173 6b70  .tasknote..taskp
+00000230: 0874 6173 6b6e 6f74 655a 0f74 6173 6b70  .tasknoteZ.taskp
 00000240: 7265 6465 6365 7373 6f72 da15 7461 736b  redecessor..task
 00000250: 7365 636f 6e64 6172 7972 6573 6f75 7263  secondaryresourc
 00000260: 65da 0a74 6963 6b65 746e 6f74 65da 1774  e..ticketnote..t
 00000270: 6963 6b65 7473 6563 6f6e 6461 7279 7265  icketsecondaryre
 00000280: 736f 7572 6365 4e29 07da 085f 5f6e 616d  sourceN)...__nam
 00000290: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
 000002a0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
 000002b0: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
 000002c0: da11 416c 7465 724d 6f64 656c 4f70 7469  ..AlterModelOpti
 000002d0: 6f6e 73da 0a6f 7065 7261 7469 6f6e 73a9  ons..operations.
-000002e0: 0072 1900 0000 7219 0000 00fa 622f 686f  .r....r.....b/ho
+000002e0: 0072 1500 0000 7215 0000 00fa 622f 686f  .r....r.....b/ho
 000002f0: 6d65 2f72 756e 6e65 722f 776f 726b 2f64  me/runner/work/d
 00000300: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
 00000310: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
 00000320: 6a61 7574 6f74 6173 6b2f 6d69 6772 6174  jautotask/migrat
 00000330: 696f 6e73 2f30 3037 365f 6175 746f 5f32  ions/0076_auto_2
 00000340: 3032 3030 3932 335f 3039 3533 2e70 7972  0200923_0953.pyr
 00000350: 0300 0000 0600 0000 7366 0000 0008 0302  ........sf......
@@ -56,10 +56,10 @@
 00000370: fe04 0404 0102 0106 fe04 0404 0102 0106  ................
 00000380: fe04 0404 0102 0106 fe04 0404 0102 0106  ................
 00000390: fe04 0404 0102 0106 fe04 0404 0102 0106  ................
 000003a0: fe04 0404 0102 0106 fe04 0404 0102 0106  ................
 000003b0: fe04 0404 0102 0106 fe04 0404 0102 0106  ................
 000003c0: fe04 d372 0300 0000 4e29 03da 0964 6a61  ...r....N)...dja
 000003d0: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
-000003e0: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-000003f0: 1a00 0000 da08 3c6d 6f64 756c 653e 0300  ......<module>..
+000003e0: 7215 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
+000003f0: 1600 0000 da08 3c6d 6f64 756c 653e 0300  ......<module>..
 00000400: 0000 7302 0000 000c 03                   ..s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0076_auto_20200925_1326.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0076_auto_20200925_1326.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 982 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 d603 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 d603 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
@@ -12,50 +12,50 @@
 000000b0: 6901 6405 8d02 6504 6a06 6402 6406 6507  i.d...e.j.d.d.e.
 000000c0: 6a08 6407 6407 6509 6a0a 6a07 6a0b 6a0c  j.d.d.e.j.j.j.j.
 000000d0: 6408 6409 640a 8d05 640b 8d03 6504 6a06  d.d.d...d...e.j.
 000000e0: 6402 640c 6507 6a08 6407 6407 6509 6a0a  d.d.e.j.d.d.e.j.
 000000f0: 6a07 6a0b 6a0c 640d 6409 640a 8d05 640b  j.j.j.d.d.d...d.
 00000100: 8d03 6703 5a0d 640e 5300 290f da09 4d69  ..g.Z.d.S.)...Mi
 00000110: 6772 6174 696f 6e29 02da 0a64 6a61 7574  gration)...djaut
-00000120: 6f74 6173 6b5a 1430 3037 355f 7461 736b  otaskZ.0075_task
-00000130: 7072 6564 6563 6573 736f 725a 0f74 6173  predecessorZ.tas
+00000120: 6f74 6173 6bda 1430 3037 355f 7461 736b  otask..0075_task
+00000130: 7072 6564 6563 6573 736f 72da 0f74 6173  predecessor..tas
 00000140: 6b70 7265 6465 6365 7373 6f72 da08 6f72  kpredecessor..or
 00000150: 6465 7269 6e67 2901 da17 7072 6564 6563  dering)...predec
 00000160: 6573 736f 725f 7461 736b 5f5f 7469 746c  essor_task__titl
 00000170: 6529 02da 046e 616d 65da 076f 7074 696f  e)...name..optio
 00000180: 6e73 da10 7072 6564 6563 6573 736f 725f  ns..predecessor_
 00000190: 7461 736b 54da 1470 7265 6465 6365 7373  taskT..predecess
 000001a0: 6f72 5f74 6173 6b5f 7365 747a 0f64 6a61  or_task_setz.dja
 000001b0: 7574 6f74 6173 6b2e 5461 736b 2905 da05  utotask.Task)...
 000001c0: 626c 616e 6bda 046e 756c 6cda 096f 6e5f  blank..null..on_
 000001d0: 6465 6c65 7465 da0c 7265 6c61 7465 645f  delete..related_
 000001e0: 6e61 6d65 da02 746f 2903 da0a 6d6f 6465  name..to)...mode
-000001f0: 6c5f 6e61 6d65 7208 0000 00da 0566 6965  l_namer......fie
+000001f0: 6c5f 6e61 6d65 720a 0000 00da 0566 6965  l_namer......fie
 00000200: 6c64 da0e 7375 6363 6573 736f 725f 7461  ld..successor_ta
 00000210: 736b da12 7375 6363 6573 736f 725f 7461  sk..successor_ta
 00000220: 736b 5f73 6574 4e29 0eda 085f 5f6e 616d  sk_setN)...__nam
 00000230: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
 00000240: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
 00000250: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
 00000260: da11 416c 7465 724d 6f64 656c 4f70 7469  ..AlterModelOpti
 00000270: 6f6e 73da 0a41 6c74 6572 4669 656c 6472  ons..AlterFieldr
 00000280: 0300 0000 da0a 466f 7265 6967 6e4b 6579  ......ForeignKey
 00000290: da06 646a 616e 676f da02 6462 da08 6465  ..django..db..de
 000002a0: 6c65 7469 6f6e da07 4341 5343 4144 45da  letion..CASCADE.
-000002b0: 0a6f 7065 7261 7469 6f6e 73a9 0072 2100  .operations..r!.
-000002c0: 0000 7221 0000 00fa 622f 686f 6d65 2f72  ..r!....b/home/r
+000002b0: 0a6f 7065 7261 7469 6f6e 73a9 0072 2300  .operations..r#.
+000002c0: 0000 7223 0000 00fa 622f 686f 6d65 2f72  ..r#....b/home/r
 000002d0: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
 000002e0: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
 000002f0: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
 00000300: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
 00000310: 2f30 3037 365f 6175 746f 5f32 3032 3030  /0076_auto_20200
 00000320: 3932 355f 3133 3236 2e70 7972 0400 0000  925_1326.pyr....
 00000330: 0700 0000 7322 0000 0008 0302 ff04 0504  ....s"..........
 00000340: 0102 0106 fe04 0404 0102 0102 011a fd04  ................
 00000350: 0504 0102 0102 011a fd04 f672 0400 0000  ...........r....
 00000360: 2906 da09 646a 616e 676f 2e64 6272 0200  )...django.dbr..
 00000370: 0000 7203 0000 00da 1964 6a61 6e67 6f2e  ..r......django.
 00000380: 6462 2e6d 6f64 656c 732e 6465 6c65 7469  db.models.deleti
-00000390: 6f6e 721c 0000 0072 0400 0000 7221 0000  onr....r....r!..
-000003a0: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
+00000390: 6f6e 721e 0000 0072 0400 0000 7223 0000  onr....r....r#..
+000003a0: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
 000003b0: da08 3c6d 6f64 756c 653e 0300 0000 7304  ..<module>....s.
 000003c0: 0000 0010 0108 03                        .......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0077_auto_20200924_1512.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0077_auto_20200924_1512.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 757 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 f502 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 f502 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0080_accountphysicallocationtracker_accounttracker_accounttypetracker_allocationcodetracker_contracttrack.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0080_accountphysicallocationtracker_accounttracker_accounttypetracker_allocationcodetracker_contracttrack.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 14818 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 e239 0000  U.........Kd.9..
+00000000: 550d 0d0a 0000 0000 3268 4c64 e239 0000  U.......2hLd.9..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 3000 0000 4000 0000 7340  ......0...@...s@
@@ -71,15 +71,15 @@
 00000460: 0067 0064 059c 0464 7664 078d 0465 046a  .g.d...dvd...e.j
 00000470: 0564 7767 0064 7864 0467 0067 0064 059c  .dwg.dxd.g.g.d..
 00000480: 0464 7964 078d 0465 046a 0564 7a67 0064  .dyd...e.j.dzg.d
 00000490: 7b64 0467 0067 0064 059c 0464 7c64 078d  {d.g.g.d...d|d..
 000004a0: 0465 046a 0564 7d67 0064 7e64 0467 0067  .e.j.d}g.d~d.g.g
 000004b0: 0064 059c 0464 7f64 078d 0467 295a 0664  .d...d.d...g)Z.d
 000004c0: 8053 0029 81da 094d 6967 7261 7469 6f6e  .S.)...Migration
-000004d0: 2902 da0a 646a 6175 746f 7461 736b 5a17  )...djautotaskZ.
+000004d0: 2902 da0a 646a 6175 746f 7461 736b da17  )...djautotask..
 000004e0: 3030 3739 5f61 7574 6f5f 3230 3230 3130  0079_auto_202010
 000004f0: 3033 5f31 3132 35da 1e41 6363 6f75 6e74  03_1125..Account
 00000500: 5068 7973 6963 616c 4c6f 6361 7469 6f6e  PhysicalLocation
 00000510: 5472 6163 6b65 72da 2264 6a61 7574 6f74  Tracker."djautot
 00000520: 6173 6b5f 6163 636f 756e 7470 6879 7369  ask_accountphysi
 00000530: 6361 6c6c 6f63 6174 696f 6e54 2904 da08  callocationT)...
 00000540: 6462 5f74 6162 6c65 da05 7072 6f78 79da  db_table..proxy.
@@ -270,15 +270,15 @@
 000010d0: 7365 7479 7065 2901 7a12 646a 6175 746f  setype).z.djauto
 000010e0: 7461 736b 2e75 7365 7479 7065 4e29 07da  task.usetypeN)..
 000010f0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
 00001100: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
 00001110: 655f 5fda 0c64 6570 656e 6465 6e63 6965  e__..dependencie
 00001120: 7372 0200 0000 da0b 4372 6561 7465 4d6f  sr......CreateMo
 00001130: 6465 6cda 0a6f 7065 7261 7469 6f6e 73a9  del..operations.
-00001140: 0072 6300 0000 7263 0000 00fa b42f 686f  .rc...rc...../ho
+00001140: 0072 6400 0000 7264 0000 00fa b42f 686f  .rd...rd...../ho
 00001150: 6d65 2f72 756e 6e65 722f 776f 726b 2f64  me/runner/work/d
 00001160: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
 00001170: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
 00001180: 6a61 7574 6f74 6173 6b2f 6d69 6772 6174  jautotask/migrat
 00001190: 696f 6e73 2f30 3038 305f 6163 636f 756e  ions/0080_accoun
 000011a0: 7470 6879 7369 6361 6c6c 6f63 6174 696f  tphysicallocatio
 000011b0: 6e74 7261 636b 6572 5f61 6363 6f75 6e74  ntracker_account
@@ -336,11 +336,11 @@
 000014f0: 0102 fc04 0602 f604 0c04 0102 0102 0302  ................
 00001500: 0102 0102 0102 fc04 0602 f604 0c04 0102  ................
 00001510: 0102 0302 0102 0102 0102 fc04 0602 f604  ................
 00001520: 0c04 0102 0102 0302 0102 0102 0102 fc04  ................
 00001530: 0602 f604 0c04 0102 0102 0302 0102 0102  ................
 00001540: 0102 fc04 0602 f604 8000 8000 8000 9f72  ...............r
 00001550: 0300 0000 4e29 03da 0964 6a61 6e67 6f2e  ....N)...django.
-00001560: 6462 7202 0000 0072 0300 0000 7263 0000  dbr....r....rc..
-00001570: 0072 6300 0000 7263 0000 0072 6400 0000  .rc...rc...rd...
+00001560: 6462 7202 0000 0072 0300 0000 7264 0000  dbr....r....rd..
+00001570: 0072 6400 0000 7264 0000 0072 6500 0000  .rd...rd...re...
 00001580: da08 3c6d 6f64 756c 653e 0300 0000 7302  ..<module>....s.
 00001590: 0000 000c 03                             .....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0081_project_department.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0091_auto_20210525_1723.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 590 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,40 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 4e02 0000  U.........KdN...
+00000000: 550d 0d0a 0000 0000 3268 4c64 a101 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
-00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
-00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
-00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
-00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
-00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
-00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
-000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
-000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
-000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
-000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
-000000e0: 02da 0a64 6a61 7574 6f74 6173 6bda 6930  ...djautotask.i0
-000000f0: 3038 305f 6163 636f 756e 7470 6879 7369  080_accountphysi
-00000100: 6361 6c6c 6f63 6174 696f 6e74 7261 636b  callocationtrack
-00000110: 6572 5f61 6363 6f75 6e74 7472 6163 6b65  er_accounttracke
-00000120: 725f 6163 636f 756e 7474 7970 6574 7261  r_accounttypetra
-00000130: 636b 6572 5f61 6c6c 6f63 6174 696f 6e63  cker_allocationc
-00000140: 6f64 6574 7261 636b 6572 5f63 6f6e 7472  odetracker_contr
-00000150: 6163 7474 7261 636b da07 7072 6f6a 6563  acttrack..projec
-00000160: 74da 0a64 6570 6172 746d 656e 7454 7a15  t..departmentTz.
-00000170: 646a 6175 746f 7461 736b 2e64 6570 6172  djautotask.depar
-00000180: 746d 656e 7429 04da 0562 6c61 6e6b da04  tment)...blank..
-00000190: 6e75 6c6c da09 6f6e 5f64 656c 6574 65da  null..on_delete.
-000001a0: 0274 6f29 03da 0a6d 6f64 656c 5f6e 616d  .to)...model_nam
-000001b0: 65da 046e 616d 65da 0566 6965 6c64 4e29  e..name..fieldN)
-000001c0: 0dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000001d0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000001e0: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
-000001f0: 6965 7372 0200 0000 da08 4164 6446 6965  iesr......AddFie
-00000200: 6c64 7203 0000 00da 0a46 6f72 6569 676e  ldr......Foreign
-00000210: 4b65 79da 0664 6a61 6e67 6fda 0264 62da  Key..django..db.
-00000220: 0864 656c 6574 696f 6eda 0853 4554 5f4e  .deletion..SET_N
-00000230: 554c 4cda 0a6f 7065 7261 7469 6f6e 73a9  ULL..operations.
-00000240: 0072 1b00 0000 721b 0000 00fa 622f 686f  .r....r.....b/ho
-00000250: 6d65 2f72 756e 6e65 722f 776f 726b 2f64  me/runner/work/d
-00000260: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
-00000270: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
-00000280: 6a61 7574 6f74 6173 6b2f 6d69 6772 6174  jautotask/migrat
-00000290: 696f 6e73 2f30 3038 315f 7072 6f6a 6563  ions/0081_projec
-000002a0: 745f 6465 7061 7274 6d65 6e74 2e70 7972  t_department.pyr
-000002b0: 0400 0000 0700 0000 7310 0000 0008 0302  ........s.......
-000002c0: ff04 0504 0102 0102 0118 fd04 ff72 0400  .............r..
-000002d0: 0000 2906 da09 646a 616e 676f 2e64 6272  ..)...django.dbr
-000002e0: 0200 0000 7203 0000 00da 1964 6a61 6e67  ....r......djang
-000002f0: 6f2e 6462 2e6d 6f64 656c 732e 6465 6c65  o.db.models.dele
-00000300: 7469 6f6e 7216 0000 0072 0400 0000 721b  tionr....r....r.
-00000310: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
-00000320: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
-00000330: 7304 0000 0010 0108 03                   s........
+00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
+00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
+00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
+00000080: 0000 0800 0000 4000 0000 7330 0000 0065  ......@...s0...e
+00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
+000000a0: 0564 0264 0365 066a 0764 0464 0564 0464  .d.d.e.j.d.d.d.d
+000000b0: 068d 0364 078d 0367 015a 0864 0853 0029  ...d...g.Z.d.S.)
+000000c0: 09da 094d 6967 7261 7469 6f6e 2902 da0a  ...Migration)...
+000000d0: 646a 6175 746f 7461 736b da17 3030 3930  djautotask..0090
+000000e0: 5f61 7574 6f5f 3230 3231 3033 3039 5f31  _auto_20210309_1
+000000f0: 3135 37da 0474 6173 6bda 0b64 6573 6372  157..task..descr
+00000100: 6970 7469 6f6e 5469 401f 0000 2903 da05  iptionTi@...)...
+00000110: 626c 616e 6bda 0a6d 6178 5f6c 656e 6774  blank..max_lengt
+00000120: 68da 046e 756c 6c29 03da 0a6d 6f64 656c  h..null)...model
+00000130: 5f6e 616d 65da 046e 616d 65da 0566 6965  _name..name..fie
+00000140: 6c64 4e29 09da 085f 5f6e 616d 655f 5fda  ldN)...__name__.
+00000150: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000160: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
+00000170: 6465 6e63 6965 7372 0200 0000 da0a 416c  denciesr......Al
+00000180: 7465 7246 6965 6c64 7203 0000 00da 0954  terFieldr......T
+00000190: 6578 7446 6965 6c64 da0a 6f70 6572 6174  extField..operat
+000001a0: 696f 6e73 a900 7216 0000 0072 1600 0000  ions..r....r....
+000001b0: fa62 2f68 6f6d 652f 7275 6e6e 6572 2f77  .b/home/runner/w
+000001c0: 6f72 6b2f 646a 616e 676f 2d61 7574 6f74  ork/django-autot
+000001d0: 6173 6b2f 646a 616e 676f 2d61 7574 6f74  ask/django-autot
+000001e0: 6173 6b2f 646a 6175 746f 7461 736b 2f6d  ask/djautotask/m
+000001f0: 6967 7261 7469 6f6e 732f 3030 3931 5f61  igrations/0091_a
+00000200: 7574 6f5f 3230 3231 3035 3235 5f31 3732  uto_20210525_172
+00000210: 332e 7079 7204 0000 0006 0000 0073 1000  3.pyr........s..
+00000220: 0000 0803 02ff 0405 0401 0201 0201 0efd  ................
+00000230: 04ff 7204 0000 004e 2904 da09 646a 616e  ..r....N)...djan
+00000240: 676f 2e64 6272 0200 0000 7203 0000 0072  go.dbr....r....r
+00000250: 0400 0000 7216 0000 0072 1600 0000 7216  ....r....r....r.
+00000260: 0000 0072 1700 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000270: 653e 0300 0000 7302 0000 0010 03         e>....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0082_auto_20201020_1617.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0082_auto_20201020_1617.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 3176 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 680c 0000  U.........Kdh...
+00000000: 550d 0d0a 0000 0000 3268 4c64 680c 0000  U.......2hLdh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
@@ -37,53 +37,53 @@
 00000240: 6410 8d03 6602 6411 6506 6a0d 6404 640d  d...f.d.e.j.d.d.
 00000250: 6404 6410 8d03 6602 6412 6506 6a0e 6405  d.d...f.d.e.j.d.
 00000260: 6413 8d01 6602 6414 6506 6a0f 6510 6413  d...f.d.e.j.e.d.
 00000270: 8d01 6602 6708 6415 6405 6901 6416 8d03  ..f.g.d.d.i.d...
 00000280: 6504 6a11 6419 641a 6506 6a0f 6404 6510  e.j.d.d.e.j.d.e.
 00000290: 6404 641b 8d03 641c 8d03 6704 5a12 641d  d.d...d...g.Z.d.
 000002a0: 5300 291e da09 4d69 6772 6174 696f 6e29  S.)...Migration)
-000002b0: 02da 0a64 6a61 7574 6f74 6173 6bda 1730  ...djautotask..0
+000002b0: 02da 0a64 6a61 7574 6f74 6173 6b5a 1730  ...djautotaskZ.0
 000002c0: 3038 315f 7072 6f6a 6563 745f 6465 7061  081_project_depa
 000002d0: 7274 6d65 6e74 da0a 5072 6f6a 6563 7455  rtment..ProjectU
 000002e0: 4446 da02 6964 5446 da02 4944 2904 da0c  DF..idTF..ID)...
 000002f0: 6175 746f 5f63 7265 6174 6564 da0b 7072  auto_created..pr
 00000300: 696d 6172 795f 6b65 79da 0973 6572 6961  imary_key..seria
 00000310: 6c69 7a65 da0c 7665 7262 6f73 655f 6e61  lize..verbose_na
 00000320: 6d65 da07 6372 6561 7465 6429 02da 0c61  me..created)...a
-00000330: 7574 6f5f 6e6f 775f 6164 6472 0d00 0000  uto_now_addr....
+00000330: 7574 6f5f 6e6f 775f 6164 6472 0c00 0000  uto_now_addr....
 00000340: da08 6d6f 6469 6669 6564 2902 da08 6175  ..modified)...au
-00000350: 746f 5f6e 6f77 720d 0000 00da 046e 616d  to_nowr......nam
+00000350: 746f 5f6e 6f77 720c 0000 00da 046e 616d  to_nowr......nam
 00000360: 65e9 3200 0000 2902 da0a 6d61 785f 6c65  e.2...)...max_le
 00000370: 6e67 7468 da06 756e 6971 7565 da05 6c61  ngth..unique..la
-00000380: 6265 6c29 03da 0562 6c61 6e6b 7214 0000  bel)...blankr...
+00000380: 6265 6c29 03da 0562 6c61 6e6b 7213 0000  bel)...blankr...
 00000390: 00da 046e 756c 6cda 0474 7970 65da 0b69  ...null..type..i
 000003a0: 735f 7069 636b 6c69 7374 2901 da07 6465  s_picklist)...de
 000003b0: 6661 756c 74da 0870 6963 6b6c 6973 74da  fault..picklist.
-000003c0: 0861 6273 7472 6163 7429 0372 1200 0000  .abstract).r....
+000003c0: 0861 6273 7472 6163 7429 0372 1100 0000  .abstract).r....
 000003d0: da06 6669 656c 6473 da07 6f70 7469 6f6e  ..fields..option
 000003e0: 73da 0754 6173 6b55 4446 da09 5469 636b  s..TaskUDF..Tick
 000003f0: 6574 5544 46da 0674 6963 6b65 74da 0375  etUDF..ticket..u
-00000400: 6466 2903 7217 0000 0072 1b00 0000 7218  df).r....r....r.
+00000400: 6466 2903 7216 0000 0072 1a00 0000 7217  df).r....r....r.
 00000410: 0000 0029 03da 0a6d 6f64 656c 5f6e 616d  ...)...model_nam
-00000420: 6572 1200 0000 da05 6669 656c 644e 2913  er......fieldN).
+00000420: 6572 1100 0000 da05 6669 656c 644e 2913  er......fieldN).
 00000430: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
 00000440: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
 00000450: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
 00000460: 6573 7202 0000 00da 0b43 7265 6174 654d  esr......CreateM
 00000470: 6f64 656c 7203 0000 00da 0941 7574 6f46  odelr......AutoF
 00000480: 6965 6c64 da11 646a 616e 676f 5f65 7874  ield..django_ext
-00000490: 656e 7369 6f6e 73da 0264 6272 1e00 0000  ensions..dbr....
+00000490: 656e 7369 6f6e 73da 0264 6272 1d00 0000  ensions..dbr....
 000004a0: da15 4372 6561 7469 6f6e 4461 7465 5469  ..CreationDateTi
 000004b0: 6d65 4669 656c 64da 194d 6f64 6966 6963  meField..Modific
 000004c0: 6174 696f 6e44 6174 6554 696d 6546 6965  ationDateTimeFie
 000004d0: 6c64 da09 4368 6172 4669 656c 64da 0c42  ld..CharField..B
 000004e0: 6f6f 6c65 616e 4669 656c 64da 094a 534f  ooleanField..JSO
 000004f0: 4e46 6965 6c64 da04 6469 6374 da08 4164  NField..dict..Ad
 00000500: 6446 6965 6c64 da0a 6f70 6572 6174 696f  dField..operatio
-00000510: 6e73 a900 7236 0000 0072 3600 0000 fa62  ns..r6...r6....b
+00000510: 6e73 a900 7235 0000 0072 3500 0000 fa62  ns..r5...r5....b
 00000520: 2f68 6f6d 652f 7275 6e6e 6572 2f77 6f72  /home/runner/wor
 00000530: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
 00000540: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
 00000550: 6b2f 646a 6175 746f 7461 736b 2f6d 6967  k/djautotask/mig
 00000560: 7261 7469 6f6e 732f 3030 3832 5f61 7574  rations/0082_aut
 00000570: 6f5f 3230 3230 3130 3230 5f31 3631 372e  o_20201020_1617.
 00000580: 7079 7204 0000 0007 0000 0073 6a00 0000  pyr........sj...
@@ -93,11 +93,11 @@
 000005c0: 1201 1201 0e01 0ef8 020b 0200 02ff 02f4  ................
 000005d0: 0410 0401 0202 1401 1401 1401 1001 1201  ................
 000005e0: 1201 0e01 0ef8 020b 0200 02ff 02f4 0410  ................
 000005f0: 0401 0201 0201 0efd 04cf 7204 0000 0029  ..........r....)
 00000600: 06da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
 00000610: 0072 0300 0000 da1b 646a 616e 676f 5f65  .r......django_e
 00000620: 7874 656e 7369 6f6e 732e 6462 2e66 6965  xtensions.db.fie
-00000630: 6c64 7372 2c00 0000 7204 0000 0072 3600  ldsr,...r....r6.
-00000640: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
+00000630: 6c64 7372 2b00 0000 7204 0000 0072 3500  ldsr+...r....r5.
+00000640: 0000 7235 0000 0072 3500 0000 7236 0000  ..r5...r5...r6..
 00000650: 00da 083c 6d6f 6475 6c65 3e03 0000 0073  ...<module>....s
 00000660: 0400 0000 1001 0803                      ........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0083_ticketudftracker.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0083_ticketudftracker.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 575 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 3f02 0000  U.........Kd?...
+00000000: 550d 0d0a 0000 0000 3268 4c64 3f02 0000  U.......2hLd?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0800 0000 4000 0000 7330  ..........@...s0
 00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
 00000090: 0365 046a 0564 0267 0064 0364 0467 0067  .e.j.d.g.d.d.g.g
 000000a0: 0064 059c 0464 0664 078d 0467 015a 0664  .d...d.d...g.Z.d
 000000b0: 0853 0029 09da 094d 6967 7261 7469 6f6e  .S.)...Migration
-000000c0: 2902 da0a 646a 6175 746f 7461 736b 5a17  )...djautotaskZ.
+000000c0: 2902 da0a 646a 6175 746f 7461 736b da17  )...djautotask..
 000000d0: 3030 3832 5f61 7574 6f5f 3230 3230 3130  0082_auto_202010
 000000e0: 3230 5f31 3631 37da 1054 6963 6b65 7455  20_1617..TicketU
 000000f0: 4446 5472 6163 6b65 72da 1464 6a61 7574  DFTracker..djaut
 00000100: 6f74 6173 6b5f 7469 636b 6574 7564 6654  otask_ticketudfT
 00000110: 2904 da08 6462 5f74 6162 6c65 da05 7072  )...db_table..pr
 00000120: 6f78 79da 0769 6e64 6578 6573 da0b 636f  oxy..indexes..co
 00000130: 6e73 7472 6169 6e74 7329 017a 1464 6a61  nstraints).z.dja
@@ -22,21 +22,21 @@
 00000150: 6629 04da 046e 616d 65da 0666 6965 6c64  f)...name..field
 00000160: 73da 076f 7074 696f 6e73 da05 6261 7365  s..options..base
 00000170: 734e 2907 da08 5f5f 6e61 6d65 5f5f da0a  sN)...__name__..
 00000180: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 00000190: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
 000001a0: 656e 6369 6573 7202 0000 00da 0b43 7265  enciesr......Cre
 000001b0: 6174 654d 6f64 656c da0a 6f70 6572 6174  ateModel..operat
-000001c0: 696f 6e73 a900 7215 0000 0072 1500 0000  ions..r....r....
+000001c0: 696f 6e73 a900 7216 0000 0072 1600 0000  ions..r....r....
 000001d0: fa60 2f68 6f6d 652f 7275 6e6e 6572 2f77  .`/home/runner/w
 000001e0: 6f72 6b2f 646a 616e 676f 2d61 7574 6f74  ork/django-autot
 000001f0: 6173 6b2f 646a 616e 676f 2d61 7574 6f74  ask/django-autot
 00000200: 6173 6b2f 646a 6175 746f 7461 736b 2f6d  ask/djautotask/m
 00000210: 6967 7261 7469 6f6e 732f 3030 3833 5f74  igrations/0083_t
 00000220: 6963 6b65 7475 6466 7472 6163 6b65 722e  icketudftracker.
 00000230: 7079 7203 0000 0006 0000 0073 1a00 0000  pyr........s....
 00000240: 0803 02ff 0405 0401 0201 0203 0201 0201  ................
 00000250: 0201 02fc 0406 02f6 04ff 7203 0000 004e  ..........r....N
 00000260: 2903 da09 646a 616e 676f 2e64 6272 0200  )...django.dbr..
-00000270: 0000 7203 0000 0072 1500 0000 7215 0000  ..r....r....r...
-00000280: 0072 1500 0000 7216 0000 00da 083c 6d6f  .r....r......<mo
+00000270: 0000 7203 0000 0072 1600 0000 7216 0000  ..r....r....r...
+00000280: 0072 1600 0000 7217 0000 00da 083c 6d6f  .r....r......<mo
 00000290: 6475 6c65 3e03 0000 0073 0200 0000 0c03  dule>....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0084_projectudftracker_taskudftracker.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0084_projectudftracker_taskudftracker.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 917 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 9503 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 9503 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0900 0000 4000 0000 734a  ..........@...sJ
 00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
 00000090: 0365 046a 0564 0267 0064 0364 0467 0067  .e.j.d.g.d.d.g.g
 000000a0: 0064 059c 0464 0664 078d 0465 046a 0564  .d...d.d...e.j.d
 000000b0: 0867 0064 0964 0467 0067 0064 059c 0464  .g.d.d.g.g.d...d
 000000c0: 0a64 078d 0467 025a 0664 0b53 0029 0cda  .d...g.Z.d.S.)..
 000000d0: 094d 6967 7261 7469 6f6e 2902 da0a 646a  .Migration)...dj
-000000e0: 6175 746f 7461 736b da15 3030 3833 5f74  autotask..0083_t
+000000e0: 6175 746f 7461 736b 5a15 3030 3833 5f74  autotaskZ.0083_t
 000000f0: 6963 6b65 7475 6466 7472 6163 6b65 72da  icketudftracker.
 00000100: 1150 726f 6a65 6374 5544 4654 7261 636b  .ProjectUDFTrack
 00000110: 6572 da15 646a 6175 746f 7461 736b 5f70  er..djautotask_p
 00000120: 726f 6a65 6374 7564 6654 2904 da08 6462  rojectudfT)...db
 00000130: 5f74 6162 6c65 da05 7072 6f78 79da 0769  _table..proxy..i
 00000140: 6e64 6578 6573 da0b 636f 6e73 7472 6169  ndexes..constrai
 00000150: 6e74 7329 017a 1564 6a61 7574 6f74 6173  nts).z.djautotas
@@ -27,24 +27,24 @@
 000001a0: 6175 746f 7461 736b 5f74 6173 6b75 6466  autotask_taskudf
 000001b0: 2901 7a12 646a 6175 746f 7461 736b 2e74  ).z.djautotask.t
 000001c0: 6173 6b75 6466 4e29 07da 085f 5f6e 616d  askudfN)...__nam
 000001d0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
 000001e0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
 000001f0: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
 00000200: da0b 4372 6561 7465 4d6f 6465 6cda 0a6f  ..CreateModel..o
-00000210: 7065 7261 7469 6f6e 73a9 0072 1800 0000  perations..r....
-00000220: 7218 0000 00fa 702f 686f 6d65 2f72 756e  r.....p/home/run
+00000210: 7065 7261 7469 6f6e 73a9 0072 1700 0000  perations..r....
+00000220: 7217 0000 00fa 702f 686f 6d65 2f72 756e  r.....p/home/run
 00000230: 6e65 722f 776f 726b 2f64 6a61 6e67 6f2d  ner/work/django-
 00000240: 6175 746f 7461 736b 2f64 6a61 6e67 6f2d  autotask/django-
 00000250: 6175 746f 7461 736b 2f64 6a61 7574 6f74  autotask/djautot
 00000260: 6173 6b2f 6d69 6772 6174 696f 6e73 2f30  ask/migrations/0
 00000270: 3038 345f 7072 6f6a 6563 7475 6466 7472  084_projectudftr
 00000280: 6163 6b65 725f 7461 736b 7564 6674 7261  acker_taskudftra
 00000290: 636b 6572 2e70 7972 0300 0000 0600 0000  cker.pyr........
 000002a0: 732e 0000 0008 0302 ff04 0504 0102 0102  s...............
 000002b0: 0302 0102 0102 0102 fc04 0602 f604 0c04  ................
 000002c0: 0102 0102 0302 0102 0102 0102 fc04 0602  ................
 000002d0: f604 f372 0300 0000 4e29 03da 0964 6a61  ...r....N)...dja
 000002e0: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
-000002f0: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000300: 1900 0000 da08 3c6d 6f64 756c 653e 0300  ......<module>..
+000002f0: 7217 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
+00000300: 1800 0000 da08 3c6d 6f64 756c 653e 0300  ......<module>..
 00000310: 0000 7302 0000 000c 03                   ..s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0085_auto_20201022_1822.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0092_auto_20210629_1124.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 589 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,49 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 4d02 0000  U.........KdM...
+00000000: 550d 0d0a 0000 0000 3268 4c64 6b02 0000  U.......2hLdk...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
-00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
-00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
-00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
-00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00000080: 0000 0900 0000 4000 0000 734a 0000 0065  ......@...sJ...e
-00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
-000000a0: 0564 0264 0365 066a 0764 0465 0864 0464  .d.d.e.j.d.e.d.d
-000000b0: 058d 0364 068d 0365 046a 0564 0764 0365  ...d...e.j.d.d.e
-000000c0: 066a 0764 0465 0864 0464 058d 0364 068d  .j.d.e.d.d...d..
-000000d0: 0367 025a 0964 0853 0029 09da 094d 6967  .g.Z.d.S.)...Mig
-000000e0: 7261 7469 6f6e 2902 da0a 646a 6175 746f  ration)...djauto
-000000f0: 7461 736b 5a25 3030 3834 5f70 726f 6a65  taskZ%0084_proje
-00000100: 6374 7564 6674 7261 636b 6572 5f74 6173  ctudftracker_tas
-00000110: 6b75 6466 7472 6163 6b65 72da 0770 726f  kudftracker..pro
-00000120: 6a65 6374 da03 7564 6654 2903 da05 626c  ject..udfT)...bl
-00000130: 616e 6bda 0764 6566 6175 6c74 da04 6e75  ank..default..nu
-00000140: 6c6c 2903 da0a 6d6f 6465 6c5f 6e61 6d65  ll)...model_name
-00000150: da04 6e61 6d65 da05 6669 656c 64da 0474  ..name..field..t
-00000160: 6173 6b4e 290a da08 5f5f 6e61 6d65 5f5f  askN)...__name__
-00000170: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000180: 7175 616c 6e61 6d65 5f5f da0c 6465 7065  qualname__..depe
-00000190: 6e64 656e 6369 6573 7202 0000 00da 0841  ndenciesr......A
-000001a0: 6464 4669 656c 6472 0300 0000 da09 4a53  ddFieldr......JS
-000001b0: 4f4e 4669 656c 64da 0464 6963 74da 0a6f  ONField..dict..o
-000001c0: 7065 7261 7469 6f6e 73a9 0072 1700 0000  perations..r....
-000001d0: 7217 0000 00fa 622f 686f 6d65 2f72 756e  r.....b/home/run
-000001e0: 6e65 722f 776f 726b 2f64 6a61 6e67 6f2d  ner/work/django-
-000001f0: 6175 746f 7461 736b 2f64 6a61 6e67 6f2d  autotask/django-
-00000200: 6175 746f 7461 736b 2f64 6a61 7574 6f74  autotask/djautot
-00000210: 6173 6b2f 6d69 6772 6174 696f 6e73 2f30  ask/migrations/0
-00000220: 3038 355f 6175 746f 5f32 3032 3031 3032  085_auto_2020102
-00000230: 325f 3138 3232 2e70 7972 0400 0000 0600  2_1822.pyr......
-00000240: 0000 731a 0000 0008 0302 ff04 0504 0102  ..s.............
-00000250: 0102 010e fd04 0504 0102 0102 010e fd04  ................
-00000260: fa72 0400 0000 4e29 04da 0964 6a61 6e67  .r....N)...djang
-00000270: 6f2e 6462 7202 0000 0072 0300 0000 7204  o.dbr....r....r.
-00000280: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
-00000290: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000002a0: 3e03 0000 0073 0200 0000 1003            >....s......
+00000020: 0004 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
+00000030: 6401 6c00 6d01 5a01 0100 6402 6403 8400  d.l.m.Z...d.d...
+00000040: 5a02 4700 6404 6405 8400 6405 6501 6a03  Z.G.d.d...d.e.j.
+00000050: 8303 5a03 6406 5300 2907 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 0a6d 6967 7261 7469 6f6e 7363 0200  ...migrationsc..
+00000070: 0000 0000 0000 0000 0000 0500 0000 0400  ................
+00000080: 0000 4300 0000 7330 0000 007c 00a0 0064  ..C...s0...|...d
+00000090: 0164 02a1 027d 027c 026a 016a 0264 0364  .d...}.|.j.j.d.d
+000000a0: 048d 017d 037c 0344 005d 0c7d 047c 04a0  ...}.|.D.].}.|..
+000000b0: 03a1 0001 0071 1e64 0053 0029 054e da0a  .....q.d.S.).N..
+000000c0: 646a 6175 746f 7461 736b da04 5461 736b  djautotask..Task
+000000d0: 5429 015a 0f70 726f 6a65 6374 5f5f 6973  T).Z.project__is
+000000e0: 6e75 6c6c 2904 da09 6765 745f 6d6f 6465  null)...get_mode
+000000f0: 6cda 076f 626a 6563 7473 da06 6669 6c74  l..objects..filt
+00000100: 6572 da06 6465 6c65 7465 2905 da04 6170  er..delete)...ap
+00000110: 7073 da0d 7363 6865 6d61 5f65 6469 746f  ps..schema_edito
+00000120: 7272 0400 0000 5a12 6e75 6c6c 5f70 726f  rr....Z.null_pro
+00000130: 6a65 6374 5f74 6173 6b73 da04 7461 736b  ject_tasks..task
+00000140: a900 720c 0000 00fa 622f 686f 6d65 2f72  ..r.....b/home/r
+00000150: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
+00000160: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
+00000170: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
+00000180: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
+00000190: 2f30 3039 325f 6175 746f 5f32 3032 3130  /0092_auto_20210
+000001a0: 3632 395f 3131 3234 2e70 79da 0d70 726f  629_1124.py..pro
+000001b0: 6365 7373 5f74 6173 6b73 0600 0000 7308  cess_tasks....s.
+000001c0: 0000 0000 010c 040e 0108 0172 0e00 0000  ...........r....
+000001d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000001e0: 0003 0000 0040 0000 0073 1e00 0000 6500  .....@...s....e.
+000001f0: 5a01 6400 5a02 6401 6701 5a03 6504 a005  Z.d.Z.d.g.Z.e...
+00000200: 6506 a101 6701 5a07 6402 5300 2903 da09  e...g.Z.d.S.)...
+00000210: 4d69 6772 6174 696f 6e29 0272 0300 0000  Migration).r....
+00000220: da17 3030 3931 5f61 7574 6f5f 3230 3231  ..0091_auto_2021
+00000230: 3035 3235 5f31 3732 334e 2908 da08 5f5f  0525_1723N)...__
+00000240: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000250: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000260: da0c 6465 7065 6e64 656e 6369 6573 7202  ..dependenciesr.
+00000270: 0000 00da 0952 756e 5079 7468 6f6e 720e  .....RunPythonr.
+00000280: 0000 00da 0a6f 7065 7261 7469 6f6e 7372  .....operationsr
+00000290: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
+000002a0: 0000 0072 0f00 0000 1000 0000 7308 0000  ...r........s...
+000002b0: 0008 0302 ff04 0508 ff72 0f00 0000 4e29  .........r....N)
+000002c0: 04da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
+000002d0: 0072 0e00 0000 720f 0000 0072 0c00 0000  .r....r....r....
+000002e0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+000002f0: 083c 6d6f 6475 6c65 3e03 0000 0073 0400  .<module>....s..
+00000300: 0000 0c03 080a                           ......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0086_auto_20201222_1402.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0086_auto_20201222_1402.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 2105 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 3908 0000  U.........Kd9...
+00000000: 550d 0d0a 0000 0000 3268 4c64 3908 0000  U.......2hLd9...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
@@ -23,77 +23,77 @@
 00000160: 6419 9c04 641a 641b 8d04 6504 6a12 641c  d...d.d...e.j.d.
 00000170: 641d 6506 6a0e 6404 6404 650f 6a09 6a06  d.e.j.d.d.e.j.j.
 00000180: 6a10 6a11 641e 6414 8d04 641f 8d03 6504  j.j.d.d...d...e.
 00000190: 6a12 6420 641d 6506 6a0e 6404 6404 650f  j.d d.e.j.d.d.e.
 000001a0: 6a09 6a06 6a10 6a11 641e 6414 8d04 641f  j.j.j.j.d.d...d.
 000001b0: 8d03 6704 5a13 6421 5300 2922 da09 4d69  ..g.Z.d!S.)"..Mi
 000001c0: 6772 6174 696f 6e29 02da 0a64 6a61 7574  gration)...djaut
-000001d0: 6f74 6173 6bda 1730 3038 355f 6175 746f  otask..0085_auto
+000001d0: 6f74 6173 6b5a 1730 3038 355f 6175 746f  otaskZ.0085_auto
 000001e0: 5f32 3032 3031 3032 325f 3138 3232 da07  _20201022_1822..
 000001f0: 436f 6e74 6163 74da 0269 6454 46da 0249  Contact..idTF..I
 00000200: 4429 04da 0c61 7574 6f5f 6372 6561 7465  D)...auto_create
 00000210: 64da 0b70 7269 6d61 7279 5f6b 6579 da09  d..primary_key..
 00000220: 7365 7269 616c 697a 65da 0c76 6572 626f  serialize..verbo
 00000230: 7365 5f6e 616d 65da 0763 7265 6174 6564  se_name..created
 00000240: 2902 da0c 6175 746f 5f6e 6f77 5f61 6464  )...auto_now_add
-00000250: 720d 0000 00da 086d 6f64 6966 6965 6429  r......modified)
-00000260: 02da 0861 7574 6f5f 6e6f 7772 0d00 0000  ...auto_nowr....
+00000250: 720c 0000 00da 086d 6f64 6966 6965 6429  r......modified)
+00000260: 02da 0861 7574 6f5f 6e6f 7772 0c00 0000  ...auto_nowr....
 00000270: da0a 6669 7273 745f 6e61 6d65 e914 0000  ..first_name....
 00000280: 0029 03da 0562 6c61 6e6b da0a 6d61 785f  .)...blank..max_
 00000290: 6c65 6e67 7468 da04 6e75 6c6c da09 6c61  length..null..la
 000002a0: 7374 5f6e 616d 65da 0d65 6d61 696c 5f61  st_name..email_a
 000002b0: 6464 7265 7373 e932 0000 00da 0761 6363  ddress.2.....acc
 000002c0: 6f75 6e74 7a12 646a 6175 746f 7461 736b  ountz.djautotask
-000002d0: 2e61 6363 6f75 6e74 2904 7214 0000 0072  .account).r....r
-000002e0: 1600 0000 da09 6f6e 5f64 656c 6574 65da  ......on_delete.
+000002d0: 2e61 6363 6f75 6e74 2904 7213 0000 0072  .account).r....r
+000002e0: 1500 0000 da09 6f6e 5f64 656c 6574 65da  ......on_delete.
 000002f0: 0274 6f29 02da 0d67 6574 5f6c 6174 6573  .to)...get_lates
 00000300: 745f 6279 da08 6162 7374 7261 6374 2903  t_by..abstract).
 00000310: da04 6e61 6d65 da06 6669 656c 6473 da07  ..name..fields..
 00000320: 6f70 7469 6f6e 73da 0e43 6f6e 7461 6374  options..Contact
 00000330: 5472 6163 6b65 72da 1264 6a61 7574 6f74  Tracker..djautot
 00000340: 6173 6b5f 636f 6e74 6163 7429 04da 0864  ask_contact)...d
 00000350: 625f 7461 626c 65da 0570 726f 7879 da07  b_table..proxy..
 00000360: 696e 6465 7865 73da 0b63 6f6e 7374 7261  indexes..constra
 00000370: 696e 7473 2901 fa12 646a 6175 746f 7461  ints)...djautota
-00000380: 736b 2e63 6f6e 7461 6374 2904 721f 0000  sk.contact).r...
-00000390: 0072 2000 0000 7221 0000 00da 0562 6173  .r ...r!.....bas
+00000380: 736b 2e63 6f6e 7461 6374 2904 721e 0000  sk.contact).r...
+00000390: 0072 1f00 0000 7220 0000 00da 0562 6173  .r....r .....bas
 000003a0: 6573 da07 7072 6f6a 6563 74da 0763 6f6e  es..project..con
-000003b0: 7461 6374 7228 0000 0029 03da 0a6d 6f64  tactr(...)...mod
-000003c0: 656c 5f6e 616d 6572 1f00 0000 da05 6669  el_namer......fi
+000003b0: 7461 6374 7227 0000 0029 03da 0a6d 6f64  tactr'...)...mod
+000003c0: 656c 5f6e 616d 6572 1e00 0000 da05 6669  el_namer......fi
 000003d0: 656c 64da 0674 6963 6b65 744e 2914 da08  eld..ticketN)...
 000003e0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
 000003f0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
 00000400: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
 00000410: 7202 0000 00da 0b43 7265 6174 654d 6f64  r......CreateMod
 00000420: 656c 7203 0000 00da 0941 7574 6f46 6965  elr......AutoFie
 00000430: 6c64 da11 646a 616e 676f 5f65 7874 656e  ld..django_exten
-00000440: 7369 6f6e 73da 0264 6272 2000 0000 da15  sions..dbr .....
+00000440: 7369 6f6e 73da 0264 6272 1f00 0000 da15  sions..dbr......
 00000450: 4372 6561 7469 6f6e 4461 7465 5469 6d65  CreationDateTime
 00000460: 4669 656c 64da 194d 6f64 6966 6963 6174  Field..Modificat
 00000470: 696f 6e44 6174 6554 696d 6546 6965 6c64  ionDateTimeField
 00000480: da09 4368 6172 4669 656c 64da 0a46 6f72  ..CharField..For
 00000490: 6569 676e 4b65 79da 0664 6a61 6e67 6fda  eignKey..django.
 000004a0: 0864 656c 6574 696f 6eda 0853 4554 5f4e  .deletion..SET_N
 000004b0: 554c 4cda 0841 6464 4669 656c 64da 0a6f  ULL..AddField..o
-000004c0: 7065 7261 7469 6f6e 73a9 0072 4000 0000  perations..r@...
-000004d0: 7240 0000 00fa 622f 686f 6d65 2f72 756e  r@....b/home/run
+000004c0: 7065 7261 7469 6f6e 73a9 0072 3f00 0000  perations..r?...
+000004d0: 723f 0000 00fa 622f 686f 6d65 2f72 756e  r?....b/home/run
 000004e0: 6e65 722f 776f 726b 2f64 6a61 6e67 6f2d  ner/work/django-
 000004f0: 6175 746f 7461 736b 2f64 6a61 6e67 6f2d  autotask/django-
 00000500: 6175 746f 7461 736b 2f64 6a61 7574 6f74  autotask/djautot
 00000510: 6173 6b2f 6d69 6772 6174 696f 6e73 2f30  ask/migrations/0
 00000520: 3038 365f 6175 746f 5f32 3032 3031 3232  086_auto_2020122
 00000530: 325f 3134 3032 2e70 7972 0400 0000 0800  2_1402.pyr......
 00000540: 0000 734a 0000 0008 0302 ff04 0504 0102  ..sJ............
 00000550: 0214 0114 0114 0112 0112 0112 011c f902  ................
 00000560: 0a02 0102 fe04 f504 1004 0102 0102 0302  ................
 00000570: 0102 0102 0102 fc04 0602 f604 0c04 0102  ................
 00000580: 0102 0118 fd04 0504 0102 0102 0118 fd04  ................
 00000590: de72 0400 0000 2908 da09 646a 616e 676f  .r....)...django
 000005a0: 2e64 6272 0200 0000 7203 0000 00da 1964  .dbr....r......d
 000005b0: 6a61 6e67 6f2e 6462 2e6d 6f64 656c 732e  jango.db.models.
-000005c0: 6465 6c65 7469 6f6e 723b 0000 00da 1b64  deletionr;.....d
+000005c0: 6465 6c65 7469 6f6e 723a 0000 00da 1b64  deletionr:.....d
 000005d0: 6a61 6e67 6f5f 6578 7465 6e73 696f 6e73  jango_extensions
-000005e0: 2e64 622e 6669 656c 6473 7235 0000 0072  .db.fieldsr5...r
-000005f0: 0400 0000 7240 0000 0072 4000 0000 7240  ....r@...r@...r@
-00000600: 0000 0072 4100 0000 da08 3c6d 6f64 756c  ...rA.....<modul
+000005e0: 2e64 622e 6669 656c 6473 7234 0000 0072  .db.fieldsr4...r
+000005f0: 0400 0000 723f 0000 0072 3f00 0000 723f  ....r?...r?...r?
+00000600: 0000 0072 4000 0000 da08 3c6d 6f64 756c  ...r@.....<modul
 00000610: 653e 0300 0000 7306 0000 0010 0108 0108  e>....s.........
 00000620: 03                                       .
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0087_auto_20210108_1214.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0087_auto_20210108_1214.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 3114 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 2a0c 0000  U.........Kd*...
+00000000: 550d 0d0a 0000 0000 3268 4c64 2a0c 0000  U.......2hLd*...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
@@ -30,15 +30,15 @@
 000001d0: 0264 068d 0365 046a 0564 1364 0365 066a  .d...e.j.d.d.e.j
 000001e0: 0764 0464 0464 058d 0264 068d 0365 046a  .d.d.d...d...e.j
 000001f0: 0564 1464 0365 066a 0764 0464 0464 058d  .d.d.e.j.d.d.d..
 00000200: 0264 068d 0365 046a 0564 1564 0365 066a  .d...e.j.d.d.e.j
 00000210: 0764 0464 0464 058d 0264 068d 0367 105a  .d.d.d...d...g.Z
 00000220: 0864 1653 0029 17da 094d 6967 7261 7469  .d.S.)...Migrati
 00000230: 6f6e 2902 da0a 646a 6175 746f 7461 736b  on)...djautotask
-00000240: 5a17 3030 3836 5f61 7574 6f5f 3230 3230  Z.0086_auto_2020
+00000240: da17 3030 3836 5f61 7574 6f5f 3230 3230  ..0086_auto_2020
 00000250: 3132 3232 5f31 3430 325a 0b61 6363 6f75  1222_1402Z.accou
 00000260: 6e74 7479 7065 da0a 736f 7274 5f6f 7264  nttype..sort_ord
 00000270: 6572 5429 02da 0562 6c61 6e6b da04 6e75  erT)...blank..nu
 00000280: 6c6c 2903 da0a 6d6f 6465 6c5f 6e61 6d65  ll)...model_name
 00000290: da04 6e61 6d65 da05 6669 656c 64da 0c64  ..name..field..d
 000002a0: 6973 706c 6179 636f 6c6f 72da 0969 7373  isplaycolor..iss
 000002b0: 7565 7479 7065 da0b 6c69 6365 6e73 6574  uetype..licenset
@@ -53,16 +53,16 @@
 00000340: 7474 7970 655a 0775 7365 7479 7065 4e29  ttypeZ.usetypeN)
 00000350: 09da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
 00000360: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
 00000370: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
 00000380: 6965 7372 0200 0000 da0a 416c 7465 7246  iesr......AlterF
 00000390: 6965 6c64 7203 0000 00da 1450 6f73 6974  ieldr......Posit
 000003a0: 6976 6549 6e74 6567 6572 4669 656c 64da  iveIntegerField.
-000003b0: 0a6f 7065 7261 7469 6f6e 73a9 0072 1e00  .operations..r..
-000003c0: 0000 721e 0000 00fa 622f 686f 6d65 2f72  ..r.....b/home/r
+000003b0: 0a6f 7065 7261 7469 6f6e 73a9 0072 1f00  .operations..r..
+000003c0: 0000 721f 0000 00fa 622f 686f 6d65 2f72  ..r.....b/home/r
 000003d0: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
 000003e0: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
 000003f0: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
 00000400: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
 00000410: 2f30 3038 375f 6175 746f 5f32 3032 3130  /0087_auto_20210
 00000420: 3130 385f 3132 3134 2e70 7972 0400 0000  108_1214.pyr....
 00000430: 0600 0000 73a6 0000 0008 0302 ff04 0504  ....s...........
@@ -74,10 +74,10 @@
 00000490: 0102 0102 010c fd04 0504 0102 0102 010c  ................
 000004a0: fd04 0504 0102 0102 010c fd04 0504 0102  ................
 000004b0: 0102 010c fd04 0504 0102 0102 010c fd04  ................
 000004c0: 0504 0102 0102 010c fd04 0504 0102 0102  ................
 000004d0: 010c fd04 0504 0102 0102 010c fd04 b472  ...............r
 000004e0: 0400 0000 4e29 04da 0964 6a61 6e67 6f2e  ....N)...django.
 000004f0: 6462 7202 0000 0072 0300 0000 7204 0000  dbr....r....r...
-00000500: 0072 1e00 0000 721e 0000 0072 1e00 0000  .r....r....r....
-00000510: 721f 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
+00000500: 0072 1f00 0000 721f 0000 0072 1f00 0000  .r....r....r....
+00000510: 7220 0000 00da 083c 6d6f 6475 6c65 3e03  r .....<module>.
 00000520: 0000 0073 0200 0000 1003                 ...s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0087_auto_20210108_1307.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0087_auto_20210108_1307.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1141 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 7504 0000  U.........Kdu...
+00000000: 550d 0d0a 0000 0000 3268 4c64 7504 0000  U.......2hLdu...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0089_auto_20210125_1649.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0089_auto_20210125_1649.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1705 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 a906 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 a906 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
@@ -19,15 +19,15 @@
 00000120: 046a 0564 0264 0c65 066a 0764 0464 0564  .j.d.d.e.j.d.d.d
 00000130: 0464 068d 0364 078d 0365 046a 0564 0264  .d...d...e.j.d.d
 00000140: 0d65 066a 0764 0464 0564 0464 068d 0364  .e.j.d.d.d.d...d
 00000150: 078d 0365 046a 0564 0264 0e65 066a 0764  ...e.j.d.d.e.j.d
 00000160: 0464 0564 0464 068d 0364 078d 0367 085a  .d.d.d...d...g.Z
 00000170: 0864 0f53 0029 10da 094d 6967 7261 7469  .d.S.)...Migrati
 00000180: 6f6e 2902 da0a 646a 6175 746f 7461 736b  on)...djautotask
-00000190: da18 3030 3838 5f6d 6572 6765 5f32 3032  ..0088_merge_202
+00000190: 5a18 3030 3838 5f6d 6572 6765 5f32 3032  Z.0088_merge_202
 000001a0: 3130 3131 335f 3137 3433 da07 636f 6e74  10113_1743..cont
 000001b0: 6163 74da 0f61 6c74 6572 6e61 7465 5f70  act..alternate_p
 000001c0: 686f 6e65 54e9 c800 0000 2903 da05 626c  honeT.....)...bl
 000001d0: 616e 6bda 0a6d 6178 5f6c 656e 6774 68da  ank..max_length.
 000001e0: 046e 756c 6c29 03da 0a6d 6f64 656c 5f6e  .null)...model_n
 000001f0: 616d 65da 046e 616d 65da 0566 6965 6c64  ame..name..field
 00000200: da0d 656d 6169 6c5f 6164 6472 6573 73da  ..email_address.
@@ -38,25 +38,25 @@
 00000250: 686f 6e65 da05 7068 6f6e 654e 2909 da08  hone..phoneN)...
 00000260: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
 00000270: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
 00000280: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
 00000290: 7202 0000 00da 0a41 6c74 6572 4669 656c  r......AlterFiel
 000002a0: 6472 0300 0000 da09 4368 6172 4669 656c  dr......CharFiel
 000002b0: 64da 0a6f 7065 7261 7469 6f6e 73a9 0072  d..operations..r
-000002c0: 1e00 0000 721e 0000 00fa 622f 686f 6d65  ....r.....b/home
+000002c0: 1d00 0000 721d 0000 00fa 622f 686f 6d65  ....r.....b/home
 000002d0: 2f72 756e 6e65 722f 776f 726b 2f64 6a61  /runner/work/dja
 000002e0: 6e67 6f2d 6175 746f 7461 736b 2f64 6a61  ngo-autotask/dja
 000002f0: 6e67 6f2d 6175 746f 7461 736b 2f64 6a61  ngo-autotask/dja
 00000300: 7574 6f74 6173 6b2f 6d69 6772 6174 696f  utotask/migratio
 00000310: 6e73 2f30 3038 395f 6175 746f 5f32 3032  ns/0089_auto_202
 00000320: 3130 3132 355f 3136 3439 2e70 7972 0400  10125_1649.pyr..
 00000330: 0000 0600 0000 7356 0000 0008 0302 ff04  ......sV........
 00000340: 0504 0102 0102 010e fd04 0504 0102 0102  ................
 00000350: 010e fd04 0504 0102 0102 010e fd04 0504  ................
 00000360: 0102 0102 010e fd04 0504 0102 0102 010e  ................
 00000370: fd04 0504 0102 0102 010e fd04 0504 0102  ................
 00000380: 0102 010e fd04 0504 0102 0102 010e fd04  ................
 00000390: dc72 0400 0000 4e29 04da 0964 6a61 6e67  .r....N)...djang
 000003a0: 6f2e 6462 7202 0000 0072 0300 0000 7204  o.dbr....r....r.
-000003b0: 0000 0072 1e00 0000 721e 0000 0072 1e00  ...r....r....r..
-000003c0: 0000 721f 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000003b0: 0000 0072 1d00 0000 721d 0000 0072 1d00  ...r....r....r..
+000003c0: 0000 721e 0000 00da 083c 6d6f 6475 6c65  ..r......<module
 000003d0: 3e03 0000 0073 0200 0000 1003            >....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0090_auto_20210309_1157.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0101_auto_20220104_1349.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 425 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 a901 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 7601 0000  U.......2hLdv...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
-00000070: 0000 0000 0000 0500 0000 4000 0000 7328  ..........@...s(
+00000070: 0000 0000 0000 0400 0000 4000 0000 7326  ..........@...s&
 00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
-00000090: 0365 046a 0564 0264 0364 0464 059c 0264  .e.j.d.d.d.d...d
-000000a0: 068d 0267 015a 0664 0753 0029 08da 094d  ...g.Z.d.S.)...M
-000000b0: 6967 7261 7469 6f6e 2902 da0a 646a 6175  igration)...djau
-000000c0: 746f 7461 736b 5a17 3030 3839 5f61 7574  totaskZ.0089_aut
-000000d0: 6f5f 3230 3231 3031 3235 5f31 3634 39da  o_20210125_1649.
-000000e0: 0974 696d 6565 6e74 7279 2903 7a10 2d73  .timeentry).z.-s
-000000f0: 7461 7274 5f64 6174 655f 7469 6d65 7a0c  tart_date_timez.
-00000100: 2d64 6174 655f 776f 726b 6564 7a03 2d69  -date_workedz.-i
-00000110: 647a 0c54 696d 6520 656e 7472 6965 7329  dz.Time entries)
-00000120: 02da 086f 7264 6572 696e 67da 1376 6572  ...ordering..ver
-00000130: 626f 7365 5f6e 616d 655f 706c 7572 616c  bose_name_plural
-00000140: 2902 da04 6e61 6d65 da07 6f70 7469 6f6e  )...name..option
-00000150: 734e 2907 da08 5f5f 6e61 6d65 5f5f da0a  sN)...__name__..
-00000160: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000170: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
-00000180: 656e 6369 6573 7202 0000 00da 1141 6c74  enciesr......Alt
-00000190: 6572 4d6f 6465 6c4f 7074 696f 6e73 da0a  erModelOptions..
-000001a0: 6f70 6572 6174 696f 6e73 a900 7210 0000  operations..r...
-000001b0: 0072 1000 0000 fa62 2f68 6f6d 652f 7275  .r.....b/home/ru
-000001c0: 6e6e 6572 2f77 6f72 6b2f 646a 616e 676f  nner/work/django
-000001d0: 2d61 7574 6f74 6173 6b2f 646a 616e 676f  -autotask/django
-000001e0: 2d61 7574 6f74 6173 6b2f 646a 6175 746f  -autotask/djauto
-000001f0: 7461 736b 2f6d 6967 7261 7469 6f6e 732f  task/migrations/
-00000200: 3030 3930 5f61 7574 6f5f 3230 3231 3033  0090_auto_202103
-00000210: 3039 5f31 3135 372e 7079 7203 0000 0006  09_1157.pyr.....
-00000220: 0000 0073 0e00 0000 0803 02ff 0405 0401  ...s............
-00000230: 0201 08fe 04ff 7203 0000 004e 2903 da09  ......r....N)...
-00000240: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
-00000250: 0000 0072 1000 0000 7210 0000 0072 1000  ...r....r....r..
-00000260: 0000 7211 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000270: 3e03 0000 0073 0200 0000 0c03            >....s......
+00000090: 0365 046a 0564 0264 0364 0469 0164 058d  .e.j.d.d.d.i.d..
+000000a0: 0267 015a 0664 0653 0029 07da 094d 6967  .g.Z.d.S.)...Mig
+000000b0: 7261 7469 6f6e 2902 da0a 646a 6175 746f  ration)...djauto
+000000c0: 7461 736b 5a17 3031 3030 5f61 7574 6f5f  taskZ.0100_auto_
+000000d0: 3230 3231 3132 3238 5f31 3434 335a 0c74  20211228_1443Z.t
+000000e0: 6173 6b63 6174 6567 6f72 79da 1376 6572  askcategory..ver
+000000f0: 626f 7365 5f6e 616d 655f 706c 7572 616c  bose_name_plural
+00000100: 7a0f 5461 736b 2063 6174 6567 6f72 6965  z.Task categorie
+00000110: 7329 02da 046e 616d 65da 076f 7074 696f  s)...name..optio
+00000120: 6e73 4e29 07da 085f 5f6e 616d 655f 5fda  nsN)...__name__.
+00000130: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000140: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
+00000150: 6465 6e63 6965 7372 0200 0000 da11 416c  denciesr......Al
+00000160: 7465 724d 6f64 656c 4f70 7469 6f6e 73da  terModelOptions.
+00000170: 0a6f 7065 7261 7469 6f6e 73a9 0072 0e00  .operations..r..
+00000180: 0000 720e 0000 00fa 622f 686f 6d65 2f72  ..r.....b/home/r
+00000190: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
+000001a0: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
+000001b0: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
+000001c0: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
+000001d0: 2f30 3130 315f 6175 746f 5f32 3032 3230  /0101_auto_20220
+000001e0: 3130 345f 3133 3439 2e70 7972 0300 0000  104_1349.pyr....
+000001f0: 0600 0000 730e 0000 0008 0302 ff04 0504  ....s...........
+00000200: 0102 0106 fe04 ff72 0300 0000 4e29 03da  .......r....N)..
+00000210: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
+00000220: 0300 0000 720e 0000 0072 0e00 0000 720e  ....r....r....r.
+00000230: 0000 0072 0f00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000240: 653e 0300 0000 7302 0000 000c 03         e>....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0091_auto_20210525_1723.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0023_auto_20191119_0923.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 417 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 a101 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 9101 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00000080: 0000 0800 0000 4000 0000 7330 0000 0065  ......@...s0...e
+00000080: 0000 0600 0000 4000 0000 732c 0000 0065  ......@...s,...e
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
-000000a0: 0564 0264 0365 066a 0764 0464 0564 0464  .d.d.e.j.d.d.d.d
-000000b0: 068d 0364 078d 0367 015a 0864 0853 0029  ...d...g.Z.d.S.)
-000000c0: 09da 094d 6967 7261 7469 6f6e 2902 da0a  ...Migration)...
-000000d0: 646a 6175 746f 7461 736b da17 3030 3930  djautotask..0090
-000000e0: 5f61 7574 6f5f 3230 3231 3033 3039 5f31  _auto_20210309_1
-000000f0: 3135 37da 0474 6173 6bda 0b64 6573 6372  157..task..descr
-00000100: 6970 7469 6f6e 5469 401f 0000 2903 da05  iptionTi@...)...
-00000110: 626c 616e 6bda 0a6d 6178 5f6c 656e 6774  blank..max_lengt
-00000120: 68da 046e 756c 6c29 03da 0a6d 6f64 656c  h..null)...model
-00000130: 5f6e 616d 65da 046e 616d 65da 0566 6965  _name..name..fie
-00000140: 6c64 4e29 09da 085f 5f6e 616d 655f 5fda  ldN)...__name__.
-00000150: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000160: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
-00000170: 6465 6e63 6965 7372 0200 0000 da0a 416c  denciesr......Al
-00000180: 7465 7246 6965 6c64 7203 0000 00da 0954  terFieldr......T
-00000190: 6578 7446 6965 6c64 da0a 6f70 6572 6174  extField..operat
-000001a0: 696f 6e73 a900 7216 0000 0072 1600 0000  ions..r....r....
-000001b0: fa62 2f68 6f6d 652f 7275 6e6e 6572 2f77  .b/home/runner/w
-000001c0: 6f72 6b2f 646a 616e 676f 2d61 7574 6f74  ork/django-autot
-000001d0: 6173 6b2f 646a 616e 676f 2d61 7574 6f74  ask/django-autot
-000001e0: 6173 6b2f 646a 6175 746f 7461 736b 2f6d  ask/djautotask/m
-000001f0: 6967 7261 7469 6f6e 732f 3030 3931 5f61  igrations/0091_a
-00000200: 7574 6f5f 3230 3231 3035 3235 5f31 3732  uto_20210525_172
-00000210: 332e 7079 7204 0000 0006 0000 0073 1000  3.pyr........s..
-00000220: 0000 0803 02ff 0405 0401 0201 0201 0efd  ................
-00000230: 04ff 7204 0000 004e 2904 da09 646a 616e  ..r....N)...djan
-00000240: 676f 2e64 6272 0200 0000 7203 0000 0072  go.dbr....r....r
-00000250: 0400 0000 7216 0000 0072 1600 0000 7216  ....r....r....r.
-00000260: 0000 0072 1700 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000270: 653e 0300 0000 7302 0000 0010 03         e>....s......
+000000a0: 0564 0264 0365 066a 0764 0464 058d 0164  .d.d.e.j.d.d...d
+000000b0: 068d 0367 015a 0864 0753 0029 08da 094d  ...g.Z.d.S.)...M
+000000c0: 6967 7261 7469 6f6e 2902 da0a 646a 6175  igration)...djau
+000000d0: 746f 7461 736b da18 3030 3232 5f6d 6572  totask..0022_mer
+000000e0: 6765 5f32 3031 3931 3033 315f 3136 3230  ge_20191031_1620
+000000f0: da07 7072 6f6a 6563 74da 0864 7572 6174  ..project..durat
+00000100: 696f 6e72 0100 0000 2901 da07 6465 6661  ionr....)...defa
+00000110: 756c 7429 03da 0a6d 6f64 656c 5f6e 616d  ult)...model_nam
+00000120: 65da 046e 616d 65da 0566 6965 6c64 4e29  e..name..fieldN)
+00000130: 09da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000140: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000150: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
+00000160: 6965 7372 0200 0000 da0a 416c 7465 7246  iesr......AlterF
+00000170: 6965 6c64 7203 0000 00da 1450 6f73 6974  ieldr......Posit
+00000180: 6976 6549 6e74 6567 6572 4669 656c 64da  iveIntegerField.
+00000190: 0a6f 7065 7261 7469 6f6e 73a9 0072 1400  .operations..r..
+000001a0: 0000 7214 0000 00fa 622f 686f 6d65 2f72  ..r.....b/home/r
+000001b0: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
+000001c0: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
+000001d0: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
+000001e0: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
+000001f0: 2f30 3032 335f 6175 746f 5f32 3031 3931  /0023_auto_20191
+00000200: 3131 395f 3039 3233 2e70 7972 0400 0000  119_0923.pyr....
+00000210: 0600 0000 7310 0000 0008 0302 ff04 0504  ....s...........
+00000220: 0102 0102 010a fd04 ff72 0400 0000 4e29  .........r....N)
+00000230: 04da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
+00000240: 0072 0300 0000 7204 0000 0072 1400 0000  .r....r....r....
+00000250: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00000260: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
+00000270: 0000 1003                                ....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0093_auto_20210629_1204.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0093_auto_20210629_1204.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 477 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 dd01 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 dd01 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
 00000080: 0000 0000 0000 0000 0000 0007 0000 0040  ...............@
 00000090: 0000 0073 3600 0000 6500 5a01 6400 5a02  ...s6...e.Z.d.Z.
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6508 6a09 6a06 6a0a 6a0b 6404 6405  j.e.j.j.j.j.d.d.
 000000c0: 8d02 6406 8d03 6701 5a0c 6407 5300 2908  ..d...g.Z.d.S.).
 000000d0: da09 4d69 6772 6174 696f 6e29 02da 0a64  ..Migration)...d
-000000e0: 6a61 7574 6f74 6173 6bda 1730 3039 325f  jautotask..0092_
+000000e0: 6a61 7574 6f74 6173 6b5a 1730 3039 325f  jautotaskZ.0092_
 000000f0: 6175 746f 5f32 3032 3130 3632 395f 3131  auto_20210629_11
 00000100: 3234 da04 7461 736b da07 7072 6f6a 6563  24..task..projec
 00000110: 747a 1264 6a61 7574 6f74 6173 6b2e 7072  tz.djautotask.pr
 00000120: 6f6a 6563 7429 02da 096f 6e5f 6465 6c65  oject)...on_dele
 00000130: 7465 da02 746f 2903 da0a 6d6f 6465 6c5f  te..to)...model_
 00000140: 6e61 6d65 da04 6e61 6d65 da05 6669 656c  name..name..fiel
 00000150: 644e 290d da08 5f5f 6e61 6d65 5f5f da0a  dN)...__name__..
 00000160: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 00000170: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
 00000180: 656e 6369 6573 7202 0000 00da 0a41 6c74  enciesr......Alt
 00000190: 6572 4669 656c 6472 0300 0000 da0a 466f  erFieldr......Fo
 000001a0: 7265 6967 6e4b 6579 da06 646a 616e 676f  reignKey..django
 000001b0: da02 6462 da08 6465 6c65 7469 6f6e da07  ..db..deletion..
 000001c0: 4341 5343 4144 45da 0a6f 7065 7261 7469  CASCADE..operati
-000001d0: 6f6e 73a9 0072 1900 0000 7219 0000 00fa  ons..r....r.....
+000001d0: 6f6e 73a9 0072 1800 0000 7218 0000 00fa  ons..r....r.....
 000001e0: 622f 686f 6d65 2f72 756e 6e65 722f 776f  b/home/runner/wo
 000001f0: 726b 2f64 6a61 6e67 6f2d 6175 746f 7461  rk/django-autota
 00000200: 736b 2f64 6a61 6e67 6f2d 6175 746f 7461  sk/django-autota
 00000210: 736b 2f64 6a61 7574 6f74 6173 6b2f 6d69  sk/djautotask/mi
 00000220: 6772 6174 696f 6e73 2f30 3039 335f 6175  grations/0093_au
 00000230: 746f 5f32 3032 3130 3632 395f 3132 3034  to_20210629_1204
 00000240: 2e70 7972 0400 0000 0700 0000 7310 0000  .pyr........s...
 00000250: 0008 0302 ff04 0504 0102 0102 0114 fd04  ................
 00000260: ff72 0400 0000 2906 da09 646a 616e 676f  .r....)...django
 00000270: 2e64 6272 0200 0000 7203 0000 00da 1964  .dbr....r......d
 00000280: 6a61 6e67 6f2e 6462 2e6d 6f64 656c 732e  jango.db.models.
-00000290: 6465 6c65 7469 6f6e 7214 0000 0072 0400  deletionr....r..
-000002a0: 0000 7219 0000 0072 1900 0000 7219 0000  ..r....r....r...
-000002b0: 0072 1a00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000290: 6465 6c65 7469 6f6e 7213 0000 0072 0400  deletionr....r..
+000002a0: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
+000002b0: 0072 1900 0000 da08 3c6d 6f64 756c 653e  .r......<module>
 000002c0: 0300 0000 7304 0000 0010 0108 03         ....s........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0094_auto_20210723_1018.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0094_auto_20210723_1018.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 797 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 1d03 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 1d03 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
@@ -11,38 +11,38 @@
 000000a0: 0564 0264 0365 066a 0764 0464 0564 068d  .d.d.e.j.d.d.d..
 000000b0: 0264 078d 0365 046a 0564 0864 0965 066a  .d...e.j.d.d.e.j
 000000c0: 0764 0464 0464 0a64 0464 0b8d 0464 078d  .d.d.d.d.d...d..
 000000d0: 0365 046a 0564 0864 0c65 066a 0764 0464  .e.j.d.d.e.j.d.d
 000000e0: 0464 0a64 0464 0b8d 0464 078d 0367 035a  .d.d.d...d...g.Z
 000000f0: 0864 0d53 0029 0eda 094d 6967 7261 7469  .d.S.)...Migrati
 00000100: 6f6e 2902 da0a 646a 6175 746f 7461 736b  on)...djautotask
-00000110: 5a17 3030 3933 5f61 7574 6f5f 3230 3231  Z.0093_auto_2021
+00000110: da17 3030 3933 5f61 7574 6f5f 3230 3231  ..0093_auto_2021
 00000120: 3036 3239 5f31 3230 34da 0761 6363 6f75  0629_1204..accou
 00000130: 6e74 da04 6e61 6d65 54e9 6400 0000 2902  nt..nameT.d...).
 00000140: da08 6462 5f69 6e64 6578 da0a 6d61 785f  ..db_index..max_
 00000150: 6c65 6e67 7468 2903 da0a 6d6f 6465 6c5f  length)...model_
-00000160: 6e61 6d65 7207 0000 00da 0566 6965 6c64  namer......field
+00000160: 6e61 6d65 7208 0000 00da 0566 6965 6c64  namer......field
 00000170: da07 636f 6e74 6163 74da 0a66 6972 7374  ..contact..first
 00000180: 5f6e 616d 65e9 c800 0000 2904 da05 626c  _name.....)...bl
-00000190: 616e 6b72 0900 0000 720a 0000 00da 046e  ankr....r......n
+00000190: 616e 6b72 0a00 0000 720b 0000 00da 046e  ankr....r......n
 000001a0: 756c 6cda 096c 6173 745f 6e61 6d65 4e29  ull..last_nameN)
 000001b0: 09da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
 000001c0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
 000001d0: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
 000001e0: 6965 7372 0200 0000 da0a 416c 7465 7246  iesr......AlterF
 000001f0: 6965 6c64 7203 0000 00da 0943 6861 7246  ieldr......CharF
 00000200: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
-00000210: a900 721a 0000 0072 1a00 0000 fa62 2f68  ..r....r.....b/h
+00000210: a900 721b 0000 0072 1b00 0000 fa62 2f68  ..r....r.....b/h
 00000220: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
 00000230: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
 00000240: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
 00000250: 646a 6175 746f 7461 736b 2f6d 6967 7261  djautotask/migra
 00000260: 7469 6f6e 732f 3030 3934 5f61 7574 6f5f  tions/0094_auto_
 00000270: 3230 3231 3037 3233 5f31 3031 382e 7079  20210723_1018.py
 00000280: 7204 0000 0006 0000 0073 2400 0000 0803  r........s$.....
 00000290: 02ff 0405 0401 0201 0201 0cfd 0405 0401  ................
 000002a0: 0201 0201 10fd 0405 0401 0201 0201 10fd  ................
 000002b0: 04f5 7204 0000 004e 2904 da09 646a 616e  ..r....N)...djan
 000002c0: 676f 2e64 6272 0200 0000 7203 0000 0072  go.dbr....r....r
-000002d0: 0400 0000 721a 0000 0072 1a00 0000 721a  ....r....r....r.
-000002e0: 0000 0072 1b00 0000 da08 3c6d 6f64 756c  ...r......<modul
+000002d0: 0400 0000 721b 0000 0072 1b00 0000 721b  ....r....r....r.
+000002e0: 0000 0072 1c00 0000 da08 3c6d 6f64 756c  ...r......<modul
 000002f0: 653e 0300 0000 7302 0000 0010 03         e>....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0094_auto_20210727_0940.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0094_auto_20210727_0940.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 608 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 6002 0000  U.........Kd`...
+00000000: 550d 0d0a 0000 0000 3268 4c64 6002 0000  U.......2hLd`...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0095_auto_20210726_1251.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0095_auto_20210726_1251.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 368 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 7001 0000  U.........Kdp...
+00000000: 550d 0d0a 0000 0000 3268 4c64 7001 0000  U.......2hLdp...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0400 0000 4000 0000 7326  ..........@...s&
 00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
 00000090: 0365 046a 0564 0264 0364 0469 0164 058d  .e.j.d.d.d.i.d..
 000000a0: 0267 015a 0664 0653 0029 07da 094d 6967  .g.Z.d.S.)...Mig
 000000b0: 7261 7469 6f6e 2902 da0a 646a 6175 746f  ration)...djauto
-000000c0: 7461 736b 5a17 3030 3934 5f61 7574 6f5f  taskZ.0094_auto_
+000000c0: 7461 736b da17 3030 3934 5f61 7574 6f5f  task..0094_auto_
 000000d0: 3230 3231 3037 3233 5f31 3031 38da 0763  20210723_1018..c
 000000e0: 6f6e 7461 6374 da08 6f72 6465 7269 6e67  ontact..ordering
 000000f0: 2902 da0a 6669 7273 745f 6e61 6d65 da09  )...first_name..
 00000100: 6c61 7374 5f6e 616d 6529 02da 046e 616d  last_name)...nam
 00000110: 65da 076f 7074 696f 6e73 4e29 07da 085f  e..optionsN)..._
 00000120: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 00000130: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
 00000140: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
 00000150: 0200 0000 da11 416c 7465 724d 6f64 656c  ......AlterModel
 00000160: 4f70 7469 6f6e 73da 0a6f 7065 7261 7469  Options..operati
-00000170: 6f6e 73a9 0072 1100 0000 7211 0000 00fa  ons..r....r.....
+00000170: 6f6e 73a9 0072 1200 0000 7212 0000 00fa  ons..r....r.....
 00000180: 622f 686f 6d65 2f72 756e 6e65 722f 776f  b/home/runner/wo
 00000190: 726b 2f64 6a61 6e67 6f2d 6175 746f 7461  rk/django-autota
 000001a0: 736b 2f64 6a61 6e67 6f2d 6175 746f 7461  sk/django-autota
 000001b0: 736b 2f64 6a61 7574 6f74 6173 6b2f 6d69  sk/djautotask/mi
 000001c0: 6772 6174 696f 6e73 2f30 3039 355f 6175  grations/0095_au
 000001d0: 746f 5f32 3032 3130 3732 365f 3132 3531  to_20210726_1251
 000001e0: 2e70 7972 0300 0000 0600 0000 730e 0000  .pyr........s...
 000001f0: 0008 0302 ff04 0504 0102 0106 fe04 ff72  ...............r
 00000200: 0300 0000 4e29 03da 0964 6a61 6e67 6f2e  ....N)...django.
-00000210: 6462 7202 0000 0072 0300 0000 7211 0000  dbr....r....r...
-00000220: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000210: 6462 7202 0000 0072 0300 0000 7212 0000  dbr....r....r...
+00000220: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
 00000230: da08 3c6d 6f64 756c 653e 0300 0000 7302  ..<module>....s.
 00000240: 0000 000c 03                             .....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0097_auto_20210819_1402.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0097_auto_20210819_1402.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 707 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 c302 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 c302 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
@@ -10,15 +10,15 @@
 00000090: 0000 0073 5000 0000 6500 5a01 6400 5a02  ...sP...e.Z.d.Z.
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6404 6405 8d01 6406 8d03 6504 6a05  j.d.d...d...e.j.
 000000c0: 6407 6408 6506 6a08 6404 6404 6509 6a0a  d.d.e.j.d.d.e.j.
 000000d0: 6a06 6a0b 6a0c 6409 640a 8d04 6406 8d03  j.j.j.d.d...d...
 000000e0: 6702 5a0d 640b 5300 290c da09 4d69 6772  g.Z.d.S.)...Migr
 000000f0: 6174 696f 6e29 02da 0a64 6a61 7574 6f74  ation)...djautot
-00000100: 6173 6b5a 1830 3039 365f 6d65 7267 655f  askZ.0096_merge_
+00000100: 6173 6bda 1830 3039 365f 6d65 7267 655f  ask..0096_merge_
 00000110: 3230 3231 3037 3238 5f31 3432 395a 1761  20210728_1429Z.a
 00000120: 6363 6f75 6e74 7068 7973 6963 616c 6c6f  ccountphysicallo
 00000130: 6361 7469 6f6e da07 7072 696d 6172 7954  cation..primaryT
 00000140: 2901 da07 6465 6661 756c 7429 03da 0a6d  )...default)...m
 00000150: 6f64 656c 5f6e 616d 65da 046e 616d 65da  odel_name..name.
 00000160: 0566 6965 6c64 da06 7469 636b 6574 da19  .field..ticket..
 00000170: 6163 636f 756e 745f 7068 7973 6963 616c  account_physical
@@ -31,24 +31,24 @@
 000001e0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
 000001f0: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
 00000200: 7202 0000 00da 0841 6464 4669 656c 6472  r......AddFieldr
 00000210: 0300 0000 da0c 426f 6f6c 6561 6e46 6965  ......BooleanFie
 00000220: 6c64 da0a 466f 7265 6967 6e4b 6579 da06  ld..ForeignKey..
 00000230: 646a 616e 676f da02 6462 da08 6465 6c65  django..db..dele
 00000240: 7469 6f6e da08 5345 545f 4e55 4c4c da0a  tion..SET_NULL..
-00000250: 6f70 6572 6174 696f 6e73 a900 721d 0000  operations..r...
-00000260: 0072 1d00 0000 fa62 2f68 6f6d 652f 7275  .r.....b/home/ru
+00000250: 6f70 6572 6174 696f 6e73 a900 721e 0000  operations..r...
+00000260: 0072 1e00 0000 fa62 2f68 6f6d 652f 7275  .r.....b/home/ru
 00000270: 6e6e 6572 2f77 6f72 6b2f 646a 616e 676f  nner/work/django
 00000280: 2d61 7574 6f74 6173 6b2f 646a 616e 676f  -autotask/django
 00000290: 2d61 7574 6f74 6173 6b2f 646a 6175 746f  -autotask/djauto
 000002a0: 7461 736b 2f6d 6967 7261 7469 6f6e 732f  task/migrations/
 000002b0: 3030 3937 5f61 7574 6f5f 3230 3231 3038  0097_auto_202108
 000002c0: 3139 5f31 3430 322e 7079 7204 0000 0007  19_1402.pyr.....
 000002d0: 0000 0073 1a00 0000 0803 02ff 0405 0401  ...s............
 000002e0: 0201 0201 0afd 0405 0401 0201 0201 18fd  ................
 000002f0: 04fa 7204 0000 0029 06da 0964 6a61 6e67  ..r....)...djang
 00000300: 6f2e 6462 7202 0000 0072 0300 0000 da19  o.dbr....r......
 00000310: 646a 616e 676f 2e64 622e 6d6f 6465 6c73  django.db.models
-00000320: 2e64 656c 6574 696f 6e72 1800 0000 7204  .deletionr....r.
-00000330: 0000 0072 1d00 0000 721d 0000 0072 1d00  ...r....r....r..
-00000340: 0000 721e 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000320: 2e64 656c 6574 696f 6e72 1900 0000 7204  .deletionr....r.
+00000330: 0000 0072 1e00 0000 721e 0000 0072 1e00  ...r....r....r..
+00000340: 0000 721f 0000 00da 083c 6d6f 6475 6c65  ..r......<module
 00000350: 3e03 0000 0073 0400 0000 1001 0803       >....s........
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0098_auto_20211029_1641.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0109_billingcode_billing_code_type.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 430 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,50 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 ae01 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 2002 0000  U.......2hLd ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
-00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
-00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
-00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
-00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00000080: 0000 0800 0000 4000 0000 7330 0000 0065  ......@...s0...e
-00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
-000000a0: 0564 0264 0365 066a 0764 0464 0564 0664  .d.d.e.j.d.d.d.d
-000000b0: 078d 0364 088d 0367 015a 0864 0953 0029  ...d...g.Z.d.S.)
-000000c0: 0ada 094d 6967 7261 7469 6f6e 2902 da0a  ...Migration)...
-000000d0: 646a 6175 746f 7461 736b da17 3030 3937  djautotask..0097
-000000e0: 5f61 7574 6f5f 3230 3231 3038 3139 5f31  _auto_20210819_1
-000000f0: 3430 32da 0570 6861 7365 da0f 6573 7469  402..phase..esti
-00000100: 6d61 7465 645f 686f 7572 73e9 0200 0000  mated_hours.....
-00000110: 6700 0000 0000 0000 00e9 0600 0000 2903  g.............).
-00000120: da0e 6465 6369 6d61 6c5f 706c 6163 6573  ..decimal_places
-00000130: da07 6465 6661 756c 74da 0a6d 6178 5f64  ..default..max_d
-00000140: 6967 6974 7329 03da 0a6d 6f64 656c 5f6e  igits)...model_n
-00000150: 616d 65da 046e 616d 65da 0566 6965 6c64  ame..name..field
-00000160: 4e29 09da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00000170: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000180: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
-00000190: 6e63 6965 7372 0200 0000 da0a 416c 7465  nciesr......Alte
-000001a0: 7246 6965 6c64 7203 0000 00da 0c44 6563  rFieldr......Dec
-000001b0: 696d 616c 4669 656c 64da 0a6f 7065 7261  imalField..opera
-000001c0: 7469 6f6e 73a9 0072 1800 0000 7218 0000  tions..r....r...
-000001d0: 00fa 622f 686f 6d65 2f72 756e 6e65 722f  ..b/home/runner/
-000001e0: 776f 726b 2f64 6a61 6e67 6f2d 6175 746f  work/django-auto
-000001f0: 7461 736b 2f64 6a61 6e67 6f2d 6175 746f  task/django-auto
-00000200: 7461 736b 2f64 6a61 7574 6f74 6173 6b2f  task/djautotask/
-00000210: 6d69 6772 6174 696f 6e73 2f30 3039 385f  migrations/0098_
-00000220: 6175 746f 5f32 3032 3131 3032 395f 3136  auto_20211029_16
-00000230: 3431 2e70 7972 0400 0000 0600 0000 7310  41.pyr........s.
-00000240: 0000 0008 0302 ff04 0504 0102 0102 010e  ................
-00000250: fd04 ff72 0400 0000 4e29 04da 0964 6a61  ...r....N)...dja
-00000260: 6e67 6f2e 6462 7202 0000 0072 0300 0000  ngo.dbr....r....
-00000270: 7204 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000280: 1800 0000 7219 0000 00da 083c 6d6f 6475  ....r......<modu
-00000290: 6c65 3e03 0000 0073 0200 0000 1003       le>....s......
+00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
+00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
+00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
+00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
+00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
+00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
+00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
+000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
+000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
+000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
+000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
+000000e0: 02da 0a64 6a61 7574 6f74 6173 6bda 2b30  ...djautotask.+0
+000000f0: 3130 385f 6269 6c6c 696e 6763 6f64 6574  108_billingcodet
+00000100: 7970 655f 6269 6c6c 696e 6763 6f64 6574  ype_billingcodet
+00000110: 7970 6574 7261 636b 6572 5a0b 6269 6c6c  ypetrackerZ.bill
+00000120: 696e 6763 6f64 65da 1162 696c 6c69 6e67  ingcode..billing
+00000130: 5f63 6f64 655f 7479 7065 547a 1a64 6a61  _code_typeTz.dja
+00000140: 7574 6f74 6173 6b2e 6269 6c6c 696e 6763  utotask.billingc
+00000150: 6f64 6574 7970 6529 04da 0562 6c61 6e6b  odetype)...blank
+00000160: da04 6e75 6c6c da09 6f6e 5f64 656c 6574  ..null..on_delet
+00000170: 65da 0274 6f29 03da 0a6d 6f64 656c 5f6e  e..to)...model_n
+00000180: 616d 65da 046e 616d 65da 0566 6965 6c64  ame..name..field
+00000190: 4e29 0dda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+000001a0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000001b0: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
+000001c0: 6e63 6965 7372 0200 0000 da08 4164 6446  nciesr......AddF
+000001d0: 6965 6c64 7203 0000 00da 0a46 6f72 6569  ieldr......Forei
+000001e0: 676e 4b65 79da 0664 6a61 6e67 6fda 0264  gnKey..django..d
+000001f0: 62da 0864 656c 6574 696f 6eda 0853 4554  b..deletion..SET
+00000200: 5f4e 554c 4cda 0a6f 7065 7261 7469 6f6e  _NULL..operation
+00000210: 73a9 0072 1a00 0000 721a 0000 00fa 6d2f  s..r....r.....m/
+00000220: 686f 6d65 2f72 756e 6e65 722f 776f 726b  home/runner/work
+00000230: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
+00000240: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
+00000250: 2f64 6a61 7574 6f74 6173 6b2f 6d69 6772  /djautotask/migr
+00000260: 6174 696f 6e73 2f30 3130 395f 6269 6c6c  ations/0109_bill
+00000270: 696e 6763 6f64 655f 6269 6c6c 696e 675f  ingcode_billing_
+00000280: 636f 6465 5f74 7970 652e 7079 7204 0000  code_type.pyr...
+00000290: 0007 0000 0073 1000 0000 0803 02ff 0405  .....s..........
+000002a0: 0401 0201 0201 18fd 04ff 7204 0000 0029  ..........r....)
+000002b0: 06da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
+000002c0: 0072 0300 0000 da19 646a 616e 676f 2e64  .r......django.d
+000002d0: 622e 6d6f 6465 6c73 2e64 656c 6574 696f  b.models.deletio
+000002e0: 6e72 1500 0000 7204 0000 0072 1a00 0000  nr....r....r....
+000002f0: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
+00000300: 083c 6d6f 6475 6c65 3e03 0000 0073 0400  .<module>....s..
+00000310: 0000 1001 0803                           ......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0099_auto_20211124_1808.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0025_auto_20191125_0939.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 528 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,36 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 1002 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 6a01 0000  U.......2hLdj...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
-00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
-00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
-00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
-00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00000080: 0000 0800 0000 4000 0000 733e 0000 0065  ......@...s>...e
-00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
-000000a0: 0564 0264 0364 0469 0164 058d 0265 046a  .d.d.d.i.d...e.j
-000000b0: 0664 0264 0665 076a 0864 0764 0864 098d  .d.d.e.j.d.d.d..
-000000c0: 0264 0a8d 0367 025a 0964 0b53 0029 0cda  .d...g.Z.d.S.)..
-000000d0: 094d 6967 7261 7469 6f6e 2902 da0a 646a  .Migration)...dj
-000000e0: 6175 746f 7461 736b 5a17 3030 3938 5f61  autotaskZ.0098_a
-000000f0: 7574 6f5f 3230 3231 3130 3239 5f31 3634  uto_20211029_164
-00000100: 31da 0863 6f6e 7472 6163 74da 086f 7264  1..contract..ord
-00000110: 6572 696e 6729 01da 046e 616d 6529 0272  ering)...name).r
-00000120: 0800 0000 da07 6f70 7469 6f6e 7372 0800  ......optionsr..
-00000130: 0000 54e9 fa00 0000 2902 da08 6462 5f69  ..T.....)...db_i
-00000140: 6e64 6578 da0a 6d61 785f 6c65 6e67 7468  ndex..max_length
-00000150: 2903 da0a 6d6f 6465 6c5f 6e61 6d65 7208  )...model_namer.
-00000160: 0000 00da 0566 6965 6c64 4e29 0ada 085f  .....fieldN)..._
-00000170: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000180: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000190: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
-000001a0: 0200 0000 da11 416c 7465 724d 6f64 656c  ......AlterModel
-000001b0: 4f70 7469 6f6e 73da 0a41 6c74 6572 4669  Options..AlterFi
-000001c0: 656c 6472 0300 0000 da09 4368 6172 4669  eldr......CharFi
-000001d0: 656c 64da 0a6f 7065 7261 7469 6f6e 73a9  eld..operations.
-000001e0: 0072 1700 0000 7217 0000 00fa 622f 686f  .r....r.....b/ho
-000001f0: 6d65 2f72 756e 6e65 722f 776f 726b 2f64  me/runner/work/d
-00000200: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
-00000210: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
-00000220: 6a61 7574 6f74 6173 6b2f 6d69 6772 6174  jautotask/migrat
-00000230: 696f 6e73 2f30 3039 395f 6175 746f 5f32  ions/0099_auto_2
-00000240: 3032 3131 3132 345f 3138 3038 2e70 7972  0211124_1808.pyr
-00000250: 0400 0000 0600 0000 7318 0000 0008 0302  ........s.......
-00000260: ff04 0504 0102 0106 fe04 0404 0102 0102  ................
-00000270: 010c fd04 fb72 0400 0000 4e29 04da 0964  .....r....N)...d
-00000280: 6a61 6e67 6f2e 6462 7202 0000 0072 0300  jango.dbr....r..
-00000290: 0000 7204 0000 0072 1700 0000 7217 0000  ..r....r....r...
-000002a0: 0072 1700 0000 7218 0000 00da 083c 6d6f  .r....r......<mo
-000002b0: 6475 6c65 3e03 0000 0073 0200 0000 1003  dule>....s......
+00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
+00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
+00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
+00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
+00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
+00000070: 0000 0000 0000 0400 0000 4000 0000 7326  ..........@...s&
+00000080: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00000090: 0267 015a 0465 056a 0664 0364 0464 058d  .g.Z.e.j.d.d.d..
+000000a0: 0267 015a 0764 0653 0029 07da 094d 6967  .g.Z.d.S.)...Mig
+000000b0: 7261 7469 6f6e 4629 02da 0a64 6a61 7574  rationF)...djaut
+000000c0: 6f74 6173 6bda 1730 3032 345f 6175 746f  otask..0024_auto
+000000d0: 5f32 3031 3931 3132 325f 3135 3136 5a0e  _20191122_1516Z.
+000000e0: 5469 636b 6574 5072 696f 7269 7479 da08  TicketPriority..
+000000f0: 5072 696f 7269 7479 2902 da08 6f6c 645f  Priority)...old_
+00000100: 6e61 6d65 da08 6e65 775f 6e61 6d65 4e29  name..new_nameN)
+00000110: 08da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000120: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000130: 616d 655f 5fda 0661 746f 6d69 63da 0c64  ame__..atomic..d
+00000140: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
+00000150: da0b 5265 6e61 6d65 4d6f 6465 6cda 0a6f  ..RenameModel..o
+00000160: 7065 7261 7469 6f6e 73a9 0072 1000 0000  perations..r....
+00000170: 7210 0000 00fa 622f 686f 6d65 2f72 756e  r.....b/home/run
+00000180: 6e65 722f 776f 726b 2f64 6a61 6e67 6f2d  ner/work/django-
+00000190: 6175 746f 7461 736b 2f64 6a61 6e67 6f2d  autotask/django-
+000001a0: 6175 746f 7461 736b 2f64 6a61 7574 6f74  autotask/djautot
+000001b0: 6173 6b2f 6d69 6772 6174 696f 6e73 2f30  ask/migrations/0
+000001c0: 3032 355f 6175 746f 5f32 3031 3931 3132  025_auto_2019112
+000001d0: 355f 3039 3339 2e70 7972 0300 0000 0600  5_0939.pyr......
+000001e0: 0000 7310 0000 0008 0104 0202 ff04 0504  ..s.............
+000001f0: 0102 0102 fe04 ff72 0300 0000 4e29 03da  .......r....N)..
+00000200: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
+00000210: 0300 0000 7210 0000 0072 1000 0000 7210  ....r....r....r.
+00000220: 0000 0072 1100 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000230: 653e 0300 0000 7302 0000 000c 03         e>....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0100_auto_20211228_1443.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0100_auto_20211228_1443.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1863 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 4707 0000  U.........KdG...
+00000000: 550d 0d0a 0000 0000 3268 4c64 4707 0000  U.......2hLdG...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6402 6c05 5a06 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6501 6a07 8303 5a07  d.d...d.e.j...Z.
 00000060: 6402 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000070: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0101_auto_20220104_1349.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0013_auto_20190923_1439.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 374 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 7601 0000  U.........Kdv...
+00000000: 550d 0d0a 0000 0000 3268 4c64 be01 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
-00000070: 0000 0000 0000 0400 0000 4000 0000 7326  ..........@...s&
+00000070: 0000 0000 0000 0500 0000 4000 0000 732e  ..........@...s.
 00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
-00000090: 0365 046a 0564 0264 0364 0469 0164 058d  .e.j.d.d.d.i.d..
-000000a0: 0267 015a 0664 0653 0029 07da 094d 6967  .g.Z.d.S.)...Mig
-000000b0: 7261 7469 6f6e 2902 da0a 646a 6175 746f  ration)...djauto
-000000c0: 7461 736b da17 3031 3030 5f61 7574 6f5f  task..0100_auto_
-000000d0: 3230 3231 3132 3238 5f31 3434 335a 0c74  20211228_1443Z.t
-000000e0: 6173 6b63 6174 6567 6f72 79da 1376 6572  askcategory..ver
-000000f0: 626f 7365 5f6e 616d 655f 706c 7572 616c  bose_name_plural
-00000100: 7a0f 5461 736b 2063 6174 6567 6f72 6965  z.Task categorie
-00000110: 7329 02da 046e 616d 65da 076f 7074 696f  s)...name..optio
-00000120: 6e73 4e29 07da 085f 5f6e 616d 655f 5fda  nsN)...__name__.
-00000130: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000140: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
-00000150: 6465 6e63 6965 7372 0200 0000 da11 416c  denciesr......Al
-00000160: 7465 724d 6f64 656c 4f70 7469 6f6e 73da  terModelOptions.
-00000170: 0a6f 7065 7261 7469 6f6e 73a9 0072 0f00  .operations..r..
-00000180: 0000 720f 0000 00fa 622f 686f 6d65 2f72  ..r.....b/home/r
-00000190: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
-000001a0: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
-000001b0: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
-000001c0: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
-000001d0: 2f30 3130 315f 6175 746f 5f32 3032 3230  /0101_auto_20220
-000001e0: 3130 345f 3133 3439 2e70 7972 0300 0000  104_1349.pyr....
-000001f0: 0600 0000 730e 0000 0008 0302 ff04 0504  ....s...........
-00000200: 0102 0106 fe04 ff72 0300 0000 4e29 03da  .......r....N)..
-00000210: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
-00000220: 0300 0000 720f 0000 0072 0f00 0000 720f  ....r....r....r.
-00000230: 0000 0072 1000 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000240: 653e 0300 0000 7302 0000 000c 03         e>....s......
+00000090: 0365 046a 0564 0264 0364 048d 0265 046a  .e.j.d.d.d...e.j
+000000a0: 0564 0564 0364 048d 0267 025a 0664 0653  .d.d.d...g.Z.d.S
+000000b0: 0029 07da 094d 6967 7261 7469 6f6e 2902  .)...Migration).
+000000c0: da0a 646a 6175 746f 7461 736b da18 3030  ..djautotask..00
+000000d0: 3132 5f6d 6572 6765 5f32 3031 3930 3932  12_merge_2019092
+000000e0: 335f 3134 3339 da0d 7072 6f6a 6563 7473  3_1439..projects
+000000f0: 7461 7475 73da 0576 616c 7565 2902 da0a  tatus..value)...
+00000100: 6d6f 6465 6c5f 6e61 6d65 da04 6e61 6d65  model_name..name
+00000110: da0b 7072 6f6a 6563 7474 7970 654e 2907  ..projecttypeN).
+00000120: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000130: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000140: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
+00000150: 6573 7202 0000 00da 0b52 656d 6f76 6546  esr......RemoveF
+00000160: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
+00000170: a900 7211 0000 0072 1100 0000 fa62 2f68  ..r....r.....b/h
+00000180: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
+00000190: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
+000001a0: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
+000001b0: 646a 6175 746f 7461 736b 2f6d 6967 7261  djautotask/migra
+000001c0: 7469 6f6e 732f 3030 3133 5f61 7574 6f5f  tions/0013_auto_
+000001d0: 3230 3139 3039 3233 5f31 3433 392e 7079  20190923_1439.py
+000001e0: 7203 0000 0006 0000 0073 1600 0000 0803  r........s......
+000001f0: 02ff 0405 0401 0201 02fe 0404 0401 0201  ................
+00000200: 02fe 04fb 7203 0000 004e 2903 da09 646a  ....r....N)...dj
+00000210: 616e 676f 2e64 6272 0200 0000 7203 0000  ango.dbr....r...
+00000220: 0072 1100 0000 7211 0000 0072 1100 0000  .r....r....r....
+00000230: 7212 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
+00000240: 0000 0073 0200 0000 0c03                 ...s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0102_auto_20220104_1655.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0102_auto_20220104_1655.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 373 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 7501 0000  U.........Kdu...
+00000000: 550d 0d0a 0000 0000 3268 4c64 7501 0000  U.......2hLdu...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0500 0000 4000 0000 7324  ..........@...s$
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0103_auto_20220106_1622.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0029_phase_last_activity_date.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 391 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 8701 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 8e01 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00000080: 0000 0600 0000 4000 0000 732c 0000 0065  ......@...s,...e
+00000080: 0000 0700 0000 4000 0000 732e 0000 0065  ......@...s....e
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
-000000a0: 0564 0264 0365 066a 0764 0464 058d 0164  .d.d.e.j.d.d...d
-000000b0: 068d 0367 015a 0864 0753 0029 08da 094d  ...g.Z.d.S.)...M
-000000c0: 6967 7261 7469 6f6e 2902 da0a 646a 6175  igration)...djau
-000000d0: 746f 7461 736b 5a17 3031 3032 5f61 7574  totaskZ.0102_aut
-000000e0: 6f5f 3230 3232 3031 3034 5f31 3635 35da  o_20220104_1655.
-000000f0: 0872 6573 6f75 7263 65da 0565 6d61 696c  .resource..email
-00000100: e9fa 0000 0029 01da 0a6d 6178 5f6c 656e  .....)...max_len
-00000110: 6774 6829 03da 0a6d 6f64 656c 5f6e 616d  gth)...model_nam
-00000120: 65da 046e 616d 65da 0566 6965 6c64 4e29  e..name..fieldN)
-00000130: 09da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000140: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000150: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
-00000160: 6965 7372 0200 0000 da0a 416c 7465 7246  iesr......AlterF
-00000170: 6965 6c64 7203 0000 00da 0943 6861 7246  ieldr......CharF
-00000180: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
-00000190: a900 7214 0000 0072 1400 0000 fa62 2f68  ..r....r.....b/h
-000001a0: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
-000001b0: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
-000001c0: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
-000001d0: 646a 6175 746f 7461 736b 2f6d 6967 7261  djautotask/migra
-000001e0: 7469 6f6e 732f 3031 3033 5f61 7574 6f5f  tions/0103_auto_
-000001f0: 3230 3232 3031 3036 5f31 3632 322e 7079  20220106_1622.py
-00000200: 7204 0000 0006 0000 0073 1000 0000 0803  r........s......
-00000210: 02ff 0405 0401 0201 0201 0afd 04ff 7204  ..............r.
-00000220: 0000 004e 2904 da09 646a 616e 676f 2e64  ...N)...django.d
-00000230: 6272 0200 0000 7203 0000 0072 0400 0000  br....r....r....
-00000240: 7214 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
-00000250: 1500 0000 da08 3c6d 6f64 756c 653e 0300  ......<module>..
-00000260: 0000 7302 0000 0010 03                   ..s......
+000000a0: 0564 0264 0365 066a 0764 0464 0464 058d  .d.d.e.j.d.d.d..
+000000b0: 0264 068d 0367 015a 0864 0753 0029 08da  .d...g.Z.d.S.)..
+000000c0: 094d 6967 7261 7469 6f6e 2902 da0a 646a  .Migration)...dj
+000000d0: 6175 746f 7461 736b da0a 3030 3238 5f70  autotask..0028_p
+000000e0: 6861 7365 da05 7068 6173 65da 126c 6173  hase..phase..las
+000000f0: 745f 6163 7469 7669 7479 5f64 6174 6554  t_activity_dateT
+00000100: 2902 da05 626c 616e 6bda 046e 756c 6c29  )...blank..null)
+00000110: 03da 0a6d 6f64 656c 5f6e 616d 65da 046e  ...model_name..n
+00000120: 616d 65da 0566 6965 6c64 4e29 09da 085f  ame..fieldN)..._
+00000130: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000140: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000150: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
+00000160: 0200 0000 da08 4164 6446 6965 6c64 7203  ......AddFieldr.
+00000170: 0000 00da 0d44 6174 6554 696d 6546 6965  .....DateTimeFie
+00000180: 6c64 da0a 6f70 6572 6174 696f 6e73 a900  ld..operations..
+00000190: 7215 0000 0072 1500 0000 fa68 2f68 6f6d  r....r.....h/hom
+000001a0: 652f 7275 6e6e 6572 2f77 6f72 6b2f 646a  e/runner/work/dj
+000001b0: 616e 676f 2d61 7574 6f74 6173 6b2f 646a  ango-autotask/dj
+000001c0: 616e 676f 2d61 7574 6f74 6173 6b2f 646a  ango-autotask/dj
+000001d0: 6175 746f 7461 736b 2f6d 6967 7261 7469  autotask/migrati
+000001e0: 6f6e 732f 3030 3239 5f70 6861 7365 5f6c  ons/0029_phase_l
+000001f0: 6173 745f 6163 7469 7669 7479 5f64 6174  ast_activity_dat
+00000200: 652e 7079 7204 0000 0006 0000 0073 1000  e.pyr........s..
+00000210: 0000 0803 02ff 0405 0401 0201 0201 0cfd  ................
+00000220: 04ff 7204 0000 004e 2904 da09 646a 616e  ..r....N)...djan
+00000230: 676f 2e64 6272 0200 0000 7203 0000 0072  go.dbr....r....r
+00000240: 0400 0000 7215 0000 0072 1500 0000 7215  ....r....r....r.
+00000250: 0000 0072 1600 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000260: 653e 0300 0000 7302 0000 0010 03         e>....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0104_rename_allocationcode_billingcode_and_more.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0104_rename_allocationcode_billingcode_and_more.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1242 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 da04 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 da04 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
 00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
 00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
 00000070: 0000 0000 0000 0a00 0000 4000 0000 7370  ..........@...sp
@@ -14,51 +14,51 @@
 000000d0: 046a 0864 1164 0e64 0f64 108d 0365 046a  .j.d.d.d.d...e.j
 000000e0: 0864 1264 0e64 0f64 108d 0367 065a 0964  .d.d.d.d...g.Z.d
 000000f0: 1353 0029 14da 094d 6967 7261 7469 6f6e  .S.)...Migration
 00000100: 2902 da0a 646a 6175 746f 7461 736b da17  )...djautotask..
 00000110: 3031 3033 5f61 7574 6f5f 3230 3232 3031  0103_auto_202201
 00000120: 3036 5f31 3632 32da 1541 6c6c 6f63 6174  06_1622..Allocat
 00000130: 696f 6e43 6f64 6554 7261 636b 6572 2901  ionCodeTracker).
-00000140: da04 6e61 6d65 5a0e 416c 6c6f 6361 7469  ..nameZ.Allocati
+00000140: da04 6e61 6d65 da0e 416c 6c6f 6361 7469  ..name..Allocati
 00000150: 6f6e 436f 6465 da0b 4269 6c6c 696e 6743  onCode..BillingC
 00000160: 6f64 6529 02da 086f 6c64 5f6e 616d 65da  ode)...old_name.
 00000170: 086e 6577 5f6e 616d 65da 1242 696c 6c69  .new_name..Billi
 00000180: 6e67 436f 6465 5472 6163 6b65 72da 1664  ngCodeTracker..d
 00000190: 6a61 7574 6f74 6173 6b5f 6269 6c6c 696e  jautotask_billin
 000001a0: 6763 6f64 6554 2904 da08 6462 5f74 6162  gcodeT)...db_tab
 000001b0: 6c65 da05 7072 6f78 79da 0769 6e64 6578  le..proxy..index
 000001c0: 6573 da0b 636f 6e73 7472 6169 6e74 7329  es..constraints)
 000001d0: 017a 1664 6a61 7574 6f74 6173 6b2e 6269  .z.djautotask.bi
 000001e0: 6c6c 696e 6763 6f64 6529 0472 0700 0000  llingcode).r....
 000001f0: da06 6669 656c 6473 da07 6f70 7469 6f6e  ..fields..option
 00000200: 73da 0562 6173 6573 da04 7461 736b da0f  s..bases..task..
 00000210: 616c 6c6f 6361 7469 6f6e 5f63 6f64 65da  allocation_code.
 00000220: 0c62 696c 6c69 6e67 5f63 6f64 6529 03da  .billing_code)..
-00000230: 0a6d 6f64 656c 5f6e 616d 6572 0900 0000  .model_namer....
-00000240: 720a 0000 00da 0674 6963 6b65 74da 0974  r......ticket..t
+00000230: 0a6d 6f64 656c 5f6e 616d 6572 0a00 0000  .model_namer....
+00000240: 720b 0000 00da 0674 6963 6b65 74da 0974  r......ticket..t
 00000250: 696d 6565 6e74 7279 4e29 0ada 085f 5f6e  imeentryN)...__n
 00000260: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
 00000270: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
 00000280: 0c64 6570 656e 6465 6e63 6965 7372 0200  .dependenciesr..
 00000290: 0000 da0b 4465 6c65 7465 4d6f 6465 6cda  ....DeleteModel.
 000002a0: 0b52 656e 616d 654d 6f64 656c da0b 4372  .RenameModel..Cr
 000002b0: 6561 7465 4d6f 6465 6cda 0b52 656e 616d  eateModel..Renam
 000002c0: 6546 6965 6c64 da0a 6f70 6572 6174 696f  eField..operatio
-000002d0: 6e73 a900 7223 0000 0072 2300 0000 fa7a  ns..r#...r#....z
+000002d0: 6e73 a900 7224 0000 0072 2400 0000 fa7a  ns..r$...r$....z
 000002e0: 2f68 6f6d 652f 7275 6e6e 6572 2f77 6f72  /home/runner/wor
 000002f0: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
 00000300: 6b2f 646a 616e 676f 2d61 7574 6f74 6173  k/django-autotas
 00000310: 6b2f 646a 6175 746f 7461 736b 2f6d 6967  k/djautotask/mig
 00000320: 7261 7469 6f6e 732f 3031 3034 5f72 656e  rations/0104_ren
 00000330: 616d 655f 616c 6c6f 6361 7469 6f6e 636f  ame_allocationco
 00000340: 6465 5f62 696c 6c69 6e67 636f 6465 5f61  de_billingcode_a
 00000350: 6e64 5f6d 6f72 652e 7079 7203 0000 0006  nd_more.pyr.....
 00000360: 0000 0073 4600 0000 0803 02ff 0405 0401  ...sF...........
 00000370: 02ff 0403 0401 0201 02fe 0404 0401 0201  ................
 00000380: 0203 0201 0201 0201 02fc 0406 02f6 040c  ................
 00000390: 0401 0201 0201 02fd 0405 0401 0201 0201  ................
 000003a0: 02fd 0405 0401 0201 0201 02fd 04e2 7203  ..............r.
 000003b0: 0000 004e 2903 da09 646a 616e 676f 2e64  ...N)...django.d
-000003c0: 6272 0200 0000 7203 0000 0072 2300 0000  br....r....r#...
-000003d0: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
+000003c0: 6272 0200 0000 7203 0000 0072 2400 0000  br....r....r$...
+000003d0: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
 000003e0: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
 000003f0: 0000 0c03                                ....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0106_ticketnote_created_by_contact.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0047_auto_20200207_1126.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 525 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 0d02 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 fa02 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
-00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
-00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
+00000080: 0000 0000 0000 0000 0000 000a 0000 0040  ...............@
+00000090: 0000 0073 5e00 0000 6500 5a01 6400 5a02  ...s^...e.Z.d.Z.
 000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
 000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
-000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
-000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
-000000e0: 02da 0a64 6a61 7574 6f74 6173 6b5a 2030  ...djautotaskZ 0
-000000f0: 3130 355f 7461 736b 6e6f 7465 5f63 7265  105_tasknote_cre
-00000100: 6174 6564 5f62 795f 636f 6e74 6163 74da  ated_by_contact.
-00000110: 0a74 6963 6b65 746e 6f74 65da 1263 7265  .ticketnote..cre
-00000120: 6174 6564 5f62 795f 636f 6e74 6163 7454  ated_by_contactT
-00000130: 7a12 646a 6175 746f 7461 736b 2e63 6f6e  z.djautotask.con
-00000140: 7461 6374 2904 da05 626c 616e 6bda 046e  tact)...blank..n
-00000150: 756c 6cda 096f 6e5f 6465 6c65 7465 da02  ull..on_delete..
-00000160: 746f 2903 da0a 6d6f 6465 6c5f 6e61 6d65  to)...model_name
-00000170: da04 6e61 6d65 da05 6669 656c 644e 290d  ..name..fieldN).
-00000180: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000190: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000001a0: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
-000001b0: 6573 7202 0000 00da 0841 6464 4669 656c  esr......AddFiel
-000001c0: 6472 0300 0000 da0a 466f 7265 6967 6e4b  dr......ForeignK
-000001d0: 6579 da06 646a 616e 676f da02 6462 da08  ey..django..db..
-000001e0: 6465 6c65 7469 6f6e da08 5345 545f 4e55  deletion..SET_NU
-000001f0: 4c4c da0a 6f70 6572 6174 696f 6e73 a900  LL..operations..
-00000200: 721a 0000 0072 1a00 0000 fa6d 2f68 6f6d  r....r.....m/hom
-00000210: 652f 7275 6e6e 6572 2f77 6f72 6b2f 646a  e/runner/work/dj
-00000220: 616e 676f 2d61 7574 6f74 6173 6b2f 646a  ango-autotask/dj
-00000230: 616e 676f 2d61 7574 6f74 6173 6b2f 646a  ango-autotask/dj
-00000240: 6175 746f 7461 736b 2f6d 6967 7261 7469  autotask/migrati
-00000250: 6f6e 732f 3031 3036 5f74 6963 6b65 746e  ons/0106_ticketn
-00000260: 6f74 655f 6372 6561 7465 645f 6279 5f63  ote_created_by_c
-00000270: 6f6e 7461 6374 2e70 7972 0400 0000 0700  ontact.pyr......
-00000280: 0000 7310 0000 0008 0302 ff04 0504 0102  ..s.............
-00000290: 0102 0118 fd04 ff72 0400 0000 2906 da09  .......r....)...
-000002a0: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
-000002b0: 0000 00da 1964 6a61 6e67 6f2e 6462 2e6d  .....django.db.m
-000002c0: 6f64 656c 732e 6465 6c65 7469 6f6e 7215  odels.deletionr.
-000002d0: 0000 0072 0400 0000 721a 0000 0072 1a00  ...r....r....r..
-000002e0: 0000 721a 0000 0072 1b00 0000 da08 3c6d  ..r....r......<m
-000002f0: 6f64 756c 653e 0300 0000 7304 0000 0010  odule>....s.....
-00000300: 0108 03                                  ...
+000000c0: 6405 6406 8d04 6407 8d03 6504 6a05 6408  d.d...d...e.j.d.
+000000d0: 6403 6506 6a07 6404 6404 6508 6a09 6a06  d.e.j.d.d.e.j.j.
+000000e0: 6a0a 6a0b 6405 6406 8d04 6407 8d03 6702  j.j.d.d...d...g.
+000000f0: 5a0c 6409 5300 290a da09 4d69 6772 6174  Z.d.S.)...Migrat
+00000100: 696f 6e29 02da 0a64 6a61 7574 6f74 6173  ion)...djautotas
+00000110: 6b5a 1730 3034 365f 6175 746f 5f32 3032  kZ.0046_auto_202
+00000120: 3030 3230 375f 3130 3032 da04 7461 736b  00207_1002..task
+00000130: da0f 616c 6c6f 6361 7469 6f6e 5f63 6f64  ..allocation_cod
+00000140: 6554 7a19 646a 6175 746f 7461 736b 2e41  eTz.djautotask.A
+00000150: 6c6c 6f63 6174 696f 6e43 6f64 6529 04da  llocationCode)..
+00000160: 0562 6c61 6e6b da04 6e75 6c6c da09 6f6e  .blank..null..on
+00000170: 5f64 656c 6574 65da 0274 6f29 03da 0a6d  _delete..to)...m
+00000180: 6f64 656c 5f6e 616d 65da 046e 616d 65da  odel_name..name.
+00000190: 0566 6965 6c64 da06 7469 636b 6574 4e29  .field..ticketN)
+000001a0: 0dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000001b0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000001c0: 616d 655f 5fda 0c64 6570 656e 6465 6e63  ame__..dependenc
+000001d0: 6965 7372 0200 0000 da08 4164 6446 6965  iesr......AddFie
+000001e0: 6c64 7203 0000 00da 0a46 6f72 6569 676e  ldr......Foreign
+000001f0: 4b65 79da 0664 6a61 6e67 6fda 0264 62da  Key..django..db.
+00000200: 0864 656c 6574 696f 6eda 0853 4554 5f4e  .deletion..SET_N
+00000210: 554c 4cda 0a6f 7065 7261 7469 6f6e 73a9  ULL..operations.
+00000220: 0072 1b00 0000 721b 0000 00fa 622f 686f  .r....r.....b/ho
+00000230: 6d65 2f72 756e 6e65 722f 776f 726b 2f64  me/runner/work/d
+00000240: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
+00000250: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
+00000260: 6a61 7574 6f74 6173 6b2f 6d69 6772 6174  jautotask/migrat
+00000270: 696f 6e73 2f30 3034 375f 6175 746f 5f32  ions/0047_auto_2
+00000280: 3032 3030 3230 375f 3131 3236 2e70 7972  0200207_1126.pyr
+00000290: 0400 0000 0700 0000 731a 0000 0008 0302  ........s.......
+000002a0: ff04 0504 0102 0102 0118 fd04 0504 0102  ................
+000002b0: 0102 0118 fd04 fa72 0400 0000 2906 da09  .......r....)...
+000002c0: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
+000002d0: 0000 00da 1964 6a61 6e67 6f2e 6462 2e6d  .....django.db.m
+000002e0: 6f64 656c 732e 6465 6c65 7469 6f6e 7216  odels.deletionr.
+000002f0: 0000 0072 0400 0000 721b 0000 0072 1b00  ...r....r....r..
+00000300: 0000 721b 0000 0072 1c00 0000 da08 3c6d  ..r....r......<m
+00000310: 6f64 756c 653e 0300 0000 7304 0000 0010  odule>....s.....
+00000320: 0108 03                                  ...
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0107_contact_extension.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0107_contact_extension.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 425 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 a901 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 a901 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0108_billingcodetype_billingcodetypetracker.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0108_billingcodetype_billingcodetypetracker.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 1600 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 4006 0000  U.........Kd@...
+00000000: 550d 0d0a 0000 0000 3268 4c64 4006 0000  U.......2hLd@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
 00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0109_billingcode_billing_code_type.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0099_auto_20211124_1808.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 544 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,44 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 2002 0000  U.........Kd ...
+00000000: 550d 0d0a 0000 0000 3268 4c64 1002 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
-00000040: 6402 6c03 5a04 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
-00000050: 6501 6a05 8303 5a05 6402 5300 2905 e900  e.j...Z.d.S.)...
-00000060: 0000 0029 02da 0a6d 6967 7261 7469 6f6e  ...)...migration
-00000070: 73da 066d 6f64 656c 734e 6300 0000 0000  s..modelsNc.....
-00000080: 0000 0000 0000 0000 0000 0009 0000 0040  ...............@
-00000090: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
-000000a0: 6401 6701 5a03 6504 6a05 6402 6403 6506  d.g.Z.e.j.d.d.e.
-000000b0: 6a07 6404 6404 6508 6a09 6a06 6a0a 6a0b  j.d.d.e.j.j.j.j.
-000000c0: 6405 6406 8d04 6407 8d03 6701 5a0c 6408  d.d...d...g.Z.d.
-000000d0: 5300 2909 da09 4d69 6772 6174 696f 6e29  S.)...Migration)
-000000e0: 02da 0a64 6a61 7574 6f74 6173 6b5a 2b30  ...djautotaskZ+0
-000000f0: 3130 385f 6269 6c6c 696e 6763 6f64 6574  108_billingcodet
-00000100: 7970 655f 6269 6c6c 696e 6763 6f64 6574  ype_billingcodet
-00000110: 7970 6574 7261 636b 6572 5a0b 6269 6c6c  ypetrackerZ.bill
-00000120: 696e 6763 6f64 65da 1162 696c 6c69 6e67  ingcode..billing
-00000130: 5f63 6f64 655f 7479 7065 547a 1a64 6a61  _code_typeTz.dja
-00000140: 7574 6f74 6173 6b2e 6269 6c6c 696e 6763  utotask.billingc
-00000150: 6f64 6574 7970 6529 04da 0562 6c61 6e6b  odetype)...blank
-00000160: da04 6e75 6c6c da09 6f6e 5f64 656c 6574  ..null..on_delet
-00000170: 65da 0274 6f29 03da 0a6d 6f64 656c 5f6e  e..to)...model_n
-00000180: 616d 65da 046e 616d 65da 0566 6965 6c64  ame..name..field
-00000190: 4e29 0dda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-000001a0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000001b0: 6c6e 616d 655f 5fda 0c64 6570 656e 6465  lname__..depende
-000001c0: 6e63 6965 7372 0200 0000 da08 4164 6446  nciesr......AddF
-000001d0: 6965 6c64 7203 0000 00da 0a46 6f72 6569  ieldr......Forei
-000001e0: 676e 4b65 79da 0664 6a61 6e67 6fda 0264  gnKey..django..d
-000001f0: 62da 0864 656c 6574 696f 6eda 0853 4554  b..deletion..SET
-00000200: 5f4e 554c 4cda 0a6f 7065 7261 7469 6f6e  _NULL..operation
-00000210: 73a9 0072 1900 0000 7219 0000 00fa 6d2f  s..r....r.....m/
-00000220: 686f 6d65 2f72 756e 6e65 722f 776f 726b  home/runner/work
-00000230: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
-00000240: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
-00000250: 2f64 6a61 7574 6f74 6173 6b2f 6d69 6772  /djautotask/migr
-00000260: 6174 696f 6e73 2f30 3130 395f 6269 6c6c  ations/0109_bill
-00000270: 696e 6763 6f64 655f 6269 6c6c 696e 675f  ingcode_billing_
-00000280: 636f 6465 5f74 7970 652e 7079 7204 0000  code_type.pyr...
-00000290: 0007 0000 0073 1000 0000 0803 02ff 0405  .....s..........
-000002a0: 0401 0201 0201 18fd 04ff 7204 0000 0029  ..........r....)
-000002b0: 06da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
-000002c0: 0072 0300 0000 da19 646a 616e 676f 2e64  .r......django.d
-000002d0: 622e 6d6f 6465 6c73 2e64 656c 6574 696f  b.models.deletio
-000002e0: 6e72 1400 0000 7204 0000 0072 1900 0000  nr....r....r....
-000002f0: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00000300: 083c 6d6f 6475 6c65 3e03 0000 0073 0400  .<module>....s..
-00000310: 0000 1001 0803                           ......
+00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
+00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
+00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
+00000080: 0000 0800 0000 4000 0000 733e 0000 0065  ......@...s>...e
+00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
+000000a0: 0564 0264 0364 0469 0164 058d 0265 046a  .d.d.d.i.d...e.j
+000000b0: 0664 0264 0665 076a 0864 0764 0864 098d  .d.d.e.j.d.d.d..
+000000c0: 0264 0a8d 0367 025a 0964 0b53 0029 0cda  .d...g.Z.d.S.)..
+000000d0: 094d 6967 7261 7469 6f6e 2902 da0a 646a  .Migration)...dj
+000000e0: 6175 746f 7461 736b da17 3030 3938 5f61  autotask..0098_a
+000000f0: 7574 6f5f 3230 3231 3130 3239 5f31 3634  uto_20211029_164
+00000100: 31da 0863 6f6e 7472 6163 74da 086f 7264  1..contract..ord
+00000110: 6572 696e 6729 01da 046e 616d 6529 0272  ering)...name).r
+00000120: 0900 0000 da07 6f70 7469 6f6e 7372 0900  ......optionsr..
+00000130: 0000 54e9 fa00 0000 2902 da08 6462 5f69  ..T.....)...db_i
+00000140: 6e64 6578 da0a 6d61 785f 6c65 6e67 7468  ndex..max_length
+00000150: 2903 da0a 6d6f 6465 6c5f 6e61 6d65 7209  )...model_namer.
+00000160: 0000 00da 0566 6965 6c64 4e29 0ada 085f  .....fieldN)..._
+00000170: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000180: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000190: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
+000001a0: 0200 0000 da11 416c 7465 724d 6f64 656c  ......AlterModel
+000001b0: 4f70 7469 6f6e 73da 0a41 6c74 6572 4669  Options..AlterFi
+000001c0: 656c 6472 0300 0000 da09 4368 6172 4669  eldr......CharFi
+000001d0: 656c 64da 0a6f 7065 7261 7469 6f6e 73a9  eld..operations.
+000001e0: 0072 1800 0000 7218 0000 00fa 622f 686f  .r....r.....b/ho
+000001f0: 6d65 2f72 756e 6e65 722f 776f 726b 2f64  me/runner/work/d
+00000200: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
+00000210: 6a61 6e67 6f2d 6175 746f 7461 736b 2f64  jango-autotask/d
+00000220: 6a61 7574 6f74 6173 6b2f 6d69 6772 6174  jautotask/migrat
+00000230: 696f 6e73 2f30 3039 395f 6175 746f 5f32  ions/0099_auto_2
+00000240: 3032 3131 3132 345f 3138 3038 2e70 7972  0211124_1808.pyr
+00000250: 0400 0000 0600 0000 7318 0000 0008 0302  ........s.......
+00000260: ff04 0504 0102 0106 fe04 0404 0102 0102  ................
+00000270: 010c fd04 fb72 0400 0000 4e29 04da 0964  .....r....N)...d
+00000280: 6a61 6e67 6f2e 6462 7202 0000 0072 0300  jango.dbr....r..
+00000290: 0000 7204 0000 0072 1800 0000 7218 0000  ..r....r....r...
+000002a0: 0072 1800 0000 7219 0000 00da 083c 6d6f  .r....r......<mo
+000002b0: 6475 6c65 3e03 0000 0073 0200 0000 1003  dule>....s......
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0110_account_phone.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0110_account_phone.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 422 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 a601 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 a601 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
```

### Comparing `django-autotask-1.0.1/djautotask/migrations/__pycache__/0111_alter_phase_estimated_hours.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/migrations/__pycache__/0111_alter_phase_estimated_hours.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 425 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 a901 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 a901 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
 00000080: 0000 0800 0000 4000 0000 7330 0000 0065  ......@...s0...e
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
 000000a0: 0564 0264 0365 066a 0764 0464 0564 0664  .d.d.e.j.d.d.d.d
 000000b0: 078d 0364 088d 0367 015a 0864 0953 0029  ...d...g.Z.d.S.)
 000000c0: 0ada 094d 6967 7261 7469 6f6e 2902 da0a  ...Migration)...
-000000d0: 646a 6175 746f 7461 736b da12 3031 3130  djautotask..0110
+000000d0: 646a 6175 746f 7461 736b 5a12 3031 3130  djautotaskZ.0110
 000000e0: 5f61 6363 6f75 6e74 5f70 686f 6e65 da05  _account_phone..
 000000f0: 7068 6173 65da 0f65 7374 696d 6174 6564  phase..estimated
 00000100: 5f68 6f75 7273 e902 0000 0067 0000 0000  _hours.....g....
 00000110: 0000 0000 e909 0000 0029 03da 0e64 6563  .........)...dec
 00000120: 696d 616c 5f70 6c61 6365 73da 0764 6566  imal_places..def
 00000130: 6175 6c74 da0a 6d61 785f 6469 6769 7473  ault..max_digits
 00000140: 2903 da0a 6d6f 6465 6c5f 6e61 6d65 da04  )...model_name..
 00000150: 6e61 6d65 da05 6669 656c 644e 2909 da08  name..fieldN)...
 00000160: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
 00000170: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
 00000180: 5f5f da0c 6465 7065 6e64 656e 6369 6573  __..dependencies
 00000190: 7202 0000 00da 0a41 6c74 6572 4669 656c  r......AlterFiel
 000001a0: 6472 0300 0000 da0c 4465 6369 6d61 6c46  dr......DecimalF
 000001b0: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
-000001c0: a900 7218 0000 0072 1800 0000 fa6b 2f68  ..r....r.....k/h
+000001c0: a900 7217 0000 0072 1700 0000 fa6b 2f68  ..r....r.....k/h
 000001d0: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
 000001e0: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
 000001f0: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
 00000200: 646a 6175 746f 7461 736b 2f6d 6967 7261  djautotask/migra
 00000210: 7469 6f6e 732f 3031 3131 5f61 6c74 6572  tions/0111_alter
 00000220: 5f70 6861 7365 5f65 7374 696d 6174 6564  _phase_estimated
 00000230: 5f68 6f75 7273 2e70 7972 0400 0000 0600  _hours.pyr......
 00000240: 0000 7310 0000 0008 0302 ff04 0504 0102  ..s.............
 00000250: 0102 010e fd04 ff72 0400 0000 4e29 04da  .......r....N)..
 00000260: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
-00000270: 0300 0000 7204 0000 0072 1800 0000 7218  ....r....r....r.
-00000280: 0000 0072 1800 0000 7219 0000 00da 083c  ...r....r......<
+00000270: 0300 0000 7204 0000 0072 1700 0000 7217  ....r....r....r.
+00000280: 0000 0072 1700 0000 7218 0000 00da 083c  ...r....r......<
 00000290: 6d6f 6475 6c65 3e03 0000 0073 0200 0000  module>....s....
 000002a0: 1003                                     ..
```

### Comparing `django-autotask-1.0.1/djautotask/models.py` & `django-autotask-1.1.1/djautotask/models.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/sync.py` & `django-autotask-1.1.1/djautotask/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import logging
+import os
+import base64
 from dateutil.parser import parse
 from decimal import Decimal
 
 from django.db import transaction, IntegrityError
 from django.db.models import Q
 from django.utils import timezone
 
@@ -10,14 +12,16 @@
 from djautotask import models
 from .api import ApiCondition as A, AutotaskRecordNotFoundError
 from .utils import DjautotaskSettings
 
 CREATED = 1
 UPDATED = 2
 SKIPPED = 3
+FILE_UMASK = 0o022
+
 
 logger = logging.getLogger(__name__)
 
 
 class InvalidObjectException(Exception):
     """
     If for any reason an object can't be created (for example, it references
@@ -1627,14 +1631,53 @@
     def _assign_field_data(self, instance, object_data):
         instance.id = object_data['id']
         self.set_relations(instance, object_data)
 
         return instance
 
 
+class AttachmentSynchronizer(Synchronizer):
+    client_class = api.AttachmentInfoAPIClient
+
+    def __init__(self, record_type=None, field=None, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.type = record_type
+        self.field = field
+
+        if kwargs.get('object_id'):
+            self.client.add_condition(
+                A(op='eq', field=self.field, value=kwargs.get('object_id'))
+            )
+
+    def download_attachment(self, object_id, attachment_id, path):
+        response = self.client.get_attachment(object_id,
+                                              attachment_id,
+                                              self.type)
+
+        filename = response.get('fullPath')
+        unique_filename = f'{attachment_id}-{filename}'
+
+        logger.debug(f'Writing attachment {unique_filename} to {path}')
+
+        file_path = os.path.join(path, f'{unique_filename}')
+        # Set permissions on file before creating and writing to it.
+        previous_umask = os.umask(FILE_UMASK)
+        data = response.get('data')
+        decoded_data = base64.b64decode(data)
+
+        with open(file_path, 'wb') as f:
+            f.write(decoded_data)
+        os.umask(previous_umask)
+
+        return unique_filename
+
+    def get_count(self):
+        return self.client.count()
+
+
 class BillingCodeSynchronizer(Synchronizer):
     client_class = api.BillingCodesAPIClient
     model_class = models.BillingCodeTracker
     last_updated_field = None
 
     related_meta = {
         'useType': (models.UseType, 'use_type'),
```

### Comparing `django-autotask-1.0.1/djautotask/tests/__pycache__/fixture_utils.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/tests/__pycache__/fixture_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 11695 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 af2d 0000  U.........Kd.-..
+00000000: 550d 0d0a 0000 0000 3268 4c64 af2d 0000  U.......2hLd.-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 a401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6404 6405 8400 5a06 6406  m.Z...d.d...Z.d.
 00000060: 6407 8400 5a07 6408 6409 8400 5a08 640a  d...Z.d.d...Z.d.
 00000070: 640b 8400 5a09 640c 640d 8400 5a0a 640e  d...Z.d.d...Z.d.
```

### Comparing `django-autotask-1.0.1/djautotask/tests/__pycache__/fixtures.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/tests/__pycache__/fixtures.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 39489 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 419a 0000  U.........KdA...
+00000000: 550d 0d0a 0000 0000 3268 4c64 419a 0000  U.......2hLdA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 002d 0000 0040 0000 0073 260b 0000 6400  .-...@...s&...d.
 00000030: 6401 6402 6402 6403 9c04 5a00 6700 6404  d.d.d.d...Z.g.d.
 00000040: 6401 6402 6402 6403 9c04 6405 9c02 5a01  d.d.d.d...d...Z.
 00000050: 6406 6700 6901 5a02 6406 6407 6407 6408  d.g.i.Z.d.d.d.d.
 00000060: 6409 640a 640b 640c 640d 6404 6402 640a  d.d.d.d.d.d.d.d.
 00000070: 640d 640e 9c07 6701 640f 9c06 6701 6901  d.d...g.d...g.i.
```

### Comparing `django-autotask-1.0.1/djautotask/tests/__pycache__/mocks.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/tests/__pycache__/mocks.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 8430 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 ee20 0000  U.........Kd. ..
+00000000: 550d 0d0a 0000 0000 3268 4c64 ee20 0000  U.......2hLd. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9a01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6461 6403 6404  Z.d.d.l.Z.dad.d.
 00000050: 8401 5a04 6462 6405 6406 8401 5a05 6463  ..Z.dbd.d...Z.dc
 00000060: 6407 6408 8401 5a06 6409 640a 8400 5a07  d.d...Z.d.d...Z.
 00000070: 640b 640c 8400 5a08 640d 640e 8400 5a09  d.d...Z.d.d...Z.
```

### Comparing `django-autotask-1.0.1/djautotask/tests/__pycache__/test_api.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/tests/__pycache__/test_api.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 6592 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 c019 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 c019 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 6406 6c08 6d09 5a0a 0100 6407  ..d.d.l.m.Z...d.
 00000070: 6408 6c08 6d0b 5a0b 0100 6407 6409 6c0b  d.l.m.Z...d.d.l.
```

### Comparing `django-autotask-1.0.1/djautotask/tests/__pycache__/test_commands.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/tests/__pycache__/test_commands.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 31888 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 907c 0000  U.........Kd.|..
+00000000: 550d 0d0a 0000 0000 3268 4c64 907c 0000  U.......2hLd.|..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e803 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6473  ..d.d.l.m.Z...ds
 00000070: 6406 6407 8401 5a0b 6474 6408 6409 8401  d.d...Z.dtd.d...
```

### Comparing `django-autotask-1.0.1/djautotask/tests/__pycache__/test_model.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/tests/__pycache__/test_model.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 3794 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 d20e 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 d20e 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c03  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6400 6406 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6407 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
```

### Comparing `django-autotask-1.0.1/djautotask/tests/__pycache__/test_sync.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/tests/__pycache__/test_sync.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 53083 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 5bcf 0000  U.........Kd[...
+00000000: 550d 0d0a 0000 0000 3268 4c64 5bcf 0000  U.......2hLd[...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 d803 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c06 6d08 5a08 0100 6400 6406 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `django-autotask-1.0.1/djautotask/tests/__pycache__/test_views.cpython-38.pyc` & `django-autotask-1.1.1/djautotask/tests/__pycache__/test_views.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 28 17:00:53 2023 UTC, .py size: 2268 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c5fb 4b64 dc08 0000  U.........Kd....
+00000000: 550d 0d0a 0000 0000 3268 4c64 dc08 0000  U.......2hLd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 4700 6405 6406  m.Z.m.Z...G.d.d.
 00000070: 8400 6406 6504 8303 5a0b 6407 5300 2908  ..d.e...Z.d.S.).
```

### Comparing `django-autotask-1.0.1/djautotask/tests/fixture_utils.py` & `django-autotask-1.1.1/djautotask/tests/fixture_utils.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/tests/fixtures.py` & `django-autotask-1.1.1/djautotask/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/tests/mocks.py` & `django-autotask-1.1.1/djautotask/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/tests/test_api.py` & `django-autotask-1.1.1/djautotask/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/tests/test_commands.py` & `django-autotask-1.1.1/djautotask/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/tests/test_model.py` & `django-autotask-1.1.1/djautotask/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/tests/test_sync.py` & `django-autotask-1.1.1/djautotask/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/tests/test_views.py` & `django-autotask-1.1.1/djautotask/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/djautotask/views.py` & `django-autotask-1.1.1/djautotask/views.py`

 * *Files identical despite different names*

### Comparing `django-autotask-1.0.1/setup.py` & `django-autotask-1.1.1/setup.py`

 * *Files identical despite different names*

