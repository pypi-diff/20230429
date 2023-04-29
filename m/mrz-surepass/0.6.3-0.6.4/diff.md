# Comparing `tmp/mrz-surepass-0.6.3.tar.gz` & `tmp/mrz-surepass-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrz-surepass-0.6.3.tar", last modified: Sat Apr 29 14:41:19 2023, max compression
+gzip compressed data, was "mrz-surepass-0.6.4.tar", last modified: Sat Apr 29 14:48:05 2023, max compression
```

## Comparing `mrz-surepass-0.6.3.tar` & `mrz-surepass-0.6.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:41:19.092298 mrz-surepass-0.6.3/
--rwxr-xr-x   0 spooderman   (501) staff       (20)    35147 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/LICENSE
--rw-r--r--   0 spooderman   (501) staff       (20)    15330 2023-04-29 14:41:19.092397 mrz-surepass-0.6.3/PKG-INFO
--rwxr-xr-x   0 spooderman   (501) staff       (20)    16358 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/README.rst
-drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:41:19.085169 mrz-surepass-0.6.3/mrz/
--rwxr-xr-x   0 spooderman   (501) staff       (20)      618 2023-04-29 14:26:46.000000 mrz-surepass-0.6.3/mrz/__init__.py
-drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:41:19.086491 mrz-surepass-0.6.3/mrz/base/
--rwxr-xr-x   0 spooderman   (501) staff       (20)     7992 2023-04-29 13:59:48.000000 mrz-surepass-0.6.3/mrz/base/countries.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     3985 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/base/countries_ops.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     1973 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/base/errors.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     3548 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/base/functions.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     4343 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/base/string_checkers.py
-drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:41:19.088234 mrz-surepass-0.6.3/mrz/checker/
--rwxr-xr-x   0 spooderman   (501) staff       (20)      954 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/checker/__init__.py
--rw-r--r--   0 spooderman   (501) staff       (20)      271 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/checker/_enums.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)    11085 2023-04-29 13:59:48.000000 mrz-surepass-0.6.3/mrz/checker/_fields.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     1917 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/checker/_hash_fields.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     1808 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/checker/_honorifics.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     1687 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/checker/_report.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     2727 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/checker/mrva.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     2727 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/checker/mrvb.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     6034 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/checker/td1.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     5595 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/checker/td2.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     6374 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/checker/td3.py
-drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:41:19.089482 mrz-surepass-0.6.3/mrz/generator/
--rwxr-xr-x   0 spooderman   (501) staff       (20)     1003 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/__init__.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     3231 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/_fields.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     2290 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/_hash_fields.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     2939 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/_holder_name.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     1664 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/_transliterations.py
-drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:41:19.090929 mrz-surepass-0.6.3/mrz/generator/dictionaries/
--rwxr-xr-x   0 spooderman   (501) staff       (20)      602 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/dictionaries/__init__.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     2724 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/dictionaries/arabic.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     3027 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/dictionaries/cyrillic.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     3140 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/dictionaries/cyrillic_belarussian.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     3085 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/dictionaries/cyrillic_bulgarian.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     3086 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/dictionaries/cyrillic_macedonian.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     3080 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/dictionaries/cyrillic_serbian.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     3136 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/dictionaries/cyrillic_ukrainian.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     2233 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/dictionaries/greek.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     6348 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/dictionaries/hebrew.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     5924 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/dictionaries/latin_based.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     4075 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/mrva.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     3933 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/mrvb.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     6712 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/td1.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     5517 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/td2.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     5798 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/generator/td3.py
-drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:41:19.084116 mrz-surepass-0.6.3/mrz/special_cases/
-drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:41:19.091545 mrz-surepass-0.6.3/mrz/special_cases/checker/
--rw-r--r--   0 spooderman   (501) staff       (20)        0 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/special_cases/checker/__init__.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)      772 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/special_cases/checker/id_card_belgium.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     1110 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/special_cases/checker/id_card_germany.py
--rw-r--r--   0 spooderman   (501) staff       (20)      530 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/special_cases/checker/residence_permit_estonia.py
--rwxr-xr-x   0 spooderman   (501) staff       (20)     4020 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/special_cases/checker/td3_india.py
-drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:41:19.091759 mrz-surepass-0.6.3/mrz/special_cases/generator/
--rw-r--r--   0 spooderman   (501) staff       (20)        0 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/special_cases/generator/__init__.py
--rw-r--r--   0 spooderman   (501) staff       (20)     1347 2023-04-29 09:40:59.000000 mrz-surepass-0.6.3/mrz/special_cases/generator/belgium_id_card.py
-drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:41:19.092197 mrz-surepass-0.6.3/mrz_surepass.egg-info/
--rw-r--r--   0 spooderman   (501) staff       (20)    15330 2023-04-29 14:41:19.000000 mrz-surepass-0.6.3/mrz_surepass.egg-info/PKG-INFO
--rw-r--r--   0 spooderman   (501) staff       (20)     1595 2023-04-29 14:41:19.000000 mrz-surepass-0.6.3/mrz_surepass.egg-info/SOURCES.txt
--rw-r--r--   0 spooderman   (501) staff       (20)        1 2023-04-29 14:41:19.000000 mrz-surepass-0.6.3/mrz_surepass.egg-info/dependency_links.txt
--rw-r--r--   0 spooderman   (501) staff       (20)        4 2023-04-29 14:41:19.000000 mrz-surepass-0.6.3/mrz_surepass.egg-info/top_level.txt
--rwxr-xr-x   0 spooderman   (501) staff       (20)       67 2023-04-29 14:41:19.092657 mrz-surepass-0.6.3/setup.cfg
--rwxr-xr-x   0 spooderman   (501) staff       (20)     1646 2023-04-29 14:39:45.000000 mrz-surepass-0.6.3/setup.py
+drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:48:05.457194 mrz-surepass-0.6.4/
+-rwxr-xr-x   0 spooderman   (501) staff       (20)    35147 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/LICENSE
+-rw-r--r--   0 spooderman   (501) staff       (20)    15568 2023-04-29 14:48:05.457292 mrz-surepass-0.6.4/PKG-INFO
+-rwxr-xr-x   0 spooderman   (501) staff       (20)    16358 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/README.rst
+drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:48:05.450290 mrz-surepass-0.6.4/mrz/
+-rwxr-xr-x   0 spooderman   (501) staff       (20)      618 2023-04-29 14:46:51.000000 mrz-surepass-0.6.4/mrz/__init__.py
+drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:48:05.451455 mrz-surepass-0.6.4/mrz/base/
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     7992 2023-04-29 13:59:48.000000 mrz-surepass-0.6.4/mrz/base/countries.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     3985 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/base/countries_ops.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     1973 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/base/errors.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     3548 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/base/functions.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     4343 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/base/string_checkers.py
+drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:48:05.453049 mrz-surepass-0.6.4/mrz/checker/
+-rwxr-xr-x   0 spooderman   (501) staff       (20)      954 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/checker/__init__.py
+-rw-r--r--   0 spooderman   (501) staff       (20)      271 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/checker/_enums.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)    11085 2023-04-29 13:59:48.000000 mrz-surepass-0.6.4/mrz/checker/_fields.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     1917 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/checker/_hash_fields.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     1808 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/checker/_honorifics.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     1687 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/checker/_report.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     2727 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/checker/mrva.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     2727 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/checker/mrvb.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     6034 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/checker/td1.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     5595 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/checker/td2.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     6374 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/checker/td3.py
+drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:48:05.454368 mrz-surepass-0.6.4/mrz/generator/
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     1003 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/__init__.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     3231 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/_fields.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     2290 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/_hash_fields.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     2939 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/_holder_name.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     1664 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/_transliterations.py
+drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:48:05.455809 mrz-surepass-0.6.4/mrz/generator/dictionaries/
+-rwxr-xr-x   0 spooderman   (501) staff       (20)      602 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/dictionaries/__init__.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     2724 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/dictionaries/arabic.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     3027 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/dictionaries/cyrillic.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     3140 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/dictionaries/cyrillic_belarussian.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     3085 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/dictionaries/cyrillic_bulgarian.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     3086 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/dictionaries/cyrillic_macedonian.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     3080 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/dictionaries/cyrillic_serbian.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     3136 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/dictionaries/cyrillic_ukrainian.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     2233 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/dictionaries/greek.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     6348 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/dictionaries/hebrew.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     5924 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/dictionaries/latin_based.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     4075 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/mrva.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     3933 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/mrvb.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     6712 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/td1.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     5517 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/td2.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     5798 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/generator/td3.py
+drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:48:05.448931 mrz-surepass-0.6.4/mrz/special_cases/
+drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:48:05.456426 mrz-surepass-0.6.4/mrz/special_cases/checker/
+-rw-r--r--   0 spooderman   (501) staff       (20)        0 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/special_cases/checker/__init__.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)      772 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/special_cases/checker/id_card_belgium.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     1110 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/special_cases/checker/id_card_germany.py
+-rw-r--r--   0 spooderman   (501) staff       (20)      530 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/special_cases/checker/residence_permit_estonia.py
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     4020 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/special_cases/checker/td3_india.py
+drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:48:05.456650 mrz-surepass-0.6.4/mrz/special_cases/generator/
+-rw-r--r--   0 spooderman   (501) staff       (20)        0 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/special_cases/generator/__init__.py
+-rw-r--r--   0 spooderman   (501) staff       (20)     1347 2023-04-29 09:40:59.000000 mrz-surepass-0.6.4/mrz/special_cases/generator/belgium_id_card.py
+drwxr-xr-x   0 spooderman   (501) staff       (20)        0 2023-04-29 14:48:05.457092 mrz-surepass-0.6.4/mrz_surepass.egg-info/
+-rw-r--r--   0 spooderman   (501) staff       (20)    15568 2023-04-29 14:48:05.000000 mrz-surepass-0.6.4/mrz_surepass.egg-info/PKG-INFO
+-rw-r--r--   0 spooderman   (501) staff       (20)     1595 2023-04-29 14:48:05.000000 mrz-surepass-0.6.4/mrz_surepass.egg-info/SOURCES.txt
+-rw-r--r--   0 spooderman   (501) staff       (20)        1 2023-04-29 14:48:05.000000 mrz-surepass-0.6.4/mrz_surepass.egg-info/dependency_links.txt
+-rw-r--r--   0 spooderman   (501) staff       (20)        4 2023-04-29 14:48:05.000000 mrz-surepass-0.6.4/mrz_surepass.egg-info/top_level.txt
+-rwxr-xr-x   0 spooderman   (501) staff       (20)       67 2023-04-29 14:48:05.457578 mrz-surepass-0.6.4/setup.cfg
+-rwxr-xr-x   0 spooderman   (501) staff       (20)     1646 2023-04-29 14:39:45.000000 mrz-surepass-0.6.4/setup.py
```

### Comparing `mrz-surepass-0.6.3/LICENSE` & `mrz-surepass-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/PKG-INFO` & `mrz-surepass-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrz-surepass
-Version: 0.6.3
+Version: 0.6.4
 Summary: Machine readable zone generator and checker for passports, visas, id cards and other travel documents
 Home-page: https://github.com/surepassio/mrz-surepass
 Author: Rishabh Chauhan
 Author-email: rc@surepass.io
 License: GPLv3
 Keywords: mrz passports visas id cards td1 td2 td3 mrva mrvb icao
 Classifier: Development Status :: 4 - Beta
@@ -286,7 +286,22 @@
 - MRZ is a Python module to be used as library in other programs. So, its intended audience are developers. 
 **MRZ will never have a user interface nor will have CLI support.** (Of course.. if someone wants, can do it)
 However, **if someone is curious and wants to generate or check the mrz code of a passport or ID card, 
 can modify any of the [examples](https://github.com/Arg0s1080/mrz/tree/master/examples)**.
 
 - Right now I am very busy and have very little free time. Please, before creating an issue or consulting by email, 
 read [this issue](https://github.com/Arg0s1080/mrz/issues/31)
+
+
+### Uploading to PyPi
+1. Remove existing directories
+   ```shell
+   rm -r build dist
+   ```
+2. Build
+    ```shell
+     python3 setup.py sdist bdist_wheel
+    ```
+3. Upload to PyPi
+    ```shell
+     twine upload --verbose dist/*
+    ```
```

### Comparing `mrz-surepass-0.6.3/README.rst` & `mrz-surepass-0.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/__init__.py` & `mrz-surepass-0.6.4/mrz/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # For more information on this, and how to apply and follow the GNU GPL, see:
 # http://www.gnu.org/licenses
 #
 # (ɔ) Iván Rincón 2019
 
 __author__  = "Iván Rincón"
 __license__ = "GPL3"
-__version__ = "0.6.3"
+__version__ = "0.6.4"
```

### Comparing `mrz-surepass-0.6.3/mrz/base/countries.py` & `mrz-surepass-0.6.4/mrz/base/countries.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/base/countries_ops.py` & `mrz-surepass-0.6.4/mrz/base/countries_ops.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/base/errors.py` & `mrz-surepass-0.6.4/mrz/base/errors.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/base/functions.py` & `mrz-surepass-0.6.4/mrz/base/functions.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/base/string_checkers.py` & `mrz-surepass-0.6.4/mrz/base/string_checkers.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/checker/__init__.py` & `mrz-surepass-0.6.4/mrz/checker/__init__.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/checker/_fields.py` & `mrz-surepass-0.6.4/mrz/checker/_fields.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/checker/_hash_fields.py` & `mrz-surepass-0.6.4/mrz/checker/_hash_fields.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/checker/_honorifics.py` & `mrz-surepass-0.6.4/mrz/checker/_honorifics.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/checker/_report.py` & `mrz-surepass-0.6.4/mrz/checker/_report.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/checker/mrva.py` & `mrz-surepass-0.6.4/mrz/checker/mrva.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/checker/mrvb.py` & `mrz-surepass-0.6.4/mrz/checker/mrvb.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/checker/td1.py` & `mrz-surepass-0.6.4/mrz/checker/td1.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/checker/td2.py` & `mrz-surepass-0.6.4/mrz/checker/td2.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/checker/td3.py` & `mrz-surepass-0.6.4/mrz/checker/td3.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/__init__.py` & `mrz-surepass-0.6.4/mrz/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/_fields.py` & `mrz-surepass-0.6.4/mrz/generator/_fields.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/_hash_fields.py` & `mrz-surepass-0.6.4/mrz/generator/_hash_fields.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/_holder_name.py` & `mrz-surepass-0.6.4/mrz/generator/_holder_name.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/_transliterations.py` & `mrz-surepass-0.6.4/mrz/generator/_transliterations.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/dictionaries/__init__.py` & `mrz-surepass-0.6.4/mrz/generator/dictionaries/__init__.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/dictionaries/arabic.py` & `mrz-surepass-0.6.4/mrz/generator/dictionaries/arabic.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/dictionaries/cyrillic.py` & `mrz-surepass-0.6.4/mrz/generator/dictionaries/cyrillic.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/dictionaries/cyrillic_belarussian.py` & `mrz-surepass-0.6.4/mrz/generator/dictionaries/cyrillic_belarussian.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/dictionaries/cyrillic_bulgarian.py` & `mrz-surepass-0.6.4/mrz/generator/dictionaries/cyrillic_bulgarian.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/dictionaries/cyrillic_macedonian.py` & `mrz-surepass-0.6.4/mrz/generator/dictionaries/cyrillic_macedonian.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/dictionaries/cyrillic_serbian.py` & `mrz-surepass-0.6.4/mrz/generator/dictionaries/cyrillic_serbian.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/dictionaries/cyrillic_ukrainian.py` & `mrz-surepass-0.6.4/mrz/generator/dictionaries/cyrillic_ukrainian.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/dictionaries/greek.py` & `mrz-surepass-0.6.4/mrz/generator/dictionaries/greek.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/dictionaries/hebrew.py` & `mrz-surepass-0.6.4/mrz/generator/dictionaries/hebrew.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/dictionaries/latin_based.py` & `mrz-surepass-0.6.4/mrz/generator/dictionaries/latin_based.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/mrva.py` & `mrz-surepass-0.6.4/mrz/generator/mrva.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/mrvb.py` & `mrz-surepass-0.6.4/mrz/generator/mrvb.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/td1.py` & `mrz-surepass-0.6.4/mrz/generator/td1.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/td2.py` & `mrz-surepass-0.6.4/mrz/generator/td2.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/generator/td3.py` & `mrz-surepass-0.6.4/mrz/generator/td3.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/special_cases/checker/id_card_belgium.py` & `mrz-surepass-0.6.4/mrz/special_cases/checker/id_card_belgium.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/special_cases/checker/id_card_germany.py` & `mrz-surepass-0.6.4/mrz/special_cases/checker/id_card_germany.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/special_cases/checker/residence_permit_estonia.py` & `mrz-surepass-0.6.4/mrz/special_cases/checker/residence_permit_estonia.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/special_cases/checker/td3_india.py` & `mrz-surepass-0.6.4/mrz/special_cases/checker/td3_india.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz/special_cases/generator/belgium_id_card.py` & `mrz-surepass-0.6.4/mrz/special_cases/generator/belgium_id_card.py`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/mrz_surepass.egg-info/PKG-INFO` & `mrz-surepass-0.6.4/mrz_surepass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrz-surepass
-Version: 0.6.3
+Version: 0.6.4
 Summary: Machine readable zone generator and checker for passports, visas, id cards and other travel documents
 Home-page: https://github.com/surepassio/mrz-surepass
 Author: Rishabh Chauhan
 Author-email: rc@surepass.io
 License: GPLv3
 Keywords: mrz passports visas id cards td1 td2 td3 mrva mrvb icao
 Classifier: Development Status :: 4 - Beta
@@ -286,7 +286,22 @@
 - MRZ is a Python module to be used as library in other programs. So, its intended audience are developers. 
 **MRZ will never have a user interface nor will have CLI support.** (Of course.. if someone wants, can do it)
 However, **if someone is curious and wants to generate or check the mrz code of a passport or ID card, 
 can modify any of the [examples](https://github.com/Arg0s1080/mrz/tree/master/examples)**.
 
 - Right now I am very busy and have very little free time. Please, before creating an issue or consulting by email, 
 read [this issue](https://github.com/Arg0s1080/mrz/issues/31)
+
+
+### Uploading to PyPi
+1. Remove existing directories
+   ```shell
+   rm -r build dist
+   ```
+2. Build
+    ```shell
+     python3 setup.py sdist bdist_wheel
+    ```
+3. Upload to PyPi
+    ```shell
+     twine upload --verbose dist/*
+    ```
```

### Comparing `mrz-surepass-0.6.3/mrz_surepass.egg-info/SOURCES.txt` & `mrz-surepass-0.6.4/mrz_surepass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mrz-surepass-0.6.3/setup.py` & `mrz-surepass-0.6.4/setup.py`

 * *Files identical despite different names*

