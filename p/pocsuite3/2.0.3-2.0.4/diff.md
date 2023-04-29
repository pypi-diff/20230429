# Comparing `tmp/pocsuite3-2.0.3.tar.gz` & `tmp/pocsuite3-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocsuite3-2.0.3.tar", last modified: Tue Mar 21 06:23:14 2023, max compression
+gzip compressed data, was "pocsuite3-2.0.4.tar", last modified: Sat Apr 29 06:21:23 2023, max compression
```

## Comparing `pocsuite3-2.0.3.tar` & `pocsuite3-2.0.4.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.725285 pocsuite3-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-21 06:23:14.725285 pocsuite3-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.697285 pocsuite3-2.0.3/pocsuite3/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.697285 pocsuite3-2.0.3/pocsuite3/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.701285 pocsuite3-2.0.3/pocsuite3/data/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/data/password-top100.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.701285 pocsuite3-2.0.3/pocsuite3/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.701285 pocsuite3-2.0.3/pocsuite3/lib/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/controller/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.705285 pocsuite3-2.0.3/pocsuite3/lib/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/clear.py
--rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    22453 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/interpreter_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    25653 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/optiondict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    20155 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/poc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/readlineng.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/statistics_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/core/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.705285 pocsuite3-2.0.3/pocsuite3/lib/helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.705285 pocsuite3-2.0.3/pocsuite3/lib/helper/archieve/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/helper/archieve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/helper/archieve/jar.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/helper/archieve/memoryzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/helper/archieve/war.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/helper/archieve/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.705285 pocsuite3-2.0.3/pocsuite3/lib/helper/java/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/helper/java/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32903 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/helper/java/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.705285 pocsuite3-2.0.3/pocsuite3/lib/parse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/parse/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/parse/configfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/parse/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/parse/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.705285 pocsuite3-2.0.3/pocsuite3/lib/request/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.705285 pocsuite3-2.0.3/pocsuite3/lib/request/patch/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/request/patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/request/patch/add_httpraw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/request/patch/hook_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/request/patch/hook_request_redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/request/patch/hook_urllib3_parse_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/request/patch/remove_ssl_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/request/patch/remove_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/request/patch/unquote_request_uri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.705285 pocsuite3-2.0.3/pocsuite3/lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/utils/markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/utils/pcap_sniffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.705285 pocsuite3-2.0.3/pocsuite3/lib/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.705285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.705285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/operators/
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/operators/extrators/
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/operators/extrators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/operators/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/operators/matchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.693285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/
--rw-r--r--   0 runner    (1001) docker     (123)    22868 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/safe_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/interactsh/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/interactsh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/replacer/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/replacer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/http/
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/network/
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/modules/censys/
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/censys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/modules/ceye/
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/ceye/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/modules/fofa/
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/fofa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/modules/httpserver/
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/httpserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/modules/hunter/
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/hunter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/modules/interactsh/
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/interactsh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/modules/listener/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/listener/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/listener/bind_tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/listener/reverse_tcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/modules/quake/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/quake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/modules/seebug/
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/seebug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/modules/shodan/
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/shodan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/modules/spider/
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/spider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.709285 pocsuite3-2.0.3/pocsuite3/modules/zoomeye/
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/modules/zoomeye/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.713285 pocsuite3-2.0.3/pocsuite3/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/file_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/html_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/poc_from_pocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/poc_from_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/poc_from_seebug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/target_from_censys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/target_from_cidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/target_from_fofa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/target_from_hunter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/target_from_quake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/target_from_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/target_from_shodan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/plugins/target_from_zoomeye.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.717285 pocsuite3-2.0.3/pocsuite3/pocs/
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/20190404_WEB_Confluence_path_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/20210923_WEB_Vmware_vCenter_Server_FIleUpload_CVE-2021-22005.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/20211008_web_apache-httpd_dir-traversal-rce_cve-2021-41773_cve-2021-42013.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/demo_poc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/drupalgeddon2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/ecshop_rce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/ftp_burst.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/libssh_auth_bypass.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/node_red_unauthorized_rce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/redis_unauthorized_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/ssh_burst.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/telnet_burst.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/thinkphp_rce.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/thinkphp_rce2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/wd_nas_login_bypass_rce.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/pocs/weblogic_cve_2017_10271_unserialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.717285 pocsuite3-2.0.3/pocsuite3/shellcodes/
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.697285 pocsuite3-2.0.3/pocsuite3/shellcodes/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.697285 pocsuite3-2.0.3/pocsuite3/shellcodes/data/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.697285 pocsuite3-2.0.3/pocsuite3/shellcodes/data/java/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.717285 pocsuite3-2.0.3/pocsuite3/shellcodes/data/java/src/ReverseTCP/
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/java/src/ReverseTCP/Payload.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.717285 pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/bind_tcp.bin
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/reverse_tcp.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.717285 pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/src/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/src/bind_tcp.asm
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/src/reverse_tcp.asm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.717285 pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/x64/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/x64/bind_tcp.bin
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/x64/reverse_tcp.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.717285 pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/x64/src/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/x64/src/bind_tcp.asm
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/x64/src/reverse_tcp.asm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.721285 pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/bind_tcp.bin
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/reverse_tcp.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.721285 pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/src/bind_tcp.asm
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/src/reverse_tcp.asm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.721285 pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/x64/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/x64/bind_tcp.bin
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/x64/reverse_tcp.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.721285 pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/x64/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/x64/src/bind_tcp.asm
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/x64/src/reverse_tcp.asm
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/dotnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19194 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/php.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/pocsuite3/shellcodes/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.697285 pocsuite3-2.0.3/pocsuite3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-21 06:23:14.000000 pocsuite3-2.0.3/pocsuite3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-03-21 06:23:14.000000 pocsuite3-2.0.3/pocsuite3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 06:23:14.000000 pocsuite3-2.0.3/pocsuite3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-21 06:23:14.000000 pocsuite3-2.0.3/pocsuite3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 06:23:14.000000 pocsuite3-2.0.3/pocsuite3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-21 06:23:14.000000 pocsuite3-2.0.3/pocsuite3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-21 06:23:14.000000 pocsuite3-2.0.3/pocsuite3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-21 06:23:14.725285 pocsuite3-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:23:14.725285 pocsuite3-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/login_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_api_diy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_api_get_poc_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_build_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_check_install_requires.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_cmd_diy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_configfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_generate_shellcode_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_httpserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_import_pocsuite_execute.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_interactsh_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_nuclei_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_osshell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_parse_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_request_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_show_poc_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_spier_crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-21 06:22:49.000000 pocsuite3-2.0.3/tests/test_webshell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.575683 pocsuite3-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-29 06:21:23.575683 pocsuite3-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.547683 pocsuite3-2.0.4/pocsuite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.547683 pocsuite3-2.0.4/pocsuite3/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.547683 pocsuite3-2.0.4/pocsuite3/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/data/password-top100.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.547683 pocsuite3-2.0.4/pocsuite3/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.547683 pocsuite3-2.0.4/pocsuite3/lib/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/controller/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.551683 pocsuite3-2.0.4/pocsuite3/lib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22453 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/interpreter_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25653 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/optiondict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20155 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/poc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/readlineng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/statistics_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/core/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.551683 pocsuite3-2.0.4/pocsuite3/lib/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/memoryzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/war.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/helper/java/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32903 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/helper/java/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/parse/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/parse/configfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/parse/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/parse/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/request/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/request/patch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/add_httpraw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/hook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/hook_request_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/hook_urllib3_parse_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/remove_ssl_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/remove_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/request/patch/unquote_request_uri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/utils/markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/utils/pcap_sniffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.555683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/extrators/
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/extrators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/matchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.543683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)    22868 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/safe_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/interactsh/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/interactsh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/replacer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/http/
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/censys/
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/censys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/ceye/
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/ceye/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/fofa/
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/fofa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/httpserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/httpserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/hunter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/hunter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/interactsh/
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/interactsh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/listener/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/listener/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/listener/bind_tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/listener/reverse_tcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/quake/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/quake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/seebug/
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/seebug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/shodan/
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/shodan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.559683 pocsuite3-2.0.4/pocsuite3/modules/spider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/spider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.563683 pocsuite3-2.0.4/pocsuite3/modules/zoomeye/
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/modules/zoomeye/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.563683 pocsuite3-2.0.4/pocsuite3/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/file_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/html_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/poc_from_pocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/poc_from_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/poc_from_seebug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_censys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_cidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_fofa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_hunter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_quake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_shodan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/plugins/target_from_zoomeye.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/pocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/20190404_WEB_Confluence_path_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/20210923_WEB_Vmware_vCenter_Server_FIleUpload_CVE-2021-22005.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/20211008_web_apache-httpd_dir-traversal-rce_cve-2021-41773_cve-2021-42013.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/demo_poc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/drupalgeddon2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/ecshop_rce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/ftp_burst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/libssh_auth_bypass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/node_red_unauthorized_rce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/redis_unauthorized_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/ssh_burst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/telnet_burst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/thinkphp_rce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/thinkphp_rce2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/wd_nas_login_bypass_rce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/pocs/weblogic_cve_2017_10271_unserialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/shellcodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.543683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.543683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.543683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/java/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/java/src/ReverseTCP/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/java/src/ReverseTCP/Payload.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/bind_tcp.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/reverse_tcp.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/src/bind_tcp.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/src/reverse_tcp.asm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/bind_tcp.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/reverse_tcp.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.567683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/src/bind_tcp.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/src/reverse_tcp.asm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.571683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/bind_tcp.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/reverse_tcp.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.571683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/src/bind_tcp.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/src/reverse_tcp.asm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.571683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/bind_tcp.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/reverse_tcp.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.571683 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/src/bind_tcp.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/src/reverse_tcp.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/dotnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19194 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/php.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/pocsuite3/shellcodes/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.547683 pocsuite3-2.0.4/pocsuite3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 06:21:23.000000 pocsuite3-2.0.4/pocsuite3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-29 06:21:23.575683 pocsuite3-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:21:23.571683 pocsuite3-2.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/login_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_api_diy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_api_get_poc_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_build_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_check_install_requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_cmd_diy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_configfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_generate_shellcode_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_httpserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_import_pocsuite_execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_interactsh_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_nuclei_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_osshell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_parse_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_request_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_show_poc_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_spier_crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-29 06:20:59.000000 pocsuite3-2.0.4/tests/test_webshell.py
```

### Comparing `pocsuite3-2.0.3/CHANGELOG.md` & `pocsuite3-2.0.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# version 2.0.4
+----------------
+* Updated protocol names that are compatible with Nuclei v2.9.1
+
 # version 2.0.3
 ----------------
 * optimized URL protocol correction #356, thanks @chenjiewei123
 * support disable protocol correction and honeypot checks through --no-check option
 
 # version 2.0.2
 ----------------
```

### Comparing `pocsuite3-2.0.3/CONTRIBUTORS.md` & `pocsuite3-2.0.4/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/COPYING` & `pocsuite3-2.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/PKG-INFO` & `pocsuite3-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocsuite3
-Version: 2.0.3
+Version: 2.0.4
 Summary: Open-sourced remote vulnerability testing framework.
 Home-page: https://pocsuite.org
 Author: Knownsec 404 Team
 Author-email: 404-team@knownsec.com
 Maintainer: Knownsec 404 Team
 License: GPLv2
 Keywords: PoC,Exp,Pocsuite
```

### Comparing `pocsuite3-2.0.3/README.md` & `pocsuite3-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/api/__init__.py` & `pocsuite3-2.0.4/pocsuite3/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/cli.py` & `pocsuite3-2.0.4/pocsuite3/cli.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/console.py` & `pocsuite3-2.0.4/pocsuite3/console.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/data/password-top100.txt` & `pocsuite3-2.0.4/pocsuite3/data/password-top100.txt`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/controller/controller.py` & `pocsuite3-2.0.4/pocsuite3/lib/controller/controller.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/common.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/common.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/convert.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/convert.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/data.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/data.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/datatype.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/datatype.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/enums.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/enums.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/exception.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/exception.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/interpreter.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/interpreter.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/interpreter_option.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/interpreter_option.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/log.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/log.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/option.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/option.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/optiondict.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/optiondict.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/plugin.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/plugin.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/poc.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/poc.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/readlineng.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/readlineng.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/register.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/register.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/revision.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/revision.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/settings.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/settings.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/shell.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/shell.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/statistics_comparison.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/statistics_comparison.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/template.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/template.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/threads.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/threads.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/core/update.py` & `pocsuite3-2.0.4/pocsuite3/lib/core/update.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/helper/archieve/jar.py` & `pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/jar.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/helper/archieve/memoryzip.py` & `pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/memoryzip.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/helper/archieve/war.py` & `pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/war.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/helper/archieve/zip.py` & `pocsuite3-2.0.4/pocsuite3/lib/helper/archieve/zip.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/helper/java/serialization.py` & `pocsuite3-2.0.4/pocsuite3/lib/helper/java/serialization.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/parse/cmd.py` & `pocsuite3-2.0.4/pocsuite3/lib/parse/cmd.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/parse/configfile.py` & `pocsuite3-2.0.4/pocsuite3/lib/parse/configfile.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/parse/rules.py` & `pocsuite3-2.0.4/pocsuite3/lib/parse/rules.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/parse/url.py` & `pocsuite3-2.0.4/pocsuite3/lib/parse/url.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/request/patch/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/request/patch/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/request/patch/add_httpraw.py` & `pocsuite3-2.0.4/pocsuite3/lib/request/patch/add_httpraw.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/request/patch/hook_request.py` & `pocsuite3-2.0.4/pocsuite3/lib/request/patch/hook_request.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/request/patch/hook_request_redirect.py` & `pocsuite3-2.0.4/pocsuite3/lib/request/patch/hook_request_redirect.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/request/patch/hook_urllib3_parse_url.py` & `pocsuite3-2.0.4/pocsuite3/lib/request/patch/hook_urllib3_parse_url.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/request/patch/unquote_request_uri.py` & `pocsuite3-2.0.4/pocsuite3/lib/request/patch/unquote_request_uri.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/utils/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/utils/markup.py` & `pocsuite3-2.0.4/pocsuite3/lib/utils/markup.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/utils/pcap_sniffer.py` & `pocsuite3-2.0.4/pocsuite3/lib/utils/pcap_sniffer.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,24 @@
     def __init__(self, template, target=''):
         self.yaml_template = template
         try:
             self.yaml_template = binascii.unhexlify(self.yaml_template).decode()
         except ValueError:
             pass
         self.json_template = yaml.safe_load(expand_preprocessors(self.yaml_template))
+
+        # Breaking Changes in nuclei v2.9.1, Updated protocol attribute name (requests=> http & network => tcp)
+        # in templates, Templates with the use of requests and network will still work but will be deprecated
+        # completely in the future.
+
+        if 'http' in self.json_template:
+            self.json_template['requests'] = self.json_template['http']
+        if 'tcp' in self.json_template:
+            self.json_template['network'] = self.json_template['tcp']
+
         self.template = dacite.from_dict(
             Template, hyphen_to_underscore(self.json_template),
             config=dacite.Config(cast=[Severify, ExtractorType, MatcherType, HTTPMethod, AttackType, NetworkInputType]))
 
         self.target = target
         self.interactsh = None
         self.dynamic_values = OrderedDict()
```

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/model/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/operators/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/operators/extrators/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/extrators/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/operators/matchers/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/operators/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/safe_eval.py` & `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/expressions/safe_eval.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/generators/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/interactsh/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/interactsh/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/common/replacer/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/common/replacer/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/http/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/http/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/protocols/network/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/protocols/network/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/lib/yaml/nuclei/templates/__init__.py` & `pocsuite3-2.0.4/pocsuite3/lib/yaml/nuclei/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/modules/censys/__init__.py` & `pocsuite3-2.0.4/pocsuite3/modules/censys/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/modules/ceye/__init__.py` & `pocsuite3-2.0.4/pocsuite3/modules/ceye/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/modules/fofa/__init__.py` & `pocsuite3-2.0.4/pocsuite3/modules/fofa/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/modules/httpserver/__init__.py` & `pocsuite3-2.0.4/pocsuite3/modules/httpserver/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/modules/hunter/__init__.py` & `pocsuite3-2.0.4/pocsuite3/modules/hunter/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/modules/interactsh/__init__.py` & `pocsuite3-2.0.4/pocsuite3/modules/interactsh/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/modules/listener/bind_tcp.py` & `pocsuite3-2.0.4/pocsuite3/modules/listener/bind_tcp.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/modules/listener/reverse_tcp.py` & `pocsuite3-2.0.4/pocsuite3/modules/listener/reverse_tcp.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/modules/quake/__init__.py` & `pocsuite3-2.0.4/pocsuite3/modules/quake/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/modules/seebug/__init__.py` & `pocsuite3-2.0.4/pocsuite3/modules/seebug/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/modules/shodan/__init__.py` & `pocsuite3-2.0.4/pocsuite3/modules/shodan/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/modules/spider/__init__.py` & `pocsuite3-2.0.4/pocsuite3/modules/spider/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/modules/zoomeye/__init__.py` & `pocsuite3-2.0.4/pocsuite3/modules/zoomeye/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/plugins/file_record.py` & `pocsuite3-2.0.4/pocsuite3/plugins/file_record.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/plugins/html_report.py` & `pocsuite3-2.0.4/pocsuite3/plugins/html_report.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/plugins/poc_from_pocs.py` & `pocsuite3-2.0.4/pocsuite3/plugins/poc_from_pocs.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/plugins/poc_from_redis.py` & `pocsuite3-2.0.4/pocsuite3/plugins/poc_from_redis.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/plugins/poc_from_seebug.py` & `pocsuite3-2.0.4/pocsuite3/plugins/poc_from_seebug.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/plugins/target_from_censys.py` & `pocsuite3-2.0.4/pocsuite3/plugins/target_from_censys.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/plugins/target_from_cidr.py` & `pocsuite3-2.0.4/pocsuite3/plugins/target_from_cidr.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/plugins/target_from_fofa.py` & `pocsuite3-2.0.4/pocsuite3/plugins/target_from_fofa.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/plugins/target_from_hunter.py` & `pocsuite3-2.0.4/pocsuite3/plugins/target_from_hunter.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/plugins/target_from_quake.py` & `pocsuite3-2.0.4/pocsuite3/plugins/target_from_quake.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/plugins/target_from_redis.py` & `pocsuite3-2.0.4/pocsuite3/plugins/target_from_redis.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/plugins/target_from_shodan.py` & `pocsuite3-2.0.4/pocsuite3/plugins/target_from_shodan.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/plugins/target_from_zoomeye.py` & `pocsuite3-2.0.4/pocsuite3/plugins/target_from_zoomeye.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/20190404_WEB_Confluence_path_traversal.py` & `pocsuite3-2.0.4/pocsuite3/pocs/20190404_WEB_Confluence_path_traversal.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/20210923_WEB_Vmware_vCenter_Server_FIleUpload_CVE-2021-22005.py` & `pocsuite3-2.0.4/pocsuite3/pocs/20210923_WEB_Vmware_vCenter_Server_FIleUpload_CVE-2021-22005.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/20211008_web_apache-httpd_dir-traversal-rce_cve-2021-41773_cve-2021-42013.py` & `pocsuite3-2.0.4/pocsuite3/pocs/20211008_web_apache-httpd_dir-traversal-rce_cve-2021-41773_cve-2021-42013.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/demo_poc.py` & `pocsuite3-2.0.4/pocsuite3/pocs/demo_poc.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/drupalgeddon2.py` & `pocsuite3-2.0.4/pocsuite3/pocs/drupalgeddon2.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/ecshop_rce.py` & `pocsuite3-2.0.4/pocsuite3/pocs/ecshop_rce.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/ftp_burst.py` & `pocsuite3-2.0.4/pocsuite3/pocs/ftp_burst.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/libssh_auth_bypass.py` & `pocsuite3-2.0.4/pocsuite3/pocs/libssh_auth_bypass.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/node_red_unauthorized_rce.py` & `pocsuite3-2.0.4/pocsuite3/pocs/node_red_unauthorized_rce.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/redis_unauthorized_access.py` & `pocsuite3-2.0.4/pocsuite3/pocs/redis_unauthorized_access.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/ssh_burst.py` & `pocsuite3-2.0.4/pocsuite3/pocs/ssh_burst.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/telnet_burst.py` & `pocsuite3-2.0.4/pocsuite3/pocs/telnet_burst.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/thinkphp_rce.py` & `pocsuite3-2.0.4/pocsuite3/pocs/thinkphp_rce.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/thinkphp_rce2.py` & `pocsuite3-2.0.4/pocsuite3/pocs/thinkphp_rce2.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/wd_nas_login_bypass_rce.py` & `pocsuite3-2.0.4/pocsuite3/pocs/wd_nas_login_bypass_rce.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/pocs/weblogic_cve_2017_10271_unserialization.py` & `pocsuite3-2.0.4/pocsuite3/pocs/weblogic_cve_2017_10271_unserialization.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/__init__.py` & `pocsuite3-2.0.4/pocsuite3/shellcodes/__init__.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/base.py` & `pocsuite3-2.0.4/pocsuite3/shellcodes/base.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/data/java/src/ReverseTCP/Payload.java` & `pocsuite3-2.0.4/pocsuite3/shellcodes/data/java/src/ReverseTCP/Payload.java`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/src/bind_tcp.asm` & `pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/src/bind_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/src/reverse_tcp.asm` & `pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/src/reverse_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/x64/src/bind_tcp.asm` & `pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/src/bind_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/data/linux/x64/src/reverse_tcp.asm` & `pocsuite3-2.0.4/pocsuite3/shellcodes/data/linux/x64/src/reverse_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/bind_tcp.bin` & `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/bind_tcp.bin`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/reverse_tcp.bin` & `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/reverse_tcp.bin`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/src/bind_tcp.asm` & `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/src/bind_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/src/reverse_tcp.asm` & `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/src/reverse_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/x64/bind_tcp.bin` & `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/bind_tcp.bin`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/x64/reverse_tcp.bin` & `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/reverse_tcp.bin`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/x64/src/bind_tcp.asm` & `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/src/bind_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/data/windows/x64/src/reverse_tcp.asm` & `pocsuite3-2.0.4/pocsuite3/shellcodes/data/windows/x64/src/reverse_tcp.asm`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/dotnet.py` & `pocsuite3-2.0.4/pocsuite3/shellcodes/dotnet.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/encoder.py` & `pocsuite3-2.0.4/pocsuite3/shellcodes/encoder.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/generator.py` & `pocsuite3-2.0.4/pocsuite3/shellcodes/generator.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/java.py` & `pocsuite3-2.0.4/pocsuite3/shellcodes/java.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/php.py` & `pocsuite3-2.0.4/pocsuite3/shellcodes/php.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3/shellcodes/python.py` & `pocsuite3-2.0.4/pocsuite3/shellcodes/python.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/pocsuite3.egg-info/PKG-INFO` & `pocsuite3-2.0.4/pocsuite3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocsuite3
-Version: 2.0.3
+Version: 2.0.4
 Summary: Open-sourced remote vulnerability testing framework.
 Home-page: https://pocsuite.org
 Author: Knownsec 404 Team
 Author-email: 404-team@knownsec.com
 Maintainer: Knownsec 404 Team
 License: GPLv2
 Keywords: PoC,Exp,Pocsuite
```

### Comparing `pocsuite3-2.0.3/pocsuite3.egg-info/SOURCES.txt` & `pocsuite3-2.0.4/pocsuite3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/setup.py` & `pocsuite3-2.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'developed by the Knownsec 404 Team. It comes with a powerful proof-of-concept engine, many nice '
     'features for the ultimate penetration testers and security researchers.'
 )
 
 
 setup(
     name='pocsuite3',
-    version='2.0.3',
+    version='2.0.4',
     url='https://pocsuite.org',
     description='Open-sourced remote vulnerability testing framework.',
     long_description=long_description,
     keywords='PoC,Exp,Pocsuite',
     author='Knownsec 404 Team',
     author_email='404-team@knownsec.com',
     maintainer='Knownsec 404 Team',
```

### Comparing `pocsuite3-2.0.3/tests/login_demo.py` & `pocsuite3-2.0.4/tests/login_demo.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_api_diy_options.py` & `pocsuite3-2.0.4/tests/test_api_diy_options.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_api_get_poc_info.py` & `pocsuite3-2.0.4/tests/test_api_get_poc_info.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_build_url.py` & `pocsuite3-2.0.4/tests/test_build_url.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_check_install_requires.py` & `pocsuite3-2.0.4/tests/test_check_install_requires.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_cmd_diy_options.py` & `pocsuite3-2.0.4/tests/test_cmd_diy_options.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_configfile.py` & `pocsuite3-2.0.4/tests/test_configfile.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_generate_shellcode_list.py` & `pocsuite3-2.0.4/tests/test_generate_shellcode_list.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_httpserver.py` & `pocsuite3-2.0.4/tests/test_httpserver.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_import_pocsuite_execute.py` & `pocsuite3-2.0.4/tests/test_import_pocsuite_execute.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_interactsh_module.py` & `pocsuite3-2.0.4/tests/test_interactsh_module.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_nuclei_helper_functions.py` & `pocsuite3-2.0.4/tests/test_nuclei_helper_functions.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_osshell.py` & `pocsuite3-2.0.4/tests/test_osshell.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_parse_target.py` & `pocsuite3-2.0.4/tests/test_parse_target.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_request_raw.py` & `pocsuite3-2.0.4/tests/test_request_raw.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_spier_crawl.py` & `pocsuite3-2.0.4/tests/test_spier_crawl.py`

 * *Files identical despite different names*

### Comparing `pocsuite3-2.0.3/tests/test_webshell.py` & `pocsuite3-2.0.4/tests/test_webshell.py`

 * *Files identical despite different names*

