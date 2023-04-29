# Comparing `tmp/seleniumbase-4.9.8.tar.gz` & `tmp/seleniumbase-4.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seleniumbase-4.9.8.tar", last modified: Fri Dec 16 22:47:58 2022, max compression
+gzip compressed data, was "seleniumbase-4.9.9.tar", last modified: Sun Dec 18 20:07:02 2022, max compression
```

## Comparing `seleniumbase-4.9.8.tar` & `seleniumbase-4.9.9.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.351356 seleniumbase-4.9.8/
--rw-r--r--   0 michael    (501) staff       (20)     1833 2022-11-29 06:20:07.000000 seleniumbase-4.9.8/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)     1085 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)      710 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)    69523 2022-12-16 22:47:58.351503 seleniumbase-4.9.8/PKG-INFO
--rwxr-xr-x   0 michael    (501) staff       (20)    67150 2022-12-07 19:49:43.000000 seleniumbase-4.9.8/README.md
--rwxr-xr-x   0 michael    (501) staff       (20)      216 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/install.sh
--rw-r--r--   0 michael    (501) staff       (20)     1436 2022-11-25 20:04:06.000000 seleniumbase-4.9.8/pytest.ini
--rwxr-xr-x   0 michael    (501) staff       (20)     5704 2022-12-16 22:45:24.000000 seleniumbase-4.9.8/requirements.txt
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.334273 seleniumbase-4.9.8/sbase/
--rwxr-xr-x   0 michael    (501) staff       (20)      516 2022-11-26 20:58:40.000000 seleniumbase-4.9.8/sbase/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      647 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/sbase/__main__.py
--rw-r--r--   0 michael    (501) staff       (20)    18304 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/sbase/steps.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.334660 seleniumbase-4.9.8/seleniumbase/
--rwxr-xr-x   0 michael    (501) staff       (20)     2192 2022-12-15 15:51:24.000000 seleniumbase-4.9.8/seleniumbase/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      654 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/__main__.py
--rwxr-xr-x   0 michael    (501) staff       (20)       45 2022-12-16 22:45:24.000000 seleniumbase-4.9.8/seleniumbase/__version__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.335857 seleniumbase-4.9.8/seleniumbase/behave/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/behave/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    16106 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/behave/behave_helper.py
--rw-r--r--   0 michael    (501) staff       (20)    52202 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/behave/behave_sb.py
--rw-r--r--   0 michael    (501) staff       (20)      390 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/behave/steps.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.336537 seleniumbase-4.9.8/seleniumbase/common/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/common/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)     7859 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/common/decorators.py
--rwxr-xr-x   0 michael    (501) staff       (20)     5622 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/common/encryption.py
--rwxr-xr-x   0 michael    (501) staff       (20)      803 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/common/exceptions.py
--rwxr-xr-x   0 michael    (501) staff       (20)     1204 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/common/obfuscate.py
--rwxr-xr-x   0 michael    (501) staff       (20)      979 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/common/unobfuscate.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.336969 seleniumbase-4.9.8/seleniumbase/config/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/config/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)     3197 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/config/ad_block_list.py
--rwxr-xr-x   0 michael    (501) staff       (20)     1091 2022-11-03 20:37:05.000000 seleniumbase-4.9.8/seleniumbase/config/proxy_list.py
--rwxr-xr-x   0 michael    (501) staff       (20)     7027 2022-11-23 07:24:32.000000 seleniumbase-4.9.8/seleniumbase/config/settings.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.338932 seleniumbase-4.9.8/seleniumbase/console_scripts/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)     1732 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/logo_helper.py
--rwxr-xr-x   0 michael    (501) staff       (20)     1582 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/rich_helper.py
--rw-r--r--   0 michael    (501) staff       (20)    55778 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/run.py
--rwxr-xr-x   0 michael    (501) staff       (20)    14510 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/sb_behave_gui.py
--rwxr-xr-x   0 michael    (501) staff       (20)    17651 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/sb_caseplans.py
--rwxr-xr-x   0 michael    (501) staff       (20)    10803 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/sb_commander.py
--rwxr-xr-x   0 michael    (501) staff       (20)    37106 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/sb_install.py
--rwxr-xr-x   0 michael    (501) staff       (20)    11152 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/sb_mkchart.py
--rwxr-xr-x   0 michael    (501) staff       (20)    29500 2022-12-03 00:14:22.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/sb_mkdir.py
--rwxr-xr-x   0 michael    (501) staff       (20)    11141 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/sb_mkfile.py
--rwxr-xr-x   0 michael    (501) staff       (20)    11211 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/sb_mkpres.py
--rwxr-xr-x   0 michael    (501) staff       (20)     8496 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/sb_mkrec.py
--rwxr-xr-x   0 michael    (501) staff       (20)   118593 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/sb_objectify.py
--rwxr-xr-x   0 michael    (501) staff       (20)    31986 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/sb_print.py
--rwxr-xr-x   0 michael    (501) staff       (20)     9831 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/console_scripts/sb_recorder.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.341513 seleniumbase-4.9.8/seleniumbase/core/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/core/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)      576 2022-11-25 20:04:06.000000 seleniumbase-4.9.8/seleniumbase/core/application_manager.py
--rwxr-xr-x   0 michael    (501) staff       (20)   119708 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/core/browser_launcher.py
--rwxr-xr-x   0 michael    (501) staff       (20)     5760 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/core/capabilities_parser.py
--rw-r--r--   0 michael    (501) staff       (20)     2060 2022-12-16 22:45:24.000000 seleniumbase-4.9.8/seleniumbase/core/colored_traceback.py
--rwxr-xr-x   0 michael    (501) staff       (20)      972 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/core/create_db_tables.sql
--rw-r--r--   0 michael    (501) staff       (20)     5860 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/core/detect_b_ver.py
--rwxr-xr-x   0 michael    (501) staff       (20)     2057 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/core/download_helper.py
--rwxr-xr-x   0 michael    (501) staff       (20)    14209 2022-11-02 06:42:15.000000 seleniumbase-4.9.8/seleniumbase/core/encoded_images.py
--rwxr-xr-x   0 michael    (501) staff       (20)    10423 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/core/jqc_helper.py
--rwxr-xr-x   0 michael    (501) staff       (20)    20965 2022-12-16 22:45:24.000000 seleniumbase-4.9.8/seleniumbase/core/log_helper.py
--rwxr-xr-x   0 michael    (501) staff       (20)     3890 2022-11-25 20:04:06.000000 seleniumbase-4.9.8/seleniumbase/core/mysql.py
--rwxr-xr-x   0 michael    (501) staff       (20)     5134 2022-11-25 20:04:06.000000 seleniumbase-4.9.8/seleniumbase/core/proxy_helper.py
--rwxr-xr-x   0 michael    (501) staff       (20)    13013 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/core/report_helper.py
--rwxr-xr-x   0 michael    (501) staff       (20)     3441 2022-11-25 20:04:06.000000 seleniumbase-4.9.8/seleniumbase/core/s3_manager.py
--rwxr-xr-x   0 michael    (501) staff       (20)     7070 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/core/settings_parser.py
--rwxr-xr-x   0 michael    (501) staff       (20)    11456 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/core/style_sheet.py
--rwxr-xr-x   0 michael    (501) staff       (20)     4633 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/core/testcase_manager.py
--rwxr-xr-x   0 michael    (501) staff       (20)    40669 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/core/tour_helper.py
--rwxr-xr-x   0 michael    (501) staff       (20)     3408 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/core/visual_helper.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.341633 seleniumbase-4.9.8/seleniumbase/drivers/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/drivers/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.342302 seleniumbase-4.9.8/seleniumbase/extensions/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/extensions/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    11978 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/extensions/ad_block.zip
--rw-r--r--   0 michael    (501) staff       (20)    11824 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/extensions/disable_csp.zip
--rw-r--r--   0 michael    (501) staff       (20)    12085 2022-11-18 01:37:09.000000 seleniumbase-4.9.8/seleniumbase/extensions/recorder.zip
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.344121 seleniumbase-4.9.8/seleniumbase/fixtures/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/fixtures/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)   621437 2022-12-16 22:45:24.000000 seleniumbase-4.9.8/seleniumbase/fixtures/base_case.py
--rwxr-xr-x   0 michael    (501) staff       (20)    10418 2022-11-25 20:04:06.000000 seleniumbase-4.9.8/seleniumbase/fixtures/constants.py
--rwxr-xr-x   0 michael    (501) staff       (20)     2015 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/fixtures/css_to_xpath.py
--rwxr-xr-x   0 michael    (501) staff       (20)      560 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/fixtures/errors.py
--rwxr-xr-x   0 michael    (501) staff       (20)    44112 2022-11-08 20:06:55.000000 seleniumbase-4.9.8/seleniumbase/fixtures/js_utils.py
--rwxr-xr-x   0 michael    (501) staff       (20)    46131 2022-11-06 04:45:36.000000 seleniumbase-4.9.8/seleniumbase/fixtures/page_actions.py
--rwxr-xr-x   0 michael    (501) staff       (20)     8208 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/fixtures/page_utils.py
--rwxr-xr-x   0 michael    (501) staff       (20)     4587 2022-11-25 20:04:06.000000 seleniumbase-4.9.8/seleniumbase/fixtures/shared_utils.py
--rwxr-xr-x   0 michael    (501) staff       (20)     5309 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/fixtures/words.py
--rwxr-xr-x   0 michael    (501) staff       (20)     8877 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/fixtures/xpath_to_css.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.344477 seleniumbase-4.9.8/seleniumbase/js_code/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/js_code/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)     6619 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/js_code/live_js.py
--rwxr-xr-x   0 michael    (501) staff       (20)    31462 2022-11-18 01:37:09.000000 seleniumbase-4.9.8/seleniumbase/js_code/recorder_js.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.344735 seleniumbase-4.9.8/seleniumbase/masterqa/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/masterqa/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)    19700 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/masterqa/master_qa.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.346271 seleniumbase-4.9.8/seleniumbase/plugins/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/plugins/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)    15370 2022-12-16 22:45:24.000000 seleniumbase-4.9.8/seleniumbase/plugins/base_plugin.py
--rwxr-xr-x   0 michael    (501) staff       (20)     2417 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/plugins/basic_test_info.py
--rwxr-xr-x   0 michael    (501) staff       (20)     6841 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/plugins/db_reporting_plugin.py
--rw-r--r--   0 michael    (501) staff       (20)    16442 2022-11-18 20:28:25.000000 seleniumbase-4.9.8/seleniumbase/plugins/driver_manager.py
--rwxr-xr-x   0 michael    (501) staff       (20)     2226 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/plugins/page_source.py
--rw-r--r--   0 michael    (501) staff       (20)    87339 2022-12-16 22:45:24.000000 seleniumbase-4.9.8/seleniumbase/plugins/pytest_plugin.py
--rwxr-xr-x   0 michael    (501) staff       (20)     1985 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/plugins/s3_logging_plugin.py
--rw-r--r--   0 michael    (501) staff       (20)    34349 2022-12-16 22:45:24.000000 seleniumbase-4.9.8/seleniumbase/plugins/sb_manager.py
--rwxr-xr-x   0 michael    (501) staff       (20)     1304 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/plugins/screen_shots.py
--rwxr-xr-x   0 michael    (501) staff       (20)    50052 2022-12-02 07:14:32.000000 seleniumbase-4.9.8/seleniumbase/plugins/selenium_plugin.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.346430 seleniumbase-4.9.8/seleniumbase/resources/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/resources/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.348084 seleniumbase-4.9.8/seleniumbase/translate/
--rwxr-xr-x   0 michael    (501) staff       (20)      459 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/translate/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)    23325 2022-11-11 19:50:19.000000 seleniumbase-4.9.8/seleniumbase/translate/chinese.py
--rwxr-xr-x   0 michael    (501) staff       (20)    23948 2022-11-11 19:50:19.000000 seleniumbase-4.9.8/seleniumbase/translate/dutch.py
--rwxr-xr-x   0 michael    (501) staff       (20)    24179 2022-11-11 19:50:19.000000 seleniumbase-4.9.8/seleniumbase/translate/french.py
--rwxr-xr-x   0 michael    (501) staff       (20)    24016 2022-11-11 19:50:19.000000 seleniumbase-4.9.8/seleniumbase/translate/italian.py
--rwxr-xr-x   0 michael    (501) staff       (20)    25508 2022-11-11 19:50:19.000000 seleniumbase-4.9.8/seleniumbase/translate/japanese.py
--rwxr-xr-x   0 michael    (501) staff       (20)    24515 2022-11-11 19:50:19.000000 seleniumbase-4.9.8/seleniumbase/translate/korean.py
--rwxr-xr-x   0 michael    (501) staff       (20)   115835 2022-11-11 19:50:19.000000 seleniumbase-4.9.8/seleniumbase/translate/master_dict.py
--rwxr-xr-x   0 michael    (501) staff       (20)    23964 2022-11-11 19:50:19.000000 seleniumbase-4.9.8/seleniumbase/translate/portuguese.py
--rwxr-xr-x   0 michael    (501) staff       (20)    26430 2022-11-11 19:50:19.000000 seleniumbase-4.9.8/seleniumbase/translate/russian.py
--rwxr-xr-x   0 michael    (501) staff       (20)    24121 2022-11-11 19:50:19.000000 seleniumbase-4.9.8/seleniumbase/translate/spanish.py
--rwxr-xr-x   0 michael    (501) staff       (20)    50427 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/translate/translator.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.348888 seleniumbase-4.9.8/seleniumbase/undetected/
--rw-r--r--   0 michael    (501) staff       (20)    20729 2022-12-03 00:14:22.000000 seleniumbase-4.9.8/seleniumbase/undetected/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     3508 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/undetected/cdp.py
--rw-r--r--   0 michael    (501) staff       (20)     1884 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/undetected/dprocess.py
--rw-r--r--   0 michael    (501) staff       (20)     2718 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/undetected/options.py
--rw-r--r--   0 michael    (501) staff       (20)     8431 2022-11-09 06:27:52.000000 seleniumbase-4.9.8/seleniumbase/undetected/patcher.py
--rw-r--r--   0 michael    (501) staff       (20)     2898 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/undetected/reactor.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.349011 seleniumbase-4.9.8/seleniumbase/utilities/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/utilities/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.350990 seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)     1862 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/download_selenium_server.py
--rwxr-xr-x   0 michael    (501) staff       (20)      468 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/font_color
--rwxr-xr-x   0 michael    (501) staff       (20)     3021 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/grid-hub
--rwxr-xr-x   0 michael    (501) staff       (20)     3186 2022-11-18 20:28:25.000000 seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/grid-node
--rwxr-xr-x   0 michael    (501) staff       (20)     5023 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/grid_hub.py
--rwxr-xr-x   0 michael    (501) staff       (20)     5444 2022-11-18 20:28:25.000000 seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/grid_node.py
--rwxr-xr-x   0 michael    (501) staff       (20)      263 2022-11-18 20:28:25.000000 seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/register-grid-node.bat
--rwxr-xr-x   0 michael    (501) staff       (20)      275 2022-11-18 20:28:25.000000 seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/register-grid-node.sh
--rwxr-xr-x   0 michael    (501) staff       (20)       94 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/start-grid-hub.bat
--rwxr-xr-x   0 michael    (501) staff       (20)      106 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/start-grid-hub.sh
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.351227 seleniumbase-4.9.8/seleniumbase/utilities/selenium_ide/
--rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/utilities/selenium_ide/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)    32256 2022-10-30 23:14:39.000000 seleniumbase-4.9.8/seleniumbase/utilities/selenium_ide/convert_ide.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:47:58.335384 seleniumbase-4.9.8/seleniumbase.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)    69523 2022-12-16 22:47:58.000000 seleniumbase-4.9.8/seleniumbase.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     4860 2022-12-16 22:47:58.000000 seleniumbase-4.9.8/seleniumbase.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2022-12-16 22:47:58.000000 seleniumbase-4.9.8/seleniumbase.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)      623 2022-12-16 22:47:58.000000 seleniumbase-4.9.8/seleniumbase.egg-info/entry_points.txt
--rw-r--r--   0 michael    (501) staff       (20)     3978 2022-12-16 22:47:58.000000 seleniumbase-4.9.8/seleniumbase.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       19 2022-12-16 22:47:58.000000 seleniumbase-4.9.8/seleniumbase.egg-info/top_level.txt
--rwxr-xr-x   0 michael    (501) staff       (20)      217 2022-12-16 22:47:58.351725 seleniumbase-4.9.8/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)    16779 2022-12-16 22:45:24.000000 seleniumbase-4.9.8/setup.py
--rwxr-xr-x   0 michael    (501) staff       (20)     1512 2022-10-31 00:28:14.000000 seleniumbase-4.9.8/virtualenv_install.sh
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.314125 seleniumbase-4.9.9/
+-rw-r--r--   0 michael    (501) staff       (20)     1833 2022-11-29 06:20:07.000000 seleniumbase-4.9.9/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)     1085 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)      710 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)    69523 2022-12-18 20:07:02.314267 seleniumbase-4.9.9/PKG-INFO
+-rwxr-xr-x   0 michael    (501) staff       (20)    67150 2022-12-18 20:04:47.000000 seleniumbase-4.9.9/README.md
+-rwxr-xr-x   0 michael    (501) staff       (20)      216 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/install.sh
+-rw-r--r--   0 michael    (501) staff       (20)     1436 2022-11-25 20:04:06.000000 seleniumbase-4.9.9/pytest.ini
+-rwxr-xr-x   0 michael    (501) staff       (20)     5704 2022-12-18 20:04:47.000000 seleniumbase-4.9.9/requirements.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.296013 seleniumbase-4.9.9/sbase/
+-rwxr-xr-x   0 michael    (501) staff       (20)      516 2022-11-26 20:58:40.000000 seleniumbase-4.9.9/sbase/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      647 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/sbase/__main__.py
+-rw-r--r--   0 michael    (501) staff       (20)    18304 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/sbase/steps.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.296416 seleniumbase-4.9.9/seleniumbase/
+-rwxr-xr-x   0 michael    (501) staff       (20)     2192 2022-12-15 15:51:24.000000 seleniumbase-4.9.9/seleniumbase/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      654 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/__main__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)       45 2022-12-18 20:04:47.000000 seleniumbase-4.9.9/seleniumbase/__version__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.298126 seleniumbase-4.9.9/seleniumbase/behave/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/behave/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    16106 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/behave/behave_helper.py
+-rw-r--r--   0 michael    (501) staff       (20)    52202 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/behave/behave_sb.py
+-rw-r--r--   0 michael    (501) staff       (20)      390 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/behave/steps.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.298857 seleniumbase-4.9.9/seleniumbase/common/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/common/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     7859 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/common/decorators.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     5622 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/common/encryption.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      803 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/common/exceptions.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     1204 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/common/obfuscate.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      979 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/common/unobfuscate.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.299290 seleniumbase-4.9.9/seleniumbase/config/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/config/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     3197 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/config/ad_block_list.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     1091 2022-11-03 20:37:05.000000 seleniumbase-4.9.9/seleniumbase/config/proxy_list.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     7027 2022-11-23 07:24:32.000000 seleniumbase-4.9.9/seleniumbase/config/settings.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.301400 seleniumbase-4.9.9/seleniumbase/console_scripts/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     1732 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/logo_helper.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     1582 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/rich_helper.py
+-rw-r--r--   0 michael    (501) staff       (20)    55778 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/run.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    14510 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/sb_behave_gui.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    17651 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/sb_caseplans.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    10803 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/sb_commander.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    37106 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/sb_install.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    11152 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/sb_mkchart.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    29500 2022-12-03 00:14:22.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/sb_mkdir.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    11141 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/sb_mkfile.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    11211 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/sb_mkpres.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     8496 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/sb_mkrec.py
+-rwxr-xr-x   0 michael    (501) staff       (20)   118593 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/sb_objectify.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    31986 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/sb_print.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     9831 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/console_scripts/sb_recorder.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.304133 seleniumbase-4.9.9/seleniumbase/core/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/core/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      576 2022-11-25 20:04:06.000000 seleniumbase-4.9.9/seleniumbase/core/application_manager.py
+-rwxr-xr-x   0 michael    (501) staff       (20)   119708 2022-12-16 23:12:03.000000 seleniumbase-4.9.9/seleniumbase/core/browser_launcher.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     5760 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/core/capabilities_parser.py
+-rw-r--r--   0 michael    (501) staff       (20)     2060 2022-12-16 22:45:24.000000 seleniumbase-4.9.9/seleniumbase/core/colored_traceback.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      972 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/core/create_db_tables.sql
+-rw-r--r--   0 michael    (501) staff       (20)     5860 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/core/detect_b_ver.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     2057 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/core/download_helper.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    14209 2022-11-02 06:42:15.000000 seleniumbase-4.9.9/seleniumbase/core/encoded_images.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    10423 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/core/jqc_helper.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    20965 2022-12-16 22:45:24.000000 seleniumbase-4.9.9/seleniumbase/core/log_helper.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     3890 2022-11-25 20:04:06.000000 seleniumbase-4.9.9/seleniumbase/core/mysql.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     5134 2022-11-25 20:04:06.000000 seleniumbase-4.9.9/seleniumbase/core/proxy_helper.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    13013 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/core/report_helper.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     3441 2022-11-25 20:04:06.000000 seleniumbase-4.9.9/seleniumbase/core/s3_manager.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     7070 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/core/settings_parser.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    11456 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/core/style_sheet.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     4633 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/core/testcase_manager.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    40669 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/core/tour_helper.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     3408 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/core/visual_helper.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.304257 seleniumbase-4.9.9/seleniumbase/drivers/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/drivers/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.304928 seleniumbase-4.9.9/seleniumbase/extensions/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/extensions/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    11978 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/extensions/ad_block.zip
+-rw-r--r--   0 michael    (501) staff       (20)    11824 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/extensions/disable_csp.zip
+-rw-r--r--   0 michael    (501) staff       (20)    12085 2022-11-18 01:37:09.000000 seleniumbase-4.9.9/seleniumbase/extensions/recorder.zip
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.306858 seleniumbase-4.9.9/seleniumbase/fixtures/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/fixtures/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)   621437 2022-12-16 22:45:24.000000 seleniumbase-4.9.9/seleniumbase/fixtures/base_case.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    10418 2022-11-25 20:04:06.000000 seleniumbase-4.9.9/seleniumbase/fixtures/constants.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     2015 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/fixtures/css_to_xpath.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      560 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/fixtures/errors.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    44112 2022-11-08 20:06:55.000000 seleniumbase-4.9.9/seleniumbase/fixtures/js_utils.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    46131 2022-11-06 04:45:36.000000 seleniumbase-4.9.9/seleniumbase/fixtures/page_actions.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     8208 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/fixtures/page_utils.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     4587 2022-11-25 20:04:06.000000 seleniumbase-4.9.9/seleniumbase/fixtures/shared_utils.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     5309 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/fixtures/words.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     8877 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/fixtures/xpath_to_css.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.307202 seleniumbase-4.9.9/seleniumbase/js_code/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/js_code/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     6619 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/js_code/live_js.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    31462 2022-11-18 01:37:09.000000 seleniumbase-4.9.9/seleniumbase/js_code/recorder_js.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.307451 seleniumbase-4.9.9/seleniumbase/masterqa/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/masterqa/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    19700 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/masterqa/master_qa.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.308924 seleniumbase-4.9.9/seleniumbase/plugins/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/plugins/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    15370 2022-12-16 22:45:24.000000 seleniumbase-4.9.9/seleniumbase/plugins/base_plugin.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     2417 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/plugins/basic_test_info.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     6841 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/plugins/db_reporting_plugin.py
+-rw-r--r--   0 michael    (501) staff       (20)    16442 2022-11-18 20:28:25.000000 seleniumbase-4.9.9/seleniumbase/plugins/driver_manager.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     2226 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/plugins/page_source.py
+-rw-r--r--   0 michael    (501) staff       (20)    87339 2022-12-16 22:45:24.000000 seleniumbase-4.9.9/seleniumbase/plugins/pytest_plugin.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     1985 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/plugins/s3_logging_plugin.py
+-rw-r--r--   0 michael    (501) staff       (20)    34349 2022-12-16 22:45:24.000000 seleniumbase-4.9.9/seleniumbase/plugins/sb_manager.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     1304 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/plugins/screen_shots.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    50052 2022-12-02 07:14:32.000000 seleniumbase-4.9.9/seleniumbase/plugins/selenium_plugin.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.309091 seleniumbase-4.9.9/seleniumbase/resources/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/resources/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.310781 seleniumbase-4.9.9/seleniumbase/translate/
+-rwxr-xr-x   0 michael    (501) staff       (20)      459 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/translate/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    23325 2022-11-11 19:50:19.000000 seleniumbase-4.9.9/seleniumbase/translate/chinese.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    23948 2022-11-11 19:50:19.000000 seleniumbase-4.9.9/seleniumbase/translate/dutch.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    24179 2022-11-11 19:50:19.000000 seleniumbase-4.9.9/seleniumbase/translate/french.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    24016 2022-11-11 19:50:19.000000 seleniumbase-4.9.9/seleniumbase/translate/italian.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    25508 2022-11-11 19:50:19.000000 seleniumbase-4.9.9/seleniumbase/translate/japanese.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    24515 2022-11-11 19:50:19.000000 seleniumbase-4.9.9/seleniumbase/translate/korean.py
+-rwxr-xr-x   0 michael    (501) staff       (20)   115835 2022-11-11 19:50:19.000000 seleniumbase-4.9.9/seleniumbase/translate/master_dict.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    23964 2022-11-11 19:50:19.000000 seleniumbase-4.9.9/seleniumbase/translate/portuguese.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    26430 2022-11-11 19:50:19.000000 seleniumbase-4.9.9/seleniumbase/translate/russian.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    24121 2022-11-11 19:50:19.000000 seleniumbase-4.9.9/seleniumbase/translate/spanish.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    50427 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/translate/translator.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.311493 seleniumbase-4.9.9/seleniumbase/undetected/
+-rw-r--r--   0 michael    (501) staff       (20)    20729 2022-12-03 00:14:22.000000 seleniumbase-4.9.9/seleniumbase/undetected/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     3508 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/undetected/cdp.py
+-rw-r--r--   0 michael    (501) staff       (20)     1884 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/undetected/dprocess.py
+-rw-r--r--   0 michael    (501) staff       (20)     2718 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/undetected/options.py
+-rw-r--r--   0 michael    (501) staff       (20)     8431 2022-11-09 06:27:52.000000 seleniumbase-4.9.9/seleniumbase/undetected/patcher.py
+-rw-r--r--   0 michael    (501) staff       (20)     2898 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/undetected/reactor.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.311676 seleniumbase-4.9.9/seleniumbase/utilities/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/utilities/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.313721 seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     1862 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/download_selenium_server.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      468 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/font_color
+-rwxr-xr-x   0 michael    (501) staff       (20)     3021 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/grid-hub
+-rwxr-xr-x   0 michael    (501) staff       (20)     3186 2022-11-18 20:28:25.000000 seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/grid-node
+-rwxr-xr-x   0 michael    (501) staff       (20)     5023 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/grid_hub.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     5444 2022-11-18 20:28:25.000000 seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/grid_node.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      263 2022-11-18 20:28:25.000000 seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/register-grid-node.bat
+-rwxr-xr-x   0 michael    (501) staff       (20)      275 2022-11-18 20:28:25.000000 seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/register-grid-node.sh
+-rwxr-xr-x   0 michael    (501) staff       (20)       94 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/start-grid-hub.bat
+-rwxr-xr-x   0 michael    (501) staff       (20)      106 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/start-grid-hub.sh
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.313983 seleniumbase-4.9.9/seleniumbase/utilities/selenium_ide/
+-rwxr-xr-x   0 michael    (501) staff       (20)        0 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/utilities/selenium_ide/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    32256 2022-10-30 23:14:39.000000 seleniumbase-4.9.9/seleniumbase/utilities/selenium_ide/convert_ide.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:02.297610 seleniumbase-4.9.9/seleniumbase.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)    69523 2022-12-18 20:07:02.000000 seleniumbase-4.9.9/seleniumbase.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     4860 2022-12-18 20:07:02.000000 seleniumbase-4.9.9/seleniumbase.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2022-12-18 20:07:02.000000 seleniumbase-4.9.9/seleniumbase.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)      623 2022-12-18 20:07:02.000000 seleniumbase-4.9.9/seleniumbase.egg-info/entry_points.txt
+-rw-r--r--   0 michael    (501) staff       (20)     3978 2022-12-18 20:07:02.000000 seleniumbase-4.9.9/seleniumbase.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       19 2022-12-18 20:07:02.000000 seleniumbase-4.9.9/seleniumbase.egg-info/top_level.txt
+-rwxr-xr-x   0 michael    (501) staff       (20)      217 2022-12-18 20:07:02.314481 seleniumbase-4.9.9/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)    16779 2022-12-18 20:04:47.000000 seleniumbase-4.9.9/setup.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     1512 2022-10-31 00:28:14.000000 seleniumbase-4.9.9/virtualenv_install.sh
```

### Comparing `seleniumbase-4.9.8/.gitignore` & `seleniumbase-4.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/LICENSE` & `seleniumbase-4.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/MANIFEST.in` & `seleniumbase-4.9.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/PKG-INFO` & `seleniumbase-4.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seleniumbase
-Version: 4.9.8
+Version: 4.9.9
 Summary: A complete web automation framework for end-to-end testing.
 Home-page: https://github.com/seleniumbase/SeleniumBase
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/seleniumbase/SeleniumBase/releases
@@ -64,15 +64,15 @@
 Provides-Extra: psutil
 Provides-Extra: selenium-wire
 License-File: LICENSE
 
 <!-- SeleniumBase Docs -->
 
 
-<p align="center"><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_p3.png" alt="SeleniumBase" title="SeleniumBase" width="382" /></a></p>
+<p align="center"><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i3.png" alt="SeleniumBase" title="SeleniumBase" width="365" /></a></p>
 
 <h3 align="center"><img src="https://seleniumbase.github.io/cdn/img/python_logo.png" title="Python" width="29" /> <b>All-in-one Test Automation Framework</b> <img src="https://seleniumbase.github.io/cdn/img/python_logo.png" title="Python" width="29" /></h3>
 
 <p align="center"><a href="https://pypi.python.org/pypi/seleniumbase" target="_blank"><img src="https://img.shields.io/pypi/v/seleniumbase.svg?color=3399EE" alt="PyPI version" /></a> <a href="https://github.com/seleniumbase/SeleniumBase/releases" target="_blank"><img src="https://img.shields.io/github/v/release/seleniumbase/SeleniumBase.svg?color=22AAEE" alt="GitHub version" /></a> <a href="https://seleniumbase.io"><img src="https://img.shields.io/badge/docs-seleniumbase.io-11BBAA.svg" alt="SeleniumBase Docs" /></a> <a href="https://github.com/seleniumbase/SeleniumBase/actions" target="_blank"><img src="https://github.com/seleniumbase/SeleniumBase/workflows/CI%20build/badge.svg" alt="SeleniumBase GitHub Actions" /></a> <a href="https://gitter.im/seleniumbase/SeleniumBase" target="_blank"><img src="https://badges.gitter.im/seleniumbase/SeleniumBase.svg" alt="SeleniumBase" /></a></p>
 
 <p align="center">
 <a href="#python_installation">🏄 Start</a> |
@@ -1249,9 +1249,9 @@
 <span><a href="https://github.com/seleniumbase/SeleniumBase"><img src="https://seleniumbase.github.io/img/social/share_github.svg" title="SeleniumBase on GitHub" alt="SeleniumBase on GitHub" width="43" /></a></span>
 <span><a href="https://www.facebook.com/SeleniumBase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_facebook.svg" title="SeleniumBase on Facebook" alt="SeleniumBase on Facebook" width="37" /></a></span>
 <span><a href="https://gitter.im/seleniumbase/SeleniumBase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_gitter.svg" title="SeleniumBase on Gitter" alt="SeleniumBase on Gitter" width="35" /></a></span>
 <span><a href="https://instagram.com/seleniumbase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_instagram.svg" title="SeleniumBase on Instagram" alt="SeleniumBase on Instagram" width="33" /></a></span>
 <span><a href="https://twitter.com/seleniumbase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_twitter.svg" title="SeleniumBase on Twitter" alt="SeleniumBase on Twitter" width="39" /></a></span>
 </div></p>
 
-<p><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i2.png" alt="SeleniumBase" title="SeleniumBase" width="240" /></a></p>
+<p><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i3.png" alt="SeleniumBase" title="SeleniumBase" width="240" /></a></p>
 <p><a href="https://www.python.org/downloads/" target="_blank"><img src="https://img.shields.io/pypi/pyversions/seleniumbase.svg?color=22AAEE&logo=python&logoColor=FEDC54" title="Supported Python Versions" /></a></p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seleniumbase Version: 4.9.8 Summary: A complete web
+Metadata-Version: 2.1 Name: seleniumbase Version: 4.9.9 Summary: A complete web
 automation framework for end-to-end testing. Home-page: https://github.com/
 seleniumbase/SeleniumBase Author: Michael Mintz Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz License: MIT Project-URL: Changelog, https://
 github.com/seleniumbase/SeleniumBase/releases Project-URL: Download, https://
 pypi.org/project/seleniumbase/#files Project-URL: Gitter, https://gitter.im/
 seleniumbase/SeleniumBase Project-URL: Blog, https://seleniumbase.com/ Project-
 URL: PyPI, https://pypi.org/project/seleniumbase/ Project-URL: Source, https://
```

### Comparing `seleniumbase-4.9.8/README.md` & `seleniumbase-4.9.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <meta property="og:site_name" content="SeleniumBase">
 <meta property="og:title" content="SeleniumBase: Python Web Automation and E2E Testing" />
 <meta property="og:description" content="Fast, easy, and reliable Web/UI testing with Python." />
 <meta property="og:keywords" content="Python, pytest, selenium, webdriver, testing, automation, seleniumbase, framework, dashboard, recorder, reports, screenshots">
 <meta property="og:image" content="https://seleniumbase.github.io/cdn/img/mac_sb_logo_5b.png" />
 <link rel="icon" href="https://seleniumbase.github.io/img/logo3b.png" />
 
-<p align="center"><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_p3.png" alt="SeleniumBase" title="SeleniumBase" width="382" /></a></p>
+<p align="center"><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i3.png" alt="SeleniumBase" title="SeleniumBase" width="365" /></a></p>
 
 <h3 align="center"><img src="https://seleniumbase.github.io/cdn/img/python_logo.png" title="Python" width="29" /> <b>All-in-one Test Automation Framework</b> <img src="https://seleniumbase.github.io/cdn/img/python_logo.png" title="Python" width="29" /></h3>
 
 <p align="center"><a href="https://pypi.python.org/pypi/seleniumbase" target="_blank"><img src="https://img.shields.io/pypi/v/seleniumbase.svg?color=3399EE" alt="PyPI version" /></a> <a href="https://github.com/seleniumbase/SeleniumBase/releases" target="_blank"><img src="https://img.shields.io/github/v/release/seleniumbase/SeleniumBase.svg?color=22AAEE" alt="GitHub version" /></a> <a href="https://seleniumbase.io"><img src="https://img.shields.io/badge/docs-seleniumbase.io-11BBAA.svg" alt="SeleniumBase Docs" /></a> <a href="https://github.com/seleniumbase/SeleniumBase/actions" target="_blank"><img src="https://github.com/seleniumbase/SeleniumBase/workflows/CI%20build/badge.svg" alt="SeleniumBase GitHub Actions" /></a> <a href="https://gitter.im/seleniumbase/SeleniumBase" target="_blank"><img src="https://badges.gitter.im/seleniumbase/SeleniumBase.svg" alt="SeleniumBase" /></a></p>
 
 <p align="center">
 <a href="#python_installation">🏄 Start</a> |
@@ -1188,9 +1188,9 @@
 <span><a href="https://github.com/seleniumbase/SeleniumBase"><img src="https://seleniumbase.github.io/img/social/share_github.svg" title="SeleniumBase on GitHub" alt="SeleniumBase on GitHub" width="43" /></a></span>
 <span><a href="https://www.facebook.com/SeleniumBase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_facebook.svg" title="SeleniumBase on Facebook" alt="SeleniumBase on Facebook" width="37" /></a></span>
 <span><a href="https://gitter.im/seleniumbase/SeleniumBase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_gitter.svg" title="SeleniumBase on Gitter" alt="SeleniumBase on Gitter" width="35" /></a></span>
 <span><a href="https://instagram.com/seleniumbase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_instagram.svg" title="SeleniumBase on Instagram" alt="SeleniumBase on Instagram" width="33" /></a></span>
 <span><a href="https://twitter.com/seleniumbase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_twitter.svg" title="SeleniumBase on Twitter" alt="SeleniumBase on Twitter" width="39" /></a></span>
 </div></p>
 
-<p><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i2.png" alt="SeleniumBase" title="SeleniumBase" width="240" /></a></p>
+<p><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i3.png" alt="SeleniumBase" title="SeleniumBase" width="240" /></a></p>
 <p><a href="https://www.python.org/downloads/" target="_blank"><img src="https://img.shields.io/pypi/pyversions/seleniumbase.svg?color=22AAEE&logo=python&logoColor=FEDC54" title="Supported Python Versions" /></a></p>
```

### Comparing `seleniumbase-4.9.8/pytest.ini` & `seleniumbase-4.9.9/pytest.ini`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/requirements.txt` & `seleniumbase-4.9.9/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 cryptography==36.0.2;python_version>="3.6" and python_version<"3.7"
 cryptography==38.0.4;python_version>="3.7"
 pygments==2.5.2;python_version<"3.6"
 pygments==2.13.0;python_version>="3.6"
 pyreadline==2.1;platform_system=="Windows" and python_version<"3.6"
 pyreadline3==3.4.1;platform_system=="Windows" and python_version>="3.6"
 tabcompleter==1.1.0
-pdbp==1.2.6
+pdbp==1.2.7
 colorama==0.4.6;python_version<"3.6"
 colorama==0.4.5;python_version>="3.6" and python_version<"3.7"
 colorama==0.4.6;python_version>="3.7"
 exceptiongroup==1.0.4;python_version>="3.7"
 importlib-metadata==2.1.3;python_version<"3.6"
 importlib-metadata==4.2.0;python_version>="3.6" and python_version<"3.8"
 pycparser==2.21
```

### Comparing `seleniumbase-4.9.8/sbase/__init__.py` & `seleniumbase-4.9.9/sbase/__init__.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/sbase/__main__.py` & `seleniumbase-4.9.9/sbase/__main__.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/sbase/steps.py` & `seleniumbase-4.9.9/sbase/steps.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/__init__.py` & `seleniumbase-4.9.9/seleniumbase/__init__.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/__main__.py` & `seleniumbase-4.9.9/seleniumbase/__main__.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/behave/behave_helper.py` & `seleniumbase-4.9.9/seleniumbase/behave/behave_helper.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/behave/behave_sb.py` & `seleniumbase-4.9.9/seleniumbase/behave/behave_sb.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/common/decorators.py` & `seleniumbase-4.9.9/seleniumbase/common/decorators.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/common/encryption.py` & `seleniumbase-4.9.9/seleniumbase/common/encryption.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/common/exceptions.py` & `seleniumbase-4.9.9/seleniumbase/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/common/obfuscate.py` & `seleniumbase-4.9.9/seleniumbase/common/obfuscate.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/common/unobfuscate.py` & `seleniumbase-4.9.9/seleniumbase/common/unobfuscate.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/config/ad_block_list.py` & `seleniumbase-4.9.9/seleniumbase/config/ad_block_list.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/config/proxy_list.py` & `seleniumbase-4.9.9/seleniumbase/config/proxy_list.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/config/settings.py` & `seleniumbase-4.9.9/seleniumbase/config/settings.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/logo_helper.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/logo_helper.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/rich_helper.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/rich_helper.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/run.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/run.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/sb_behave_gui.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/sb_behave_gui.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/sb_caseplans.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/sb_caseplans.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/sb_commander.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/sb_commander.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/sb_install.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/sb_install.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/sb_mkchart.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/sb_mkchart.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/sb_mkdir.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/sb_mkdir.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/sb_mkfile.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/sb_mkfile.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/sb_mkpres.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/sb_mkpres.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/sb_mkrec.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/sb_mkrec.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/sb_objectify.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/sb_objectify.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/sb_print.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/sb_print.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/console_scripts/sb_recorder.py` & `seleniumbase-4.9.9/seleniumbase/console_scripts/sb_recorder.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/application_manager.py` & `seleniumbase-4.9.9/seleniumbase/core/application_manager.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/browser_launcher.py` & `seleniumbase-4.9.9/seleniumbase/core/browser_launcher.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/capabilities_parser.py` & `seleniumbase-4.9.9/seleniumbase/core/capabilities_parser.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/colored_traceback.py` & `seleniumbase-4.9.9/seleniumbase/core/colored_traceback.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/create_db_tables.sql` & `seleniumbase-4.9.9/seleniumbase/core/create_db_tables.sql`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/detect_b_ver.py` & `seleniumbase-4.9.9/seleniumbase/core/detect_b_ver.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/download_helper.py` & `seleniumbase-4.9.9/seleniumbase/core/download_helper.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/encoded_images.py` & `seleniumbase-4.9.9/seleniumbase/core/encoded_images.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/jqc_helper.py` & `seleniumbase-4.9.9/seleniumbase/core/jqc_helper.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/log_helper.py` & `seleniumbase-4.9.9/seleniumbase/core/log_helper.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/mysql.py` & `seleniumbase-4.9.9/seleniumbase/core/mysql.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/proxy_helper.py` & `seleniumbase-4.9.9/seleniumbase/core/proxy_helper.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/report_helper.py` & `seleniumbase-4.9.9/seleniumbase/core/report_helper.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/s3_manager.py` & `seleniumbase-4.9.9/seleniumbase/core/s3_manager.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/settings_parser.py` & `seleniumbase-4.9.9/seleniumbase/core/settings_parser.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/style_sheet.py` & `seleniumbase-4.9.9/seleniumbase/core/style_sheet.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/testcase_manager.py` & `seleniumbase-4.9.9/seleniumbase/core/testcase_manager.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/tour_helper.py` & `seleniumbase-4.9.9/seleniumbase/core/tour_helper.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/core/visual_helper.py` & `seleniumbase-4.9.9/seleniumbase/core/visual_helper.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/extensions/ad_block.zip` & `seleniumbase-4.9.9/seleniumbase/extensions/ad_block.zip`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/extensions/disable_csp.zip` & `seleniumbase-4.9.9/seleniumbase/extensions/disable_csp.zip`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/extensions/recorder.zip` & `seleniumbase-4.9.9/seleniumbase/extensions/recorder.zip`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/fixtures/base_case.py` & `seleniumbase-4.9.9/seleniumbase/fixtures/base_case.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/fixtures/constants.py` & `seleniumbase-4.9.9/seleniumbase/fixtures/constants.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/fixtures/css_to_xpath.py` & `seleniumbase-4.9.9/seleniumbase/fixtures/css_to_xpath.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/fixtures/errors.py` & `seleniumbase-4.9.9/seleniumbase/fixtures/errors.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/fixtures/js_utils.py` & `seleniumbase-4.9.9/seleniumbase/fixtures/js_utils.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/fixtures/page_actions.py` & `seleniumbase-4.9.9/seleniumbase/fixtures/page_actions.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/fixtures/page_utils.py` & `seleniumbase-4.9.9/seleniumbase/fixtures/page_utils.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/fixtures/shared_utils.py` & `seleniumbase-4.9.9/seleniumbase/fixtures/shared_utils.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/fixtures/words.py` & `seleniumbase-4.9.9/seleniumbase/fixtures/words.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/fixtures/xpath_to_css.py` & `seleniumbase-4.9.9/seleniumbase/fixtures/xpath_to_css.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/js_code/live_js.py` & `seleniumbase-4.9.9/seleniumbase/js_code/live_js.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/js_code/recorder_js.py` & `seleniumbase-4.9.9/seleniumbase/js_code/recorder_js.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/masterqa/master_qa.py` & `seleniumbase-4.9.9/seleniumbase/masterqa/master_qa.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/plugins/base_plugin.py` & `seleniumbase-4.9.9/seleniumbase/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/plugins/basic_test_info.py` & `seleniumbase-4.9.9/seleniumbase/plugins/basic_test_info.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/plugins/db_reporting_plugin.py` & `seleniumbase-4.9.9/seleniumbase/plugins/db_reporting_plugin.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/plugins/driver_manager.py` & `seleniumbase-4.9.9/seleniumbase/plugins/driver_manager.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/plugins/page_source.py` & `seleniumbase-4.9.9/seleniumbase/plugins/page_source.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/plugins/pytest_plugin.py` & `seleniumbase-4.9.9/seleniumbase/plugins/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/plugins/s3_logging_plugin.py` & `seleniumbase-4.9.9/seleniumbase/plugins/s3_logging_plugin.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/plugins/sb_manager.py` & `seleniumbase-4.9.9/seleniumbase/plugins/sb_manager.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/plugins/screen_shots.py` & `seleniumbase-4.9.9/seleniumbase/plugins/screen_shots.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/plugins/selenium_plugin.py` & `seleniumbase-4.9.9/seleniumbase/plugins/selenium_plugin.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/translate/chinese.py` & `seleniumbase-4.9.9/seleniumbase/translate/chinese.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/translate/dutch.py` & `seleniumbase-4.9.9/seleniumbase/translate/dutch.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/translate/french.py` & `seleniumbase-4.9.9/seleniumbase/translate/french.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/translate/italian.py` & `seleniumbase-4.9.9/seleniumbase/translate/italian.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/translate/japanese.py` & `seleniumbase-4.9.9/seleniumbase/translate/japanese.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/translate/korean.py` & `seleniumbase-4.9.9/seleniumbase/translate/korean.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/translate/master_dict.py` & `seleniumbase-4.9.9/seleniumbase/translate/master_dict.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/translate/portuguese.py` & `seleniumbase-4.9.9/seleniumbase/translate/portuguese.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/translate/russian.py` & `seleniumbase-4.9.9/seleniumbase/translate/russian.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/translate/spanish.py` & `seleniumbase-4.9.9/seleniumbase/translate/spanish.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/translate/translator.py` & `seleniumbase-4.9.9/seleniumbase/translate/translator.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/undetected/__init__.py` & `seleniumbase-4.9.9/seleniumbase/undetected/__init__.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/undetected/cdp.py` & `seleniumbase-4.9.9/seleniumbase/undetected/cdp.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/undetected/dprocess.py` & `seleniumbase-4.9.9/seleniumbase/undetected/dprocess.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/undetected/options.py` & `seleniumbase-4.9.9/seleniumbase/undetected/options.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/undetected/patcher.py` & `seleniumbase-4.9.9/seleniumbase/undetected/patcher.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/undetected/reactor.py` & `seleniumbase-4.9.9/seleniumbase/undetected/reactor.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/download_selenium_server.py` & `seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/download_selenium_server.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/grid-hub` & `seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/grid-hub`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/grid-node` & `seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/grid-node`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/grid_hub.py` & `seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/grid_hub.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/utilities/selenium_grid/grid_node.py` & `seleniumbase-4.9.9/seleniumbase/utilities/selenium_grid/grid_node.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase/utilities/selenium_ide/convert_ide.py` & `seleniumbase-4.9.9/seleniumbase/utilities/selenium_ide/convert_ide.py`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase.egg-info/PKG-INFO` & `seleniumbase-4.9.9/seleniumbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seleniumbase
-Version: 4.9.8
+Version: 4.9.9
 Summary: A complete web automation framework for end-to-end testing.
 Home-page: https://github.com/seleniumbase/SeleniumBase
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/seleniumbase/SeleniumBase/releases
@@ -64,15 +64,15 @@
 Provides-Extra: psutil
 Provides-Extra: selenium-wire
 License-File: LICENSE
 
 <!-- SeleniumBase Docs -->
 
 
-<p align="center"><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_p3.png" alt="SeleniumBase" title="SeleniumBase" width="382" /></a></p>
+<p align="center"><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i3.png" alt="SeleniumBase" title="SeleniumBase" width="365" /></a></p>
 
 <h3 align="center"><img src="https://seleniumbase.github.io/cdn/img/python_logo.png" title="Python" width="29" /> <b>All-in-one Test Automation Framework</b> <img src="https://seleniumbase.github.io/cdn/img/python_logo.png" title="Python" width="29" /></h3>
 
 <p align="center"><a href="https://pypi.python.org/pypi/seleniumbase" target="_blank"><img src="https://img.shields.io/pypi/v/seleniumbase.svg?color=3399EE" alt="PyPI version" /></a> <a href="https://github.com/seleniumbase/SeleniumBase/releases" target="_blank"><img src="https://img.shields.io/github/v/release/seleniumbase/SeleniumBase.svg?color=22AAEE" alt="GitHub version" /></a> <a href="https://seleniumbase.io"><img src="https://img.shields.io/badge/docs-seleniumbase.io-11BBAA.svg" alt="SeleniumBase Docs" /></a> <a href="https://github.com/seleniumbase/SeleniumBase/actions" target="_blank"><img src="https://github.com/seleniumbase/SeleniumBase/workflows/CI%20build/badge.svg" alt="SeleniumBase GitHub Actions" /></a> <a href="https://gitter.im/seleniumbase/SeleniumBase" target="_blank"><img src="https://badges.gitter.im/seleniumbase/SeleniumBase.svg" alt="SeleniumBase" /></a></p>
 
 <p align="center">
 <a href="#python_installation">🏄 Start</a> |
@@ -1249,9 +1249,9 @@
 <span><a href="https://github.com/seleniumbase/SeleniumBase"><img src="https://seleniumbase.github.io/img/social/share_github.svg" title="SeleniumBase on GitHub" alt="SeleniumBase on GitHub" width="43" /></a></span>
 <span><a href="https://www.facebook.com/SeleniumBase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_facebook.svg" title="SeleniumBase on Facebook" alt="SeleniumBase on Facebook" width="37" /></a></span>
 <span><a href="https://gitter.im/seleniumbase/SeleniumBase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_gitter.svg" title="SeleniumBase on Gitter" alt="SeleniumBase on Gitter" width="35" /></a></span>
 <span><a href="https://instagram.com/seleniumbase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_instagram.svg" title="SeleniumBase on Instagram" alt="SeleniumBase on Instagram" width="33" /></a></span>
 <span><a href="https://twitter.com/seleniumbase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_twitter.svg" title="SeleniumBase on Twitter" alt="SeleniumBase on Twitter" width="39" /></a></span>
 </div></p>
 
-<p><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i2.png" alt="SeleniumBase" title="SeleniumBase" width="240" /></a></p>
+<p><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i3.png" alt="SeleniumBase" title="SeleniumBase" width="240" /></a></p>
 <p><a href="https://www.python.org/downloads/" target="_blank"><img src="https://img.shields.io/pypi/pyversions/seleniumbase.svg?color=22AAEE&logo=python&logoColor=FEDC54" title="Supported Python Versions" /></a></p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seleniumbase Version: 4.9.8 Summary: A complete web
+Metadata-Version: 2.1 Name: seleniumbase Version: 4.9.9 Summary: A complete web
 automation framework for end-to-end testing. Home-page: https://github.com/
 seleniumbase/SeleniumBase Author: Michael Mintz Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz License: MIT Project-URL: Changelog, https://
 github.com/seleniumbase/SeleniumBase/releases Project-URL: Download, https://
 pypi.org/project/seleniumbase/#files Project-URL: Gitter, https://gitter.im/
 seleniumbase/SeleniumBase Project-URL: Blog, https://seleniumbase.com/ Project-
 URL: PyPI, https://pypi.org/project/seleniumbase/ Project-URL: Source, https://
```

### Comparing `seleniumbase-4.9.8/seleniumbase.egg-info/SOURCES.txt` & `seleniumbase-4.9.9/seleniumbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase.egg-info/entry_points.txt` & `seleniumbase-4.9.9/seleniumbase.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `seleniumbase-4.9.8/seleniumbase.egg-info/requires.txt` & `seleniumbase-4.9.9/seleniumbase.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 pytest-ordering==0.6
 parameterized==0.8.1
 sbvirtualdisplay==1.1.1
 behave==1.2.6
 parse==1.19.0
 parse-type==0.6.0
 tabcompleter==1.1.0
-pdbp==1.2.6
+pdbp==1.2.7
 pycparser==2.21
 cffi==1.15.1
 
 [:platform_system == "Windows" and python_version < "3.6"]
 pyreadline==2.1
 
 [:platform_system == "Windows" and python_version >= "3.6"]
```

### Comparing `seleniumbase-4.9.8/setup.py` & `seleniumbase-4.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         'cryptography==36.0.2;python_version>="3.6" and python_version<"3.7"',
         'cryptography==38.0.4;python_version>="3.7"',
         'pygments==2.5.2;python_version<"3.6"',
         'pygments==2.13.0;python_version>="3.6"',
         'pyreadline==2.1;platform_system=="Windows" and python_version<"3.6"',
         'pyreadline3==3.4.1;platform_system=="Windows" and python_version>="3.6"',  # noqa: E501
         "tabcompleter==1.1.0",
-        "pdbp==1.2.6",
+        "pdbp==1.2.7",
         'colorama==0.4.6;python_version<"3.6"',
         'colorama==0.4.5;python_version>="3.6" and python_version<"3.7"',
         'colorama==0.4.6;python_version>="3.7"',
         'exceptiongroup==1.0.4;python_version>="3.7"',
         'importlib-metadata==2.1.3;python_version<"3.6"',
         'importlib-metadata==4.2.0;python_version>="3.6" and python_version<"3.8"',  # noqa: E501
         "pycparser==2.21",
```

### Comparing `seleniumbase-4.9.8/virtualenv_install.sh` & `seleniumbase-4.9.9/virtualenv_install.sh`

 * *Files identical despite different names*

