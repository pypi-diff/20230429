# Comparing `tmp/types-docutils-0.19.1.7.tar.gz` & `tmp/types-docutils-0.19.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-docutils-0.19.1.7.tar", last modified: Mon Mar 27 18:23:05 2023, max compression
+gzip compressed data, was "types-docutils-0.19.1.8.tar", last modified: Sat Apr 29 15:14:09 2023, max compression
```

## Comparing `types-docutils-0.19.1.7.tar` & `types-docutils-0.19.1.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:05.110352 types-docutils-0.19.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-03-27 18:23:04.000000 types-docutils-0.19.1.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:23:04.000000 types-docutils-0.19.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-27 18:23:05.110352 types-docutils-0.19.1.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:05.102352 types-docutils-0.19.1.7/docutils-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-27 18:23:04.000000 types-docutils-0.19.1.7/docutils-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/examples.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/frontend.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/io.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:05.102352 types-docutils-0.19.1.7/docutils-stubs/languages/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/languages/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/nodes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:05.102352 types-docutils-0.19.1.7/docutils-stubs/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/null.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/recommonmark_wrapper.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:05.106352 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:05.106352 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/directives/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/directives/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/directives/admonitions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/directives/body.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/directives/html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/directives/images.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/directives/misc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/directives/parts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/directives/references.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/directives/tables.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/roles.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/parsers/rst/states.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:05.106352 types-docutils-0.19.1.7/docutils-stubs/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/readers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/readers/doctree.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/readers/pep.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/readers/standalone.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/statemachine.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:05.106352 types-docutils-0.19.1.7/docutils-stubs/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/transforms/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:05.106352 types-docutils-0.19.1.7/docutils-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:05.106352 types-docutils-0.19.1.7/docutils-stubs/writers/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/writers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/writers/docutils_xml.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/writers/html4css1.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/writers/html5_polyglot.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/writers/latex2e.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/writers/manpage.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/writers/null.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/writers/odf_odt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/writers/pep_html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/writers/pseudoxml.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/writers/s5_html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 18:21:24.000000 types-docutils-0.19.1.7/docutils-stubs/writers/xetex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:23:05.110352 types-docutils-0.19.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-27 18:23:04.000000 types-docutils-0.19.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:05.110352 types-docutils-0.19.1.7/types_docutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-27 18:23:05.000000 types-docutils-0.19.1.7/types_docutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-27 18:23:05.000000 types-docutils-0.19.1.7/types_docutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:23:05.000000 types-docutils-0.19.1.7/types_docutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-27 18:23:05.000000 types-docutils-0.19.1.7/types_docutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.832734 types-docutils-0.19.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 15:14:09.832734 types-docutils-0.19.1.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/docutils-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/examples.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/frontend.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/io.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/languages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/nodes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/null.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/recommonmark_wrapper.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/admonitions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/body.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/misc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/parts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/references.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/directives/tables.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/roles.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/parsers/rst/states.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/readers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/readers/doctree.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/readers/pep.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/readers/standalone.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/statemachine.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/transforms/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.828734 types-docutils-0.19.1.8/docutils-stubs/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/docutils_xml.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/html4css1.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/html5_polyglot.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/latex2e.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/manpage.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/null.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/odf_odt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/pep_html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/pseudoxml.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/s5_html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:13:39.000000 types-docutils-0.19.1.8/docutils-stubs/writers/xetex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:14:09.832734 types-docutils-0.19.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:09.832734 types-docutils-0.19.1.8/types_docutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/types_docutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/types_docutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/types_docutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 15:14:09.000000 types-docutils-0.19.1.8/types_docutils.egg-info/top_level.txt
```

### Comparing `types-docutils-0.19.1.7/CHANGELOG.md` & `types-docutils-0.19.1.8/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+## 0.19.1.8 (2023-04-29)
+
+docutils: Input can take bytearray (#10108)
+
+Part of #9006
+
+docutils: add nodes.General; make Element iterable (#10099)
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 0.19.1.7 (2023-03-27)
 
 Add defaults for third-party stubs A-D (#9952)
 
 ## 0.19.1.6 (2023-02-22)
 
 Update `Unused` parameters in `stubs/` (#9704)
```

### Comparing `types-docutils-0.19.1.7/PKG-INFO` & `types-docutils-0.19.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docutils
-Version: 0.19.1.7
+Version: 0.19.1.8
 Summary: Typing stubs for docutils
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docutils.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `docutils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docutils. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
```

### Comparing `types-docutils-0.19.1.7/docutils-stubs/__init__.pyi` & `types-docutils-0.19.1.8/docutils-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.7/docutils-stubs/frontend.pyi` & `types-docutils-0.19.1.8/docutils-stubs/frontend.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.7/docutils-stubs/io.pyi` & `types-docutils-0.19.1.8/docutils-stubs/io.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 def check_encoding(stream: Any, encoding: str) -> bool | None: ...
 def error_string(err: BaseException) -> str: ...
 
 class Input(TransformSpec):
     component_type: ClassVar[str]
     default_source_path: ClassVar[str | None]
     def read(self) -> Any: ...
-    def decode(self, data: str | bytes) -> str: ...
+    def decode(self, data: str | bytes | bytearray) -> str: ...
     coding_slug: ClassVar[Pattern[bytes]]
     byte_order_marks: ClassVar[tuple[tuple[bytes, str], ...]]
-    def determine_encoding_from_data(self, data: str | bytes) -> str | None: ...
+    def determine_encoding_from_data(self, data: str | bytes | bytearray) -> str | None: ...
     def isatty(self) -> bool: ...
 
 class Output(TransformSpec):
     component_type: ClassVar[str]
     default_destination_path: ClassVar[str | None]
     def __init__(
         self,
```

### Comparing `types-docutils-0.19.1.7/docutils-stubs/nodes.pyi` & `types-docutils-0.19.1.8/docutils-stubs/nodes.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import xml.dom.minidom
 from _typeshed import Incomplete
 from abc import abstractmethod
-from collections.abc import Callable, Generator, Iterable, Sequence
+from collections.abc import Callable, Generator, Iterable, Iterator, Sequence
 from typing import Any, ClassVar, Protocol, TypeVar, overload
 from typing_extensions import Literal, Self
 
 from docutils.transforms import Transformer
 
 _N = TypeVar("_N", bound=Node)
 
@@ -78,14 +78,17 @@
     def previous_sibling(self) -> Node | None: ...
 
 class Element(Node):
     children: list[Node]
     def __init__(self, rawsource: str = "", *children: Node, **attributes): ...
     def __len__(self) -> int: ...
     def __contains__(self, key: str | Node) -> bool: ...
+    # '__iter__' is added as workaround, since mypy doesn't support classes that are iterable via '__getitem__'
+    # see https://github.com/python/typeshed/pull/10099#issuecomment-1528789395
+    def __iter__(self) -> Iterator[Node]: ...
     @overload
     def __getitem__(self, key: str) -> Any: ...
     @overload
     def __getitem__(self, key: int) -> Node: ...
     @overload
     def __getitem__(self, key: slice) -> list[Node]: ...
     @overload
@@ -116,14 +119,16 @@
     def deepcopy(self) -> Self: ...
     def pformat(self, indent: str = "    ", level: int = 0) -> str: ...
     def astext(self) -> str: ...
     def rstrip(self, chars: str | None = None) -> str: ...
     def lstrip(self, chars: str | None = None) -> str: ...
 
 class Structural: ...
+class Body: ...
+class General(Body): ...
 class Root: ...
 
 class document(Root, Structural, Element):
     transformer: Transformer
     def copy(self) -> Self: ...
     def deepcopy(self) -> Self: ...
     def pformat(self, indent: str = "    ", level: int = 0) -> str: ...
```

### Comparing `types-docutils-0.19.1.7/docutils-stubs/parsers/__init__.pyi` & `types-docutils-0.19.1.8/docutils-stubs/parsers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.7/docutils-stubs/parsers/rst/__init__.pyi` & `types-docutils-0.19.1.8/docutils-stubs/parsers/rst/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.7/docutils-stubs/parsers/rst/roles.pyi` & `types-docutils-0.19.1.8/docutils-stubs/parsers/rst/roles.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.7/docutils-stubs/transforms/__init__.pyi` & `types-docutils-0.19.1.8/docutils-stubs/transforms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.7/docutils-stubs/utils/__init__.pyi` & `types-docutils-0.19.1.8/docutils-stubs/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.7/setup.py` & `types-docutils-0.19.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `docutils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docutils. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.19.1.7",
+      version="0.19.1.8",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docutils.md",
```

### Comparing `types-docutils-0.19.1.7/types_docutils.egg-info/PKG-INFO` & `types-docutils-0.19.1.8/types_docutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docutils
-Version: 0.19.1.7
+Version: 0.19.1.8
 Summary: Typing stubs for docutils
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docutils.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `docutils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docutils. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
```

### Comparing `types-docutils-0.19.1.7/types_docutils.egg-info/SOURCES.txt` & `types-docutils-0.19.1.8/types_docutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

