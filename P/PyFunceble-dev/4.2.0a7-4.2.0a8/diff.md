# Comparing `tmp/PyFunceble-dev-4.2.0a7.tar.gz` & `tmp/PyFunceble-dev-4.2.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFunceble-dev-4.2.0a7.tar", last modified: Sun Jan  8 12:06:40 2023, max compression
+gzip compressed data, was "PyFunceble-dev-4.2.0a8.tar", last modified: Sat Apr 29 16:43:44 2023, max compression
```

## Comparing `PyFunceble-dev-4.2.0a7.tar` & `PyFunceble-dev-4.2.0a8.tar`

### file list

```diff
@@ -1,350 +1,348 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.178163 PyFunceble-dev-4.2.0a7/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-01-08 12:06:40.178163 PyFunceble-dev-4.2.0a7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.126163 PyFunceble-dev-4.2.0a7/PyFunceble/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.126163 PyFunceble-dev-4.2.0a7/PyFunceble/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.130163 PyFunceble-dev-4.2.0a7/PyFunceble/checker/
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.130163 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/domain_and_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.130163 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/extras/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/extras/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/extras/parked.py
--rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/extras/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/extras/subject_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/complex_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/params_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.134163 PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/domain_and_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/status_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.138163 PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/domain_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/second_lvl_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/subdomain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.138163 PyFunceble-dev-4.2.0a7/PyFunceble/checker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/checker/utils/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.138163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.138163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38941 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/travis_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/credential_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.138163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/iana.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/public_suffix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.142163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/pyfunceble/
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/pyfunceble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/pyfunceble/argsparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    45945 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/pyfunceble/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/execution_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/file_preloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.142163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/dir_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.146163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/dir_structure/
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/dir_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/dir_structure/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/dir_structure/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/dir_structure/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/json_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.146163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/printer/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/printer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/printer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/printer/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/printer/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/registrar_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24044 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/status_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.146163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/alembic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.146163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/csv_file/
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/csv_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/csv_file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/db_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.146163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/file_cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/file_cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/file_cleanup/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/file_cleanup/hashes_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/file_cleanup/mining_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/file_cleanup/production_config_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.150163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/json2csv/
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/json2csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/json2csv/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/json2csv/inactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/json2csv/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.150163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/mariadb/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/mariadb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/mariadb/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/mariadb/file_and_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.150163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/chancy_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/chancy_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/dir_files_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/file_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/migrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/miner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.154163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/chancy_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/chancy_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/dir_files_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/file_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/file_sorter_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/migrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/miner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16660 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.154163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/scripts/iana.py
--rw-r--r--   0 runner    (1001) docker     (123)    17912 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/scripts/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/scripts/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/storage_facility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.154163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/system/
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/system/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/system/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    40350 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/system/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.154163 PyFunceble-dev-4.2.0a7/PyFunceble/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/utils/ascii_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/utils/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/cli/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.154163 PyFunceble-dev-4.2.0a7/PyFunceble/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/config/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/config/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.158163 PyFunceble-dev-4.2.0a7/PyFunceble/converter/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12833 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/converter/adblock_input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/converter/cidr2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/converter/input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/converter/internal_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/converter/rpz_input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/converter/rpz_policy2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/converter/subject2complements.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/converter/url2netloc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/converter/wildcard2subject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.158163 PyFunceble-dev-4.2.0a7/PyFunceble/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.158163 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.158163 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.162163 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.162163 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/postgresql/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/postgresql/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.162163 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/postgresql/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/postgresql/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.162163 PyFunceble-dev-4.2.0a7/PyFunceble/data/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/infrastructure/.PyFunceble_production.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/data/infrastructure/dir_structure_production.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.162163 PyFunceble-dev-4.2.0a7/PyFunceble/database/
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.162163 PyFunceble-dev-4.2.0a7/PyFunceble/database/credential/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/credential/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/credential/mariadb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/credential/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/credential/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.166163 PyFunceble-dev-4.2.0a7/PyFunceble/database/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/schemas/autocontinue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/schemas/inactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/schemas/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/schemas/whois_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.166163 PyFunceble-dev-4.2.0a7/PyFunceble/database/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/sqlalchemy/all_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/database/sqlalchemy/base_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.166163 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.166163 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/autocontinue/
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/autocontinue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/autocontinue/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/autocontinue/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/autocontinue/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/csv_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/db_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/iana.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.166163 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/inactive/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/inactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/inactive/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/inactive/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/inactive/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/ipv4_reputation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/sql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/user_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.170163 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/whois/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/whois/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/whois/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/dataset/whois/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.170163 PyFunceble-dev-4.2.0a7/PyFunceble/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/downloader/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/downloader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/downloader/iana.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/downloader/ipv4_reputation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/downloader/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/downloader/user_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.170163 PyFunceble-dev-4.2.0a7/PyFunceble/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/helpers/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/helpers/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/helpers/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/helpers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/helpers/environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/helpers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/helpers/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/helpers/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/helpers/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/helpers/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.170163 PyFunceble-dev-4.2.0a7/PyFunceble/query/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17478 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.174163 PyFunceble-dev-4.2.0a7/PyFunceble/query/dns/
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/dns/nameserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    32788 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/dns/query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/dns/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/http_status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.174163 PyFunceble-dev-4.2.0a7/PyFunceble/query/netinfo/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/netinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/netinfo/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/netinfo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/netinfo/hostbyaddr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.174163 PyFunceble-dev-4.2.0a7/PyFunceble/query/record/
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/record/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/record/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/record/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.174163 PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.174163 PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/adapter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/adapter/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/adapter/https.py
--rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.174163 PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.178163 PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/converter/
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/converter/digit2digits.py
--rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/converter/expiration_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/converter/month2unified.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/converter/registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/storage_facility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.178163 PyFunceble-dev-4.2.0a7/PyFunceble/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/utils/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/utils/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/PyFunceble/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 12:06:40.178163 PyFunceble-dev-4.2.0a7/PyFunceble_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-01-08 12:06:39.000000 PyFunceble-dev-4.2.0a7/PyFunceble_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-01-08 12:06:40.000000 PyFunceble-dev-4.2.0a7/PyFunceble_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 12:06:39.000000 PyFunceble-dev-4.2.0a7/PyFunceble_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-08 12:06:39.000000 PyFunceble-dev-4.2.0a7/PyFunceble_dev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-01-08 12:06:39.000000 PyFunceble-dev-4.2.0a7/PyFunceble_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-08 12:06:39.000000 PyFunceble-dev-4.2.0a7/PyFunceble_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/requirements.docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/requirements.win.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-01-08 12:06:40.182163 PyFunceble-dev-4.2.0a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-01-08 12:06:26.000000 PyFunceble-dev-4.2.0a7/version.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.565257 PyFunceble-dev-4.2.0a8/PyFunceble/
+-rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.565257 PyFunceble-dev-4.2.0a8/PyFunceble/checker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.565257 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/domain_and_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.569258 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/parked.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/subject_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/complex_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/params_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.569258 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/domain_and_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/status_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.569258 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/domain_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/second_lvl_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/subdomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.573258 PyFunceble-dev-4.2.0a8/PyFunceble/checker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/utils/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.573258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.573258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38941 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/travis_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/credential_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.573258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/iana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/public_suffix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.573258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/argsparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45945 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/execution_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/file_preloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.577258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.577258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/json_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.577258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/registrar_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24044 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/status_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.577258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/alembic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.577258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/db_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.581258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/hashes_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/mining_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/production_config_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.581258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/inactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.581258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/file_and_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.581258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/chancy_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/chancy_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/dir_files_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/file_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/migrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/miner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.585258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/chancy_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/chancy_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/dir_files_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/file_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/file_sorter_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/migrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/miner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16601 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.585258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/iana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17912 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/storage_facility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.585258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40349 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.585258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/ascii_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.585258 PyFunceble-dev-4.2.0a8/PyFunceble/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/config/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/config/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.589258 PyFunceble-dev-4.2.0a8/PyFunceble/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/adblock_input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/cidr2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/internal_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/rpz_input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/rpz_policy2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/subject2complements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/url2netloc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/wildcard2subject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.589258 PyFunceble-dev-4.2.0a8/PyFunceble/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.589258 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.589258 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.589258 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/data/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/infrastructure/.PyFunceble_production.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/infrastructure/dir_structure_production.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/autocontinue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/inactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/whois_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/all_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/base_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.597258 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.597258 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/csv_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/db_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/iana.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.597258 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/ipv4_reputation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/sql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/user_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.597258 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.597258 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/iana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/ipv4_reputation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/user_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.601258 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.601258 PyFunceble-dev-4.2.0a8/PyFunceble/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.601258 PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/nameserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32788 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/http_status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.601258 PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/hostbyaddr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.601258 PyFunceble-dev-4.2.0a8/PyFunceble/query/record/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/record/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/record/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/record/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.601258 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/https.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/digit2digits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/expiration_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/month2unified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/storage_facility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/PyFunceble/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/utils/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/utils/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-29 16:43:44.000000 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-04-29 16:43:44.000000 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:43:44.000000 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-29 16:43:44.000000 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-29 16:43:44.000000 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 16:43:44.000000 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/requirements.docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/requirements.win.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-29 16:43:44.609258 PyFunceble-dev-4.2.0a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/version.yaml
```

### Comparing `PyFunceble-dev-4.2.0a7/CODE_OF_CONDUCT.rst` & `PyFunceble-dev-4.2.0a8/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/CONTRIBUTING.rst` & `PyFunceble-dev-4.2.0a8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/LICENSE` & `PyFunceble-dev-4.2.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PKG-INFO` & `PyFunceble-dev-4.2.0a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFunceble-dev
-Version: 4.2.0a7
+Version: 4.2.0a8
 Summary: The tool to check the availability or syntax of domain, IP or URL.
 Home-page: https://github.com/funilrys/PyFunceble
 Author: funilrys
 Author-email: contact@funilrys.com
 License: Apache 2.0
 Project-URL: Documentation, https://pyfunceble.readthedocs.io/en/dev/
 Project-URL: Funding, https://github.com/sponsors/funilrys
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
 Requires-Python: >=3.6, <4
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: psql
 Provides-Extra: full
 License-File: LICENSE
 
 .. image:: https://raw.githubusercontent.com/PyFunceble/logo/dev/Green/HD/RM.png
 
 The tool to check the availability or syntax of domain, IP or URL
 -----------------------------------------------------------------
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/domain.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/domain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/domain_and_ip.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/domain_and_ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/extras/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/extras/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/extras/dns.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/dns.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/extras/parked.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/parked.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/extras/rules.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,14 @@
         :class:`~PyFunceble.checker.availability.status.AvailabilityCheckerStatus`
     """
 
     regex_active2inactive: dict = {}
     http_codes_dataset: Optional[Box] = None
 
     def __init__(self, status: Optional[AvailabilityCheckerStatus] = None) -> None:
-
         self.regex_active2inactive = {
             r"\.000webhostapp\.com": [
                 (self.switch_to_down_if_status_code, 410),
             ],
             r"\.24\.eu$": [(self.switch_to_down_if_status_code, 503)],
             r"\.altervista\.org$": [(self.switch_to_down_if_status_code, 403)],
             r"\.angelfire\.com$": [(self.switch_to_down_if_status_code, 404)],
@@ -97,15 +96,15 @@
             r"\.skyrock\.com$": [(self.switch_to_down_if_status_code, 404)],
             r"\.tumblr\.com$": [(self.switch_to_down_if_status_code, 404)],
             r"\.wix\.com$": [(self.switch_to_down_if_status_code, 404)],
             r"\.wordpress\.com$": [
                 (self.switch_to_down_if_status_code, 410),
                 self.handle_wordpress_dot_com,
             ],
-            r"\.weebly\.com$": [(self.switch_to_down_if_status_code, 404)],
+            r"\.weebly\.com$": [(self.switch_to_down_if_status_code, {"404", "406"})],
         }
 
         if PyFunceble.facility.ConfigLoader.is_already_loaded():
             self.http_codes_dataset = PyFunceble.storage.HTTP_CODES
         else:
             self.http_codes_dataset = PyFunceble.storage.STD_HTTP_CODES
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/extras/subject_switch.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/subject_switch.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/ip.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/params.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/params.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/status.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/availability/url.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/url.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/complex_json_encoder.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/complex_json_encoder.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/params_base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/params_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/domain.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/domain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/domain_and_ip.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/domain_and_ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/ip.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/params.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/params.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/status.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/reputation/url.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 
         if ip_syntax_checker.is_valid_v4():
             return [url_base]
 
         if ip_syntax_checker.is_valid_v6() or (
             url_base.startswith("[") and url_base.endswith("]")
         ):
-
             url_base = url_base.replace("[", "").replace("]", "")
 
             result = set()
 
             for subject in (
                 self.dns_query_tool.set_query_record_type("PTR")
                 .set_subject(url_base)
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/status_base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/status_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/domain.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/domain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/domain_base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/domain_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/ip.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/ipv4.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/ipv4.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/ipv6.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/ipv6.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/params.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/params.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/second_lvl_domain.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/second_lvl_domain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/status.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/subdomain.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/subdomain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/syntax/url.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/url.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/utils/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/checker/utils/whois.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/checker/utils/whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/exceptions.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/github_actions.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/github_actions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/gitlab_ci.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/jenkins.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/jenkins.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/travis_ci.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/travis_ci.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/continuous_integration/utils.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/utils.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/credential_loader.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/credential_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,14 @@
         Starts the loading of the credential.
 
         :param ignore_cli:
             Ignore questions to end-user.
         """
 
         if not isinstance(self.credential, CredentialBase) and self.authorized:
-
             # We directly share the credential object into the DBSession object.
             # This will let us use the DBSession without having to think about
             # any other headache.
             self.credential = (
                 PyFunceble.cli.factory.DBSession.credential
             ) = self.DB_TYPE2OBJ[self.db_type]()
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/clean.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/clean.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/iana.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/production.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/production.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/public_suffix.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/pyfunceble/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/pyfunceble/argsparser.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/argsparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,27 +47,27 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 import argparse
-from typing import Optional, Sequence, Text
+from typing import Optional, Sequence
 
 # pylint: disable=raising-bad-type
 
 
 class OurArgumentParser(argparse.ArgumentParser):
     """
     Overwrites some behavior of the default argument parser.
     """
 
     def parse_args(
         self,
-        args: Optional[Sequence[Text]] = None,
+        args: Optional[Sequence[str]] = None,
         namespace: Optional[argparse.Namespace] = None,
     ) -> argparse.Namespace:
         namespace = super().parse_args(args, namespace)
 
         if namespace.lookup__timeout is not None and namespace.lookup__timeout < 0:
             raise self.error("--timeout must be a positive digit.")
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/entry_points/pyfunceble/cli.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/cli.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/execution_time.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/execution_time.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/facility.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/factory.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/factory.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/file_preloader.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/file_preloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,15 +447,14 @@
                             rpz_policy2subject=self.rpz_policy2subject,
                             rpz_inputline2subject=self.rpz_inputline2subject,
                             inputline2subject=self.inputline2subject,
                             subject2complements=self.subject2complements,
                             url2netloc=self.url2netloc,
                             cidr2subject=self.cidr2subject,
                         ):
-
                             to_send = copy.deepcopy(self.protocol)
                             to_send["subject"] = subject
                             to_send["idna_subject"] = domain2idna(subject)
                             to_send["tested_at"] = datetime.utcnow() - timedelta(
                                 days=365.25 * 20
                             )
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/cleanup.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/cleanup.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/counter.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/counter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/dir_base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/dir_structure/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/dir_structure/backup.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/backup.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/dir_structure/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/dir_structure/restore.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/restore.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,14 @@
         file_helper = FileHelper()
 
         if dir_helper.set_path(base_dir).exists():
             for root, _, files in os.walk(dir_helper.path):
                 reduced_path = self.get_path_without_base_dir(root)
 
                 if reduced_path not in backup and root != reduced_path:
-
                     dir_helper.set_path(root).delete()
 
                     PyFunceble.facility.Logger.debug(
                         "Added %r into the list of directories to delete. "
                         "Reason: not found in own dataset.",
                         root,
                     )
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/json_base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/json_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/printer/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/printer/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/printer/file.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/printer/stdout.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/stdout.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/registrar_counter.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/registrar_counter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/filesystem/status_file.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/status_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/alembic.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/alembic.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 """
 
 import functools
 import os
 from typing import Any, Optional
 
 from sqlalchemy.orm import Session
+from sqlalchemy.sql import text
 
 try:
     import importlib.resources as package_resources
 except ImportError:  # pragma: no cover ## Retro compatibility
     import importlib_resources as package_resources
 
 import alembic
@@ -160,15 +161,17 @@
 
         revision_id = (
             ScriptDirectory.from_config(self.alembic_config)
             .get_revision(revision)
             .revision
         )
 
-        statement = "SELECT * from alembic_version WHERE version_num = :db_revision"
+        statement = text(
+            "SELECT * from alembic_version WHERE version_num = :db_revision"
+        )
 
         result = self.db_session.execute(statement, {"db_revision": revision_id})
 
         return result.fetchone() is None
 
     @execute_if_authorized(None)
     def upgrade(self, revision: str = "head") -> "Alembic":
@@ -204,15 +207,14 @@
         """
 
         self.configure()
 
         if not self.migrator_base.does_table_exists(
             "alembic_version"
         ) or self.is_revision_different(revision):
-
             PyFunceble.facility.Logger.info(
                 "Started downgrade (%r) of the database schema(s).", revision
             )
 
             alembic_command.downgrade(self.alembic_config, revision)
 
             PyFunceble.facility.Logger.info(
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/csv_file/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/csv_file/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/db_base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/db_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/file_cleanup/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/file_cleanup/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/file_cleanup/hashes_file.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/hashes_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/file_cleanup/mining_file.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/mining_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/file_cleanup/production_config_file.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/production_config_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/json2csv/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/json2csv/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/json2csv/inactive.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/inactive.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/json2csv/whois.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/mariadb/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/mariadb/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 import functools
 from typing import Any, Generator, Tuple
 
+from sqlalchemy.sql import text
+
 import PyFunceble.cli.facility
 import PyFunceble.cli.factory
 import PyFunceble.sessions
 from PyFunceble.cli.migrators.db_base import DBMigratorBase
 
 
 class MariaDBMigratorBase(DBMigratorBase):
@@ -90,15 +92,15 @@
         .. warning::
             If you don't delete the given rows, this method will be infinite.
         """
 
         statement += f" LIMIT {limit}"
 
         while True:
-            db_result = list(self.db_session.execute(statement).fetchall())
+            db_result = list(self.db_session.execute(text(statement)).fetchall())
 
             if not db_result:
                 break
 
             for result in db_result:
                 yield dict(result)
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/mariadb/file_and_status.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/file_and_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 import domain2idna
+from sqlalchemy.sql import text
 
 import PyFunceble.cli.facility
 import PyFunceble.cli.factory
 import PyFunceble.cli.utils.testing
 import PyFunceble.facility
 import PyFunceble.sessions
 import PyFunceble.storage
@@ -92,15 +93,14 @@
 
         inactive_dataset = PyFunceble.cli.utils.testing.get_inactive_dataset_object()
         continue_dataset = PyFunceble.cli.utils.testing.get_continue_databaset_object()
 
         drop_table = True
 
         for file_info in self.get_rows("SELECT * from pyfunceble_file"):
-
             if (
                 self.continuous_integration
                 and self.continuous_integration.is_time_exceeded()
             ):
                 drop_table = False
                 break
 
@@ -140,44 +140,44 @@
 
                 PyFunceble.facility.Logger.info(
                     "Added %r into %r", to_send["idna_subject"], continue_dataset
                 )
 
                 # pylint: disable=line-too-long
                 self.db_session.execute(
-                    f"DELETE from pyfunceble_status WHERE id = {status['id']}"
+                    text(f"DELETE from pyfunceble_status WHERE id = {status['id']}")
                 )
                 self.db_session.commit()
 
                 PyFunceble.facility.Logger.debug(
                     "Deleted from pyfunceble_status: \n%r", status
                 )
 
             if drop_table:
                 # pylint: disable=line-too-long
                 self.db_session.execute(
-                    f"DELETE from pyfunceble_file WHERE id = {file_info['id']}"
+                    text(f"DELETE from pyfunceble_file WHERE id = {file_info['id']}")
                 )
                 self.db_session.commit()
 
                 PyFunceble.facility.Logger.debug(
                     "Deleted from pyfunceble_file: \n%r", file_info
                 )
             else:
                 PyFunceble.facility.Logger.debug(
                     "Not deleted from pyfunceble_file (not authorized): \n%r", file_info
                 )
 
         if drop_table:
-            self.db_session.execute("DROP TABLE pyfunceble_file")
+            self.db_session.execute(text("DROP TABLE pyfunceble_file"))
             self.db_session.commit()
 
             PyFunceble.facility.Logger.debug("Deleted pyfunceble_file table.")
 
-            self.db_session.execute("DROP TABLE pyfunceble_status")
+            self.db_session.execute(text("DROP TABLE pyfunceble_status"))
             self.db_session.commit()
 
             PyFunceble.facility.Logger.debug("Deleted pyfunceble_status table.")
 
             self.done = True
         else:
             PyFunceble.facility.Logger.debug(
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/chancy_producer.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/chancy_producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/chancy_tester.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/chancy_tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/dir_files_sorter.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/dir_files_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/file_sorter.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/file_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/migrator.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/migrator.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/miner.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/miner.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/producer.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/tester.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/chancy_producer.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/chancy_producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/chancy_tester.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/chancy_tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/dir_files_sorter.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/dir_files_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/file_sorter.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/file_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/file_sorter_base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/file_sorter_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/migrator.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/migrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,14 @@
     to handle the mining of dataset to test.
     """
 
     STD_NAME: str = "pyfunceble_migrator_worker"
 
     def run(self) -> None:
         try:
-
             try:
                 self.target(self.continuous_integration, db_session=self.db_session)
             except TypeError:
                 self.target(self.continuous_integration)
             self._child_connection.send(None)
         except Exception as exception:  # pylint: disable=broad-except
             PyFunceble.facility.Logger.critical(
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/miner.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/miner.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/producer.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/producer.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,19 +211,17 @@
             # from the database.
 
             self.whois_dataset.update(
                 {
                     "subject": test_result.subject,
                     "idna_subject": test_result.idna_subject,
                     "expiration_date": test_result.expiration_date,
-                    "epoch": str(
-                        datetime.datetime.strptime(
-                            test_result.expiration_date, "%d-%b-%Y"
-                        ).timestamp()
-                    ),
+                    "epoch": datetime.datetime.strptime(
+                        test_result.expiration_date, "%d-%b-%Y"
+                    ).timestamp(),
                     "registrar": test_result.registrar,
                 }
             )
 
     def run_inactive_backup(
         self, test_dataset: dict, test_result: CheckerStatusBase
     ) -> None:
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/processes/workers/tester.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/scripts/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/scripts/iana.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/scripts/production.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/production.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/scripts/public_suffix.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/storage.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/storage.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/storage_facility.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/storage_facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/system/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/system/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/system/integrator.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/integrator.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/system/launcher.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,15 +546,14 @@
                     )
 
                 self.__start_core_processes()
 
                 for subject in self.continue_dataset.get_to_test(
                     protocol["session_id"]
                 ):
-
                     self.ci_stop_in_the_middle_if_time_exceeded()
 
                     to_send = copy.deepcopy(protocol)
                     to_send["subject"], to_send["idna_subject"] = subject, subject
                     to_send["from_preload"] = True
 
                     self.tester_process_manager.add_to_input_queue(
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/utils/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/utils/ascii_logo.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/ascii_logo.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/utils/sort.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/sort.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/utils/stdout.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/utils/testing.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/testing.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/cli/utils/version.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/config/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/config/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/config/compare.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/config/compare.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/config/loader.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/config/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,14 @@
 
         if (
             not config
             or not isinstance(config, dict)
             or self.merge_upstream
             or is_3_x_version(config)
         ):  # pragma: no cover ## Testing the underlying comparison method is sufficent
-
             config = ConfigComparison(
                 local_config=config,
                 upstream_config=self.dict_helper.from_yaml_file(
                     self.path_to_default_config
                 ),
             ).get_merged()
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/converter/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/converter/adblock_input_line2subject.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/converter/adblock_input_line2subject.py`

 * *Files 16% similar despite different names*

```diff
@@ -63,23 +63,30 @@
     """
     Provides an interface for the conversion or extraction of valuable subjects
     from an inputted AdBlock line.
     """
 
     _aggressive: bool = False
 
-    __regex_helper: Optional[RegexHelper] = None
+    _regex_helper: Optional[RegexHelper] = None
 
     def __init__(
-        self, data_to_convert: Optional[Any] = None, aggressive: bool = False
+        self,
+        data_to_convert: Optional[Any] = None,
+        aggressive: bool = False,
+        *,
+        regex_helper: Optional[RegexHelper] = None,
     ) -> None:
         if aggressive is not None:
             self.aggressive = aggressive
 
-        self.__regex_helper = RegexHelper()
+        if regex_helper is None:
+            self._regex_helper = RegexHelper()
+        else:
+            self._regex_helper = regex_helper
 
         super().__init__(data_to_convert=data_to_convert)
 
     @ConverterBase.data_to_convert.setter
     def data_to_convert(self, value: Any) -> None:
         """
         Overrites the default behavior.
@@ -164,15 +171,15 @@
 
         :param decoded:
             The decoded part to split.
         """
 
         result = set()
 
-        rematch = self.__regex_helper.set_regex(r"((?:[^~\*,]+))").match(
+        rematch = self._regex_helper.set_regex(r"((?:[^~\*,]+))").match(
             decoded, rematch=True, return_match=True
         )
 
         if rematch:
             result.update({self.extract_base(x) for x in rematch})
 
         return result
@@ -197,15 +204,15 @@
             if "domain=" in rule:
                 rule = rule.replace("domain=", "").replace("|", ",")
 
                 result.update(self._decode_multiple_subject(rule))
                 continue
 
             if "href" in rule:
-                matched = self.__regex_helper.set_regex(
+                matched = self._regex_helper.set_regex(
                     r"((?:\"|\')(.*)(?:\"|\'))"
                 ).match(rule, return_match=True, rematch=True, group=1)
 
                 if matched:
                     result.add(self.extract_base(matched))
                 continue
 
@@ -265,27 +272,29 @@
             local_line = local_line.replace("|", "", 1)
             local_line = "".join(local_line.rsplit("|", 1))
 
             result.add(self.extract_base(local_line))
 
         return {x for x in result if "." in x}
 
-    def _decode_v3(self, line: str) -> Set[str]:
+    def _decode_v3(self, line: str, *, aggressive: bool = False) -> Set[str]:
         """
         Implementation of our third decoding mode.
 
         In this mode, we try to decode the simple:
 
             ||ads.example.com^$script,image,domain=example.com|~foo.example.info
             ||ads.example.com$script,image,domain=example.com|~foo.example.info
 
         rule.
 
         :param line:
             The line to decode.
+        :param aggressive:
+            Whether we should aggressively extract datasets.
         """
 
         result = set()
 
         local_line = line.strip()
 
         if not local_line.startswith("||"):
@@ -295,42 +304,44 @@
             v1_mode, options = local_line.split("$", 1)
 
             if not v1_mode.endswith("^"):
                 v1_mode += "^"
 
             result.update(self._decode_v1(v1_mode))
 
-            if self.aggressive:
+            if aggressive:
                 result.update(self._decode_options(options.split(",")))
         elif "^" not in local_line:
             result.update(self._decode_v1(f"{local_line}^"))
         else:
             result.update(self._decode_v1(local_line[: local_line.find("^") + 1]))
 
         return {x for x in result if "." in x}
 
-    def _decode_v4(self, line: str) -> Set[str]:
+    def _decode_v4(self, line: str, *, aggressive: bool = False) -> Set[str]:
         """
         Implementation of our fourth decoding mode.
 
         In this mode, we try to decode the simple:
 
             @@||ads.example.com/notbanner^$~script
 
         rule.
 
         :param line:
             The line to decode.
+        :param aggressive:
+            Whether we should aggressively extract datasets.
         """
 
         result = set()
         local_line = line.strip()
 
         if (
-            not self.aggressive
+            not aggressive
             or not local_line.startswith("@@||")
             or "^$" not in local_line
         ):
             return result
 
         v1_mode, options = local_line.split("$", 1)
 
@@ -338,35 +349,37 @@
             {self.extract_base(x) for x in self._decode_v1(v1_mode.replace("@@", ""))}
         )
 
         result.update(self._decode_options(options.split(",")))
 
         return {x for x in result if "." in x}
 
-    def _decode_v5(self, line: str) -> Set[str]:
+    def _decode_v5(self, line: str, *, aggressive: bool = False) -> Set[str]:
         """
         Implementation of our fifth decoding mode.
 
         In this mode, we try to decode the simple:
 
             example.com,example.net##.advert
             exception.example.com#@#.advert
             example.com,example.net#?#div:-abp-has(> div > img.advert)
             exception.example.com#@#div:-abp-has(> div > img.advert)
 
         rule.
 
         :param line:
             The line to decode.
+        :param aggressive:
+            Whether we should aggressively extract datasets.
         """
 
         local_line = line.strip()
         result = set()
 
-        if not self.aggressive:
+        if not aggressive:
             return result
 
         separators = ["##", "#@#", "#?#"]
 
         obj_of_interest, options = "", ""
 
         for separator in separators:
@@ -375,33 +388,35 @@
                 break
 
         result.update(self._decode_multiple_subject(obj_of_interest))
         result.update(self._decode_options(options.split(",")))
 
         return {x for x in result if "." in x}
 
-    def _decode_v6(self, line: str) -> Set[str]:
+    def _decode_v6(self, line: str, *, aggressive: bool = False) -> Set[str]:
         """
         Implementation of our sixth decoding mode.
 
         In this mode we try to decode the simple:
 
             $domain=exam.pl|elpmaxe.pl|example.pl
             ^hello^$domain=example.com
 
         rule.
 
         :param line:
             The line to decode.
+        :param aggressive:
+            Whether we should aggressively extract datasets.
         """
 
         local_line = line.strip()
         result = set()
 
-        if not self.aggressive:
+        if not aggressive:
             return result
 
         separators = ["$"]
 
         for separator in separators:
             if separator not in line:
                 continue
@@ -413,19 +428,31 @@
         return {x for x in result if "." in x}
 
     def get_converted(self) -> List[str]:
         """
         Provides the converted data.
         """
 
+        return self.convert(self.data_to_convert, aggressive=self.aggressive)
+
+    def convert(self, data: Any, *, aggressive: bool = False) -> List[str]:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        :param aggressive:
+            Whether we should aggressively extract datasets.
+        """
+
         result = set()
 
-        if not self.should_be_ignored(self.data_to_convert.strip()):
-            result.update(self._decode_v1(self.data_to_convert))
-            result.update(self._decode_v2(self.data_to_convert))
-            result.update(self._decode_v3(self.data_to_convert))
-            result.update(self._decode_v5(self.data_to_convert))
-            result.update(self._decode_v6(self.data_to_convert))
+        if not self.should_be_ignored(data.strip()):
+            result.update(self._decode_v1(data))
+            result.update(self._decode_v2(data))
+            result.update(self._decode_v3(data, aggressive=aggressive))
+            result.update(self._decode_v5(data, aggressive=aggressive))
+            result.update(self._decode_v6(data, aggressive=aggressive))
 
-        result.update(self._decode_v4(self.data_to_convert))
+        result.update(self._decode_v4(data, aggressive=aggressive))
 
         return ListHelper(list(result)).sort().subject
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/converter/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/converter/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,7 +97,14 @@
 
     def get_converted(self) -> Optional[Any]:
         """
         Provides the converted data.
         """
 
         raise NotImplementedError()
+
+    def convert(self, data: Any) -> Optional[Any]:
+        """
+        Converts the given dataset.
+        """
+
+        raise NotImplementedError()
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/converter/cidr2subject.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/converter/cidr2subject.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,18 +61,26 @@
 class CIDR2Subject(ConverterBase):
     """
     Converts/Extracts the subjects of from the given CIDR.
     """
 
     ip_syntax_checker: Optional[IPSyntaxChecker] = None
 
-    def __init__(self, data_to_convert: Optional[Any] = None) -> None:
+    def __init__(
+        self,
+        data_to_convert: Optional[Any] = None,
+        *,
+        ip_syntax_checker: Optional[IPSyntaxChecker] = None,
+    ) -> None:
         super().__init__(data_to_convert=data_to_convert)
 
-        self.ip_syntax_checker = IPSyntaxChecker()
+        if ip_syntax_checker is None:
+            self.ip_syntax_checker = IPSyntaxChecker()
+        else:
+            self.ip_syntax_checker = ip_syntax_checker
 
     @ConverterBase.data_to_convert.setter
     def data_to_convert(self, value: Any) -> None:
         """
         Overrites the default behavior.
 
         :raise TypeError:
@@ -86,17 +94,27 @@
         super(CIDR2Subject, self.__class__).data_to_convert.fset(self, value)
 
     def get_converted(self) -> List[str]:
         """
         Provides the subject-s to test.
         """
 
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> List[str]:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
         result = set()
 
-        subject = self.data_to_convert.strip()
+        subject = data.strip()
 
         if subject:
             try:
                 self.ip_syntax_checker.set_subject(subject)
                 if self.ip_syntax_checker.is_valid_v4_range():
                     result.update(
                         str(x) for x in IPv4Network(self.ip_syntax_checker.subject)
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/converter/input_line2subject.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/converter/input_line2subject.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,17 +84,27 @@
         super(InputLine2Subject, self.__class__).data_to_convert.fset(self, value)
 
     def get_converted(self) -> List[str]:
         """
         Provides the subject to test.
         """
 
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> List[str]:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
         result = []
 
-        subject = self.data_to_convert.strip()
+        subject = data.strip()
 
         if subject and (
             not subject.startswith(self.COMMENT)
             and any(not subject.startswith(x) for x in self.PARTICULAR_COMMENT)
         ):
             if self.COMMENT in subject:
                 subject = subject[: subject.find(self.COMMENT)].strip()
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/converter/internal_url.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/digit2digits.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides a way to convert our internal URL.
+Provides an easy way to convert a digit string to 2 digits.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -45,48 +45,44 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
+# pylint: enable=line-too-long
 
 from typing import Any
 
-import PyFunceble.storage
-from PyFunceble.converter.base import ConverterBase
-from PyFunceble.utils.version import VersionUtility
+from PyFunceble.query.whois.converter.base import ConverterBase
 
 
-class InternalUrlConverter(ConverterBase):
+class Digit2Digits(ConverterBase):
     """
-    Converter of the internal URLs.
-
-    .. note::
-        The internal URLs are actually the URL that has nothing to
-        do with what we are going to test.
-
-        They are only relevant for the software itself.
+    Converts a given digit to a 2 digits string.
     """
 
     @ConverterBase.data_to_convert.setter
-    def data_to_convert(self, value: Any) -> None:
+    def data_to_convert(self, value: Any) -> Any:
         """
         Overrites the default behavior.
 
+        :param value:
+            The data to convert.
+
         :raise TypeError:
             When the given data to convert is not :py:class:`str`
         """
+
         if not isinstance(value, str):
             raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
         # pylint: disable=no-member
-        super(InternalUrlConverter, self.__class__).data_to_convert.fset(self, value)
+        super(Digit2Digits, self.__class__).data_to_convert.fset(self, value)
 
+    @ConverterBase.ensure_data_to_convert_is_given
     def get_converted(self) -> str:
         """
         Provides the converted data (after conversion)
         """
 
-        if VersionUtility(PyFunceble.storage.PROJECT_VERSION).is_dev():
-            return self.data_to_convert.replace("master", "dev")
-        return self.data_to_convert.replace("dev", "master")
+        return str(self.data_to_convert).zfill(2)
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/converter/rpz_input_line2subject.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/converter/rpz_input_line2subject.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 # pylint: enable=line-too-long
 
-from typing import List
+from typing import Any, List
 
 from PyFunceble.converter.input_line2subject import InputLine2Subject
 
 
 class RPZInputLine2Subject(InputLine2Subject):
     """
     Converts/Extracts the subject from the given RPZ inputline.
@@ -66,16 +66,26 @@
     SPECIAL: list = ["$", "@"]
 
     def get_converted(self) -> List[str]:
         """
         Provides the converted data.
         """
 
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> List[str]:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
         result = []
-        subject = self.data_to_convert.strip()
+        subject = data.strip()
 
         if (
             subject
             and not any(subject.startswith(x) for x in self.COMMENT)
             and not any(subject.startswith(x) for x in self.SPECIAL)
         ):
             for comment_sign in self.COMMENT:
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/converter/rpz_policy2subject.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/converter/rpz_policy2subject.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,28 +64,35 @@
     """
 
     CLEANUP_MARKERS: list = [".rpz-nsdname"]
     IP_MARKERS: list = [".rpz-client-ip", ".rpz-ip", ".rpz-nsip"]
 
     _soa: Optional[str] = None
     _soas: List[str] = []
+    wilcard2subject: Optional[Wildcard2Subject] = None
 
     def __init__(
         self,
         data_to_convert: Optional[Any] = None,
         soas: Optional[List[str]] = None,
         soa: Optional[str] = None,
+        *,
+        wildcard2subject: Optional[Wildcard2Subject] = None,
     ) -> None:
-
         if soas is not None:
             self.soas = soas
 
         if soa is not None:
             self.soa = soa
 
+        if wildcard2subject is not None:
+            self.wilcard2subject = wildcard2subject
+        else:
+            self.wilcard2subject = Wildcard2Subject()
+
         super().__init__(data_to_convert=data_to_convert)
 
     @property
     def soa(self) -> Optional[str]:
         """
         Provides the currently set SOA.
         """
@@ -253,26 +260,36 @@
         return result
 
     def get_converted(self) -> Optional[str]:
         """
         Provides the converted data.
         """
 
-        subject = self.data_to_convert.strip()
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> Optional[str]:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
+        subject = data.strip()
 
         if (
             subject
             and not any(subject.startswith(x) for x in self.COMMENT)
             and not any(subject.startswith(x) for x in self.SPECIAL)
         ):
             for comment_sign in self.COMMENT:
                 if comment_sign in subject:
                     subject = self.remove_marker(subject, comment_sign).strip()
 
-            subject = Wildcard2Subject(subject).get_converted()
+            subject = self.wilcard2subject.convert(subject)
 
             if self._soas:
                 for soa in self._soas:
                     subject = self.remove_marker(subject, f".{soa}")
                     subject = self.remove_marker(subject, soa)
 
             found_cleanup_marker = self.get_matching_cleanup_marker(subject)
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/converter/subject2complements.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/converter/subject2complements.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,20 +126,30 @@
         return self
 
     def get_converted(self) -> List[str]:
         """
         Provides the converted data.
         """
 
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> List[str]:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
         result = []
 
-        checker = DomainSyntaxChecker(self.data_to_convert)
+        checker = DomainSyntaxChecker(data)
 
-        if self.include_given and self.data_to_convert not in result:
-            result.append(self.data_to_convert)
+        if self.include_given and data not in result:
+            result.append(data)
 
-        if self.data_to_convert.startswith("www."):
-            result.append(self.data_to_convert[4:])
+        if data.startswith("www."):
+            result.append(data[4:])
         elif checker.is_valid_second_level():
-            result.append(f"www.{self.data_to_convert}")
+            result.append(f"www.{data}")
 
         return result
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/converter/url2netloc.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/converter/url2netloc.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,36 +83,59 @@
 
         if not value:
             raise ValueError("<value> should not be empty.")
 
         # pylint: disable=no-member
         super(Url2Netloc, self.__class__).data_to_convert.fset(self, value)
 
+    @staticmethod
+    def parse_single_url(data) -> Optional[urllib.parse.ParseResult]:
+        """
+        Parses the URL.
+        """
+
+        if data:
+            return urllib.parse.urlparse(data)
+        return None
+
     def parse_url(self) -> "Url2Netloc":
         """
         Parses the URL.
         """
 
-        if self.data_to_convert:
-            self.parsed_url = urllib.parse.urlparse(self.data_to_convert)
+        self.parsed_url = self.parse_single_url(self.data_to_convert)
+
         return self
 
     def get_converted(self) -> str:
         """
         Provides the converted data (after conversion)
         """
 
+        # Retrocompatibility.
         self.parse_url()
 
-        if not self.parsed_url.netloc and self.parsed_url.path:
-            netloc = self.parsed_url.path
-        elif self.parsed_url.netloc:
-            netloc = self.parsed_url.netloc
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> str:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
+        parsed_url = self.parse_single_url(data)
+
+        if not parsed_url.netloc and parsed_url.path:
+            netloc = parsed_url.path
+        elif parsed_url.netloc:
+            netloc = parsed_url.netloc
         else:  # pragma: no cover ## Safety
-            netloc = self.data_to_convert
+            netloc = data
 
         if "//" in netloc:
             netloc = netloc[netloc.find("//") + 2 :]
 
         if "/" in netloc:
             netloc = netloc[: netloc.find("/")]
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/converter/wildcard2subject.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/converter/wildcard2subject.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,25 @@
         super(Wildcard2Subject, self.__class__).data_to_convert.fset(self, value)
 
     def get_converted(self) -> str:
         """
         Provides the converted data.
         """
 
-        subject = self.data_to_convert.strip()
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> str:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
+        subject = data.strip()
 
         if not subject:
             return None
 
         if subject.startswith(self.WILDCARD):
             return subject[2:]
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/env.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/env.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/postgresql/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/postgresql/env.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/env.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/postgresql/versions/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/infrastructure/.PyFunceble_production.yaml` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/infrastructure/.PyFunceble_production.yaml`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/data/infrastructure/dir_structure_production.json` & `PyFunceble-dev-4.2.0a8/PyFunceble/data/infrastructure/dir_structure_production.json`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/credential/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/credential/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,14 @@
         host: Optional[str] = None,
         port: Optional[int] = None,
         name: Optional[str] = None,
         username: Optional[str] = None,
         password: Optional[str] = None,
         charset: Optional[str] = None,
     ) -> None:
-
         if host is not None:
             self.host = host
         else:
             self.host = self.STD_HOST
 
         if port is not None:
             self.port = port
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/credential/mariadb.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/mariadb.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/credential/mysql.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/mysql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/credential/postgresql.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/postgresql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/schemas/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/schemas/autocontinue.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/autocontinue.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/schemas/inactive.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/inactive.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/schemas/status.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/schemas/whois_record.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/whois_record.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/session.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/session.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/sqlalchemy/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/sqlalchemy/all_schemas.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/all_schemas.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/database/sqlalchemy/base_schema.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/base_schema.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/autocontinue/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/autocontinue/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/autocontinue/csv.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
     def update_source_file_afterwards(func):  # pylint: disable=no-self-argument
         """
         Updates the source file before launching the decorated method.
         """
 
         @functools.wraps(func)
         def wrapper(self, *args, **kwargs):
-
             result = func(self, *args, **kwargs)  # pylint: disable=not-callable
 
             self.source_file = os.path.join(
                 self.base_directory, PyFunceble.cli.storage.AUTOCONTINUE_FILE
             )
 
             return result
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/autocontinue/sql.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/sql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/csv_base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/csv_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/db_base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/db_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/iana.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/inactive/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/inactive/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/inactive/csv.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 
         return super().__post_init__()
 
     @CSVDatasetBase.execute_if_authorized(None)
     def get_to_retest(
         self, destination: str, checker_type: str, *, min_days: Optional[int]
     ) -> Generator[Tuple[str, str, Optional[int]], dict, None]:
-
         days_ago = datetime.utcnow() - timedelta(days=min_days)
 
         for dataset in self.get_filtered_content(
             {"destination": destination, "checker_type": checker_type}
         ):
             if not isinstance(dataset["tested_at"], datetime):
                 try:
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/inactive/sql.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     ORM_OBJ: Inactive = Inactive
 
     @SQLDBDatasetBase.execute_if_authorized(None)
     @SQLDBDatasetBase.ensure_orm_obj_is_given
     def get_to_retest(
         self, destination: str, checker_type: str, *, min_days: Optional[int]
     ) -> Generator[Tuple[str, str, Optional[int]], dict, None]:
-
         days_ago = datetime.utcnow() - timedelta(days=min_days)
 
         result = (
             self.db_session.query(self.ORM_OBJ)
             .filter(self.ORM_OBJ.destination == destination)
             .filter(self.ORM_OBJ.checker_type == checker_type)
             .filter(self.ORM_OBJ.tested_at < days_ago)
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/ipv4_reputation.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/ipv4_reputation.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/public_suffix.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/sql_base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/sql_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
             if "expiration_date" not in row and "epoch" not in row:
                 raise exception
 
             y2k38_limit = datetime(2037, 12, 31, 0, 0)
             new_date = datetime.fromtimestamp(float(row["epoch"]))
             new_date -= new_date - y2k38_limit
 
-            row["epoch"] = str(new_date.timestamp())
+            row["epoch"] = new_date.timestamp()
             row["expiration_date"] = new_date.strftime("%d-%b-%Y")
 
             self.db_session.execute(self.ORM_OBJ.__table__.insert(), row)
             self.db_session.commit()
 
         PyFunceble.facility.Logger.debug("Added row:\n%r", row)
         PyFunceble.facility.Logger.info("Finished to add row.")
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/user_agent.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/user_agent.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/whois/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/whois/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/whois/csv.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/csv.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/dataset/whois/sql.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/sql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/downloader/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/downloader/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/downloader/exceptions.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/downloader/iana.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/downloader/ipv4_reputation.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/ipv4_reputation.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/downloader/public_suffix.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/downloader/user_agents.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/user_agents.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/exceptions.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/facility.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/factory.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/factory.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/helpers/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/helpers/command.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 
     def __init__(
         self,
         command: Optional[Union[str, list]] = None,
         *,
         encoding: Optional[str] = None,
     ) -> None:
-
         if command is not None:
             self.command = command
 
         if encoding is not None:
             self.encoding = encoding
 
     @property
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/helpers/dict.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/helpers/directory.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/directory.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/helpers/download.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/download.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/helpers/environment_variable.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/environment_variable.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/helpers/exceptions.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/helpers/file.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/helpers/hash.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/hash.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/helpers/list.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/list.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/helpers/merge.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/merge.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/helpers/regex.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/regex.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/logger.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,14 @@
     def __init__(
         self,
         *,
         activated: Optional[bool] = None,
         min_level: Optional[int] = None,
         output_dir: Optional[str] = None,
     ) -> None:
-
         if output_dir:
             self.output_directory = output_dir
         else:
             self.output_directory = os.path.join(
                 PyFunceble.cli.storage.OUTPUT_DIRECTORY,
                 PyFunceble.cli.storage.OUTPUTS.logs.directories.parent,
             )
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/collection.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,14 @@
     def __init__(
         self,
         *,
         token: Optional[str] = None,
         url_base: Optional[str] = None,
         preferred_status_origin: Optional[str] = None,
     ) -> None:
-
         if token is not None:
             self.token = token
         else:
             self.token = EnvironmentVariableHelper(
                 "PYFUNCEBLE_COLLECTION_API_TOKEN"
             ).get_value(default="")
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/dns/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/dns/nameserver.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/nameserver.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/dns/query_tool.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/query_tool.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/dns/resolver.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/resolver.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/http_status_code.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/http_status_code.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/netinfo/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/netinfo/address.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/address.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/netinfo/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/netinfo/hostbyaddr.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/hostbyaddr.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/record/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/record/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/record/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/record/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/record/dns.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/record/dns.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/record/whois.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/record/whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/adapter/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/adapter/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/adapter/http.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/http.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/adapter/https.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/https.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/requests/requester.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/requester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/converter/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/converter/base.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/converter/digit2digits.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/converter/internal_url.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides an easy way to convert a digit string to 2 digits.
+Provides a way to convert our internal URL.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -45,44 +45,58 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
-# pylint: enable=line-too-long
 
 from typing import Any
 
-from PyFunceble.query.whois.converter.base import ConverterBase
+import PyFunceble.storage
+from PyFunceble.converter.base import ConverterBase
+from PyFunceble.utils.version import VersionUtility
 
 
-class Digit2Digits(ConverterBase):
+class InternalUrlConverter(ConverterBase):
     """
-    Converts a given digit to a 2 digits string.
+    Converter of the internal URLs.
+
+    .. note::
+        The internal URLs are actually the URL that has nothing to
+        do with what we are going to test.
+
+        They are only relevant for the software itself.
     """
 
     @ConverterBase.data_to_convert.setter
-    def data_to_convert(self, value: Any) -> Any:
+    def data_to_convert(self, value: Any) -> None:
         """
         Overrites the default behavior.
 
-        :param value:
-            The data to convert.
-
         :raise TypeError:
             When the given data to convert is not :py:class:`str`
         """
-
         if not isinstance(value, str):
             raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
         # pylint: disable=no-member
-        super(Digit2Digits, self.__class__).data_to_convert.fset(self, value)
+        super(InternalUrlConverter, self.__class__).data_to_convert.fset(self, value)
 
-    @ConverterBase.ensure_data_to_convert_is_given
     def get_converted(self) -> str:
         """
         Provides the converted data (after conversion)
         """
 
-        return str(self.data_to_convert).zfill(2)
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> str:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
+        if VersionUtility(PyFunceble.storage.PROJECT_VERSION).is_dev():
+            return data.replace("master", "dev")
+        return data.replace("dev", "master")
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/converter/expiration_date.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/expiration_date.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/converter/month2unified.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/month2unified.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/converter/registrar.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/registrar.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/query/whois/query_tool.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/query_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,14 @@
     ) -> str:  # pragma: no cover ## The effect of the response of this method
         ## are more important.
         """
         Queries the WHOIS record and return the current object.
         """
 
         if self.lookup_record.record is None:
-
             if not self.server:
                 whois_server = self.get_whois_server()
             else:
                 whois_server = self.server
 
             if whois_server:
                 self.lookup_record.server = whois_server
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/sessions.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/sessions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/storage.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 from box import Box
 from dotenv import load_dotenv
 
 from PyFunceble.storage_facility import get_config_directory
 
 PROJECT_NAME: str = "PyFunceble"
-PROJECT_VERSION: str = "4.2.0a7.dev (Blue Duckling: Ixora)"
+PROJECT_VERSION: str = "4.2.0a8.dev (Blue Duckling: Ixora)"
 
 DISTRIBUTED_CONFIGURATION_FILENAME: str = ".PyFunceble_production.yaml"
 DISTRIBUTED_DIR_STRUCTURE_FILENAME: str = "dir_structure_production.json"
 
 IANA_DUMP_FILENAME: str = "iana-domains-db.json"
 PUBLIC_SUFFIX_DUMP_FILENAME: str = "public-suffix.json"
 CONFIGURATION_FILENAME: str = ".PyFunceble.yaml"
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/storage_facility.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/storage_facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/utils/__init__.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/utils/platform.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/utils/platform.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/utils/profile.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/utils/profile.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble/utils/version.py` & `PyFunceble-dev-4.2.0a8/PyFunceble/utils/version.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble_dev.egg-info/PKG-INFO` & `PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFunceble-dev
-Version: 4.2.0a7
+Version: 4.2.0a8
 Summary: The tool to check the availability or syntax of domain, IP or URL.
 Home-page: https://github.com/funilrys/PyFunceble
 Author: funilrys
 Author-email: contact@funilrys.com
 License: Apache 2.0
 Project-URL: Documentation, https://pyfunceble.readthedocs.io/en/dev/
 Project-URL: Funding, https://github.com/sponsors/funilrys
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
 Requires-Python: >=3.6, <4
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: psql
 Provides-Extra: full
 License-File: LICENSE
 
 .. image:: https://raw.githubusercontent.com/PyFunceble/logo/dev/Green/HD/RM.png
 
 The tool to check the availability or syntax of domain, IP or URL
 -----------------------------------------------------------------
```

### Comparing `PyFunceble-dev-4.2.0a7/PyFunceble_dev.egg-info/SOURCES.txt` & `PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 PyFunceble/exceptions.py
 PyFunceble/facility.py
 PyFunceble/factory.py
 PyFunceble/logger.py
 PyFunceble/sessions.py
 PyFunceble/storage.py
 PyFunceble/storage_facility.py
-PyFunceble/.vscode/settings.json
 PyFunceble/checker/__init__.py
 PyFunceble/checker/base.py
 PyFunceble/checker/complex_json_encoder.py
 PyFunceble/checker/params_base.py
 PyFunceble/checker/status_base.py
 PyFunceble/checker/availability/__init__.py
 PyFunceble/checker/availability/base.py
```

### Comparing `PyFunceble-dev-4.2.0a7/README.rst` & `PyFunceble-dev-4.2.0a8/README.rst`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a7/setup.py` & `PyFunceble-dev-4.2.0a8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
     """
 
     mode2files = {
         "standard": ["requirements.txt"],
         "dev": ["requirements.dev.txt"],
         "docs": ["requirements.docs.txt"],
         "test": ["requirements.test.txt"],
+        "psql": ["requirements.txt"],
     }
 
     if is_win_platform():
         for mode, files in mode2files.items():
             new_files = set()
 
             for file in files:
@@ -172,14 +173,17 @@
                     line = line[: line.find("#")].strip()
 
                 if not line:
                     continue
 
                 result.add(line)
 
+    if mode == "psql":
+        result.add("psycopg2")
+
     return list(result)
 
 
 def get_version():
     """
     This function will extract the version from PyFunceble/__init__.py
     """
@@ -213,14 +217,15 @@
         version=get_version(),
         python_requires=">=3.6, <4",
         install_requires=get_requirements(mode="standard"),
         extras_require={
             "docs": get_requirements(mode="docs"),
             "dev": get_requirements(mode="dev"),
             "test": get_requirements(mode="test"),
+            "psql": get_requirements(mode="psql"),
             "full": get_requirements(mode="full"),
         },
         description="The tool to check the availability or syntax of domain, IP or URL.",
         long_description=get_long_description(),
         author="funilrys",
         author_email="contact@funilrys.com",
         license="Apache 2.0",
```

### Comparing `PyFunceble-dev-4.2.0a7/version.yaml` & `PyFunceble-dev-4.2.0a8/version.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-current_version: '4.2.0a7.dev (Blue Duckling: Ixora)'
+current_version: '4.2.0a8.dev (Blue Duckling: Ixora)'
 deprecated:
 - 3.0.21
 - 3.1.20
 - 3.2.13
 - 4.0.0a1
 - 4.1.0b1
 - 4.2.0a1
```

