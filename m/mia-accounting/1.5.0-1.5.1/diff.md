# Comparing `tmp/mia-accounting-1.5.0.tar.gz` & `tmp/mia-accounting-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia-accounting-1.5.0.tar", last modified: Sun Apr 23 10:49:14 2023, max compression
+gzip compressed data, was "mia-accounting-1.5.1.tar", last modified: Sat Apr 29 21:54:28 2023, max compression
```

## Comparing `mia-accounting-1.5.0.tar` & `mia-accounting-1.5.1.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.5.0/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.5.0/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     2525 2023-04-23 10:42:54.000000 mia-accounting-1.5.0/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.424269 mia-accounting-1.5.0/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.5.0/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.5.0/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.424269 mia-accounting-1.5.0/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.424269 mia-accounting-1.5.0/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.5.0/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.424269 mia-accounting-1.5.0/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.5.0/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.account.rst
--rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.base_account.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.currency.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.journal_entry.forms.rst
--rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.journal_entry.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.journal_entry.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.option.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.report.period.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-04-18 01:32:44.000000 mia-accounting-1.5.0/docs/source/accounting.report.reports.rst
--rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-18 01:25:56.000000 mia-accounting-1.5.0/docs/source/accounting.report.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2168 2023-04-18 01:32:44.000000 mia-accounting-1.5.0/docs/source/accounting.report.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1301 2023-04-18 01:32:44.000000 mia-accounting-1.5.0/docs/source/accounting.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2405 2023-04-18 01:32:44.000000 mia-accounting-1.5.0/docs/source/accounting.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     7170 2023-04-23 10:48:38.000000 mia-accounting-1.5.0/docs/source/changelog.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1051 2023-04-23 10:42:54.000000 mia-accounting-1.5.0/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.5.0/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.5.0/docs/source/history.rst
--rw-r--r--   0 imacat    (1000) users      (100)      521 2023-04-23 05:51:17.000000 mia-accounting-1.5.0/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     3462 2023-04-23 10:42:55.000000 mia-accounting-1.5.0/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.5.0/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1994 2023-04-23 10:42:54.000000 mia-accounting-1.5.0/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.428269 mia-accounting-1.5.0/src/accounting/
--rw-r--r--   0 imacat    (1000) users      (100)     3045 2023-04-23 10:46:14.000000 mia-accounting-1.5.0/src/accounting/__init__.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.428269 mia-accounting-1.5.0/src/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.5.0/src/accounting/account/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.5.0/src/accounting/account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.428269 mia-accounting-1.5.0/src/accounting/base_account/
--rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/base_account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/base_account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/base_account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.5.0/src/accounting/base_account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.5.0/src/accounting/base_account/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/commands.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.428269 mia-accounting-1.5.0/src/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/currency/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2212 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/src/accounting/currency/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/currency/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.5.0/src/accounting/currency/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/currency/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.5.0/src/accounting/currency/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.428269 mia-accounting-1.5.0/src/accounting/data/
--rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.5.0/src/accounting/data/base_accounts.csv
--rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.5.0/src/accounting/data/currencies.csv
--rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.5.0/src/accounting/forms.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.428269 mia-accounting-1.5.0/src/accounting/journal_entry/
--rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/journal_entry/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3297 2023-04-23 01:52:21.000000 mia-accounting-1.5.0/src/accounting/journal_entry/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.432269 mia-accounting-1.5.0/src/accounting/journal_entry/forms/
--rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.5.0/src/accounting/journal_entry/forms/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    11003 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/journal_entry/forms/currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.5.0/src/accounting/journal_entry/forms/journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    19808 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/journal_entry/forms/line_item.py
--rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/journal_entry/forms/reorder.py
--rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.5.0/src/accounting/journal_entry/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.432269 mia-accounting-1.5.0/src/accounting/journal_entry/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.5.0/src/accounting/journal_entry/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1802 2023-04-17 23:37:17.000000 mia-accounting-1.5.0/src/accounting/journal_entry/utils/account_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    12987 2023-04-17 23:42:37.000000 mia-accounting-1.5.0/src/accounting/journal_entry/utils/description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/journal_entry/utils/operators.py
--rw-r--r--   0 imacat    (1000) users      (100)     3722 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/journal_entry/utils/original_line_items.py
--rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.5.0/src/accounting/journal_entry/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.5.0/src/accounting/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    32027 2023-04-23 05:21:54.000000 mia-accounting-1.5.0/src/accounting/models.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.432269 mia-accounting-1.5.0/src/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/option/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.5.0/src/accounting/option/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.5.0/src/accounting/option/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.432269 mia-accounting-1.5.0/src/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.5.0/src/accounting/report/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.5.0/src/accounting/report/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.432269 mia-accounting-1.5.0/src/accounting/report/period/
--rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.5.0/src/accounting/report/period/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/report/period/chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/report/period/description.py
--rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.5.0/src/accounting/report/period/month_end.py
--rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.5.0/src/accounting/report/period/parser.py
--rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.5.0/src/accounting/report/period/period.py
--rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/report/period/shortcuts.py
--rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/report/period/specification.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.436269 mia-accounting-1.5.0/src/accounting/report/reports/
--rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.5.0/src/accounting/report/reports/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.5.0/src/accounting/report/reports/balance_sheet.py
--rw-r--r--   0 imacat    (1000) users      (100)    18844 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/report/reports/income_expenses.py
--rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.5.0/src/accounting/report/reports/income_statement.py
--rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.5.0/src/accounting/report/reports/journal.py
--rw-r--r--   0 imacat    (1000) users      (100)    16567 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/report/reports/ledger.py
--rw-r--r--   0 imacat    (1000) users      (100)     8772 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/report/reports/search.py
--rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.5.0/src/accounting/report/reports/trial_balance.py
--rw-r--r--   0 imacat    (1000) users      (100)     8094 2023-04-18 01:09:36.000000 mia-accounting-1.5.0/src/accounting/report/reports/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     5212 2023-04-18 01:09:36.000000 mia-accounting-1.5.0/src/accounting/report/reports/unapplied_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     8164 2023-04-18 01:14:44.000000 mia-accounting-1.5.0/src/accounting/report/reports/unmatched.py
--rw-r--r--   0 imacat    (1000) users      (100)     5193 2023-04-18 01:09:36.000000 mia-accounting-1.5.0/src/accounting/report/reports/unmatched_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.5.0/src/accounting/report/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.436269 mia-accounting-1.5.0/src/accounting/report/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/report/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/report/utils/base_page_params.py
--rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.5.0/src/accounting/report/utils/base_report.py
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.5.0/src/accounting/report/utils/csv_export.py
--rw-r--r--   0 imacat    (1000) users      (100)     7369 2023-04-18 01:18:28.000000 mia-accounting-1.5.0/src/accounting/report/utils/offset_matcher.py
--rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.5.0/src/accounting/report/utils/option_link.py
--rw-r--r--   0 imacat    (1000) users      (100)     7865 2023-04-18 01:17:12.000000 mia-accounting-1.5.0/src/accounting/report/utils/report_chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     1371 2023-04-17 08:41:57.000000 mia-accounting-1.5.0/src/accounting/report/utils/report_type.py
--rw-r--r--   0 imacat    (1000) users      (100)     4385 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/report/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     2221 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/report/utils/unmatched.py
--rw-r--r--   0 imacat    (1000) users      (100)     5440 2023-04-18 00:59:05.000000 mia-accounting-1.5.0/src/accounting/report/utils/urls.py
--rw-r--r--   0 imacat    (1000) users      (100)    14167 2023-04-18 01:14:44.000000 mia-accounting-1.5.0/src/accounting/report/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/src/accounting/static/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.436269 mia-accounting-1.5.0/src/accounting/static/css/
--rw-r--r--   0 imacat    (1000) users      (100)    13431 2023-04-18 00:10:33.000000 mia-accounting-1.5.0/src/accounting/static/css/style.css
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/static/js/
--rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/account-form.js
--rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/account-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/currency-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    38865 2023-04-17 23:44:56.000000 mia-accounting-1.5.0/src/accounting/static/js/description-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/drag-and-drop-reorder.js
--rw-r--r--   0 imacat    (1000) users      (100)     9211 2023-04-17 23:32:14.000000 mia-accounting-1.5.0/src/accounting/static/js/journal-entry-account-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    33086 2023-04-17 23:52:58.000000 mia-accounting-1.5.0/src/accounting/static/js/journal-entry-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    19574 2023-04-19 16:28:28.000000 mia-accounting-1.5.0/src/accounting/static/js/journal-entry-line-item-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/journal-entry-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/material-fab-speed-dial.js
--rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/option-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    11670 2023-04-17 23:40:31.000000 mia-accounting-1.5.0/src/accounting/static/js/original-line-item-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.5.0/src/accounting/static/js/period-chooser.js
--rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.5.0/src/accounting/template_filters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1137 2023-04-23 01:43:59.000000 mia-accounting-1.5.0/src/accounting/template_globals.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/src/accounting/templates/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/account/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/account/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/account/include/
--rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/account/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/account/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/base-account/
--rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/base-account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/base-account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/base.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/currency/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-17 15:07:31.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/include/nav.html
--rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/include/pagination.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/
--rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.440269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3406 2023-04-17 23:32:14.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)    14492 2023-04-17 23:42:37.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3242 2023-04-17 23:11:57.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
--rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
--rw-r--r--   0 imacat    (1000) users      (100)     6442 2023-04-17 23:54:15.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
--rw-r--r--   0 imacat    (1000) users      (100)     3791 2023-04-18 00:10:33.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/
--rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/
--rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/option/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/option/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.444269 mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
--rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/form-recurring-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.448269 mia-accounting-1.5.0/src/accounting/templates/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     5435 2023-04-18 00:39:27.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/balance-sheet.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.448269 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
--rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html
--rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/period-chooser.html
--rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/search-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     5600 2023-04-18 00:10:33.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html
--rw-r--r--   0 imacat    (1000) users      (100)     4841 2023-04-18 00:34:44.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/income-expenses.html
--rw-r--r--   0 imacat    (1000) users      (100)     4618 2023-04-18 00:37:47.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/income-statement.html
--rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/journal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4946 2023-04-18 00:33:38.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/ledger.html
--rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/search.html
--rw-r--r--   0 imacat    (1000) users      (100)     3710 2023-04-18 00:36:16.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/trial-balance.html
--rw-r--r--   0 imacat    (1000) users      (100)     3037 2023-04-18 00:59:05.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/unapplied-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     3843 2023-04-18 00:59:06.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/unapplied.html
--rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-18 00:59:05.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/unmatched-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     6998 2023-04-18 00:59:05.000000 mia-accounting-1.5.0/src/accounting/templates/accounting/report/unmatched.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.448269 mia-accounting-1.5.0/src/accounting/translations/
--rw-r--r--   0 imacat    (1000) users      (100)    49437 2023-04-18 01:32:01.000000 mia-accounting-1.5.0/src/accounting/translations/accounting.pot
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.5.0/src/accounting/translations/babel.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/src/accounting/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.448269 mia-accounting-1.5.0/src/accounting/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/src/accounting/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.448269 mia-accounting-1.5.0/src/accounting/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.452268 mia-accounting-1.5.0/src/accounting/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.5.0/src/accounting/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-23 05:21:41.000000 mia-accounting-1.5.0/src/accounting/utils/cast.py
--rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/utils/current_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/utils/flash_errors.py
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.5.0/src/accounting/utils/journal_entry_types.py
--rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.5.0/src/accounting/utils/next_uri.py
--rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.5.0/src/accounting/utils/offset_alias.py
--rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.5.0/src/accounting/utils/options.py
--rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.5.0/src/accounting/utils/pagination.py
--rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.5.0/src/accounting/utils/permission.py
--rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/utils/query.py
--rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/utils/random_id.py
--rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.5.0/src/accounting/utils/strip_text.py
--rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.5.0/src/accounting/utils/user.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.452268 mia-accounting-1.5.0/src/mia_accounting.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-04-23 10:49:14.000000 mia-accounting-1.5.0/src/mia_accounting.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    11434 2023-04-23 10:49:14.000000 mia-accounting-1.5.0/src/mia_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-23 10:49:14.000000 mia-accounting-1.5.0/src/mia_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)      107 2023-04-23 10:49:14.000000 mia-accounting-1.5.0/src/mia_accounting.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-23 10:49:14.000000 mia-accounting-1.5.0/src/mia_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/
--rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.5.0/tests/babel-utils-test-site.py
--rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.5.0/tests/babel-utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    32736 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/tests/test_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/tests/test_base_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/tests/test_commands.py
--rw-r--r--   0 imacat    (1000) users      (100)    23824 2023-04-10 15:59:48.000000 mia-accounting-1.5.0/tests/test_currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    15999 2023-04-13 01:09:51.000000 mia-accounting-1.5.0/tests/test_description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)   103461 2023-04-13 01:09:51.000000 mia-accounting-1.5.0/tests/test_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    38887 2023-04-13 01:09:51.000000 mia-accounting-1.5.0/tests/test_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    15935 2023-04-13 01:09:51.000000 mia-accounting-1.5.0/tests/test_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    17862 2023-04-18 01:19:22.000000 mia-accounting-1.5.0/tests/test_report.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/test_site/
--rw-r--r--   0 imacat    (1000) users      (100)     4505 2023-04-13 00:49:22.000000 mia-accounting-1.5.0/tests/test_site/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3898 2023-04-13 01:52:58.000000 mia-accounting-1.5.0/tests/test_site/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)    13223 2023-04-13 01:30:40.000000 mia-accounting-1.5.0/tests/test_site/lib.py
--rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.5.0/tests/test_site/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    13048 2023-04-13 01:52:58.000000 mia-accounting-1.5.0/tests/test_site/reset.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/test_site/static/
--rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.5.0/tests/test_site/static/favicon.svg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/test_site/templates/
--rw-r--r--   0 imacat    (1000) users      (100)     6435 2023-04-12 10:05:13.000000 mia-accounting-1.5.0/tests/test_site/templates/base.html
--rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.5.0/tests/test_site/templates/home.html
--rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.5.0/tests/test_site/templates/login.html
--rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.5.0/tests/test_site/templates/reset.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/test_site/translations/
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.5.0/tests/test_site/translations/babel.cfg
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.5.0/tests/test_site/translations/messages.pot
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/tests/test_site/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.5.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.420269 mia-accounting-1.5.0/tests/test_site/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-23 10:49:14.456268 mia-accounting-1.5.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.5.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0 imacat    (1000) users      (100)    27794 2023-04-18 01:14:44.000000 mia-accounting-1.5.0/tests/test_unmatched_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.5.0/tests/test_utils.py
--rw-r--r--   0 imacat    (1000) users      (100)     5169 2023-04-13 01:09:51.000000 mia-accounting-1.5.0/tests/testlib.py
--rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-13 01:09:51.000000 mia-accounting-1.5.0/tests/testlib_journal_entry.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.906054 mia-accounting-1.5.1/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.5.1/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.5.1/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-04-29 21:54:28.906054 mia-accounting-1.5.1/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     2525 2023-04-23 12:04:20.000000 mia-accounting-1.5.1/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.686058 mia-accounting-1.5.1/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.5.1/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.5.1/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.718057 mia-accounting-1.5.1/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.718057 mia-accounting-1.5.1/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.5.1/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.718057 mia-accounting-1.5.1/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.5.1/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-18 01:25:56.000000 mia-accounting-1.5.1/docs/source/accounting.account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-18 01:25:56.000000 mia-accounting-1.5.1/docs/source/accounting.base_account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-18 01:25:56.000000 mia-accounting-1.5.1/docs/source/accounting.currency.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-18 01:25:56.000000 mia-accounting-1.5.1/docs/source/accounting.journal_entry.forms.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-18 01:25:56.000000 mia-accounting-1.5.1/docs/source/accounting.journal_entry.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-18 01:25:56.000000 mia-accounting-1.5.1/docs/source/accounting.journal_entry.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-18 01:25:56.000000 mia-accounting-1.5.1/docs/source/accounting.option.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-18 01:25:56.000000 mia-accounting-1.5.1/docs/source/accounting.report.period.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-04-18 01:32:44.000000 mia-accounting-1.5.1/docs/source/accounting.report.reports.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-18 01:25:56.000000 mia-accounting-1.5.1/docs/source/accounting.report.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2168 2023-04-18 01:32:44.000000 mia-accounting-1.5.1/docs/source/accounting.report.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1301 2023-04-18 01:32:44.000000 mia-accounting-1.5.1/docs/source/accounting.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2405 2023-04-18 01:32:44.000000 mia-accounting-1.5.1/docs/source/accounting.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     7399 2023-04-29 21:45:45.000000 mia-accounting-1.5.1/docs/source/changelog.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1051 2023-04-23 12:12:53.000000 mia-accounting-1.5.1/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.5.1/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.5.1/docs/source/history.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      521 2023-04-23 12:04:21.000000 mia-accounting-1.5.1/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     3462 2023-04-23 12:13:33.000000 mia-accounting-1.5.1/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.5.1/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1994 2023-04-23 12:12:53.000000 mia-accounting-1.5.1/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-29 21:54:28.906054 mia-accounting-1.5.1/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.674058 mia-accounting-1.5.1/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.718057 mia-accounting-1.5.1/src/accounting/
+-rw-r--r--   0 imacat    (1000) users      (100)     3045 2023-04-29 21:45:45.000000 mia-accounting-1.5.1/src/accounting/__init__.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.718057 mia-accounting-1.5.1/src/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.5.1/src/accounting/account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-29 21:45:45.000000 mia-accounting-1.5.1/src/accounting/account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.5.1/src/accounting/account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.5.1/src/accounting/account/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.5.1/src/accounting/account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.5.1/src/accounting/account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.722057 mia-accounting-1.5.1/src/accounting/base_account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.5.1/src/accounting/base_account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.5.1/src/accounting/base_account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.5.1/src/accounting/base_account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.5.1/src/accounting/base_account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.5.1/src/accounting/base_account/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.5.1/src/accounting/commands.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.722057 mia-accounting-1.5.1/src/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.5.1/src/accounting/currency/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2206 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/currency/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.5.1/src/accounting/currency/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.5.1/src/accounting/currency/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.5.1/src/accounting/currency/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.5.1/src/accounting/currency/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.722057 mia-accounting-1.5.1/src/accounting/data/
+-rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.5.1/src/accounting/data/base_accounts.csv
+-rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.5.1/src/accounting/data/currencies.csv
+-rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.5.1/src/accounting/forms.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.722057 mia-accounting-1.5.1/src/accounting/journal_entry/
+-rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.5.1/src/accounting/journal_entry/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3302 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/journal_entry/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.722057 mia-accounting-1.5.1/src/accounting/journal_entry/forms/
+-rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.5.1/src/accounting/journal_entry/forms/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11003 2023-04-23 05:21:41.000000 mia-accounting-1.5.1/src/accounting/journal_entry/forms/currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24568 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/journal_entry/forms/journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    19807 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/journal_entry/forms/line_item.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3291 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/journal_entry/forms/reorder.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.5.1/src/accounting/journal_entry/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.722057 mia-accounting-1.5.1/src/accounting/journal_entry/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.5.1/src/accounting/journal_entry/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1802 2023-04-17 23:37:17.000000 mia-accounting-1.5.1/src/accounting/journal_entry/utils/account_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12981 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/journal_entry/utils/description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12676 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/journal_entry/utils/operators.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3722 2023-04-23 05:21:41.000000 mia-accounting-1.5.1/src/accounting/journal_entry/utils/original_line_items.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9351 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/journal_entry/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.5.1/src/accounting/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32517 2023-04-29 21:51:30.000000 mia-accounting-1.5.1/src/accounting/models.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.722057 mia-accounting-1.5.1/src/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.5.1/src/accounting/option/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.5.1/src/accounting/option/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.5.1/src/accounting/option/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.726057 mia-accounting-1.5.1/src/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.5.1/src/accounting/report/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.5.1/src/accounting/report/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.726057 mia-accounting-1.5.1/src/accounting/report/period/
+-rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.5.1/src/accounting/report/period/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3702 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/period/chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5557 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/period/description.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1050 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/period/month_end.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4127 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/period/parser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4522 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/period/period.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4785 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/period/shortcuts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3915 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/period/specification.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.730057 mia-accounting-1.5.1/src/accounting/report/reports/
+-rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.5.1/src/accounting/report/reports/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.5.1/src/accounting/report/reports/balance_sheet.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18807 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/reports/income_expenses.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.5.1/src/accounting/report/reports/income_statement.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8130 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/reports/journal.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16530 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/reports/ledger.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8472 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/reports/search.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.5.1/src/accounting/report/reports/trial_balance.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8099 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/reports/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5210 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/reports/unapplied_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8169 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/reports/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5191 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/reports/unmatched_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.5.1/src/accounting/report/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.730057 mia-accounting-1.5.1/src/accounting/report/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.5.1/src/accounting/report/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/utils/base_page_params.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.5.1/src/accounting/report/utils/base_report.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3334 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/utils/csv_export.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7369 2023-04-18 01:18:28.000000 mia-accounting-1.5.1/src/accounting/report/utils/offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.5.1/src/accounting/report/utils/option_link.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7881 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/report/utils/report_chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1371 2023-04-17 08:41:57.000000 mia-accounting-1.5.1/src/accounting/report/utils/report_type.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4385 2023-04-23 05:21:41.000000 mia-accounting-1.5.1/src/accounting/report/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2221 2023-04-23 05:21:41.000000 mia-accounting-1.5.1/src/accounting/report/utils/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5440 2023-04-18 00:59:05.000000 mia-accounting-1.5.1/src/accounting/report/utils/urls.py
+-rw-r--r--   0 imacat    (1000) users      (100)    14167 2023-04-18 01:14:44.000000 mia-accounting-1.5.1/src/accounting/report/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.670058 mia-accounting-1.5.1/src/accounting/static/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.730057 mia-accounting-1.5.1/src/accounting/static/css/
+-rw-r--r--   0 imacat    (1000) users      (100)    13431 2023-04-18 00:10:33.000000 mia-accounting-1.5.1/src/accounting/static/css/style.css
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.734057 mia-accounting-1.5.1/src/accounting/static/js/
+-rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.5.1/src/accounting/static/js/account-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.5.1/src/accounting/static/js/account-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.5.1/src/accounting/static/js/currency-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    38865 2023-04-17 23:44:56.000000 mia-accounting-1.5.1/src/accounting/static/js/description-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.5.1/src/accounting/static/js/drag-and-drop-reorder.js
+-rw-r--r--   0 imacat    (1000) users      (100)     9211 2023-04-17 23:32:14.000000 mia-accounting-1.5.1/src/accounting/static/js/journal-entry-account-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    33086 2023-04-17 23:52:58.000000 mia-accounting-1.5.1/src/accounting/static/js/journal-entry-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    19524 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/static/js/journal-entry-line-item-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.5.1/src/accounting/static/js/journal-entry-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.5.1/src/accounting/static/js/material-fab-speed-dial.js
+-rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.5.1/src/accounting/static/js/option-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    11670 2023-04-17 23:40:31.000000 mia-accounting-1.5.1/src/accounting/static/js/original-line-item-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.5.1/src/accounting/static/js/period-chooser.js
+-rw-r--r--   0 imacat    (1000) users      (100)     2712 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/template_filters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1137 2023-04-23 01:43:59.000000 mia-accounting-1.5.1/src/accounting/template_globals.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.670058 mia-accounting-1.5.1/src/accounting/templates/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.734057 mia-accounting-1.5.1/src/accounting/templates/accounting/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.734057 mia-accounting-1.5.1/src/accounting/templates/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/account/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/account/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.734057 mia-accounting-1.5.1/src/accounting/templates/accounting/account/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/account/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/account/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.734057 mia-accounting-1.5.1/src/accounting/templates/accounting/base-account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/base-account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/base-account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/base.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.734057 mia-accounting-1.5.1/src/accounting/templates/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/currency/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/currency/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/currency/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.734057 mia-accounting-1.5.1/src/accounting/templates/accounting/currency/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/currency/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/currency/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.738057 mia-accounting-1.5.1/src/accounting/templates/accounting/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-17 15:07:31.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/include/nav.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/include/pagination.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.738057 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.738057 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/disbursement/
+-rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/disbursement/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.738057 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/disbursement/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.738057 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3406 2023-04-17 23:32:14.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)    14492 2023-04-17 23:42:37.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3242 2023-04-17 23:11:57.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4554 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6442 2023-04-17 23:54:15.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3791 2023-04-18 00:10:33.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3069 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.738057 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/receipt/
+-rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/receipt/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/receipt/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/receipt/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.738057 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/receipt/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.738057 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/transfer/
+-rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/transfer/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/transfer/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/transfer/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.738057 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/transfer/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.742057 mia-accounting-1.5.1/src/accounting/templates/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/option/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/option/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.742057 mia-accounting-1.5.1/src/accounting/templates/accounting/option/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/option/include/form-recurring-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.742057 mia-accounting-1.5.1/src/accounting/templates/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     5435 2023-04-18 00:39:27.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/balance-sheet.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.742057 mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/balance-sheet-section.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/period-chooser.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/search-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     5600 2023-04-18 00:10:33.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/toolbar-buttons.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4841 2023-04-18 00:34:44.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/income-expenses.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4618 2023-04-18 00:37:47.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/income-statement.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/journal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4946 2023-04-18 00:33:38.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/ledger.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/search.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3710 2023-04-18 00:36:16.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/trial-balance.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3037 2023-04-18 00:59:05.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/unapplied-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3843 2023-04-18 00:59:06.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/unapplied.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-18 00:59:05.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/unmatched-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6998 2023-04-18 00:59:05.000000 mia-accounting-1.5.1/src/accounting/templates/accounting/report/unmatched.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.766057 mia-accounting-1.5.1/src/accounting/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)    49437 2023-04-18 01:32:01.000000 mia-accounting-1.5.1/src/accounting/translations/accounting.pot
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.5.1/src/accounting/translations/babel.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.670058 mia-accounting-1.5.1/src/accounting/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.790056 mia-accounting-1.5.1/src/accounting/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.670058 mia-accounting-1.5.1/src/accounting/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.794056 mia-accounting-1.5.1/src/accounting/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.802056 mia-accounting-1.5.1/src/accounting/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.5.1/src/accounting/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1058 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/utils/cast.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3363 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/utils/current_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1426 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/utils/flash_errors.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.5.1/src/accounting/utils/journal_entry_types.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.5.1/src/accounting/utils/next_uri.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/utils/offset_alias.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.5.1/src/accounting/utils/options.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11745 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/utils/pagination.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4262 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/utils/permission.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.5.1/src/accounting/utils/query.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1221 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/utils/random_id.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.5.1/src/accounting/utils/strip_text.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4985 2023-04-29 21:45:46.000000 mia-accounting-1.5.1/src/accounting/utils/user.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.802056 mia-accounting-1.5.1/src/mia_accounting.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-04-29 21:54:28.000000 mia-accounting-1.5.1/src/mia_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)    11434 2023-04-29 21:54:28.000000 mia-accounting-1.5.1/src/mia_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-29 21:54:28.000000 mia-accounting-1.5.1/src/mia_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)      107 2023-04-29 21:54:28.000000 mia-accounting-1.5.1/src/mia_accounting.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-29 21:54:28.000000 mia-accounting-1.5.1/src/mia_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.806056 mia-accounting-1.5.1/tests/
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.5.1/tests/babel-utils-test-site.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.5.1/tests/babel-utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32727 2023-04-29 21:45:47.000000 mia-accounting-1.5.1/tests/test_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.5.1/tests/test_base_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-29 21:45:47.000000 mia-accounting-1.5.1/tests/test_commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)    23815 2023-04-29 21:45:47.000000 mia-accounting-1.5.1/tests/test_currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15998 2023-04-29 21:45:47.000000 mia-accounting-1.5.1/tests/test_description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)   103428 2023-04-29 21:45:47.000000 mia-accounting-1.5.1/tests/test_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    38887 2023-04-13 01:09:51.000000 mia-accounting-1.5.1/tests/test_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15940 2023-04-29 21:45:47.000000 mia-accounting-1.5.1/tests/test_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17864 2023-04-29 21:45:47.000000 mia-accounting-1.5.1/tests/test_report.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.806056 mia-accounting-1.5.1/tests/test_site/
+-rw-r--r--   0 imacat    (1000) users      (100)     4508 2023-04-29 21:45:47.000000 mia-accounting-1.5.1/tests/test_site/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3958 2023-04-29 21:45:47.000000 mia-accounting-1.5.1/tests/test_site/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13199 2023-04-29 21:45:47.000000 mia-accounting-1.5.1/tests/test_site/lib.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.5.1/tests/test_site/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13050 2023-04-29 21:45:47.000000 mia-accounting-1.5.1/tests/test_site/reset.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.806056 mia-accounting-1.5.1/tests/test_site/static/
+-rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.5.1/tests/test_site/static/favicon.svg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.838055 mia-accounting-1.5.1/tests/test_site/templates/
+-rw-r--r--   0 imacat    (1000) users      (100)     6435 2023-04-12 10:05:13.000000 mia-accounting-1.5.1/tests/test_site/templates/base.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.5.1/tests/test_site/templates/home.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.5.1/tests/test_site/templates/login.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.5.1/tests/test_site/templates/reset.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.854055 mia-accounting-1.5.1/tests/test_site/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.5.1/tests/test_site/translations/babel.cfg
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.5.1/tests/test_site/translations/messages.pot
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.674058 mia-accounting-1.5.1/tests/test_site/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.870055 mia-accounting-1.5.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.5.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.674058 mia-accounting-1.5.1/tests/test_site/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-29 21:54:28.898054 mia-accounting-1.5.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.5.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0 imacat    (1000) users      (100)    27794 2023-04-18 01:14:44.000000 mia-accounting-1.5.1/tests/test_unmatched_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.5.1/tests/test_utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5175 2023-04-29 21:45:47.000000 mia-accounting-1.5.1/tests/testlib.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16669 2023-04-29 21:45:47.000000 mia-accounting-1.5.1/tests/testlib_journal_entry.py
```

### Comparing `mia-accounting-1.5.0/LICENSE` & `mia-accounting-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/MANIFEST.in` & `mia-accounting-1.5.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/PKG-INFO` & `mia-accounting-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.5.0
+Version: 1.5.1
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
```

### Comparing `mia-accounting-1.5.0/README.rst` & `mia-accounting-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/Makefile` & `mia-accounting-1.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/make.bat` & `mia-accounting-1.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/accounting.account.rst` & `mia-accounting-1.5.1/docs/source/accounting.account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/accounting.base_account.rst` & `mia-accounting-1.5.1/docs/source/accounting.base_account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/accounting.currency.rst` & `mia-accounting-1.5.1/docs/source/accounting.currency.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/accounting.journal_entry.forms.rst` & `mia-accounting-1.5.1/docs/source/accounting.journal_entry.forms.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/accounting.journal_entry.rst` & `mia-accounting-1.5.1/docs/source/accounting.journal_entry.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/accounting.journal_entry.utils.rst` & `mia-accounting-1.5.1/docs/source/accounting.journal_entry.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/accounting.option.rst` & `mia-accounting-1.5.1/docs/source/accounting.option.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/accounting.report.period.rst` & `mia-accounting-1.5.1/docs/source/accounting.report.period.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/accounting.report.reports.rst` & `mia-accounting-1.5.1/docs/source/accounting.report.reports.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/accounting.report.rst` & `mia-accounting-1.5.1/docs/source/accounting.report.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/accounting.report.utils.rst` & `mia-accounting-1.5.1/docs/source/accounting.report.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/accounting.rst` & `mia-accounting-1.5.1/docs/source/accounting.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/accounting.utils.rst` & `mia-accounting-1.5.1/docs/source/accounting.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/changelog.rst` & `mia-accounting-1.5.1/docs/source/changelog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,19 @@
-Changes
-=======
+Change Log
+==========
+
+
+Version 1.5.1
+-------------
+
+Released 2023/4/30
+
+* Fixed the error calling the old ``setEnableDescriptionAccount``
+  method in the ``saveOriginalLineItem`` method of the JavaScript
+  ``JournalEntryLineItemEditor`` class.
 
 
 Version 1.5.0
 -------------
 
 Released 2023/4/23
```

### Comparing `mia-accounting-1.5.0/docs/source/conf.py` & `mia-accounting-1.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/examples.rst` & `mia-accounting-1.5.1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/history.rst` & `mia-accounting-1.5.1/docs/source/history.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/index.rst` & `mia-accounting-1.5.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/docs/source/intro.rst` & `mia-accounting-1.5.1/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/pyproject.toml` & `mia-accounting-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/__init__.py` & `mia-accounting-1.5.1/src/accounting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pathlib import Path
 
 from flask import Flask, Blueprint
 from flask_sqlalchemy import SQLAlchemy
 
 from accounting.utils.user import UserUtilityInterface
 
-VERSION: str = "1.5.0"
+VERSION: str = "1.5.1"
 """The package version."""
 db: SQLAlchemy = SQLAlchemy()
 """The database instance."""
 data_dir: Path = Path(__file__).parent / "data"
 """The data directory."""
```

### Comparing `mia-accounting-1.5.0/src/accounting/account/__init__.py` & `mia-accounting-1.5.1/src/accounting/account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/account/commands.py` & `mia-accounting-1.5.1/src/accounting/account/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The console commands for the account management.
 
 """
-import typing as t
 from secrets import randbelow
+from typing import Any
 
 import click
+import sqlalchemy as sa
 
 from accounting import db
 from accounting.models import BaseAccount, Account, AccountL10n
 from accounting.utils.user import get_user_pk
-import sqlalchemy as sa
 
 AccountData = tuple[int, str, int, str, str, str, bool]
 """The format of the account data, as a list of (ID, base account code, number,
 English, Traditional Chinese, Simplified Chinese, is-need-offset) tuples."""
 
 
 def init_accounts_command(username: str) -> None:
@@ -59,16 +59,16 @@
         """
         while True:
             new_id: int = 100000000 + randbelow(900000000)
             if new_id not in existing_id:
                 existing_id.add(new_id)
                 return new_id
 
-    data: list[dict[str, t.Any]] = []
-    l10n_data: list[dict[str, t.Any]] = []
+    data: list[dict[str, Any]] = []
+    l10n_data: list[dict[str, Any]] = []
     for base in bases_to_add:
         l10n: dict[str, str] = {x.locale: x.title for x in base.l10n}
         account_id: int = get_new_id()
         data.append({"id": account_id,
                      "base_code": base.code,
                      "no": 1,
                      "title_l10n": base.title_l10n,
```

### Comparing `mia-accounting-1.5.0/src/accounting/account/converters.py` & `mia-accounting-1.5.1/src/accounting/account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/account/forms.py` & `mia-accounting-1.5.1/src/accounting/account/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/account/queries.py` & `mia-accounting-1.5.1/src/accounting/account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/account/views.py` & `mia-accounting-1.5.1/src/accounting/account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/base_account/__init__.py` & `mia-accounting-1.5.1/src/accounting/base_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/base_account/commands.py` & `mia-accounting-1.5.1/src/accounting/base_account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/base_account/converters.py` & `mia-accounting-1.5.1/src/accounting/base_account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/base_account/queries.py` & `mia-accounting-1.5.1/src/accounting/base_account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/base_account/views.py` & `mia-accounting-1.5.1/src/accounting/base_account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/commands.py` & `mia-accounting-1.5.1/src/accounting/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/currency/__init__.py` & `mia-accounting-1.5.1/src/accounting/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/currency/commands.py` & `mia-accounting-1.5.1/src/accounting/currency/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The console commands for the currency management.
 
 """
 import csv
-import typing as t
+from typing import Any
 
 import sqlalchemy as sa
 
 from accounting import db, data_dir
 from accounting.models import Currency, CurrencyL10n
 from accounting.utils.user import get_user_pk
 
@@ -35,19 +35,19 @@
         data: list[dict[str, str]] = [x for x in csv.DictReader(fp)]
     to_add: list[dict[str, str]] = [x for x in data
                                     if x["code"] not in existing_codes]
     if len(to_add) == 0:
         return
 
     creator_pk: int = get_user_pk(username)
-    currency_data: list[dict[str, t.Any]] = [{"code": x["code"],
-                                              "name_l10n": x["name"],
-                                              "created_by_id": creator_pk,
-                                              "updated_by_id": creator_pk}
-                                             for x in to_add]
+    currency_data: list[dict[str, Any]] = [{"code": x["code"],
+                                            "name_l10n": x["name"],
+                                            "created_by_id": creator_pk,
+                                            "updated_by_id": creator_pk}
+                                           for x in to_add]
     locales: list[str] = [x[5:] for x in to_add[0] if x.startswith("l10n-")]
     l10n_data: list[dict[str, str]] = [{"currency_code": x["code"],
                                         "locale": y,
                                         "name": x[f"l10n-{y}"]}
                                        for x in to_add for y in locales]
     db.session.execute(sa.insert(Currency), currency_data)
     db.session.execute(sa.insert(CurrencyL10n), l10n_data)
```

### Comparing `mia-accounting-1.5.0/src/accounting/currency/converters.py` & `mia-accounting-1.5.1/src/accounting/currency/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/currency/forms.py` & `mia-accounting-1.5.1/src/accounting/currency/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/currency/queries.py` & `mia-accounting-1.5.1/src/accounting/currency/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/currency/views.py` & `mia-accounting-1.5.1/src/accounting/currency/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/data/base_accounts.csv` & `mia-accounting-1.5.1/src/accounting/data/base_accounts.csv`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/forms.py` & `mia-accounting-1.5.1/src/accounting/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/__init__.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/converters.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The path converters for the journal entry management.
 
 """
-from datetime import date
+import datetime as dt
 
 from flask import abort
 from werkzeug.routing import BaseConverter
 
 from accounting import db
 from accounting.models import JournalEntry
 from accounting.utils.journal_entry_types import JournalEntryType
@@ -78,25 +78,25 @@
         return str(value.value)
 
 
 class DateConverter(BaseConverter):
     """The date converter to convert the ISO date from and to the
     corresponding date in the routes."""
 
-    def to_python(self, value: str) -> date:
+    def to_python(self, value: str) -> dt.date:
         """Converts an ISO date to a date.
 
         :param value: The ISO date.
         :return: The corresponding date.
         """
         try:
-            return date.fromisoformat(value)
+            return dt.date.fromisoformat(value)
         except ValueError:
             abort(404)
 
-    def to_url(self, value: date) -> str:
+    def to_url(self, value: dt.date) -> str:
         """Converts a date to its ISO date.
 
         :param value: The date.
         :return: The ISO date.
         """
         return value.isoformat()
```

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/forms/__init__.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/forms/currency.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/forms/currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/forms/journal_entry.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/forms/journal_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The journal entry forms for the journal entry management.
 
 """
 import datetime as dt
-import typing as t
 from abc import ABC, abstractmethod
+from typing import TypeVar, Generic, Type
 
 import sqlalchemy as sa
 from flask_babel import LazyString
 from flask_wtf import FlaskForm
 from wtforms import DateField, FieldList, FormField, TextAreaField, \
     BooleanField
 from wtforms.validators import DataRequired, ValidationError
 
 from accounting import db
-from accounting.locale import lazy_gettext
-from accounting.models import JournalEntry, Account, JournalEntryLineItem, \
-    JournalEntryCurrency
 from accounting.journal_entry.utils.account_option import AccountOption
+from accounting.journal_entry.utils.description_editor import DescriptionEditor
 from accounting.journal_entry.utils.original_line_items import \
     get_selectable_original_line_items
-from accounting.journal_entry.utils.description_editor import DescriptionEditor
+from accounting.locale import lazy_gettext
+from accounting.models import JournalEntry, Account, JournalEntryLineItem, \
+    JournalEntryCurrency
 from accounting.utils.random_id import new_id
 from accounting.utils.strip_text import strip_multiline_text
 from accounting.utils.user import get_current_user_pk
 from .currency import CurrencyForm, CashReceiptCurrencyForm, \
     CashDisbursementCurrencyForm, TransferCurrencyForm
 from .line_item import LineItemForm, DebitLineItemForm, CreditLineItemForm
 from .reorder import sort_journal_entries_in
@@ -119,15 +119,15 @@
 
         :param args: The arguments.
         :param kwargs: The keyword arguments.
         """
         super().__init__(*args, **kwargs)
         self.is_modified: bool = False
         """Whether the journal entry is modified during populate_obj()."""
-        self.collector: t.Type[LineItemCollector] = LineItemCollector
+        self.collector: Type[LineItemCollector] = LineItemCollector
         """The line item collector.  The default is the base abstract
         collector only to provide the correct type.  The subclass forms should
         provide their own collectors."""
         self.obj: JournalEntry | None = kwargs.get("obj")
         """The journal entry, when editing an existing one."""
         self._is_need_payable: bool = False
         """Whether we need the payable original line items."""
@@ -151,15 +151,15 @@
         is_new: bool = obj.id is None
         if is_new:
             obj.id = new_id(JournalEntry)
         self.date: DateField
         self.__set_date(obj, self.date.data)
         obj.note = self.note.data
 
-        collector_cls: t.Type[LineItemCollector] = self.collector
+        collector_cls: Type[LineItemCollector] = self.collector
         collector: collector_cls = collector_cls(self, obj)
         collector.collect()
 
         to_delete: set[int] = {x.id for x in obj.line_items
                                if x.id not in collector.to_keep}
         if len(to_delete) > 0:
             JournalEntryLineItem.query\
@@ -305,19 +305,19 @@
         select: sa.Select = sa.select(sa.func.min(JournalEntry.date))\
             .join(JournalEntryLineItem)\
             .filter(JournalEntryLineItem.original_line_item_id
                     .in_(line_item_id))
         return db.session.scalar(select)
 
 
-T = t.TypeVar("T", bound=JournalEntryForm)
+T = TypeVar("T", bound=JournalEntryForm)
 """A journal entry form variant."""
 
 
-class LineItemCollector(t.Generic[T], ABC):
+class LineItemCollector(Generic[T], ABC):
     """The line item collector."""
 
     def __init__(self, form: T, obj: JournalEntry):
         """Constructs the line item collector.
 
         :param form: The journal entry form.
         :param obj: The journal entry.
```

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/forms/line_item.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/forms/line_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The line item sub-forms for the journal entry management.
 
 """
-from datetime import date
+import datetime as dt
 from decimal import Decimal
 
 import sqlalchemy as sa
 from flask_babel import LazyString
 from flask_wtf import FlaskForm
 from sqlalchemy.orm import selectinload
 from wtforms import StringField, ValidationError, DecimalField, IntegerField
@@ -303,15 +303,15 @@
                     return None
                 return db.session.get(JournalEntryLineItem,
                                       self.original_line_item_id.data)
             setattr(self, "____original_line_item", get_line_item())
         return getattr(self, "____original_line_item")
 
     @property
-    def original_line_item_date(self) -> date | None:
+    def original_line_item_date(self) -> dt.date | None:
         """Returns the text representation of the original line item.
 
         :return: The text representation of the original line item.
         """
         return None if self.__original_line_item is None \
             else self.__original_line_item.journal_entry.date
```

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/forms/reorder.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/forms/reorder.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,53 +13,51 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The reorder forms for the journal entry management.
 
 """
-from datetime import date
+import datetime as dt
 
 import sqlalchemy as sa
 from flask import request
 
 from accounting import db
 from accounting.models import JournalEntry
 
 
-def sort_journal_entries_in(journal_entry_date: date,
-                            exclude: int | None = None) -> None:
+def sort_journal_entries_in(date: dt.date, exclude: int | None = None) -> None:
     """Sorts the journal entries under a date after changing the date or
     deleting a journal entry.
 
-    :param journal_entry_date: The date of the journal entry.
+    :param date: The date of the journal entry.
     :param exclude: The journal entry ID to exclude.
     :return: None.
     """
-    conditions: list[sa.BinaryExpression] \
-        = [JournalEntry.date == journal_entry_date]
+    conditions: list[sa.BinaryExpression] = [JournalEntry.date == date]
     if exclude is not None:
         conditions.append(JournalEntry.id != exclude)
     journal_entries: list[JournalEntry] = JournalEntry.query\
         .filter(*conditions)\
         .order_by(JournalEntry.no).all()
     for i in range(len(journal_entries)):
         if journal_entries[i].no != i + 1:
             journal_entries[i].no = i + 1
 
 
 class JournalEntryReorderForm:
     """The form to reorder the journal entries."""
 
-    def __init__(self, journal_entry_date: date):
+    def __init__(self, date: dt.date):
         """Constructs the form to reorder the journal entries in a day.
 
-        :param journal_entry_date: The date.
+        :param date: The date.
         """
-        self.date: date = journal_entry_date
+        self.date: dt.date = date
         self.is_modified: bool = False
 
     def save_order(self) -> None:
         """Saves the order of the account.
 
         :return:
         """
```

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/template_filters.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/utils/__init__.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/utils/account_option.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/utils/account_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/utils/description_editor.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/utils/description_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The description editor.
 
 """
 import re
-import typing as t
+from typing import Literal
 
 import sqlalchemy as sa
 
 from accounting import db
 from accounting.models import Account, JournalEntryLineItem
 from accounting.utils.options import options, Recurring
 
@@ -120,20 +120,20 @@
         """
         return [x.code for x in self.accounts]
 
 
 class DescriptionType:
     """A description type"""
 
-    def __init__(self, type_id: t.Literal["general", "travel", "bus"]):
+    def __init__(self, type_id: Literal["general", "travel", "bus"]):
         """Constructs a description type.
 
         :param type_id: The type ID, either "general", "travel", or "bus".
         """
-        self.id: t.Literal["general", "travel", "bus"] = type_id
+        self.id: Literal["general", "travel", "bus"] = type_id
         """The type ID."""
         self.__tag_dict: dict[str, DescriptionTag] = {}
         """A dictionary from the tag name to their corresponding tag."""
 
     def add_tag(self, name: str, account: Account, freq: int) -> None:
         """Adds a tag.
 
@@ -177,35 +177,35 @@
         """
         return [self.account.code]
 
 
 class DescriptionDebitCredit:
     """The description on debit or credit."""
 
-    def __init__(self, debit_credit: t.Literal["debit", "credit"]):
+    def __init__(self, debit_credit: Literal["debit", "credit"]):
         """Constructs the description on debit or credit.
 
         :param debit_credit: Either "debit" or "credit".
         """
-        self.debit_credit: t.Literal["debit", "credit"] = debit_credit
+        self.debit_credit: Literal["debit", "credit"] = debit_credit
         """Either debit or credit."""
         self.general: DescriptionType = DescriptionType("general")
         """The general tags."""
         self.travel: DescriptionType = DescriptionType("travel")
         """The travel tags."""
         self.bus: DescriptionType = DescriptionType("bus")
         """The bus tags."""
-        self.__type_dict: dict[t.Literal["general", "travel", "bus"],
+        self.__type_dict: dict[Literal["general", "travel", "bus"],
                                DescriptionType] \
             = {x.id: x for x in {self.general, self.travel, self.bus}}
         """A dictionary from the type ID to the corresponding tags."""
         self.recurring: list[DescriptionRecurring] = []
         """The recurring transactions."""
 
-    def add_tag(self, tag_type: t.Literal["general", "travel", "bus"],
+    def add_tag(self, tag_type: Literal["general", "travel", "bus"],
                 name: str, account: Account, freq: int) -> None:
         """Adds a tag.
 
         :param tag_type: The tag type, either "general", "travel", or "bus".
         :param name: The name.
         :param account: The associated account.
         :param freq: The frequency of the tag name with the account.
@@ -274,15 +274,15 @@
                     JournalEntryLineItem.original_line_item_id.is_(None))\
             .group_by(debit_credit, tag_type, tag,
                       JournalEntryLineItem.account_id)
         result: list[sa.Row] = db.session.execute(select).all()
         accounts: dict[int, Account] \
             = {x.id: x for x in Account.query
                .filter(Account.id.in_({x.account_id for x in result})).all()}
-        debit_credit_dict: dict[t.Literal["debit", "credit"],
+        debit_credit_dict: dict[Literal["debit", "credit"],
                                 DescriptionDebitCredit] \
             = {x.debit_credit: x for x in {self.debit, self.credit}}
         for row in result:
             debit_credit_dict[row.debit_credit].add_tag(
                 row.tag_type, row.tag, accounts[row.account_id], row.freq)
 
     def __init_recurring(self) -> None:
```

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/utils/operators.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/utils/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,37 +13,37 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The operators for different journal entry types.
 
 """
-import typing as t
 from abc import ABC, abstractmethod
+from typing import Type
 
 from flask import render_template, request, abort
 from flask_wtf import FlaskForm
 
-from accounting.models import JournalEntry
-from accounting.template_globals import default_currency_code
-from accounting.utils.journal_entry_types import JournalEntryType
 from accounting.journal_entry.forms import JournalEntryForm, \
     CashReceiptJournalEntryForm, CashDisbursementJournalEntryForm, \
     TransferJournalEntryForm
 from accounting.journal_entry.forms.line_item import LineItemForm
+from accounting.models import JournalEntry
+from accounting.template_globals import default_currency_code
+from accounting.utils.journal_entry_types import JournalEntryType
 
 
 class JournalEntryOperator(ABC):
     """The base journal entry operator."""
     CHECK_ORDER: int = -1
     """The order when checking the journal entry operator."""
 
     @property
     @abstractmethod
-    def form(self) -> t.Type[JournalEntryForm]:
+    def form(self) -> Type[JournalEntryForm]:
         """Returns the form class.
 
         :return: The form class.
         """
 
     @abstractmethod
     def render_create_template(self, form: FlaskForm) -> str:
@@ -96,15 +96,15 @@
 
 class CashReceiptJournalEntry(JournalEntryOperator):
     """A cash receipt journal entry."""
     CHECK_ORDER: int = 2
     """The order when checking the journal entry operator."""
 
     @property
-    def form(self) -> t.Type[JournalEntryForm]:
+    def form(self) -> Type[JournalEntryForm]:
         """Returns the form class.
 
         :return: The form class.
         """
         return CashReceiptJournalEntryForm
 
     def render_create_template(self, form: CashReceiptJournalEntryForm) -> str:
@@ -166,15 +166,15 @@
 
 class CashDisbursementJournalEntry(JournalEntryOperator):
     """A cash disbursement journal entry."""
     CHECK_ORDER: int = 1
     """The order when checking the journal entry operator."""
 
     @property
-    def form(self) -> t.Type[JournalEntryForm]:
+    def form(self) -> Type[JournalEntryForm]:
         """Returns the form class.
 
         :return: The form class.
         """
         return CashDisbursementJournalEntryForm
 
     def render_create_template(self, form: CashDisbursementJournalEntryForm) \
@@ -239,15 +239,15 @@
 
 class TransferJournalEntry(JournalEntryOperator):
     """A transfer journal entry."""
     CHECK_ORDER: int = 3
     """The order when checking the journal entry operator."""
 
     @property
-    def form(self) -> t.Type[JournalEntryForm]:
+    def form(self) -> Type[JournalEntryForm]:
         """Returns the form class.
 
         :return: The form class.
         """
         return TransferJournalEntryForm
 
     def render_create_template(self, form: TransferJournalEntryForm) -> str:
```

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/utils/original_line_items.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/utils/original_line_items.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/journal_entry/views.py` & `mia-accounting-1.5.1/src/accounting/journal_entry/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The views for the journal entry management.
 
 """
-from datetime import date
+import datetime as dt
 from urllib.parse import parse_qsl, urlencode
 
 import sqlalchemy as sa
 from flask import Blueprint, render_template, session, redirect, request, \
     flash, url_for
 from werkzeug.datastructures import ImmutableMultiDict
 
 from accounting import db
 from accounting.locale import lazy_gettext
 from accounting.models import JournalEntry
 from accounting.utils.cast import s
 from accounting.utils.flash_errors import flash_form_errors
+from accounting.utils.journal_entry_types import JournalEntryType
 from accounting.utils.next_uri import inherit_next, or_next
 from accounting.utils.permission import has_permission, can_view, can_edit
-from accounting.utils.journal_entry_types import JournalEntryType
 from accounting.utils.user import get_current_user_pk
 from .forms import sort_journal_entries_in, JournalEntryReorderForm
 from .template_filters import with_type, to_transfer, format_amount_input, \
     text2html
 from .utils.operators import JournalEntryOperator, JOURNAL_ENTRY_TYPE_TO_OP, \
     get_journal_entry_op
 
@@ -63,15 +63,15 @@
     if "form" in session:
         form = journal_entry_op.form(
             ImmutableMultiDict(parse_qsl(session["form"])))
         del session["form"]
         form.validate()
     else:
         form = journal_entry_op.form()
-        form.date.data = date.today()
+        form.date.data = dt.date.today()
     return journal_entry_op.render_create_template(form)
 
 
 @bp.post("store/<journalEntryType:journal_entry_type>", endpoint="store")
 @has_permission(can_edit)
 def add_journal_entry(journal_entry_type: JournalEntryType) -> redirect:
     """Adds a journal entry.
@@ -182,39 +182,39 @@
     sort_journal_entries_in(journal_entry.date, journal_entry.id)
     db.session.commit()
     flash(s(lazy_gettext("The journal entry is deleted successfully.")),
           "success")
     return redirect(or_next(__get_default_page_uri()))
 
 
-@bp.get("dates/<date:journal_entry_date>", endpoint="order")
+@bp.get("dates/<date:date>", endpoint="order")
 @has_permission(can_view)
-def show_journal_entry_order(journal_entry_date: date) -> str:
+def show_journal_entry_order(date: dt.date) -> str:
     """Shows the order of the journal entries in a same date.
 
-    :param journal_entry_date: The date.
+    :param date: The date.
     :return: The order of the journal entries in the date.
     """
     journal_entries: list[JournalEntry] = JournalEntry.query \
-        .filter(JournalEntry.date == journal_entry_date) \
+        .filter(JournalEntry.date == date) \
         .order_by(JournalEntry.no).all()
     return render_template("accounting/journal-entry/order.html",
-                           date=journal_entry_date, list=journal_entries)
+                           date=date, list=journal_entries)
 
 
-@bp.post("dates/<date:journal_entry_date>", endpoint="sort")
+@bp.post("dates/<date:date>", endpoint="sort")
 @has_permission(can_edit)
-def sort_journal_entries(journal_entry_date: date) -> redirect:
+def sort_journal_entries(date: dt.date) -> redirect:
     """Reorders the journal entries in a date.
 
-    :param journal_entry_date: The date.
+    :param date: The date.
     :return: The redirection to the incoming account or the account list.  The
         reordering operation does not fail.
     """
-    form: JournalEntryReorderForm = JournalEntryReorderForm(journal_entry_date)
+    form: JournalEntryReorderForm = JournalEntryReorderForm(date)
     form.save_order()
     if not form.is_modified:
         flash(s(lazy_gettext("The order was not modified.")), "success")
         return redirect(or_next(__get_default_page_uri()))
     db.session.commit()
     flash(s(lazy_gettext("The order is updated successfully.")), "success")
     return redirect(or_next(__get_default_page_uri()))
```

### Comparing `mia-accounting-1.5.0/src/accounting/locale.py` & `mia-accounting-1.5.1/src/accounting/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/models.py` & `mia-accounting-1.5.1/src/accounting/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 """The data models.
 
 """
 from __future__ import annotations
 
 import datetime as dt
 import re
-import typing as t
 from decimal import Decimal
+from typing import Type, Self
 
 import sqlalchemy as sa
 from babel import Locale
 from flask_babel import get_locale, get_babel
 from sqlalchemy import text
 from sqlalchemy.orm import Mapped, mapped_column
 
@@ -113,29 +113,29 @@
     title_l10n: Mapped[str] = mapped_column("title")
     """The title."""
     is_need_offset: Mapped[bool] = mapped_column(default=False)
     """Whether the journal entry line items of this account need offset."""
     created_at: Mapped[dt.datetime] \
         = mapped_column(db.DateTime(timezone=True),
                         server_default=db.func.now())
-    """The time of creation."""
+    """The date and time when this record was created."""
     created_by_id: Mapped[int] \
         = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
-    """The ID of the creator."""
+    """The ID of the user who created the record."""
     created_by: Mapped[user_cls] = db.relationship(foreign_keys=created_by_id)
-    """The creator."""
+    """The user who created the record."""
     updated_at: Mapped[dt.datetime] \
         = mapped_column(db.DateTime(timezone=True),
                         server_default=db.func.now())
-    """The time of last update."""
+    """The date and time when this record was last updated."""
     updated_by_id: Mapped[int] \
         = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
-    """The ID of the updator."""
+    """The ID of the last user who updated the record."""
     updated_by: Mapped[user_cls] = db.relationship(foreign_keys=updated_by_id)
-    """The updator."""
+    """The last user who updated the record."""
     l10n: Mapped[list[AccountL10n]] \
         = db.relationship(back_populates="account", lazy=False)
     """The localized titles."""
     line_items: Mapped[list[JournalEntryLineItem]] \
         = db.relationship(back_populates="account")
     """The journal entry line items."""
 
@@ -218,21 +218,21 @@
         :return: The number of items in the account.
         """
         if not hasattr(self, "__count"):
             setattr(self, "__count", 0)
         return getattr(self, "__count")
 
     @count.setter
-    def count(self, count: int) -> None:
+    def count(self, value: int) -> None:
         """Sets the number of items in the account.
 
-        :param count: The number of items in the account.
+        :param value: The number of items in the account.
         :return: None.
         """
-        setattr(self, "__count", count)
+        setattr(self, "__count", value)
 
     @property
     def query_values(self) -> list[str]:
         """Returns the values to be queried.
 
         :return: The values to be queried.
         """
@@ -263,32 +263,32 @@
 
     def delete(self) -> None:
         """Deletes this account.
 
         :return: None.
         """
         AccountL10n.query.filter(AccountL10n.account == self).delete()
-        cls: t.Type[t.Self] = self.__class__
+        cls: Type[Self] = self.__class__
         cls.query.filter(cls.id == self.id).delete()
 
     @classmethod
-    def find_by_code(cls, code: str) -> t.Self | None:
+    def find_by_code(cls, code: str) -> Self | None:
         """Finds an account by its code.
 
         :param code: The code.
         :return: The account, or None if this account does not exist.
         """
         m = re.match(r"^([1-9]{4})-(\d{3})$", code)
         if m is None:
             return None
         return cls.query.filter(cls.base_code == m.group(1),
                                 cls.no == int(m.group(2))).first()
 
     @classmethod
-    def selectable_debit(cls) -> list[t.Self]:
+    def selectable_debit(cls) -> list[Self]:
         """Returns the selectable debit accounts.
         Payable line items can not start from debit.
 
         :return: The selectable debit accounts.
         """
         return cls.query.filter(sa.or_(cls.base_code.startswith("1"),
                                        sa.and_(cls.base_code.startswith("2"),
@@ -303,15 +303,15 @@
                                        cls.base_code.startswith("8"),
                                        cls.base_code.startswith("9")),
                                 cls.base_code != "3351",
                                 cls.base_code != "3353")\
             .order_by(cls.base_code, cls.no).all()
 
     @classmethod
-    def selectable_credit(cls) -> list[t.Self]:
+    def selectable_credit(cls) -> list[Self]:
         """Returns the selectable debit accounts.
         Receivable line items can not start from credit.
 
         :return: The selectable debit accounts.
         """
         return cls.query.filter(sa.or_(sa.and_(cls.base_code.startswith("1"),
                                                sa.not_(cls.is_need_offset)),
@@ -325,23 +325,23 @@
                                        cls.base_code.startswith("8"),
                                        cls.base_code.startswith("9")),
                                 cls.base_code != "3351",
                                 cls.base_code != "3353")\
             .order_by(cls.base_code, cls.no).all()
 
     @classmethod
-    def cash(cls) -> t.Self:
+    def cash(cls) -> Self:
         """Returns the cash account.
 
         :return: The cash account
         """
         return cls.find_by_code(cls.CASH_CODE)
 
     @classmethod
-    def accumulated_change(cls) -> t.Self:
+    def accumulated_change(cls) -> Self:
         """Returns the accumulated-change account.
 
         :return: The accumulated-change account
         """
         return cls.find_by_code(cls.ACCUMULATED_CHANGE_CODE)
 
 
@@ -369,30 +369,30 @@
     code: Mapped[str] = mapped_column(primary_key=True)
     """The code."""
     name_l10n: Mapped[str] = mapped_column("name")
     """The name."""
     created_at: Mapped[dt.datetime] \
         = mapped_column(db.DateTime(timezone=True),
                         server_default=db.func.now())
-    """The time of creation."""
+    """The date and time when this record was created."""
     created_by_id: Mapped[int] \
         = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
-    """The ID of the creator."""
+    """The ID of the user who created the record."""
     created_by: Mapped[user_cls] = db.relationship(foreign_keys=created_by_id)
-    """The creator."""
+    """The user who created the record."""
     updated_at: Mapped[dt.datetime] \
         = mapped_column(db.DateTime(timezone=True),
                         server_default=db.func.now())
-    """The time of last update."""
+    """The date and time when this record was last updated."""
     updated_by_id: Mapped[int] \
         = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
-    """The ID of the updator."""
+    """The ID of the last user who updated the record."""
     updated_by: Mapped[user_cls] \
         = db.relationship(foreign_keys=updated_by_id)
-    """The updator."""
+    """The last user who updated the record."""
     l10n: Mapped[list[CurrencyL10n]] \
         = db.relationship(back_populates="currency", lazy=False)
     """The localized names."""
     line_items: Mapped[list[JournalEntryLineItem]] \
         = db.relationship(back_populates="currency")
     """The journal entry line items."""
 
@@ -463,15 +463,15 @@
 
     def delete(self) -> None:
         """Deletes the currency.
 
         :return: None.
         """
         CurrencyL10n.query.filter(CurrencyL10n.currency == self).delete()
-        cls: t.Type[t.Self] = self.__class__
+        cls: Type[Self] = self.__class__
         cls.query.filter(cls.code == self.code).delete()
 
 
 class CurrencyL10n(db.Model):
     """A localized currency name."""
     __tablename__ = "accounting_currencies_l10n"
     """The table name."""
@@ -542,29 +542,29 @@
     no: Mapped[int] = mapped_column(default=text("1"))
     """The account number under the date."""
     note: Mapped[str | None]
     """The note."""
     created_at: Mapped[dt.datetime] \
         = mapped_column(db.DateTime(timezone=True),
                         server_default=db.func.now())
-    """The time of creation."""
+    """The date and time when this record was created."""
     created_by_id: Mapped[int] \
         = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
-    """The ID of the creator."""
+    """The ID of the user who created the record."""
     created_by: Mapped[user_cls] = db.relationship(foreign_keys=created_by_id)
-    """The creator."""
+    """The user who created the record."""
     updated_at: Mapped[dt.datetime] \
         = mapped_column(db.DateTime(timezone=True),
                         server_default=db.func.now())
-    """The time of last update."""
+    """The date and time when this record was last updated."""
     updated_by_id: Mapped[int] \
         = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
-    """The ID of the updator."""
+    """The ID of the last user who updated the record."""
     updated_by: Mapped[user_cls] = db.relationship(foreign_keys=updated_by_id)
-    """The updator."""
+    """The last user who updated the record."""
     line_items: Mapped[list[JournalEntryLineItem]] \
         = db.relationship(back_populates="journal_entry")
     """The line items."""
 
     def __str__(self) -> str:
         """Returns the string representation of this journal entry.
 
@@ -731,90 +731,90 @@
         :return: The debit amount, or None if this is not a debit line item.
         """
         if not hasattr(self, "__debit"):
             setattr(self, "__debit", self.amount if self.is_debit else None)
         return getattr(self, "__debit")
 
     @debit.setter
-    def debit(self, debit: Decimal | None) -> None:
+    def debit(self, value: Decimal | None) -> None:
         """Sets the debit amount.
 
-        :param debit: The debit amount.
+        :param value: The debit amount.
         :return: None.
         """
-        setattr(self, "__debit", debit)
+        setattr(self, "__debit", value)
 
     @property
     def credit(self) -> Decimal | None:
         """Returns the credit amount.
 
         :return: The credit amount, or None if this is not a credit line item.
         """
         if not hasattr(self, "__credit"):
             setattr(self, "__credit", None if self.is_debit else self.amount)
         return getattr(self, "__credit")
 
     @credit.setter
-    def credit(self, credit: Decimal | None) -> None:
+    def credit(self, value: Decimal | None) -> None:
         """Sets the credit amount.
 
-        :param credit: The credit amount.
+        :param value: The credit amount.
         :return: None.
         """
-        setattr(self, "__credit", credit)
+        setattr(self, "__credit", value)
 
     @property
     def net_balance(self) -> Decimal:
         """Returns the net balance.
 
         :return: The net balance.
         """
         if not hasattr(self, "__net_balance"):
             setattr(self, "__net_balance", self.amount + sum(
                 [x.amount if x.is_debit == self.is_debit else -x.amount
                  for x in self.offsets]))
         return getattr(self, "__net_balance")
 
     @net_balance.setter
-    def net_balance(self, net_balance: Decimal) -> None:
+    def net_balance(self, value: Decimal) -> None:
         """Sets the net balance.
 
-        :param net_balance: The net balance.
+        :param value: The net balance.
         :return: None.
         """
-        setattr(self, "__net_balance", net_balance)
+        setattr(self, "__net_balance", value)
 
     @property
     def balance(self) -> Decimal:
-        """Returns the net balance.
+        """Returns the balance.
 
-        :return: The net balance.
+        :return: The balance.
         """
         if not hasattr(self, "__balance"):
             setattr(self, "__balance", Decimal("0"))
         return getattr(self, "__balance")
 
     @balance.setter
-    def balance(self, balance: Decimal) -> None:
-        """Sets the net balance.
+    def balance(self, value: Decimal) -> None:
+        """Sets the balance.
 
-        :param balance: The net balance.
+        :param value: The balance.
         :return: None.
         """
-        setattr(self, "__balance", balance)
+        setattr(self, "__balance", value)
 
     @property
-    def offsets(self) -> list[t.Self]:
+    def offsets(self) -> list[Self]:
         """Returns the offset items.
 
         :return: The offset items.
         """
         if not hasattr(self, "__offsets"):
-            cls: t.Type[t.Self] = self.__class__
-            offsets: list[t.Self] = cls.query.join(JournalEntry)\
+            cls: Type[Self] = self.__class__
+            offsets: list[Self] = cls.query.join(JournalEntry)\
                 .filter(JournalEntryLineItem.original_line_item_id == self.id)\
                 .order_by(JournalEntry.date, JournalEntry.no,
                           cls.is_debit, cls.no).all()
             setattr(self, "__offsets", offsets)
         return getattr(self, "__offsets")
 
     @property
@@ -824,41 +824,40 @@
         :return: True if the line item is an offset, or False otherwise.
         """
         if not hasattr(self, "__is_offset"):
             setattr(self, "__is_offset", False)
         return getattr(self, "__is_offset")
 
     @is_offset.setter
-    def is_offset(self, is_offset: bool) -> None:
+    def is_offset(self, value: bool) -> None:
         """Sets whether the line item is an offset.
 
-        :param is_offset: True if the line item is an offset, or False
-            otherwise.
+        :param value: True if the line item is an offset, or False otherwise.
         :return: None.
         """
-        setattr(self, "__is_offset", is_offset)
+        setattr(self, "__is_offset", value)
 
     @property
-    def match(self) -> t.Self | None:
+    def match(self) -> Self | None:
         """Returns the match of the line item.
 
         :return: The match of the line item.
         """
         if not hasattr(self, "__match"):
             setattr(self, "__match", None)
         return getattr(self, "__match")
 
     @match.setter
-    def match(self, match: t.Self) -> None:
+    def match(self, value: Self) -> None:
         """Sets the match of the line item.
 
-        :param match: The matcho of the line item.
+        :param value: The matcho of the line item.
         :return: None.
         """
-        setattr(self, "__match", match)
+        setattr(self, "__match", value)
 
     @property
     def query_values(self) -> list[str]:
         """Returns the values to be queried.
 
         :return: The values to be queried.
         """
@@ -882,22 +881,22 @@
     name: Mapped[str] = mapped_column(primary_key=True)
     """The name."""
     value: Mapped[str] = mapped_column(db.Text)
     """The option value."""
     created_at: Mapped[dt.datetime] \
         = mapped_column(db.DateTime(timezone=True),
                         server_default=db.func.now())
-    """The time of creation."""
+    """The date and time when this record was created."""
     created_by_id: Mapped[int] \
         = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
-    """The ID of the creator."""
+    """The ID of the user who created the record."""
     created_by: Mapped[user_cls] = db.relationship(foreign_keys=created_by_id)
-    """The creator."""
+    """The user who created the record."""
     updated_at: Mapped[dt.datetime] \
         = mapped_column(db.DateTime(timezone=True),
                         server_default=db.func.now())
-    """The time of last update."""
+    """The date and time when this record was last updated."""
     updated_by_id: Mapped[int] \
         = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
-    """The ID of the updator."""
+    """The ID of the last user who updated the record."""
     updated_by: Mapped[user_cls] = db.relationship(foreign_keys=updated_by_id)
-    """The updator."""
+    """The last user who updated the record."""
```

### Comparing `mia-accounting-1.5.0/src/accounting/option/__init__.py` & `mia-accounting-1.5.1/src/accounting/option/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/option/forms.py` & `mia-accounting-1.5.1/src/accounting/option/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/option/views.py` & `mia-accounting-1.5.1/src/accounting/option/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/__init__.py` & `mia-accounting-1.5.1/src/accounting/report/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/converters.py` & `mia-accounting-1.5.1/src/accounting/report/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/period/__init__.py` & `mia-accounting-1.5.1/src/accounting/report/period/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/period/chooser.py` & `mia-accounting-1.5.1/src/accounting/report/period/chooser.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 #  limitations under the License.
 """The period chooser.
 
 This file is largely taken from the NanoParma ERP project, first written in
 2021/9/16 by imacat (imacat@nanoparma.com).
 
 """
-import typing as t
-from datetime import date
+import datetime as dt
+from collections.abc import Callable
 
 from accounting.models import JournalEntry
 from .period import Period
 from .shortcuts import ThisMonth, LastMonth, SinceLastMonth, ThisYear, \
     LastYear, Today, Yesterday, AllTime, TemplatePeriod, YearPeriod
 
 
 class PeriodChooser:
     """The period chooser."""
 
-    def __init__(self, get_url: t.Callable[[Period], str]):
+    def __init__(self, get_url: Callable[[Period], str]):
         """Constructs a period chooser.
 
         :param get_url: The callback to return the URL of the current report in
             a period.
         """
-        self.__get_url: t.Callable[[Period], str] = get_url
+        self.__get_url: Callable[[Period], str] = get_url
         """The callback to return the URL of the current report in a period."""
 
         # Shortcut periods
         self.this_month_url: str = get_url(ThisMonth())
         """The URL for this month."""
         self.last_month_url: str = get_url(LastMonth())
         """The URL for last month."""
@@ -59,33 +59,33 @@
         self.all_url: str = get_url(AllTime())
         """The URL for all period."""
         self.url_template: str = get_url(TemplatePeriod())
         """The URL template."""
 
         first: JournalEntry | None \
             = JournalEntry.query.order_by(JournalEntry.date).first()
-        start: date | None = None if first is None else first.date
+        start: dt.date | None = None if first is None else first.date
 
         # Attributes
-        self.data_start: date | None = start
+        self.data_start: dt.date | None = start
         """The start of the data."""
         self.has_data: bool = start is not None
         """Whether there is any data."""
         self.has_last_month: bool = False
         """Where there is data in last month."""
         self.has_last_year: bool = False
         """Whether there is data in last year."""
         self.has_yesterday: bool = False
         """Whether there is data in yesterday."""
         self.available_years: list[int] = []
         """The available years."""
 
         if self.has_data:
-            today: date = date.today()
-            self.has_last_month = start < date(today.year, today.month, 1)
+            today: dt.date = dt.date.today()
+            self.has_last_month = start < dt.date(today.year, today.month, 1)
             self.has_last_year = start.year < today.year
             self.has_yesterday = start < today
             if start.year < today.year - 1:
                 self.available_years \
                     = reversed(range(start.year, today.year - 1))
 
     def year_url(self, year: int) -> str:
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/period/description.py` & `mia-accounting-1.5.1/src/accounting/report/period/description.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The period description composer.
 
 """
-from datetime import date, timedelta
+import datetime as dt
 
 from accounting.locale import gettext
 
 
-def get_desc(start: date | None, end: date | None) -> str:
+def get_desc(start: dt.date | None, end: dt.date | None) -> str:
     """Returns the period description.
 
     :param start: The start of the period.
     :param end: The end of the period.
     :return: The period description.
     """
     if start is None and end is None:
@@ -42,15 +42,15 @@
     try:
         return __get_month_desc(start, end)
     except ValueError:
         pass
     return __get_day_desc(start, end)
 
 
-def __get_since_desc(start: date) -> str:
+def __get_since_desc(start: dt.date) -> str:
     """Returns the description without the end day.
 
     :param start: The start of the period.
     :return: The description without the end day.
     """
 
     def get_start_desc() -> str:
@@ -63,36 +63,36 @@
         if start.day == 1:
             return __format_month(start)
         return __format_day(start)
 
     return gettext("since %(start)s", start=get_start_desc())
 
 
-def __get_until_desc(end: date) -> str:
+def __get_until_desc(end: dt.date) -> str:
     """Returns the description without the start day.
 
     :param end: The end of the period.
     :return: The description without the start day.
     """
 
     def get_end_desc() -> str:
         """Returns the description of the end day.
 
         :return: The description of the end day.
         """
         if end.month == 12 and end.day == 31:
             return str(end.year)
-        if (end + timedelta(days=1)).day == 1:
+        if (end + dt.timedelta(days=1)).day == 1:
             return __format_month(end)
         return __format_day(end)
 
     return gettext("until %(end)s", end=get_end_desc())
 
 
-def __get_year_desc(start: date, end: date) -> str:
+def __get_year_desc(start: dt.date, end: dt.date) -> str:
     """Returns the description as a year range.
 
     :param start: The start of the period.
     :param end: The end of the period.
     :return: The description as a year range.
     :raise ValueError: The period is not a year range.
     """
@@ -101,33 +101,33 @@
         raise ValueError
     start_text: str = str(start.year)
     if start.year == end.year:
         return __get_in_desc(start_text)
     return __get_from_to_desc(start_text, str(end.year))
 
 
-def __get_month_desc(start: date, end: date) -> str:
+def __get_month_desc(start: dt.date, end: dt.date) -> str:
     """Returns the description as a month range.
 
     :param start: The start of the period.
     :param end: The end of the period.
     :return: The description as a month range.
     :raise ValueError: The period is not a month range.
     """
-    if start.day != 1 or (end + timedelta(days=1)).day != 1:
+    if start.day != 1 or (end + dt.timedelta(days=1)).day != 1:
         raise ValueError
     start_text: str = __format_month(start)
     if start.year == end.year and start.month == end.month:
         return __get_in_desc(start_text)
     if start.year == end.year:
         return __get_from_to_desc(start_text, str(end.month))
     return __get_from_to_desc(start_text, __format_month(end))
 
 
-def __get_day_desc(start: date, end: date) -> str:
+def __get_day_desc(start: dt.date, end: dt.date) -> str:
     """Returns the description as a day range.
 
     :param start: The start of the period.
     :param end: The end of the period.
     :return: The description as a day range.
     :raise ValueError: The period is a month or year range.
     """
@@ -138,24 +138,24 @@
         return __get_from_to_desc(start_text, str(end.day))
     if start.year == end.year:
         end_month_day: str = f"{end.month}/{end.day}"
         return __get_from_to_desc(start_text, end_month_day)
     return __get_from_to_desc(start_text, __format_day(end))
 
 
-def __format_month(month: date) -> str:
+def __format_month(month: dt.date) -> str:
     """Formats a month.
 
     :param month: The month.
     :return: The formatted month.
     """
     return f"{month.year}/{month.month}"
 
 
-def __format_day(day: date) -> str:
+def __format_day(day: dt.date) -> str:
     """Formats a day.
 
     :param day: The day.
     :return: The formatted day.
     """
     return f"{day.year}/{day.month}/{day.day}"
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/period/month_end.py` & `mia-accounting-1.5.1/src/accounting/report/period/month_end.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The utility to return the end of a month.
 
 """
 import calendar
-from datetime import date
+import datetime as dt
 
 
-def month_end(day: date) -> date:
+def month_end(day: dt.date) -> dt.date:
     """Returns the end day of month for a date.
 
     :param day: The date.
     :return: The end day of the month of that day.
     """
     last_day: int = calendar.monthrange(day.year, day.month)[1]
-    return date(day.year, day.month, last_day)
+    return dt.date(day.year, day.month, last_day)
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/period/parser.py` & `mia-accounting-1.5.1/src/accounting/report/period/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The period specification parser.
 
 """
 import calendar
+import datetime as dt
 import re
-import typing as t
-from datetime import date
+from collections.abc import Callable
+from typing import Type
 
 from .period import Period
 from .shortcuts import ThisMonth, LastMonth, SinceLastMonth, ThisYear, \
     LastYear, Today, Yesterday, AllTime
 
 DATE_SPEC_RE: str = r"(\d{4})(?:-(\d{2})(?:-(\d{2}))?)?"
 """The regular expression of a date specification."""
@@ -35,15 +36,15 @@
 
     :param spec: The period specification, or omit for the default.
     :return: The period instance.
     :raise ValueError: When the period specification is invalid.
     """
     if spec is None:
         return ThisMonth()
-    named_periods: dict[str, t.Type[t.Callable[[], Period]]] = {
+    named_periods: dict[str, Type[Callable[[], Period]]] = {
         "this-month": lambda: ThisMonth(),
         "last-month": lambda: LastMonth(),
         "since-last-month": lambda: SinceLastMonth(),
         "this-year": lambda: ThisYear(),
         "last-year": lambda: LastYear(),
         "today": lambda: Today(),
         "yesterday": lambda: Yesterday(),
@@ -53,15 +54,15 @@
         return named_periods[spec]()
     start, end = __parse_spec(spec)
     if start is not None and end is not None and start > end:
         raise ValueError
     return Period(start, end)
 
 
-def __parse_spec(text: str) -> tuple[date | None, date | None]:
+def __parse_spec(text: str) -> tuple[dt.date | None, dt.date | None]:
     """Parses the period specification.
 
     :param text: The period specification.
     :return: The start and end day of the period.  The start and end day
         may be None.
     :raise ValueError: When the date is invalid.
     """
@@ -80,40 +81,40 @@
     m = re.match(f"^{DATE_SPEC_RE}-{DATE_SPEC_RE}$", text)
     if m is not None:
         return __get_start(m[1], m[2], m[3]), \
                __get_end(m[4], m[5], m[6])
     raise ValueError
 
 
-def __get_start(year: str, month: str | None, day: str | None) -> date:
+def __get_start(year: str, month: str | None, day: str | None) -> dt.date:
     """Returns the start of the period from the date representation.
 
     :param year: The year.
     :param month: The month, if any.
     :param day: The day, if any.
     :return: The start of the period.
     :raise ValueError: When the date is invalid.
     """
     if day is not None:
-        return date(int(year), int(month), int(day))
+        return dt.date(int(year), int(month), int(day))
     if month is not None:
-        return date(int(year), int(month), 1)
-    return date(int(year), 1, 1)
+        return dt.date(int(year), int(month), 1)
+    return dt.date(int(year), 1, 1)
 
 
-def __get_end(year: str, month: str | None, day: str | None) -> date:
+def __get_end(year: str, month: str | None, day: str | None) -> dt.date:
     """Returns the end of the period from the date representation.
 
     :param year: The year.
     :param month: The month, if any.
     :param day: The day, if any.
     :return: The end of the period.
     :raise ValueError: When the date is invalid.
     """
     if day is not None:
-        return date(int(year), int(month), int(day))
+        return dt.date(int(year), int(month), int(day))
     if month is not None:
         year_n: int = int(year)
         month_n: int = int(month)
         day_n: int = calendar.monthrange(year_n, month_n)[1]
-        return date(year_n, month_n, day_n)
-    return date(int(year), 12, 31)
+        return dt.date(year_n, month_n, day_n)
+    return dt.date(int(year), 12, 31)
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/period/period.py` & `mia-accounting-1.5.1/src/accounting/report/period/period.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,34 +16,34 @@
 #  limitations under the License.
 """The date period.
 
 This file is largely taken from the NanoParma ERP project, first written in
 2021/9/16 by imacat (imacat@nanoparma.com).
 
 """
-import typing as t
-from datetime import date, timedelta
+import datetime as dt
+from typing import Self
 
 from .description import get_desc
 from .month_end import month_end
 from .specification import get_spec
 
 
 class Period:
     """A date period."""
 
-    def __init__(self, start: date | None, end: date | None):
+    def __init__(self, start: dt.date | None, end: dt.date | None):
         """Constructs a new date period.
 
         :param start: The start date, or None from the very beginning.
         :param end: The end date, or None till no end.
         """
-        self.start: date | None = start
+        self.start: dt.date | None = start
         """The start of the period."""
-        self.end: date | None = end
+        self.end: dt.date | None = end
         """The end of the period."""
         self.is_default: bool = False
         """Whether the is the default period."""
         self.is_this_month: bool = False
         """Whether the period is this month."""
         self.is_last_month: bool = False
         """Whether the period is last month."""
@@ -91,16 +91,16 @@
         self.spec = get_spec(self.start, self.end)
         self.desc = get_desc(self.start, self.end)
         if self.start is None or self.end is None:
             return
         self.is_a_month = self.start.day == 1 \
             and self.end == month_end(self.start)
         self.is_type_month = self.is_a_month
-        self.is_a_year = self.start == date(self.start.year, 1, 1) \
-            and self.end == date(self.start.year, 12, 31)
+        self.is_a_year = self.start == dt.date(self.start.year, 1, 1) \
+            and self.end == dt.date(self.start.year, 12, 31)
         self.is_a_day = self.start == self.end
 
     def is_year(self, year: int) -> bool:
         """Returns whether the period is the specific year period.
 
         :param year: The year.
         :return: True if the period is the year period, or False otherwise.
@@ -115,15 +115,15 @@
 
         :return: True if this is an arbitrary period, or False otherwise.
         """
         return not self.is_type_month and not self.is_a_year \
             and not self.is_a_day
 
     @property
-    def before(self) -> t.Self | None:
+    def before(self) -> Self | None:
         """Returns the period before this period.
 
         :return: The period before this period.
         """
         if self.start is None:
             return None
-        return Period(None, self.start - timedelta(days=1))
+        return Period(None, self.start - dt.timedelta(days=1))
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/period/shortcuts.py` & `mia-accounting-1.5.1/src/accounting/report/period/shortcuts.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,123 +13,123 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The named shortcut periods.
 
 """
-from datetime import date, timedelta
+import datetime as dt
 
 from accounting.locale import gettext
 from .month_end import month_end
 from .period import Period
 
 
 class ThisMonth(Period):
     """The period of this month."""
     def __init__(self):
-        today: date = date.today()
-        this_month_start: date = date(today.year, today.month, 1)
+        today: dt.date = dt.date.today()
+        this_month_start: dt.date = dt.date(today.year, today.month, 1)
         super().__init__(this_month_start, month_end(today))
         self.is_default = True
         self.is_this_month = True
 
     def _set_properties(self) -> None:
         self.spec = "this-month"
         self.desc = gettext("This Month")
         self.is_a_month = True
         self.is_type_month = True
 
 
 class LastMonth(Period):
     """The period of this month."""
     def __init__(self):
-        today: date = date.today()
+        today: dt.date = dt.date.today()
         year: int = today.year
         month: int = today.month - 1
         if month < 1:
             year = year - 1
             month = 12
-        start: date = date(year, month, 1)
+        start: dt.date = dt.date(year, month, 1)
         super().__init__(start, month_end(start))
         self.is_last_month = True
 
     def _set_properties(self) -> None:
         self.spec = "last-month"
         self.desc = gettext("Last Month")
         self.is_a_month = True
         self.is_type_month = True
 
 
 class SinceLastMonth(Period):
     """The period of this month."""
     def __init__(self):
-        today: date = date.today()
+        today: dt.date = dt.date.today()
         year: int = today.year
         month: int = today.month - 1
         if month < 1:
             year = year - 1
             month = 12
-        start: date = date(year, month, 1)
+        start: dt.date = dt.date(year, month, 1)
         super().__init__(start, None)
         self.is_since_last_month = True
 
     def _set_properties(self) -> None:
         self.spec = "since-last-month"
         self.desc = gettext("Since Last Month")
         self.is_type_month = True
 
 
 class ThisYear(Period):
     """The period of this year."""
     def __init__(self):
-        year: int = date.today().year
-        start: date = date(year, 1, 1)
-        end: date = date(year, 12, 31)
+        year: int = dt.date.today().year
+        start: dt.date = dt.date(year, 1, 1)
+        end: dt.date = dt.date(year, 12, 31)
         super().__init__(start, end)
         self.is_this_year = True
 
     def _set_properties(self) -> None:
         self.spec = "this-year"
         self.desc = gettext("This Year")
         self.is_a_year = True
 
 
 class LastYear(Period):
     """The period of last year."""
     def __init__(self):
-        year: int = date.today().year
-        start: date = date(year - 1, 1, 1)
-        end: date = date(year - 1, 12, 31)
+        year: int = dt.date.today().year
+        start: dt.date = dt.date(year - 1, 1, 1)
+        end: dt.date = dt.date(year - 1, 12, 31)
         super().__init__(start, end)
         self.is_last_year = True
 
     def _set_properties(self) -> None:
         self.spec = "last-year"
         self.desc = gettext("Last Year")
         self.is_a_year = True
 
 
 class Today(Period):
     """The period of today."""
     def __init__(self):
-        today: date = date.today()
+        today: dt.date = dt.date.today()
         super().__init__(today, today)
         self.is_today = True
 
     def _set_properties(self) -> None:
         self.spec = "today"
         self.desc = gettext("Today")
         self.is_a_day = True
 
 
 class Yesterday(Period):
     """The period of yesterday."""
     def __init__(self):
-        yesterday: date = date.today() - timedelta(days=1)
+        yesterday: dt.date = dt.date.today() - dt.timedelta(days=1)
         super().__init__(yesterday, yesterday)
         self.is_yesterday = True
 
     def _set_properties(self) -> None:
         self.spec = "yesterday"
         self.desc = gettext("Yesterday")
         self.is_a_day = True
@@ -159,10 +159,10 @@
     """A year period."""
 
     def __init__(self, year: int):
         """Constructs a year period.
 
         :param year: The year.
         """
-        start: date = date(year, 1, 1)
-        end: date = date(year, 12, 31)
+        start: dt.date = dt.date(year, 1, 1)
+        end: dt.date = dt.date(year, 12, 31)
         super().__init__(start, end)
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/period/specification.py` & `mia-accounting-1.5.1/src/accounting/report/period/specification.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The period specification composer.
 
 """
-from datetime import date, timedelta
+import datetime as dt
 
 
-def get_spec(start: date | None, end: date | None) -> str:
+def get_spec(start: dt.date | None, end: dt.date | None) -> str:
     """Returns the period specification.
 
     :param start: The start of the period.
     :param end: The end of the period.
     :return: The period specification.
     """
     if start is None and end is None:
@@ -40,41 +40,41 @@
     try:
         return __get_month_spec(start, end)
     except ValueError:
         pass
     return __get_day_spec(start, end)
 
 
-def __get_since_spec(start: date) -> str:
+def __get_since_spec(start: dt.date) -> str:
     """Returns the period specification without the end day.
 
     :param start: The start of the period.
     :return: The period specification without the end day
     """
     if start.month == 1 and start.day == 1:
         return start.strftime("%Y-")
     if start.day == 1:
         return start.strftime("%Y-%m-")
     return start.strftime("%Y-%m-%d-")
 
 
-def __get_until_spec(end: date) -> str:
+def __get_until_spec(end: dt.date) -> str:
     """Returns the period specification without the start day.
 
     :param end: The end of the period.
     :return: The period specification without the start day
     """
     if end.month == 12 and end.day == 31:
         return end.strftime("-%Y")
-    if (end + timedelta(days=1)).day == 1:
+    if (end + dt.timedelta(days=1)).day == 1:
         return end.strftime("-%Y-%m")
     return end.strftime("-%Y-%m-%d")
 
 
-def __get_year_spec(start: date, end: date) -> str:
+def __get_year_spec(start: dt.date, end: dt.date) -> str:
     """Returns the period specification as a year range.
 
     :param start: The start of the period.
     :param end: The end of the period.
     :return: The period specification as a year range.
     :raise ValueError: The period is not a year range.
     """
@@ -84,32 +84,32 @@
     start_spec: str = start.strftime("%Y")
     if start.year == end.year:
         return start_spec
     end_spec: str = end.strftime("%Y")
     return f"{start_spec}-{end_spec}"
 
 
-def __get_month_spec(start: date, end: date) -> str:
+def __get_month_spec(start: dt.date, end: dt.date) -> str:
     """Returns the period specification as a month range.
 
     :param start: The start of the period.
     :param end: The end of the period.
     :return: The period specification as a month range.
     :raise ValueError: The period is not a month range.
     """
-    if start.day != 1 or (end + timedelta(days=1)).day != 1:
+    if start.day != 1 or (end + dt.timedelta(days=1)).day != 1:
         raise ValueError
     start_spec: str = start.strftime("%Y-%m")
     if start.year == end.year and start.month == end.month:
         return start_spec
     end_spec: str = end.strftime("%Y-%m")
     return f"{start_spec}-{end_spec}"
 
 
-def __get_day_spec(start: date, end: date) -> str:
+def __get_day_spec(start: dt.date, end: dt.date) -> str:
     """Returns the period specification as a day range.
 
     :param start: The start of the period.
     :param end: The end of the period.
     :return: The period specification as a day range.
     :raise ValueError: The period is a month or year range.
     """
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/reports/__init__.py` & `mia-accounting-1.5.1/src/accounting/report/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/reports/balance_sheet.py` & `mia-accounting-1.5.1/src/accounting/report/reports/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/reports/income_expenses.py` & `mia-accounting-1.5.1/src/accounting/report/reports/income_expenses.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The income and expenses log.
 
 """
-from datetime import date
+import datetime as dt
 from decimal import Decimal
 
 import sqlalchemy as sa
 from flask import url_for, render_template, Response
 from sqlalchemy.orm import selectinload
 
 from accounting import db
@@ -49,15 +49,15 @@
 
         :param line_item: The journal entry line item.
         """
         self.is_brought_forward: bool = False
         """Whether this is the brought-forward line item."""
         self.is_total: bool = False
         """Whether this is the total line item."""
-        self.date: date | None = None
+        self.date: dt.date | None = None
         """The date."""
         self.account: Account | None = None
         """The account."""
         self.description: str | None = None
         """The description."""
         self.income: Decimal | None = None
         """The income amount."""
@@ -209,32 +209,32 @@
                 balance = balance - line_item.expense
             line_item.balance = balance
 
 
 class CSVRow(BaseCSVRow):
     """A row in the CSV."""
 
-    def __init__(self, journal_entry_date: date | str | None,
+    def __init__(self, date: dt.date | str | None,
                  account: str | None,
                  description: str | None,
                  income: str | Decimal | None,
                  expense: str | Decimal | None,
                  balance: str | Decimal | None,
                  note: str | None):
         """Constructs a row in the CSV.
 
-        :param journal_entry_date: The journal entry date.
+        :param date: The journal entry date.
         :param account: The account.
         :param description: The description.
         :param income: The income.
         :param expense: The expense.
         :param balance: The balance.
         :param note: The note.
         """
-        self.date: date | str | None = journal_entry_date
+        self.date: dt.date | str | None = date
         """The date."""
         self.account: str | None = account
         """The account."""
         self.description: str | None = description
         """The description."""
         self.income: str | Decimal | None = income
         """The income."""
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/reports/income_statement.py` & `mia-accounting-1.5.1/src/accounting/report/reports/income_statement.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/reports/journal.py` & `mia-accounting-1.5.1/src/accounting/report/reports/journal.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The journal.
 
 """
-from datetime import date
+import datetime as dt
 from decimal import Decimal
 
 import sqlalchemy as sa
 from flask import render_template, Response
 from sqlalchemy.orm import selectinload
 
 from accounting.locale import gettext
@@ -63,15 +63,15 @@
         self.amount: Decimal = line_item.amount
         """The amount."""
 
 
 class CSVRow(BaseCSVRow):
     """A row in the CSV."""
 
-    def __init__(self, journal_entry_date: str | date,
+    def __init__(self, journal_entry_date: str | dt.date,
                  currency: str,
                  account: str,
                  description: str | None,
                  debit: str | Decimal | None,
                  credit: str | Decimal | None,
                  note: str | None):
         """Constructs a row in the CSV.
@@ -80,15 +80,15 @@
         :param currency: The currency.
         :param account: The account.
         :param description: The description.
         :param debit: The debit amount.
         :param credit: The credit amount.
         :param note: The note.
         """
-        self.date: str | date = journal_entry_date
+        self.date: str | dt.date = journal_entry_date
         """The date."""
         self.currency: str = currency
         """The currency."""
         self.account: str = account
         """The account."""
         self.description: str | None = description
         """The description."""
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/reports/ledger.py` & `mia-accounting-1.5.1/src/accounting/report/reports/ledger.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The ledger.
 
 """
-from datetime import date
+import datetime as dt
 from decimal import Decimal
 
 import sqlalchemy as sa
 from flask import url_for, render_template, Response
 from sqlalchemy.orm import selectinload
 
 from accounting import db
@@ -48,15 +48,15 @@
 
         :param line_item: The journal entry line item.
         """
         self.is_brought_forward: bool = False
         """Whether this is the brought-forward line item."""
         self.is_total: bool = False
         """Whether this is the total line item."""
-        self.date: date | None = None
+        self.date: dt.date | None = None
         """The date."""
         self.description: str | None = None
         """The description."""
         self.debit: Decimal | None = None
         """The debit amount."""
         self.credit: Decimal | None = None
         """The credit amount."""
@@ -192,30 +192,30 @@
                 balance = balance - line_item.credit
             line_item.balance = balance
 
 
 class CSVRow(BaseCSVRow):
     """A row in the CSV."""
 
-    def __init__(self, journal_entry_date: date | str | None,
+    def __init__(self, date: dt.date | str | None,
                  description: str | None,
                  debit: str | Decimal | None,
                  credit: str | Decimal | None,
                  balance: str | Decimal | None,
                  note: str | None):
         """Constructs a row in the CSV.
 
-        :param journal_entry_date: The journal entry date.
+        :param date: The journal entry date.
         :param description: The description.
         :param debit: The debit amount.
         :param credit: The credit amount.
         :param balance: The balance.
         :param note: The note.
         """
-        self.date: date | str | None = journal_entry_date
+        self.date: dt.date | str | None = date
         """The date."""
         self.description: str | None = description
         """The description."""
         self.debit: str | Decimal | None = debit
         """The debit amount."""
         self.credit: str | Decimal | None = credit
         """The credit amount."""
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/reports/search.py` & `mia-accounting-1.5.1/src/accounting/report/reports/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The search.
 
 """
-from datetime import datetime
+import datetime as dt
 from decimal import Decimal
 
 import sqlalchemy as sa
 from flask import Response, render_template, request
 from sqlalchemy.orm import selectinload
 
 from accounting.locale import gettext
@@ -120,48 +120,41 @@
         """Composes and returns the condition to filter the journal entry.
 
         :param k: The keyword.
         :return: The condition to filter the journal entry.
         """
         conditions: list[sa.BinaryExpression] \
             = [JournalEntry.note.icontains(k)]
-        journal_entry_date: datetime
+        date: dt.datetime
         try:
-            journal_entry_date = datetime.strptime(k, "%Y")
-            conditions.append(sa.extract("year", JournalEntry.date)
-                              == journal_entry_date.year)
+            date = dt.datetime.strptime(k, "%Y")
+            conditions.append(
+                sa.extract("year", JournalEntry.date) == date.year)
         except ValueError:
             pass
         try:
-            journal_entry_date = datetime.strptime(k, "%Y/%m")
+            date = dt.datetime.strptime(k, "%Y/%m")
             conditions.append(sa.and_(
-                sa.extract("year", JournalEntry.date)
-                == journal_entry_date.year,
-                sa.extract("month", JournalEntry.date)
-                == journal_entry_date.month))
+                sa.extract("year", JournalEntry.date) == date.year,
+                sa.extract("month", JournalEntry.date) == date.month))
         except ValueError:
             pass
         try:
-            journal_entry_date = datetime.strptime(f"2000/{k}", "%Y/%m/%d")
+            date = dt.datetime.strptime(f"2000/{k}", "%Y/%m/%d")
             conditions.append(sa.and_(
-                sa.extract("month", JournalEntry.date)
-                == journal_entry_date.month,
-                sa.extract("day", JournalEntry.date)
-                == journal_entry_date.day))
+                sa.extract("month", JournalEntry.date) == date.month,
+                sa.extract("day", JournalEntry.date) == date.day))
         except ValueError:
             pass
         try:
-            journal_entry_date = datetime.strptime(k, "%Y/%m/%d")
+            date = dt.datetime.strptime(k, "%Y/%m/%d")
             conditions.append(sa.and_(
-                sa.extract("year", JournalEntry.date)
-                == journal_entry_date.year,
-                sa.extract("month", JournalEntry.date)
-                == journal_entry_date.month,
-                sa.extract("day", JournalEntry.date)
-                == journal_entry_date.day))
+                sa.extract("year", JournalEntry.date) == date.year,
+                sa.extract("month", JournalEntry.date) == date.month,
+                sa.extract("day", JournalEntry.date) == date.day))
         except ValueError:
             pass
         return sa.select(JournalEntry.id).filter(sa.or_(*conditions))
 
 
 class PageParams(BasePageParams):
     """The HTML page parameters."""
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/reports/trial_balance.py` & `mia-accounting-1.5.1/src/accounting/report/reports/trial_balance.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/reports/unapplied.py` & `mia-accounting-1.5.1/src/accounting/report/reports/unapplied.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The unapplied original line items.
 
 """
-from datetime import date
+import datetime as dt
 from decimal import Decimal
 
 from flask import render_template, Response
 from sqlalchemy.orm import selectinload
 
 from accounting.locale import gettext
 from accounting.models import Currency, Account, JournalEntry, \
@@ -37,38 +37,38 @@
 from accounting.report.utils.urls import unapplied_url
 from accounting.utils.pagination import Pagination
 
 
 class CSVRow(BaseCSVRow):
     """A row in the CSV."""
 
-    def __init__(self, journal_entry_date: str | date, currency: str,
+    def __init__(self, journal_entry_date: str | dt.date, currency: str,
                  description: str | None, amount: str | Decimal,
                  net_balance: str | Decimal):
         """Constructs a row in the CSV.
 
         :param journal_entry_date: The journal entry date.
         :param currency: The currency.
         :param description: The description.
         :param amount: The amount.
         :param net_balance: The net balance.
         """
-        self.date: str | date = journal_entry_date
+        self.date: str | dt.date = journal_entry_date
         """The date."""
         self.currency: str = currency
         """The currency."""
         self.description: str | None = description
         """The description."""
         self.amount: str | Decimal = amount
         """The amount."""
         self.net_balance: str | Decimal = net_balance
         """The net balance."""
 
     @property
-    def values(self) -> list[str | date | Decimal | None]:
+    def values(self) -> list[str | dt.date | Decimal | None]:
         """Returns the values of the row.
 
         :return: The values of the row.
         """
         return [self.date, self.currency, self.description, self.amount,
                 self.net_balance]
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/reports/unapplied_accounts.py` & `mia-accounting-1.5.1/src/accounting/report/reports/unapplied_accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The accounts with unapplied original line items.
 
 """
-from datetime import date
+import datetime as dt
 from decimal import Decimal
 
 from flask import render_template, Response
 
 from accounting.locale import gettext
 from accounting.models import Currency, Account
 from accounting.report.utils.base_page_params import BasePageParams
@@ -45,15 +45,15 @@
         """
         self.account: str = account
         """The currency."""
         self.count: int | str = count
         """The number of unapplied original line items."""
 
     @property
-    def values(self) -> list[str | date | Decimal | None]:
+    def values(self) -> list[str | dt.date | Decimal | None]:
         """Returns the values of the row.
 
         :return: The values of the row.
         """
         return [self.account, self.count]
 
 
@@ -139,15 +139,15 @@
         """The accounts."""
 
     def csv(self) -> Response:
         """Returns the report as CSV for download.
 
         :return: The response of the report for download.
         """
-        filename: str = f"unapplied-accounts.csv"
+        filename: str = "unapplied-accounts.csv"
         return csv_download(filename, get_csv_rows(self.__accounts))
 
     def html(self) -> str:
         """Composes and returns the report as HTML.
 
         :return: The report as HTML.
         """
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/reports/unmatched.py` & `mia-accounting-1.5.1/src/accounting/report/reports/unmatched.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The unmatched offsets.
 
 """
-from datetime import date
+import datetime as dt
 from decimal import Decimal
 
 from flask import render_template, Response
 from flask_babel import LazyString
 
 from accounting.locale import gettext
 from accounting.models import Currency, Account, JournalEntryLineItem
@@ -36,41 +36,41 @@
 from accounting.report.utils.urls import unmatched_url
 from accounting.utils.pagination import Pagination
 
 
 class CSVRow(BaseCSVRow):
     """A row in the CSV."""
 
-    def __init__(self, journal_entry_date: str | date, currency: str,
+    def __init__(self, journal_entry_date: str | dt.date, currency: str,
                  description: str | None, debit: str | Decimal,
                  credit: str | Decimal, balance: str | Decimal):
         """Constructs a row in the CSV.
 
         :param journal_entry_date: The journal entry date.
         :param currency: The currency.
         :param description: The description.
         :param debit: The debit amount.
         :param credit: The credit amount.
         :param balance: The balance.
         """
-        self.date: str | date = journal_entry_date
+        self.date: str | dt.date = journal_entry_date
         """The date."""
         self.currency: str = currency
         """The currency."""
         self.description: str | None = description
         """The description."""
         self.debit: str | Decimal | None = debit
         """The debit amount."""
         self.credit: str | Decimal | None = credit
         """The credit amount."""
         self.balance: str | Decimal = balance
         """The balance."""
 
     @property
-    def values(self) -> list[str | date | Decimal | None]:
+    def values(self) -> list[str | dt.date | Decimal | None]:
         """Returns the values of the row.
 
         :return: The values of the row.
         """
         return [self.date, self.currency, self.description, self.debit,
                 self.credit, self.balance]
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/reports/unmatched_accounts.py` & `mia-accounting-1.5.1/src/accounting/report/reports/unmatched_accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The accounts with unmatched offsets.
 
 """
-from datetime import date
+import datetime as dt
 from decimal import Decimal
 
 from flask import render_template, Response
 
 from accounting.locale import gettext
 from accounting.models import Currency, Account
 from accounting.report.utils.base_page_params import BasePageParams
@@ -45,15 +45,15 @@
         """
         self.account: str = account
         """The currency."""
         self.count: int | str = count
         """The number of unapplied original line items."""
 
     @property
-    def values(self) -> list[str | date | Decimal | None]:
+    def values(self) -> list[str | dt.date | Decimal | None]:
         """Returns the values of the row.
 
         :return: The values of the row.
         """
         return [self.account, self.count]
 
 
@@ -140,15 +140,15 @@
         """The accounts."""
 
     def csv(self) -> Response:
         """Returns the report as CSV for download.
 
         :return: The response of the report for download.
         """
-        filename: str = f"unapplied-accounts.csv"
+        filename: str = "unmatched-accounts.csv"
         return csv_download(filename, get_csv_rows(self.__accounts))
 
     def html(self) -> str:
         """Composes and returns the report as HTML.
 
         :return: The report as HTML.
         """
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/template_filters.py` & `mia-accounting-1.5.1/src/accounting/report/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/utils/__init__.py` & `mia-accounting-1.5.1/src/accounting/report/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/utils/base_page_params.py` & `mia-accounting-1.5.1/src/accounting/report/utils/base_page_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The page parameters of a report.
 
 """
-import typing as t
 from abc import ABC, abstractmethod
+from collections.abc import Callable
+from typing import Type
 from urllib.parse import urlparse, ParseResult, parse_qsl, urlencode, \
     urlunparse
 
 import sqlalchemy as sa
 from flask import request
 
 from accounting import db
@@ -48,15 +49,15 @@
     def report_chooser(self) -> ReportChooser:
         """Returns the report chooser.
 
         :return: The report chooser.
         """
 
     @property
-    def journal_entry_types(self) -> t.Type[JournalEntryType]:
+    def journal_entry_types(self) -> Type[JournalEntryType]:
         """Returns the journal entry types.
 
         :return: The journal entry types.
         """
         return JournalEntryType
 
     @property
@@ -68,15 +69,15 @@
         params = [x for x in params if x[0] != "as"]
         params.append(("as", "csv"))
         parts: list[str] = list(uri_p)
         parts[4] = urlencode(params)
         return urlunparse(parts)
 
     @staticmethod
-    def _get_currency_options(get_url: t.Callable[[Currency], str],
+    def _get_currency_options(get_url: Callable[[Currency], str],
                               active_currency: Currency) -> list[OptionLink]:
         """Returns the currency options.
 
         :param get_url: The callback to return the URL of a currency.
         :param active_currency: The active currency.
         :return: The currency options.
         """
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/utils/base_report.py` & `mia-accounting-1.5.1/src/accounting/report/utils/base_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/utils/csv_export.py` & `mia-accounting-1.5.1/src/accounting/report/utils/csv_export.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The utilities to export the report as CSV for download.
 
 """
 import csv
+import datetime as dt
 from abc import ABC, abstractmethod
-from datetime import timedelta, date
 from decimal import Decimal
 from io import StringIO
 from urllib.parse import quote
 
 from flask import Response
 
 from accounting.report.period import Period
@@ -73,15 +73,15 @@
     if period.start is None:
         return f"until-{end}"
     if period.end is None:
         return f"since-{start}"
     return f"{start}-{end}"
 
 
-def __get_start_str(start: date | None) -> str | None:
+def __get_start_str(start: dt.date | None) -> str | None:
     """Returns the string representation of the start date.
 
     :param start: The start date.
     :return: The string representation of the start date, or None if the start
         date is None.
     """
     if start is None:
@@ -89,21 +89,21 @@
     if start.month == 1 and start.day == 1:
         return str(start.year)
     if start.day == 1:
         return start.strftime("%Y%m")
     return start.strftime("%Y%m%d")
 
 
-def __get_end_str(end: date | None) -> str | None:
+def __get_end_str(end: dt.date | None) -> str | None:
     """Returns the string representation of the end date.
 
     :param end: The end date.
     :return: The string representation of the end date, or None if the end
         date is None.
     """
     if end is None:
         return None
     if end.month == 12 and end.day == 31:
         return str(end.year)
-    if (end + timedelta(days=1)).day == 1:
+    if (end + dt.timedelta(days=1)).day == 1:
         return end.strftime("%Y%m")
     return end.strftime("%Y%m%d")
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/utils/offset_matcher.py` & `mia-accounting-1.5.1/src/accounting/report/utils/offset_matcher.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/utils/option_link.py` & `mia-accounting-1.5.1/src/accounting/report/utils/option_link.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/utils/report_chooser.py` & `mia-accounting-1.5.1/src/accounting/report/utils/report_chooser.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """The report chooser.
 
 This file is largely taken from the NanoParma ERP project, first written in
 2021/9/16 by imacat (imacat@nanoparma.com).
 
 """
 import re
-import typing as t
+from collections.abc import Iterator
 
 from flask_babel import LazyString
 
 from accounting import db
 from accounting.locale import gettext
 from accounting.models import Currency, Account
 from accounting.report.period import Period, get_period
@@ -186,13 +186,13 @@
                               self.__active_report == ReportType.UNMATCHED,
                               fa_icon="fa-solid fa-file-circle-question")
         return OptionLink(gettext("Unmatched Offsets"),
                           unmatched_url(self.__currency, self.__account),
                           self.__active_report == ReportType.UNMATCHED,
                           fa_icon="fa-solid fa-file-circle-question")
 
-    def __iter__(self) -> t.Iterator[OptionLink]:
+    def __iter__(self) -> Iterator[OptionLink]:
         """Returns the iteration of the reports.
 
         :return: The iteration of the reports.
         """
         return iter(self.__reports)
```

### Comparing `mia-accounting-1.5.0/src/accounting/report/utils/report_type.py` & `mia-accounting-1.5.1/src/accounting/report/utils/report_type.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/utils/unapplied.py` & `mia-accounting-1.5.1/src/accounting/report/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/utils/unmatched.py` & `mia-accounting-1.5.1/src/accounting/report/utils/unmatched.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/utils/urls.py` & `mia-accounting-1.5.1/src/accounting/report/utils/urls.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/report/views.py` & `mia-accounting-1.5.1/src/accounting/report/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/static/css/style.css` & `mia-accounting-1.5.1/src/accounting/static/css/style.css`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/static/js/account-form.js` & `mia-accounting-1.5.1/src/accounting/static/js/account-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/static/js/account-order.js` & `mia-accounting-1.5.1/src/accounting/static/js/account-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/static/js/currency-form.js` & `mia-accounting-1.5.1/src/accounting/static/js/currency-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/static/js/description-editor.js` & `mia-accounting-1.5.1/src/accounting/static/js/description-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/static/js/drag-and-drop-reorder.js` & `mia-accounting-1.5.1/src/accounting/static/js/drag-and-drop-reorder.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/static/js/journal-entry-account-selector.js` & `mia-accounting-1.5.1/src/accounting/static/js/journal-entry-account-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/static/js/journal-entry-form.js` & `mia-accounting-1.5.1/src/accounting/static/js/journal-entry-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/static/js/journal-entry-line-item-editor.js` & `mia-accounting-1.5.1/src/accounting/static/js/journal-entry-line-item-editor.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -272,15 +272,14 @@
     saveOriginalLineItem(originalLineItem) {
         this.#originalLineItemContainer.classList.remove("d-none");
         this.#originalLineItemControl.classList.add("accounting-not-empty");
         this.originalLineItemId = originalLineItem.id;
         this.originalLineItemDate = originalLineItem.date;
         this.originalLineItemText = originalLineItem.text;
         this.#originalLineItemText.innerText = originalLineItem.text;
-        this.#setEnableDescriptionAccount(false);
         if (this.description === null) {
             if (originalLineItem.description === "") {
                 this.#descriptionControl.classList.remove("accounting-not-empty");
             } else {
                 this.#descriptionControl.classList.add("accounting-not-empty");
             }
             this.description = originalLineItem.description === "" ? null : originalLineItem.description;
```

### Comparing `mia-accounting-1.5.0/src/accounting/static/js/journal-entry-order.js` & `mia-accounting-1.5.1/src/accounting/static/js/journal-entry-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/static/js/material-fab-speed-dial.js` & `mia-accounting-1.5.1/src/accounting/static/js/material-fab-speed-dial.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/static/js/option-form.js` & `mia-accounting-1.5.1/src/accounting/static/js/option-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/static/js/original-line-item-selector.js` & `mia-accounting-1.5.1/src/accounting/static/js/original-line-item-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/static/js/period-chooser.js` & `mia-accounting-1.5.1/src/accounting/static/js/period-chooser.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/template_filters.py` & `mia-accounting-1.5.1/src/accounting/template_filters.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The template filters.
 
 """
-import typing as t
-from datetime import date, timedelta
+import datetime as dt
 from decimal import Decimal
+from typing import Any
 
 from flask_babel import get_locale
 
 from accounting.locale import gettext
 
 
 def format_amount(value: Decimal | None) -> str | None:
@@ -37,45 +37,45 @@
     if value == 0:
         return "-"
     whole: int = int(value)
     frac: Decimal = (value - whole).normalize()
     return "{:,}".format(whole) + str(abs(frac))[1:]
 
 
-def format_date(value: date) -> str:
+def format_date(value: dt.date) -> str:
     """Formats a date to be human-friendly.
 
     :param value: The date.
     :return: The human-friendly date text.
     """
-    today: date = date.today()
+    today: dt.date = dt.date.today()
     if value == today:
         return gettext("Today")
-    if value == today - timedelta(days=1):
+    if value == today - dt.timedelta(days=1):
         return gettext("Yesterday")
-    if value == today + timedelta(days=1):
+    if value == today + dt.timedelta(days=1):
         return gettext("Tomorrow")
     locale = str(get_locale())
     if locale == "zh" or locale.startswith("zh_"):
-        if value == today - timedelta(days=2):
+        if value == today - dt.timedelta(days=2):
             return gettext("The day before yesterday")
-        if value == today + timedelta(days=2):
+        if value == today + dt.timedelta(days=2):
             return gettext("The day after tomorrow")
     if locale == "zh" or locale.startswith("zh_"):
         weekdays = ["一", "二", "三", "四", "五", "六", "日"]
         weekday = weekdays[value.weekday()]
     else:
         weekday = value.strftime("%a")
     if value.year != today.year:
         return "{}/{}/{}({})".format(
             value.year, value.month, value.day, weekday)
     return "{}/{}({})".format(value.month, value.day, weekday)
 
 
-def default(value: t.Any, default_value: t.Any = "") -> t.Any:
+def default(value: Any, default_value: Any = "") -> Any:
     """Returns the default value if the given value is None.
 
     :param value: The value.
     :param default_value: The default value when the given value is None.
     :return: The value, or the default value if the given value is None.
     """
     return default_value if value is None else value
```

### Comparing `mia-accounting-1.5.0/src/accounting/template_globals.py` & `mia-accounting-1.5.1/src/accounting/template_globals.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/account/create.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/account/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/account/detail.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/account/edit.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/account/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/account/include/form.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/account/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/account/list.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/account/order.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/account/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/base-account/detail.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/base-account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/base-account/list.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/base-account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/base.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/currency/create.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/currency/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/currency/detail.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/currency/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/currency/edit.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/currency/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/currency/include/form.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/currency/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/currency/list.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/currency/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/include/nav.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/include/nav.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/include/pagination.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/include/pagination.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/disbursement/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/disbursement/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/disbursement/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/detail.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/detail.html`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   </a>
   {% if accounting_can_edit() %}
     <a class="btn btn-primary d-none d-md-inline" role="button" href="{{ url_for("accounting.journal-entry.edit", journal_entry=obj)|accounting_inherit_next }}">
       <i class="fa-solid fa-pen-to-square"></i>
       {{ A_("Edit") }}
     </a>
   {% endif %}
-  <a class="btn btn-primary" role="button" href="{{ url_for("accounting.journal-entry.order", journal_entry_date=obj.date)|accounting_append_next }}">
+  <a class="btn btn-primary" role="button" href="{{ url_for("accounting.journal-entry.order", date=obj.date)|accounting_append_next }}">
     <i class="fa-solid fa-bars-staggered"></i>
     <span class="d-none d-md-inline">{{ A_("Order") }}</span>
   </a>
   {% if accounting_can_edit() %}
     {% block as_trasfer %}{% endblock %}
     {% if obj.can_delete %}
       <button class="btn btn-danger" type="button" data-bs-toggle="modal" data-bs-target="#accounting-delete-modal">
```

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/form-line-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/form.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/order.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/order.html`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   <a class="btn btn-primary" role="button" href="{{ url_for("accounting-report.default")|accounting_or_next }}">
     <i class="fa-solid fa-circle-chevron-left"></i>
     <span class="d-none d-md-inline">{{ A_("Back") }}</span>
   </a>
 </div>
 
 {% if list|length > 1 and accounting_can_edit() %}
-  <form action="{{ url_for("accounting.journal-entry.sort", journal_entry_date=date) }}" method="post">
+  <form action="{{ url_for("accounting.journal-entry.sort", date=date) }}" method="post">
     <input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
     {% if request.args.next %}
       <input type="hidden" name="next" value="{{ request.args.next }}">
     {% endif %}
     <ul id="accounting-order-list" class="list-group mb-3">
       {% for item in list %}
         <li class="list-group-item d-flex justify-content-between" data-id="{{ item.id }}">
```

#### html2text {}

```diff
@@ -12,16 +12,16 @@
 static", filename="js/drag-and-drop-reorder.js") }}">
 static", filename="js/journal-entry-order.js") }}">
 {% endblock %} {% block header %}{% block title %}{{ A_("Journal Entries on %
 (date)s", date=date|accounting_format_date) }}{% endblock %}{% endblock %} {%
 block content %}
 default")|accounting_or_next }}">  {{ A_("Back") }}
 {% if list|length > 1 and accounting_can_edit() %}
-journal-entry.sort", journal_entry_date=date) }}" method="post">  {% if
-request.args.next %}  {% endif %}
+journal-entry.sort", date=date) }}" method="post">  {% if request.args.next %}
+{% endif %}
     * {% for item in list %}
     *  {% with journal_entry = item %} {% include "accounting/journal-entry/
       include/order-journal-entry.html" %} {% endwith %}
     * {% endfor %}
   {{ A_("Save") }}
 
 {% elif list %}
```

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/create.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/receipt/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/receipt/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/receipt/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/receipt/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/create.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/transfer/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/transfer/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/transfer/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/journal-entry/transfer/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/option/detail.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/option/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/option/form.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/option/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/form-recurring-item.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/option/include/form-recurring-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/balance-sheet.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/balance-sheet.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/balance-sheet-section.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/ledger-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/ledger-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/period-chooser.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/period-chooser.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/search-modal.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/search-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/include/toolbar-buttons.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/income-expenses.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/income-expenses.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/income-statement.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/income-statement.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/journal.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/journal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/ledger.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/ledger.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/search.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/search.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/trial-balance.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/trial-balance.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/unapplied-accounts.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/unapplied-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/unapplied.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/unapplied.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/unmatched-accounts.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/unmatched-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/templates/accounting/report/unmatched.html` & `mia-accounting-1.5.1/src/accounting/templates/accounting/report/unmatched.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/translations/accounting.pot` & `mia-accounting-1.5.1/src/accounting/translations/accounting.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo` & `mia-accounting-1.5.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po` & `mia-accounting-1.5.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo` & `mia-accounting-1.5.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po` & `mia-accounting-1.5.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/utils/__init__.py` & `mia-accounting-1.5.1/src/accounting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/utils/cast.py` & `mia-accounting-1.5.1/src/accounting/utils/cast.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 #  limitations under the License.
 """The utility to cast a SQLAlchemy column into the column type, to avoid
 warnings from the IDE.
 
 This module should not import any other module from the application.
 
 """
-import typing as t
+from typing import Any
 
-import sqlalchemy as sa
 
-
-def s(message: t.Any) -> str:
+def s(message: Any) -> str:
     """Casts the LazyString message to the string type.
 
     :param message: The message.
     :return: The binary expression itself.
     """
     return message
```

### Comparing `mia-accounting-1.5.0/src/accounting/utils/current_account.py` & `mia-accounting-1.5.1/src/accounting/utils/current_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The current assets and liabilities account.
 
 """
-import typing as t
+from typing import Self
+
+import sqlalchemy as sa
 
 from accounting import db
 from accounting.locale import gettext
 from accounting.models import Account
-import sqlalchemy as sa
 
 
 class CurrentAccount:
     """A current assets and liabilities account."""
     CURRENT_AL_CODE: str = "0000-000"
     """The account code for all current assets and liabilities."""
 
@@ -50,28 +51,28 @@
         """Returns the string representation of the account.
 
         :return: The string representation of the account.
         """
         return self.str
 
     @classmethod
-    def current_assets_and_liabilities(cls) -> t.Self:
+    def current_assets_and_liabilities(cls) -> Self:
         """Returns the pseudo account for all current assets and liabilities.
 
         :return: The pseudo account for all current assets and liabilities.
         """
         account: cls = cls()
         account.id = 0
         account.code = cls.CURRENT_AL_CODE
         account.title = gettext("current assets and liabilities")
         account.str = account.title
         return account
 
     @classmethod
-    def accounts(cls) -> list[t.Self]:
+    def accounts(cls) -> list[Self]:
         """Returns the current assets and liabilities accounts.
 
         :return: The current assets and liabilities accounts.
         """
         accounts: list[cls] = [cls.current_assets_and_liabilities()]
         accounts.extend([CurrentAccount(x)
                          for x in db.session.query(Account)
```

### Comparing `mia-accounting-1.5.0/src/accounting/utils/flash_errors.py` & `mia-accounting-1.5.1/src/accounting/utils/flash_errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The utility to flash all errors from the forms.
 
 This module should not import any other module from the application.
 
 """
-import typing as t
+from typing import Any
 
 from flask import flash
 from flask_wtf import FlaskForm
 
 
 def flash_form_errors(form: FlaskForm) -> None:
     """Flash all errors from a form recursively.
 
     :param form: The form.
     :return: None.
     """
     __flash_errors(form.errors)
 
 
-def __flash_errors(error: t.Any) -> None:
+def __flash_errors(error: Any) -> None:
     """Flash all errors recursively.
 
     :param error: The errors.
     :return: None.
     """
     if isinstance(error, dict):
         for key in error:
```

### Comparing `mia-accounting-1.5.0/src/accounting/utils/journal_entry_types.py` & `mia-accounting-1.5.1/src/accounting/utils/journal_entry_types.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/utils/next_uri.py` & `mia-accounting-1.5.1/src/accounting/utils/next_uri.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/utils/offset_alias.py` & `mia-accounting-1.5.1/src/accounting/utils/offset_alias.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The SQLAlchemy alias for the offset items.
 
 """
-import typing as t
+from typing import Any
 
 import sqlalchemy as sa
 
 from accounting.models import JournalEntryLineItem
 
 
 def offset_alias() -> sa.Alias:
     """Returns the SQLAlchemy alias for the offset items.
 
     :return: The SQLAlchemy alias for the offset items.
     """
 
-    def as_from(model_cls: t.Any) -> sa.FromClause:
+    def as_from(model_cls: Any) -> sa.FromClause:
         return model_cls
 
-    def as_alias(alias: t.Any) -> sa.Alias:
+    def as_alias(alias: Any) -> sa.Alias:
         return alias
 
     return as_alias(sa.alias(as_from(JournalEntryLineItem), name="offset"))
```

### Comparing `mia-accounting-1.5.0/src/accounting/utils/options.py` & `mia-accounting-1.5.1/src/accounting/utils/options.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/utils/pagination.py` & `mia-accounting-1.5.1/src/accounting/utils/pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The pagination utilities.
 
 This module should not import any other module from the application.
 
 """
-import typing as t
+from typing import TypeVar, Generic
 from urllib.parse import urlparse, parse_qsl, urlencode, urlunparse, \
     ParseResult
 
 from flask import request
 from werkzeug.routing import RequestRedirect
 
 from accounting.locale import pgettext
@@ -58,18 +58,18 @@
     code = 302
     """The HTTP code."""
 
 
 DEFAULT_PAGE_SIZE: int = 10
 """The default page size."""
 
-T = t.TypeVar("T")
+T = TypeVar("T")
 
 
-class Pagination(t.Generic[T]):
+class Pagination(Generic[T]):
     """The pagination utility."""
 
     def __init__(self, items: list[T], is_reversed: bool = False):
         """Constructs the pagination.
 
         :param items: The items.
         :param is_reversed: True if the default page is the last page, or False
@@ -87,15 +87,15 @@
         """The pages."""
         self.page_size: int = pagination.page_size
         """The number of items in a page."""
         self.page_size_options: list[Link] = pagination.page_size_options
         """The options to the number of items in a page."""
 
 
-class AbstractPagination(t.Generic[T]):
+class AbstractPagination(Generic[T]):
     """An abstract pagination."""
 
     def __init__(self):
         """Constructs an empty pagination."""
         self.page_size: int = DEFAULT_PAGE_SIZE
         """The number of items in a page."""
         self.is_paged: bool = False
```

### Comparing `mia-accounting-1.5.0/src/accounting/utils/permission.py` & `mia-accounting-1.5.1/src/accounting/utils/permission.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The permissions.
 
 This module should not import any other module from the application.
 
 """
-import typing as t
+from collections.abc import Callable
 
 from flask import abort, Blueprint, Response
 
 from accounting.utils.user import get_current_user, UserUtilityInterface
 
 
-def has_permission(rule: t.Callable[[], bool]) -> t.Callable:
+def has_permission(rule: Callable[[], bool]) -> Callable:
     """The permission decorator to check whether the current user is allowed.
 
     :param rule: The permission rule.
     :return: The view decorator.
     """
 
-    def decorator(view: t.Callable) -> t.Callable:
+    def decorator(view: Callable) -> Callable:
         """The view decorator to decorate a view with permission tests.
 
         :param view: The view.
         :return: The decorated view.
         """
 
         def decorated_view(*args, **kwargs):
@@ -57,24 +57,24 @@
             return view(*args, **kwargs)
 
         return decorated_view
 
     return decorator
 
 
-__can_view_func: t.Callable[[], bool] = lambda: True
+__can_view_func: Callable[[], bool] = lambda: True
 """The callback that returns whether the current user can view the accounting
 data."""
-__can_edit_func: t.Callable[[], bool] = lambda: True
+__can_edit_func: Callable[[], bool] = lambda: True
 """The callback that returns whether the current user can edit the accounting
 data."""
-__can_admin_func: t.Callable[[], bool] = lambda: True
+__can_admin_func: Callable[[], bool] = lambda: True
 """The callback that returns whether the current user can administrate the
 accounting settings."""
-_unauthorized_func: t.Callable[[], Response | None] \
+_unauthorized_func: Callable[[], Response | None] \
     = lambda: Response(status=403)
 """The callback that returns the response to require the user to log in."""
 
 
 def can_view() -> bool:
     """Returns whether the current user can view the accounting data.
```

### Comparing `mia-accounting-1.5.0/src/accounting/utils/query.py` & `mia-accounting-1.5.1/src/accounting/utils/query.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/utils/random_id.py` & `mia-accounting-1.5.1/src/accounting/utils/random_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-"""The random ID mixin for the data models.
+"""The random ID utility for the data models.
 
 This module should not import any other module from the application.
 
 """
-import typing as t
 from secrets import randbelow
+from typing import Type
 
 from accounting import db
 
 
-def new_id(cls: t.Type):
-    """Returns a new random ID for the data model.
+def new_id(cls: Type[db.Model]):
+    """Generates and returns a new, unused random ID for the data model.
 
     :param cls: The data model.
-    :return: The generated new random ID.
+    :return: The newly-generated, unused random ID.
     """
     while True:
         obj_id: int = 100000000 + randbelow(900000000)
         if db.session.get(cls, obj_id) is None:
             return obj_id
```

### Comparing `mia-accounting-1.5.0/src/accounting/utils/strip_text.py` & `mia-accounting-1.5.1/src/accounting/utils/strip_text.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/src/accounting/utils/user.py` & `mia-accounting-1.5.1/src/accounting/utils/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The user utilities.
 
 This module should not import any other module from the application.
 
 """
-import typing as t
 from abc import ABC, abstractmethod
+from typing import TypeVar, Generic, Type
 
 import sqlalchemy as sa
 from flask import g, Response
 from flask_sqlalchemy.model import Model
 
-T = t.TypeVar("T", bound=Model)
+T = TypeVar("T", bound=Model)
 
 
-class UserUtilityInterface(t.Generic[T], ABC):
+class UserUtilityInterface(Generic[T], ABC):
     """The interface for the user utilities."""
 
     @abstractmethod
     def can_view(self) -> bool:
         """Returns whether the currently logged-in user can view the accounting
         data.
 
@@ -68,15 +68,15 @@
         an HTTP 403 Forbidden response is return to the user.
 
         :return: The response to require the user to log in.
         """
 
     @property
     @abstractmethod
-    def cls(self) -> t.Type[T]:
+    def cls(self) -> Type[T]:
         """Returns the class of the user data model.
 
         :return: The class of the user data model.
         """
 
     @property
     @abstractmethod
@@ -108,15 +108,15 @@
 
         :return: The primary key of the user, as an integer.
         """
 
 
 __user_utils: UserUtilityInterface
 """The user utilities."""
-user_cls: t.Type[Model] = Model
+user_cls: Type[Model] = Model
 """The user class."""
 user_pk_column: sa.Column = sa.Column(sa.Integer)
 """The primary key column of the user class."""
 
 
 def init_user_utils(utils: UserUtilityInterface) -> None:
     """Initializes the user utilities.
```

### Comparing `mia-accounting-1.5.0/src/mia_accounting.egg-info/PKG-INFO` & `mia-accounting-1.5.1/src/mia_accounting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.5.0
+Version: 1.5.1
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
```

### Comparing `mia-accounting-1.5.0/src/mia_accounting.egg-info/SOURCES.txt` & `mia-accounting-1.5.1/src/mia_accounting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/babel-utils-test-site.py` & `mia-accounting-1.5.1/tests/babel-utils-test-site.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/babel-utils.py` & `mia-accounting-1.5.1/tests/babel-utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_account.py` & `mia-accounting-1.5.1/tests/test_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The test for the account management.
 
 """
+import datetime as dt
 import unittest
-from datetime import timedelta, date
 
 import httpx
 from flask import Flask
 
 from test_site import db
 from testlib import NEXT_URI, create_test_app, get_client, set_locale, \
     add_journal_entry
@@ -457,15 +457,15 @@
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             account = Account.find_by_code(CASH.code)
             self.assertIsNotNone(account)
             account.created_at \
-                = account.created_at - timedelta(seconds=5)
+                = account.created_at - dt.timedelta(seconds=5)
             account.updated_at = account.created_at
             db.session.commit()
 
         response = self.client.post(update_uri,
                                     data={"csrf_token": self.csrf_token,
                                           "base_code": CASH.base_code,
                                           "title": STOCK.title})
@@ -588,15 +588,15 @@
                                           "title": PETTY.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         add_journal_entry(self.client,
                           form={"csrf_token": self.csrf_token,
                                 "next": NEXT_URI,
-                                "date": date.today().isoformat(),
+                                "date": dt.date.today().isoformat(),
                                 "currency-1-code": "USD",
                                 "currency-1-credit-1-account_code": BANK.code,
                                 "currency-1-credit-1-amount": "20"})
 
         with self.app.app_context():
             self.assertEqual({x.code for x in Account.query.all()},
                              {CASH.code, PETTY.code, BANK.code})
```

### Comparing `mia-accounting-1.5.0/tests/test_base_account.py` & `mia-accounting-1.5.1/tests/test_base_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_commands.py` & `mia-accounting-1.5.1/tests/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The test for the console commands.
 
 """
 import csv
-import typing as t
 import unittest
+from typing import Any
 
 import sqlalchemy as sa
 from click.testing import Result
 from flask import Flask
 from flask.testing import FlaskCliRunner
 from sqlalchemy.sql.ddl import DropTable
 
@@ -76,15 +76,15 @@
 
         :return: None.
         """
         from accounting import data_dir
         from accounting.models import BaseAccount
 
         with open(data_dir / "base_accounts.csv") as fp:
-            data: dict[dict[str, t.Any]] \
+            data: dict[dict[str, Any]] \
                 = {x["code"]: {"code": x["code"],
                                "title": x["title"],
                                "l10n": {y[5:]: x[y]
                                         for y in x if y.startswith("l10n-")}}
                    for x in csv.DictReader(fp)}
 
         with self.app.app_context():
@@ -131,15 +131,15 @@
 
         :return: None.
         """
         from accounting import data_dir
         from accounting.models import Currency
 
         with open(data_dir / "currencies.csv") as fp:
-            data: dict[dict[str, t.Any]] \
+            data: dict[dict[str, Any]] \
                 = {x["code"]: {"code": x["code"],
                                "name": x["name"],
                                "l10n": {y[5:]: x[y]
                                         for y in x if y.startswith("l10n-")}}
                    for x in csv.DictReader(fp)}
 
         with self.app.app_context():
```

### Comparing `mia-accounting-1.5.0/tests/test_currency.py` & `mia-accounting-1.5.1/tests/test_currency.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The test for the currency management.
 
 """
+import datetime as dt
 import unittest
-from datetime import timedelta, date
 
 import httpx
 from flask import Flask
 
 from test_site import db
 from testlib import NEXT_URI, create_test_app, get_client, set_locale, \
     add_journal_entry
@@ -380,15 +380,15 @@
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             currency = db.session.get(Currency, USD.code)
             self.assertIsNotNone(currency)
             currency.created_at \
-                = currency.created_at - timedelta(seconds=5)
+                = currency.created_at - dt.timedelta(seconds=5)
             currency.updated_at = currency.created_at
             db.session.commit()
 
         response = self.client.post(update_uri,
                                     data={"csrf_token": self.csrf_token,
                                           "code": USD.code,
                                           "name": TWD.name})
@@ -530,15 +530,15 @@
                                           "name": JPY.name})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         add_journal_entry(self.client,
                           form={"csrf_token": self.csrf_token,
                                 "next": NEXT_URI,
-                                "date": date.today().isoformat(),
+                                "date": dt.date.today().isoformat(),
                                 "currency-1-code": EUR.code,
                                 "currency-1-credit-1-account_code": "1111-001",
                                 "currency-1-credit-1-amount": "20"})
 
         with self.app.app_context():
             self.assertEqual({x.code for x in Currency.query.all()},
                              {USD.code, EUR.code, JPY.code})
```

### Comparing `mia-accounting-1.5.0/tests/test_description_editor.py` & `mia-accounting-1.5.1/tests/test_description_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The test for the description editor.
 
 """
+import datetime as dt
 import unittest
-from datetime import date
 
 from flask import Flask
 
 from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
     add_journal_entry
 
 
@@ -145,15 +145,15 @@
 
 def get_form_data(csrf_token: str) -> list[dict[str, str]]:
     """Returns the form data for multiple journal entry forms.
 
     :param csrf_token: The CSRF token.
     :return: A list of the form data.
     """
-    journal_entry_date: str = date.today().isoformat()
+    journal_entry_date: str = dt.date.today().isoformat()
     return [{"csrf_token": csrf_token,
              "next": NEXT_URI,
              "date": journal_entry_date,
              "currency-0-code": "USD",
              "currency-0-credit-0-account_code": Accounts.SERVICE,
              "currency-0-credit-0-description": " Salary ",
              "currency-0-credit-0-amount": "2500"},
```

### Comparing `mia-accounting-1.5.0/tests/test_journal_entry.py` & `mia-accounting-1.5.1/tests/test_journal_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The test for the journal entry management.
 
 """
+import datetime as dt
 import unittest
-from datetime import date, timedelta
 from decimal import Decimal
 
 import httpx
 from flask import Flask
 
 from test_site import db
 from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
@@ -496,15 +496,15 @@
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             journal_entry.created_at \
-                = journal_entry.created_at - timedelta(seconds=5)
+                = journal_entry.created_at - dt.timedelta(seconds=5)
             journal_entry.updated_at = journal_entry.created_at
             db.session.commit()
 
         response = self.client.post(
             update_uri, data=self.__get_update_form(journal_entry_id))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
@@ -572,15 +572,15 @@
             line_item: JournalEntryLineItem \
                 = [x for x in journal_entry.line_items
                    if x.account_code == Accounts.PAYABLE][0]
         add_journal_entry(
             self.client,
             form={"csrf_token": self.csrf_token,
                   "next": NEXT_URI,
-                  "date": date.today().isoformat(),
+                  "date": dt.date.today().isoformat(),
                   "currency-1-code": line_item.currency_code,
                   "currency-1-debit-1-original_line_item_id": line_item.id,
                   "currency-1-debit-1-account_code": line_item.account_code,
                   "currency-1-debit-1-amount": "1"})
 
         # Cannot delete the journal entry that is in use
         response = self.client.post(f"{PREFIX}/{journal_entry_id_2}/delete",
@@ -1108,15 +1108,15 @@
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             journal_entry.created_at \
-                = journal_entry.created_at - timedelta(seconds=5)
+                = journal_entry.created_at - dt.timedelta(seconds=5)
             journal_entry.updated_at = journal_entry.created_at
             db.session.commit()
 
         response = self.client.post(
             update_uri, data=self.__get_update_form(journal_entry_id))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
@@ -1769,15 +1769,15 @@
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             journal_entry.created_at \
-                = journal_entry.created_at - timedelta(seconds=5)
+                = journal_entry.created_at - dt.timedelta(seconds=5)
             journal_entry.updated_at = journal_entry.created_at
             db.session.commit()
 
         response = self.client.post(
             update_uri, data=self.__get_update_form(journal_entry_id))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
@@ -2120,17 +2120,17 @@
         id_4: int = add_journal_entry(self.client,
                                       self.__get_add_receipt_form())
         id_5: int = add_journal_entry(self.client,
                                       self.__get_add_disbursement_form())
 
         with self.app.app_context():
             journal_entry_1: JournalEntry = db.session.get(JournalEntry, id_1)
-            journal_entry_date_2: date = journal_entry_1.date
-            journal_entry_date_1: date \
-                = journal_entry_date_2 - timedelta(days=1)
+            journal_entry_date_2: dt.date = journal_entry_1.date
+            journal_entry_date_1: dt.date \
+                = journal_entry_date_2 - dt.timedelta(days=1)
             journal_entry_1.date = journal_entry_date_1
             journal_entry_1.no = 3
             journal_entry_2: JournalEntry = db.session.get(JournalEntry, id_2)
             journal_entry_2.date = journal_entry_date_1
             journal_entry_2.no = 5
             journal_entry_3: JournalEntry = db.session.get(JournalEntry, id_3)
             journal_entry_3.date = journal_entry_date_1
@@ -2172,18 +2172,18 @@
                                       self.__get_add_transfer_form())
         id_4: int = add_journal_entry(self.client,
                                       self.__get_add_receipt_form())
         id_5: int = add_journal_entry(self.client,
                                       self.__get_add_disbursement_form())
 
         with self.app.app_context():
-            journal_entry_date: date = db.session.get(JournalEntry, id_1).date
+            date: dt.date = db.session.get(JournalEntry, id_1).date
 
         response = self.client.post(
-            f"{PREFIX}/dates/{journal_entry_date.isoformat()}",
+            f"{PREFIX}/dates/{date.isoformat()}",
             data={"csrf_token": self.csrf_token,
                   "next": "/next",
                   f"{id_1}-no": "4",
                   f"{id_2}-no": "1",
                   f"{id_3}-no": "5",
                   f"{id_4}-no": "2",
                   f"{id_5}-no": "3"})
@@ -2203,15 +2203,15 @@
             db.session.get(JournalEntry, id_2).no = 4
             db.session.get(JournalEntry, id_3).no = 6
             db.session.get(JournalEntry, id_4).no = 8
             db.session.get(JournalEntry, id_5).no = 9
             db.session.commit()
 
         response = self.client.post(
-            f"{PREFIX}/dates/{journal_entry_date.isoformat()}",
+            f"{PREFIX}/dates/{date.isoformat()}",
             data={"csrf_token": self.csrf_token,
                   "next": "/next",
                   f"{id_2}-no": "3a",
                   f"{id_3}-no": "5",
                   f"{id_4}-no": "2"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], f"/next")
```

### Comparing `mia-accounting-1.5.0/tests/test_offset.py` & `mia-accounting-1.5.1/tests/test_offset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_option.py` & `mia-accounting-1.5.1/tests/test_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The test for the options.
 
 """
+import datetime as dt
 import unittest
-from datetime import datetime, timedelta
 
 import httpx
 from flask import Flask
 
 from test_site import db
 from testlib import NEXT_URI, Accounts, create_test_app, get_client
 
@@ -282,15 +282,16 @@
         response = self.client.post(UPDATE_URI, data=self.__get_form())
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], DETAIL_URI)
 
         with self.app.app_context():
             option = db.session.get(Option, "recurring")
             self.assertIsNotNone(option)
-            timestamp: datetime = option.created_at - timedelta(seconds=5)
+            timestamp: dt.datetime \
+                = option.created_at - dt.timedelta(seconds=5)
             option.created_at = timestamp
             option.updated_at = timestamp
             db.session.commit()
 
         # The recurring setting was not modified
         form = self.__get_form()
         form["default_currency_code"] = "JPY"
```

### Comparing `mia-accounting-1.5.0/tests/test_report.py` & `mia-accounting-1.5.1/tests/test_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The test for the reports.
 
 """
+import datetime as dt
 import unittest
-from datetime import date
 
 import httpx
 from flask import Flask
 
 from test_site.lib import BaseTestData
 from testlib import create_test_app, get_client, Accounts
 
@@ -442,23 +442,23 @@
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
 
 class ReportTestData(BaseTestData):
     """The report test data."""
 
     def _init_data(self) -> None:
-        today: date = date.today()
+        today: dt.date = dt.date.today()
         year: int = today.year - 5
         month: int = today.month
         while True:
-            j_date: date = date(year, month, 5)
-            if j_date > today:
+            date: dt.date = dt.date(year, month, 5)
+            if date > today:
                 break
             self._add_simple_journal_entry(
-                (j_date - today).days, "USD",
+                (date - today).days, "USD",
                 "Salary薪水", "1200", Accounts.BANK, Accounts.SERVICE)
             month = month + 1
             if month > 12:
                 year = year + 1
                 month = 1
         self._add_simple_journal_entry(
             1, "USD", "Withdraw領錢", "1000", Accounts.CASH, Accounts.BANK)
```

### Comparing `mia-accounting-1.5.0/tests/test_site/__init__.py` & `mia-accounting-1.5.1/tests/test_site/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The Mia! Accounting demonstration website.
 
 """
 import os
-import typing as t
 from secrets import token_urlsafe
+from typing import Type
 
 from click.testing import Result
 from flask import Flask, Blueprint, render_template, redirect, Response, \
     url_for
 from flask.testing import FlaskCliRunner
 from flask_babel_js import BabelJS
 from flask_sqlalchemy import SQLAlchemy
@@ -90,15 +90,15 @@
                 and auth.current_user().username == "admin"
 
         def unauthorized(self) -> Response:
             from accounting.utils.next_uri import append_next
             return redirect(append_next(url_for("auth.login-form")))
 
         @property
-        def cls(self) -> t.Type[auth.User]:
+        def cls(self) -> Type[auth.User]:
             return auth.User
 
         @property
         def pk_column(self) -> Column:
             return auth.User.id
 
         @property
```

### Comparing `mia-accounting-1.5.0/tests/test_site/auth.py` & `mia-accounting-1.5.1/tests/test_site/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,32 +13,33 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The authentication for the Mia! Accounting demonstration website.
 
 """
-import typing as t
+from collections.abc import Callable
 
 from flask import Blueprint, render_template, Flask, redirect, url_for, \
     session, request, g, Response, abort
+from sqlalchemy.orm import Mapped, mapped_column
 
 from . import db
 
 bp: Blueprint = Blueprint("auth", __name__, url_prefix="/")
+"""The authentication blueprint."""
 
 
 class User(db.Model):
     """A user."""
     __tablename__ = "users"
     """The table name."""
-    id = db.Column(db.Integer, nullable=False, primary_key=True,
-                   autoincrement=True)
-    """The ID"""
-    username = db.Column(db.String, nullable=False, unique=True)
+    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
+    """The ID."""
+    username: Mapped[str] = mapped_column(unique=True)
     """The username."""
 
     def __str__(self) -> str:
         """Returns the string representation of the user.
 
         :return: The string representation of the user.
         """
@@ -91,15 +92,15 @@
             g.user = None
         else:
             g.user = User.query.filter(
                 User.username == session["user"]).first()
     return g.user
 
 
-def admin_required(view: t.Callable) -> t.Callable:
+def admin_required(view: Callable) -> Callable:
     """The view decorator to require the user to be an administrator.
 
     :param view: The view.
     :return: The decorated view.
     """
 
     def decorated_view(*args, **kwargs):
```

### Comparing `mia-accounting-1.5.0/tests/test_site/lib.py` & `mia-accounting-1.5.1/tests/test_site/lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The common library for the Mia! Accounting demonstration website.
 
 """
 from __future__ import annotations
 
-import typing as t
+import datetime as dt
 from abc import ABC, abstractmethod
-from datetime import date, timedelta
 from decimal import Decimal
 from secrets import randbelow
+from typing import Any
 
 import sqlalchemy as sa
 from flask import Flask
 
 from . import db
 from .auth import User
 
@@ -163,18 +163,18 @@
         """Returns the journal entry as a form.
 
         :param csrf_token: The CSRF token.
         :param next_uri: The next URI.
         :param is_update: True for an update operation, or False otherwise
         :return: The journal entry as a form.
         """
-        journal_entry_date: date = date.today() - timedelta(days=self.days)
+        date: dt.date = dt.date.today() - dt.timedelta(days=self.days)
         form: dict[str, str] = {"csrf_token": csrf_token,
                                 "next": next_uri,
-                                "date": journal_entry_date.isoformat()}
+                                "date": date.isoformat()}
         for i in range(len(self.currencies)):
             form.update(self.currencies[i].form(i + 1, is_update))
         if self.note is not None:
             form["note"] = self.note
         return form
 
 
@@ -189,16 +189,16 @@
         """
         self._app: Flask = app
         with self._app.app_context():
             current_user: User | None = User.query\
                 .filter(User.username == username).first()
             assert current_user is not None
             self.__current_user_id: int = current_user.id
-            self.__journal_entries: list[dict[str, t.Any]] = []
-            self.__line_items: list[dict[str, t.Any]] = []
+            self.__journal_entries: list[dict[str, Any]] = []
+            self.__line_items: list[dict[str, Any]] = []
             self._init_data()
 
     @abstractmethod
     def _init_data(self) -> None:
         """Initializes the test data.
 
         :return: None
@@ -236,32 +236,33 @@
         :param journal_entry_data: The journal entry data.
         :return: None.
         """
         from accounting.models import Account
         existing_j_id: set[int] = {x["id"] for x in self.__journal_entries}
         existing_l_id: set[int] = {x["id"] for x in self.__line_items}
         journal_entry_data.id = self.__new_id(existing_j_id)
-        j_date: date = date.today() - timedelta(days=journal_entry_data.days)
+        date: dt.date \
+            = dt.date.today() - dt.timedelta(days=journal_entry_data.days)
         self.__journal_entries.append(
             {"id": journal_entry_data.id,
-             "date": j_date,
-             "no": self.__next_j_no(j_date),
+             "date": date,
+             "no": self.__next_j_no(date),
              "note": journal_entry_data.note,
              "created_by_id": self.__current_user_id,
              "updated_by_id": self.__current_user_id})
         debit_no: int = 0
         credit_no: int = 0
         for currency in journal_entry_data.currencies:
             for line_item in currency.debit:
                 account: Account | None \
                     = Account.find_by_code(line_item.account)
                 assert account is not None
                 debit_no = debit_no + 1
                 line_item.id = self.__new_id(existing_l_id)
-                data: dict[str, t.Any] \
+                data: dict[str, Any] \
                     = {"id": line_item.id,
                        "journal_entry_id": journal_entry_data.id,
                        "is_debit": True,
                        "no": debit_no,
                        "account_id": account.id,
                        "currency_code": currency.code,
                        "description": line_item.description,
@@ -272,15 +273,15 @@
                 self.__line_items.append(data)
             for line_item in currency.credit:
                 account: Account | None \
                     = Account.find_by_code(line_item.account)
                 assert account is not None
                 credit_no = credit_no + 1
                 line_item.id = self.__new_id(existing_l_id)
-                data: dict[str, t.Any] \
+                data: dict[str, Any] \
                     = {"id": line_item.id,
                        "journal_entry_id": journal_entry_data.id,
                        "is_debit": False,
                        "no": credit_no,
                        "account_id": account.id,
                        "currency_code": currency.code,
                        "description": line_item.description,
@@ -299,22 +300,22 @@
         """
         while True:
             obj_id: int = 100000000 + randbelow(900000000)
             if obj_id not in existing_id:
                 existing_id.add(obj_id)
                 return obj_id
 
-    def __next_j_no(self, j_date: date) -> int:
+    def __next_j_no(self, date: dt.date) -> int:
         """Returns the next journal entry number in a day.
 
-        :param j_date: The journal entry date.
+        :param date: The journal entry date.
         :return: The next journal entry number.
         """
         existing: set[int] = {x["no"] for x in self.__journal_entries
-                              if x["date"] == j_date}
+                              if x["date"] == date}
         return 1 if len(existing) == 0 else max(existing) + 1
 
     def _add_simple_journal_entry(
             self, days: int, currency: str, description: str, amount: str,
             debit: str, credit: str) \
             -> tuple[JournalEntryLineItemData, JournalEntryLineItemData]:
         """Adds a simple journal entry.
```

### Comparing `mia-accounting-1.5.0/tests/test_site/locale.py` & `mia-accounting-1.5.1/tests/test_site/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_site/reset.py` & `mia-accounting-1.5.1/tests/test_site/reset.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The data reset for the Mia! Accounting demonstration website.
 
 """
-from datetime import date, timedelta
+import datetime as dt
 
 from flask import Flask, Blueprint, url_for, flash, redirect, session, \
     render_template, current_app
 from flask_babel import lazy_gettext
 
 from . import db
 from .auth import admin_required
@@ -112,23 +112,23 @@
         self.__add_twd_recurring()
 
     def __add_usd_recurring(self) -> None:
         """Adds the recurring data in USD.
 
         :return: None.
         """
-        today: date = date.today()
+        today: dt.date = dt.date.today()
         days: int
         year: int
         month: int
 
         # Recurring in USD
-        j_date: date = date(today.year - 5, today.month, today.day)
-        j_date = j_date + timedelta(days=(4 - j_date.weekday()))
-        days = (today - j_date).days
+        date: dt.date = dt.date(today.year - 5, today.month, today.day)
+        date = date + dt.timedelta(days=(4 - date.weekday()))
+        days = (today - date).days
         while True:
             if days < 0:
                 break
             self.__add_journal_entry(
                 days, "USD", "2600",
                 Accounts.BANK, "Transfer", Accounts.SERVICE, "Payroll")
 
@@ -143,32 +143,32 @@
         year = today.year - 5
         month = today.month
         while True:
             month = month + 1
             if month > 12:
                 year = year + 1
                 month = 1
-            days = (today - date(year, month, 1)).days
+            days = (today - dt.date(year, month, 1)).days
             if days < 0:
                 break
             self.__add_journal_entry(
                 days, "USD", "1800",
                 Accounts.RENT_EXPENSE, "Rent", Accounts.BANK, "Transfer")
 
     def __add_twd_recurring(self) -> None:
         """Adds the recurring data in TWD.
 
         :return: None.
         """
-        today: date = date.today()
+        today: dt.date = dt.date.today()
 
         year: int = today.year - 5
         month: int = today.month
         while True:
-            days: int = (today - date(year, month, 5)).days
+            days: int = (today - dt.date(year, month, 5)).days
             if days < 0:
                 break
             self.__add_journal_entry(
                 days, "TWD", "50000",
                 Accounts.BANK, "薪資轉帳", Accounts.SERVICE, "薪水")
 
             days = days - 1
```

### Comparing `mia-accounting-1.5.0/tests/test_site/static/favicon.svg` & `mia-accounting-1.5.1/tests/test_site/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_site/templates/base.html` & `mia-accounting-1.5.1/tests/test_site/templates/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_site/templates/home.html` & `mia-accounting-1.5.1/tests/test_site/templates/home.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_site/templates/login.html` & `mia-accounting-1.5.1/tests/test_site/templates/login.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_site/templates/reset.html` & `mia-accounting-1.5.1/tests/test_site/templates/reset.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_site/translations/messages.pot` & `mia-accounting-1.5.1/tests/test_site/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo` & `mia-accounting-1.5.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po` & `mia-accounting-1.5.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo` & `mia-accounting-1.5.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po` & `mia-accounting-1.5.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_unmatched_offset.py` & `mia-accounting-1.5.1/tests/test_unmatched_offset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/test_utils.py` & `mia-accounting-1.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.0/tests/testlib.py` & `mia-accounting-1.5.1/tests/testlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  limitations under the License.
 """The common test libraries.
 
 """
 from __future__ import annotations
 
 import re
-import typing as t
+from typing import Literal
 
 import httpx
 from flask import Flask, render_template_string
 
 from test_site import create_app
 
 TEST_SERVER: str = "https://testserver"
@@ -104,15 +104,15 @@
                                                  "username": username})
     assert response.status_code == 302
     assert response.headers["Location"] == "/"
     return client, csrf_token
 
 
 def set_locale(client: httpx.Client, csrf_token: str,
-               locale: t.Literal["en", "zh_Hant", "zh_Hans"]) -> None:
+               locale: Literal["en", "zh_Hant", "zh_Hans"]) -> None:
     """Sets the current locale.
 
     :param client: The test client.
     :param csrf_token: The CSRF token.
     :param locale: The locale.
     :return: None.
     """
```

### Comparing `mia-accounting-1.5.0/tests/testlib_journal_entry.py` & `mia-accounting-1.5.1/tests/testlib_journal_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The common test libraries for the journal entry test cases.
 
 """
+import datetime as dt
 import re
-from datetime import date
 from decimal import Decimal
 from secrets import randbelow
 
 from flask import Flask
 
 from test_site import db
 from testlib import NEXT_URI, Accounts
@@ -37,15 +37,15 @@
     """Returns the form data to add a new journal entry.
 
     :param csrf_token: The CSRF token.
     :return: The form data to add a new journal entry.
     """
     return {"csrf_token": csrf_token,
             "next": NEXT_URI,
-            "date": date.today().isoformat(),
+            "date": dt.date.today().isoformat(),
             "currency-0-code": "USD",
             "currency-0-debit-0-no": "16",
             "currency-0-debit-0-account_code": Accounts.CASH,
             "currency-0-debit-0-description": " ",
             "currency-0-debit-0-amount": " 495.26 ",
             "currency-0-debit-6-no": "2",
             "currency-0-debit-6-account_code": Accounts.BANK,
```

