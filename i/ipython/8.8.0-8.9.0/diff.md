# Comparing `tmp/ipython-8.8.0.tar.gz` & `tmp/ipython-8.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Jan  3 14:03:24 2023, max compression
+gzip compressed data, last modified: Fri Jan 27 11:56:59 2023, max compression
```

## Comparing `ipython-8.8.0.tar` & `ipython-8.9.0.tar`

### file list

```diff
@@ -1,549 +1,554 @@
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/
--rw-r--r--   0        0        0      143 2023-01-03 13:18:33.000000 ipython-8.8.0/.flake8
--rw-r--r--   0        0        0    12671 2023-01-03 13:18:33.000000 ipython-8.8.0/.mailmap
--rw-r--r--   0        0        0      409 2023-01-03 13:18:33.000000 ipython-8.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1639 2023-01-03 13:18:33.000000 ipython-8.8.0/COPYING.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/
--rw-r--r--   0        0        0     5962 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/__init__.py
--rw-r--r--   0        0        0      488 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/__main__.py
--rw-r--r--   0        0        0     2618 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/conftest.py
--rw-r--r--   0        0        0      415 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/consoleapp.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/core/
--rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/core/__init__.py
--rw-r--r--   0        0        0    10034 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/alias.py
--rw-r--r--   0        0        0    18953 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/application.py
--rw-r--r--   0        0        0     4297 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/async_helpers.py
--rw-r--r--   0        0        0     1991 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/autocall.py
--rw-r--r--   0        0        0     3009 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/builtin_trap.py
--rw-r--r--   0        0        0     7730 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/compilerop.py
--rw-r--r--   0        0        0   116855 2023-01-03 13:26:22.000000 ipython-8.8.0/IPython/core/completer.py
--rw-r--r--   0        0        0    12259 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/completerlib.py
--rw-r--r--   0        0        0     8508 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/crashhandler.py
--rw-r--r--   0        0        0    33382 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/debugger.py
--rw-r--r--   0        0        0    42476 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/display.py
--rw-r--r--   0        0        0    12918 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/display_functions.py
--rw-r--r--   0        0        0     2098 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/core/display_trap.py
--rw-r--r--   0        0        0    12608 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/displayhook.py
--rw-r--r--   0        0        0     4944 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/displaypub.py
--rw-r--r--   0        0        0     1734 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/core/error.py
--rw-r--r--   0        0        0     5349 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/events.py
--rw-r--r--   0        0        0     4928 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/excolors.py
--rw-r--r--   0        0        0     5780 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/extensions.py
--rw-r--r--   0        0        0    34952 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/formatters.py
--rw-r--r--   0        0        0      912 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/getipython.py
--rw-r--r--   0        0        0    24054 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/guarded_eval.py
--rw-r--r--   0        0        0    34174 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/history.py
--rw-r--r--   0        0        0     5909 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/historyapp.py
--rw-r--r--   0        0        0     5663 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/hooks.py
--rw-r--r--   0        0        0    28119 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/inputsplitter.py
--rw-r--r--   0        0        0    17942 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/inputtransformer.py
--rw-r--r--   0        0        0    28374 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/inputtransformer2.py
--rw-r--r--   0        0        0   150371 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/interactiveshell.py
--rw-r--r--   0        0        0    31288 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/latex_symbols.py
--rw-r--r--   0        0        0     7930 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/logger.py
--rw-r--r--   0        0        0     1734 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/macro.py
--rw-r--r--   0        0        0    28478 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magic.py
--rw-r--r--   0        0        0     9736 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magic_arguments.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/core/magics/
--rw-r--r--   0        0        0     1619 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/__init__.py
--rw-r--r--   0        0        0     4816 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/auto.py
--rw-r--r--   0        0        0    22932 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/basic.py
--rw-r--r--   0        0        0    28051 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/code.py
--rw-r--r--   0        0        0     4881 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/config.py
--rw-r--r--   0        0        0     3130 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/display.py
--rw-r--r--   0        0        0    57843 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/execution.py
--rw-r--r--   0        0        0     2477 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/extension.py
--rw-r--r--   0        0        0    12628 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/history.py
--rw-r--r--   0        0        0     6859 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/logging.py
--rw-r--r--   0        0        0    24823 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/namespace.py
--rw-r--r--   0        0        0    30681 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/osm.py
--rw-r--r--   0        0        0     3916 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/packaging.py
--rw-r--r--   0        0        0     6574 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/pylab.py
--rw-r--r--   0        0        0    12173 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/magics/script.py
--rw-r--r--   0        0        0    37073 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/oinspect.py
--rw-r--r--   0        0        0    11753 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/page.py
--rw-r--r--   0        0        0     1758 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/core/payload.py
--rw-r--r--   0        0        0     1431 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/payloadpage.py
--rw-r--r--   0        0        0    25583 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/prefilter.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/core/profile/
--rw-r--r--   0        0        0      371 2021-11-27 18:00:22.000000 ipython-8.8.0/IPython/core/profile/README_STARTUP
--rw-r--r--   0        0        0    10631 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/profileapp.py
--rw-r--r--   0        0        0     8029 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/profiledir.py
--rw-r--r--   0        0        0      607 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/prompts.py
--rw-r--r--   0        0        0    13809 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/pylabtools.py
--rw-r--r--   0        0        0     2177 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/core/release.py
--rw-r--r--   0        0        0    17846 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/shellapp.py
--rw-r--r--   0        0        0     4787 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/splitinput.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/core/tests/
--rw-r--r--   0        0        0      331 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/core/tests/2x2.jpg
--rw-r--r--   0        0        0       71 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/core/tests/2x2.png
--rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/core/tests/__init__.py
--rw-r--r--   0        0        0      206 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/core/tests/bad_all.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/core/tests/daft_extension/
--rw-r--r--   0        0        0      285 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/core/tests/daft_extension/daft_extension.py
--rw-r--r--   0        0        0      135 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/nonascii.py
--rw-r--r--   0        0        0      155 2022-10-29 11:03:53.000000 ipython-8.8.0/IPython/core/tests/nonascii2.py
--rw-r--r--   0        0        0       32 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/print_argv.py
--rw-r--r--   0        0        0     1494 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/refbug.py
--rw-r--r--   0        0        0      583 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/simpleerr.py
--rw-r--r--   0        0        0      921 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/tclass.py
--rw-r--r--   0        0        0     2007 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_alias.py
--rw-r--r--   0        0        0     2245 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_application.py
--rw-r--r--   0        0        0     8769 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_async_helpers.py
--rw-r--r--   0        0        0     1425 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_autocall.py
--rw-r--r--   0        0        0     2174 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_compilerop.py
--rw-r--r--   0        0        0    60333 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_completer.py
--rw-r--r--   0        0        0     6473 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_completerlib.py
--rw-r--r--   0        0        0    14502 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_debugger.py
--rw-r--r--   0        0        0    15946 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_display.py
--rw-r--r--   0        0        0     3593 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_displayhook.py
--rw-r--r--   0        0        0     2799 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_events.py
--rw-r--r--   0        0        0     3026 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_extension.py
--rw-r--r--   0        0        0    14249 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_formatters.py
--rw-r--r--   0        0        0    14853 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_guarded_eval.py
--rw-r--r--   0        0        0     3286 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_handlers.py
--rw-r--r--   0        0        0    11698 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_history.py
--rw-r--r--   0        0        0     2316 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_hooks.py
--rw-r--r--   0        0        0     1153 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_imports.py
--rw-r--r--   0        0        0    23159 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_inputsplitter.py
--rw-r--r--   0        0        0    15755 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_inputtransformer.py
--rw-r--r--   0        0        0    11263 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_inputtransformer2.py
--rw-r--r--   0        0        0     2971 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_inputtransformer2_line.py
--rw-r--r--   0        0        0    37182 2023-01-03 13:59:11.000000 ipython-8.8.0/IPython/core/tests/test_interactiveshell.py
--rw-r--r--   0        0        0     8470 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_iplib.py
--rw-r--r--   0        0        0      776 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_logger.py
--rw-r--r--   0        0        0    40984 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_magic.py
--rw-r--r--   0        0        0     4778 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_magic_arguments.py
--rw-r--r--   0        0        0     5996 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_magic_terminal.py
--rw-r--r--   0        0        0    14809 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_oinspect.py
--rw-r--r--   0        0        0      772 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/core/tests/test_page.py
--rw-r--r--   0        0        0     7081 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_paths.py
--rw-r--r--   0        0        0     4214 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_prefilter.py
--rw-r--r--   0        0        0     5064 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_profile.py
--rw-r--r--   0        0        0      845 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_prompts.py
--rw-r--r--   0        0        0     7883 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_pylabtools.py
--rw-r--r--   0        0        0    19369 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_run.py
--rw-r--r--   0        0        0     1892 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_shellapp.py
--rw-r--r--   0        0        0     1227 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_splitinput.py
--rw-r--r--   0        0        0    11495 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/tests/test_ultratb.py
--rw-r--r--   0        0        0    46165 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/ultratb.py
--rw-r--r--   0        0        0    13542 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/core/usage.py
--rw-r--r--   0        0        0     1119 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/display.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/extensions/
--rw-r--r--   0        0        0       78 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/extensions/__init__.py
--rw-r--r--   0        0        0    19741 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/extensions/autoreload.py
--rw-r--r--   0        0        0     8161 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/extensions/storemagic.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/extensions/tests/
--rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/extensions/tests/__init__.py
--rw-r--r--   0        0        0    18691 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/extensions/tests/test_autoreload.py
--rw-r--r--   0        0        0     2081 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/extensions/tests/test_storemagic.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/external/
--rw-r--r--   0        0        0      126 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/external/__init__.py
--rw-r--r--   0        0        0     3445 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/external/qt_for_kernel.py
--rw-r--r--   0        0        0    11158 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/external/qt_loaders.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/external/tests/
--rw-r--r--   0        0        0        0 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/external/tests/__init__.py
--rw-r--r--   0        0        0      367 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/external/tests/test_qt_loaders.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/lib/
--rw-r--r--   0        0        0      409 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/__init__.py
--rw-r--r--   0        0        0    17738 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/backgroundjobs.py
--rw-r--r--   0        0        0     3050 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/clipboard.py
--rw-r--r--   0        0        0     9431 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/deepreload.py
--rw-r--r--   0        0        0    24518 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/demo.py
--rw-r--r--   0        0        0    24532 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/display.py
--rw-r--r--   0        0        0     3982 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/editorhooks.py
--rw-r--r--   0        0        0     6305 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/guisupport.py
--rw-r--r--   0        0        0     8299 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/latextools.py
--rw-r--r--   0        0        0    20218 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/lexers.py
--rw-r--r--   0        0        0    30872 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/pretty.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/lib/tests/
--rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/lib/tests/__init__.py
--rw-r--r--   0        0        0    44144 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/lib/tests/test.wav
--rw-r--r--   0        0        0     2698 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/tests/test_backgroundjobs.py
--rw-r--r--   0        0        0      630 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/tests/test_clipboard.py
--rw-r--r--   0        0        0     1854 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/tests/test_deepreload.py
--rw-r--r--   0        0        0     9313 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/tests/test_display.py
--rw-r--r--   0        0        0      884 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/tests/test_editorhooks.py
--rw-r--r--   0        0        0      273 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/tests/test_imports.py
--rw-r--r--   0        0        0     5736 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/tests/test_latextools.py
--rw-r--r--   0        0        0     6017 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/tests/test_lexers.py
--rw-r--r--   0        0        0    14830 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/tests/test_pretty.py
--rw-r--r--   0        0        0      824 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/lib/tests/test_pygments.py
--rw-r--r--   0        0        0     4335 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/paths.py
--rw-r--r--   0        0        0        0 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/py.typed
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/sphinxext/
--rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/sphinxext/__init__.py
--rw-r--r--   0        0        0     4615 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/sphinxext/custom_doctests.py
--rw-r--r--   0        0        0      970 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/sphinxext/ipython_console_highlighting.py
--rw-r--r--   0        0        0    45069 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/sphinxext/ipython_directive.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/terminal/
--rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/terminal/__init__.py
--rw-r--r--   0        0        0      691 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/terminal/console.py
--rw-r--r--   0        0        0     6618 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/debugger.py
--rw-r--r--   0        0        0    15220 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/embed.py
--rw-r--r--   0        0        0    28312 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/interactiveshell.py
--rwxr-xr-x   0        0        0    12351 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/ipapp.py
--rw-r--r--   0        0        0     7705 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/magics.py
--rw-r--r--   0        0        0     3360 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/prompts.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/terminal/pt_inputhooks/
--rw-r--r--   0        0        0     1266 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/pt_inputhooks/__init__.py
--rw-r--r--   0        0        0     1844 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/pt_inputhooks/asyncio.py
--rw-r--r--   0        0        0     4997 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/pt_inputhooks/glut.py
--rw-r--r--   0        0        0     2427 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/pt_inputhooks/gtk.py
--rw-r--r--   0        0        0      280 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/pt_inputhooks/gtk3.py
--rw-r--r--   0        0        0      557 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/pt_inputhooks/gtk4.py
--rw-r--r--   0        0        0     4789 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/pt_inputhooks/osx.py
--rw-r--r--   0        0        0     2368 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/pt_inputhooks/pyglet.py
--rw-r--r--   0        0        0     3206 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/pt_inputhooks/qt.py
--rw-r--r--   0        0        0     3648 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/pt_inputhooks/tk.py
--rw-r--r--   0        0        0     7132 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/pt_inputhooks/wx.py
--rw-r--r--   0        0        0     7481 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/ptutils.py
--rw-r--r--   0        0        0    19041 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/shortcuts.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/terminal/tests/
--rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/terminal/tests/__init__.py
--rw-r--r--   0        0        0     2375 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/tests/test_debug_magic.py
--rw-r--r--   0        0        0     4804 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/tests/test_embed.py
--rw-r--r--   0        0        0      722 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/tests/test_help.py
--rw-r--r--   0        0        0     7749 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/terminal/tests/test_interactivshell.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/testing/
--rw-r--r--   0        0        0      784 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/__init__.py
--rw-r--r--   0        0        0     6777 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/decorators.py
--rw-r--r--   0        0        0     3948 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/globalipapp.py
--rw-r--r--   0        0        0     6540 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/ipunittest.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/testing/plugin/
--rw-r--r--   0        0        0     1437 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/plugin/Makefile
--rw-r--r--   0        0        0     1043 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/plugin/README.txt
--rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/testing/plugin/__init__.py
--rw-r--r--   0        0        0     2921 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/plugin/dtexample.py
--rw-r--r--   0        0        0    11881 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/plugin/ipdoctest.py
--rw-r--r--   0        0        0    29690 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/plugin/pytest_ipdoctest.py
--rwxr-xr-x   0        0        0      539 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/testing/plugin/setup.py
--rw-r--r--   0        0        0      727 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/plugin/simple.py
--rw-r--r--   0        0        0       24 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/plugin/simplevars.py
--rw-r--r--   0        0        0      923 2022-03-19 09:18:04.000000 ipython-8.8.0/IPython/testing/plugin/test_combo.txt
--rw-r--r--   0        0        0      730 2022-03-19 09:18:04.000000 ipython-8.8.0/IPython/testing/plugin/test_example.txt
--rw-r--r--   0        0        0      814 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/plugin/test_exampleip.txt
--rw-r--r--   0        0        0     1907 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/plugin/test_ipdoctest.py
--rw-r--r--   0        0        0      715 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/plugin/test_refs.py
--rw-r--r--   0        0        0      717 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/skipdoctest.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/testing/tests/
--rw-r--r--   0        0        0      558 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/testing/tests/__init__.py
--rw-r--r--   0        0        0     3955 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/tests/test_decorators.py
--rw-r--r--   0        0        0     3301 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/tests/test_ipunittest.py
--rw-r--r--   0        0        0     4157 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/tests/test_tools.py
--rw-r--r--   0        0        0    14105 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/testing/tools.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/tests/
--rw-r--r--   0        0        0     2000 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/tests/cve.py
--rw-r--r--   0        0        0     1302 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/tests/test_shortcuts.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/utils/
--rw-r--r--   0        0        0    10875 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/PyColorize.py
--rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/utils/__init__.py
--rw-r--r--   0        0        0     2020 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/_process_cli.py
--rw-r--r--   0        0        0     7003 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/_process_common.py
--rw-r--r--   0        0        0     8666 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/_process_posix.py
--rw-r--r--   0        0        0     6132 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/_process_win32.py
--rw-r--r--   0        0        0    21329 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/_process_win32_controller.py
--rw-r--r--   0        0        0       45 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/utils/_sysinfo.py
--rw-r--r--   0        0        0     5161 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/capture.py
--rw-r--r--   0        0        0      786 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/colorable.py
--rw-r--r--   0        0        0     6972 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/coloransi.py
--rw-r--r--   0        0        0     1619 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/contexts.py
--rw-r--r--   0        0        0      200 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/daemonize.py
--rw-r--r--   0        0        0     1015 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/data.py
--rw-r--r--   0        0        0     2680 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/decorators.py
--rw-r--r--   0        0        0     2232 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/dir2.py
--rw-r--r--   0        0        0       86 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/docs.py
--rw-r--r--   0        0        0     2843 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/encoding.py
--rw-r--r--   0        0        0      138 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/eventful.py
--rw-r--r--   0        0        0     3048 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/frame.py
--rw-r--r--   0        0        0      706 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/generics.py
--rw-r--r--   0        0        0     1050 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/importstring.py
--rw-r--r--   0        0        0     4777 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/io.py
--rw-r--r--   0        0        0    11856 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/ipstruct.py
--rw-r--r--   0        0        0      148 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/jsonutil.py
--rw-r--r--   0        0        0      169 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/localinterfaces.py
--rw-r--r--   0        0        0      123 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/log.py
--rw-r--r--   0        0        0     2329 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/module_paths.py
--rw-r--r--   0        0        0     3417 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/openpy.py
--rw-r--r--   0        0        0    11937 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/path.py
--rw-r--r--   0        0        0     1878 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/process.py
--rw-r--r--   0        0        0     1601 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/py3compat.py
--rw-r--r--   0        0        0      421 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/utils/sentinel.py
--rw-r--r--   0        0        0     2669 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/shimmodule.py
--rw-r--r--   0        0        0      474 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/signatures.py
--rw-r--r--   0        0        0     1838 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/utils/strdispatch.py
--rw-r--r--   0        0        0     4324 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/sysinfo.py
--rw-r--r--   0        0        0     1952 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/syspathcontext.py
--rw-r--r--   0        0        0     1867 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tempdir.py
--rw-r--r--   0        0        0     3793 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/terminal.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/IPython/utils/tests/
--rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.8.0/IPython/utils/tests/__init__.py
--rw-r--r--   0        0        0     5319 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_capture.py
--rw-r--r--   0        0        0      170 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/utils/tests/test_decorators.py
--rw-r--r--   0        0        0      183 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_deprecated.py
--rw-r--r--   0        0        0     1446 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_dir2.py
--rw-r--r--   0        0        0      439 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_imports.py
--rw-r--r--   0        0        0     1213 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_importstring.py
--rw-r--r--   0        0        0     1410 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_io.py
--rw-r--r--   0        0        0     3272 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_module_paths.py
--rw-r--r--   0        0        0     1219 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_openpy.py
--rw-r--r--   0        0        0    16104 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_path.py
--rw-r--r--   0        0        0     6134 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_process.py
--rw-r--r--   0        0        0     1711 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_pycolorize.py
--rw-r--r--   0        0        0      387 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_shimmodule.py
--rw-r--r--   0        0        0      464 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_sysinfo.py
--rw-r--r--   0        0        0     1108 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_tempdir.py
--rw-r--r--   0        0        0     7114 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_text.py
--rw-r--r--   0        0        0     3918 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tests/test_tokenutil.py
--rw-r--r--   0        0        0     4729 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/utils/tests/test_wildcard.py
--rw-r--r--   0        0        0    22794 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/text.py
--rw-r--r--   0        0        0     4238 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/timing.py
--rw-r--r--   0        0        0     3928 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/tokenutil.py
--rw-r--r--   0        0        0      143 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/traitlets.py
--rw-r--r--   0        0        0     1352 2022-10-29 11:02:00.000000 ipython-8.8.0/IPython/utils/tz.py
--rw-r--r--   0        0        0      684 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/ulinecache.py
--rw-r--r--   0        0        0     1223 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/version.py
--rw-r--r--   0        0        0     4612 2023-01-03 13:18:33.000000 ipython-8.8.0/IPython/utils/wildcard.py
--rw-r--r--   0        0        0     1720 2023-01-03 13:18:33.000000 ipython-8.8.0/LICENSE
--rw-r--r--   0        0        0      882 2023-01-03 13:18:33.000000 ipython-8.8.0/MANIFEST.in
--rw-r--r--   0        0        0     2706 2023-01-03 14:03:24.000000 ipython-8.8.0/PKG-INFO
--rw-r--r--   0        0        0     6477 2023-01-03 13:18:33.000000 ipython-8.8.0/README.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/
--rw-r--r--   0        0        0     4774 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/Makefile
--rw-r--r--   0        0        0     1873 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/README.rst
--rwxr-xr-x   0        0        0     2934 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/autogen_api.py
--rwxr-xr-x   0        0        0     4196 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/autogen_config.py
--rw-r--r--   0        0        0     1998 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/autogen_magics.py
--rwxr-xr-x   0        0        0     2679 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/autogen_shortcuts.py
--rw-r--r--   0        0        0     2685 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/make.cmd
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/man/
--rw-r--r--   0        0        0     2058 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/man/ipython.1
--rw-r--r--   0        0        0       10 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/requirements.txt
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/_images/
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/_images/2.0/
--rw-r--r--   0        0        0   113866 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/_images/2.0/running-crop.png
--rw-r--r--   0        0        0   122393 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/_images/2.0/running.png
--rw-r--r--   0        0        0   134168 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/_images/2.0/treeview.png
--rw-r--r--   0        0        0   284971 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/_images/2.0/user-interface.png
--rw-r--r--   0        0        0   222518 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/_images/2.0/widgets.png
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/_images/8.0/
--rw-r--r--   0        0        0     6225 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_images/8.0/auto_suggest_1_prompt_no_text.png
--rw-r--r--   0        0        0    13654 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_images/8.0/auto_suggest_2_print_hello_suggest.png
--rw-r--r--   0        0        0    16308 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_images/8.0/auto_suggest_3_print_hello_suggest.png
--rw-r--r--   0        0        0    17190 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_images/8.0/auto_suggest_4_print_hello.png
--rw-r--r--   0        0        0    14362 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_images/8.0/auto_suggest_d_completions.png
--rw-r--r--   0        0        0     4731 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_images/8.0/auto_suggest_d_phantom.png
--rw-r--r--   0        0        0    17497 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_images/8.0/auto_suggest_def_completions.png
--rw-r--r--   0        0        0     4947 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_images/8.0/auto_suggest_def_phantom.png
--rw-r--r--   0        0        0     6603 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_images/8.0/auto_suggest_match_parens.png
--rw-r--r--   0        0        0     7602 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_images/8.0/auto_suggest_second_prompt.png
--rw-r--r--   0        0        0    77651 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_images/8.0/pathlib_pathlib_everywhere.jpg
--rw-r--r--   0        0        0    38090 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/ipy_013_dashboard.png
--rw-r--r--   0        0        0    41133 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/ipy_013_dashboard_cluster.png
--rw-r--r--   0        0        0    76125 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/ipy_013_notebook_cythonmagic.png
--rw-r--r--   0        0        0    18803 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/ipy_013_notebook_long_out.png
--rw-r--r--   0        0        0   274282 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/ipy_013_notebook_octavemagic.png
--rw-r--r--   0        0        0   132820 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/ipy_013_notebook_rmagic.png
--rw-r--r--   0        0        0    17912 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/ipy_013_notebook_script_cells.png
--rw-r--r--   0        0        0   355455 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/ipy_013_notebook_spectrogram.png
--rw-r--r--   0        0        0   136934 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/ipy_013_notebook_tooltip.png
--rw-r--r--   0        0        0    30116 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/ipy_013_par_tb.png
--rw-r--r--   0        0        0   162832 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/ipy_013_qtconsole_baboon.png
--rw-r--r--   0        0        0    28262 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/ipy_013_qtconsole_completer.png
--rw-r--r--   0        0        0    55988 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_images/ipython-6-screenshot.png
--rw-r--r--   0        0        0    59846 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_images/jedi_type_inference_60.png
--rw-r--r--   0        0        0     9693 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/_images/kernel_selector_screenshot.png
--rw-r--r--   0        0        0   117077 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/ms_visual_studio.png
--rw-r--r--   0        0        0   214948 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/notebook_specgram.png
--rw-r--r--   0        0        0    13520 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/_images/ptshell_features.png
--rw-r--r--   0        0        0   153249 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/qtconsole.png
--rw-r--r--   0        0        0   188627 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_images/qtconsole_tabbed.png
--rw-r--r--   0        0        0     5809 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/_images/unicode_completion.png
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/_static/
--rw-r--r--   0        0        0     1430 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/_static/favicon.ico
--rw-r--r--   0        0        0     9216 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/_static/logo.png
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/_templates/
--rw-r--r--   0        0        0      177 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/_templates/breadcrumbs.html
--rw-r--r--   0        0        0      274 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/_templates/notebook_redirect.html
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/about/
--rw-r--r--   0        0        0     1428 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/about/history.rst
--rw-r--r--   0        0        0      128 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/about/index.rst
--rw-r--r--   0        0        0    19620 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/about/license_and_copyright.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/api/
--rw-r--r--   0        0        0      164 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/api/index.rst
--rwxr-xr-x   0        0        0    10818 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/conf.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/config/
--rw-r--r--   0        0        0     3932 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/config/callbacks.rst
--rw-r--r--   0        0        0     6906 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/config/custommagics.rst
--rw-r--r--   0        0        0    12024 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/config/details.rst
--rw-r--r--   0        0        0     4428 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/config/eventloops.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/config/extensions/
--rw-r--r--   0        0        0      131 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/config/extensions/autoreload.rst
--rw-r--r--   0        0        0     3736 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/config/extensions/index.rst
--rw-r--r--   0        0        0      143 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/config/extensions/storemagic.rst
--rw-r--r--   0        0        0      563 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/config/index.rst
--rw-r--r--   0        0        0     3621 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/config/inputtransforms.rst
--rw-r--r--   0        0        0     4856 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/config/integrating.rst
--rw-r--r--   0        0        0     7251 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/config/intro.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/config/options/
--rw-r--r--   0        0        0      229 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/config/options/index.rst
--rw-r--r--   0        0        0     2413 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/config/shell_mimerenderer.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/config/shortcuts/
--rwxr-xr-x   0        0        0      675 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/config/shortcuts/index.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/coredev/
--rw-r--r--   0        0        0    10786 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/coredev/index.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/development/
--rw-r--r--   0        0        0     4768 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/development/config.rst
--rw-r--r--   0        0        0     2812 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/development/execution.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/development/figs/
--rw-r--r--   0        0        0    28265 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/development/figs/ipy_kernel_and_terminal.png
--rw-r--r--   0        0        0    12607 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/development/figs/ipy_kernel_and_terminal.svg
--rw-r--r--   0        0        0    41180 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/development/figs/other_kernels.png
--rw-r--r--   0        0        0    14272 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/development/figs/other_kernels.svg
--rw-r--r--   0        0        0     2511 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/development/how_ipython_works.rst
--rw-r--r--   0        0        0      539 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/development/index.rst
--rw-r--r--   0        0        0     2235 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/development/inputhook_app.rst
--rw-r--r--   0        0        0      182 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/development/kernels.rst
--rw-r--r--   0        0        0     2413 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/development/lexer.rst
--rw-r--r--   0        0        0      162 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/development/messaging.rst
--rw-r--r--   0        0        0      268 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/development/parallel_connections.rst
--rw-r--r--   0        0        0      223 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/development/parallel_messages.rst
--rw-r--r--   0        0        0     1237 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/development/pycompat.rst
--rw-r--r--   0        0        0     6144 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/development/wrapperkernels.rst
--rw-r--r--   0        0        0     3224 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/index.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/install/
--rw-r--r--   0        0        0     1159 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/install/index.rst
--rw-r--r--   0        0        0     4000 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/install/install.rst
--rw-r--r--   0        0        0     3767 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/install/kernel_install.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/interactive/
--rw-r--r--   0        0        0    11525 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/interactive/autoawait.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/interactive/figs/
--rw-r--r--   0        0        0    53726 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/interactive/figs/besselj.png
--rw-r--r--   0        0        0    61184 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/interactive/figs/colors_dark.png
--rw-r--r--   0        0        0    44935 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/interactive/figs/jn.html
--rw-r--r--   0        0        0    29224 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/interactive/figs/jn.xhtml
--rw-r--r--   0        0        0      814 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/interactive/index.rst
--rw-r--r--   0        0        0      939 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/interactive/magics.rst
--rw-r--r--   0        0        0     2697 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/interactive/plotting.rst
--rw-r--r--   0        0        0     6577 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/interactive/python-ipython-diff.rst
--rw-r--r--   0        0        0    39542 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/interactive/reference.rst
--rw-r--r--   0        0        0     7556 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/interactive/shell.rst
--rw-r--r--   0        0        0     3577 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/interactive/tips.rst
--rw-r--r--   0        0        0    11837 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/interactive/tutorial.rst
--rw-r--r--   0        0        0     4129 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/links.txt
--rw-r--r--   0        0        0    11594 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/overview.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/parallel/
--rw-r--r--   0        0        0      230 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/parallel/index.rst
--rw-r--r--   0        0        0    13703 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/sphinxext.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/whatsnew/
--rw-r--r--   0        0        0      619 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/development.rst
--rw-r--r--   0        0        0    51362 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/github-stats-0.11.rst
--rw-r--r--   0        0        0    59041 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/github-stats-0.12.rst
--rw-r--r--   0        0        0    71911 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/github-stats-0.13.rst
--rw-r--r--   0        0        0   107462 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/github-stats-1.0.rst
--rw-r--r--   0        0        0    87788 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/github-stats-2.0.rst
--rw-r--r--   0        0        0     4973 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/whatsnew/github-stats-3.rst
--rw-r--r--   0        0        0     3386 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/whatsnew/github-stats-4.rst
--rw-r--r--   0        0        0     4399 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/github-stats-5.rst
--rw-r--r--   0        0        0     3753 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/github-stats-6.rst
--rw-r--r--   0        0        0    12480 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/github-stats-7.rst
--rw-r--r--   0        0        0     2002 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/github-stats-8.rst
--rw-r--r--   0        0        0     1803 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/index.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/source/whatsnew/pr/
--rw-r--r--   0        0        0     1036 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/whatsnew/pr/README.md
--rw-r--r--   0        0        0      124 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/pr/antigravity-feature.rst
--rw-r--r--   0        0        0      255 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/pr/incompat-switching-to-perl.rst
--rw-r--r--   0        0        0    15433 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/version0.10.rst
--rw-r--r--   0        0        0    34904 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/version0.11.rst
--rw-r--r--   0        0        0    16577 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/version0.12.rst
--rw-r--r--   0        0        0    28297 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/version0.13.rst
--rw-r--r--   0        0        0      912 2021-10-27 18:09:58.000000 ipython-8.8.0/docs/source/whatsnew/version0.8.rst
--rw-r--r--   0        0        0    12469 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/version0.9.rst
--rw-r--r--   0        0        0    12949 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/whatsnew/version1.0.rst
--rw-r--r--   0        0        0    14061 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/version2.0.rst
--rw-r--r--   0        0        0    17305 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/version3.rst
--rw-r--r--   0        0        0    15393 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/version3_widget_migration.rst
--rw-r--r--   0        0        0     3407 2021-11-27 18:00:22.000000 ipython-8.8.0/docs/source/whatsnew/version4.rst
--rw-r--r--   0        0        0    18391 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/version5.rst
--rw-r--r--   0        0        0    14330 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/version6.rst
--rw-r--r--   0        0        0    64879 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/version7.rst
--rw-r--r--   0        0        0    50352 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/source/whatsnew/version8.rst
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/docs/sphinxext/
--rw-r--r--   0        0        0    17210 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/sphinxext/apigen.py
--rw-r--r--   0        0        0      414 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/sphinxext/configtraits.py
--rw-r--r--   0        0        0     5684 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/sphinxext/github.py
--rw-r--r--   0        0        0     1496 2023-01-03 13:18:33.000000 ipython-8.8.0/docs/sphinxext/magics.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/examples/
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/examples/Embedding/
--rw-r--r--   0        0        0     5074 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/Embedding/Index.ipynb
--rwxr-xr-x   0        0        0     4849 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/Embedding/embed_class_long.py
--rw-r--r--   0        0        0     1674 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/Embedding/embed_class_short.py
--rw-r--r--   0        0        0      258 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/Embedding/embed_function.py
--rwxr-xr-x   0        0        0      739 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/Embedding/start_ipython_config.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/examples/IPython Kernel/
--rw-r--r--   0        0        0   107963 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/Animations Using clear_output.ipynb
--rw-r--r--   0        0        0    15419 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/Background Jobs.ipynb
--rw-r--r--   0        0        0   132731 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/IPython Kernel/Beyond Plain Python.ipynb
--rw-r--r--   0        0        0    19695 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/Capturing Output.ipynb
--rw-r--r--   0        0        0    16860 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/Cell Magics.ipynb
--rw-r--r--   0        0        0    83998 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/IPython Kernel/Custom Display Logic.ipynb
--rw-r--r--   0        0        0    22198 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/IPython Kernel/Importing Notebooks.ipynb
--rw-r--r--   0        0        0     4884 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/IPython Kernel/Index.ipynb
--rw-r--r--   0        0        0   370083 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/IPython Kernel/Plotting in the Notebook.ipynb
--rw-r--r--   0        0        0     6054 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/Raw Input in the Notebook.ipynb
--rw-r--r--   0        0        0   300702 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/IPython Kernel/Rich Output.ipynb
--rw-r--r--   0        0        0     9347 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/IPython Kernel/Script Magics.ipynb
--rw-r--r--   0        0        0   305111 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/SymPy.ipynb
--rw-r--r--   0        0        0     5964 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/IPython Kernel/Terminal Usage.ipynb
--rw-r--r--   0        0        0   261308 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/Third Party Rich Output.ipynb
--rw-r--r--   0        0        0    75473 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/Trapezoid Rule.ipynb
--rw-r--r--   0        0        0     6953 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/Updating Displays.ipynb
--rw-r--r--   0        0        0    48173 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/Working With External Code.ipynb
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/examples/IPython Kernel/data/
--rw-r--r--   0        0        0    11414 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/data/flare.json
--rw-r--r--   0        0        0     1182 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/IPython Kernel/example-demo.py
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/examples/IPython Kernel/gui/
--rwxr-xr-x   0        0        0     1297 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/gui/gui-glut.py
--rw-r--r--   0        0        0      716 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/IPython Kernel/gui/gui-gtk4.py
--rwxr-xr-x   0        0        0     1009 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/gui/gui-qt.py
--rw-r--r--   0        0        0     4271 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/ipython-completion.bash
--rwxr-xr-x   0        0        0     1136 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/IPython Kernel/ipython-get-history.py
--rw-r--r--   0        0        0      400 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/ipython.desktop
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/examples/IPython Kernel/nbpackage/
--rw-r--r--   0        0        0        0 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/nbpackage/__init__.py
--rw-r--r--   0        0        0     1144 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/nbpackage/mynotebook.ipynb
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/examples/IPython Kernel/nbpackage/nbs/
--rw-r--r--   0        0        0        0 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/nbpackage/nbs/__init__.py
--rw-r--r--   0        0        0      748 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/IPython Kernel/nbpackage/nbs/other.ipynb
--rw-r--r--   0        0        0     1458 2023-01-03 13:18:33.000000 ipython-8.8.0/examples/Index.ipynb
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/examples/images/
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/examples/images/FrontendKernel.graffle/
--rw-r--r--   0        0        0    10212 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/images/FrontendKernel.graffle/data.plist
--rw-r--r--   0        0        0    14726 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/images/FrontendKernel.graffle/image1.png
--rw-r--r--   0        0        0    33170 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/images/FrontendKernel.png
--rw-r--r--   0        0        0    11903 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/images/animation.m4v
--rw-r--r--   0        0        0     9216 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/images/ipython_logo.png
--rw-r--r--   0        0        0    15301 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/images/python_logo.svg
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/examples/utils/
--rw-r--r--   0        0        0      616 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/utils/cwd_prompt.py
--rw-r--r--   0        0        0      182 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/utils/list_pyfiles.ipy
--rw-r--r--   0        0        0      194 2021-11-27 18:00:22.000000 ipython-8.8.0/examples/utils/list_subdirs.ipy
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/ipython.egg-info/
--rw-r--r--   0        0        0     2706 2023-01-03 14:03:24.000000 ipython-8.8.0/ipython.egg-info/PKG-INFO
--rw-r--r--   0        0        0    16638 2023-01-03 14:03:24.000000 ipython-8.8.0/ipython.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-01-03 14:03:24.000000 ipython-8.8.0/ipython.egg-info/dependency_links.txt
--rw-r--r--   0        0        0      244 2023-01-03 14:03:24.000000 ipython-8.8.0/ipython.egg-info/entry_points.txt
--rw-r--r--   0        0        0        1 2023-01-03 14:03:24.000000 ipython-8.8.0/ipython.egg-info/not-zip-safe
--rw-r--r--   0        0        0      988 2023-01-03 14:03:24.000000 ipython-8.8.0/ipython.egg-info/requires.txt
--rw-r--r--   0        0        0        8 2023-01-03 14:03:24.000000 ipython-8.8.0/ipython.egg-info/top_level.txt
--rw-r--r--   0        0        0     1387 2023-01-03 13:18:33.000000 ipython-8.8.0/long_description.rst
--rw-r--r--   0        0        0       82 2023-01-03 13:18:33.000000 ipython-8.8.0/mypy.ini
--rw-r--r--   0        0        0       91 2023-01-03 13:18:33.000000 ipython-8.8.0/pyproject.toml
--rw-r--r--   0        0        0     1419 2023-01-03 13:18:33.000000 ipython-8.8.0/pytest.ini
-drwxr-xr-x   0        0        0        0 2023-01-03 14:03:24.000000 ipython-8.8.0/scripts/
--rw-r--r--   0        0        0    32580 2021-10-27 18:09:58.000000 ipython-8.8.0/scripts/ipython.ico
--rw-r--r--   0        0        0    44204 2021-10-27 18:09:58.000000 ipython-8.8.0/scripts/ipython_nb.ico
--rw-r--r--   0        0        0     2203 2023-01-03 14:03:24.000000 ipython-8.8.0/setup.cfg
--rw-r--r--   0        0        0     5179 2023-01-03 13:18:33.000000 ipython-8.8.0/setup.py
--rw-r--r--   0        0        0    11786 2023-01-03 13:18:33.000000 ipython-8.8.0/setupbase.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/
+-rw-r--r--   0        0        0      143 2023-01-26 13:54:33.000000 ipython-8.9.0/.flake8
+-rw-r--r--   0        0        0    12671 2023-01-26 13:54:33.000000 ipython-8.9.0/.mailmap
+-rw-r--r--   0        0        0      409 2023-01-26 13:54:33.000000 ipython-8.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1639 2023-01-26 13:54:33.000000 ipython-8.9.0/COPYING.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/
+-rw-r--r--   0        0        0     5962 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/__init__.py
+-rw-r--r--   0        0        0      488 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/__main__.py
+-rw-r--r--   0        0        0     2618 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/conftest.py
+-rw-r--r--   0        0        0      415 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/consoleapp.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/core/
+-rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.9.0/IPython/core/__init__.py
+-rw-r--r--   0        0        0    10034 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/alias.py
+-rw-r--r--   0        0        0    18937 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/application.py
+-rw-r--r--   0        0        0     4297 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/core/async_helpers.py
+-rw-r--r--   0        0        0     1991 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/autocall.py
+-rw-r--r--   0        0        0     3009 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/builtin_trap.py
+-rw-r--r--   0        0        0     7730 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/compilerop.py
+-rw-r--r--   0        0        0   116855 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/completer.py
+-rw-r--r--   0        0        0    12259 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/completerlib.py
+-rw-r--r--   0        0        0     8508 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/crashhandler.py
+-rw-r--r--   0        0        0    33382 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/debugger.py
+-rw-r--r--   0        0        0    42476 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/display.py
+-rw-r--r--   0        0        0    12918 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/display_functions.py
+-rw-r--r--   0        0        0     2098 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/display_trap.py
+-rw-r--r--   0        0        0    12608 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/displayhook.py
+-rw-r--r--   0        0        0     4944 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/displaypub.py
+-rw-r--r--   0        0        0     1734 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/error.py
+-rw-r--r--   0        0        0     5349 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/events.py
+-rw-r--r--   0        0        0     4928 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/excolors.py
+-rw-r--r--   0        0        0     5780 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/extensions.py
+-rw-r--r--   0        0        0    34952 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/formatters.py
+-rw-r--r--   0        0        0      912 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/getipython.py
+-rw-r--r--   0        0        0    24054 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/core/guarded_eval.py
+-rw-r--r--   0        0        0    34174 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/history.py
+-rw-r--r--   0        0        0     5909 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/historyapp.py
+-rw-r--r--   0        0        0     5663 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/hooks.py
+-rw-r--r--   0        0        0    28119 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/inputsplitter.py
+-rw-r--r--   0        0        0    17942 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/inputtransformer.py
+-rw-r--r--   0        0        0    28374 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/inputtransformer2.py
+-rw-r--r--   0        0        0   150371 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/interactiveshell.py
+-rw-r--r--   0        0        0    31288 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/latex_symbols.py
+-rw-r--r--   0        0        0     7930 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/logger.py
+-rw-r--r--   0        0        0     1734 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/macro.py
+-rw-r--r--   0        0        0    28478 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magic.py
+-rw-r--r--   0        0        0     9736 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magic_arguments.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/core/magics/
+-rw-r--r--   0        0        0     1619 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/__init__.py
+-rw-r--r--   0        0        0     4816 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/auto.py
+-rw-r--r--   0        0        0    22932 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/basic.py
+-rw-r--r--   0        0        0    28051 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/code.py
+-rw-r--r--   0        0        0     4881 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/config.py
+-rw-r--r--   0        0        0     3130 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/display.py
+-rw-r--r--   0        0        0    57843 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/execution.py
+-rw-r--r--   0        0        0     2477 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/extension.py
+-rw-r--r--   0        0        0    12628 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/history.py
+-rw-r--r--   0        0        0     6859 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/logging.py
+-rw-r--r--   0        0        0    24823 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/namespace.py
+-rw-r--r--   0        0        0    30681 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/osm.py
+-rw-r--r--   0        0        0     3916 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/packaging.py
+-rw-r--r--   0        0        0     6574 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/pylab.py
+-rw-r--r--   0        0        0    12191 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/magics/script.py
+-rw-r--r--   0        0        0    37073 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/oinspect.py
+-rw-r--r--   0        0        0    11753 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/page.py
+-rw-r--r--   0        0        0     1758 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/payload.py
+-rw-r--r--   0        0        0     1431 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/payloadpage.py
+-rw-r--r--   0        0        0    25583 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/prefilter.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/core/profile/
+-rw-r--r--   0        0        0      371 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/core/profile/README_STARTUP
+-rw-r--r--   0        0        0    10631 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/profileapp.py
+-rw-r--r--   0        0        0     8029 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/profiledir.py
+-rw-r--r--   0        0        0      607 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/prompts.py
+-rw-r--r--   0        0        0    13809 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/pylabtools.py
+-rw-r--r--   0        0        0     2177 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/core/release.py
+-rw-r--r--   0        0        0    17845 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/shellapp.py
+-rw-r--r--   0        0        0     4787 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/splitinput.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/core/tests/
+-rw-r--r--   0        0        0      331 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/core/tests/2x2.jpg
+-rw-r--r--   0        0        0       71 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/core/tests/2x2.png
+-rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.9.0/IPython/core/tests/__init__.py
+-rw-r--r--   0        0        0      206 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/bad_all.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/core/tests/daft_extension/
+-rw-r--r--   0        0        0      285 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/daft_extension/daft_extension.py
+-rw-r--r--   0        0        0      135 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/core/tests/nonascii.py
+-rw-r--r--   0        0        0      155 2023-01-27 10:04:39.000000 ipython-8.9.0/IPython/core/tests/nonascii2.py
+-rw-r--r--   0        0        0       32 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/core/tests/print_argv.py
+-rw-r--r--   0        0        0     1494 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/refbug.py
+-rw-r--r--   0        0        0      583 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/simpleerr.py
+-rw-r--r--   0        0        0      921 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/tclass.py
+-rw-r--r--   0        0        0     2007 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_alias.py
+-rw-r--r--   0        0        0     2245 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_application.py
+-rw-r--r--   0        0        0     8769 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_async_helpers.py
+-rw-r--r--   0        0        0     1425 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/core/tests/test_autocall.py
+-rw-r--r--   0        0        0     2174 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_compilerop.py
+-rw-r--r--   0        0        0    60333 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_completer.py
+-rw-r--r--   0        0        0     6473 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_completerlib.py
+-rw-r--r--   0        0        0    14502 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_debugger.py
+-rw-r--r--   0        0        0    15946 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_display.py
+-rw-r--r--   0        0        0     3593 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_displayhook.py
+-rw-r--r--   0        0        0     2799 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_events.py
+-rw-r--r--   0        0        0     3026 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_extension.py
+-rw-r--r--   0        0        0    14249 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_formatters.py
+-rw-r--r--   0        0        0    14853 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/core/tests/test_guarded_eval.py
+-rw-r--r--   0        0        0     3286 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_handlers.py
+-rw-r--r--   0        0        0    11698 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_history.py
+-rw-r--r--   0        0        0     2316 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_hooks.py
+-rw-r--r--   0        0        0     1153 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_imports.py
+-rw-r--r--   0        0        0    23159 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_inputsplitter.py
+-rw-r--r--   0        0        0    15755 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_inputtransformer.py
+-rw-r--r--   0        0        0    11263 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_inputtransformer2.py
+-rw-r--r--   0        0        0     2971 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_inputtransformer2_line.py
+-rw-r--r--   0        0        0    37182 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_interactiveshell.py
+-rw-r--r--   0        0        0     8470 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_iplib.py
+-rw-r--r--   0        0        0      776 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_logger.py
+-rw-r--r--   0        0        0    40984 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_magic.py
+-rw-r--r--   0        0        0     4778 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_magic_arguments.py
+-rw-r--r--   0        0        0     5996 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_magic_terminal.py
+-rw-r--r--   0        0        0    14809 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_oinspect.py
+-rw-r--r--   0        0        0      772 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_page.py
+-rw-r--r--   0        0        0     7081 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_paths.py
+-rw-r--r--   0        0        0     4214 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_prefilter.py
+-rw-r--r--   0        0        0     5064 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_profile.py
+-rw-r--r--   0        0        0      845 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_prompts.py
+-rw-r--r--   0        0        0     7883 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_pylabtools.py
+-rw-r--r--   0        0        0    19369 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_run.py
+-rw-r--r--   0        0        0     1892 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_shellapp.py
+-rw-r--r--   0        0        0     1227 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/core/tests/test_splitinput.py
+-rw-r--r--   0        0        0    11495 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/tests/test_ultratb.py
+-rw-r--r--   0        0        0    46165 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/ultratb.py
+-rw-r--r--   0        0        0    13542 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/core/usage.py
+-rw-r--r--   0        0        0     1119 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/display.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/extensions/
+-rw-r--r--   0        0        0       78 2021-10-27 18:09:58.000000 ipython-8.9.0/IPython/extensions/__init__.py
+-rw-r--r--   0        0        0    19741 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/extensions/autoreload.py
+-rw-r--r--   0        0        0     8161 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/extensions/storemagic.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/extensions/tests/
+-rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.9.0/IPython/extensions/tests/__init__.py
+-rw-r--r--   0        0        0    18691 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/extensions/tests/test_autoreload.py
+-rw-r--r--   0        0        0     2081 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/extensions/tests/test_storemagic.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/external/
+-rw-r--r--   0        0        0      126 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/external/__init__.py
+-rw-r--r--   0        0        0     3445 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/external/qt_for_kernel.py
+-rw-r--r--   0        0        0    11158 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/external/qt_loaders.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/external/tests/
+-rw-r--r--   0        0        0        0 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/external/tests/__init__.py
+-rw-r--r--   0        0        0      367 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/external/tests/test_qt_loaders.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/lib/
+-rw-r--r--   0        0        0      409 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/__init__.py
+-rw-r--r--   0        0        0    17738 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/backgroundjobs.py
+-rw-r--r--   0        0        0     3050 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/clipboard.py
+-rw-r--r--   0        0        0     9431 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/deepreload.py
+-rw-r--r--   0        0        0    24518 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/demo.py
+-rw-r--r--   0        0        0    24532 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/display.py
+-rw-r--r--   0        0        0     3982 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/editorhooks.py
+-rw-r--r--   0        0        0     6305 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/guisupport.py
+-rw-r--r--   0        0        0     8299 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/latextools.py
+-rw-r--r--   0        0        0    20218 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/lexers.py
+-rw-r--r--   0        0        0    30872 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/pretty.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/lib/tests/
+-rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.9.0/IPython/lib/tests/__init__.py
+-rw-r--r--   0        0        0    44144 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/lib/tests/test.wav
+-rw-r--r--   0        0        0     2698 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/tests/test_backgroundjobs.py
+-rw-r--r--   0        0        0      630 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/lib/tests/test_clipboard.py
+-rw-r--r--   0        0        0     1854 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/lib/tests/test_deepreload.py
+-rw-r--r--   0        0        0     9313 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/tests/test_display.py
+-rw-r--r--   0        0        0      884 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/tests/test_editorhooks.py
+-rw-r--r--   0        0        0      273 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/lib/tests/test_imports.py
+-rw-r--r--   0        0        0     5736 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/tests/test_latextools.py
+-rw-r--r--   0        0        0     6017 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/tests/test_lexers.py
+-rw-r--r--   0        0        0    14830 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/lib/tests/test_pretty.py
+-rw-r--r--   0        0        0      824 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/lib/tests/test_pygments.py
+-rw-r--r--   0        0        0     4335 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/paths.py
+-rw-r--r--   0        0        0        0 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/py.typed
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/sphinxext/
+-rw-r--r--   0        0        0        0 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/sphinxext/__init__.py
+-rw-r--r--   0        0        0     4615 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/sphinxext/custom_doctests.py
+-rw-r--r--   0        0        0      970 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/sphinxext/ipython_console_highlighting.py
+-rw-r--r--   0        0        0    45069 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/sphinxext/ipython_directive.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/terminal/
+-rw-r--r--   0        0        0        0 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/terminal/__init__.py
+-rw-r--r--   0        0        0      691 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/console.py
+-rw-r--r--   0        0        0     6618 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/debugger.py
+-rw-r--r--   0        0        0    15220 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/embed.py
+-rw-r--r--   0        0        0    29739 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/interactiveshell.py
+-rwxr-xr-x   0        0        0    12407 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/ipapp.py
+-rw-r--r--   0        0        0     7705 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/magics.py
+-rw-r--r--   0        0        0     3360 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/prompts.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/terminal/pt_inputhooks/
+-rw-r--r--   0        0        0     1266 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/pt_inputhooks/__init__.py
+-rw-r--r--   0        0        0     1844 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/terminal/pt_inputhooks/asyncio.py
+-rw-r--r--   0        0        0     4997 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/pt_inputhooks/glut.py
+-rw-r--r--   0        0        0     2427 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/terminal/pt_inputhooks/gtk.py
+-rw-r--r--   0        0        0      280 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/terminal/pt_inputhooks/gtk3.py
+-rw-r--r--   0        0        0      557 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/terminal/pt_inputhooks/gtk4.py
+-rw-r--r--   0        0        0     4789 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/pt_inputhooks/osx.py
+-rw-r--r--   0        0        0     2368 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/pt_inputhooks/pyglet.py
+-rw-r--r--   0        0        0     3206 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/pt_inputhooks/qt.py
+-rw-r--r--   0        0        0     3648 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/pt_inputhooks/tk.py
+-rw-r--r--   0        0        0     7132 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/pt_inputhooks/wx.py
+-rw-r--r--   0        0        0     7481 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/ptutils.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/terminal/shortcuts/
+-rw-r--r--   0        0        0    20431 2023-01-26 13:54:36.000000 ipython-8.9.0/IPython/terminal/shortcuts/__init__.py
+-rw-r--r--   0        0        0     3055 2023-01-26 13:54:36.000000 ipython-8.9.0/IPython/terminal/shortcuts/auto_match.py
+-rw-r--r--   0        0        0    12971 2023-01-26 13:54:36.000000 ipython-8.9.0/IPython/terminal/shortcuts/auto_suggest.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/terminal/tests/
+-rw-r--r--   0        0        0        0 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/terminal/tests/__init__.py
+-rw-r--r--   0        0        0     2375 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/tests/test_debug_magic.py
+-rw-r--r--   0        0        0     4804 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/tests/test_embed.py
+-rw-r--r--   0        0        0      722 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/tests/test_help.py
+-rw-r--r--   0        0        0     7749 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/terminal/tests/test_interactivshell.py
+-rw-r--r--   0        0        0     9625 2023-01-26 13:54:36.000000 ipython-8.9.0/IPython/terminal/tests/test_shortcuts.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/testing/
+-rw-r--r--   0        0        0      784 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/__init__.py
+-rw-r--r--   0        0        0     6777 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/decorators.py
+-rw-r--r--   0        0        0     3948 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/globalipapp.py
+-rw-r--r--   0        0        0     6540 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/ipunittest.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/testing/plugin/
+-rw-r--r--   0        0        0     1437 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/testing/plugin/Makefile
+-rw-r--r--   0        0        0     1043 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/testing/plugin/README.txt
+-rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.9.0/IPython/testing/plugin/__init__.py
+-rw-r--r--   0        0        0     2921 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/plugin/dtexample.py
+-rw-r--r--   0        0        0    11881 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/plugin/ipdoctest.py
+-rw-r--r--   0        0        0    29690 2023-01-27 09:51:54.000000 ipython-8.9.0/IPython/testing/plugin/pytest_ipdoctest.py
+-rwxr-xr-x   0        0        0      539 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/plugin/setup.py
+-rw-r--r--   0        0        0      727 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/plugin/simple.py
+-rw-r--r--   0        0        0       24 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/testing/plugin/simplevars.py
+-rw-r--r--   0        0        0      923 2022-03-19 09:18:04.000000 ipython-8.9.0/IPython/testing/plugin/test_combo.txt
+-rw-r--r--   0        0        0      730 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/testing/plugin/test_example.txt
+-rw-r--r--   0        0        0      814 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/testing/plugin/test_exampleip.txt
+-rw-r--r--   0        0        0     1907 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/plugin/test_ipdoctest.py
+-rw-r--r--   0        0        0      715 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/plugin/test_refs.py
+-rw-r--r--   0        0        0      717 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/testing/skipdoctest.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/testing/tests/
+-rw-r--r--   0        0        0      558 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/tests/__init__.py
+-rw-r--r--   0        0        0     3955 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/tests/test_decorators.py
+-rw-r--r--   0        0        0     3301 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/tests/test_ipunittest.py
+-rw-r--r--   0        0        0     4157 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/tests/test_tools.py
+-rw-r--r--   0        0        0    14105 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/testing/tools.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/tests/
+-rw-r--r--   0        0        0     2000 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/tests/cve.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/utils/
+-rw-r--r--   0        0        0    10875 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/PyColorize.py
+-rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.9.0/IPython/utils/__init__.py
+-rw-r--r--   0        0        0     2020 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/_process_cli.py
+-rw-r--r--   0        0        0     7003 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/_process_common.py
+-rw-r--r--   0        0        0     8666 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/_process_posix.py
+-rw-r--r--   0        0        0     6132 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/_process_win32.py
+-rw-r--r--   0        0        0    21329 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/_process_win32_controller.py
+-rw-r--r--   0        0        0       45 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/utils/_sysinfo.py
+-rw-r--r--   0        0        0     5161 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/capture.py
+-rw-r--r--   0        0        0      786 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/colorable.py
+-rw-r--r--   0        0        0     6972 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/coloransi.py
+-rw-r--r--   0        0        0     1619 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/utils/contexts.py
+-rw-r--r--   0        0        0      200 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/daemonize.py
+-rw-r--r--   0        0        0     1015 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/data.py
+-rw-r--r--   0        0        0     2680 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/decorators.py
+-rw-r--r--   0        0        0     2232 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/dir2.py
+-rw-r--r--   0        0        0       86 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/utils/docs.py
+-rw-r--r--   0        0        0     2843 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/encoding.py
+-rw-r--r--   0        0        0      138 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/utils/eventful.py
+-rw-r--r--   0        0        0     3048 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/frame.py
+-rw-r--r--   0        0        0      706 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/utils/generics.py
+-rw-r--r--   0        0        0     1050 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/importstring.py
+-rw-r--r--   0        0        0     4631 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/io.py
+-rw-r--r--   0        0        0    11856 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/ipstruct.py
+-rw-r--r--   0        0        0      148 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/utils/jsonutil.py
+-rw-r--r--   0        0        0      169 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/localinterfaces.py
+-rw-r--r--   0        0        0      123 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/utils/log.py
+-rw-r--r--   0        0        0     2329 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/module_paths.py
+-rw-r--r--   0        0        0     3417 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/openpy.py
+-rw-r--r--   0        0        0    11937 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/path.py
+-rw-r--r--   0        0        0     1878 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/process.py
+-rw-r--r--   0        0        0     1601 2023-01-27 09:51:54.000000 ipython-8.9.0/IPython/utils/py3compat.py
+-rw-r--r--   0        0        0      421 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/sentinel.py
+-rw-r--r--   0        0        0     2669 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/shimmodule.py
+-rw-r--r--   0        0        0      474 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/signatures.py
+-rw-r--r--   0        0        0     1838 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/strdispatch.py
+-rw-r--r--   0        0        0     4324 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/sysinfo.py
+-rw-r--r--   0        0        0     1952 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/syspathcontext.py
+-rw-r--r--   0        0        0     1867 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/utils/tempdir.py
+-rw-r--r--   0        0        0     3793 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/terminal.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/IPython/utils/tests/
+-rw-r--r--   0        0        0        0 2021-10-27 18:09:58.000000 ipython-8.9.0/IPython/utils/tests/__init__.py
+-rw-r--r--   0        0        0     5319 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tests/test_capture.py
+-rw-r--r--   0        0        0      170 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tests/test_decorators.py
+-rw-r--r--   0        0        0      183 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/utils/tests/test_deprecated.py
+-rw-r--r--   0        0        0     1446 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/utils/tests/test_dir2.py
+-rw-r--r--   0        0        0      439 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tests/test_imports.py
+-rw-r--r--   0        0        0     1213 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tests/test_importstring.py
+-rw-r--r--   0        0        0     1410 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tests/test_io.py
+-rw-r--r--   0        0        0     3272 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tests/test_module_paths.py
+-rw-r--r--   0        0        0     1219 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/utils/tests/test_openpy.py
+-rw-r--r--   0        0        0    16104 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tests/test_path.py
+-rw-r--r--   0        0        0     6134 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tests/test_process.py
+-rw-r--r--   0        0        0     1711 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tests/test_pycolorize.py
+-rw-r--r--   0        0        0      387 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/utils/tests/test_shimmodule.py
+-rw-r--r--   0        0        0      464 2023-01-26 13:54:33.000000 ipython-8.9.0/IPython/utils/tests/test_sysinfo.py
+-rw-r--r--   0        0        0     1108 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tests/test_tempdir.py
+-rw-r--r--   0        0        0     7114 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tests/test_text.py
+-rw-r--r--   0        0        0     3918 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tests/test_tokenutil.py
+-rw-r--r--   0        0        0     4729 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tests/test_wildcard.py
+-rw-r--r--   0        0        0    22794 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/text.py
+-rw-r--r--   0        0        0     4238 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/timing.py
+-rw-r--r--   0        0        0     3928 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tokenutil.py
+-rw-r--r--   0        0        0      143 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/traitlets.py
+-rw-r--r--   0        0        0     1352 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/tz.py
+-rw-r--r--   0        0        0      684 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/ulinecache.py
+-rw-r--r--   0        0        0     1223 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/version.py
+-rw-r--r--   0        0        0     4612 2023-01-27 09:45:27.000000 ipython-8.9.0/IPython/utils/wildcard.py
+-rw-r--r--   0        0        0     1720 2023-01-26 13:54:33.000000 ipython-8.9.0/LICENSE
+-rw-r--r--   0        0        0      882 2023-01-26 13:54:33.000000 ipython-8.9.0/MANIFEST.in
+-rw-r--r--   0        0        0     2706 2023-01-27 11:56:59.000000 ipython-8.9.0/PKG-INFO
+-rw-r--r--   0        0        0     6477 2023-01-26 13:54:33.000000 ipython-8.9.0/README.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/
+-rw-r--r--   0        0        0     4774 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/Makefile
+-rw-r--r--   0        0        0     1873 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/README.rst
+-rwxr-xr-x   0        0        0     2934 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/autogen_api.py
+-rwxr-xr-x   0        0        0     4196 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/autogen_config.py
+-rw-r--r--   0        0        0     1998 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/autogen_magics.py
+-rwxr-xr-x   0        0        0     6688 2023-01-27 10:35:51.000000 ipython-8.9.0/docs/autogen_shortcuts.py
+-rw-r--r--   0        0        0     2685 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/make.cmd
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/man/
+-rw-r--r--   0        0        0     2058 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/man/ipython.1
+-rw-r--r--   0        0        0       10 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/requirements.txt
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/_images/
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/_images/2.0/
+-rw-r--r--   0        0        0   113866 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/2.0/running-crop.png
+-rw-r--r--   0        0        0   122393 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/2.0/running.png
+-rw-r--r--   0        0        0   134168 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/2.0/treeview.png
+-rw-r--r--   0        0        0   284971 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/2.0/user-interface.png
+-rw-r--r--   0        0        0   222518 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/2.0/widgets.png
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/_images/8.0/
+-rw-r--r--   0        0        0     6225 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/8.0/auto_suggest_1_prompt_no_text.png
+-rw-r--r--   0        0        0    13654 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/8.0/auto_suggest_2_print_hello_suggest.png
+-rw-r--r--   0        0        0    16308 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/8.0/auto_suggest_3_print_hello_suggest.png
+-rw-r--r--   0        0        0    17190 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/8.0/auto_suggest_4_print_hello.png
+-rw-r--r--   0        0        0    14362 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/8.0/auto_suggest_d_completions.png
+-rw-r--r--   0        0        0     4731 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/8.0/auto_suggest_d_phantom.png
+-rw-r--r--   0        0        0    17497 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/8.0/auto_suggest_def_completions.png
+-rw-r--r--   0        0        0     4947 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/8.0/auto_suggest_def_phantom.png
+-rw-r--r--   0        0        0     6603 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/8.0/auto_suggest_match_parens.png
+-rw-r--r--   0        0        0     7602 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/8.0/auto_suggest_second_prompt.png
+-rw-r--r--   0        0        0    77651 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/8.0/pathlib_pathlib_everywhere.jpg
+-rw-r--r--   0        0        0   137790 2023-01-26 13:54:36.000000 ipython-8.9.0/docs/source/_images/autosuggest.gif
+-rw-r--r--   0        0        0    38090 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ipy_013_dashboard.png
+-rw-r--r--   0        0        0    41133 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ipy_013_dashboard_cluster.png
+-rw-r--r--   0        0        0    76125 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ipy_013_notebook_cythonmagic.png
+-rw-r--r--   0        0        0    18803 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ipy_013_notebook_long_out.png
+-rw-r--r--   0        0        0   274282 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ipy_013_notebook_octavemagic.png
+-rw-r--r--   0        0        0   132820 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ipy_013_notebook_rmagic.png
+-rw-r--r--   0        0        0    17912 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ipy_013_notebook_script_cells.png
+-rw-r--r--   0        0        0   355455 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ipy_013_notebook_spectrogram.png
+-rw-r--r--   0        0        0   136934 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ipy_013_notebook_tooltip.png
+-rw-r--r--   0        0        0    30116 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ipy_013_par_tb.png
+-rw-r--r--   0        0        0   162832 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ipy_013_qtconsole_baboon.png
+-rw-r--r--   0        0        0    28262 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ipy_013_qtconsole_completer.png
+-rw-r--r--   0        0        0    55988 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ipython-6-screenshot.png
+-rw-r--r--   0        0        0    59846 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/jedi_type_inference_60.png
+-rw-r--r--   0        0        0     9693 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/kernel_selector_screenshot.png
+-rw-r--r--   0        0        0   117077 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ms_visual_studio.png
+-rw-r--r--   0        0        0   214948 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/notebook_specgram.png
+-rw-r--r--   0        0        0    13520 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/ptshell_features.png
+-rw-r--r--   0        0        0   153249 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/qtconsole.png
+-rw-r--r--   0        0        0   188627 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/qtconsole_tabbed.png
+-rw-r--r--   0        0        0     5809 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_images/unicode_completion.png
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/_static/
+-rw-r--r--   0        0        0     1430 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_static/favicon.ico
+-rw-r--r--   0        0        0     9216 2021-10-27 18:09:58.000000 ipython-8.9.0/docs/source/_static/logo.png
+-rw-r--r--   0        0        0      257 2023-01-26 13:54:36.000000 ipython-8.9.0/docs/source/_static/theme_overrides.css
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/_templates/
+-rw-r--r--   0        0        0      177 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_templates/breadcrumbs.html
+-rw-r--r--   0        0        0      274 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/_templates/notebook_redirect.html
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/about/
+-rw-r--r--   0        0        0     1428 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/about/history.rst
+-rw-r--r--   0        0        0      128 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/about/index.rst
+-rw-r--r--   0        0        0    19620 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/about/license_and_copyright.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/api/
+-rw-r--r--   0        0        0      164 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/api/index.rst
+-rwxr-xr-x   0        0        0    10879 2023-01-27 10:35:51.000000 ipython-8.9.0/docs/source/conf.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/config/
+-rw-r--r--   0        0        0     3932 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/config/callbacks.rst
+-rw-r--r--   0        0        0     6906 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/config/custommagics.rst
+-rw-r--r--   0        0        0    12024 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/config/details.rst
+-rw-r--r--   0        0        0     4428 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/config/eventloops.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/config/extensions/
+-rw-r--r--   0        0        0      131 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/config/extensions/autoreload.rst
+-rw-r--r--   0        0        0     3736 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/config/extensions/index.rst
+-rw-r--r--   0        0        0      143 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/config/extensions/storemagic.rst
+-rw-r--r--   0        0        0      563 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/config/index.rst
+-rw-r--r--   0        0        0     3621 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/config/inputtransforms.rst
+-rw-r--r--   0        0        0     4856 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/config/integrating.rst
+-rw-r--r--   0        0        0     7251 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/config/intro.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/config/options/
+-rw-r--r--   0        0        0      229 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/config/options/index.rst
+-rw-r--r--   0        0        0     2413 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/config/shell_mimerenderer.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/config/shortcuts/
+-rwxr-xr-x   0        0        0      814 2023-01-26 13:54:36.000000 ipython-8.9.0/docs/source/config/shortcuts/index.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/coredev/
+-rw-r--r--   0        0        0    10786 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/coredev/index.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/development/
+-rw-r--r--   0        0        0     4768 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/config.rst
+-rw-r--r--   0        0        0     2812 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/execution.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/development/figs/
+-rw-r--r--   0        0        0    28265 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/figs/ipy_kernel_and_terminal.png
+-rw-r--r--   0        0        0    12607 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/figs/ipy_kernel_and_terminal.svg
+-rw-r--r--   0        0        0    41180 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/figs/other_kernels.png
+-rw-r--r--   0        0        0    14272 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/figs/other_kernels.svg
+-rw-r--r--   0        0        0     2511 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/how_ipython_works.rst
+-rw-r--r--   0        0        0      539 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/index.rst
+-rw-r--r--   0        0        0     2235 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/inputhook_app.rst
+-rw-r--r--   0        0        0      182 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/kernels.rst
+-rw-r--r--   0        0        0     2413 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/lexer.rst
+-rw-r--r--   0        0        0      162 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/messaging.rst
+-rw-r--r--   0        0        0      268 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/parallel_connections.rst
+-rw-r--r--   0        0        0      223 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/parallel_messages.rst
+-rw-r--r--   0        0        0     1237 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/pycompat.rst
+-rw-r--r--   0        0        0     6144 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/development/wrapperkernels.rst
+-rw-r--r--   0        0        0     3224 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/index.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/install/
+-rw-r--r--   0        0        0     1159 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/install/index.rst
+-rw-r--r--   0        0        0     4000 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/install/install.rst
+-rw-r--r--   0        0        0     3767 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/install/kernel_install.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/interactive/
+-rw-r--r--   0        0        0    11525 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/interactive/autoawait.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/interactive/figs/
+-rw-r--r--   0        0        0    53726 2021-10-27 18:09:58.000000 ipython-8.9.0/docs/source/interactive/figs/besselj.png
+-rw-r--r--   0        0        0    61184 2021-10-27 18:09:58.000000 ipython-8.9.0/docs/source/interactive/figs/colors_dark.png
+-rw-r--r--   0        0        0    44935 2021-10-27 18:09:58.000000 ipython-8.9.0/docs/source/interactive/figs/jn.html
+-rw-r--r--   0        0        0    29224 2021-10-27 18:09:58.000000 ipython-8.9.0/docs/source/interactive/figs/jn.xhtml
+-rw-r--r--   0        0        0      814 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/interactive/index.rst
+-rw-r--r--   0        0        0      939 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/interactive/magics.rst
+-rw-r--r--   0        0        0     2697 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/interactive/plotting.rst
+-rw-r--r--   0        0        0     6577 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/interactive/python-ipython-diff.rst
+-rw-r--r--   0        0        0    39542 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/interactive/reference.rst
+-rw-r--r--   0        0        0     7556 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/interactive/shell.rst
+-rw-r--r--   0        0        0     3577 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/interactive/tips.rst
+-rw-r--r--   0        0        0    11837 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/interactive/tutorial.rst
+-rw-r--r--   0        0        0     4129 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/links.txt
+-rw-r--r--   0        0        0    11594 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/overview.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/parallel/
+-rw-r--r--   0        0        0      230 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/parallel/index.rst
+-rw-r--r--   0        0        0    13703 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/sphinxext.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/whatsnew/
+-rw-r--r--   0        0        0      619 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/development.rst
+-rw-r--r--   0        0        0    51362 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/github-stats-0.11.rst
+-rw-r--r--   0        0        0    59041 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/github-stats-0.12.rst
+-rw-r--r--   0        0        0    71911 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/github-stats-0.13.rst
+-rw-r--r--   0        0        0   107462 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/github-stats-1.0.rst
+-rw-r--r--   0        0        0    87788 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/github-stats-2.0.rst
+-rw-r--r--   0        0        0     4973 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/github-stats-3.rst
+-rw-r--r--   0        0        0     3386 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/github-stats-4.rst
+-rw-r--r--   0        0        0     4399 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/github-stats-5.rst
+-rw-r--r--   0        0        0     3753 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/github-stats-6.rst
+-rw-r--r--   0        0        0    12480 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/github-stats-7.rst
+-rw-r--r--   0        0        0     2002 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/github-stats-8.rst
+-rw-r--r--   0        0        0     1803 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/index.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/source/whatsnew/pr/
+-rw-r--r--   0        0        0     1036 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/pr/README.md
+-rw-r--r--   0        0        0      124 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/pr/antigravity-feature.rst
+-rw-r--r--   0        0        0      255 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/pr/incompat-switching-to-perl.rst
+-rw-r--r--   0        0        0    15433 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version0.10.rst
+-rw-r--r--   0        0        0    34904 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version0.11.rst
+-rw-r--r--   0        0        0    16577 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version0.12.rst
+-rw-r--r--   0        0        0    28297 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version0.13.rst
+-rw-r--r--   0        0        0      912 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version0.8.rst
+-rw-r--r--   0        0        0    12469 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version0.9.rst
+-rw-r--r--   0        0        0    12949 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version1.0.rst
+-rw-r--r--   0        0        0    14061 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version2.0.rst
+-rw-r--r--   0        0        0    17305 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version3.rst
+-rw-r--r--   0        0        0    15393 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version3_widget_migration.rst
+-rw-r--r--   0        0        0     3407 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version4.rst
+-rw-r--r--   0        0        0    18391 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version5.rst
+-rw-r--r--   0        0        0    14330 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version6.rst
+-rw-r--r--   0        0        0    64879 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/source/whatsnew/version7.rst
+-rw-r--r--   0        0        0    52334 2023-01-27 09:44:19.000000 ipython-8.9.0/docs/source/whatsnew/version8.rst
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/docs/sphinxext/
+-rw-r--r--   0        0        0    17210 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/sphinxext/apigen.py
+-rw-r--r--   0        0        0      414 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/sphinxext/configtraits.py
+-rw-r--r--   0        0        0     5684 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/sphinxext/github.py
+-rw-r--r--   0        0        0     1496 2023-01-26 13:54:33.000000 ipython-8.9.0/docs/sphinxext/magics.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/examples/
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/examples/Embedding/
+-rw-r--r--   0        0        0     5074 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/Embedding/Index.ipynb
+-rwxr-xr-x   0        0        0     4849 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/Embedding/embed_class_long.py
+-rw-r--r--   0        0        0     1674 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/Embedding/embed_class_short.py
+-rw-r--r--   0        0        0      258 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/Embedding/embed_function.py
+-rwxr-xr-x   0        0        0      739 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/Embedding/start_ipython_config.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/examples/IPython Kernel/
+-rw-r--r--   0        0        0   107963 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Animations Using clear_output.ipynb
+-rw-r--r--   0        0        0    15419 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Background Jobs.ipynb
+-rw-r--r--   0        0        0   132731 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Beyond Plain Python.ipynb
+-rw-r--r--   0        0        0    19695 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Capturing Output.ipynb
+-rw-r--r--   0        0        0    16860 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Cell Magics.ipynb
+-rw-r--r--   0        0        0    83998 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Custom Display Logic.ipynb
+-rw-r--r--   0        0        0    22198 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Importing Notebooks.ipynb
+-rw-r--r--   0        0        0     4884 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Index.ipynb
+-rw-r--r--   0        0        0   370083 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Plotting in the Notebook.ipynb
+-rw-r--r--   0        0        0     6054 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Raw Input in the Notebook.ipynb
+-rw-r--r--   0        0        0   300702 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Rich Output.ipynb
+-rw-r--r--   0        0        0     9347 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Script Magics.ipynb
+-rw-r--r--   0        0        0   305111 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/SymPy.ipynb
+-rw-r--r--   0        0        0     5964 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Terminal Usage.ipynb
+-rw-r--r--   0        0        0   261308 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Third Party Rich Output.ipynb
+-rw-r--r--   0        0        0    75473 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Trapezoid Rule.ipynb
+-rw-r--r--   0        0        0     6953 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Updating Displays.ipynb
+-rw-r--r--   0        0        0    48173 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/Working With External Code.ipynb
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/examples/IPython Kernel/data/
+-rw-r--r--   0        0        0    11414 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/data/flare.json
+-rw-r--r--   0        0        0     1182 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/example-demo.py
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/examples/IPython Kernel/gui/
+-rwxr-xr-x   0        0        0     1297 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/gui/gui-glut.py
+-rw-r--r--   0        0        0      716 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/gui/gui-gtk4.py
+-rwxr-xr-x   0        0        0     1009 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/gui/gui-qt.py
+-rw-r--r--   0        0        0     4271 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/ipython-completion.bash
+-rwxr-xr-x   0        0        0     1136 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/ipython-get-history.py
+-rw-r--r--   0        0        0      400 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/ipython.desktop
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/examples/IPython Kernel/nbpackage/
+-rw-r--r--   0        0        0        0 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/nbpackage/__init__.py
+-rw-r--r--   0        0        0     1144 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/nbpackage/mynotebook.ipynb
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/examples/IPython Kernel/nbpackage/nbs/
+-rw-r--r--   0        0        0        0 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/nbpackage/nbs/__init__.py
+-rw-r--r--   0        0        0      748 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/IPython Kernel/nbpackage/nbs/other.ipynb
+-rw-r--r--   0        0        0     1458 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/Index.ipynb
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/examples/images/
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/examples/images/FrontendKernel.graffle/
+-rw-r--r--   0        0        0    10212 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/images/FrontendKernel.graffle/data.plist
+-rw-r--r--   0        0        0    14726 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/images/FrontendKernel.graffle/image1.png
+-rw-r--r--   0        0        0    33170 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/images/FrontendKernel.png
+-rw-r--r--   0        0        0    11903 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/images/animation.m4v
+-rw-r--r--   0        0        0     9216 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/images/ipython_logo.png
+-rw-r--r--   0        0        0    15301 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/images/python_logo.svg
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/examples/utils/
+-rw-r--r--   0        0        0      616 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/utils/cwd_prompt.py
+-rw-r--r--   0        0        0      182 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/utils/list_pyfiles.ipy
+-rw-r--r--   0        0        0      194 2023-01-26 13:54:33.000000 ipython-8.9.0/examples/utils/list_subdirs.ipy
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/ipython.egg-info/
+-rw-r--r--   0        0        0     2706 2023-01-27 11:56:59.000000 ipython-8.9.0/ipython.egg-info/PKG-INFO
+-rw-r--r--   0        0        0    16816 2023-01-27 11:56:59.000000 ipython-8.9.0/ipython.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-01-27 11:56:59.000000 ipython-8.9.0/ipython.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0      244 2023-01-27 11:56:59.000000 ipython-8.9.0/ipython.egg-info/entry_points.txt
+-rw-r--r--   0        0        0        1 2023-01-27 11:56:59.000000 ipython-8.9.0/ipython.egg-info/not-zip-safe
+-rw-r--r--   0        0        0      988 2023-01-27 11:56:59.000000 ipython-8.9.0/ipython.egg-info/requires.txt
+-rw-r--r--   0        0        0        8 2023-01-27 11:56:59.000000 ipython-8.9.0/ipython.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1387 2023-01-26 13:54:33.000000 ipython-8.9.0/long_description.rst
+-rw-r--r--   0        0        0       82 2023-01-26 13:54:33.000000 ipython-8.9.0/mypy.ini
+-rw-r--r--   0        0        0       91 2023-01-26 13:54:33.000000 ipython-8.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1419 2023-01-26 13:54:33.000000 ipython-8.9.0/pytest.ini
+drwxr-xr-x   0        0        0        0 2023-01-27 11:56:59.000000 ipython-8.9.0/scripts/
+-rw-r--r--   0        0        0    32580 2023-01-26 13:54:33.000000 ipython-8.9.0/scripts/ipython.ico
+-rw-r--r--   0        0        0    44204 2023-01-26 13:54:33.000000 ipython-8.9.0/scripts/ipython_nb.ico
+-rw-r--r--   0        0        0     2203 2023-01-27 11:56:59.000000 ipython-8.9.0/setup.cfg
+-rw-r--r--   0        0        0     5179 2023-01-26 13:54:33.000000 ipython-8.9.0/setup.py
+-rw-r--r--   0        0        0    11786 2023-01-26 13:54:33.000000 ipython-8.9.0/setupbase.py
```

### Comparing `ipython-8.8.0/.mailmap` & `ipython-8.9.0/.mailmap`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/COPYING.rst` & `ipython-8.9.0/COPYING.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/__init__.py` & `ipython-8.9.0/IPython/__init__.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/conftest.py` & `ipython-8.9.0/IPython/conftest.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/alias.py` & `ipython-8.9.0/IPython/core/alias.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/application.py` & `ipython-8.9.0/IPython/core/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,16 @@
                 )
             except ProfileDirError:
                 return
             path = profile_dir.location
         return super(ProfileAwareConfigLoader, self).load_subconfig(fname, path=path)
 
 class BaseIPythonApplication(Application):
-
-    name = u'ipython'
-    description = Unicode(u'IPython: an enhanced interactive Python shell.')
+    name = "ipython"
+    description = "IPython: an enhanced interactive Python shell."
     version = Unicode(release.version)
 
     aliases = base_aliases
     flags = base_flags
     classes = List([ProfileDir])
     
     # enable `load_subconfig('cfg.py', profile='name')`
@@ -307,15 +306,15 @@
             for d in ("extensions", "nbextensions"):
                 path = os.path.join(new, d)
                 try:
                     ensure_dir_exists(path)
                 except OSError as e:
                     # this will not be EEXIST
                     self.log.error("couldn't create path %s: %s", path, e)
-            self.log.debug("IPYTHONDIR set to: %s" % new)
+            self.log.debug("IPYTHONDIR set to: %s", new)
 
     def load_config_file(self, suppress_errors=IPYTHON_SUPPRESS_CONFIG_ERRORS):
         """Load the config file.
 
         By default, errors in loading config are handled, and a warning
         printed on screen. For testing, the suppress_errors option is set
         to False, so errors will make tests fail.
@@ -397,15 +396,15 @@
                         self.exit(1)
                     else:
                         self.log.info("Created profile dir: %r"%p.location)
                 else:
                     self.log.fatal("Profile %r not found."%self.profile)
                     self.exit(1)
             else:
-                self.log.debug(f"Using existing profile dir: {p.location!r}")
+                self.log.debug("Using existing profile dir: %r", p.location)
         else:
             location = self.config.ProfileDir.location
             # location is fully specified
             try:
                 p = ProfileDir.find_profile_dir(location, self.config)
             except ProfileDirError:
                 # not found, maybe create it
@@ -417,15 +416,15 @@
                         self.exit(1)
                     else:
                         self.log.debug("Creating new profile dir: %r"%location)
                 else:
                     self.log.fatal("Profile directory %r not found."%location)
                     self.exit(1)
             else:
-                self.log.debug(f"Using existing profile dir: {p.location!r}")
+                self.log.debug("Using existing profile dir: %r", p.location)
             # if profile_dir is specified explicitly, set profile name
             dir_name = os.path.basename(p.location)
             if dir_name.startswith('profile_'):
                 self.profile = dir_name[8:]
 
         self.profile_dir = p
         self.config_file_paths.append(p.location)
@@ -464,15 +463,15 @@
 
 
     def stage_default_config_file(self):
         """auto generate default config file, and stage it into the profile."""
         s = self.generate_config_file()
         config_file = Path(self.profile_dir.location) / self.config_file_name
         if self.overwrite or not config_file.exists():
-            self.log.warning("Generating default config file: %r" % (config_file))
+            self.log.warning("Generating default config file: %r", (config_file))
             config_file.write_text(s, encoding="utf-8")
 
     @catch_config_error
     def initialize(self, argv=None):
         # don't hook up crash handler before parsing command-line
         self.parse_command_line(argv)
         self.init_crash_handler()
```

### Comparing `ipython-8.8.0/IPython/core/async_helpers.py` & `ipython-8.9.0/IPython/core/async_helpers.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/autocall.py` & `ipython-8.9.0/IPython/core/autocall.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/builtin_trap.py` & `ipython-8.9.0/IPython/core/builtin_trap.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/compilerop.py` & `ipython-8.9.0/IPython/core/compilerop.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/completer.py` & `ipython-8.9.0/IPython/core/completer.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/completerlib.py` & `ipython-8.9.0/IPython/core/completerlib.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/crashhandler.py` & `ipython-8.9.0/IPython/core/crashhandler.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/debugger.py` & `ipython-8.9.0/IPython/core/debugger.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/display.py` & `ipython-8.9.0/IPython/core/display.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/display_functions.py` & `ipython-8.9.0/IPython/core/display_functions.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/display_trap.py` & `ipython-8.9.0/IPython/core/display_trap.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/displayhook.py` & `ipython-8.9.0/IPython/core/displayhook.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/displaypub.py` & `ipython-8.9.0/IPython/core/displaypub.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/error.py` & `ipython-8.9.0/IPython/core/error.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/events.py` & `ipython-8.9.0/IPython/core/events.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/excolors.py` & `ipython-8.9.0/IPython/core/excolors.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/extensions.py` & `ipython-8.9.0/IPython/core/extensions.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/formatters.py` & `ipython-8.9.0/IPython/core/formatters.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/getipython.py` & `ipython-8.9.0/IPython/core/getipython.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/guarded_eval.py` & `ipython-8.9.0/IPython/core/guarded_eval.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/history.py` & `ipython-8.9.0/IPython/core/history.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/historyapp.py` & `ipython-8.9.0/IPython/core/historyapp.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/hooks.py` & `ipython-8.9.0/IPython/core/hooks.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/inputsplitter.py` & `ipython-8.9.0/IPython/core/inputsplitter.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/inputtransformer.py` & `ipython-8.9.0/IPython/core/inputtransformer.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/inputtransformer2.py` & `ipython-8.9.0/IPython/core/inputtransformer2.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/interactiveshell.py` & `ipython-8.9.0/IPython/core/interactiveshell.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/latex_symbols.py` & `ipython-8.9.0/IPython/core/latex_symbols.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/logger.py` & `ipython-8.9.0/IPython/core/logger.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/macro.py` & `ipython-8.9.0/IPython/core/macro.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magic.py` & `ipython-8.9.0/IPython/core/magic.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magic_arguments.py` & `ipython-8.9.0/IPython/core/magic_arguments.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/__init__.py` & `ipython-8.9.0/IPython/core/magics/__init__.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/auto.py` & `ipython-8.9.0/IPython/core/magics/auto.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/basic.py` & `ipython-8.9.0/IPython/core/magics/basic.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/code.py` & `ipython-8.9.0/IPython/core/magics/code.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/config.py` & `ipython-8.9.0/IPython/core/magics/config.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/display.py` & `ipython-8.9.0/IPython/core/magics/display.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/execution.py` & `ipython-8.9.0/IPython/core/magics/execution.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/extension.py` & `ipython-8.9.0/IPython/core/magics/extension.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/history.py` & `ipython-8.9.0/IPython/core/magics/history.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/logging.py` & `ipython-8.9.0/IPython/core/magics/logging.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/namespace.py` & `ipython-8.9.0/IPython/core/magics/namespace.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/osm.py` & `ipython-8.9.0/IPython/core/magics/osm.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/packaging.py` & `ipython-8.9.0/IPython/core/magics/packaging.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/pylab.py` & `ipython-8.9.0/IPython/core/magics/pylab.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/magics/script.py` & `ipython-8.9.0/IPython/core/magics/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 
         def in_thread(coro):
             """Call a coroutine on the asyncio thread"""
             return asyncio.run_coroutine_threadsafe(coro, event_loop).result()
 
         async def _handle_stream(stream, stream_arg, file_object):
             while True:
-                line = (await stream.readline()).decode("utf8")
+                line = (await stream.readline()).decode("utf8", errors="replace")
                 if not line:
                     break
                 if stream_arg:
                     self.shell.user_ns[stream_arg] = line
                 else:
                     file_object.write(line)
                     file_object.flush()
```

### Comparing `ipython-8.8.0/IPython/core/oinspect.py` & `ipython-8.9.0/IPython/core/oinspect.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/page.py` & `ipython-8.9.0/IPython/core/page.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/payload.py` & `ipython-8.9.0/IPython/core/payload.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/payloadpage.py` & `ipython-8.9.0/IPython/core/payloadpage.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/prefilter.py` & `ipython-8.9.0/IPython/core/prefilter.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/profileapp.py` & `ipython-8.9.0/IPython/core/profileapp.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/profiledir.py` & `ipython-8.9.0/IPython/core/profiledir.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/prompts.py` & `ipython-8.9.0/IPython/core/prompts.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/pylabtools.py` & `ipython-8.9.0/IPython/core/pylabtools.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/release.py` & `ipython-8.9.0/IPython/core/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  The full license is in the file COPYING.txt, distributed with this software.
 #-----------------------------------------------------------------------------
 
 # IPython version information.  An empty _version_extra corresponds to a full
 # release.  'dev' as a _version_extra string means this is a development
 # version
 _version_major = 8
-_version_minor = 8
+_version_minor = 9
 _version_patch = 0
 _version_extra = ".dev"
 # _version_extra = "rc1"
 _version_extra = ""  # Uncomment this for full releases
 
 # Construct full version string from these.
 _ver = [_version_major, _version_minor, _version_patch]
```

### Comparing `ipython-8.8.0/IPython/core/shellapp.py` & `ipython-8.9.0/IPython/core/shellapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
         try:
             self.log.debug("Loading IPython extensions...")
             extensions = (
                 self.default_extensions + self.extensions + self.extra_extensions
             )
             for ext in extensions:
                 try:
-                    self.log.info("Loading IPython extension: %s" % ext)
+                    self.log.info("Loading IPython extension: %s", ext)
                     self.shell.extension_manager.load_extension(ext)
                 except:
                     if self.reraise_ipython_extension_failures:
                         raise
                     msg = ("Error in loading extension: {ext}\n"
                            "Check your config files in {location}".format(
                                ext=ext,
```

### Comparing `ipython-8.8.0/IPython/core/splitinput.py` & `ipython-8.9.0/IPython/core/splitinput.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/refbug.py` & `ipython-8.9.0/IPython/core/tests/refbug.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/simpleerr.py` & `ipython-8.9.0/IPython/core/tests/simpleerr.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/tclass.py` & `ipython-8.9.0/IPython/core/tests/tclass.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_alias.py` & `ipython-8.9.0/IPython/core/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_application.py` & `ipython-8.9.0/IPython/core/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_async_helpers.py` & `ipython-8.9.0/IPython/core/tests/test_async_helpers.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_autocall.py` & `ipython-8.9.0/IPython/core/tests/test_autocall.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_compilerop.py` & `ipython-8.9.0/IPython/core/tests/test_compilerop.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_completer.py` & `ipython-8.9.0/IPython/core/tests/test_completer.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_completerlib.py` & `ipython-8.9.0/IPython/core/tests/test_completerlib.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_debugger.py` & `ipython-8.9.0/IPython/core/tests/test_debugger.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_display.py` & `ipython-8.9.0/IPython/core/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_displayhook.py` & `ipython-8.9.0/IPython/core/tests/test_displayhook.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_events.py` & `ipython-8.9.0/IPython/core/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_extension.py` & `ipython-8.9.0/IPython/core/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_formatters.py` & `ipython-8.9.0/IPython/core/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_guarded_eval.py` & `ipython-8.9.0/IPython/core/tests/test_guarded_eval.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_handlers.py` & `ipython-8.9.0/IPython/core/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_history.py` & `ipython-8.9.0/IPython/core/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_hooks.py` & `ipython-8.9.0/IPython/core/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_imports.py` & `ipython-8.9.0/IPython/core/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_inputsplitter.py` & `ipython-8.9.0/IPython/core/tests/test_inputsplitter.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_inputtransformer.py` & `ipython-8.9.0/IPython/core/tests/test_inputtransformer.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_inputtransformer2.py` & `ipython-8.9.0/IPython/core/tests/test_inputtransformer2.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_inputtransformer2_line.py` & `ipython-8.9.0/IPython/core/tests/test_inputtransformer2_line.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_interactiveshell.py` & `ipython-8.9.0/IPython/core/tests/test_interactiveshell.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_iplib.py` & `ipython-8.9.0/IPython/core/tests/test_iplib.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_logger.py` & `ipython-8.9.0/IPython/core/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_magic.py` & `ipython-8.9.0/IPython/core/tests/test_magic.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_magic_arguments.py` & `ipython-8.9.0/IPython/core/tests/test_magic_arguments.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_magic_terminal.py` & `ipython-8.9.0/IPython/core/tests/test_magic_terminal.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_oinspect.py` & `ipython-8.9.0/IPython/core/tests/test_oinspect.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_page.py` & `ipython-8.9.0/IPython/core/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_paths.py` & `ipython-8.9.0/IPython/core/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_prefilter.py` & `ipython-8.9.0/IPython/core/tests/test_prefilter.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_profile.py` & `ipython-8.9.0/IPython/core/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_prompts.py` & `ipython-8.9.0/IPython/core/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_pylabtools.py` & `ipython-8.9.0/IPython/core/tests/test_pylabtools.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_run.py` & `ipython-8.9.0/IPython/core/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_shellapp.py` & `ipython-8.9.0/IPython/core/tests/test_shellapp.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_splitinput.py` & `ipython-8.9.0/IPython/core/tests/test_splitinput.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/tests/test_ultratb.py` & `ipython-8.9.0/IPython/core/tests/test_ultratb.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/ultratb.py` & `ipython-8.9.0/IPython/core/ultratb.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/core/usage.py` & `ipython-8.9.0/IPython/core/usage.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/display.py` & `ipython-8.9.0/IPython/display.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/extensions/autoreload.py` & `ipython-8.9.0/IPython/extensions/autoreload.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/extensions/storemagic.py` & `ipython-8.9.0/IPython/extensions/storemagic.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/extensions/tests/test_autoreload.py` & `ipython-8.9.0/IPython/extensions/tests/test_autoreload.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/extensions/tests/test_storemagic.py` & `ipython-8.9.0/IPython/extensions/tests/test_storemagic.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/external/qt_for_kernel.py` & `ipython-8.9.0/IPython/external/qt_for_kernel.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/external/qt_loaders.py` & `ipython-8.9.0/IPython/external/qt_loaders.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/backgroundjobs.py` & `ipython-8.9.0/IPython/lib/backgroundjobs.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/clipboard.py` & `ipython-8.9.0/IPython/lib/clipboard.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/deepreload.py` & `ipython-8.9.0/IPython/lib/deepreload.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/demo.py` & `ipython-8.9.0/IPython/lib/demo.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/display.py` & `ipython-8.9.0/IPython/lib/display.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/editorhooks.py` & `ipython-8.9.0/IPython/lib/editorhooks.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/guisupport.py` & `ipython-8.9.0/IPython/lib/guisupport.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/latextools.py` & `ipython-8.9.0/IPython/lib/latextools.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/lexers.py` & `ipython-8.9.0/IPython/lib/lexers.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/pretty.py` & `ipython-8.9.0/IPython/lib/pretty.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/tests/test.wav` & `ipython-8.9.0/IPython/lib/tests/test.wav`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/tests/test_backgroundjobs.py` & `ipython-8.9.0/IPython/lib/tests/test_backgroundjobs.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/tests/test_clipboard.py` & `ipython-8.9.0/IPython/lib/tests/test_clipboard.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/tests/test_deepreload.py` & `ipython-8.9.0/IPython/lib/tests/test_deepreload.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/tests/test_display.py` & `ipython-8.9.0/IPython/lib/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/tests/test_editorhooks.py` & `ipython-8.9.0/IPython/lib/tests/test_editorhooks.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/tests/test_latextools.py` & `ipython-8.9.0/IPython/lib/tests/test_latextools.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/tests/test_lexers.py` & `ipython-8.9.0/IPython/lib/tests/test_lexers.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/tests/test_pretty.py` & `ipython-8.9.0/IPython/lib/tests/test_pretty.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/lib/tests/test_pygments.py` & `ipython-8.9.0/IPython/lib/tests/test_pygments.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/paths.py` & `ipython-8.9.0/IPython/paths.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/sphinxext/custom_doctests.py` & `ipython-8.9.0/IPython/sphinxext/custom_doctests.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/sphinxext/ipython_console_highlighting.py` & `ipython-8.9.0/IPython/sphinxext/ipython_console_highlighting.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/sphinxext/ipython_directive.py` & `ipython-8.9.0/IPython/sphinxext/ipython_directive.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/console.py` & `ipython-8.9.0/IPython/terminal/console.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/debugger.py` & `ipython-8.9.0/IPython/terminal/debugger.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/embed.py` & `ipython-8.9.0/IPython/terminal/embed.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/interactiveshell.py` & `ipython-8.9.0/IPython/terminal/interactiveshell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """IPython terminal interface using prompt_toolkit"""
 
 import asyncio
 import os
 import sys
 from warnings import warn
+from typing import Union as UnionType
 
 from IPython.core.async_helpers import get_asyncio_loop
 from IPython.core.interactiveshell import InteractiveShell, InteractiveShellABC
 from IPython.utils.py3compat import input
 from IPython.utils.terminal import toggle_set_term_title, set_term_title, restore_term_title
 from IPython.utils.process import abbrev_cwd
 from traitlets import (
@@ -45,14 +46,18 @@
 
 from .debugger import TerminalPdb, Pdb
 from .magics import TerminalMagics
 from .pt_inputhooks import get_inputhook_name_and_func
 from .prompts import Prompts, ClassicPrompts, RichPromptDisplayHook
 from .ptutils import IPythonPTCompleter, IPythonPTLexer
 from .shortcuts import create_ipython_shortcuts
+from .shortcuts.auto_suggest import (
+    NavigableAutoSuggestFromHistory,
+    AppendAutoSuggestionInAnyLine,
+)
 
 PTK3 = ptk_version.startswith('3.')
 
 
 class _NoStyle(Style): pass
 
 
@@ -138,14 +143,18 @@
 class PtkHistoryAdapter(History):
     """
     Prompt toolkit has it's own way of handling history, Where it assumes it can
     Push/pull from history.
 
     """
 
+    auto_suggest: UnionType[
+        AutoSuggestFromHistory, NavigableAutoSuggestFromHistory, None
+    ]
+
     def __init__(self, shell):
         super().__init__()
         self.shell = shell
         self._refresh()
 
     def append_string(self, string):
         # we rely on sql for that.
@@ -179,15 +188,15 @@
                                      'to reserve for the tab completion menu, '
                                      'search history, ...etc, the height of '
                                      'these menus will at most this value. '
                                      'Increase it is you prefer long and skinny '
                                      'menus, decrease for short and wide.'
                             ).tag(config=True)
 
-    pt_app = None
+    pt_app: UnionType[PromptSession, None] = None
     debugger_history = None
 
     debugger_history_file = Unicode(
         "~/.pdbhistory", help="File in which to store and read history"
     ).tag(config=True)
 
     simple_prompt = Bool(_use_simple_prompt,
@@ -372,26 +381,35 @@
     ).tag(config=True)
 
     enable_history_search = Bool(True,
         help="Allows to enable/disable the prompt toolkit history search"
     ).tag(config=True)
 
     autosuggestions_provider = Unicode(
-        "AutoSuggestFromHistory",
+        "NavigableAutoSuggestFromHistory",
         help="Specifies from which source automatic suggestions are provided. "
-        "Can be set to `'AutoSuggestFromHistory`' or `None` to disable"
-        "automatic suggestions. Default is `'AutoSuggestFromHistory`'.",
+        "Can be set to ``'NavigableAutoSuggestFromHistory'`` (:kbd:`up` and "
+        ":kbd:`down` swap suggestions), ``'AutoSuggestFromHistory'``, "
+        " or ``None`` to disable automatic suggestions. "
+        "Default is `'NavigableAutoSuggestFromHistory`'.",
         allow_none=True,
     ).tag(config=True)
 
     def _set_autosuggestions(self, provider):
+        # disconnect old handler
+        if self.auto_suggest and isinstance(
+            self.auto_suggest, NavigableAutoSuggestFromHistory
+        ):
+            self.auto_suggest.disconnect()
         if provider is None:
             self.auto_suggest = None
         elif provider == "AutoSuggestFromHistory":
             self.auto_suggest = AutoSuggestFromHistory()
+        elif provider == "NavigableAutoSuggestFromHistory":
+            self.auto_suggest = NavigableAutoSuggestFromHistory()
         else:
             raise ValueError("No valid provider.")
         if self.pt_app:
             self.pt_app.auto_suggest = self.auto_suggest
 
     @observe("autosuggestions_provider")
     def _autosuggestions_provider_changed(self, change):
@@ -458,14 +476,16 @@
             include_default_pygments_style=False,
             mouse_support=self.mouse_support,
             enable_open_in_editor=self.extra_open_editor_shortcuts,
             color_depth=self.color_depth,
             tempfile_suffix=".py",
             **self._extra_prompt_options()
         )
+        if isinstance(self.auto_suggest, NavigableAutoSuggestFromHistory):
+            self.auto_suggest.connect(self.pt_app)
 
     def _make_style_from_name_or_cls(self, name_or_cls):
         """
         Small wrapper that make an IPython compatible style from a style name
 
         We need that to add style for prompt ... etc.
         """
@@ -556,31 +576,47 @@
             # here I'm going to favor the default keybinding which almost
             # everybody uses to decrease CPU usage.
             # if we have issues with users with custom Prompts we can see how to
             # work around this.
             get_message = get_message()
 
         options = {
-                'complete_in_thread': False,
-                'lexer':IPythonPTLexer(),
-                'reserve_space_for_menu':self.space_for_menu,
-                'message': get_message,
-                'prompt_continuation': (
-                    lambda width, lineno, is_soft_wrap:
-                        PygmentsTokens(self.prompts.continuation_prompt_tokens(width))),
-                'multiline': True,
-                'complete_style': self.pt_complete_style,
-
+            "complete_in_thread": False,
+            "lexer": IPythonPTLexer(),
+            "reserve_space_for_menu": self.space_for_menu,
+            "message": get_message,
+            "prompt_continuation": (
+                lambda width, lineno, is_soft_wrap: PygmentsTokens(
+                    self.prompts.continuation_prompt_tokens(width)
+                )
+            ),
+            "multiline": True,
+            "complete_style": self.pt_complete_style,
+            "input_processors": [
                 # Highlight matching brackets, but only when this setting is
                 # enabled, and only when the DEFAULT_BUFFER has the focus.
-                'input_processors': [ConditionalProcessor(
-                        processor=HighlightMatchingBracketProcessor(chars='[](){}'),
-                        filter=HasFocus(DEFAULT_BUFFER) & ~IsDone() &
-                            Condition(lambda: self.highlight_matching_brackets))],
-                }
+                ConditionalProcessor(
+                    processor=HighlightMatchingBracketProcessor(chars="[](){}"),
+                    filter=HasFocus(DEFAULT_BUFFER)
+                    & ~IsDone()
+                    & Condition(lambda: self.highlight_matching_brackets),
+                ),
+                # Show auto-suggestion in lines other than the last line.
+                ConditionalProcessor(
+                    processor=AppendAutoSuggestionInAnyLine(),
+                    filter=HasFocus(DEFAULT_BUFFER)
+                    & ~IsDone()
+                    & Condition(
+                        lambda: isinstance(
+                            self.auto_suggest, NavigableAutoSuggestFromHistory
+                        )
+                    ),
+                ),
+            ],
+        }
         if not PTK3:
             options['inputhook'] = self.inputhook
 
         return options
 
     def prompt_for_code(self):
         if self.rl_next_input:
@@ -643,16 +679,17 @@
         # need direct access to the console in a way that we can't emulate in
         # GUI or web frontend
         if os.name == 'posix':
             for cmd in ('clear', 'more', 'less', 'man'):
                 self.alias_manager.soft_define_alias(cmd, cmd)
 
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super(TerminalInteractiveShell, self).__init__(*args, **kwargs)
+        self.auto_suggest = None
         self._set_autosuggestions(self.autosuggestions_provider)
         self.init_prompt_toolkit_cli()
         self.init_term_title()
         self.keep_running = True
         self._set_formatter(self.autoformatter)
```

### Comparing `ipython-8.8.0/IPython/terminal/ipapp.py` & `ipython-8.9.0/IPython/terminal/ipapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     It is often useful to follow this with `--` to treat remaining flags as
     script arguments.
     """
 )
 flags.update(frontend_flags)
 
 aliases = dict(base_aliases)
-aliases.update(shell_aliases)
+aliases.update(shell_aliases)  # type: ignore[arg-type]
 
 #-----------------------------------------------------------------------------
 # Main classes and functions
 #-----------------------------------------------------------------------------
 
 
 class LocateIPythonApp(BaseIPythonApplication):
@@ -176,15 +176,15 @@
         else:
             print(self.ipython_dir)
 
 
 class TerminalIPythonApp(BaseIPythonApplication, InteractiveShellApp):
     name = u'ipython'
     description = usage.cl_usage
-    crash_handler_class = IPAppCrashHandler
+    crash_handler_class = IPAppCrashHandler  # typing: ignore[assignment]
     examples = _examples
 
     flags = flags
     aliases = aliases
     classes = List()
 
     interactive_shell_class = Type(
```

### Comparing `ipython-8.8.0/IPython/terminal/magics.py` & `ipython-8.9.0/IPython/terminal/magics.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/prompts.py` & `ipython-8.9.0/IPython/terminal/prompts.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/pt_inputhooks/__init__.py` & `ipython-8.9.0/IPython/terminal/pt_inputhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/pt_inputhooks/asyncio.py` & `ipython-8.9.0/IPython/terminal/pt_inputhooks/asyncio.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/pt_inputhooks/glut.py` & `ipython-8.9.0/IPython/terminal/pt_inputhooks/glut.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/pt_inputhooks/gtk.py` & `ipython-8.9.0/IPython/terminal/pt_inputhooks/gtk.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/pt_inputhooks/gtk4.py` & `ipython-8.9.0/IPython/terminal/pt_inputhooks/gtk4.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/pt_inputhooks/osx.py` & `ipython-8.9.0/IPython/terminal/pt_inputhooks/osx.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/pt_inputhooks/pyglet.py` & `ipython-8.9.0/IPython/terminal/pt_inputhooks/pyglet.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/pt_inputhooks/qt.py` & `ipython-8.9.0/IPython/terminal/pt_inputhooks/qt.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/pt_inputhooks/tk.py` & `ipython-8.9.0/IPython/terminal/pt_inputhooks/tk.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/pt_inputhooks/wx.py` & `ipython-8.9.0/IPython/terminal/pt_inputhooks/wx.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/ptutils.py` & `ipython-8.9.0/IPython/terminal/ptutils.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/shortcuts.py` & `ipython-8.9.0/IPython/terminal/shortcuts/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,114 +2,161 @@
 Module to define and register Terminal IPython shortcuts with
 :mod:`prompt_toolkit`
 """
 
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 
-import warnings
+import os
+import re
 import signal
 import sys
-import re
-import os
-from typing import Callable
-
+import warnings
+from typing import Callable, Dict, Union
 
 from prompt_toolkit.application.current import get_app
 from prompt_toolkit.enums import DEFAULT_BUFFER, SEARCH_BUFFER
-from prompt_toolkit.filters import (has_focus, has_selection, Condition,
-    vi_insert_mode, emacs_insert_mode, has_completions, vi_mode)
-from prompt_toolkit.key_binding.bindings.completion import display_completions_like_readline
+from prompt_toolkit.filters import Condition, emacs_insert_mode, has_completions
+from prompt_toolkit.filters import has_focus as has_focus_impl
+from prompt_toolkit.filters import (
+    has_selection,
+    has_suggestion,
+    vi_insert_mode,
+    vi_mode,
+)
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.key_binding.bindings import named_commands as nc
+from prompt_toolkit.key_binding.bindings.completion import (
+    display_completions_like_readline,
+)
 from prompt_toolkit.key_binding.vi_state import InputMode, ViState
+from prompt_toolkit.layout.layout import FocusableElement
 
+from IPython.terminal.shortcuts import auto_match as match
+from IPython.terminal.shortcuts import auto_suggest
 from IPython.utils.decorators import undoc
 
+__all__ = ["create_ipython_shortcuts"]
+
+
 @undoc
 @Condition
 def cursor_in_leading_ws():
     before = get_app().current_buffer.document.current_line_before_cursor
     return (not before) or before.isspace()
 
 
-# Needed for to accept autosuggestions in vi insert mode
-def _apply_autosuggest(event):
-    """
-    Apply autosuggestion if at end of line.
-    """
-    b = event.current_buffer
-    d = b.document
-    after_cursor = d.text[d.cursor_position :]
-    lines = after_cursor.split("\n")
-    end_of_current_line = lines[0].strip()
-    suggestion = b.suggestion
-    if (suggestion is not None) and (suggestion.text) and (end_of_current_line == ""):
-        b.insert_text(suggestion.text)
-    else:
-        nc.end_of_line(event)
+def has_focus(value: FocusableElement):
+    """Wrapper around has_focus adding a nice `__name__` to tester function"""
+    tester = has_focus_impl(value).func
+    tester.__name__ = f"is_focused({value})"
+    return Condition(tester)
+
+
+@undoc
+@Condition
+def has_line_below() -> bool:
+    document = get_app().current_buffer.document
+    return document.cursor_position_row < len(document.lines) - 1
 
-def create_ipython_shortcuts(shell):
-    """Set up the prompt_toolkit keyboard shortcuts for IPython"""
+
+@undoc
+@Condition
+def has_line_above() -> bool:
+    document = get_app().current_buffer.document
+    return document.cursor_position_row != 0
+
+
+def create_ipython_shortcuts(shell, for_all_platforms: bool = False) -> KeyBindings:
+    """Set up the prompt_toolkit keyboard shortcuts for IPython.
+
+    Parameters
+    ----------
+    shell: InteractiveShell
+        The current IPython shell Instance
+    for_all_platforms: bool (default false)
+        This parameter is mostly used in generating the documentation
+        to create the shortcut binding for all the platforms, and export
+        them.
+
+    Returns
+    -------
+    KeyBindings
+        the keybinding instance for prompt toolkit.
+
+    """
+    # Warning: if possible, do NOT define handler functions in the locals
+    # scope of this function, instead define functions in the global
+    # scope, or a separate module, and include a user-friendly docstring
+    # describing the action.
 
     kb = KeyBindings()
     insert_mode = vi_insert_mode | emacs_insert_mode
 
-    if getattr(shell, 'handle_return', None):
+    if getattr(shell, "handle_return", None):
         return_handler = shell.handle_return(shell)
     else:
         return_handler = newline_or_execute_outer(shell)
 
-    kb.add('enter', filter=(has_focus(DEFAULT_BUFFER)
-                            & ~has_selection
-                            & insert_mode
-                        ))(return_handler)
-
-    def reformat_and_execute(event):
-        reformat_text_before_cursor(event.current_buffer, event.current_buffer.document, shell)
-        event.current_buffer.validate_and_handle()
+    kb.add("enter", filter=(has_focus(DEFAULT_BUFFER) & ~has_selection & insert_mode))(
+        return_handler
+    )
 
     @Condition
     def ebivim():
         return shell.emacs_bindings_in_vi_insert_mode
 
-    kb.add(
+    @kb.add(
         "escape",
         "enter",
         filter=(has_focus(DEFAULT_BUFFER) & ~has_selection & insert_mode & ebivim),
-    )(reformat_and_execute)
+    )
+    def reformat_and_execute(event):
+        """Reformat code and execute it"""
+        reformat_text_before_cursor(
+            event.current_buffer, event.current_buffer.document, shell
+        )
+        event.current_buffer.validate_and_handle()
 
     kb.add("c-\\")(quit)
 
-    kb.add('c-p', filter=(vi_insert_mode & has_focus(DEFAULT_BUFFER))
-                )(previous_history_or_previous_completion)
+    kb.add("c-p", filter=(vi_insert_mode & has_focus(DEFAULT_BUFFER)))(
+        previous_history_or_previous_completion
+    )
 
-    kb.add('c-n', filter=(vi_insert_mode & has_focus(DEFAULT_BUFFER))
-                )(next_history_or_next_completion)
+    kb.add("c-n", filter=(vi_insert_mode & has_focus(DEFAULT_BUFFER)))(
+        next_history_or_next_completion
+    )
 
-    kb.add('c-g', filter=(has_focus(DEFAULT_BUFFER) & has_completions)
-                )(dismiss_completion)
+    kb.add("c-g", filter=(has_focus(DEFAULT_BUFFER) & has_completions))(
+        dismiss_completion
+    )
 
-    kb.add('c-c', filter=has_focus(DEFAULT_BUFFER))(reset_buffer)
+    kb.add("c-c", filter=has_focus(DEFAULT_BUFFER))(reset_buffer)
 
-    kb.add('c-c', filter=has_focus(SEARCH_BUFFER))(reset_search_buffer)
+    kb.add("c-c", filter=has_focus(SEARCH_BUFFER))(reset_search_buffer)
 
-    supports_suspend = Condition(lambda: hasattr(signal, 'SIGTSTP'))
-    kb.add('c-z', filter=supports_suspend)(suspend_to_bg)
+    supports_suspend = Condition(lambda: hasattr(signal, "SIGTSTP"))
+    kb.add("c-z", filter=supports_suspend)(suspend_to_bg)
 
     # Ctrl+I == Tab
-    kb.add('tab', filter=(has_focus(DEFAULT_BUFFER)
-                          & ~has_selection
-                          & insert_mode
-                          & cursor_in_leading_ws
-                        ))(indent_buffer)
-    kb.add('c-o', filter=(has_focus(DEFAULT_BUFFER) & emacs_insert_mode)
-           )(newline_autoindent_outer(shell.input_transformer_manager))
+    kb.add(
+        "tab",
+        filter=(
+            has_focus(DEFAULT_BUFFER)
+            & ~has_selection
+            & insert_mode
+            & cursor_in_leading_ws
+        ),
+    )(indent_buffer)
+    kb.add("c-o", filter=(has_focus(DEFAULT_BUFFER) & emacs_insert_mode))(
+        newline_autoindent_outer(shell.input_transformer_manager)
+    )
 
-    kb.add('f2', filter=has_focus(DEFAULT_BUFFER))(open_input_in_editor)
+    kb.add("f2", filter=has_focus(DEFAULT_BUFFER))(open_input_in_editor)
 
     @Condition
     def auto_match():
         return shell.auto_match
 
     def all_quotes_paired(quote, buf):
         paired = True
@@ -120,36 +167,39 @@
                 paired = not paired
             elif c == "\\":
                 i += 1
             i += 1
         return paired
 
     focused_insert = (vi_insert_mode | emacs_insert_mode) & has_focus(DEFAULT_BUFFER)
-    _preceding_text_cache = {}
-    _following_text_cache = {}
+    _preceding_text_cache: Dict[Union[str, Callable], Condition] = {}
+    _following_text_cache: Dict[Union[str, Callable], Condition] = {}
 
-    def preceding_text(pattern):
+    def preceding_text(pattern: Union[str, Callable]):
         if pattern in _preceding_text_cache:
             return _preceding_text_cache[pattern]
 
         if callable(pattern):
 
             def _preceding_text():
                 app = get_app()
                 before_cursor = app.current_buffer.document.current_line_before_cursor
-                return bool(pattern(before_cursor))
+                # mypy can't infer if(callable): https://github.com/python/mypy/issues/3603
+                return bool(pattern(before_cursor))  # type: ignore[operator]
 
         else:
             m = re.compile(pattern)
 
             def _preceding_text():
                 app = get_app()
                 before_cursor = app.current_buffer.document.current_line_before_cursor
                 return bool(m.match(before_cursor))
 
+            _preceding_text.__name__ = f"preceding_text({pattern!r})"
+
         condition = Condition(_preceding_text)
         _preceding_text_cache[pattern] = condition
         return condition
 
     def following_text(pattern):
         try:
             return _following_text_cache[pattern]
@@ -157,14 +207,16 @@
             pass
         m = re.compile(pattern)
 
         def _following_text():
             app = get_app()
             return bool(m.match(app.current_buffer.document.current_line_after_cursor))
 
+        _following_text.__name__ = f"following_text({pattern!r})"
+
         condition = Condition(_following_text)
         _following_text_cache[pattern] = condition
         return condition
 
     @Condition
     def not_inside_unclosed_string():
         app = get_app()
@@ -174,202 +226,183 @@
         # remove triple-quoted string literals
         s = re.sub(r"(?:\"\"\"[\s\S]*\"\"\"|'''[\s\S]*''')", "", s)
         # remove single-quoted string literals
         s = re.sub(r"""(?:"[^"]*["\n]|'[^']*['\n])""", "", s)
         return not ('"' in s or "'" in s)
 
     # auto match
-    @kb.add("(", filter=focused_insert & auto_match & following_text(r"[,)}\]]|$"))
-    def _(event):
-        event.current_buffer.insert_text("()")
-        event.current_buffer.cursor_left()
-
-    @kb.add("[", filter=focused_insert & auto_match & following_text(r"[,)}\]]|$"))
-    def _(event):
-        event.current_buffer.insert_text("[]")
-        event.current_buffer.cursor_left()
-
-    @kb.add("{", filter=focused_insert & auto_match & following_text(r"[,)}\]]|$"))
-    def _(event):
-        event.current_buffer.insert_text("{}")
-        event.current_buffer.cursor_left()
+    for key, cmd in match.auto_match_parens.items():
+        kb.add(key, filter=focused_insert & auto_match & following_text(r"[,)}\]]|$"))(
+            cmd
+        )
 
-    @kb.add(
+    # raw string
+    for key, cmd in match.auto_match_parens_raw_string.items():
+        kb.add(
+            key,
+            filter=focused_insert & auto_match & preceding_text(r".*(r|R)[\"'](-*)$"),
+        )(cmd)
+
+    kb.add(
         '"',
         filter=focused_insert
         & auto_match
         & not_inside_unclosed_string
         & preceding_text(lambda line: all_quotes_paired('"', line))
         & following_text(r"[,)}\]]|$"),
-    )
-    def _(event):
-        event.current_buffer.insert_text('""')
-        event.current_buffer.cursor_left()
+    )(match.double_quote)
 
-    @kb.add(
+    kb.add(
         "'",
         filter=focused_insert
         & auto_match
         & not_inside_unclosed_string
         & preceding_text(lambda line: all_quotes_paired("'", line))
         & following_text(r"[,)}\]]|$"),
-    )
-    def _(event):
-        event.current_buffer.insert_text("''")
-        event.current_buffer.cursor_left()
+    )(match.single_quote)
 
-    @kb.add(
+    kb.add(
         '"',
         filter=focused_insert
         & auto_match
         & not_inside_unclosed_string
         & preceding_text(r'^.*""$'),
-    )
-    def _(event):
-        event.current_buffer.insert_text('""""')
-        event.current_buffer.cursor_left(3)
+    )(match.docstring_double_quotes)
 
-    @kb.add(
+    kb.add(
         "'",
         filter=focused_insert
         & auto_match
         & not_inside_unclosed_string
         & preceding_text(r"^.*''$"),
-    )
-    def _(event):
-        event.current_buffer.insert_text("''''")
-        event.current_buffer.cursor_left(3)
+    )(match.docstring_single_quotes)
 
-    # raw string
-    @kb.add(
-        "(", filter=focused_insert & auto_match & preceding_text(r".*(r|R)[\"'](-*)$")
+    # just move cursor
+    kb.add(")", filter=focused_insert & auto_match & following_text(r"^\)"))(
+        match.skip_over
     )
-    def _(event):
-        matches = re.match(
-            r".*(r|R)[\"'](-*)",
-            event.current_buffer.document.current_line_before_cursor,
-        )
-        dashes = matches.group(2) or ""
-        event.current_buffer.insert_text("()" + dashes)
-        event.current_buffer.cursor_left(len(dashes) + 1)
-
-    @kb.add(
-        "[", filter=focused_insert & auto_match & preceding_text(r".*(r|R)[\"'](-*)$")
+    kb.add("]", filter=focused_insert & auto_match & following_text(r"^\]"))(
+        match.skip_over
     )
-    def _(event):
-        matches = re.match(
-            r".*(r|R)[\"'](-*)",
-            event.current_buffer.document.current_line_before_cursor,
-        )
-        dashes = matches.group(2) or ""
-        event.current_buffer.insert_text("[]" + dashes)
-        event.current_buffer.cursor_left(len(dashes) + 1)
-
-    @kb.add(
-        "{", filter=focused_insert & auto_match & preceding_text(r".*(r|R)[\"'](-*)$")
+    kb.add("}", filter=focused_insert & auto_match & following_text(r"^\}"))(
+        match.skip_over
+    )
+    kb.add('"', filter=focused_insert & auto_match & following_text('^"'))(
+        match.skip_over
+    )
+    kb.add("'", filter=focused_insert & auto_match & following_text("^'"))(
+        match.skip_over
     )
-    def _(event):
-        matches = re.match(
-            r".*(r|R)[\"'](-*)",
-            event.current_buffer.document.current_line_before_cursor,
-        )
-        dashes = matches.group(2) or ""
-        event.current_buffer.insert_text("{}" + dashes)
-        event.current_buffer.cursor_left(len(dashes) + 1)
-
-    # just move cursor
-    @kb.add(")", filter=focused_insert & auto_match & following_text(r"^\)"))
-    @kb.add("]", filter=focused_insert & auto_match & following_text(r"^\]"))
-    @kb.add("}", filter=focused_insert & auto_match & following_text(r"^\}"))
-    @kb.add('"', filter=focused_insert & auto_match & following_text('^"'))
-    @kb.add("'", filter=focused_insert & auto_match & following_text("^'"))
-    def _(event):
-        event.current_buffer.cursor_right()
 
-    @kb.add(
+    kb.add(
         "backspace",
         filter=focused_insert
         & preceding_text(r".*\($")
         & auto_match
         & following_text(r"^\)"),
-    )
-    @kb.add(
+    )(match.delete_pair)
+    kb.add(
         "backspace",
         filter=focused_insert
         & preceding_text(r".*\[$")
         & auto_match
         & following_text(r"^\]"),
-    )
-    @kb.add(
+    )(match.delete_pair)
+    kb.add(
         "backspace",
         filter=focused_insert
         & preceding_text(r".*\{$")
         & auto_match
         & following_text(r"^\}"),
-    )
-    @kb.add(
+    )(match.delete_pair)
+    kb.add(
         "backspace",
         filter=focused_insert
         & preceding_text('.*"$')
         & auto_match
         & following_text('^"'),
-    )
-    @kb.add(
+    )(match.delete_pair)
+    kb.add(
         "backspace",
         filter=focused_insert
         & preceding_text(r".*'$")
         & auto_match
         & following_text(r"^'"),
-    )
-    def _(event):
-        event.current_buffer.delete()
-        event.current_buffer.delete_before_cursor()
+    )(match.delete_pair)
 
     if shell.display_completions == "readlinelike":
         kb.add(
             "c-i",
             filter=(
                 has_focus(DEFAULT_BUFFER)
                 & ~has_selection
                 & insert_mode
                 & ~cursor_in_leading_ws
             ),
         )(display_completions_like_readline)
 
-    if sys.platform == "win32":
+    if sys.platform == "win32" or for_all_platforms:
         kb.add("c-v", filter=(has_focus(DEFAULT_BUFFER) & ~vi_mode))(win_paste)
 
     focused_insert_vi = has_focus(DEFAULT_BUFFER) & vi_insert_mode
 
-    @kb.add("end", filter=has_focus(DEFAULT_BUFFER) & (ebivim | ~vi_insert_mode))
-    def _(event):
-        _apply_autosuggest(event)
-
-    @kb.add("c-e", filter=focused_insert_vi & ebivim)
-    def _(event):
-        _apply_autosuggest(event)
-
-    @kb.add("c-f", filter=focused_insert_vi)
-    def _(event):
-        b = event.current_buffer
-        suggestion = b.suggestion
-        if suggestion:
-            b.insert_text(suggestion.text)
-        else:
-            nc.forward_char(event)
+    # autosuggestions
+    @Condition
+    def navigable_suggestions():
+        return isinstance(
+            shell.auto_suggest, auto_suggest.NavigableAutoSuggestFromHistory
+        )
 
-    @kb.add("escape", "f", filter=focused_insert_vi & ebivim)
-    def _(event):
-        b = event.current_buffer
-        suggestion = b.suggestion
-        if suggestion:
-            t = re.split(r"(\S+\s+)", suggestion.text)
-            b.insert_text(next((x for x in t if x), ""))
-        else:
-            nc.forward_word(event)
+    kb.add("end", filter=has_focus(DEFAULT_BUFFER) & (ebivim | ~vi_insert_mode))(
+        auto_suggest.accept_in_vi_insert_mode
+    )
+    kb.add("c-e", filter=focused_insert_vi & ebivim)(
+        auto_suggest.accept_in_vi_insert_mode
+    )
+    kb.add("c-f", filter=focused_insert_vi)(auto_suggest.accept)
+    kb.add("escape", "f", filter=focused_insert_vi & ebivim)(auto_suggest.accept_word)
+    kb.add("c-right", filter=has_suggestion & has_focus(DEFAULT_BUFFER))(
+        auto_suggest.accept_token
+    )
+    kb.add(
+        "escape", filter=has_suggestion & has_focus(DEFAULT_BUFFER) & emacs_insert_mode
+    )(auto_suggest.discard)
+    kb.add(
+        "up",
+        filter=navigable_suggestions
+        & ~has_line_above
+        & has_suggestion
+        & has_focus(DEFAULT_BUFFER),
+    )(auto_suggest.swap_autosuggestion_up(shell.auto_suggest))
+    kb.add(
+        "down",
+        filter=navigable_suggestions
+        & ~has_line_below
+        & has_suggestion
+        & has_focus(DEFAULT_BUFFER),
+    )(auto_suggest.swap_autosuggestion_down(shell.auto_suggest))
+    kb.add(
+        "up", filter=has_line_above & navigable_suggestions & has_focus(DEFAULT_BUFFER)
+    )(auto_suggest.up_and_update_hint)
+    kb.add(
+        "down",
+        filter=has_line_below & navigable_suggestions & has_focus(DEFAULT_BUFFER),
+    )(auto_suggest.down_and_update_hint)
+    kb.add("right", filter=has_suggestion & has_focus(DEFAULT_BUFFER))(
+        auto_suggest.accept_character
+    )
+    kb.add("c-left", filter=has_suggestion & has_focus(DEFAULT_BUFFER))(
+        auto_suggest.accept_and_move_cursor_left
+    )
+    kb.add("c-down", filter=has_suggestion & has_focus(DEFAULT_BUFFER))(
+        auto_suggest.accept_and_keep_cursor
+    )
+    kb.add("backspace", filter=has_suggestion & has_focus(DEFAULT_BUFFER))(
+        auto_suggest.backspace_and_resume_hint
+    )
 
     # Simple Control keybindings
     key_cmd_dict = {
         "c-a": nc.beginning_of_line,
         "c-b": nc.backward_char,
         "c-k": nc.kill_line,
         "c-w": nc.backward_kill_word,
@@ -412,31 +445,29 @@
 
         sys.stdout.write(cursor)
         sys.stdout.flush()
 
         self._input_mode = mode
 
     if shell.editing_mode == "vi" and shell.modal_cursor:
-        ViState._input_mode = InputMode.INSERT
-        ViState.input_mode = property(get_input_mode, set_input_mode)
-
+        ViState._input_mode = InputMode.INSERT  # type: ignore
+        ViState.input_mode = property(get_input_mode, set_input_mode)  # type: ignore
     return kb
 
 
 def reformat_text_before_cursor(buffer, document, shell):
-    text = buffer.delete_before_cursor(len(document.text[:document.cursor_position]))
+    text = buffer.delete_before_cursor(len(document.text[: document.cursor_position]))
     try:
         formatted_text = shell.reformat_handler(text)
         buffer.insert_text(formatted_text)
     except Exception as e:
         buffer.insert_text(text)
 
 
 def newline_or_execute_outer(shell):
-
     def newline_or_execute(event):
         """When the user presses return, insert a newline or execute the code."""
         b = event.current_buffer
         d = b.document
 
         if b.complete_state:
             cc = b.complete_state.current_completion
@@ -447,42 +478,46 @@
             return
 
         # If there's only one line, treat it as if the cursor is at the end.
         # See https://github.com/ipython/ipython/issues/10425
         if d.line_count == 1:
             check_text = d.text
         else:
-            check_text = d.text[:d.cursor_position]
+            check_text = d.text[: d.cursor_position]
         status, indent = shell.check_complete(check_text)
-       
+
         # if all we have after the cursor is whitespace: reformat current text
         # before cursor
-        after_cursor = d.text[d.cursor_position:]
+        after_cursor = d.text[d.cursor_position :]
         reformatted = False
         if not after_cursor.strip():
             reformat_text_before_cursor(b, d, shell)
             reformatted = True
-        if not (d.on_last_line or
-                d.cursor_position_row >= d.line_count - d.empty_line_count_at_the_end()
-                ):
+        if not (
+            d.on_last_line
+            or d.cursor_position_row >= d.line_count - d.empty_line_count_at_the_end()
+        ):
             if shell.autoindent:
-                b.insert_text('\n' + indent)
+                b.insert_text("\n" + indent)
             else:
-                b.insert_text('\n')
+                b.insert_text("\n")
             return
 
-        if (status != 'incomplete') and b.accept_handler:
+        if (status != "incomplete") and b.accept_handler:
             if not reformatted:
                 reformat_text_before_cursor(b, d, shell)
             b.validate_and_handle()
         else:
             if shell.autoindent:
-                b.insert_text('\n' + indent)
+                b.insert_text("\n" + indent)
             else:
-                b.insert_text('\n')
+                b.insert_text("\n")
+
+    newline_or_execute.__qualname__ = "newline_or_execute"
+
     return newline_or_execute
 
 
 def previous_history_or_previous_completion(event):
     """
     Control-P in vi edit mode on readline is history next, unlike default prompt toolkit.
 
@@ -497,112 +532,139 @@
 
     If completer is open this still select next completion.
     """
     event.current_buffer.auto_down()
 
 
 def dismiss_completion(event):
+    """Dismiss completion"""
     b = event.current_buffer
     if b.complete_state:
         b.cancel_completion()
 
 
 def reset_buffer(event):
+    """Reset buffer"""
     b = event.current_buffer
     if b.complete_state:
         b.cancel_completion()
     else:
         b.reset()
 
 
 def reset_search_buffer(event):
+    """Reset search buffer"""
     if event.current_buffer.document.text:
         event.current_buffer.reset()
     else:
         event.app.layout.focus(DEFAULT_BUFFER)
 
+
 def suspend_to_bg(event):
+    """Suspend to background"""
     event.app.suspend_to_background()
 
+
 def quit(event):
     """
+    Quit application with ``SIGQUIT`` if supported or ``sys.exit`` otherwise.
+
     On platforms that support SIGQUIT, send SIGQUIT to the current process.
     On other platforms, just exit the process with a message.
     """
     sigquit = getattr(signal, "SIGQUIT", None)
     if sigquit is not None:
         os.kill(0, signal.SIGQUIT)
     else:
         sys.exit("Quit")
 
+
 def indent_buffer(event):
-    event.current_buffer.insert_text(' ' * 4)
+    """Indent buffer"""
+    event.current_buffer.insert_text(" " * 4)
+
 
 @undoc
 def newline_with_copy_margin(event):
     """
     DEPRECATED since IPython 6.0
 
     See :any:`newline_autoindent_outer` for a replacement.
 
     Preserve margin and cursor position when using
     Control-O to insert a newline in EMACS mode
     """
-    warnings.warn("`newline_with_copy_margin(event)` is deprecated since IPython 6.0. "
-      "see `newline_autoindent_outer(shell)(event)` for a replacement.",
-                  DeprecationWarning, stacklevel=2)
+    warnings.warn(
+        "`newline_with_copy_margin(event)` is deprecated since IPython 6.0. "
+        "see `newline_autoindent_outer(shell)(event)` for a replacement.",
+        DeprecationWarning,
+        stacklevel=2,
+    )
 
     b = event.current_buffer
     cursor_start_pos = b.document.cursor_position_col
     b.newline(copy_margin=True)
     b.cursor_up(count=1)
     cursor_end_pos = b.document.cursor_position_col
     if cursor_start_pos != cursor_end_pos:
         pos_diff = cursor_start_pos - cursor_end_pos
         b.cursor_right(count=pos_diff)
 
+
 def newline_autoindent_outer(inputsplitter) -> Callable[..., None]:
     """
     Return a function suitable for inserting a indented newline after the cursor.
 
     Fancier version of deprecated ``newline_with_copy_margin`` which should
     compute the correct indentation of the inserted line. That is to say, indent
     by 4 extra space after a function definition, class definition, context
     manager... And dedent by 4 space after ``pass``, ``return``, ``raise ...``.
     """
 
     def newline_autoindent(event):
-        """insert a newline after the cursor indented appropriately."""
+        """Insert a newline after the cursor indented appropriately."""
         b = event.current_buffer
         d = b.document
 
         if b.complete_state:
             b.cancel_completion()
-        text = d.text[:d.cursor_position] + '\n'
+        text = d.text[: d.cursor_position] + "\n"
         _, indent = inputsplitter.check_complete(text)
-        b.insert_text('\n' + (' ' * (indent or 0)), move_cursor=False)
+        b.insert_text("\n" + (" " * (indent or 0)), move_cursor=False)
+
+    newline_autoindent.__qualname__ = "newline_autoindent"
 
     return newline_autoindent
 
 
 def open_input_in_editor(event):
+    """Open code from input in external editor"""
     event.app.current_buffer.open_in_editor()
 
 
-if sys.platform == 'win32':
+if sys.platform == "win32":
     from IPython.core.error import TryNext
-    from IPython.lib.clipboard import (ClipboardEmpty,
-                                       win32_clipboard_get,
-                                       tkinter_clipboard_get)
+    from IPython.lib.clipboard import (
+        ClipboardEmpty,
+        tkinter_clipboard_get,
+        win32_clipboard_get,
+    )
 
     @undoc
     def win_paste(event):
         try:
             text = win32_clipboard_get()
         except TryNext:
             try:
                 text = tkinter_clipboard_get()
             except (TryNext, ClipboardEmpty):
                 return
         except ClipboardEmpty:
             return
         event.current_buffer.insert_text(text.replace("\t", " " * 4))
+
+else:
+
+    @undoc
+    def win_paste(event):
+        """Stub used when auto-generating shortcuts for documentation"""
+        pass
```

### Comparing `ipython-8.8.0/IPython/terminal/tests/test_debug_magic.py` & `ipython-8.9.0/IPython/terminal/tests/test_debug_magic.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/tests/test_embed.py` & `ipython-8.9.0/IPython/terminal/tests/test_embed.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/tests/test_help.py` & `ipython-8.9.0/IPython/terminal/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/terminal/tests/test_interactivshell.py` & `ipython-8.9.0/IPython/terminal/tests/test_interactivshell.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/__init__.py` & `ipython-8.9.0/IPython/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/decorators.py` & `ipython-8.9.0/IPython/testing/decorators.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/globalipapp.py` & `ipython-8.9.0/IPython/testing/globalipapp.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/ipunittest.py` & `ipython-8.9.0/IPython/testing/ipunittest.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/plugin/Makefile` & `ipython-8.9.0/IPython/testing/plugin/Makefile`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/plugin/README.txt` & `ipython-8.9.0/IPython/testing/plugin/README.txt`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/plugin/dtexample.py` & `ipython-8.9.0/IPython/testing/plugin/dtexample.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/plugin/ipdoctest.py` & `ipython-8.9.0/IPython/testing/plugin/ipdoctest.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/plugin/pytest_ipdoctest.py` & `ipython-8.9.0/IPython/testing/plugin/pytest_ipdoctest.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/plugin/setup.py` & `ipython-8.9.0/IPython/testing/plugin/setup.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/plugin/simple.py` & `ipython-8.9.0/IPython/testing/plugin/simple.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/plugin/test_combo.txt` & `ipython-8.9.0/IPython/testing/plugin/test_combo.txt`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/plugin/test_example.txt` & `ipython-8.9.0/IPython/testing/plugin/test_example.txt`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/plugin/test_exampleip.txt` & `ipython-8.9.0/IPython/testing/plugin/test_exampleip.txt`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/plugin/test_ipdoctest.py` & `ipython-8.9.0/IPython/testing/plugin/test_ipdoctest.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/plugin/test_refs.py` & `ipython-8.9.0/IPython/testing/plugin/test_refs.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/skipdoctest.py` & `ipython-8.9.0/IPython/testing/skipdoctest.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/tests/__init__.py` & `ipython-8.9.0/IPython/testing/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/tests/test_decorators.py` & `ipython-8.9.0/IPython/testing/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/tests/test_ipunittest.py` & `ipython-8.9.0/IPython/testing/tests/test_ipunittest.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/tests/test_tools.py` & `ipython-8.9.0/IPython/testing/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/testing/tools.py` & `ipython-8.9.0/IPython/testing/tools.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/tests/cve.py` & `ipython-8.9.0/IPython/tests/cve.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/PyColorize.py` & `ipython-8.9.0/IPython/utils/PyColorize.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/_process_cli.py` & `ipython-8.9.0/IPython/utils/_process_cli.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/_process_common.py` & `ipython-8.9.0/IPython/utils/_process_common.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/_process_posix.py` & `ipython-8.9.0/IPython/utils/_process_posix.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/_process_win32.py` & `ipython-8.9.0/IPython/utils/_process_win32.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/_process_win32_controller.py` & `ipython-8.9.0/IPython/utils/_process_win32_controller.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/capture.py` & `ipython-8.9.0/IPython/utils/capture.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/colorable.py` & `ipython-8.9.0/IPython/utils/colorable.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/coloransi.py` & `ipython-8.9.0/IPython/utils/coloransi.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/contexts.py` & `ipython-8.9.0/IPython/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/data.py` & `ipython-8.9.0/IPython/utils/data.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/decorators.py` & `ipython-8.9.0/IPython/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/dir2.py` & `ipython-8.9.0/IPython/utils/dir2.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/encoding.py` & `ipython-8.9.0/IPython/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/frame.py` & `ipython-8.9.0/IPython/utils/frame.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/generics.py` & `ipython-8.9.0/IPython/utils/generics.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/importstring.py` & `ipython-8.9.0/IPython/utils/importstring.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/io.py` & `ipython-8.9.0/IPython/utils/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,14 @@
 import tempfile
 from pathlib import Path
 from warnings import warn
 
 from IPython.utils.decorators import undoc
 from .capture import CapturedIO, capture_output
 
-# setup stdin/stdout/stderr to sys.stdin/sys.stdout/sys.stderr
-devnull = open(os.devnull, "w", encoding="utf-8")
-atexit.register(devnull.close)
-
-
 class Tee(object):
     """A class to duplicate an output stream to stdout/err.
 
     This works in a manner very similar to the Unix 'tee' command.
 
     When the object is closed or deleted, it closes the original file given to
     it for duplication.
```

### Comparing `ipython-8.8.0/IPython/utils/ipstruct.py` & `ipython-8.9.0/IPython/utils/ipstruct.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/module_paths.py` & `ipython-8.9.0/IPython/utils/module_paths.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/openpy.py` & `ipython-8.9.0/IPython/utils/openpy.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/path.py` & `ipython-8.9.0/IPython/utils/path.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/process.py` & `ipython-8.9.0/IPython/utils/process.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/py3compat.py` & `ipython-8.9.0/IPython/utils/py3compat.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/shimmodule.py` & `ipython-8.9.0/IPython/utils/shimmodule.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/strdispatch.py` & `ipython-8.9.0/IPython/utils/strdispatch.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/sysinfo.py` & `ipython-8.9.0/IPython/utils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/syspathcontext.py` & `ipython-8.9.0/IPython/utils/syspathcontext.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tempdir.py` & `ipython-8.9.0/IPython/utils/tempdir.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/terminal.py` & `ipython-8.9.0/IPython/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tests/test_capture.py` & `ipython-8.9.0/IPython/utils/tests/test_capture.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tests/test_dir2.py` & `ipython-8.9.0/IPython/utils/tests/test_dir2.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tests/test_importstring.py` & `ipython-8.9.0/IPython/utils/tests/test_importstring.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tests/test_io.py` & `ipython-8.9.0/IPython/utils/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tests/test_module_paths.py` & `ipython-8.9.0/IPython/utils/tests/test_module_paths.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tests/test_openpy.py` & `ipython-8.9.0/IPython/utils/tests/test_openpy.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tests/test_path.py` & `ipython-8.9.0/IPython/utils/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tests/test_process.py` & `ipython-8.9.0/IPython/utils/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tests/test_pycolorize.py` & `ipython-8.9.0/IPython/utils/tests/test_pycolorize.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tests/test_tempdir.py` & `ipython-8.9.0/IPython/utils/tests/test_tempdir.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tests/test_text.py` & `ipython-8.9.0/IPython/utils/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tests/test_tokenutil.py` & `ipython-8.9.0/IPython/utils/tests/test_tokenutil.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tests/test_wildcard.py` & `ipython-8.9.0/IPython/utils/tests/test_wildcard.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/text.py` & `ipython-8.9.0/IPython/utils/text.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/timing.py` & `ipython-8.9.0/IPython/utils/timing.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tokenutil.py` & `ipython-8.9.0/IPython/utils/tokenutil.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/tz.py` & `ipython-8.9.0/IPython/utils/tz.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/ulinecache.py` & `ipython-8.9.0/IPython/utils/ulinecache.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/version.py` & `ipython-8.9.0/IPython/utils/version.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/IPython/utils/wildcard.py` & `ipython-8.9.0/IPython/utils/wildcard.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/LICENSE` & `ipython-8.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/MANIFEST.in` & `ipython-8.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/PKG-INFO` & `ipython-8.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipython
-Version: 8.8.0
+Version: 8.9.0
 Summary: IPython: Productive Interactive Computing
 Home-page: https://ipython.org
 Author: The IPython Development Team
 Author-email: ipython-dev@python.org
 License: BSD-3-Clause
 Project-URL: Documentation, https://ipython.readthedocs.io/
 Project-URL: Funding, https://numfocus.org/
```

### Comparing `ipython-8.8.0/README.rst` & `ipython-8.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/Makefile` & `ipython-8.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/README.rst` & `ipython-8.9.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/autogen_api.py` & `ipython-8.9.0/docs/autogen_api.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/autogen_config.py` & `ipython-8.9.0/docs/autogen_config.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/autogen_magics.py` & `ipython-8.9.0/docs/autogen_magics.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/make.cmd` & `ipython-8.9.0/docs/make.cmd`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/man/ipython.1` & `ipython-8.9.0/docs/man/ipython.1`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/2.0/running-crop.png` & `ipython-8.9.0/docs/source/_images/2.0/running-crop.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/2.0/running.png` & `ipython-8.9.0/docs/source/_images/2.0/running.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/2.0/treeview.png` & `ipython-8.9.0/docs/source/_images/2.0/treeview.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/2.0/user-interface.png` & `ipython-8.9.0/docs/source/_images/2.0/user-interface.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/2.0/widgets.png` & `ipython-8.9.0/docs/source/_images/2.0/widgets.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/8.0/auto_suggest_1_prompt_no_text.png` & `ipython-8.9.0/docs/source/_images/8.0/auto_suggest_1_prompt_no_text.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/8.0/auto_suggest_2_print_hello_suggest.png` & `ipython-8.9.0/docs/source/_images/8.0/auto_suggest_2_print_hello_suggest.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/8.0/auto_suggest_3_print_hello_suggest.png` & `ipython-8.9.0/docs/source/_images/8.0/auto_suggest_3_print_hello_suggest.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/8.0/auto_suggest_4_print_hello.png` & `ipython-8.9.0/docs/source/_images/8.0/auto_suggest_4_print_hello.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/8.0/auto_suggest_d_completions.png` & `ipython-8.9.0/docs/source/_images/8.0/auto_suggest_d_completions.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/8.0/auto_suggest_d_phantom.png` & `ipython-8.9.0/docs/source/_images/8.0/auto_suggest_d_phantom.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/8.0/auto_suggest_def_completions.png` & `ipython-8.9.0/docs/source/_images/8.0/auto_suggest_def_completions.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/8.0/auto_suggest_def_phantom.png` & `ipython-8.9.0/docs/source/_images/8.0/auto_suggest_def_phantom.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/8.0/auto_suggest_match_parens.png` & `ipython-8.9.0/docs/source/_images/8.0/auto_suggest_match_parens.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/8.0/auto_suggest_second_prompt.png` & `ipython-8.9.0/docs/source/_images/8.0/auto_suggest_second_prompt.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/8.0/pathlib_pathlib_everywhere.jpg` & `ipython-8.9.0/docs/source/_images/8.0/pathlib_pathlib_everywhere.jpg`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ipy_013_dashboard.png` & `ipython-8.9.0/docs/source/_images/ipy_013_dashboard.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ipy_013_dashboard_cluster.png` & `ipython-8.9.0/docs/source/_images/ipy_013_dashboard_cluster.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ipy_013_notebook_cythonmagic.png` & `ipython-8.9.0/docs/source/_images/ipy_013_notebook_cythonmagic.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ipy_013_notebook_long_out.png` & `ipython-8.9.0/docs/source/_images/ipy_013_notebook_long_out.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ipy_013_notebook_octavemagic.png` & `ipython-8.9.0/docs/source/_images/ipy_013_notebook_octavemagic.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ipy_013_notebook_rmagic.png` & `ipython-8.9.0/docs/source/_images/ipy_013_notebook_rmagic.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ipy_013_notebook_script_cells.png` & `ipython-8.9.0/docs/source/_images/ipy_013_notebook_script_cells.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ipy_013_notebook_spectrogram.png` & `ipython-8.9.0/docs/source/_images/ipy_013_notebook_spectrogram.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ipy_013_notebook_tooltip.png` & `ipython-8.9.0/docs/source/_images/ipy_013_notebook_tooltip.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ipy_013_par_tb.png` & `ipython-8.9.0/docs/source/_images/ipy_013_par_tb.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ipy_013_qtconsole_baboon.png` & `ipython-8.9.0/docs/source/_images/ipy_013_qtconsole_baboon.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ipy_013_qtconsole_completer.png` & `ipython-8.9.0/docs/source/_images/ipy_013_qtconsole_completer.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ipython-6-screenshot.png` & `ipython-8.9.0/docs/source/_images/ipython-6-screenshot.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/jedi_type_inference_60.png` & `ipython-8.9.0/docs/source/_images/jedi_type_inference_60.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/kernel_selector_screenshot.png` & `ipython-8.9.0/docs/source/_images/kernel_selector_screenshot.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ms_visual_studio.png` & `ipython-8.9.0/docs/source/_images/ms_visual_studio.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/notebook_specgram.png` & `ipython-8.9.0/docs/source/_images/notebook_specgram.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/ptshell_features.png` & `ipython-8.9.0/docs/source/_images/ptshell_features.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/qtconsole.png` & `ipython-8.9.0/docs/source/_images/qtconsole.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/qtconsole_tabbed.png` & `ipython-8.9.0/docs/source/_images/qtconsole_tabbed.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_images/unicode_completion.png` & `ipython-8.9.0/docs/source/_images/unicode_completion.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_static/favicon.ico` & `ipython-8.9.0/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/_static/logo.png` & `ipython-8.9.0/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/about/history.rst` & `ipython-8.9.0/docs/source/about/history.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/about/license_and_copyright.rst` & `ipython-8.9.0/docs/source/about/license_and_copyright.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/conf.py` & `ipython-8.9.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,14 @@
 # -----------------------
 
 # The style sheet to use for HTML and HTML Help pages. A file of that name
 # must exist either in Sphinx' static/ path, or in one of the custom paths
 # given in html_static_path.
 # html_style = 'default.css'
 
-
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 #html_title = None
 
 # The name of an image file (within the static path) to place at the top of
 # the sidebar.
 #html_logo = None
@@ -323,12 +322,16 @@
    'Programming',
    1),
 ]
 
 modindex_common_prefix = ['IPython.']
 
 
+def setup(app):
+    app.add_css_file("theme_overrides.css")
+
+
 # Cleanup
 # -------
 # delete release info to avoid pickling errors from sphinx
 
 del iprelease
```

### Comparing `ipython-8.8.0/docs/source/config/callbacks.rst` & `ipython-8.9.0/docs/source/config/callbacks.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/config/custommagics.rst` & `ipython-8.9.0/docs/source/config/custommagics.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/config/details.rst` & `ipython-8.9.0/docs/source/config/details.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/config/eventloops.rst` & `ipython-8.9.0/docs/source/config/eventloops.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/config/extensions/index.rst` & `ipython-8.9.0/docs/source/config/extensions/index.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/config/index.rst` & `ipython-8.9.0/docs/source/config/index.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/config/inputtransforms.rst` & `ipython-8.9.0/docs/source/config/inputtransforms.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/config/integrating.rst` & `ipython-8.9.0/docs/source/config/integrating.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/config/intro.rst` & `ipython-8.9.0/docs/source/config/intro.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/config/shell_mimerenderer.rst` & `ipython-8.9.0/docs/source/config/shell_mimerenderer.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/coredev/index.rst` & `ipython-8.9.0/docs/source/coredev/index.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/development/config.rst` & `ipython-8.9.0/docs/source/development/config.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/development/execution.rst` & `ipython-8.9.0/docs/source/development/execution.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/development/figs/ipy_kernel_and_terminal.png` & `ipython-8.9.0/docs/source/development/figs/ipy_kernel_and_terminal.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/development/figs/ipy_kernel_and_terminal.svg` & `ipython-8.9.0/docs/source/development/figs/ipy_kernel_and_terminal.svg`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/development/figs/other_kernels.png` & `ipython-8.9.0/docs/source/development/figs/other_kernels.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/development/figs/other_kernels.svg` & `ipython-8.9.0/docs/source/development/figs/other_kernels.svg`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/development/how_ipython_works.rst` & `ipython-8.9.0/docs/source/development/how_ipython_works.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/development/index.rst` & `ipython-8.9.0/docs/source/development/index.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/development/inputhook_app.rst` & `ipython-8.9.0/docs/source/development/inputhook_app.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/development/lexer.rst` & `ipython-8.9.0/docs/source/development/lexer.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/development/pycompat.rst` & `ipython-8.9.0/docs/source/development/pycompat.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/development/wrapperkernels.rst` & `ipython-8.9.0/docs/source/development/wrapperkernels.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/index.rst` & `ipython-8.9.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/install/index.rst` & `ipython-8.9.0/docs/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/install/install.rst` & `ipython-8.9.0/docs/source/install/install.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/install/kernel_install.rst` & `ipython-8.9.0/docs/source/install/kernel_install.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/interactive/autoawait.rst` & `ipython-8.9.0/docs/source/interactive/autoawait.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/interactive/figs/besselj.png` & `ipython-8.9.0/docs/source/interactive/figs/besselj.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/interactive/figs/colors_dark.png` & `ipython-8.9.0/docs/source/interactive/figs/colors_dark.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/interactive/figs/jn.html` & `ipython-8.9.0/docs/source/interactive/figs/jn.html`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/interactive/figs/jn.xhtml` & `ipython-8.9.0/docs/source/interactive/figs/jn.xhtml`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/interactive/index.rst` & `ipython-8.9.0/docs/source/interactive/index.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/interactive/magics.rst` & `ipython-8.9.0/docs/source/interactive/magics.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/interactive/plotting.rst` & `ipython-8.9.0/docs/source/interactive/plotting.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/interactive/python-ipython-diff.rst` & `ipython-8.9.0/docs/source/interactive/python-ipython-diff.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/interactive/reference.rst` & `ipython-8.9.0/docs/source/interactive/reference.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/interactive/shell.rst` & `ipython-8.9.0/docs/source/interactive/shell.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/interactive/tips.rst` & `ipython-8.9.0/docs/source/interactive/tips.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/interactive/tutorial.rst` & `ipython-8.9.0/docs/source/interactive/tutorial.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/links.txt` & `ipython-8.9.0/docs/source/links.txt`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/overview.rst` & `ipython-8.9.0/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/sphinxext.rst` & `ipython-8.9.0/docs/source/sphinxext.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/development.rst` & `ipython-8.9.0/docs/source/whatsnew/development.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/github-stats-0.11.rst` & `ipython-8.9.0/docs/source/whatsnew/github-stats-0.11.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/github-stats-0.12.rst` & `ipython-8.9.0/docs/source/whatsnew/github-stats-0.12.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/github-stats-0.13.rst` & `ipython-8.9.0/docs/source/whatsnew/github-stats-0.13.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/github-stats-1.0.rst` & `ipython-8.9.0/docs/source/whatsnew/github-stats-1.0.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/github-stats-2.0.rst` & `ipython-8.9.0/docs/source/whatsnew/github-stats-2.0.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/github-stats-3.rst` & `ipython-8.9.0/docs/source/whatsnew/github-stats-3.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/github-stats-4.rst` & `ipython-8.9.0/docs/source/whatsnew/github-stats-4.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/github-stats-5.rst` & `ipython-8.9.0/docs/source/whatsnew/github-stats-5.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/github-stats-6.rst` & `ipython-8.9.0/docs/source/whatsnew/github-stats-6.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/github-stats-7.rst` & `ipython-8.9.0/docs/source/whatsnew/github-stats-7.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/github-stats-8.rst` & `ipython-8.9.0/docs/source/whatsnew/github-stats-8.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/index.rst` & `ipython-8.9.0/docs/source/whatsnew/index.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/pr/README.md` & `ipython-8.9.0/docs/source/whatsnew/pr/README.md`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version0.10.rst` & `ipython-8.9.0/docs/source/whatsnew/version0.10.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version0.11.rst` & `ipython-8.9.0/docs/source/whatsnew/version0.11.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version0.12.rst` & `ipython-8.9.0/docs/source/whatsnew/version0.12.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version0.13.rst` & `ipython-8.9.0/docs/source/whatsnew/version0.13.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version0.8.rst` & `ipython-8.9.0/docs/source/whatsnew/version0.8.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version0.9.rst` & `ipython-8.9.0/docs/source/whatsnew/version0.9.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version1.0.rst` & `ipython-8.9.0/docs/source/whatsnew/version1.0.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version2.0.rst` & `ipython-8.9.0/docs/source/whatsnew/version2.0.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version3.rst` & `ipython-8.9.0/docs/source/whatsnew/version3.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version3_widget_migration.rst` & `ipython-8.9.0/docs/source/whatsnew/version3_widget_migration.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version4.rst` & `ipython-8.9.0/docs/source/whatsnew/version4.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version5.rst` & `ipython-8.9.0/docs/source/whatsnew/version5.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version6.rst` & `ipython-8.9.0/docs/source/whatsnew/version6.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version7.rst` & `ipython-8.9.0/docs/source/whatsnew/version7.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/source/whatsnew/version8.rst` & `ipython-8.9.0/docs/source/whatsnew/version8.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,59 @@
 ============
  8.x Series
 ============
 
+.. _version 8.9.0:
+
+IPython 8.9.0
+-------------
+
+Second release of IPython in 2023, last Friday of the month, we are back on
+track. This is a small release with a few bug-fixes, and improvements, mostly
+with respect to terminal shortcuts.
+
+
+The biggest improvement for 8.9 is a drastic amelioration if the
+auto-suggestions sponsored by D.E. Shaw and implemented by the more and more
+active contributor `@krassowski <https://github.com/krassowski>`.
+
+- ``right`` accepts a single character from suggestion
+- ``ctrl+right`` accepts a semantic token (macos default shortcuts take
+  precedence and need to be disabled to make this work)
+- ``backspace`` deletes a character and resumes hinting autosuggestions
+- ``ctrl-left`` accepts suggestion and moves cursor left one character.
+- ``backspace`` deletes a character and resumes hinting autosuggestions
+- ``down`` moves to suggestion to later in history when no lines are present below the cursors.
+- ``up`` moves to suggestion from earlier in history when no lines are present above the cursor.
+
+This is best described by the Gif posted by `@krassowski
+<https://github.com/krassowski>`, and in the PR itself :ghpull:`13888`.
+
+.. image:: ../_images/autosuggest.gif
+
+Please report any feedback in order for us to improve the user experience.
+In particular we are also working on making the shortcuts configurable.
+
+If you are interested into better terminal shortcut, I also invite you to
+participate in issue `13879
+<https://github.com/ipython/ipython/issues/13879>`__.
+
+
+As we follow `NEP29
+<https://numpy.org/neps/nep-0029-deprecation_policy.html>`__, next version of
+IPython will officially stop supporting numpy 1.20, and will stop supporting
+Python 3.8 after April release.
+
+As usual you can find the full list of PRs on GitHub under `the 8.9 milestone
+<https://github.com/ipython/ipython/milestone/111?closed=1>`__.
+
+
+Thanks to the `D. E. Shaw group <https://deshaw.com/>`__ for sponsoring
+work on IPython and related libraries.
+
 .. _version 8.8.0:
 
 IPython 8.8.0
 -------------
 
 First release of IPython in 2023 as there was no release at the end of
 December.
```

### Comparing `ipython-8.8.0/docs/sphinxext/apigen.py` & `ipython-8.9.0/docs/sphinxext/apigen.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/sphinxext/github.py` & `ipython-8.9.0/docs/sphinxext/github.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/docs/sphinxext/magics.py` & `ipython-8.9.0/docs/sphinxext/magics.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/Embedding/Index.ipynb` & `ipython-8.9.0/examples/Embedding/Index.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/Embedding/embed_class_long.py` & `ipython-8.9.0/examples/Embedding/embed_class_long.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/Embedding/embed_class_short.py` & `ipython-8.9.0/examples/Embedding/embed_class_short.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/Embedding/start_ipython_config.py` & `ipython-8.9.0/examples/Embedding/start_ipython_config.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Animations Using clear_output.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Animations Using clear_output.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Background Jobs.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Background Jobs.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Beyond Plain Python.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Beyond Plain Python.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Capturing Output.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Capturing Output.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Cell Magics.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Cell Magics.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Custom Display Logic.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Custom Display Logic.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Importing Notebooks.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Importing Notebooks.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Index.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Index.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Plotting in the Notebook.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Plotting in the Notebook.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Raw Input in the Notebook.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Raw Input in the Notebook.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Rich Output.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Rich Output.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Script Magics.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Script Magics.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/SymPy.ipynb` & `ipython-8.9.0/examples/IPython Kernel/SymPy.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Terminal Usage.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Terminal Usage.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Third Party Rich Output.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Third Party Rich Output.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Trapezoid Rule.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Trapezoid Rule.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Updating Displays.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Updating Displays.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/Working With External Code.ipynb` & `ipython-8.9.0/examples/IPython Kernel/Working With External Code.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/data/flare.json` & `ipython-8.9.0/examples/IPython Kernel/data/flare.json`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/example-demo.py` & `ipython-8.9.0/examples/IPython Kernel/example-demo.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/gui/gui-glut.py` & `ipython-8.9.0/examples/IPython Kernel/gui/gui-glut.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/gui/gui-gtk4.py` & `ipython-8.9.0/examples/IPython Kernel/gui/gui-gtk4.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/gui/gui-qt.py` & `ipython-8.9.0/examples/IPython Kernel/gui/gui-qt.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/ipython-completion.bash` & `ipython-8.9.0/examples/IPython Kernel/ipython-completion.bash`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/ipython-get-history.py` & `ipython-8.9.0/examples/IPython Kernel/ipython-get-history.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/nbpackage/mynotebook.ipynb` & `ipython-8.9.0/examples/IPython Kernel/nbpackage/mynotebook.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/IPython Kernel/nbpackage/nbs/other.ipynb` & `ipython-8.9.0/examples/IPython Kernel/nbpackage/nbs/other.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/Index.ipynb` & `ipython-8.9.0/examples/Index.ipynb`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/images/FrontendKernel.graffle/data.plist` & `ipython-8.9.0/examples/images/FrontendKernel.graffle/data.plist`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/images/FrontendKernel.graffle/image1.png` & `ipython-8.9.0/examples/images/FrontendKernel.graffle/image1.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/images/FrontendKernel.png` & `ipython-8.9.0/examples/images/FrontendKernel.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/images/animation.m4v` & `ipython-8.9.0/examples/images/animation.m4v`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/images/ipython_logo.png` & `ipython-8.9.0/examples/images/ipython_logo.png`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/images/python_logo.svg` & `ipython-8.9.0/examples/images/python_logo.svg`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/examples/utils/cwd_prompt.py` & `ipython-8.9.0/examples/utils/cwd_prompt.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/ipython.egg-info/PKG-INFO` & `ipython-8.9.0/ipython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipython
-Version: 8.8.0
+Version: 8.9.0
 Summary: IPython: Productive Interactive Computing
 Home-page: https://ipython.org
 Author: The IPython Development Team
 Author-email: ipython-dev@python.org
 License: BSD-3-Clause
 Project-URL: Documentation, https://ipython.readthedocs.io/
 Project-URL: Funding, https://numfocus.org/
```

### Comparing `ipython-8.8.0/ipython.egg-info/SOURCES.txt` & `ipython-8.9.0/ipython.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -177,31 +177,34 @@
 IPython/terminal/debugger.py
 IPython/terminal/embed.py
 IPython/terminal/interactiveshell.py
 IPython/terminal/ipapp.py
 IPython/terminal/magics.py
 IPython/terminal/prompts.py
 IPython/terminal/ptutils.py
-IPython/terminal/shortcuts.py
 IPython/terminal/pt_inputhooks/__init__.py
 IPython/terminal/pt_inputhooks/asyncio.py
 IPython/terminal/pt_inputhooks/glut.py
 IPython/terminal/pt_inputhooks/gtk.py
 IPython/terminal/pt_inputhooks/gtk3.py
 IPython/terminal/pt_inputhooks/gtk4.py
 IPython/terminal/pt_inputhooks/osx.py
 IPython/terminal/pt_inputhooks/pyglet.py
 IPython/terminal/pt_inputhooks/qt.py
 IPython/terminal/pt_inputhooks/tk.py
 IPython/terminal/pt_inputhooks/wx.py
+IPython/terminal/shortcuts/__init__.py
+IPython/terminal/shortcuts/auto_match.py
+IPython/terminal/shortcuts/auto_suggest.py
 IPython/terminal/tests/__init__.py
 IPython/terminal/tests/test_debug_magic.py
 IPython/terminal/tests/test_embed.py
 IPython/terminal/tests/test_help.py
 IPython/terminal/tests/test_interactivshell.py
+IPython/terminal/tests/test_shortcuts.py
 IPython/testing/__init__.py
 IPython/testing/decorators.py
 IPython/testing/globalipapp.py
 IPython/testing/ipunittest.py
 IPython/testing/skipdoctest.py
 IPython/testing/tools.py
 IPython/testing/plugin/Makefile
@@ -219,15 +222,14 @@
 IPython/testing/plugin/test_ipdoctest.py
 IPython/testing/plugin/test_refs.py
 IPython/testing/tests/__init__.py
 IPython/testing/tests/test_decorators.py
 IPython/testing/tests/test_ipunittest.py
 IPython/testing/tests/test_tools.py
 IPython/tests/cve.py
-IPython/tests/test_shortcuts.py
 IPython/utils/PyColorize.py
 IPython/utils/__init__.py
 IPython/utils/_process_cli.py
 IPython/utils/_process_common.py
 IPython/utils/_process_posix.py
 IPython/utils/_process_win32.py
 IPython/utils/_process_win32_controller.py
@@ -301,14 +303,15 @@
 docs/requirements.txt
 docs/man/ipython.1
 docs/source/conf.py
 docs/source/index.rst
 docs/source/links.txt
 docs/source/overview.rst
 docs/source/sphinxext.rst
+docs/source/_images/autosuggest.gif
 docs/source/_images/ipy_013_dashboard.png
 docs/source/_images/ipy_013_dashboard_cluster.png
 docs/source/_images/ipy_013_notebook_cythonmagic.png
 docs/source/_images/ipy_013_notebook_long_out.png
 docs/source/_images/ipy_013_notebook_octavemagic.png
 docs/source/_images/ipy_013_notebook_rmagic.png
 docs/source/_images/ipy_013_notebook_script_cells.png
@@ -340,14 +343,15 @@
 docs/source/_images/8.0/auto_suggest_def_completions.png
 docs/source/_images/8.0/auto_suggest_def_phantom.png
 docs/source/_images/8.0/auto_suggest_match_parens.png
 docs/source/_images/8.0/auto_suggest_second_prompt.png
 docs/source/_images/8.0/pathlib_pathlib_everywhere.jpg
 docs/source/_static/favicon.ico
 docs/source/_static/logo.png
+docs/source/_static/theme_overrides.css
 docs/source/_templates/breadcrumbs.html
 docs/source/_templates/notebook_redirect.html
 docs/source/about/history.rst
 docs/source/about/index.rst
 docs/source/about/license_and_copyright.rst
 docs/source/api/index.rst
 docs/source/config/callbacks.rst
```

### Comparing `ipython-8.8.0/ipython.egg-info/requires.txt` & `ipython-8.9.0/ipython.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 backcall
 decorator
 jedi>=0.16
 matplotlib-inline
 pickleshare
-prompt_toolkit<3.1.0,>=3.0.11
+prompt_toolkit<3.1.0,>=3.0.30
 pygments>=2.4.0
 stack_data
 traitlets>=5
 
 [:sys_platform != "win32"]
 pexpect>4.3
```

### Comparing `ipython-8.8.0/long_description.rst` & `ipython-8.9.0/long_description.rst`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/pytest.ini` & `ipython-8.9.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/scripts/ipython.ico` & `ipython-8.9.0/scripts/ipython.ico`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/scripts/ipython_nb.ico` & `ipython-8.9.0/scripts/ipython_nb.ico`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/setup.cfg` & `ipython-8.9.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 	backcall
 	colorama; sys_platform == "win32"
 	decorator
 	jedi>=0.16
 	matplotlib-inline
 	pexpect>4.3; sys_platform != "win32"
 	pickleshare
-	prompt_toolkit>=3.0.11,<3.1.0
+	prompt_toolkit>=3.0.30,<3.1.0
 	pygments>=2.4.0
 	stack_data
 	traitlets>=5
 
 [options.extras_require]
 black = 
 	black
```

### Comparing `ipython-8.8.0/setup.py` & `ipython-8.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ipython-8.8.0/setupbase.py` & `ipython-8.9.0/setupbase.py`

 * *Files identical despite different names*

