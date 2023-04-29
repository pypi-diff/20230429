# Comparing `tmp/ManimPango-0.4.3.tar.gz` & `tmp/ManimPango-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ManimPango-0.4.3.tar", last modified: Sun Nov 27 17:06:56 2022, max compression
+gzip compressed data, was "ManimPango-1.0.0a1.tar", last modified: Sat Apr 29 17:38:49 2023, max compression
```

## Comparing `ManimPango-0.4.3.tar` & `ManimPango-1.0.0a1.tar`

### file list

```diff
@@ -1,59 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 17:06:56.235625 ManimPango-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2022-11-27 17:06:42.000000 ManimPango-0.4.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      189 2022-11-27 17:06:42.000000 ManimPango-0.4.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2022-11-27 17:06:42.000000 ManimPango-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      201 2022-11-27 17:06:42.000000 ManimPango-0.4.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 17:06:56.227625 ManimPango-0.4.3/ManimPango.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2022-11-27 17:06:56.000000 ManimPango-0.4.3/ManimPango.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-11-27 17:06:56.000000 ManimPango-0.4.3/ManimPango.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-27 17:06:56.000000 ManimPango-0.4.3/ManimPango.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-27 17:06:56.000000 ManimPango-0.4.3/ManimPango.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-11-27 17:06:56.000000 ManimPango-0.4.3/ManimPango.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2022-11-27 17:06:56.235625 ManimPango-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2022-11-27 17:06:42.000000 ManimPango-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 17:06:56.227625 ManimPango-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2022-11-27 17:06:42.000000 ManimPango-0.4.3/docs/RELEASE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 17:06:56.227625 ManimPango-0.4.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2022-11-27 17:06:42.000000 ManimPango-0.4.3/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 17:06:56.227625 ManimPango-0.4.3/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 17:06:56.227625 ManimPango-0.4.3/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2022-11-27 17:06:42.000000 ManimPango-0.4.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      943 2022-11-27 17:06:42.000000 ManimPango-0.4.3/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2022-11-27 17:06:42.000000 ManimPango-0.4.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2022-11-27 17:06:42.000000 ManimPango-0.4.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2022-11-27 17:06:42.000000 ManimPango-0.4.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      384 2022-11-27 17:06:42.000000 ManimPango-0.4.3/docs/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 17:06:56.227625 ManimPango-0.4.3/manimpango/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2022-11-27 17:06:42.000000 ManimPango-0.4.3/manimpango/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-11-27 17:06:42.000000 ManimPango-0.4.3/manimpango/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2022-11-27 17:06:42.000000 ManimPango-0.4.3/manimpango/cairo.pxd
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-11-27 17:06:42.000000 ManimPango-0.4.3/manimpango/cmanimpango.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2022-11-27 17:06:42.000000 ManimPango-0.4.3/manimpango/cmanimpango.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2022-11-27 17:06:42.000000 ManimPango-0.4.3/manimpango/enums.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      374 2022-11-27 17:06:42.000000 ManimPango-0.4.3/manimpango/glib.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2022-11-27 17:06:42.000000 ManimPango-0.4.3/manimpango/pango.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2022-11-27 17:06:42.000000 ManimPango-0.4.3/manimpango/register_font.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2022-11-27 17:06:42.000000 ManimPango-0.4.3/manimpango/register_font.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2022-11-27 17:06:42.000000 ManimPango-0.4.3/manimpango/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2022-11-27 17:06:42.000000 ManimPango-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-11-27 17:06:42.000000 ManimPango-0.4.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2022-11-27 17:06:56.235625 ManimPango-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2022-11-27 17:06:42.000000 ManimPango-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 17:06:56.231625 ManimPango-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/_manim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 17:06:56.231625 ManimPango-0.4.3/tests/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   183752 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/fonts/AdobeVFPrototype.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    75348 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/fonts/BungeeColor-Regular_colr_Windows.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   235924 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/fonts/BungeeOutline-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      541 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/fonts/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  5856032 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/fonts/MaShanZheng-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/svg_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/test_fonts.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/test_list_fonts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/test_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/test_valid_svg.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2022-11-27 17:06:42.000000 ManimPango-0.4.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.567579 ManimPango-1.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.543579 ManimPango-1.0.0a1/ManimPango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-29 17:38:49.000000 ManimPango-1.0.0a1/ManimPango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-29 17:38:49.000000 ManimPango-1.0.0a1/ManimPango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:38:49.000000 ManimPango-1.0.0a1/ManimPango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:38:49.000000 ManimPango-1.0.0a1/ManimPango.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 17:38:49.000000 ManimPango-1.0.0a1/ManimPango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-29 17:38:49.567579 ManimPango-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.547579 ManimPango-1.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.547579 ManimPango-1.0.0a1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.539579 ManimPango-1.0.0a1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.547579 ManimPango-1.0.0a1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/building.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/news.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/docs/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.547579 ManimPango-1.0.0a1/manimpango/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/_distributor_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.547579 ManimPango-1.0.0a1/manimpango/attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/cmanimpango.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/cmanimpango.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/enums.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.551579 ManimPango-1.0.0a1/manimpango/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/fonts/_font_desc.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/fonts/_font_desc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/fonts/_font_desc.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/fonts/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/fonts/enums.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.551579 ManimPango-1.0.0a1/manimpango/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/include/cairo.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/include/glib.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/include/pango.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/include/pango_attributes.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.551579 ManimPango-1.0.0a1/manimpango/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/layout/_layout.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/register_font.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/register_font.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.551579 ManimPango-1.0.0a1/manimpango/renderer/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/image_renderer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/image_renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/image_renderer.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/svg_renderer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/svg_renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/renderer/svg_renderer.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.555579 ManimPango-1.0.0a1/manimpango/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/utils/_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/manimpango/utils/utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-29 17:38:49.567579 ManimPango-1.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.555579 ManimPango-1.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/_manim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:38:49.559579 ManimPango-1.0.0a1/tests/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   183752 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/fonts/AdobeVFPrototype.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    75348 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/fonts/BungeeColor-Regular_colr_Windows.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   235924 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/fonts/BungeeOutline-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-29 17:38:13.000000 ManimPango-1.0.0a1/tests/fonts/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  5856032 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/fonts/MaShanZheng-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/svg_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_font_desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_fonts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_list_fonts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_valid_svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-29 17:38:14.000000 ManimPango-1.0.0a1/tests/test_version.py
```

### Comparing `ManimPango-0.4.3/LICENSE` & `ManimPango-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/ManimPango.egg-info/PKG-INFO` & `ManimPango-1.0.0a1/ManimPango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ManimPango
-Version: 0.4.3
+Version: 1.0.0a1
 Summary: Bindings for Pango for using with Manim.
 Home-page: https://manimpango.manim.community/
 Author: Naveen M K
 Author-email: naveen@manim.community
 Maintainer: The Manim Community Developers
 License: MIT
 Project-URL: Documentation, https://manimpango.manim.community/
@@ -202,9 +202,9 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Cython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ManimPango Version: 0.4.3 Summary: Bindings for
+Metadata-Version: 2.1 Name: ManimPango Version: 1.0.0a1 Summary: Bindings for
 Pango for using with Manim. Home-page: https://manimpango.manim.community/
 Author: Naveen M K Author-email: naveen@manim.community Maintainer: The Manim
 Community Developers License: MIT Project-URL: Documentation, https://
 manimpango.manim.community/ Project-URL: Source, https://github.com/
 ManimCommunity/manimpango Project-URL: Release notes, https://github.com/
 ManimCommunity/ManimPango/releases/ Description: # ManimPango
 [PyPI_Latest_Release] [PyPI_-_Wheel] [PyPI_-_Downloads] [PyPI_-_License] [PyPI
@@ -93,8 +93,8 @@
 Platform: Linux Platform: macOS Platform: Windows Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Cython Requires-Python: >=3.7 Description-Content-Type: text/markdown
+:: Cython Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `ManimPango-0.4.3/PKG-INFO` & `ManimPango-1.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ManimPango
-Version: 0.4.3
+Version: 1.0.0a1
 Summary: Bindings for Pango for using with Manim.
 Home-page: https://manimpango.manim.community/
 Author: Naveen M K
 Author-email: naveen@manim.community
 Maintainer: The Manim Community Developers
 License: MIT
 Project-URL: Documentation, https://manimpango.manim.community/
@@ -202,9 +202,9 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Cython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ManimPango Version: 0.4.3 Summary: Bindings for
+Metadata-Version: 2.1 Name: ManimPango Version: 1.0.0a1 Summary: Bindings for
 Pango for using with Manim. Home-page: https://manimpango.manim.community/
 Author: Naveen M K Author-email: naveen@manim.community Maintainer: The Manim
 Community Developers License: MIT Project-URL: Documentation, https://
 manimpango.manim.community/ Project-URL: Source, https://github.com/
 ManimCommunity/manimpango Project-URL: Release notes, https://github.com/
 ManimCommunity/ManimPango/releases/ Description: # ManimPango
 [PyPI_Latest_Release] [PyPI_-_Wheel] [PyPI_-_Downloads] [PyPI_-_License] [PyPI
@@ -93,8 +93,8 @@
 Platform: Linux Platform: macOS Platform: Windows Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Cython Requires-Python: >=3.7 Description-Content-Type: text/markdown
+:: Cython Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `ManimPango-0.4.3/README.md` & `ManimPango-1.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/docs/RELEASE.rst` & `ManimPango-1.0.0a1/docs/RELEASE.rst`

 * *Files 9% similar despite different names*

```diff
@@ -14,17 +14,23 @@
 3. Check whether the `Wheels Build`_,
    against the main branch works as expected.
 
 4. Clone the repository locally.
 
 5. Bump the version in `manimpango/_version`_ accordingly.
 
-6. Make a commit with the changes done, as ``Release v<version here>``
+6. Generate the changelog using `towncrier <https://pypi.org/project/towncrier/>`_.
 
-7. Create a tag, locally with
+.. code-block:: sh
+
+   towncrier
+
+7. Make a commit with the changes done, as ``Release v<version here>``
+
+8. Create a tag, locally with
 
 .. code-block:: sh
 
    git tag -s v<version-number>
 
 .. note::
 
@@ -35,29 +41,29 @@
 .. important::
 
     The message should include the changelog of the release.
     There is a github actions which will creates a draft `release`_
     with the changelog. You can edit them and copy it to the tag you
     create.
 
-8. Push the tag to remote.
+9. Push the tag to remote.
 
-9. Go to `Github`_, and `draft a new release`_ with the same tag pushed.
-   You can copy the same changelog you copied when you created the tag.
+10. Go to `Github`_, and `draft a new release`_ with the same tag pushed.
+    You can copy the same changelog you copied when you created the tag.
 
 .. important::
 
    You should actually "draft a new release" instead of just publishing
    a previously present draft release created by the Github Action. This is
    important so that the wheels build workflow triggers.
 
-10. Check whether the CI uploads the wheels and the ``.tar.gz`` file to
+11. Check whether the CI uploads the wheels and the ``.tar.gz`` file to
     PyPi.
 
-11. Finally, test the ``.tar.gz`` which was uploaded to `PyPi`_, and install
+12. Finally, test the ``.tar.gz`` which was uploaded to `PyPi`_, and install
     it in a new virtual environment.
 
 .. _Wheels Build: https://github.com/ManimCommunity/ManimPango/actions?query=workflow%3A%22Build+Wheels%22
 .. _manimpango/_version: https://github.com/ManimCommunity/ManimPango/blob/main/manimpango/_version.py
 .. _Github: https://github.com
 .. _draft a new release: https://docs.github.com/en/free-pro-team@latest/github/administering-a-repository/managing-releases-in-a-repository#creating-a-release
 .. _PyPi: https://pypi.org/project/manimpango/
```

### Comparing `ManimPango-0.4.3/docs/_static/favicon.ico` & `ManimPango-1.0.0a1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/docs/_templates/autosummary/module.rst` & `ManimPango-1.0.0a1/docs/_templates/autosummary/module.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{{ fullname | escape | underline }}
+{{ name | escape | underline }}
 
 .. currentmodule:: {{ fullname }}
 
 .. automodule:: {{ fullname }}
 
    {% block attributes %}
    {% if attributes %}
@@ -44,7 +44,20 @@
 
    .. autosummary::
    {% for item in exceptions %}
       {{ item }}
    {%- endfor %}
    {% endif %}
    {% endblock %}
+
+{% block modules %}
+{% if modules %}
+.. rubric:: Modules
+
+.. autosummary::
+   :toctree:
+   :recursive:
+{% for item in modules %}
+   {{ item }}
+{%- endfor %}
+{% endif %}
+{% endblock %}
```

### Comparing `ManimPango-0.4.3/docs/conf.py` & `ManimPango-1.0.0a1/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath(".."))
 
-
 from pathlib import Path
 
+import manimpango
+
 # -- Project information -----------------------------------------------------
-from pkg_resources import get_distribution
 
 project = "ManimPango"
-copyright = "2021, The Manim Community Dev Team"
+copyright = "2021-2023, The Manim Community Dev Team"
 author = "The Manim Community Dev Team"
 
-release = get_distribution("ManimPango").version
+release = manimpango.__version__
 version = ".".join(release.split(".")[:2])
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -54,15 +54,15 @@
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "furo"
+html_theme = "alabaster"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 html_favicon = str(Path("_static/favicon.ico"))
 autosummary_generate = True
@@ -72,14 +72,16 @@
 autoclass_content = "both"
 
 # controls whether functions documented by the autofunction directive
 # appear with their full module names
 add_module_names = False
 
 intersphinx_mapping = {
-    "manim": ("https://docs.manim.community/en/v0.2.0", None),
+    "manim": ("https://docs.manim.community/en/stable", None),
     "python": ("https://docs.python.org/3", None),
 }
 
-ogp_image = "https://www.manim.community/logo.png"
-ogp_site_name = "Manim Pango | Documentation"
+ogp_site_name = "ManimPango | Documentation"
 ogp_site_url = "https://manimpango.manim.community/"
+ogp_social_cards = {
+    "image": "_static/logo.png",
+}
```

### Comparing `ManimPango-0.4.3/docs/make.bat` & `ManimPango-1.0.0a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/manimpango/__init__.py` & `ManimPango-1.0.0a1/manimpango/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # -*- coding: utf-8 -*-
-import os
 import sys
 
+from . import _distributor_init  # noqa: F401
 from ._version import __version__  # noqa: F403,F401
 
-if os.name == "nt":  # pragma: no cover
-    os.environ["PATH"] = (
-        f"{os.path.abspath(os.path.dirname(__file__))}"
-        f"{os.pathsep}"
-        f"{os.environ['PATH']}"
-    )
 try:
+    from .attributes import *  # noqa: F403,F401
     from .cmanimpango import *  # noqa: F403,F401
     from .enums import *  # noqa: F403,F401
+    from .fonts import *  # noqa: F403,F401
+    from .layout import *  # noqa: F403,F401
     from .register_font import *  # noqa: F403,F401
+    from .renderer import *  # noqa: F403,F401
 except ImportError as ie:  # pragma: no cover
     py_ver = ".".join(map(str, sys.version_info[:3]))
     msg = f"""
 
 ManimPango could not import and load the necessary shared libraries.
 This error may occur when ManimPango and its dependencies are improperly set up.
 Please make sure the following versions are what you expect:
```

### Comparing `ManimPango-0.4.3/manimpango/cmanimpango.pyx` & `ManimPango-1.0.0a1/manimpango/cmanimpango.pyx`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/manimpango/enums.pyx` & `ManimPango-1.0.0a1/manimpango/enums.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -90,24 +90,15 @@
     SMALL_CAPS :
         A font with the lower case characters replaced by smaller variants
         of the capital characters.
     """
     NORMAL = PANGO_VARIANT_NORMAL
     SMALL_CAPS = PANGO_VARIANT_SMALL_CAPS
 
+
 class Alignment(Enum):
     """
     An enumeration specifying alignment.
-
-    Attributes
-    ----------
-
-    NORMAL :
-        A normal font.
-
-    SMALL_CAPS :
-        A font with the lower case characters replaced by smaller variants
-        of the capital characters.
     """
     LEFT = PANGO_ALIGN_LEFT
     CENTER = PANGO_ALIGN_CENTER
     RIGHT = PANGO_ALIGN_RIGHT
```

### Comparing `ManimPango-0.4.3/manimpango/pango.pxd` & `ManimPango-1.0.0a1/manimpango/include/pango.pxd`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from cairo cimport *
 from glib cimport *
+from pango_attributes cimport *
 
 
 cdef extern from "pango/pangocairo.h":
     int PANGO_SCALE
     int pango_units_from_double(double d)
     double pango_units_to_double (int i)
     ctypedef struct PangoLayout:
@@ -12,14 +13,19 @@
         pass
     ctypedef struct PangoFontMap:
         pass
     ctypedef struct PangoFontDescription:
         pass
     ctypedef struct PangoFontFamily:
         pass
+    ctypedef struct PangoRectangle:
+        int x
+        int y
+        int width
+        int height
     ctypedef enum PangoStyle:
         PANGO_STYLE_NORMAL
         PANGO_STYLE_OBLIQUE
         PANGO_STYLE_ITALIC
     ctypedef enum PangoWeight:
         PANGO_WEIGHT_THIN
         PANGO_WEIGHT_ULTRALIGHT
@@ -39,28 +45,36 @@
         PANGO_WRAP_WORD
         PANGO_WRAP_CHAR
         PANGO_WRAP_WORD_CHAR
     ctypedef enum PangoAlignment:
         PANGO_ALIGN_LEFT
         PANGO_ALIGN_CENTER
         PANGO_ALIGN_RIGHT
+    ctypedef struct PangoColor:
+        guint16 red
+        guint16 green
+        guint16 blue
     PangoLayout* pango_cairo_create_layout(cairo_t* cr)
     void pango_cairo_show_layout(
         cairo_t* cr,
         PangoLayout* layout
     )
     void pango_cairo_update_layout(
         cairo_t* cr,
         PangoLayout* layout
     )
     PangoFontDescription* pango_font_description_new()
     void pango_font_description_set_size(
         PangoFontDescription* desc,
         gint size
     )
+    void pango_font_description_set_absolute_size(
+        PangoFontDescription* desc,
+        double size
+    )
     void pango_font_description_set_family(
         PangoFontDescription* desc,
         const char* family
     )
     void pango_font_description_set_style(
         PangoFontDescription* desc,
         PangoStyle style
@@ -69,19 +83,52 @@
         PangoFontDescription* desc,
         PangoWeight weight
     )
     void pango_font_description_set_variant(
         PangoFontDescription* desc,
         PangoVariant variant
     )
+    char* pango_font_description_to_string(
+        const PangoFontDescription* desc
+    )
+    gboolean pango_font_description_equal(
+        const PangoFontDescription* desc1,
+        const PangoFontDescription* desc2
+    )
+    PangoFontDescription* pango_font_description_copy(
+        const PangoFontDescription* desc
+    )
+    const char* pango_font_description_get_family(
+        const PangoFontDescription* desc
+    )
+    gint pango_font_description_get_size(
+        const PangoFontDescription* desc
+    )
+    PangoStyle pango_font_description_get_style(
+        const PangoFontDescription* desc
+    )
+    PangoWeight pango_font_description_get_weight(
+        const PangoFontDescription* desc
+    )
+    PangoVariant pango_font_description_get_variant(
+        const PangoFontDescription* desc
+    )
+    PangoFontDescription* pango_font_description_from_string(
+        const char* str
+    )
+
 
     void pango_layout_set_width(
         PangoLayout* layout,
         int width
     )
+    void pango_layout_set_height(
+        PangoLayout* layout,
+        int height
+    )
     void pango_layout_set_font_description(
         PangoLayout* layout,
         const PangoFontDescription* desc
     )
     void pango_layout_set_text(
         PangoLayout* layout,
         const char* text,
@@ -135,14 +182,28 @@
         PangoLayout *layout,
         int indent
     )
     void pango_layout_set_alignment(
         PangoLayout *layout,
         PangoAlignment alignment
     )
+    void pango_layout_set_attributes (
+        PangoLayout* layout,
+        PangoAttrList* attrs
+    )
+    gboolean pango_color_parse(
+        PangoColor* color,
+        const char* spec
+    )
+    void pango_layout_get_pixel_extents (
+        PangoLayout* layout,
+        PangoRectangle* ink_rect,
+        PangoRectangle* logical_rect
+    )
+
 
 cdef extern from *:
     """
     #if PANGO_VERSION_CHECK(1,44,0)
         int set_line_width(PangoLayout *layout,float spacing)
         {
           pango_layout_set_line_spacing(layout, spacing);
```

### Comparing `ManimPango-0.4.3/manimpango/register_font.pxd` & `ManimPango-1.0.0a1/manimpango/register_font.pxd`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/manimpango/register_font.pyx` & `ManimPango-1.0.0a1/manimpango/register_font.pyx`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/manimpango/utils.py` & `ManimPango-1.0.0a1/manimpango/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 import re
 
-from .enums import Style, Weight
+from ..enums import Style, Weight
+
+__all__ = ["PangoUtils"]
 
 
 class PangoUtils:
     @staticmethod
     def str2style(string: str) -> Style:
         """Internally used function. Converts text to Pango Understandable Styles."""
         styles = {
```

### Comparing `ManimPango-0.4.3/setup.py` & `ManimPango-1.0.0a1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -185,22 +185,22 @@
     def setuptools_args(self):
         return update_dict(self.libs, self.cflags)
 
 
 def update_dict(dict1: dict, dict2: dict):
     for key in dict1:
         if key in dict2:
-            dict2[key] = dict1[key] + dict2[key]
+            dict2[key] = list(set(dict1[key] + dict2[key]))
         else:
             dict2[key] = dict1[key]
     return dict2
 
 
 ext = ".pyx" if USE_CYTHON else ".c"
-base_file = Path(__file__).parent / "manimpango"
+base_file = Path("manimpango/")
 _pkg_config_pangocairo = PKG_CONFIG("pangocairo")
 _pkg_config_fontconfig = PKG_CONFIG("pangofc")
 if _pkg_config_pangocairo.check_pkgconfig:
     _pkg_config_pangocairo.check_min_version(MINIMUM_PANGO_VERSION)
     returns = update_dict(
         _pkg_config_pangocairo.setuptools_args, _pkg_config_fontconfig.setuptools_args
     )
@@ -233,20 +233,50 @@
         **returns,
     ),
     Extension(
         "manimpango.register_font",
         [str(base_file / ("register_font" + ext))],
         **returns,
     ),
+    Extension(
+        "manimpango.utils._utils",
+        [str(base_file / "utils" / ("utils" + ext))],
+        **returns,
+    ),
+    Extension(
+        "manimpango.fonts._font_desc",
+        [str(base_file / "fonts" / ("_font_desc" + ext))],
+        **returns,
+    ),
+    Extension(
+        "manimpango.fonts.enums",
+        [str(base_file / "fonts" / ("enums" + ext))],
+        **returns,
+    ),
+    Extension(
+        "manimpango.layout._layout",
+        [str(base_file / "layout" / ("_layout" + ext))],
+        **returns,
+    ),
+    Extension(
+        "manimpango.renderer.svg_renderer",
+        [str(base_file / "renderer" / ("svg_renderer" + ext))],
+        **returns,
+    ),
+    Extension(
+        "manimpango.renderer.image_renderer",
+        [str(base_file / "renderer" / ("image_renderer" + ext))],
+        **returns,
+    ),
 ]
 if USE_CYTHON:
     ext_modules = cythonize(
         ext_modules,
         language_level=3,
-        include_path=["manimpango"],
+        include_path=["manimpango/include"],
         gdb_debug=DEBUG,
         compiler_directives={"linetrace": coverage},
     )
 with open("README.md") as fh:
     long_description = fh.read()
 
 setup(
@@ -256,16 +286,24 @@
     author_email="naveen@manim.community",
     maintainer="The Manim Community Developers",
     url="https://manimpango.manim.community/",
     description="Bindings for Pango for using with Manim.",
     long_description=long_description,
     zip_safe=False,
     long_description_content_type="text/markdown",
-    packages=["manimpango"],
-    python_requires=">=3.7",
+    include_package_data=True,
+    packages=[
+        "manimpango",
+        "manimpango.attributes",
+        "manimpango.utils",
+        "manimpango.layout",
+        "manimpango.fonts",
+        "manimpango.renderer",
+    ],
+    python_requires=">=3.8",
     platforms=["Linux", "macOS", "Windows"],
     keywords=["cython", "pango", "cairo", "manim"],
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
@@ -280,10 +318,10 @@
     project_urls={
         "Documentation": "https://manimpango.manim.community/",
         "Source": "https://github.com/ManimCommunity/manimpango",
         "Release notes": "https://github.com/ManimCommunity/ManimPango/releases/",
     },
     ext_modules=ext_modules,
     package_data={
-        "manimpango": ["*.pxd", "*.pyx"],
+        "manimpango": ["*.pxd", "*.pyx", "*.pyi"],
     },
 )
```

### Comparing `ManimPango-0.4.3/tests/__init__.py` & `ManimPango-1.0.0a1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/tests/_manim.py` & `ManimPango-1.0.0a1/tests/_manim.py`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/tests/conftest.py` & `ManimPango-1.0.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/tests/fonts/AdobeVFPrototype.ttf` & `ManimPango-1.0.0a1/tests/fonts/AdobeVFPrototype.ttf`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/tests/fonts/BungeeColor-Regular_colr_Windows.ttf` & `ManimPango-1.0.0a1/tests/fonts/BungeeColor-Regular_colr_Windows.ttf`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/tests/fonts/BungeeOutline-Regular.ttf` & `ManimPango-1.0.0a1/tests/fonts/BungeeOutline-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/tests/fonts/LICENSE.txt` & `ManimPango-1.0.0a1/tests/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/tests/fonts/MaShanZheng-Regular.ttf` & `ManimPango-1.0.0a1/tests/fonts/MaShanZheng-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/tests/svg_tester.py` & `ManimPango-1.0.0a1/tests/svg_tester.py`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/tests/test_colors.py` & `ManimPango-1.0.0a1/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/tests/test_fonts.py` & `ManimPango-1.0.0a1/tests/test_fonts.py`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/tests/test_list_fonts.py` & `ManimPango-1.0.0a1/tests/test_list_fonts.py`

 * *Files identical despite different names*

### Comparing `ManimPango-0.4.3/tests/test_markup.py` & `ManimPango-1.0.0a1/tests/test_markup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     "occaecat cupidatat non proident, sunt in culpa qui"
     "officia deserunt mollit anim id est laborum."
 )
 
 
 @pytest.mark.parametrize("text", ["foo", "<b>bar</b>", "வணக்கம்"])
 def test_good_markup(text):
-
     assert not manimpango.MarkupUtils.validate(
         text,
     ), f"{text} should not fail validation"
 
 
 @pytest.mark.parametrize("text", ["<b>foo", "<xyz>foo</xyz>"])
 def test_bad_markup(text):
```

### Comparing `ManimPango-0.4.3/tests/test_utils.py` & `ManimPango-1.0.0a1/tests/test_utils.py`

 * *Files identical despite different names*

