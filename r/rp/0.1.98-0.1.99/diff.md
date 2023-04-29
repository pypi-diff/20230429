# Comparing `tmp/rp-0.1.98.tar.gz` & `tmp/rp-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rp-0.1.98.tar", last modified: Wed Sep 11 23:39:03 2019, max compression
+gzip compressed data, was "dist/rp-0.1.99.tar", last modified: Thu Sep 12 01:42:01 2019, max compression
```

## Comparing `rp-0.1.98.tar` & `rp-0.1.99.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:03.000000 rp-0.1.98/
--rw-r--r--   0 Ryan       (502) staff       (20)      347 2019-09-11 23:39:03.000000 rp-0.1.98/PKG-INFO
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp.egg-info/
--rw-r--r--   0 Ryan       (502) staff       (20)      347 2019-09-11 23:39:02.000000 rp-0.1.98/rp.egg-info/PKG-INFO
--rw-r--r--   0 Ryan       (502) staff       (20)     6148 2017-12-31 00:44:33.000000 rp-0.1.98/rp.egg-info/.DS_Store
--rw-r--r--   0 Ryan       (502) staff       (20)     4974 2019-09-11 23:39:02.000000 rp-0.1.98/rp.egg-info/SOURCES.txt
--rw-r--r--   0 Ryan       (502) staff       (20)       41 2019-09-11 23:39:02.000000 rp-0.1.98/rp.egg-info/entry_points.txt
--rw-r--r--   0 Ryan       (502) staff       (20)       29 2019-09-11 23:39:02.000000 rp-0.1.98/rp.egg-info/requires.txt
--rw-r--r--   0 Ryan       (502) staff       (20)        3 2019-09-11 23:39:02.000000 rp-0.1.98/rp.egg-info/top_level.txt
--rw-r--r--   0 Ryan       (502) staff       (20)        1 2019-09-11 23:39:02.000000 rp-0.1.98/rp.egg-info/dependency_links.txt
--rw-r--r--   0 Ryan       (502) staff       (20)      605 2017-12-15 05:14:49.000000 rp-0.1.98/README
--rw-r--r--   0 Ryan       (502) staff       (20)     2460 2019-09-11 22:47:01.000000 rp-0.1.98/setup.py
--rw-r--r--   0 Ryan       (502) staff       (20)       38 2019-09-11 23:39:03.000000 rp-0.1.98/setup.cfg
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/
--rw-r--r--   0 Ryan       (502) staff       (20)   402279 2019-09-11 23:39:01.000000 rp-0.1.98/rp/automips2.py
--rw-r--r--   0 Ryan       (502) staff       (20)        2 2019-09-11 23:39:01.000000 rp-0.1.98/rp/version.py
--rw-r--r--   0 Ryan       (502) staff       (20)   419323 2019-09-11 23:39:01.000000 rp-0.1.98/rp/r.py
--rw-r--r--   0 Ryan       (502) staff       (20)    15604 2019-09-11 23:39:01.000000 rp-0.1.98/rp/pychess.py
--rw-r--r--   0 Ryan       (502) staff       (20)    19495 2019-09-11 23:39:01.000000 rp-0.1.98/rp/TestOSC.py
--rw-r--r--   0 Ryan       (502) staff       (20)     7388 2019-09-11 23:39:01.000000 rp-0.1.98/rp/Pyperclip.py
--rw-r--r--   0 Ryan       (502) staff       (20)      421 2019-09-11 23:39:01.000000 rp-0.1.98/rp/google_colab.py
--rw-r--r--   0 Ryan       (502) staff       (20)       19 2019-09-11 23:39:01.000000 rp-0.1.98/rp/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)      548 2019-09-11 23:39:01.000000 rp-0.1.98/rp/Test.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1470 2019-09-11 23:39:01.000000 rp-0.1.98/rp/shotgun.py
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:03.000000 rp-0.1.98/rp/rp_ptpython/
--rw-r--r--   0 Ryan       (502) staff       (20)     1667 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/validator.py
--rw-r--r--   0 Ryan       (502) staff       (20)   152845 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/key_bindings.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1998 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/prompt_style.py
--rw-r--r--   0 Ryan       (502) staff       (20)    12204 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/style.py
--rw-r--r--   0 Ryan       (502) staff       (20)    29993 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/layout.py
--rw-r--r--   0 Ryan       (502) staff       (20)    10466 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/repl.py
--rw-r--r--   0 Ryan       (502) staff       (20)    14048 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/completerbackup.py
--rw-r--r--   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)     2435 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/eventloop.py
--rw-r--r--   0 Ryan       (502) staff       (20)    12653 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/completer.py
--rw-r--r--   0 Ryan       (502) staff       (20)    12891 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/completer_stable.py
--rw-r--r--   0 Ryan       (502) staff       (20)    10606 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/ipython.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3956 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/utils.py
--rw-r--r--   0 Ryan       (502) staff       (20)    21239 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/history_browser.py
--rw-r--r--   0 Ryan       (502) staff       (20)      159 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/__main__.py
--rw-r--r--   0 Ryan       (502) staff       (20)     2772 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/untitled.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1582 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/filters.py
--rw-r--r--   0 Ryan       (502) staff       (20)    32079 2019-09-11 23:39:01.000000 rp-0.1.98/rp/rp_ptpython/python_input.py
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/filters/
--rw-r--r--   0 Ryan       (502) staff       (20)     1691 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/filters/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1514 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/filters/types.py
--rw-r--r--   0 Ryan       (502) staff       (20)     9233 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/filters/cli.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1114 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/filters/utils.py
--rw-r--r--   0 Ryan       (502) staff       (20)     6082 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/filters/base.py
--rw-r--r--   0 Ryan       (502) staff       (20)      792 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/enums.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1420 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/token.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1380 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/mouse_events.py
--rw-r--r--   0 Ryan       (502) staff       (20)     5723 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/completion.py
--rw-r--r--   0 Ryan       (502) staff       (20)    28167 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/shortcuts.py
--rw-r--r--   0 Ryan       (502) staff       (20)    19753 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/renderer.py
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/layout/
--rw-r--r--   0 Ryan       (502) staff       (20)     4490 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/layout/screen.py
--rw-r--r--   0 Ryan       (502) staff       (20)    28561 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/layout/controls.py
--rw-r--r--   0 Ryan       (502) staff       (20)     7048 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/layout/toolbars.py
--rw-r--r--   0 Ryan       (502) staff       (20)    67803 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/layout/containers.py
--rw-r--r--   0 Ryan       (502) staff       (20)      780 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/layout/mouse_handlers.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1909 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/layout/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)     8858 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/layout/margins.py
--rw-r--r--   0 Ryan       (502) staff       (20)     5472 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/layout/utils.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3242 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/layout/prompt.py
--rw-r--r--   0 Ryan       (502) staff       (20)    21760 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/layout/processors.py
--rw-r--r--   0 Ryan       (502) staff       (20)    19438 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/layout/menus.py
--rw-r--r--   0 Ryan       (502) staff       (20)    11343 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/layout/lexers.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3154 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/layout/dimension.py
--rw-r--r--   0 Ryan       (502) staff       (20)     2842 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/auto_suggest.py
--rw-r--r--   0 Ryan       (502) staff       (20)     4046 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/win32_types.py
--rw-r--r--   0 Ryan       (502) staff       (20)    42395 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/interface.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1841 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/reactive.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3400 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/cache.py
--rw-r--r--   0 Ryan       (502) staff       (20)      632 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/__init__.py
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/terminal/
--rw-r--r--   0 Ryan       (502) staff       (20)    19863 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/terminal/vt100_output.py
--rw-r--r--   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/terminal/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)    19622 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/terminal/win32_output.py
--rw-r--r--   0 Ryan       (502) staff       (20)    13064 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/terminal/win32_input.py
--rw-r--r--   0 Ryan       (502) staff       (20)    18428 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/terminal/vt100_input.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1397 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/terminal/conemu_output.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3630 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/keys.py
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/contrib/
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/contrib/completers/
--rw-r--r--   0 Ryan       (502) staff       (20)     1922 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/completers/system.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3762 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/completers/filesystem.py
--rw-r--r--   0 Ryan       (502) staff       (20)      147 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/completers/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)     2275 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/completers/base.py
--rw-r--r--   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/__init__.py
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/contrib/regular_languages/
--rw-r--r--   0 Ryan       (502) staff       (20)    15633 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/regular_languages/compiler.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3032 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/regular_languages/completion.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3286 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/regular_languages/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3414 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/regular_languages/lexer.py
--rw-r--r--   0 Ryan       (502) staff       (20)     7266 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/regular_languages/regex_parser.py
--rw-r--r--   0 Ryan       (502) staff       (20)     2065 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/regular_languages/validation.py
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/contrib/validators/
--rw-r--r--   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/validators/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1243 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/validators/base.py
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/contrib/telnet/
--rw-r--r--   0 Ryan       (502) staff       (20)    12914 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/telnet/server.py
--rw-r--r--   0 Ryan       (502) staff       (20)      170 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/telnet/log.py
--rw-r--r--   0 Ryan       (502) staff       (20)     4884 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/telnet/protocol.py
--rw-r--r--   0 Ryan       (502) staff       (20)       49 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/telnet/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)      894 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/contrib/telnet/application.py
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/
--rw-r--r--   0 Ryan       (502) staff       (20)    11499 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/registry.py
--rw-r--r--   0 Ryan       (502) staff       (20)       40 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)    11937 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/input_processor.py
--rw-r--r--   0 Ryan       (502) staff       (20)     4933 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/defaults.py
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/
--rw-r--r--   0 Ryan       (502) staff       (20)    15940 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/named_commands.py
--rw-r--r--   0 Ryan       (502) staff       (20)     5659 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/completion.py
--rw-r--r--   0 Ryan       (502) staff       (20)     5711 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/scroll.py
--rw-r--r--   0 Ryan       (502) staff       (20)    67865 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/vi.py
--rw-r--r--   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)    15542 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/emacs.py
--rw-r--r--   0 Ryan       (502) staff       (20)    13352 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/basic.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1734 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/vi_state.py
--rw-r--r--   0 Ryan       (502) staff       (20)    32842 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/digraphs.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3730 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/key_binding/manager.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1099 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/search_state.py
--rw-r--r--   0 Ryan       (502) staff       (20)     8747 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/application.py
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/styles/
--rw-r--r--   0 Ryan       (502) staff       (20)      504 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/styles/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1198 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/styles/utils.py
--rw-r--r--   0 Ryan       (502) staff       (20)     4579 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/styles/from_dict.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3698 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/styles/defaults.py
--rw-r--r--   0 Ryan       (502) staff       (20)     2349 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/styles/from_pygments.py
--rw-r--r--   0 Ryan       (502) staff       (20)     2489 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/styles/base.py
--rw-r--r--   0 Ryan       (502) staff       (20)     6359 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/utils.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3214 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/input.py
--rw-r--r--   0 Ryan       (502) staff       (20)    51517 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/buffer.py
--rw-r--r--   0 Ryan       (502) staff       (20)    35976 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/document.py
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/eventloop/
--rw-r--r--   0 Ryan       (502) staff       (20)     3312 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/eventloop/posix_utils.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3363 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/eventloop/asyncio_posix.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1152 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/eventloop/asyncio_base.py
--rw-r--r--   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/eventloop/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)     6196 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/eventloop/win32.py
--rw-r--r--   0 Ryan       (502) staff       (20)      497 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/eventloop/utils.py
--rw-r--r--   0 Ryan       (502) staff       (20)     2427 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/eventloop/asyncio_win32.py
--rw-r--r--   0 Ryan       (502) staff       (20)      735 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/eventloop/callbacks.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3568 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/eventloop/inputhook.py
--rw-r--r--   0 Ryan       (502) staff       (20)    11950 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/eventloop/posix.py
--rw-r--r--   0 Ryan       (502) staff       (20)     5930 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/eventloop/select.py
--rw-r--r--   0 Ryan       (502) staff       (20)     2752 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/eventloop/base.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1120 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/selection.py
--rw-r--r--   0 Ryan       (502) staff       (20)     2890 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/buffer_mapping.py
--rw-r--r--   0 Ryan       (502) staff       (20)     5033 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/output.py
--rw-r--r--   0 Ryan       (502) staff       (20)     3868 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/history.py
-drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-11 23:39:02.000000 rp-0.1.98/rp/prompt_toolkit/clipboard/
--rw-r--r--   0 Ryan       (502) staff       (20)     1140 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/clipboard/pyperclip.py
--rw-r--r--   0 Ryan       (502) staff       (20)      245 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/clipboard/__init__.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1493 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/clipboard/base.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1023 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/clipboard/in_memory.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1755 2019-09-11 23:39:01.000000 rp-0.1.98/rp/prompt_toolkit/validation.py
--rw-r--r--   0 Ryan       (502) staff       (20)       71 2019-09-11 23:39:01.000000 rp-0.1.98/rp/r_credentials.py
--rw-r--r--   0 Ryan       (502) staff       (20)     1015 2019-09-11 23:39:01.000000 rp-0.1.98/rp/r_iterm_comm.py
--rw-r--r--   0 Ryan       (502) staff       (20)     2052 2019-09-11 23:39:01.000000 rp-0.1.98/rp/vispy_test.py
--rw-r--r--   0 Ryan       (502) staff       (20)       95 2019-09-11 23:39:01.000000 rp-0.1.98/rp/__main__.py
--rw-r--r--   0 Ryan       (502) staff       (20)   242790 2019-09-11 23:39:01.000000 rp-0.1.98/rp/death_of_the_mind.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/
+-rw-r--r--   0 Ryan       (502) staff       (20)      347 2019-09-12 01:42:01.000000 rp-0.1.99/PKG-INFO
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp.egg-info/
+-rw-r--r--   0 Ryan       (502) staff       (20)      347 2019-09-12 01:42:01.000000 rp-0.1.99/rp.egg-info/PKG-INFO
+-rw-r--r--   0 Ryan       (502) staff       (20)     6148 2017-12-31 00:44:33.000000 rp-0.1.99/rp.egg-info/.DS_Store
+-rw-r--r--   0 Ryan       (502) staff       (20)     4974 2019-09-12 01:42:01.000000 rp-0.1.99/rp.egg-info/SOURCES.txt
+-rw-r--r--   0 Ryan       (502) staff       (20)       41 2019-09-12 01:42:01.000000 rp-0.1.99/rp.egg-info/entry_points.txt
+-rw-r--r--   0 Ryan       (502) staff       (20)       29 2019-09-12 01:42:01.000000 rp-0.1.99/rp.egg-info/requires.txt
+-rw-r--r--   0 Ryan       (502) staff       (20)        3 2019-09-12 01:42:01.000000 rp-0.1.99/rp.egg-info/top_level.txt
+-rw-r--r--   0 Ryan       (502) staff       (20)        1 2019-09-12 01:42:01.000000 rp-0.1.99/rp.egg-info/dependency_links.txt
+-rw-r--r--   0 Ryan       (502) staff       (20)      605 2017-12-15 05:14:49.000000 rp-0.1.99/README
+-rw-r--r--   0 Ryan       (502) staff       (20)     2460 2019-09-11 22:47:01.000000 rp-0.1.99/setup.py
+-rw-r--r--   0 Ryan       (502) staff       (20)       38 2019-09-12 01:42:01.000000 rp-0.1.99/setup.cfg
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/
+-rw-r--r--   0 Ryan       (502) staff       (20)   402279 2019-09-12 01:41:58.000000 rp-0.1.99/rp/automips2.py
+-rw-r--r--   0 Ryan       (502) staff       (20)        2 2019-09-12 01:42:00.000000 rp-0.1.99/rp/version.py
+-rw-r--r--   0 Ryan       (502) staff       (20)   421940 2019-09-12 01:41:58.000000 rp-0.1.99/rp/r.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    15604 2019-09-12 01:41:58.000000 rp-0.1.99/rp/pychess.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    19495 2019-09-12 01:41:58.000000 rp-0.1.99/rp/TestOSC.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     7388 2019-09-12 01:41:58.000000 rp-0.1.99/rp/Pyperclip.py
+-rw-r--r--   0 Ryan       (502) staff       (20)      421 2019-09-12 01:41:58.000000 rp-0.1.99/rp/google_colab.py
+-rw-r--r--   0 Ryan       (502) staff       (20)       19 2019-09-12 01:41:58.000000 rp-0.1.99/rp/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)      548 2019-09-12 01:41:58.000000 rp-0.1.99/rp/Test.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1470 2019-09-12 01:41:58.000000 rp-0.1.99/rp/shotgun.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/rp_ptpython/
+-rw-r--r--   0 Ryan       (502) staff       (20)     1667 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/validator.py
+-rw-r--r--   0 Ryan       (502) staff       (20)   152845 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/key_bindings.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1998 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/prompt_style.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    12204 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/style.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    29993 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/layout.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    10466 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/repl.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    14048 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/completerbackup.py
+-rw-r--r--   0 Ryan       (502) staff       (20)        0 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     2435 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/eventloop.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    12653 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/completer.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    12891 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/completer_stable.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    10606 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/ipython.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3956 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/utils.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    21239 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/history_browser.py
+-rw-r--r--   0 Ryan       (502) staff       (20)      159 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/__main__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     2772 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/untitled.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1582 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/filters.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    32079 2019-09-12 01:41:58.000000 rp-0.1.99/rp/rp_ptpython/python_input.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/filters/
+-rw-r--r--   0 Ryan       (502) staff       (20)     1691 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/filters/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1514 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/filters/types.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     9233 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/filters/cli.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1114 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/filters/utils.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     6082 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/filters/base.py
+-rw-r--r--   0 Ryan       (502) staff       (20)      792 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/enums.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1420 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/token.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1380 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/mouse_events.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     5723 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/completion.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    28167 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/shortcuts.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    19753 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/renderer.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/layout/
+-rw-r--r--   0 Ryan       (502) staff       (20)     4490 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/layout/screen.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    28561 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/layout/controls.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     7048 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/layout/toolbars.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    67803 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/layout/containers.py
+-rw-r--r--   0 Ryan       (502) staff       (20)      780 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/layout/mouse_handlers.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1909 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/layout/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     8858 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/layout/margins.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     5472 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/layout/utils.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3242 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/layout/prompt.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    21760 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/layout/processors.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    19438 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/layout/menus.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    11343 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/layout/lexers.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3154 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/layout/dimension.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     2842 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/auto_suggest.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     4046 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/win32_types.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    42395 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/interface.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1841 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/reactive.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3400 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/cache.py
+-rw-r--r--   0 Ryan       (502) staff       (20)      632 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/__init__.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/terminal/
+-rw-r--r--   0 Ryan       (502) staff       (20)    19863 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/terminal/vt100_output.py
+-rw-r--r--   0 Ryan       (502) staff       (20)        0 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/terminal/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    19622 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/terminal/win32_output.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    13064 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/terminal/win32_input.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    18428 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/terminal/vt100_input.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1397 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/terminal/conemu_output.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3630 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/keys.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/contrib/
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/contrib/completers/
+-rw-r--r--   0 Ryan       (502) staff       (20)     1922 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/completers/system.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3762 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/completers/filesystem.py
+-rw-r--r--   0 Ryan       (502) staff       (20)      147 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/completers/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     2275 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/completers/base.py
+-rw-r--r--   0 Ryan       (502) staff       (20)        0 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/__init__.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/contrib/regular_languages/
+-rw-r--r--   0 Ryan       (502) staff       (20)    15633 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/regular_languages/compiler.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3032 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/regular_languages/completion.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3286 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/regular_languages/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3414 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/regular_languages/lexer.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     7266 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/regular_languages/regex_parser.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     2065 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/regular_languages/validation.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/contrib/validators/
+-rw-r--r--   0 Ryan       (502) staff       (20)        0 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/validators/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1243 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/validators/base.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/contrib/telnet/
+-rw-r--r--   0 Ryan       (502) staff       (20)    12914 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/telnet/server.py
+-rw-r--r--   0 Ryan       (502) staff       (20)      170 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/telnet/log.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     4884 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/telnet/protocol.py
+-rw-r--r--   0 Ryan       (502) staff       (20)       49 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/telnet/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)      894 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/contrib/telnet/application.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/
+-rw-r--r--   0 Ryan       (502) staff       (20)    11499 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/registry.py
+-rw-r--r--   0 Ryan       (502) staff       (20)       40 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    11937 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/input_processor.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     4933 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/defaults.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/
+-rw-r--r--   0 Ryan       (502) staff       (20)    15940 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/named_commands.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     5659 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/completion.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     5711 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/scroll.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    67865 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/vi.py
+-rw-r--r--   0 Ryan       (502) staff       (20)        0 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    15542 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/emacs.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    13352 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/basic.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1734 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/vi_state.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    32842 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/digraphs.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3730 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/key_binding/manager.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1099 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/search_state.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     8747 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/application.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/styles/
+-rw-r--r--   0 Ryan       (502) staff       (20)      504 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/styles/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1198 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/styles/utils.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     4579 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/styles/from_dict.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3698 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/styles/defaults.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     2349 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/styles/from_pygments.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     2489 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/styles/base.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     6359 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/utils.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3214 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/input.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    51517 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/buffer.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    35976 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/document.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/eventloop/
+-rw-r--r--   0 Ryan       (502) staff       (20)     3312 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/eventloop/posix_utils.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3363 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/eventloop/asyncio_posix.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1152 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/eventloop/asyncio_base.py
+-rw-r--r--   0 Ryan       (502) staff       (20)        0 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/eventloop/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     6196 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/eventloop/win32.py
+-rw-r--r--   0 Ryan       (502) staff       (20)      497 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/eventloop/utils.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     2427 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/eventloop/asyncio_win32.py
+-rw-r--r--   0 Ryan       (502) staff       (20)      735 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/eventloop/callbacks.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3568 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/eventloop/inputhook.py
+-rw-r--r--   0 Ryan       (502) staff       (20)    11950 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/eventloop/posix.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     5930 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/eventloop/select.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     2752 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/eventloop/base.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1120 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/selection.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     2890 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/buffer_mapping.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     5033 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/output.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     3868 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/history.py
+drwxr-xr-x   0 Ryan       (502) staff       (20)        0 2019-09-12 01:42:01.000000 rp-0.1.99/rp/prompt_toolkit/clipboard/
+-rw-r--r--   0 Ryan       (502) staff       (20)     1140 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/clipboard/pyperclip.py
+-rw-r--r--   0 Ryan       (502) staff       (20)      245 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/clipboard/__init__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1493 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/clipboard/base.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1023 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/clipboard/in_memory.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1755 2019-09-12 01:41:58.000000 rp-0.1.99/rp/prompt_toolkit/validation.py
+-rw-r--r--   0 Ryan       (502) staff       (20)       71 2019-09-12 01:41:58.000000 rp-0.1.99/rp/r_credentials.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     1015 2019-09-12 01:41:58.000000 rp-0.1.99/rp/r_iterm_comm.py
+-rw-r--r--   0 Ryan       (502) staff       (20)     2052 2019-09-12 01:41:59.000000 rp-0.1.99/rp/vispy_test.py
+-rw-r--r--   0 Ryan       (502) staff       (20)       95 2019-09-12 01:41:59.000000 rp-0.1.99/rp/__main__.py
+-rw-r--r--   0 Ryan       (502) staff       (20)   242790 2019-09-12 01:41:59.000000 rp-0.1.99/rp/death_of_the_mind.py
```

### Comparing `rp-0.1.98/rp.egg-info/.DS_Store` & `rp-0.1.99/rp.egg-info/.DS_Store`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp.egg-info/SOURCES.txt` & `rp-0.1.99/rp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/README` & `rp-0.1.99/README`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/setup.py` & `rp-0.1.99/setup.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/automips2.py` & `rp-0.1.99/rp/automips2.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/r.py` & `rp-0.1.99/rp/r.py`

 * *Files 0% similar despite different names*

```diff
@@ -938,44 +938,48 @@
         return False
     try:
         result=urlparse(url)
         return all([result.scheme, result.netloc])
     except:
         return False
 # region  Saving/Loading Images: ［load_image，load_image_from_url，save_image，save_image_jpg］
+
 _load_image_cache={}#TODO Test this and make sure it works. This is currently untested.
 def load_image(location,*,from_cache=False):
     #Automatically detect if location is a URL or a file path and try to smartly choose the appropriate function to load the image
     assert isinstance(location,str),'load_image error: location should be a string representing a URL or file path. However, location is not a string. type(location)=='+repr(type(location))+' and location=='+repr(location)
     if from_cache and location in _load_image_cache and from_cache:
-        return _load_image_cache[location]
+        return _load_image_cache[location].copy()
     if is_valid_url(location):
         out = load_image_from_url (location)
     else:
         out = load_image_from_file(location)
     _load_image_cache[location]=out
     return out
 
+def load_images(*locations,from_cache=False):
+    #Simply the plural form of load_image
+    locations=delist(detuple(locations))
+    return [load_image(location,from_cache=from_cache) for location in locations]
+
 def load_image_from_file(file_name):
     #Can try opencv as a fallback if this ever breaks
     try               :return _load_image_from_file_via_scipy (file_name)
     except ImportError:return _load_image_from_file_via_opencv(file_name)#Expecting that scipy.misc.imread doesn't exist on the interpereter for whatever reason
 
 def _load_image_from_file_via_scipy(file_name):
     from scipy.misc import imread
     return imread(file_name)
 
 def _load_image_from_file_via_opencv(file_name):
     import cv2
     image=cv2.imread(file_name)
     if image is None:
         raise FileNotFoundError("Cannot find an image file at the file path: "+file_name)#By default, opencv doesn't raise an error when the file isn't found, and just returns None....which is dumb. It should act like scipy.misc.imread, which throws a FileNotFoundError when given an invalid path.
-    out=image.copy()#In order to swap the color channels, we have to make a copy (else it will mutate the original image in the middle of copying it, which is no good)
-    out[:,:,0],out[:,:,2]=image[:,:,2],image[:,:,0]#OpenCV is really weird and doesn't use RGB: It uses BGR for some strange legacy reason. We have to swap the channels to make it useful.
-    return out
+    return cv_bgr_rgb_swap(image)#OpenCV is really weird and doesn't use RGB: It uses BGR for some strange legacy reason. We have to swap the channels to make it useful.
 
 
 
 def load_image_from_url(url: str):
     assert is_valid_url(url),'load_image_from_url error: invalid url: '+repr(url)
     from PIL import Image
     import requests
@@ -7236,15 +7240,16 @@
 
 def input_yes_no(question):
     #A boolean function of the user's console input
     #The user must say y, ye, yes, n or no to continue
     #Example: input_yes_no('Are you feeling well today?')
     return 'yes'.startswith(input_conditional(question+'\nPlease enter yes or no.', lambda x: x.lower() in {'y','ye','yes','n','no'}).lower())
 
-def download_youtube_video(url,path='./',):
+@memoized
+def download_youtube_video(url,path='./'):
     #TODO: Implement a fallback method using 'you_get' (you_get is a pypy package. where pytube gets 403 permission errors donwloading lindsey stirling videos, you_get succeedes)
     import pytube
     yt = pytube.YouTube(url)
     stream = yt.streams.first()
     stream.download(path)
     return os.path.join(path,stream.default_filename)
 
@@ -7387,18 +7392,85 @@
         os.mkdir(path)
     return path
 make_folder=make_directory
 
 def delete_all_files_in_directory(directory,*,permanent=False):
     assert directory_exists(directory)
     delete_paths(get_file_paths(directory),permanent=permanent)
+delete_all_files_in_folder=delete_all_files_in_directory
 
 joined_paths=os.path.join
 
-delete_all_files_in_folder=delete_all_files_in_directory
+
+
+_get_cutscene_frame_numbers_cache={}
+def get_cutscene_frame_numbers(video_path,*,from_cache=False):
+    #Returns a list of ints containing all the framenumers of the cutscenes in a video
+    #Confirmed to work with mp4 files
+    #Note: Right now this only supports reading from a video file, as opposed to reading from a numpy array containing
+    #pip install scenedetect
+    #Code from https://pyscenedetect-manual.readthedocs.io/en/latest/api/scene_manager.html#scenemanager-example
+    #EXAMPLE:
+    #    video_path=download_youtube_video('https://www.youtube.com/watch?v=K5qACexzwOI')
+    #    cutscene_frames_numbers=get_cutscene_frame_numbers(video_path)
+    #    for i,frame in enumerate(load_video_stream(video_path)):
+    #        if i in cutscene_frames_numbers:
+    #            input('Hit enter to continue')
+    #        cv_imshow(frame)
+    #        sleep(1/30)
+            
+    if video_path in _get_cutscene_frame_numbers_cache:
+        return _get_cutscene_frame_numbers_cache[video_path]
+
+    # Standard PySceneDetect imports:
+    from scenedetect.video_manager import VideoManager
+    from scenedetect.scene_manager import SceneManager
+    # For caching detection metrics and saving/loading to a stats file
+    from scenedetect.stats_manager import StatsManager
+
+    # For content-aware scene detection:
+    from scenedetect.detectors.content_detector import ContentDetector
+
+    # type: (str) -> List[Tuple[FrameTimecode, FrameTimecode]]
+    video_manager = VideoManager([video_path])
+    stats_manager = StatsManager()
+    # Construct our SceneManager and pass it our StatsManager.
+    scene_manager = SceneManager(stats_manager)
+
+    # Add ContentDetector algorithm (each detector's constructor
+    # takes detector options, e.g. threshold).
+    scene_manager.add_detector(ContentDetector())
+    base_timecode = video_manager.get_base_timecode()
+
+    # We save our stats file to {VIDEO_PATH}.stats.csv.
+
+    scene_list = []
+
+    try:
+        # Set downscale factor to improve processing speed.
+        video_manager.set_downscale_factor()
+
+        # Start video_manager.
+        video_manager.start()
+
+        # Perform scene detection on video_manager.
+        scene_manager.detect_scenes(frame_source=video_manager)
+
+        # Obtain list of detected scenes.
+        scene_list = scene_manager.get_scene_list(base_timecode)
+        # Each scene is a tuple of (start, end) FrameTimecodes.
+
+    finally:
+        video_manager.release()
+
+    output = [x[1].frame_num for x in scene_list]
+    _get_cutscene_frame_numbers_cache[video_path]=output
+    return output
+
+
 if __name__ == "__main__":
     print(end='\r')
     pterm()
 
 
 # endregion
```

### Comparing `rp-0.1.98/rp/pychess.py` & `rp-0.1.99/rp/pychess.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/TestOSC.py` & `rp-0.1.99/rp/TestOSC.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/Pyperclip.py` & `rp-0.1.99/rp/Pyperclip.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/Test.py` & `rp-0.1.99/rp/Test.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/shotgun.py` & `rp-0.1.99/rp/shotgun.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/validator.py` & `rp-0.1.99/rp/rp_ptpython/validator.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/key_bindings.py` & `rp-0.1.99/rp/rp_ptpython/key_bindings.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/prompt_style.py` & `rp-0.1.99/rp/rp_ptpython/prompt_style.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/style.py` & `rp-0.1.99/rp/rp_ptpython/style.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/layout.py` & `rp-0.1.99/rp/rp_ptpython/layout.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/repl.py` & `rp-0.1.99/rp/rp_ptpython/repl.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/completerbackup.py` & `rp-0.1.99/rp/rp_ptpython/completerbackup.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/eventloop.py` & `rp-0.1.99/rp/rp_ptpython/eventloop.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/completer.py` & `rp-0.1.99/rp/rp_ptpython/completer.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/completer_stable.py` & `rp-0.1.99/rp/rp_ptpython/completer_stable.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/ipython.py` & `rp-0.1.99/rp/rp_ptpython/ipython.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/utils.py` & `rp-0.1.99/rp/rp_ptpython/utils.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/history_browser.py` & `rp-0.1.99/rp/rp_ptpython/history_browser.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/untitled.py` & `rp-0.1.99/rp/rp_ptpython/untitled.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/filters.py` & `rp-0.1.99/rp/rp_ptpython/filters.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/rp_ptpython/python_input.py` & `rp-0.1.99/rp/rp_ptpython/python_input.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/filters/__init__.py` & `rp-0.1.99/rp/prompt_toolkit/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/filters/types.py` & `rp-0.1.99/rp/prompt_toolkit/filters/types.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/filters/cli.py` & `rp-0.1.99/rp/prompt_toolkit/filters/cli.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/filters/utils.py` & `rp-0.1.99/rp/prompt_toolkit/filters/utils.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/filters/base.py` & `rp-0.1.99/rp/prompt_toolkit/filters/base.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/enums.py` & `rp-0.1.99/rp/prompt_toolkit/enums.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/token.py` & `rp-0.1.99/rp/prompt_toolkit/token.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/mouse_events.py` & `rp-0.1.99/rp/prompt_toolkit/mouse_events.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/completion.py` & `rp-0.1.99/rp/prompt_toolkit/completion.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/shortcuts.py` & `rp-0.1.99/rp/prompt_toolkit/shortcuts.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/renderer.py` & `rp-0.1.99/rp/prompt_toolkit/renderer.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/layout/screen.py` & `rp-0.1.99/rp/prompt_toolkit/layout/screen.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/layout/controls.py` & `rp-0.1.99/rp/prompt_toolkit/layout/controls.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/layout/toolbars.py` & `rp-0.1.99/rp/prompt_toolkit/layout/toolbars.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/layout/containers.py` & `rp-0.1.99/rp/prompt_toolkit/layout/containers.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/layout/mouse_handlers.py` & `rp-0.1.99/rp/prompt_toolkit/layout/mouse_handlers.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/layout/__init__.py` & `rp-0.1.99/rp/prompt_toolkit/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/layout/margins.py` & `rp-0.1.99/rp/prompt_toolkit/layout/margins.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/layout/utils.py` & `rp-0.1.99/rp/prompt_toolkit/layout/utils.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/layout/prompt.py` & `rp-0.1.99/rp/prompt_toolkit/layout/prompt.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/layout/processors.py` & `rp-0.1.99/rp/prompt_toolkit/layout/processors.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/layout/menus.py` & `rp-0.1.99/rp/prompt_toolkit/layout/menus.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/layout/lexers.py` & `rp-0.1.99/rp/prompt_toolkit/layout/lexers.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/layout/dimension.py` & `rp-0.1.99/rp/prompt_toolkit/layout/dimension.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/auto_suggest.py` & `rp-0.1.99/rp/prompt_toolkit/auto_suggest.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/win32_types.py` & `rp-0.1.99/rp/prompt_toolkit/win32_types.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/interface.py` & `rp-0.1.99/rp/prompt_toolkit/interface.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/reactive.py` & `rp-0.1.99/rp/prompt_toolkit/reactive.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/cache.py` & `rp-0.1.99/rp/prompt_toolkit/cache.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/__init__.py` & `rp-0.1.99/rp/prompt_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/terminal/vt100_output.py` & `rp-0.1.99/rp/prompt_toolkit/terminal/vt100_output.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/terminal/win32_output.py` & `rp-0.1.99/rp/prompt_toolkit/terminal/win32_output.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/terminal/win32_input.py` & `rp-0.1.99/rp/prompt_toolkit/terminal/win32_input.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/terminal/vt100_input.py` & `rp-0.1.99/rp/prompt_toolkit/terminal/vt100_input.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/terminal/conemu_output.py` & `rp-0.1.99/rp/prompt_toolkit/terminal/conemu_output.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/keys.py` & `rp-0.1.99/rp/prompt_toolkit/keys.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/contrib/completers/system.py` & `rp-0.1.99/rp/prompt_toolkit/contrib/completers/system.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/contrib/completers/filesystem.py` & `rp-0.1.99/rp/prompt_toolkit/contrib/completers/filesystem.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/contrib/completers/base.py` & `rp-0.1.99/rp/prompt_toolkit/contrib/completers/base.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/contrib/regular_languages/compiler.py` & `rp-0.1.99/rp/prompt_toolkit/contrib/regular_languages/compiler.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/contrib/regular_languages/completion.py` & `rp-0.1.99/rp/prompt_toolkit/contrib/regular_languages/completion.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/contrib/regular_languages/__init__.py` & `rp-0.1.99/rp/prompt_toolkit/contrib/regular_languages/__init__.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/contrib/regular_languages/lexer.py` & `rp-0.1.99/rp/prompt_toolkit/contrib/regular_languages/lexer.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/contrib/regular_languages/regex_parser.py` & `rp-0.1.99/rp/prompt_toolkit/contrib/regular_languages/regex_parser.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/contrib/regular_languages/validation.py` & `rp-0.1.99/rp/prompt_toolkit/contrib/regular_languages/validation.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/contrib/validators/base.py` & `rp-0.1.99/rp/prompt_toolkit/contrib/validators/base.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/contrib/telnet/server.py` & `rp-0.1.99/rp/prompt_toolkit/contrib/telnet/server.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/contrib/telnet/protocol.py` & `rp-0.1.99/rp/prompt_toolkit/contrib/telnet/protocol.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/contrib/telnet/application.py` & `rp-0.1.99/rp/prompt_toolkit/contrib/telnet/application.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/key_binding/registry.py` & `rp-0.1.99/rp/prompt_toolkit/key_binding/registry.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/key_binding/input_processor.py` & `rp-0.1.99/rp/prompt_toolkit/key_binding/input_processor.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/key_binding/defaults.py` & `rp-0.1.99/rp/prompt_toolkit/key_binding/defaults.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/named_commands.py` & `rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/named_commands.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/completion.py` & `rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/completion.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/scroll.py` & `rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/scroll.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/vi.py` & `rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/vi.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/emacs.py` & `rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/emacs.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/key_binding/bindings/basic.py` & `rp-0.1.99/rp/prompt_toolkit/key_binding/bindings/basic.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/key_binding/vi_state.py` & `rp-0.1.99/rp/prompt_toolkit/key_binding/vi_state.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/key_binding/digraphs.py` & `rp-0.1.99/rp/prompt_toolkit/key_binding/digraphs.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/key_binding/manager.py` & `rp-0.1.99/rp/prompt_toolkit/key_binding/manager.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/search_state.py` & `rp-0.1.99/rp/prompt_toolkit/search_state.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/application.py` & `rp-0.1.99/rp/prompt_toolkit/application.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/styles/utils.py` & `rp-0.1.99/rp/prompt_toolkit/styles/utils.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/styles/from_dict.py` & `rp-0.1.99/rp/prompt_toolkit/styles/from_dict.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/styles/defaults.py` & `rp-0.1.99/rp/prompt_toolkit/styles/defaults.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/styles/from_pygments.py` & `rp-0.1.99/rp/prompt_toolkit/styles/from_pygments.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/styles/base.py` & `rp-0.1.99/rp/prompt_toolkit/styles/base.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/utils.py` & `rp-0.1.99/rp/prompt_toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/input.py` & `rp-0.1.99/rp/prompt_toolkit/input.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/buffer.py` & `rp-0.1.99/rp/prompt_toolkit/buffer.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/document.py` & `rp-0.1.99/rp/prompt_toolkit/document.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/eventloop/posix_utils.py` & `rp-0.1.99/rp/prompt_toolkit/eventloop/posix_utils.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/eventloop/asyncio_posix.py` & `rp-0.1.99/rp/prompt_toolkit/eventloop/asyncio_posix.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/eventloop/asyncio_base.py` & `rp-0.1.99/rp/prompt_toolkit/eventloop/asyncio_base.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/eventloop/win32.py` & `rp-0.1.99/rp/prompt_toolkit/eventloop/win32.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/eventloop/asyncio_win32.py` & `rp-0.1.99/rp/prompt_toolkit/eventloop/asyncio_win32.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/eventloop/callbacks.py` & `rp-0.1.99/rp/prompt_toolkit/eventloop/callbacks.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/eventloop/inputhook.py` & `rp-0.1.99/rp/prompt_toolkit/eventloop/inputhook.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/eventloop/posix.py` & `rp-0.1.99/rp/prompt_toolkit/eventloop/posix.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/eventloop/select.py` & `rp-0.1.99/rp/prompt_toolkit/eventloop/select.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/eventloop/base.py` & `rp-0.1.99/rp/prompt_toolkit/eventloop/base.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/selection.py` & `rp-0.1.99/rp/prompt_toolkit/selection.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/buffer_mapping.py` & `rp-0.1.99/rp/prompt_toolkit/buffer_mapping.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/output.py` & `rp-0.1.99/rp/prompt_toolkit/output.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/history.py` & `rp-0.1.99/rp/prompt_toolkit/history.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/clipboard/pyperclip.py` & `rp-0.1.99/rp/prompt_toolkit/clipboard/pyperclip.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/clipboard/base.py` & `rp-0.1.99/rp/prompt_toolkit/clipboard/base.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/clipboard/in_memory.py` & `rp-0.1.99/rp/prompt_toolkit/clipboard/in_memory.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/prompt_toolkit/validation.py` & `rp-0.1.99/rp/prompt_toolkit/validation.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/r_iterm_comm.py` & `rp-0.1.99/rp/r_iterm_comm.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/vispy_test.py` & `rp-0.1.99/rp/vispy_test.py`

 * *Files identical despite different names*

### Comparing `rp-0.1.98/rp/death_of_the_mind.py` & `rp-0.1.99/rp/death_of_the_mind.py`

 * *Files identical despite different names*

