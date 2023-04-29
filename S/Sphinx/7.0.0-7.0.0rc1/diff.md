# Comparing `tmp/Sphinx-7.0.0.tar.gz` & `tmp/Sphinx-7.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sphinx-7.0.0.tar", last modified: Sat Apr 29 21:26:23 2023, max compression
+gzip compressed data, was "Sphinx-7.0.0rc1.tar", last modified: Fri Apr 28 11:33:50 2023, max compression
```

## Comparing `Sphinx-7.0.0.tar` & `Sphinx-7.0.0rc1.tar`

### file list

```diff
@@ -1,1601 +1,1601 @@
--rw-r--r--   0        0        0     3818 2023-04-28 21:49:43.726426 Sphinx-7.0.0/AUTHORS
--rw-r--r--   0        0        0   369614 2023-04-29 21:25:37.705825 Sphinx-7.0.0/CHANGES
--rw-r--r--   0        0        0     3530 2023-04-23 19:57:27.292374 Sphinx-7.0.0/CODE_OF_CONDUCT
--rw-r--r--   0        0        0    26647 2023-04-23 19:57:27.293375 Sphinx-7.0.0/EXAMPLES
--rw-r--r--   0        0        0     3135 2023-04-23 19:57:27.293375 Sphinx-7.0.0/LICENSE
--rw-r--r--   0        0        0     2654 2023-04-23 19:57:27.294379 Sphinx-7.0.0/README.rst
--rw-r--r--   0        0        0      607 2023-04-23 19:57:27.294379 Sphinx-7.0.0/doc/Makefile
--rw-r--r--   0        0        0      152 2023-04-23 19:57:27.294379 Sphinx-7.0.0/doc/_static/Makefile
--rw-r--r--   0        0        0    27523 2023-04-23 19:57:27.294379 Sphinx-7.0.0/doc/_static/bookcover.png
--rw-r--r--   0        0        0     9875 2023-04-23 19:57:27.295374 Sphinx-7.0.0/doc/_static/conf.py.txt
--rw-r--r--   0        0        0     3307 2023-04-23 19:57:27.295374 Sphinx-7.0.0/doc/_static/favicon.svg
--rw-r--r--   0        0        0     1351 2023-04-23 19:57:27.295374 Sphinx-7.0.0/doc/_static/more.png
--rw-r--r--   0        0        0    34213 2023-04-23 19:57:27.295374 Sphinx-7.0.0/doc/_static/sphinx.png
--rw-r--r--   0        0        0    25792 2023-04-23 19:57:27.296374 Sphinx-7.0.0/doc/_static/themes/agogo.png
--rw-r--r--   0        0        0    32356 2023-04-23 19:57:27.296374 Sphinx-7.0.0/doc/_static/themes/alabaster.png
--rw-r--r--   0        0        0    27139 2023-04-23 19:57:27.296374 Sphinx-7.0.0/doc/_static/themes/bizstyle.png
--rw-r--r--   0        0        0    39927 2023-04-23 19:57:27.297375 Sphinx-7.0.0/doc/_static/themes/classic.png
--rw-r--r--   0        0        0    56954 2023-04-23 19:57:27.297375 Sphinx-7.0.0/doc/_static/themes/fullsize/agogo.png
--rw-r--r--   0        0        0    40248 2023-04-23 19:57:27.297375 Sphinx-7.0.0/doc/_static/themes/fullsize/alabaster.png
--rw-r--r--   0        0        0    75192 2023-04-23 19:57:27.298374 Sphinx-7.0.0/doc/_static/themes/fullsize/bizstyle.png
--rw-r--r--   0        0        0    72597 2023-04-23 19:57:27.299374 Sphinx-7.0.0/doc/_static/themes/fullsize/classic.png
--rw-r--r--   0        0        0    84200 2023-04-23 19:57:27.299374 Sphinx-7.0.0/doc/_static/themes/fullsize/haiku.png
--rw-r--r--   0        0        0    32266 2023-04-23 19:57:27.300375 Sphinx-7.0.0/doc/_static/themes/fullsize/nature.png
--rw-r--r--   0        0        0   102717 2023-04-23 19:57:27.300375 Sphinx-7.0.0/doc/_static/themes/fullsize/pyramid.png
--rw-r--r--   0        0        0    88111 2023-04-23 19:57:27.301375 Sphinx-7.0.0/doc/_static/themes/fullsize/scrolls.png
--rw-r--r--   0        0        0    39411 2023-04-23 19:57:27.302374 Sphinx-7.0.0/doc/_static/themes/fullsize/sphinx_rtd_theme.png
--rw-r--r--   0        0        0    84439 2023-04-23 19:57:27.302374 Sphinx-7.0.0/doc/_static/themes/fullsize/sphinxdoc.png
--rw-r--r--   0        0        0    91744 2023-04-23 19:57:27.303374 Sphinx-7.0.0/doc/_static/themes/fullsize/traditional.png
--rw-r--r--   0        0        0    43184 2023-04-23 19:57:27.303374 Sphinx-7.0.0/doc/_static/themes/haiku.png
--rw-r--r--   0        0        0    28536 2023-04-23 19:57:27.303374 Sphinx-7.0.0/doc/_static/themes/nature.png
--rw-r--r--   0        0        0    38805 2023-04-23 19:57:27.304374 Sphinx-7.0.0/doc/_static/themes/pyramid.png
--rw-r--r--   0        0        0    27800 2023-04-23 19:57:27.304374 Sphinx-7.0.0/doc/_static/themes/scrolls.png
--rw-r--r--   0        0        0    29138 2023-04-23 19:57:27.304374 Sphinx-7.0.0/doc/_static/themes/sphinx_rtd_theme.png
--rw-r--r--   0        0        0    30225 2023-04-23 19:57:27.304374 Sphinx-7.0.0/doc/_static/themes/sphinxdoc.png
--rw-r--r--   0        0        0    32258 2023-04-23 19:57:27.305374 Sphinx-7.0.0/doc/_static/themes/traditional.png
--rw-r--r--   0        0        0    16371 2023-04-23 19:57:27.305374 Sphinx-7.0.0/doc/_static/translation.png
--rw-r--r--   0        0        0      342 2023-04-23 19:57:27.305374 Sphinx-7.0.0/doc/_static/translation.puml
--rw-r--r--   0        0        0     8232 2023-04-25 10:59:46.881271 Sphinx-7.0.0/doc/_static/translation.svg
--rw-r--r--   0        0        0    26500 2023-04-23 19:57:27.306374 Sphinx-7.0.0/doc/_static/tutorial/lumache-autosummary.png
--rw-r--r--   0        0        0    52126 2023-04-23 19:57:27.306374 Sphinx-7.0.0/doc/_static/tutorial/lumache-first-light.png
--rw-r--r--   0        0        0    51223 2023-04-23 19:57:27.307374 Sphinx-7.0.0/doc/_static/tutorial/lumache-furo.png
--rw-r--r--   0        0        0    71741 2023-04-23 19:57:27.308375 Sphinx-7.0.0/doc/_static/tutorial/lumache-py-function-full.png
--rw-r--r--   0        0        0    41828 2023-04-23 19:57:27.308375 Sphinx-7.0.0/doc/_static/tutorial/lumache-py-function.png
--rw-r--r--   0        0        0      225 2023-04-23 19:57:27.308375 Sphinx-7.0.0/doc/_templates/contents.html
--rw-r--r--   0        0        0     1968 2023-04-23 19:57:27.309374 Sphinx-7.0.0/doc/_themes/sphinx13/layout.html
--rw-r--r--   0        0        0     6552 2023-04-23 19:57:27.309374 Sphinx-7.0.0/doc/_themes/sphinx13/static/sphinx13.css
--rw-r--r--   0        0        0    11719 2023-04-23 19:57:27.309374 Sphinx-7.0.0/doc/_themes/sphinx13/static/sphinxheader.png
--rw-r--r--   0        0        0       60 2023-04-23 19:57:27.310374 Sphinx-7.0.0/doc/_themes/sphinx13/theme.conf
--rw-r--r--   0        0        0       98 2023-04-23 19:57:27.310374 Sphinx-7.0.0/doc/authors.rst
--rw-r--r--   0        0        0      400 2023-04-23 19:57:27.310374 Sphinx-7.0.0/doc/changes.rst
--rw-r--r--   0        0        0     9004 2023-04-27 00:31:27.920451 Sphinx-7.0.0/doc/conf.py
--rw-r--r--   0        0        0     1151 2023-04-23 19:57:27.311375 Sphinx-7.0.0/doc/development/builders.rst
--rw-r--r--   0        0        0      649 2023-04-23 19:57:27.311375 Sphinx-7.0.0/doc/development/index.rst
--rw-r--r--   0        0        0     1051 2023-04-23 19:57:27.311375 Sphinx-7.0.0/doc/development/overview.rst
--rw-r--r--   0        0        0    15048 2023-04-28 09:32:47.966025 Sphinx-7.0.0/doc/development/templating.rst
--rw-r--r--   0        0        0    12324 2023-04-23 19:57:27.312375 Sphinx-7.0.0/doc/development/theming.rst
--rw-r--r--   0        0        0     4020 2023-04-23 19:57:27.312375 Sphinx-7.0.0/doc/development/tutorials/autodoc_ext.rst
--rw-r--r--   0        0        0      438 2023-04-23 19:57:27.312375 Sphinx-7.0.0/doc/development/tutorials/examples/README.rst
--rw-r--r--   0        0        0     1802 2023-04-23 19:57:27.312375 Sphinx-7.0.0/doc/development/tutorials/examples/autodoc_intenum.py
--rw-r--r--   0        0        0      400 2023-04-23 19:57:27.312375 Sphinx-7.0.0/doc/development/tutorials/examples/helloworld.py
--rw-r--r--   0        0        0     5030 2023-04-23 19:57:27.313375 Sphinx-7.0.0/doc/development/tutorials/examples/recipe.py
--rw-r--r--   0        0        0     3942 2023-04-23 19:57:27.313375 Sphinx-7.0.0/doc/development/tutorials/examples/todo.py
--rw-r--r--   0        0        0     5289 2023-04-23 19:57:27.313375 Sphinx-7.0.0/doc/development/tutorials/helloworld.rst
--rw-r--r--   0        0        0      262 2023-04-23 19:57:27.313375 Sphinx-7.0.0/doc/development/tutorials/index.rst
--rw-r--r--   0        0        0     8216 2023-04-23 19:57:27.313375 Sphinx-7.0.0/doc/development/tutorials/recipe.rst
--rw-r--r--   0        0        0    13435 2023-04-23 19:57:27.313375 Sphinx-7.0.0/doc/development/tutorials/todo.rst
--rw-r--r--   0        0        0       54 2023-04-23 19:57:27.313375 Sphinx-7.0.0/doc/examples.rst
--rw-r--r--   0        0        0    14235 2023-04-23 19:57:27.314375 Sphinx-7.0.0/doc/extdev/appapi.rst
--rw-r--r--   0        0        0     1103 2023-04-23 19:57:27.314375 Sphinx-7.0.0/doc/extdev/builderapi.rst
--rw-r--r--   0        0        0      165 2023-04-23 19:57:27.314375 Sphinx-7.0.0/doc/extdev/collectorapi.rst
--rw-r--r--   0        0        0    40815 2023-04-27 00:31:27.920451 Sphinx-7.0.0/doc/extdev/deprecated.rst
--rw-r--r--   0        0        0      518 2023-04-23 19:57:27.315375 Sphinx-7.0.0/doc/extdev/domainapi.rst
--rw-r--r--   0        0        0     1043 2023-04-23 19:57:27.315375 Sphinx-7.0.0/doc/extdev/envapi.rst
--rw-r--r--   0        0        0     2817 2023-04-23 19:57:27.315375 Sphinx-7.0.0/doc/extdev/i18n.rst
--rw-r--r--   0        0        0     8597 2023-04-23 19:57:27.315375 Sphinx-7.0.0/doc/extdev/index.rst
--rw-r--r--   0        0        0     2384 2023-04-23 19:57:27.316375 Sphinx-7.0.0/doc/extdev/logging.rst
--rw-r--r--   0        0        0     4787 2023-04-23 19:57:27.316375 Sphinx-7.0.0/doc/extdev/markupapi.rst
--rw-r--r--   0        0        0     1563 2023-04-23 19:57:27.316375 Sphinx-7.0.0/doc/extdev/nodes.rst
--rw-r--r--   0        0        0     1243 2023-04-23 19:57:27.316375 Sphinx-7.0.0/doc/extdev/parserapi.rst
--rw-r--r--   0        0        0      114 2023-04-23 19:57:27.316375 Sphinx-7.0.0/doc/extdev/projectapi.rst
--rw-r--r--   0        0        0      943 2023-04-23 19:57:27.316375 Sphinx-7.0.0/doc/extdev/utils.rst
--rw-r--r--   0        0        0    13329 2023-04-23 19:57:27.316375 Sphinx-7.0.0/doc/faq.rst
--rw-r--r--   0        0        0     4173 2023-04-23 19:57:27.317375 Sphinx-7.0.0/doc/glossary.rst
--rw-r--r--   0        0        0     3539 2023-04-23 19:57:27.317375 Sphinx-7.0.0/doc/index.rst
--rw-r--r--   0        0        0       71 2023-04-23 19:57:27.317375 Sphinx-7.0.0/doc/internals/code-of-conduct.rst
--rw-r--r--   0        0        0    11482 2023-04-23 19:57:27.317375 Sphinx-7.0.0/doc/internals/contributing.rst
--rw-r--r--   0        0        0      353 2023-04-23 19:57:27.317375 Sphinx-7.0.0/doc/internals/index.rst
--rw-r--r--   0        0        0     1964 2023-04-23 19:57:27.317375 Sphinx-7.0.0/doc/internals/organization.rst
--rw-r--r--   0        0        0     4395 2023-04-23 19:57:27.318375 Sphinx-7.0.0/doc/internals/release-process.rst
--rw-r--r--   0        0        0    68725 2023-04-23 19:57:27.318375 Sphinx-7.0.0/doc/latex.rst
--rwxr-xr-x   0        0        0      784 2023-04-25 10:59:46.881271 Sphinx-7.0.0/doc/make.bat
--rw-r--r--   0        0        0      314 2023-04-23 19:57:27.319375 Sphinx-7.0.0/doc/man/index.rst
--rw-r--r--   0        0        0     4508 2023-04-23 19:57:27.319375 Sphinx-7.0.0/doc/man/sphinx-apidoc.rst
--rw-r--r--   0        0        0     2122 2023-04-23 19:57:27.319375 Sphinx-7.0.0/doc/man/sphinx-autogen.rst
--rw-r--r--   0        0        0    10497 2023-04-23 19:57:27.319375 Sphinx-7.0.0/doc/man/sphinx-build.rst
--rw-r--r--   0        0        0     3692 2023-04-23 19:57:27.319375 Sphinx-7.0.0/doc/man/sphinx-quickstart.rst
--rw-r--r--   0        0        0      806 2023-04-23 19:57:27.319375 Sphinx-7.0.0/doc/support.rst
--rw-r--r--   0        0        0     4981 2023-04-23 19:57:27.320375 Sphinx-7.0.0/doc/tutorial/automatic-doc-generation.rst
--rw-r--r--   0        0        0    11036 2023-04-23 19:57:27.320375 Sphinx-7.0.0/doc/tutorial/deploying.rst
--rw-r--r--   0        0        0     9134 2023-04-23 19:57:27.320375 Sphinx-7.0.0/doc/tutorial/describing-code.rst
--rw-r--r--   0        0        0      240 2023-04-23 19:57:27.320375 Sphinx-7.0.0/doc/tutorial/end.rst
--rw-r--r--   0        0        0     3450 2023-04-23 19:57:27.320375 Sphinx-7.0.0/doc/tutorial/first-steps.rst
--rw-r--r--   0        0        0     3723 2023-04-23 19:57:27.321380 Sphinx-7.0.0/doc/tutorial/getting-started.rst
--rw-r--r--   0        0        0     1433 2023-04-23 19:57:27.321380 Sphinx-7.0.0/doc/tutorial/index.rst
--rw-r--r--   0        0        0     2528 2023-04-23 19:57:27.321380 Sphinx-7.0.0/doc/tutorial/more-sphinx-customization.rst
--rw-r--r--   0        0        0     4177 2023-04-23 19:57:27.321380 Sphinx-7.0.0/doc/tutorial/narrative-documentation.rst
--rw-r--r--   0        0        0    11259 2023-04-23 19:57:27.322375 Sphinx-7.0.0/doc/usage/advanced/intl.rst
--rw-r--r--   0        0        0     2670 2023-04-23 19:57:27.322375 Sphinx-7.0.0/doc/usage/advanced/websupport/api.rst
--rw-r--r--   0        0        0      302 2023-04-23 19:57:27.322375 Sphinx-7.0.0/doc/usage/advanced/websupport/index.rst
--rw-r--r--   0        0        0     9640 2023-04-23 19:57:27.323375 Sphinx-7.0.0/doc/usage/advanced/websupport/quickstart.rst
--rw-r--r--   0        0        0     1368 2023-04-23 19:57:27.323375 Sphinx-7.0.0/doc/usage/advanced/websupport/searchadapters.rst
--rw-r--r--   0        0        0     1231 2023-04-23 19:57:27.323375 Sphinx-7.0.0/doc/usage/advanced/websupport/storagebackends.rst
--rw-r--r--   0        0        0    17742 2023-04-23 19:57:27.323375 Sphinx-7.0.0/doc/usage/builders/index.rst
--rw-r--r--   0        0        0    99806 2023-04-23 19:57:27.324375 Sphinx-7.0.0/doc/usage/configuration.rst
--rw-r--r--   0        0        0    29861 2023-04-23 19:57:27.324375 Sphinx-7.0.0/doc/usage/extensions/autodoc.rst
--rw-r--r--   0        0        0     1899 2023-04-23 19:57:27.325374 Sphinx-7.0.0/doc/usage/extensions/autosectionlabel.rst
--rw-r--r--   0        0        0    11098 2023-04-23 19:57:27.325374 Sphinx-7.0.0/doc/usage/extensions/autosummary.rst
--rw-r--r--   0        0        0     1584 2023-04-23 19:57:27.325374 Sphinx-7.0.0/doc/usage/extensions/coverage.rst
--rw-r--r--   0        0        0    11838 2023-04-23 19:57:27.325374 Sphinx-7.0.0/doc/usage/extensions/doctest.rst
--rw-r--r--   0        0        0      404 2023-04-23 19:57:27.325374 Sphinx-7.0.0/doc/usage/extensions/duration.rst
--rw-r--r--   0        0        0     9665 2023-04-23 19:57:27.326376 Sphinx-7.0.0/doc/usage/extensions/example_google.py
--rw-r--r--   0        0        0      296 2023-04-23 19:57:27.326376 Sphinx-7.0.0/doc/usage/extensions/example_google.rst
--rw-r--r--   0        0        0     9714 2023-04-23 19:57:27.326376 Sphinx-7.0.0/doc/usage/extensions/example_numpy.py
--rw-r--r--   0        0        0      292 2023-04-23 19:57:27.326376 Sphinx-7.0.0/doc/usage/extensions/example_numpy.rst
--rw-r--r--   0        0        0     2781 2023-04-23 19:57:27.326376 Sphinx-7.0.0/doc/usage/extensions/extlinks.rst
--rw-r--r--   0        0        0      491 2023-04-23 19:57:27.326376 Sphinx-7.0.0/doc/usage/extensions/githubpages.rst
--rw-r--r--   0        0        0     6292 2023-04-23 19:57:27.327375 Sphinx-7.0.0/doc/usage/extensions/graphviz.rst
--rw-r--r--   0        0        0     1329 2023-04-23 19:57:27.327375 Sphinx-7.0.0/doc/usage/extensions/ifconfig.rst
--rw-r--r--   0        0        0     1705 2023-04-23 19:57:27.327375 Sphinx-7.0.0/doc/usage/extensions/imgconverter.rst
--rw-r--r--   0        0        0     2410 2023-04-23 19:57:27.327375 Sphinx-7.0.0/doc/usage/extensions/index.rst
--rw-r--r--   0        0        0     5594 2023-04-23 19:57:27.327375 Sphinx-7.0.0/doc/usage/extensions/inheritance.rst
--rw-r--r--   0        0        0     9934 2023-04-23 19:57:27.328374 Sphinx-7.0.0/doc/usage/extensions/intersphinx.rst
--rw-r--r--   0        0        0     1756 2023-04-23 19:57:27.328374 Sphinx-7.0.0/doc/usage/extensions/linkcode.rst
--rw-r--r--   0        0        0    11756 2023-04-23 19:57:27.328374 Sphinx-7.0.0/doc/usage/extensions/math.rst
--rw-r--r--   0        0        0    15980 2023-04-23 19:57:27.328374 Sphinx-7.0.0/doc/usage/extensions/napoleon.rst
--rw-r--r--   0        0        0     1644 2023-04-23 19:57:27.328374 Sphinx-7.0.0/doc/usage/extensions/todo.rst
--rw-r--r--   0        0        0     3748 2023-04-23 19:57:27.328374 Sphinx-7.0.0/doc/usage/extensions/viewcode.rst
--rw-r--r--   0        0        0      537 2023-04-27 00:31:27.920451 Sphinx-7.0.0/doc/usage/index.rst
--rw-r--r--   0        0        0     7146 2023-04-23 19:57:27.329374 Sphinx-7.0.0/doc/usage/installation.rst
--rw-r--r--   0        0        0     1584 2023-04-23 19:57:27.329374 Sphinx-7.0.0/doc/usage/markdown.rst
--rw-r--r--   0        0        0    13150 2023-04-27 00:31:27.920451 Sphinx-7.0.0/doc/usage/quickstart.rst
--rw-r--r--   0        0        0    20508 2023-04-23 19:57:27.330375 Sphinx-7.0.0/doc/usage/restructuredtext/basics.rst
--rw-r--r--   0        0        0    45004 2023-04-23 19:57:27.330375 Sphinx-7.0.0/doc/usage/restructuredtext/directives.rst
--rw-r--r--   0        0        0    62364 2023-04-23 19:57:27.330375 Sphinx-7.0.0/doc/usage/restructuredtext/domains.rst
--rw-r--r--   0        0        0     1967 2023-04-23 19:57:27.331375 Sphinx-7.0.0/doc/usage/restructuredtext/field-lists.rst
--rw-r--r--   0        0        0      574 2023-04-23 19:57:27.331375 Sphinx-7.0.0/doc/usage/restructuredtext/index.rst
--rw-r--r--   0        0        0    18187 2023-04-23 19:57:27.331375 Sphinx-7.0.0/doc/usage/restructuredtext/roles.rst
--rw-r--r--   0        0        0    14326 2023-04-23 19:57:27.331375 Sphinx-7.0.0/doc/usage/theming.rst
--rw-r--r--   0        0        0    12593 2023-04-27 00:31:27.920451 Sphinx-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     1829 2023-04-29 21:25:37.705825 Sphinx-7.0.0/sphinx/__init__.py
--rw-r--r--   0        0        0      103 2023-04-23 19:57:27.333374 Sphinx-7.0.0/sphinx/__main__.py
--rw-r--r--   0        0        0    17579 2023-04-23 19:57:27.334375 Sphinx-7.0.0/sphinx/addnodes.py
--rw-r--r--   0        0        0    55683 2023-04-29 20:33:06.374738 Sphinx-7.0.0/sphinx/application.py
--rw-r--r--   0        0        0    26838 2023-04-28 09:26:30.898486 Sphinx-7.0.0/sphinx/builders/__init__.py
--rw-r--r--   0        0        0    28999 2023-04-23 19:57:27.335380 Sphinx-7.0.0/sphinx/builders/_epub_base.py
--rw-r--r--   0        0        0     6474 2023-04-23 19:57:27.335380 Sphinx-7.0.0/sphinx/builders/changes.py
--rw-r--r--   0        0        0     1504 2023-04-23 19:57:27.335380 Sphinx-7.0.0/sphinx/builders/dirhtml.py
--rw-r--r--   0        0        0      982 2023-04-23 19:57:27.335380 Sphinx-7.0.0/sphinx/builders/dummy.py
--rw-r--r--   0        0        0    11284 2023-04-23 19:57:27.336375 Sphinx-7.0.0/sphinx/builders/epub3.py
--rw-r--r--   0        0        0    11407 2023-04-23 19:57:27.336375 Sphinx-7.0.0/sphinx/builders/gettext.py
--rw-r--r--   0        0        0    58281 2023-04-28 10:59:56.013366 Sphinx-7.0.0/sphinx/builders/html/__init__.py
--rw-r--r--   0        0        0     2525 2023-04-23 19:57:27.337375 Sphinx-7.0.0/sphinx/builders/html/transforms.py
--rw-r--r--   0        0        0    24143 2023-04-23 19:57:27.338035 Sphinx-7.0.0/sphinx/builders/latex/__init__.py
--rw-r--r--   0        0        0     7365 2023-04-23 19:57:27.338035 Sphinx-7.0.0/sphinx/builders/latex/constants.py
--rw-r--r--   0        0        0      866 2023-04-23 19:57:27.338035 Sphinx-7.0.0/sphinx/builders/latex/nodes.py
--rw-r--r--   0        0        0     4445 2023-04-23 19:57:27.338035 Sphinx-7.0.0/sphinx/builders/latex/theming.py
--rw-r--r--   0        0        0    20998 2023-04-23 19:57:27.338961 Sphinx-7.0.0/sphinx/builders/latex/transforms.py
--rw-r--r--   0        0        0     1703 2023-04-23 19:57:27.338961 Sphinx-7.0.0/sphinx/builders/latex/util.py
--rw-r--r--   0        0        0    23404 2023-04-23 19:57:27.338961 Sphinx-7.0.0/sphinx/builders/linkcheck.py
--rw-r--r--   0        0        0     4511 2023-04-23 19:57:27.338961 Sphinx-7.0.0/sphinx/builders/manpage.py
--rw-r--r--   0        0        0     7425 2023-04-23 19:57:27.338961 Sphinx-7.0.0/sphinx/builders/singlehtml.py
--rw-r--r--   0        0        0     9634 2023-04-23 19:57:27.339975 Sphinx-7.0.0/sphinx/builders/texinfo.py
--rw-r--r--   0        0        0     2870 2023-04-23 19:57:27.339975 Sphinx-7.0.0/sphinx/builders/text.py
--rw-r--r--   0        0        0     3726 2023-04-23 19:57:27.339975 Sphinx-7.0.0/sphinx/builders/xml.py
--rw-r--r--   0        0        0       44 2023-04-23 19:57:27.339975 Sphinx-7.0.0/sphinx/cmd/__init__.py
--rw-r--r--   0        0        0    13411 2023-04-23 19:57:27.339975 Sphinx-7.0.0/sphinx/cmd/build.py
--rw-r--r--   0        0        0     6552 2023-04-23 19:57:27.340974 Sphinx-7.0.0/sphinx/cmd/make_mode.py
--rw-r--r--   0        0        0    23835 2023-04-23 19:57:27.340974 Sphinx-7.0.0/sphinx/cmd/quickstart.py
--rw-r--r--   0        0        0    21519 2023-04-26 16:05:03.832456 Sphinx-7.0.0/sphinx/config.py
--rw-r--r--   0        0        0     1816 2023-04-28 11:10:33.021919 Sphinx-7.0.0/sphinx/deprecation.py
--rw-r--r--   0        0        0    13518 2023-04-23 19:57:27.341975 Sphinx-7.0.0/sphinx/directives/__init__.py
--rw-r--r--   0        0        0    18354 2023-04-23 19:57:27.341975 Sphinx-7.0.0/sphinx/directives/code.py
--rw-r--r--   0        0        0    14672 2023-04-23 19:57:27.341975 Sphinx-7.0.0/sphinx/directives/other.py
--rw-r--r--   0        0        0     6781 2023-04-23 19:57:27.342974 Sphinx-7.0.0/sphinx/directives/patches.py
--rw-r--r--   0        0        0    15320 2023-04-23 19:57:27.342974 Sphinx-7.0.0/sphinx/domains/__init__.py
--rw-r--r--   0        0        0   150745 2023-04-27 00:29:16.230978 Sphinx-7.0.0/sphinx/domains/c.py
--rw-r--r--   0        0        0     5524 2023-04-23 19:57:27.343975 Sphinx-7.0.0/sphinx/domains/changeset.py
--rw-r--r--   0        0        0     5676 2023-04-23 19:57:27.343975 Sphinx-7.0.0/sphinx/domains/citation.py
--rw-r--r--   0        0        0   329631 2023-04-23 19:57:27.344974 Sphinx-7.0.0/sphinx/domains/cpp.py
--rw-r--r--   0        0        0     4086 2023-04-23 19:57:27.344974 Sphinx-7.0.0/sphinx/domains/index.py
--rw-r--r--   0        0        0    18294 2023-04-27 00:29:16.230978 Sphinx-7.0.0/sphinx/domains/javascript.py
--rw-r--r--   0        0        0     5459 2023-04-23 19:57:27.345974 Sphinx-7.0.0/sphinx/domains/math.py
--rw-r--r--   0        0        0    59777 2023-04-27 00:29:16.230978 Sphinx-7.0.0/sphinx/domains/python.py
--rw-r--r--   0        0        0    10292 2023-04-27 00:29:16.230978 Sphinx-7.0.0/sphinx/domains/rst.py
--rw-r--r--   0        0        0    45842 2023-04-27 00:29:16.230978 Sphinx-7.0.0/sphinx/domains/std.py
--rw-r--r--   0        0        0    29692 2023-04-23 19:57:27.347974 Sphinx-7.0.0/sphinx/environment/__init__.py
--rw-r--r--   0        0        0       34 2023-04-23 19:57:27.347974 Sphinx-7.0.0/sphinx/environment/adapters/__init__.py
--rw-r--r--   0        0        0      418 2023-04-23 19:57:27.347974 Sphinx-7.0.0/sphinx/environment/adapters/asset.py
--rw-r--r--   0        0        0     7509 2023-04-23 19:57:27.347974 Sphinx-7.0.0/sphinx/environment/adapters/indexentries.py
--rw-r--r--   0        0        0    16449 2023-04-23 19:57:27.348974 Sphinx-7.0.0/sphinx/environment/adapters/toctree.py
--rw-r--r--   0        0        0     2784 2023-04-23 19:57:27.348974 Sphinx-7.0.0/sphinx/environment/collectors/__init__.py
--rw-r--r--   0        0        0     6161 2023-04-23 19:57:27.348974 Sphinx-7.0.0/sphinx/environment/collectors/asset.py
--rw-r--r--   0        0        0     1887 2023-04-23 19:57:27.348974 Sphinx-7.0.0/sphinx/environment/collectors/dependencies.py
--rw-r--r--   0        0        0     2609 2023-04-23 19:57:27.349974 Sphinx-7.0.0/sphinx/environment/collectors/metadata.py
--rw-r--r--   0        0        0     2144 2023-04-23 19:57:27.349974 Sphinx-7.0.0/sphinx/environment/collectors/title.py
--rw-r--r--   0        0        0    15869 2023-04-23 19:57:27.349974 Sphinx-7.0.0/sphinx/environment/collectors/toctree.py
--rw-r--r--   0        0        0     3388 2023-04-23 19:57:27.349974 Sphinx-7.0.0/sphinx/errors.py
--rw-r--r--   0        0        0     4230 2023-04-23 19:57:27.349974 Sphinx-7.0.0/sphinx/events.py
--rw-r--r--   0        0        0       57 2023-04-23 19:57:27.349974 Sphinx-7.0.0/sphinx/ext/__init__.py
--rw-r--r--   0        0        0    19197 2023-04-23 19:57:27.350974 Sphinx-7.0.0/sphinx/ext/apidoc.py
--rw-r--r--   0        0        0   114236 2023-04-23 19:57:27.350974 Sphinx-7.0.0/sphinx/ext/autodoc/__init__.py
--rw-r--r--   0        0        0     5925 2023-04-23 19:57:27.351975 Sphinx-7.0.0/sphinx/ext/autodoc/directive.py
--rw-r--r--   0        0        0    11371 2023-04-23 19:57:27.351975 Sphinx-7.0.0/sphinx/ext/autodoc/importer.py
--rw-r--r--   0        0        0     5900 2023-04-23 19:57:27.351975 Sphinx-7.0.0/sphinx/ext/autodoc/mock.py
--rw-r--r--   0        0        0     4588 2023-04-23 19:57:27.351975 Sphinx-7.0.0/sphinx/ext/autodoc/preserve_defaults.py
--rw-r--r--   0        0        0     5292 2023-04-23 19:57:27.351975 Sphinx-7.0.0/sphinx/ext/autodoc/type_comment.py
--rw-r--r--   0        0        0     7789 2023-04-23 19:57:27.352974 Sphinx-7.0.0/sphinx/ext/autodoc/typehints.py
--rw-r--r--   0        0        0     2292 2023-04-23 19:57:27.352974 Sphinx-7.0.0/sphinx/ext/autosectionlabel.py
--rw-r--r--   0        0        0    31056 2023-04-28 09:21:04.216236 Sphinx-7.0.0/sphinx/ext/autosummary/__init__.py
--rw-r--r--   0        0        0    26212 2023-04-23 19:57:27.353975 Sphinx-7.0.0/sphinx/ext/autosummary/generate.py
--rw-r--r--   0        0        0      106 2023-04-23 19:57:27.353975 Sphinx-7.0.0/sphinx/ext/autosummary/templates/autosummary/base.rst
--rw-r--r--   0        0        0      553 2023-04-23 19:57:27.353975 Sphinx-7.0.0/sphinx/ext/autosummary/templates/autosummary/class.rst
--rw-r--r--   0        0        0     1071 2023-04-23 19:57:27.353975 Sphinx-7.0.0/sphinx/ext/autosummary/templates/autosummary/module.rst
--rw-r--r--   0        0        0    14065 2023-04-23 19:57:27.354974 Sphinx-7.0.0/sphinx/ext/coverage.py
--rw-r--r--   0        0        0    22423 2023-04-23 19:57:27.354974 Sphinx-7.0.0/sphinx/ext/doctest.py
--rw-r--r--   0        0        0     2887 2023-04-23 19:57:27.354974 Sphinx-7.0.0/sphinx/ext/duration.py
--rw-r--r--   0        0        0     4523 2023-04-23 19:57:27.354974 Sphinx-7.0.0/sphinx/ext/extlinks.py
--rw-r--r--   0        0        0     1962 2023-04-23 19:57:27.355975 Sphinx-7.0.0/sphinx/ext/githubpages.py
--rw-r--r--   0        0        0    15864 2023-04-23 19:57:27.355975 Sphinx-7.0.0/sphinx/ext/graphviz.py
--rw-r--r--   0        0        0     2517 2023-04-23 19:57:27.355975 Sphinx-7.0.0/sphinx/ext/ifconfig.py
--rw-r--r--   0        0        0     3582 2023-04-23 19:57:27.355975 Sphinx-7.0.0/sphinx/ext/imgconverter.py
--rw-r--r--   0        0        0    15117 2023-04-23 19:57:27.355975 Sphinx-7.0.0/sphinx/ext/imgmath.py
--rw-r--r--   0        0        0    17031 2023-04-23 19:57:27.356974 Sphinx-7.0.0/sphinx/ext/inheritance_diagram.py
--rw-r--r--   0        0        0    28440 2023-04-27 00:29:16.230978 Sphinx-7.0.0/sphinx/ext/intersphinx.py
--rw-r--r--   0        0        0     2203 2023-04-23 19:57:27.356974 Sphinx-7.0.0/sphinx/ext/linkcode.py
--rw-r--r--   0        0        0     5182 2023-04-23 19:57:27.356974 Sphinx-7.0.0/sphinx/ext/mathjax.py
--rw-r--r--   0        0        0    17936 2023-04-23 19:57:27.357974 Sphinx-7.0.0/sphinx/ext/napoleon/__init__.py
--rw-r--r--   0        0        0    48417 2023-04-23 19:57:27.357974 Sphinx-7.0.0/sphinx/ext/napoleon/docstring.py
--rw-r--r--   0        0        0     8017 2023-04-23 19:57:27.357974 Sphinx-7.0.0/sphinx/ext/todo.py
--rw-r--r--   0        0        0    12900 2023-04-23 19:57:27.358974 Sphinx-7.0.0/sphinx/ext/viewcode.py
--rw-r--r--   0        0        0     2995 2023-04-23 19:57:27.358974 Sphinx-7.0.0/sphinx/extension.py
--rw-r--r--   0        0        0     6986 2023-04-23 19:57:27.358974 Sphinx-7.0.0/sphinx/highlighting.py
--rw-r--r--   0        0        0     6190 2023-04-27 15:02:05.988638 Sphinx-7.0.0/sphinx/io.py
--rw-r--r--   0        0        0     7107 2023-04-23 19:57:27.358974 Sphinx-7.0.0/sphinx/jinja2glue.py
--rw-r--r--   0        0        0      165 2023-04-25 10:59:46.881271 Sphinx-7.0.0/sphinx/locale/.tx/config
--rw-r--r--   0        0        0     7316 2023-04-23 19:57:27.359974 Sphinx-7.0.0/sphinx/locale/__init__.py
--rw-r--r--   0        0        0     3735 2023-04-23 19:57:27.359974 Sphinx-7.0.0/sphinx/locale/ar/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     7947 2023-04-23 19:57:27.360974 Sphinx-7.0.0/sphinx/locale/ar/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    87617 2023-04-23 19:57:27.361975 Sphinx-7.0.0/sphinx/locale/ar/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2361 2023-04-23 19:57:27.362172 Sphinx-7.0.0/sphinx/locale/bg/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      492 2023-04-23 19:57:27.362172 Sphinx-7.0.0/sphinx/locale/bg/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84994 2023-04-23 19:57:27.362172 Sphinx-7.0.0/sphinx/locale/bg/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     6038 2023-04-23 19:57:27.363207 Sphinx-7.0.0/sphinx/locale/bn/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     7976 2023-04-23 19:57:27.363207 Sphinx-7.0.0/sphinx/locale/bn/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    89077 2023-04-23 19:57:27.364207 Sphinx-7.0.0/sphinx/locale/bn/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3259 2023-04-23 19:57:27.364207 Sphinx-7.0.0/sphinx/locale/ca/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     5587 2023-04-23 19:57:27.364207 Sphinx-7.0.0/sphinx/locale/ca/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86709 2023-04-23 19:57:27.364207 Sphinx-7.0.0/sphinx/locale/ca/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2446 2023-04-23 19:57:27.365207 Sphinx-7.0.0/sphinx/locale/cak/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     2424 2023-04-23 19:57:27.365207 Sphinx-7.0.0/sphinx/locale/cak/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85717 2023-04-23 19:57:27.365207 Sphinx-7.0.0/sphinx/locale/cak/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4037 2023-04-23 19:57:27.366207 Sphinx-7.0.0/sphinx/locale/cs/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     8265 2023-04-23 19:57:27.366207 Sphinx-7.0.0/sphinx/locale/cs/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    87804 2023-04-23 19:57:27.366207 Sphinx-7.0.0/sphinx/locale/cs/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3472 2023-04-23 19:57:27.366207 Sphinx-7.0.0/sphinx/locale/cy/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6214 2023-04-23 19:57:27.367207 Sphinx-7.0.0/sphinx/locale/cy/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    87070 2023-04-23 19:57:27.367425 Sphinx-7.0.0/sphinx/locale/cy/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3726 2023-04-23 19:57:27.367425 Sphinx-7.0.0/sphinx/locale/da/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    13099 2023-04-23 19:57:27.367425 Sphinx-7.0.0/sphinx/locale/da/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    89619 2023-04-23 19:57:27.367425 Sphinx-7.0.0/sphinx/locale/da/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3594 2023-04-23 19:57:27.368431 Sphinx-7.0.0/sphinx/locale/de/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    11216 2023-04-23 19:57:27.368431 Sphinx-7.0.0/sphinx/locale/de/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    89151 2023-04-23 19:57:27.368431 Sphinx-7.0.0/sphinx/locale/de/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     8904 2023-04-23 19:57:27.369431 Sphinx-7.0.0/sphinx/locale/el/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    81979 2023-04-23 19:57:27.369431 Sphinx-7.0.0/sphinx/locale/el/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   133241 2023-04-23 19:57:27.370445 Sphinx-7.0.0/sphinx/locale/el/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2363 2023-04-23 19:57:27.370445 Sphinx-7.0.0/sphinx/locale/en_FR/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      462 2023-04-23 19:57:27.370445 Sphinx-7.0.0/sphinx/locale/en_FR/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84193 2023-04-23 19:57:27.371431 Sphinx-7.0.0/sphinx/locale/en_FR/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2364 2023-04-23 19:57:27.371431 Sphinx-7.0.0/sphinx/locale/en_GB/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    13825 2023-04-23 19:57:27.371431 Sphinx-7.0.0/sphinx/locale/en_GB/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    89843 2023-04-23 19:57:27.373431 Sphinx-7.0.0/sphinx/locale/en_GB/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2364 2023-04-23 19:57:27.373431 Sphinx-7.0.0/sphinx/locale/en_HK/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      508 2023-04-23 19:57:27.374431 Sphinx-7.0.0/sphinx/locale/en_HK/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84196 2023-04-23 19:57:27.374431 Sphinx-7.0.0/sphinx/locale/en_HK/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2518 2023-04-23 19:57:27.374431 Sphinx-7.0.0/sphinx/locale/eo/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     1864 2023-04-23 19:57:27.374431 Sphinx-7.0.0/sphinx/locale/eo/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84676 2023-04-23 19:57:27.374431 Sphinx-7.0.0/sphinx/locale/eo/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4319 2023-04-23 19:57:27.375430 Sphinx-7.0.0/sphinx/locale/es/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    82560 2023-04-23 19:57:27.375430 Sphinx-7.0.0/sphinx/locale/es/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   122518 2023-04-23 19:57:27.376438 Sphinx-7.0.0/sphinx/locale/es/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3781 2023-04-23 19:57:27.376438 Sphinx-7.0.0/sphinx/locale/et/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    33706 2023-04-23 19:57:27.377431 Sphinx-7.0.0/sphinx/locale/et/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    97950 2023-04-23 19:57:27.377431 Sphinx-7.0.0/sphinx/locale/et/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3163 2023-04-23 19:57:27.377431 Sphinx-7.0.0/sphinx/locale/eu/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6727 2023-04-23 19:57:27.378430 Sphinx-7.0.0/sphinx/locale/eu/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86399 2023-04-23 19:57:27.378510 Sphinx-7.0.0/sphinx/locale/eu/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     7742 2023-04-23 19:57:27.378510 Sphinx-7.0.0/sphinx/locale/fa/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    98774 2023-04-23 19:57:27.379515 Sphinx-7.0.0/sphinx/locale/fa/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   140105 2023-04-23 19:57:27.379515 Sphinx-7.0.0/sphinx/locale/fa/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2848 2023-04-23 19:57:27.380514 Sphinx-7.0.0/sphinx/locale/fi/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     2912 2023-04-23 19:57:27.380514 Sphinx-7.0.0/sphinx/locale/fi/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84980 2023-04-23 19:57:27.380514 Sphinx-7.0.0/sphinx/locale/fi/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4309 2023-04-23 19:57:27.381514 Sphinx-7.0.0/sphinx/locale/fr/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    85079 2023-04-23 19:57:27.381514 Sphinx-7.0.0/sphinx/locale/fr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   125547 2023-04-23 19:57:27.381514 Sphinx-7.0.0/sphinx/locale/fr/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2415 2023-04-23 19:57:27.381514 Sphinx-7.0.0/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      555 2023-04-23 19:57:27.381514 Sphinx-7.0.0/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84243 2023-04-23 19:57:27.382515 Sphinx-7.0.0/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4946 2023-04-23 19:57:27.382515 Sphinx-7.0.0/sphinx/locale/he/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     4947 2023-04-23 19:57:27.382515 Sphinx-7.0.0/sphinx/locale/he/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86015 2023-04-23 19:57:27.382515 Sphinx-7.0.0/sphinx/locale/he/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     7677 2023-04-23 19:57:27.383515 Sphinx-7.0.0/sphinx/locale/hi/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    98543 2023-04-23 19:57:27.383515 Sphinx-7.0.0/sphinx/locale/hi/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   147260 2023-04-23 19:57:27.384515 Sphinx-7.0.0/sphinx/locale/hi/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2364 2023-04-23 19:57:27.384515 Sphinx-7.0.0/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      502 2023-04-23 19:57:27.384515 Sphinx-7.0.0/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84190 2023-04-23 19:57:27.385517 Sphinx-7.0.0/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3797 2023-04-23 19:57:27.385517 Sphinx-7.0.0/sphinx/locale/hr/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    17189 2023-04-23 19:57:27.385517 Sphinx-7.0.0/sphinx/locale/hr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    90656 2023-04-23 19:57:27.386515 Sphinx-7.0.0/sphinx/locale/hr/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4041 2023-04-23 19:57:27.386515 Sphinx-7.0.0/sphinx/locale/hu/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    11533 2023-04-23 19:57:27.386515 Sphinx-7.0.0/sphinx/locale/hu/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88685 2023-04-23 19:57:27.386515 Sphinx-7.0.0/sphinx/locale/hu/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3613 2023-04-23 19:57:27.387514 Sphinx-7.0.0/sphinx/locale/id/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    60590 2023-04-23 19:57:27.387514 Sphinx-7.0.0/sphinx/locale/id/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   109933 2023-04-23 19:57:27.387514 Sphinx-7.0.0/sphinx/locale/id/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2886 2023-04-23 19:57:27.388515 Sphinx-7.0.0/sphinx/locale/is/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     3082 2023-04-23 19:57:27.388515 Sphinx-7.0.0/sphinx/locale/is/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85100 2023-04-23 19:57:27.388515 Sphinx-7.0.0/sphinx/locale/is/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3727 2023-04-23 19:57:27.388515 Sphinx-7.0.0/sphinx/locale/it/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    10819 2023-04-23 19:57:27.389514 Sphinx-7.0.0/sphinx/locale/it/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88216 2023-04-23 19:57:27.389514 Sphinx-7.0.0/sphinx/locale/it/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     5105 2023-04-23 19:57:27.389514 Sphinx-7.0.0/sphinx/locale/ja/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    87432 2023-04-23 19:57:27.390514 Sphinx-7.0.0/sphinx/locale/ja/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   129215 2023-04-23 19:57:27.390514 Sphinx-7.0.0/sphinx/locale/ja/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4973 2023-04-23 19:57:27.391515 Sphinx-7.0.0/sphinx/locale/ko/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    83942 2023-04-23 19:57:27.391515 Sphinx-7.0.0/sphinx/locale/ko/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   123556 2023-04-23 19:57:27.392514 Sphinx-7.0.0/sphinx/locale/ko/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3534 2023-04-23 19:57:27.392514 Sphinx-7.0.0/sphinx/locale/lt/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     7104 2023-04-23 19:57:27.392514 Sphinx-7.0.0/sphinx/locale/lt/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86600 2023-04-23 19:57:27.392514 Sphinx-7.0.0/sphinx/locale/lt/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3506 2023-04-23 19:57:27.393514 Sphinx-7.0.0/sphinx/locale/lv/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6786 2023-04-23 19:57:27.393514 Sphinx-7.0.0/sphinx/locale/lv/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86319 2023-04-23 19:57:27.393514 Sphinx-7.0.0/sphinx/locale/lv/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2476 2023-04-23 19:57:27.393514 Sphinx-7.0.0/sphinx/locale/mk/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     2011 2023-04-23 19:57:27.394514 Sphinx-7.0.0/sphinx/locale/mk/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84870 2023-04-23 19:57:27.394514 Sphinx-7.0.0/sphinx/locale/mk/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3169 2023-04-23 19:57:27.394514 Sphinx-7.0.0/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6766 2023-04-23 19:57:27.394514 Sphinx-7.0.0/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86123 2023-04-23 19:57:27.394514 Sphinx-7.0.0/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     6284 2023-04-23 19:57:27.395514 Sphinx-7.0.0/sphinx/locale/ne/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     8869 2023-04-23 19:57:27.395514 Sphinx-7.0.0/sphinx/locale/ne/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88391 2023-04-23 19:57:27.395514 Sphinx-7.0.0/sphinx/locale/ne/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3637 2023-04-23 19:57:27.396514 Sphinx-7.0.0/sphinx/locale/nl/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    19426 2023-04-23 19:57:27.396514 Sphinx-7.0.0/sphinx/locale/nl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    91992 2023-04-23 19:57:27.396514 Sphinx-7.0.0/sphinx/locale/nl/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3967 2023-04-23 19:57:27.397514 Sphinx-7.0.0/sphinx/locale/pl/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    29754 2023-04-23 19:57:27.397514 Sphinx-7.0.0/sphinx/locale/pl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    96611 2023-04-23 19:57:27.397514 Sphinx-7.0.0/sphinx/locale/pl/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2412 2023-04-23 19:57:27.397514 Sphinx-7.0.0/sphinx/locale/pt/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      544 2023-04-23 19:57:27.397514 Sphinx-7.0.0/sphinx/locale/pt/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84232 2023-04-23 19:57:27.398514 Sphinx-7.0.0/sphinx/locale/pt/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4325 2023-04-23 19:57:27.398514 Sphinx-7.0.0/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    80235 2023-04-23 19:57:27.399515 Sphinx-7.0.0/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   120545 2023-04-23 19:57:27.400031 Sphinx-7.0.0/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3806 2023-04-23 19:57:27.400031 Sphinx-7.0.0/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     8035 2023-04-23 19:57:27.400031 Sphinx-7.0.0/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86961 2023-04-23 19:57:27.401036 Sphinx-7.0.0/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3761 2023-04-23 19:57:27.401036 Sphinx-7.0.0/sphinx/locale/ro/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     8822 2023-04-23 19:57:27.401036 Sphinx-7.0.0/sphinx/locale/ro/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    87272 2023-04-23 19:57:27.401036 Sphinx-7.0.0/sphinx/locale/ro/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     8313 2023-04-23 19:57:27.402036 Sphinx-7.0.0/sphinx/locale/ru/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    16339 2023-04-23 19:57:27.402036 Sphinx-7.0.0/sphinx/locale/ru/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    92408 2023-04-23 19:57:27.402036 Sphinx-7.0.0/sphinx/locale/ru/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3877 2023-04-23 19:57:27.403036 Sphinx-7.0.0/sphinx/locale/si/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     3602 2023-04-23 19:57:27.403036 Sphinx-7.0.0/sphinx/locale/si/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85680 2023-04-23 19:57:27.403036 Sphinx-7.0.0/sphinx/locale/si/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4265 2023-04-23 19:57:27.404037 Sphinx-7.0.0/sphinx/locale/sk/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    67619 2023-04-23 19:57:27.404037 Sphinx-7.0.0/sphinx/locale/sk/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   113547 2023-04-23 19:57:27.404037 Sphinx-7.0.0/sphinx/locale/sk/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3246 2023-04-23 19:57:27.405036 Sphinx-7.0.0/sphinx/locale/sl/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     5417 2023-04-23 19:57:27.405036 Sphinx-7.0.0/sphinx/locale/sl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85800 2023-04-23 19:57:27.405036 Sphinx-7.0.0/sphinx/locale/sl/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0    84162 2023-04-23 19:57:27.405036 Sphinx-7.0.0/sphinx/locale/sphinx.pot
--rw-r--r--   0        0        0     4390 2023-04-23 19:57:27.406036 Sphinx-7.0.0/sphinx/locale/sq/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    78940 2023-04-23 19:57:27.406036 Sphinx-7.0.0/sphinx/locale/sq/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   120398 2023-04-23 19:57:27.407039 Sphinx-7.0.0/sphinx/locale/sq/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2441 2023-04-23 19:57:27.408036 Sphinx-7.0.0/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      584 2023-04-23 19:57:27.408036 Sphinx-7.0.0/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84272 2023-04-23 19:57:27.408036 Sphinx-7.0.0/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4161 2023-04-23 19:57:27.407039 Sphinx-7.0.0/sphinx/locale/sr/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     9426 2023-04-23 19:57:27.407039 Sphinx-7.0.0/sphinx/locale/sr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88404 2023-04-23 19:57:27.408036 Sphinx-7.0.0/sphinx/locale/sr/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2443 2023-04-23 19:57:27.408036 Sphinx-7.0.0/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      579 2023-04-23 19:57:27.409036 Sphinx-7.0.0/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84267 2023-04-23 19:57:27.409036 Sphinx-7.0.0/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3342 2023-04-23 19:57:27.409036 Sphinx-7.0.0/sphinx/locale/sv/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6754 2023-04-23 19:57:27.409036 Sphinx-7.0.0/sphinx/locale/sv/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86142 2023-04-23 19:57:27.410038 Sphinx-7.0.0/sphinx/locale/sv/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2361 2023-04-23 19:57:27.410038 Sphinx-7.0.0/sphinx/locale/ta/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      647 2023-04-23 19:57:27.410038 Sphinx-7.0.0/sphinx/locale/ta/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84340 2023-04-23 19:57:27.410038 Sphinx-7.0.0/sphinx/locale/ta/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2361 2023-04-23 19:57:27.411036 Sphinx-7.0.0/sphinx/locale/te/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      489 2023-04-23 19:57:27.411036 Sphinx-7.0.0/sphinx/locale/te/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84177 2023-04-23 19:57:27.411036 Sphinx-7.0.0/sphinx/locale/te/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4099 2023-04-23 19:57:27.411036 Sphinx-7.0.0/sphinx/locale/tr/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    58138 2023-04-23 19:57:27.412036 Sphinx-7.0.0/sphinx/locale/tr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   109922 2023-04-23 19:57:27.412036 Sphinx-7.0.0/sphinx/locale/tr/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     6344 2023-04-23 19:57:27.413036 Sphinx-7.0.0/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6693 2023-04-23 19:57:27.413036 Sphinx-7.0.0/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    87195 2023-04-23 19:57:27.413036 Sphinx-7.0.0/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2361 2023-04-23 19:57:27.413036 Sphinx-7.0.0/sphinx/locale/ur/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      487 2023-04-23 19:57:27.413036 Sphinx-7.0.0/sphinx/locale/ur/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84175 2023-04-23 19:57:27.414036 Sphinx-7.0.0/sphinx/locale/ur/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3581 2023-04-23 19:57:27.414036 Sphinx-7.0.0/sphinx/locale/vi/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     5971 2023-04-23 19:57:27.414036 Sphinx-7.0.0/sphinx/locale/vi/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86239 2023-04-23 19:57:27.414036 Sphinx-7.0.0/sphinx/locale/vi/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2355 2023-04-23 19:57:27.415036 Sphinx-7.0.0/sphinx/locale/yue/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      487 2023-04-23 19:57:27.415036 Sphinx-7.0.0/sphinx/locale/yue/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84175 2023-04-23 19:57:27.415036 Sphinx-7.0.0/sphinx/locale/yue/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4455 2023-04-23 19:57:27.415036 Sphinx-7.0.0/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    76383 2023-04-23 19:57:27.416271 Sphinx-7.0.0/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   116078 2023-04-23 19:57:27.416725 Sphinx-7.0.0/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2362 2023-04-23 19:57:27.416725 Sphinx-7.0.0/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      501 2023-04-23 19:57:27.416725 Sphinx-7.0.0/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84189 2023-04-23 19:57:27.417852 Sphinx-7.0.0/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2362 2023-04-23 19:57:27.417852 Sphinx-7.0.0/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      516 2023-04-23 19:57:27.417852 Sphinx-7.0.0/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84204 2023-04-23 19:57:27.417852 Sphinx-7.0.0/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4639 2023-04-23 19:57:27.418852 Sphinx-7.0.0/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    75797 2023-04-23 19:57:27.418852 Sphinx-7.0.0/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   115249 2023-04-23 19:57:27.419852 Sphinx-7.0.0/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3098 2023-04-23 19:57:27.419852 Sphinx-7.0.0/sphinx/parsers.py
--rw-r--r--   0        0        0     3432 2023-04-23 19:57:27.420852 Sphinx-7.0.0/sphinx/project.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.420852 Sphinx-7.0.0/sphinx/py.typed
--rw-r--r--   0        0        0     5581 2023-04-23 19:57:27.420852 Sphinx-7.0.0/sphinx/pycode/__init__.py
--rw-r--r--   0        0        0     6648 2023-04-27 13:52:14.963498 Sphinx-7.0.0/sphinx/pycode/ast.py
--rw-r--r--   0        0        0    21072 2023-04-23 19:57:27.420852 Sphinx-7.0.0/sphinx/pycode/parser.py
--rw-r--r--   0        0        0     2861 2023-04-23 19:57:27.421852 Sphinx-7.0.0/sphinx/pygments_styles.py
--rw-r--r--   0        0        0    21983 2023-04-28 09:26:30.898486 Sphinx-7.0.0/sphinx/registry.py
--rw-r--r--   0        0        0    15975 2023-04-23 19:57:27.421852 Sphinx-7.0.0/sphinx/roles.py
--rw-r--r--   0        0        0    23064 2023-04-27 00:29:16.230978 Sphinx-7.0.0/sphinx/search/__init__.py
--rw-r--r--   0        0        0     3561 2023-04-23 19:57:27.422852 Sphinx-7.0.0/sphinx/search/da.py
--rw-r--r--   0        0        0     4637 2023-04-23 19:57:27.422852 Sphinx-7.0.0/sphinx/search/de.py
--rw-r--r--   0        0        0     4899 2023-04-23 19:57:27.422852 Sphinx-7.0.0/sphinx/search/en.py
--rw-r--r--   0        0        0     5723 2023-04-23 19:57:27.422852 Sphinx-7.0.0/sphinx/search/es.py
--rw-r--r--   0        0        0     3207 2023-04-23 19:57:27.423852 Sphinx-7.0.0/sphinx/search/fi.py
--rw-r--r--   0        0        0     3438 2023-04-23 19:57:27.423852 Sphinx-7.0.0/sphinx/search/fr.py
--rw-r--r--   0        0        0     1949 2023-04-23 19:57:27.423852 Sphinx-7.0.0/sphinx/search/hu.py
--rw-r--r--   0        0        0     5089 2023-04-23 19:57:27.424852 Sphinx-7.0.0/sphinx/search/it.py
--rw-r--r--   0        0        0    30997 2023-04-27 00:29:16.230978 Sphinx-7.0.0/sphinx/search/ja.py
--rw-r--r--   0        0        0     3594 2023-04-23 19:57:27.424852 Sphinx-7.0.0/sphinx/search/minified-js/base-stemmer.js
--rw-r--r--   0        0        0     3123 2023-04-23 19:57:27.424852 Sphinx-7.0.0/sphinx/search/minified-js/danish-stemmer.js
--rw-r--r--   0        0        0     5529 2023-04-23 19:57:27.425852 Sphinx-7.0.0/sphinx/search/minified-js/dutch-stemmer.js
--rw-r--r--   0        0        0     7529 2023-04-23 19:57:27.425852 Sphinx-7.0.0/sphinx/search/minified-js/finnish-stemmer.js
--rw-r--r--   0        0        0    11571 2023-04-23 19:57:27.426185 Sphinx-7.0.0/sphinx/search/minified-js/french-stemmer.js
--rw-r--r--   0        0        0     4669 2023-04-23 19:57:27.426185 Sphinx-7.0.0/sphinx/search/minified-js/german-stemmer.js
--rw-r--r--   0        0        0     6614 2023-04-23 19:57:27.426185 Sphinx-7.0.0/sphinx/search/minified-js/hungarian-stemmer.js
--rw-r--r--   0        0        0     9100 2023-04-23 19:57:27.426185 Sphinx-7.0.0/sphinx/search/minified-js/italian-stemmer.js
--rw-r--r--   0        0        0     2594 2023-04-23 19:57:27.426185 Sphinx-7.0.0/sphinx/search/minified-js/norwegian-stemmer.js
--rw-r--r--   0        0        0     6439 2023-04-23 19:57:27.427191 Sphinx-7.0.0/sphinx/search/minified-js/porter-stemmer.js
--rw-r--r--   0        0        0     8373 2023-04-23 19:57:27.427191 Sphinx-7.0.0/sphinx/search/minified-js/portuguese-stemmer.js
--rw-r--r--   0        0        0     8333 2023-04-23 19:57:27.427191 Sphinx-7.0.0/sphinx/search/minified-js/romanian-stemmer.js
--rw-r--r--   0        0        0     5735 2023-04-23 19:57:27.427191 Sphinx-7.0.0/sphinx/search/minified-js/russian-stemmer.js
--rw-r--r--   0        0        0     9121 2023-04-23 19:57:27.427191 Sphinx-7.0.0/sphinx/search/minified-js/spanish-stemmer.js
--rw-r--r--   0        0        0     2654 2023-04-23 19:57:27.427191 Sphinx-7.0.0/sphinx/search/minified-js/swedish-stemmer.js
--rw-r--r--   0        0        0    19972 2023-04-23 19:57:27.428192 Sphinx-7.0.0/sphinx/search/minified-js/turkish-stemmer.js
--rw-r--r--   0        0        0     4571 2023-04-23 19:57:27.428192 Sphinx-7.0.0/sphinx/search/nl.py
--rw-r--r--   0        0        0     4893 2023-04-23 19:57:27.428192 Sphinx-7.0.0/sphinx/search/no.py
--rw-r--r--   0        0        0     8133 2023-04-23 19:57:27.428192 Sphinx-7.0.0/sphinx/search/non-minified-js/base-stemmer.js
--rw-r--r--   0        0        0     8134 2023-04-23 19:57:27.429191 Sphinx-7.0.0/sphinx/search/non-minified-js/danish-stemmer.js
--rw-r--r--   0        0        0    19495 2023-04-23 19:57:27.429191 Sphinx-7.0.0/sphinx/search/non-minified-js/dutch-stemmer.js
--rw-r--r--   0        0        0    21286 2023-04-23 19:57:27.429191 Sphinx-7.0.0/sphinx/search/non-minified-js/finnish-stemmer.js
--rw-r--r--   0        0        0    42080 2023-04-23 19:57:27.429191 Sphinx-7.0.0/sphinx/search/non-minified-js/french-stemmer.js
--rw-r--r--   0        0        0    17647 2023-04-23 19:57:27.430191 Sphinx-7.0.0/sphinx/search/non-minified-js/german-stemmer.js
--rw-r--r--   0        0        0    17564 2023-04-23 19:57:27.430191 Sphinx-7.0.0/sphinx/search/non-minified-js/hungarian-stemmer.js
--rw-r--r--   0        0        0    29065 2023-04-23 19:57:27.430191 Sphinx-7.0.0/sphinx/search/non-minified-js/italian-stemmer.js
--rw-r--r--   0        0        0     6870 2023-04-23 19:57:27.430191 Sphinx-7.0.0/sphinx/search/non-minified-js/norwegian-stemmer.js
--rw-r--r--   0        0        0    20391 2023-04-23 19:57:27.431192 Sphinx-7.0.0/sphinx/search/non-minified-js/porter-stemmer.js
--rw-r--r--   0        0        0    26718 2023-04-23 19:57:27.431192 Sphinx-7.0.0/sphinx/search/non-minified-js/portuguese-stemmer.js
--rw-r--r--   0        0        0    25006 2023-04-23 19:57:27.431192 Sphinx-7.0.0/sphinx/search/non-minified-js/romanian-stemmer.js
--rw-r--r--   0        0        0    17996 2023-04-23 19:57:27.431192 Sphinx-7.0.0/sphinx/search/non-minified-js/russian-stemmer.js
--rw-r--r--   0        0        0    28534 2023-04-23 19:57:27.431192 Sphinx-7.0.0/sphinx/search/non-minified-js/spanish-stemmer.js
--rw-r--r--   0        0        0     6851 2023-04-23 19:57:27.432192 Sphinx-7.0.0/sphinx/search/non-minified-js/swedish-stemmer.js
--rw-r--r--   0        0        0    77511 2023-04-23 19:57:27.432192 Sphinx-7.0.0/sphinx/search/non-minified-js/turkish-stemmer.js
--rw-r--r--   0        0        0     4648 2023-04-23 19:57:27.432192 Sphinx-7.0.0/sphinx/search/pt.py
--rw-r--r--   0        0        0      557 2023-04-23 19:57:27.432192 Sphinx-7.0.0/sphinx/search/ro.py
--rw-r--r--   0        0        0     7905 2023-04-23 19:57:27.433192 Sphinx-7.0.0/sphinx/search/ru.py
--rw-r--r--   0        0        0     3436 2023-04-23 19:57:27.433192 Sphinx-7.0.0/sphinx/search/sv.py
--rw-r--r--   0        0        0      551 2023-04-23 19:57:27.433192 Sphinx-7.0.0/sphinx/search/tr.py
--rw-r--r--   0        0        0     6146 2023-04-23 19:57:27.433192 Sphinx-7.0.0/sphinx/search/zh.py
--rw-r--r--   0        0        0      196 2023-04-23 19:57:27.434192 Sphinx-7.0.0/sphinx/templates/apidoc/module.rst_t
--rw-r--r--   0        0        0     1173 2023-04-23 19:57:27.434192 Sphinx-7.0.0/sphinx/templates/apidoc/package.rst_t
--rw-r--r--   0        0        0      128 2023-04-23 19:57:27.434192 Sphinx-7.0.0/sphinx/templates/apidoc/toc.rst_t
--rw-r--r--   0        0        0      246 2023-04-23 19:57:27.434192 Sphinx-7.0.0/sphinx/templates/epub3/container.xml
--rw-r--r--   0        0        0     2127 2023-04-23 19:57:27.434192 Sphinx-7.0.0/sphinx/templates/epub3/content.opf_t
--rw-r--r--   0        0        0       20 2023-04-23 19:57:27.434192 Sphinx-7.0.0/sphinx/templates/epub3/mimetype
--rw-r--r--   0        0        0      629 2023-04-23 19:57:27.435192 Sphinx-7.0.0/sphinx/templates/epub3/nav.xhtml_t
--rw-r--r--   0        0        0      743 2023-04-23 19:57:27.435192 Sphinx-7.0.0/sphinx/templates/epub3/toc.ncx_t
--rw-r--r--   0        0        0      875 2023-04-23 19:57:27.435192 Sphinx-7.0.0/sphinx/templates/gettext/message.pot_t
--rw-r--r--   0        0        0      299 2023-04-23 19:57:27.435192 Sphinx-7.0.0/sphinx/templates/graphviz/graphviz.css
--rw-r--r--   0        0        0      864 2023-04-23 19:57:27.435192 Sphinx-7.0.0/sphinx/templates/htmlhelp/project.hhc
--rw-r--r--   0        0        0      570 2023-04-23 19:57:27.436192 Sphinx-7.0.0/sphinx/templates/htmlhelp/project.hhp
--rw-r--r--   0        0        0      165 2023-04-25 10:59:46.881271 Sphinx-7.0.0/sphinx/templates/htmlhelp/project.stp
--rw-r--r--   0        0        0      397 2023-04-23 19:57:27.436192 Sphinx-7.0.0/sphinx/templates/imgmath/preview.tex_t
--rw-r--r--   0        0        0      321 2023-04-23 19:57:27.436192 Sphinx-7.0.0/sphinx/templates/imgmath/template.tex_t
--rw-r--r--   0        0        0     2986 2023-04-23 19:57:27.436192 Sphinx-7.0.0/sphinx/templates/latex/latex.tex_t
--rw-r--r--   0        0        0     2156 2023-04-23 19:57:27.437192 Sphinx-7.0.0/sphinx/templates/latex/longtable.tex_t
--rw-r--r--   0        0        0      944 2023-04-23 19:57:27.437192 Sphinx-7.0.0/sphinx/templates/latex/sphinxmessages.sty_t
--rw-r--r--   0        0        0     1406 2023-04-23 19:57:27.437192 Sphinx-7.0.0/sphinx/templates/latex/tabular.tex_t
--rw-r--r--   0        0        0     1420 2023-04-23 19:57:27.437192 Sphinx-7.0.0/sphinx/templates/latex/tabulary.tex_t
--rw-r--r--   0        0        0      656 2023-04-23 19:57:27.437192 Sphinx-7.0.0/sphinx/templates/quickstart/Makefile.new_t
--rw-r--r--   0        0        0     4031 2023-04-23 19:57:27.437192 Sphinx-7.0.0/sphinx/templates/quickstart/Makefile_t
--rw-r--r--   0        0        0     2129 2023-04-23 19:57:27.438192 Sphinx-7.0.0/sphinx/templates/quickstart/conf.py_t
--rw-r--r--   0        0        0      787 2023-04-23 19:57:27.438192 Sphinx-7.0.0/sphinx/templates/quickstart/make.bat.new_t
--rw-r--r--   0        0        0     3293 2023-04-23 19:57:27.438192 Sphinx-7.0.0/sphinx/templates/quickstart/make.bat_t
--rw-r--r--   0        0        0      492 2023-04-23 19:57:27.438192 Sphinx-7.0.0/sphinx/templates/quickstart/root_doc.rst_t
--rw-r--r--   0        0        0     1423 2023-04-23 19:57:27.438192 Sphinx-7.0.0/sphinx/templates/texinfo/Makefile
--rw-r--r--   0        0        0      171 2023-04-23 19:57:27.439192 Sphinx-7.0.0/sphinx/testing/__init__.py
--rw-r--r--   0        0        0     2710 2023-04-23 19:57:27.439192 Sphinx-7.0.0/sphinx/testing/comparer.py
--rw-r--r--   0        0        0     7508 2023-04-23 19:57:27.439192 Sphinx-7.0.0/sphinx/testing/fixtures.py
--rw-r--r--   0        0        0     6317 2023-04-25 10:53:02.931530 Sphinx-7.0.0/sphinx/testing/path.py
--rw-r--r--   0        0        0     1029 2023-04-23 19:57:27.439192 Sphinx-7.0.0/sphinx/testing/restructuredtext.py
--rw-r--r--   0        0        0     7297 2023-04-23 19:57:27.439192 Sphinx-7.0.0/sphinx/testing/util.py
--rw-r--r--   0        0        0     4366 2023-04-23 19:57:27.440192 Sphinx-7.0.0/sphinx/texinputs/LICRcyr2utf8.xdy
--rw-r--r--   0        0        0    10188 2023-04-23 19:57:27.440192 Sphinx-7.0.0/sphinx/texinputs/LICRlatin2utf8.xdy
--rw-r--r--   0        0        0    18890 2023-04-23 19:57:27.440192 Sphinx-7.0.0/sphinx/texinputs/LatinRules.xdy
--rw-r--r--   0        0        0     2401 2023-04-23 19:57:27.440192 Sphinx-7.0.0/sphinx/texinputs/Makefile_t
--rw-r--r--   0        0        0      695 2023-04-23 19:57:27.440192 Sphinx-7.0.0/sphinx/texinputs/latexmkjarc_t
--rw-r--r--   0        0        0     1104 2023-04-23 19:57:27.441192 Sphinx-7.0.0/sphinx/texinputs/latexmkrc_t
--rw-r--r--   0        0        0     1041 2023-04-23 19:57:27.441192 Sphinx-7.0.0/sphinx/texinputs/make.bat_t
--rw-r--r--   0        0        0      392 2023-04-23 19:57:27.441192 Sphinx-7.0.0/sphinx/texinputs/python.ist
--rw-r--r--   0        0        0    44560 2023-04-23 19:57:27.441192 Sphinx-7.0.0/sphinx/texinputs/sphinx.sty
--rw-r--r--   0        0        0     9474 2023-04-23 19:57:27.442192 Sphinx-7.0.0/sphinx/texinputs/sphinx.xdy
--rw-r--r--   0        0        0     3256 2023-04-23 19:57:27.442510 Sphinx-7.0.0/sphinx/texinputs/sphinxhowto.cls
--rw-r--r--   0        0        0    10989 2023-04-23 19:57:27.442791 Sphinx-7.0.0/sphinx/texinputs/sphinxlatexadmonitions.sty
--rw-r--r--   0        0        0      901 2023-04-23 19:57:27.442999 Sphinx-7.0.0/sphinx/texinputs/sphinxlatexcontainers.sty
--rw-r--r--   0        0        0     4840 2023-04-23 19:57:27.443155 Sphinx-7.0.0/sphinx/texinputs/sphinxlatexgraphics.sty
--rw-r--r--   0        0        0     2066 2023-04-23 19:57:27.443155 Sphinx-7.0.0/sphinx/texinputs/sphinxlatexindbibtoc.sty
--rw-r--r--   0        0        0     5139 2023-04-23 19:57:27.443523 Sphinx-7.0.0/sphinx/texinputs/sphinxlatexlists.sty
--rw-r--r--   0        0        0    46048 2023-04-23 19:57:27.443889 Sphinx-7.0.0/sphinx/texinputs/sphinxlatexliterals.sty
--rw-r--r--   0        0        0     4532 2023-04-23 19:57:27.444274 Sphinx-7.0.0/sphinx/texinputs/sphinxlatexnumfig.sty
--rw-r--r--   0        0        0     9067 2023-04-23 19:57:27.444274 Sphinx-7.0.0/sphinx/texinputs/sphinxlatexobjects.sty
--rw-r--r--   0        0        0     5066 2023-04-23 19:57:27.444274 Sphinx-7.0.0/sphinx/texinputs/sphinxlatexshadowbox.sty
--rw-r--r--   0        0        0     3445 2023-04-23 19:57:27.444274 Sphinx-7.0.0/sphinx/texinputs/sphinxlatexstyleheadings.sty
--rw-r--r--   0        0        0     3064 2023-04-23 19:57:27.445286 Sphinx-7.0.0/sphinx/texinputs/sphinxlatexstylepage.sty
--rw-r--r--   0        0        0     8232 2023-04-23 19:57:27.445286 Sphinx-7.0.0/sphinx/texinputs/sphinxlatexstyletext.sty
--rw-r--r--   0        0        0    57830 2023-04-23 19:57:27.445286 Sphinx-7.0.0/sphinx/texinputs/sphinxlatextables.sty
--rw-r--r--   0        0        0     4241 2023-04-23 19:57:27.445286 Sphinx-7.0.0/sphinx/texinputs/sphinxmanual.cls
--rw-r--r--   0        0        0     2061 2023-04-23 19:57:27.446286 Sphinx-7.0.0/sphinx/texinputs/sphinxoptionsgeometry.sty
--rw-r--r--   0        0        0     1094 2023-04-23 19:57:27.446286 Sphinx-7.0.0/sphinx/texinputs/sphinxoptionshyperref.sty
--rw-r--r--   0        0        0    36615 2023-04-23 19:57:27.446286 Sphinx-7.0.0/sphinx/texinputs/sphinxpackageboxes.sty
--rw-r--r--   0        0        0     2590 2023-04-23 19:57:27.446286 Sphinx-7.0.0/sphinx/texinputs/sphinxpackagecyrillic.sty
--rw-r--r--   0        0        0    15254 2023-04-23 19:57:27.447286 Sphinx-7.0.0/sphinx/texinputs/sphinxpackagefootnote.sty
--rw-r--r--   0        0        0     2503 2023-04-23 19:57:27.447286 Sphinx-7.0.0/sphinx/texinputs_win/Makefile_t
--rw-r--r--   0        0        0     3321 2023-04-23 19:57:27.447286 Sphinx-7.0.0/sphinx/themes/agogo/layout.html
--rw-r--r--   0        0        0     9144 2023-04-23 19:57:27.448286 Sphinx-7.0.0/sphinx/themes/agogo/static/agogo.css_t
--rw-r--r--   0        0        0      276 2023-04-23 19:57:27.448286 Sphinx-7.0.0/sphinx/themes/agogo/static/bgfooter.png
--rw-r--r--   0        0        0      266 2023-04-23 19:57:27.448286 Sphinx-7.0.0/sphinx/themes/agogo/static/bgtop.png
--rw-r--r--   0        0        0      477 2023-04-23 19:57:27.448286 Sphinx-7.0.0/sphinx/themes/agogo/theme.conf
--rw-r--r--   0        0        0      466 2023-04-23 19:57:27.448286 Sphinx-7.0.0/sphinx/themes/basic/changes/frameset.html
--rw-r--r--   0        0        0      485 2023-04-23 19:57:27.448286 Sphinx-7.0.0/sphinx/themes/basic/changes/rstsource.html
--rw-r--r--   0        0        0     1306 2023-04-23 19:57:27.449286 Sphinx-7.0.0/sphinx/themes/basic/changes/versionchanges.html
--rw-r--r--   0        0        0     1636 2023-04-23 19:57:27.449286 Sphinx-7.0.0/sphinx/themes/basic/defindex.html
--rw-r--r--   0        0        0     1892 2023-04-23 19:57:27.449286 Sphinx-7.0.0/sphinx/themes/basic/domainindex.html
--rw-r--r--   0        0        0     1804 2023-04-23 19:57:27.449286 Sphinx-7.0.0/sphinx/themes/basic/genindex-single.html
--rw-r--r--   0        0        0     1210 2023-04-23 19:57:27.449286 Sphinx-7.0.0/sphinx/themes/basic/genindex-split.html
--rw-r--r--   0        0        0     2069 2023-04-23 19:57:27.449286 Sphinx-7.0.0/sphinx/themes/basic/genindex.html
--rw-r--r--   0        0        0      432 2023-04-23 19:57:27.450286 Sphinx-7.0.0/sphinx/themes/basic/globaltoc.html
--rw-r--r--   0        0        0     7128 2023-04-28 10:59:41.037038 Sphinx-7.0.0/sphinx/themes/basic/layout.html
--rw-r--r--   0        0        0      370 2023-04-23 19:57:27.450286 Sphinx-7.0.0/sphinx/themes/basic/localtoc.html
--rw-r--r--   0        0        0      679 2023-04-23 19:57:27.450286 Sphinx-7.0.0/sphinx/themes/basic/opensearch.xml
--rw-r--r--   0        0        0      273 2023-04-23 19:57:27.450286 Sphinx-7.0.0/sphinx/themes/basic/page.html
--rw-r--r--   0        0        0      652 2023-04-23 19:57:27.450286 Sphinx-7.0.0/sphinx/themes/basic/relations.html
--rw-r--r--   0        0        0     2039 2023-04-23 19:57:27.450286 Sphinx-7.0.0/sphinx/themes/basic/search.html
--rw-r--r--   0        0        0      809 2023-04-23 19:57:27.451286 Sphinx-7.0.0/sphinx/themes/basic/searchbox.html
--rw-r--r--   0        0        0      947 2023-04-23 19:57:27.451286 Sphinx-7.0.0/sphinx/themes/basic/searchfield.html
--rw-r--r--   0        0        0      544 2023-04-23 19:57:27.451286 Sphinx-7.0.0/sphinx/themes/basic/sourcelink.html
--rw-r--r--   0        0        0    14893 2023-04-23 19:57:27.451286 Sphinx-7.0.0/sphinx/themes/basic/static/basic.css_t
--rw-r--r--   0        0        0     4472 2023-04-23 19:57:27.452286 Sphinx-7.0.0/sphinx/themes/basic/static/doctools.js
--rw-r--r--   0        0        0      673 2023-04-23 19:57:27.452286 Sphinx-7.0.0/sphinx/themes/basic/static/documentation_options.js_t
--rw-r--r--   0        0        0      286 2023-04-23 19:57:27.452286 Sphinx-7.0.0/sphinx/themes/basic/static/file.png
--rw-r--r--   0        0        0      676 2023-04-23 19:57:27.452286 Sphinx-7.0.0/sphinx/themes/basic/static/language_data.js_t
--rw-r--r--   0        0        0       90 2023-04-23 19:57:27.452286 Sphinx-7.0.0/sphinx/themes/basic/static/minus.png
--rw-r--r--   0        0        0       90 2023-04-23 19:57:27.452286 Sphinx-7.0.0/sphinx/themes/basic/static/plus.png
--rw-r--r--   0        0        0    18215 2023-04-23 19:57:27.453287 Sphinx-7.0.0/sphinx/themes/basic/static/searchtools.js
--rw-r--r--   0        0        0     4712 2023-04-23 19:57:27.453287 Sphinx-7.0.0/sphinx/themes/basic/static/sphinx_highlight.js
--rw-r--r--   0        0        0      371 2023-04-23 19:57:27.453287 Sphinx-7.0.0/sphinx/themes/basic/theme.conf
--rw-r--r--   0        0        0      664 2023-04-23 19:57:27.454287 Sphinx-7.0.0/sphinx/themes/bizstyle/layout.html
--rw-r--r--   0        0        0       78 2023-04-23 19:57:27.454287 Sphinx-7.0.0/sphinx/themes/bizstyle/static/background_b01.png
--rw-r--r--   0        0        0    10314 2023-04-23 19:57:27.454287 Sphinx-7.0.0/sphinx/themes/bizstyle/static/bizstyle.css_t
--rw-r--r--   0        0        0     1129 2023-04-23 19:57:27.454287 Sphinx-7.0.0/sphinx/themes/bizstyle/static/bizstyle.js_t
--rw-r--r--   0        0        0    14940 2023-04-23 19:57:27.455286 Sphinx-7.0.0/sphinx/themes/bizstyle/static/css3-mediaqueries.js
--rw-r--r--   0        0        0    28634 2023-04-23 19:57:27.455286 Sphinx-7.0.0/sphinx/themes/bizstyle/static/css3-mediaqueries_src.js
--rw-r--r--   0        0        0      148 2023-04-23 19:57:27.455286 Sphinx-7.0.0/sphinx/themes/bizstyle/theme.conf
--rw-r--r--   0        0        0      661 2023-04-23 19:57:27.455286 Sphinx-7.0.0/sphinx/themes/classic/layout.html
--rw-r--r--   0        0        0     6635 2023-04-23 19:57:27.456285 Sphinx-7.0.0/sphinx/themes/classic/static/classic.css_t
--rw-r--r--   0        0        0     2659 2023-04-23 19:57:27.456285 Sphinx-7.0.0/sphinx/themes/classic/static/sidebar.js_t
--rw-r--r--   0        0        0      719 2023-04-23 19:57:27.456285 Sphinx-7.0.0/sphinx/themes/classic/theme.conf
--rw-r--r--   0        0        0       28 2023-04-23 19:57:27.456285 Sphinx-7.0.0/sphinx/themes/default/static/default.css
--rw-r--r--   0        0        0       26 2023-04-23 19:57:27.457285 Sphinx-7.0.0/sphinx/themes/default/theme.conf
--rw-r--r--   0        0        0      693 2023-04-23 19:57:27.457285 Sphinx-7.0.0/sphinx/themes/epub/epub-cover.html
--rw-r--r--   0        0        0      543 2023-04-23 19:57:27.457285 Sphinx-7.0.0/sphinx/themes/epub/layout.html
--rw-r--r--   0        0        0    12262 2023-04-23 19:57:27.457285 Sphinx-7.0.0/sphinx/themes/epub/static/epub.css_t
--rw-r--r--   0        0        0      108 2023-04-23 19:57:27.457285 Sphinx-7.0.0/sphinx/themes/epub/theme.conf
--rw-r--r--   0        0        0     2012 2023-04-23 19:57:27.458401 Sphinx-7.0.0/sphinx/themes/haiku/layout.html
--rw-r--r--   0        0        0     1128 2023-04-23 19:57:27.458401 Sphinx-7.0.0/sphinx/themes/haiku/static/alert_info_32.png
--rw-r--r--   0        0        0      944 2023-04-23 19:57:27.458401 Sphinx-7.0.0/sphinx/themes/haiku/static/alert_warning_32.png
--rw-r--r--   0        0        0       82 2023-04-23 19:57:27.458401 Sphinx-7.0.0/sphinx/themes/haiku/static/bg-page.png
--rw-r--r--   0        0        0      165 2023-04-23 19:57:27.458401 Sphinx-7.0.0/sphinx/themes/haiku/static/bullet_orange.png
--rw-r--r--   0        0        0     7059 2023-04-23 19:57:27.458401 Sphinx-7.0.0/sphinx/themes/haiku/static/haiku.css_t
--rw-r--r--   0        0        0      298 2023-04-23 19:57:27.458401 Sphinx-7.0.0/sphinx/themes/haiku/theme.conf
--rw-r--r--   0        0        0     4234 2023-04-23 19:57:27.459407 Sphinx-7.0.0/sphinx/themes/nature/static/nature.css_t
--rw-r--r--   0        0        0       71 2023-04-23 19:57:27.459407 Sphinx-7.0.0/sphinx/themes/nature/theme.conf
--rw-r--r--   0        0        0      642 2023-04-23 19:57:27.459407 Sphinx-7.0.0/sphinx/themes/nonav/layout.html
--rw-r--r--   0        0        0     9636 2023-04-23 19:57:27.460407 Sphinx-7.0.0/sphinx/themes/nonav/static/nonav.css_t
--rw-r--r--   0        0        0      109 2023-04-23 19:57:27.460407 Sphinx-7.0.0/sphinx/themes/nonav/theme.conf
--rw-r--r--   0        0        0      875 2023-04-23 19:57:27.460407 Sphinx-7.0.0/sphinx/themes/pyramid/layout.html
--rw-r--r--   0        0        0     1394 2023-04-23 19:57:27.460407 Sphinx-7.0.0/sphinx/themes/pyramid/static/dialog-note.png
--rw-r--r--   0        0        0     1351 2023-04-23 19:57:27.460407 Sphinx-7.0.0/sphinx/themes/pyramid/static/dialog-seealso.png
--rw-r--r--   0        0        0     1186 2023-04-23 19:57:27.461407 Sphinx-7.0.0/sphinx/themes/pyramid/static/dialog-todo.png
--rw-r--r--   0        0        0     1798 2023-04-23 19:57:27.461407 Sphinx-7.0.0/sphinx/themes/pyramid/static/dialog-topic.png
--rw-r--r--   0        0        0     1280 2023-04-23 19:57:27.461407 Sphinx-7.0.0/sphinx/themes/pyramid/static/dialog-warning.png
--rw-r--r--   0        0        0     5629 2023-04-23 19:57:27.461407 Sphinx-7.0.0/sphinx/themes/pyramid/static/epub.css_t
--rw-r--r--   0        0        0      333 2023-04-23 19:57:27.461407 Sphinx-7.0.0/sphinx/themes/pyramid/static/footerbg.png
--rw-r--r--   0        0        0      190 2023-04-23 19:57:27.461407 Sphinx-7.0.0/sphinx/themes/pyramid/static/headerbg.png
--rw-r--r--   0        0        0      726 2023-04-23 19:57:27.461407 Sphinx-7.0.0/sphinx/themes/pyramid/static/ie6.css
--rw-r--r--   0        0        0      101 2023-04-23 19:57:27.462407 Sphinx-7.0.0/sphinx/themes/pyramid/static/middlebg.png
--rw-r--r--   0        0        0     6301 2023-04-23 19:57:27.462407 Sphinx-7.0.0/sphinx/themes/pyramid/static/pyramid.css_t
--rw-r--r--   0        0        0       49 2023-04-23 19:57:27.462407 Sphinx-7.0.0/sphinx/themes/pyramid/static/transparent.gif
--rw-r--r--   0        0        0      102 2023-04-23 19:57:27.462407 Sphinx-7.0.0/sphinx/themes/pyramid/theme.conf
--rw-r--r--   0        0        0     5775 2023-04-23 19:57:27.462407 Sphinx-7.0.0/sphinx/themes/scrolls/artwork/logo.svg
--rw-r--r--   0        0        0     1661 2023-04-23 19:57:27.463407 Sphinx-7.0.0/sphinx/themes/scrolls/layout.html
--rw-r--r--   0        0        0    25238 2023-04-23 19:57:27.463407 Sphinx-7.0.0/sphinx/themes/scrolls/static/darkmetal.png
--rw-r--r--   0        0        0      172 2023-04-23 19:57:27.463407 Sphinx-7.0.0/sphinx/themes/scrolls/static/headerbg.png
--rw-r--r--   0        0        0     8305 2023-04-23 19:57:27.463407 Sphinx-7.0.0/sphinx/themes/scrolls/static/logo.png
--rw-r--r--   0        0        0     7547 2023-04-23 19:57:27.463407 Sphinx-7.0.0/sphinx/themes/scrolls/static/metal.png
--rw-r--r--   0        0        0      124 2023-04-23 19:57:27.464407 Sphinx-7.0.0/sphinx/themes/scrolls/static/navigation.png
--rw-r--r--   0        0        0      303 2023-04-23 19:57:27.464407 Sphinx-7.0.0/sphinx/themes/scrolls/static/print.css
--rw-r--r--   0        0        0     7977 2023-04-23 19:57:27.464407 Sphinx-7.0.0/sphinx/themes/scrolls/static/scrolls.css_t
--rw-r--r--   0        0        0      527 2023-04-23 19:57:27.464407 Sphinx-7.0.0/sphinx/themes/scrolls/static/theme_extras.js
--rw-r--r--   0        0        0    44483 2023-04-23 19:57:27.465407 Sphinx-7.0.0/sphinx/themes/scrolls/static/watermark.png
--rw-r--r--   0        0        0     8049 2023-04-23 19:57:27.465407 Sphinx-7.0.0/sphinx/themes/scrolls/static/watermark_blur.png
--rw-r--r--   0        0        0      260 2023-04-23 19:57:27.465407 Sphinx-7.0.0/sphinx/themes/scrolls/theme.conf
--rw-r--r--   0        0        0      107 2023-04-23 19:57:27.465407 Sphinx-7.0.0/sphinx/themes/sphinxdoc/static/contents.png
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.465407 Sphinx-7.0.0/sphinx/themes/sphinxdoc/static/navigation.png
--rw-r--r--   0        0        0     6314 2023-04-23 19:57:27.465407 Sphinx-7.0.0/sphinx/themes/sphinxdoc/static/sphinxdoc.css_t
--rw-r--r--   0        0        0       77 2023-04-23 19:57:27.466407 Sphinx-7.0.0/sphinx/themes/sphinxdoc/theme.conf
--rw-r--r--   0        0        0    12162 2023-04-23 19:57:27.466407 Sphinx-7.0.0/sphinx/themes/traditional/static/traditional.css_t
--rw-r--r--   0        0        0      105 2023-04-23 19:57:27.466407 Sphinx-7.0.0/sphinx/themes/traditional/theme.conf
--rw-r--r--   0        0        0     7937 2023-04-23 19:57:27.466407 Sphinx-7.0.0/sphinx/theming.py
--rw-r--r--   0        0        0    14420 2023-04-23 19:57:27.467407 Sphinx-7.0.0/sphinx/transforms/__init__.py
--rw-r--r--   0        0        0     2768 2023-04-23 19:57:27.467407 Sphinx-7.0.0/sphinx/transforms/compact_bullet_list.py
--rw-r--r--   0        0        0    23400 2023-04-23 19:57:27.467407 Sphinx-7.0.0/sphinx/transforms/i18n.py
--rw-r--r--   0        0        0    12011 2023-04-23 19:57:27.467407 Sphinx-7.0.0/sphinx/transforms/post_transforms/__init__.py
--rw-r--r--   0        0        0     4486 2023-04-23 19:57:27.468408 Sphinx-7.0.0/sphinx/transforms/post_transforms/code.py
--rw-r--r--   0        0        0    10043 2023-04-23 19:57:27.468408 Sphinx-7.0.0/sphinx/transforms/post_transforms/images.py
--rw-r--r--   0        0        0     1361 2023-04-23 19:57:27.468408 Sphinx-7.0.0/sphinx/transforms/references.py
--rw-r--r--   0        0        0    12535 2023-04-27 14:47:43.282341 Sphinx-7.0.0/sphinx/util/__init__.py
--rw-r--r--   0        0        0      240 2023-04-23 19:57:27.468408 Sphinx-7.0.0/sphinx/util/build_phase.py
--rw-r--r--   0        0        0    15290 2023-04-23 19:57:27.469407 Sphinx-7.0.0/sphinx/util/cfamily.py
--rw-r--r--   0        0        0     3218 2023-04-23 19:57:27.469407 Sphinx-7.0.0/sphinx/util/console.py
--rw-r--r--   0        0        0     2281 2023-04-23 19:57:27.469407 Sphinx-7.0.0/sphinx/util/display.py
--rw-r--r--   0        0        0    16330 2023-04-23 19:57:27.469407 Sphinx-7.0.0/sphinx/util/docfields.py
--rw-r--r--   0        0        0     2930 2023-04-23 19:57:27.470407 Sphinx-7.0.0/sphinx/util/docstrings.py
--rw-r--r--   0        0        0    22713 2023-04-28 09:03:22.692472 Sphinx-7.0.0/sphinx/util/docutils.py
--rw-r--r--   0        0        0     1960 2023-04-23 19:57:27.470407 Sphinx-7.0.0/sphinx/util/exceptions.py
--rw-r--r--   0        0        0     3722 2023-04-23 19:57:27.470407 Sphinx-7.0.0/sphinx/util/fileutil.py
--rw-r--r--   0        0        0      513 2023-04-23 19:57:27.470407 Sphinx-7.0.0/sphinx/util/http_date.py
--rw-r--r--   0        0        0     9598 2023-04-27 00:28:57.465794 Sphinx-7.0.0/sphinx/util/i18n.py
--rw-r--r--   0        0        0     3451 2023-04-23 19:57:27.471407 Sphinx-7.0.0/sphinx/util/images.py
--rw-r--r--   0        0        0    28244 2023-04-23 19:57:27.471407 Sphinx-7.0.0/sphinx/util/inspect.py
--rw-r--r--   0        0        0     6311 2023-04-23 19:57:27.472407 Sphinx-7.0.0/sphinx/util/inventory.py
--rw-r--r--   0        0        0    18103 2023-04-23 19:57:27.472407 Sphinx-7.0.0/sphinx/util/logging.py
--rw-r--r--   0        0        0     5274 2023-04-23 19:57:27.472407 Sphinx-7.0.0/sphinx/util/matching.py
--rw-r--r--   0        0        0     1816 2023-04-23 19:57:27.473407 Sphinx-7.0.0/sphinx/util/math.py
--rw-r--r--   0        0        0    22872 2023-04-23 19:57:27.473407 Sphinx-7.0.0/sphinx/util/nodes.py
--rw-r--r--   0        0        0     6973 2023-04-23 19:57:27.473407 Sphinx-7.0.0/sphinx/util/osutil.py
--rw-r--r--   0        0        0     5023 2023-04-23 19:57:27.473407 Sphinx-7.0.0/sphinx/util/parallel.py
--rw-r--r--   0        0        0     1445 2023-04-23 19:57:27.474408 Sphinx-7.0.0/sphinx/util/png.py
--rw-r--r--   0        0        0     2870 2023-04-23 19:57:27.474408 Sphinx-7.0.0/sphinx/util/requests.py
--rw-r--r--   0        0        0     3330 2023-04-23 19:57:27.474408 Sphinx-7.0.0/sphinx/util/rst.py
--rw-r--r--   0        0        0     2651 2023-04-23 19:57:27.475407 Sphinx-7.0.0/sphinx/util/tags.py
--rw-r--r--   0        0        0     4691 2023-04-23 19:57:27.475407 Sphinx-7.0.0/sphinx/util/template.py
--rw-r--r--   0        0        0     5442 2023-04-23 19:57:27.475407 Sphinx-7.0.0/sphinx/util/texescape.py
--rw-r--r--   0        0        0    14984 2023-04-23 19:57:27.475407 Sphinx-7.0.0/sphinx/util/typing.py
--rw-r--r--   0        0        0     5801 2023-04-23 19:57:27.475407 Sphinx-7.0.0/sphinx/versioning.py
--rw-r--r--   0        0        0       31 2023-04-23 19:57:27.476407 Sphinx-7.0.0/sphinx/writers/__init__.py
--rw-r--r--   0        0        0     1605 2023-04-28 10:59:41.037038 Sphinx-7.0.0/sphinx/writers/html.py
--rw-r--r--   0        0        0    31991 2023-04-23 19:57:27.477407 Sphinx-7.0.0/sphinx/writers/html5.py
--rw-r--r--   0        0        0    84706 2023-04-28 09:42:17.461902 Sphinx-7.0.0/sphinx/writers/latex.py
--rw-r--r--   0        0        0    15475 2023-04-23 19:57:27.478407 Sphinx-7.0.0/sphinx/writers/manpage.py
--rw-r--r--   0        0        0    52823 2023-04-23 19:57:27.478407 Sphinx-7.0.0/sphinx/writers/texinfo.py
--rw-r--r--   0        0        0    37916 2023-04-23 19:57:27.479408 Sphinx-7.0.0/sphinx/writers/text.py
--rw-r--r--   0        0        0     1457 2023-04-23 19:57:27.479408 Sphinx-7.0.0/sphinx/writers/xml.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.479408 Sphinx-7.0.0/tests/__init__.py
--rw-r--r--   0        0        0     3054 2023-04-23 19:57:27.479408 Sphinx-7.0.0/tests/certs/cert.pem
--rw-r--r--   0        0        0     1574 2023-04-23 19:57:27.480407 Sphinx-7.0.0/tests/conftest.py
--rw-r--r--   0        0        0      363 2023-04-23 19:57:27.480407 Sphinx-7.0.0/tests/ext_napoleon_pep526_data_google.py
--rw-r--r--   0        0        0      385 2023-04-23 19:57:27.480407 Sphinx-7.0.0/tests/ext_napoleon_pep526_data_numpy.py
--rw-r--r--   0        0        0       34 2023-04-23 19:57:27.480407 Sphinx-7.0.0/tests/js/documentation_options.js
--rw-r--r--   0        0        0     1694 2023-04-23 19:57:27.480407 Sphinx-7.0.0/tests/js/searchtools.js
--rw-r--r--   0        0        0     1985 2023-04-23 19:57:27.481407 Sphinx-7.0.0/tests/js/sphinx_highlight.js
--rw-r--r--   0        0        0      111 2023-04-23 19:57:27.481407 Sphinx-7.0.0/tests/roots/test-add_enumerable_node/conf.py
--rw-r--r--   0        0        0     1464 2023-04-23 19:57:27.481407 Sphinx-7.0.0/tests/roots/test-add_enumerable_node/enumerable_node.py
--rw-r--r--   0        0        0      763 2023-04-23 19:57:27.481407 Sphinx-7.0.0/tests/roots/test-add_enumerable_node/index.rst
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.481407 Sphinx-7.0.0/tests/roots/test-add_enumerable_node/rimg.png
--rw-r--r--   0        0        0      277 2023-04-23 19:57:27.481407 Sphinx-7.0.0/tests/roots/test-add_source_parser-conflicts-with-users-setting/conf.py
--rw-r--r--   0        0        0      201 2023-04-23 19:57:27.482407 Sphinx-7.0.0/tests/roots/test-add_source_parser-conflicts-with-users-setting/source_parser.py
--rw-r--r--   0        0        0      121 2023-04-23 19:57:27.482407 Sphinx-7.0.0/tests/roots/test-add_source_parser/conf.py
--rw-r--r--   0        0        0      201 2023-04-23 19:57:27.482407 Sphinx-7.0.0/tests/roots/test-add_source_parser/source_parser.py
--rw-r--r--   0        0        0     1659 2023-04-23 19:57:27.482407 Sphinx-7.0.0/tests/roots/test-api-set-translator/conf.py
--rw-r--r--   0        0        0       72 2023-04-23 19:57:27.482407 Sphinx-7.0.0/tests/roots/test-api-set-translator/index.rst
--rw-r--r--   0        0        0       98 2023-04-23 19:57:27.483407 Sphinx-7.0.0/tests/roots/test-api-set-translator/nonext/conf.py
--rw-r--r--   0        0        0      101 2023-04-23 19:57:27.483407 Sphinx-7.0.0/tests/roots/test-api-set-translator/translator.py
--rw-r--r--   0        0        0        0 2023-04-25 10:59:46.881271 Sphinx-7.0.0/tests/roots/test-apidoc-duplicates/fish_licence/halibut.cpython-38-x86_64-linux-gnu.so
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.483407 Sphinx-7.0.0/tests/roots/test-apidoc-duplicates/fish_licence/halibut.pyx
--rw-r--r--   0        0        0       12 2023-04-23 19:57:27.484407 Sphinx-7.0.0/tests/roots/test-apidoc-pep420/a/b/c/__init__.py
--rw-r--r--   0        0        0       11 2023-04-23 19:57:27.484407 Sphinx-7.0.0/tests/roots/test-apidoc-pep420/a/b/c/d.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.484407 Sphinx-7.0.0/tests/roots/test-apidoc-pep420/a/b/e/__init__.py
--rw-r--r--   0        0        0       11 2023-04-23 19:57:27.484407 Sphinx-7.0.0/tests/roots/test-apidoc-pep420/a/b/e/f.py
--rw-r--r--   0        0        0       11 2023-04-23 19:57:27.484407 Sphinx-7.0.0/tests/roots/test-apidoc-pep420/a/b/x/y.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.484407 Sphinx-7.0.0/tests/roots/test-apidoc-subpackage-in-toc/parent/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.485407 Sphinx-7.0.0/tests/roots/test-apidoc-subpackage-in-toc/parent/child/__init__.py
--rw-r--r--   0        0        0        6 2023-04-23 19:57:27.485407 Sphinx-7.0.0/tests/roots/test-apidoc-subpackage-in-toc/parent/child/foo.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.485407 Sphinx-7.0.0/tests/roots/test-apidoc-toc/mypackage/__init__.py
--rw-r--r--   0        0        0      404 2023-04-25 10:59:46.885153 Sphinx-7.0.0/tests/roots/test-apidoc-toc/mypackage/main.py
--rw-r--r--   0        0        0       79 2023-04-23 19:57:27.485407 Sphinx-7.0.0/tests/roots/test-apidoc-toc/mypackage/no_init/foo.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.485407 Sphinx-7.0.0/tests/roots/test-apidoc-toc/mypackage/resource/__init__.py
--rw-r--r--   0        0        0       96 2023-04-23 19:57:27.486407 Sphinx-7.0.0/tests/roots/test-apidoc-toc/mypackage/resource/resource.txt
--rw-r--r--   0        0        0       23 2023-04-23 19:57:27.486407 Sphinx-7.0.0/tests/roots/test-apidoc-toc/mypackage/something/__init__.py
--rw-r--r--   0        0        0       44 2023-04-23 19:57:27.486407 Sphinx-7.0.0/tests/roots/test-apidoc-trailing-underscore/package_/__init__.py
--rw-r--r--   0        0        0      215 2023-04-23 19:57:27.486407 Sphinx-7.0.0/tests/roots/test-apidoc-trailing-underscore/package_/module_.py
--rw-r--r--   0        0        0      221 2023-04-23 19:57:27.486407 Sphinx-7.0.0/tests/roots/test-autosummary/conf.py
--rw-r--r--   0        0        0     1335 2023-04-23 19:57:27.487407 Sphinx-7.0.0/tests/roots/test-autosummary/dummy_module.py
--rw-r--r--   0        0        0       98 2023-04-23 19:57:27.487407 Sphinx-7.0.0/tests/roots/test-autosummary/index.rst
--rw-r--r--   0        0        0      507 2023-04-23 19:57:27.487407 Sphinx-7.0.0/tests/roots/test-autosummary/sphinx.rst
--rw-r--r--   0        0        0      198 2023-04-23 19:57:27.487407 Sphinx-7.0.0/tests/roots/test-autosummary/underscore_module_.py
--rw-r--r--   0        0        0      114 2023-04-23 19:57:27.487407 Sphinx-7.0.0/tests/roots/test-basic/conf.py
--rw-r--r--   0        0        0     1477 2023-04-27 00:31:27.920451 Sphinx-7.0.0/tests/roots/test-basic/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.488407 Sphinx-7.0.0/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/_static/extra.css
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.488407 Sphinx-7.0.0/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/_static/mytheme.css
--rw-r--r--   0        0        0       60 2023-04-23 19:57:27.488407 Sphinx-7.0.0/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/theme.conf
--rw-r--r--   0        0        0       53 2023-04-23 19:57:27.488407 Sphinx-7.0.0/tests/roots/test-build-html-theme-having-multiple-stylesheets/conf.py
--rw-r--r--   0        0        0      100 2023-04-23 19:57:27.488407 Sphinx-7.0.0/tests/roots/test-build-html-theme-having-multiple-stylesheets/index.rst
--rw-r--r--   0        0        0      372 2023-04-23 19:57:27.488407 Sphinx-7.0.0/tests/roots/test-build-html-translator/conf.py
--rw-r--r--   0        0        0      252 2023-04-23 19:57:27.489407 Sphinx-7.0.0/tests/roots/test-build-html-translator/index.rst
--rw-r--r--   0        0        0       53 2023-04-23 19:57:27.489407 Sphinx-7.0.0/tests/roots/test-build-text/conf.py
--rw-r--r--   0        0        0       20 2023-04-23 19:57:27.489407 Sphinx-7.0.0/tests/roots/test-build-text/doc1.txt
--rw-r--r--   0        0        0       51 2023-04-23 19:57:27.489407 Sphinx-7.0.0/tests/roots/test-build-text/doc2.txt
--rw-r--r--   0        0        0      135 2023-04-23 19:57:27.489407 Sphinx-7.0.0/tests/roots/test-build-text/index.txt
--rw-r--r--   0        0        0       62 2023-04-23 19:57:27.489407 Sphinx-7.0.0/tests/roots/test-build-text/lineblock.txt
--rw-r--r--   0        0        0       40 2023-04-23 19:57:27.489407 Sphinx-7.0.0/tests/roots/test-build-text/listitems.txt
--rw-r--r--   0        0        0      388 2023-04-23 19:57:27.489407 Sphinx-7.0.0/tests/roots/test-build-text/maxwidth.txt
--rw-r--r--   0        0        0      478 2023-04-23 19:57:27.490407 Sphinx-7.0.0/tests/roots/test-build-text/nonascii_maxwidth.txt
--rw-r--r--   0        0        0       75 2023-04-23 19:57:27.490407 Sphinx-7.0.0/tests/roots/test-build-text/nonascii_table.txt
--rw-r--r--   0        0        0       17 2023-04-23 19:57:27.490407 Sphinx-7.0.0/tests/roots/test-build-text/nonascii_title.txt
--rw-r--r--   0        0        0       98 2023-04-23 19:57:27.490407 Sphinx-7.0.0/tests/roots/test-build-text/table.txt
--rw-r--r--   0        0        0       98 2023-04-23 19:57:27.490407 Sphinx-7.0.0/tests/roots/test-build-text/table_colspan.txt
--rw-r--r--   0        0        0      140 2023-04-23 19:57:27.490407 Sphinx-7.0.0/tests/roots/test-build-text/table_colspan_and_rowspan.txt
--rw-r--r--   0        0        0       98 2023-04-23 19:57:27.490407 Sphinx-7.0.0/tests/roots/test-build-text/table_colspan_left.txt
--rw-r--r--   0        0        0       98 2023-04-23 19:57:27.490407 Sphinx-7.0.0/tests/roots/test-build-text/table_rowspan.txt
--rw-r--r--   0        0        0       18 2023-04-23 19:57:27.491407 Sphinx-7.0.0/tests/roots/test-builder-dirhtml/bar.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.491407 Sphinx-7.0.0/tests/roots/test-builder-dirhtml/conf.py
--rw-r--r--   0        0        0       32 2023-04-23 19:57:27.491407 Sphinx-7.0.0/tests/roots/test-builder-dirhtml/foo/foo_1.rst
--rw-r--r--   0        0        0       32 2023-04-23 19:57:27.491407 Sphinx-7.0.0/tests/roots/test-builder-dirhtml/foo/foo_2.rst
--rw-r--r--   0        0        0       63 2023-04-23 19:57:27.491407 Sphinx-7.0.0/tests/roots/test-builder-dirhtml/foo/index.rst
--rw-r--r--   0        0        0       59 2023-04-23 19:57:27.491407 Sphinx-7.0.0/tests/roots/test-builder-dirhtml/index.rst
--rw-r--r--   0        0        0       74 2023-04-23 19:57:27.491407 Sphinx-7.0.0/tests/roots/test-builder-gettext-dont-rebuild-mo/bom.rst
--rw-r--r--   0        0        0       16 2023-04-23 19:57:27.492406 Sphinx-7.0.0/tests/roots/test-builder-gettext-dont-rebuild-mo/conf.py
--rw-r--r--   0        0        0      108 2023-04-23 19:57:27.492406 Sphinx-7.0.0/tests/roots/test-builder-gettext-dont-rebuild-mo/index.rst
--rw-r--r--   0        0        0      264 2023-04-23 19:57:27.492406 Sphinx-7.0.0/tests/roots/test-builder-gettext-dont-rebuild-mo/xx/LC_MESSAGES/bom.po
--rw-r--r--   0        0        0      330 2023-04-23 19:57:27.492406 Sphinx-7.0.0/tests/roots/test-changes/base.rst
--rw-r--r--   0        0        0      371 2023-04-23 19:57:27.492406 Sphinx-7.0.0/tests/roots/test-changes/c-api.rst
--rw-r--r--   0        0        0      134 2023-04-23 19:57:27.492406 Sphinx-7.0.0/tests/roots/test-changes/conf.py
--rw-r--r--   0        0        0      189 2023-04-23 19:57:27.493407 Sphinx-7.0.0/tests/roots/test-changes/contents.rst
--rw-r--r--   0        0        0      443 2023-04-23 19:57:27.493407 Sphinx-7.0.0/tests/roots/test-changes/library/utils.rst
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.493407 Sphinx-7.0.0/tests/roots/test-circular/conf.py
--rw-r--r--   0        0        0       22 2023-04-23 19:57:27.493407 Sphinx-7.0.0/tests/roots/test-circular/index.rst
--rw-r--r--   0        0        0       23 2023-04-23 19:57:27.493407 Sphinx-7.0.0/tests/roots/test-circular/sub.rst
--rw-r--r--   0        0        0       81 2023-04-23 19:57:27.494407 Sphinx-7.0.0/tests/roots/test-config/conf.py
--rw-r--r--   0        0        0       32 2023-04-23 19:57:27.494407 Sphinx-7.0.0/tests/roots/test-correct-year/conf.py
--rw-r--r--   0        0        0       55 2023-04-23 19:57:27.494407 Sphinx-7.0.0/tests/roots/test-correct-year/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.494407 Sphinx-7.0.0/tests/roots/test-default_role/conf.py
--rw-r--r--   0        0        0       29 2023-04-23 19:57:27.494407 Sphinx-7.0.0/tests/roots/test-default_role/foo.rst
--rw-r--r--   0        0        0       54 2023-04-23 19:57:27.494407 Sphinx-7.0.0/tests/roots/test-default_role/index.rst
--rw-r--r--   0        0        0      762 2023-04-23 19:57:27.495407 Sphinx-7.0.0/tests/roots/test-directive-code/caption.rst
--rw-r--r--   0        0        0      263 2023-04-23 19:57:27.495407 Sphinx-7.0.0/tests/roots/test-directive-code/classes.rst
--rw-r--r--   0        0        0       44 2023-04-23 19:57:27.495407 Sphinx-7.0.0/tests/roots/test-directive-code/conf.py
--rw-r--r--   0        0        0     1434 2023-04-23 19:57:27.495407 Sphinx-7.0.0/tests/roots/test-directive-code/dedent.rst
--rw-r--r--   0        0        0      170 2023-04-23 19:57:27.495407 Sphinx-7.0.0/tests/roots/test-directive-code/emphasize.rst
--rw-r--r--   0        0        0        3 2023-04-23 19:57:27.495407 Sphinx-7.0.0/tests/roots/test-directive-code/empty.inc
--rw-r--r--   0        0        0       21 2023-04-23 19:57:27.496407 Sphinx-7.0.0/tests/roots/test-directive-code/error.inc
--rw-r--r--   0        0        0      203 2023-04-23 19:57:27.496407 Sphinx-7.0.0/tests/roots/test-directive-code/force.rst
--rw-r--r--   0        0        0      345 2023-04-23 19:57:27.496407 Sphinx-7.0.0/tests/roots/test-directive-code/highlight.rst
--rw-r--r--   0        0        0      267 2023-04-23 19:57:27.496407 Sphinx-7.0.0/tests/roots/test-directive-code/index.rst
--rw-r--r--   0        0        0      349 2023-04-23 19:57:27.496407 Sphinx-7.0.0/tests/roots/test-directive-code/linenos.rst
--rw-r--r--   0        0        0      396 2023-04-23 19:57:27.496407 Sphinx-7.0.0/tests/roots/test-directive-code/linenothreshold.rst
--rw-r--r--   0        0        0      206 2023-04-23 19:57:27.497407 Sphinx-7.0.0/tests/roots/test-directive-code/literal-diff.inc
--rw-r--r--   0        0        0       67 2023-04-23 19:57:27.497407 Sphinx-7.0.0/tests/roots/test-directive-code/literal-short.inc
--rw-r--r--   0        0        0      213 2023-04-23 19:57:27.497407 Sphinx-7.0.0/tests/roots/test-directive-code/literal.inc
--rw-r--r--   0        0        0      421 2023-04-23 19:57:27.497407 Sphinx-7.0.0/tests/roots/test-directive-code/namedblocks.rst
--rw-r--r--   0        0        0      263 2023-04-23 19:57:27.497407 Sphinx-7.0.0/tests/roots/test-directive-code/py-decorators.inc
--rw-r--r--   0        0        0      391 2023-04-23 19:57:27.497407 Sphinx-7.0.0/tests/roots/test-directive-code/py-decorators.rst
--rw-r--r--   0        0        0      305 2023-04-25 10:59:46.885153 Sphinx-7.0.0/tests/roots/test-directive-code/python.rst
--rw-r--r--   0        0        0      355 2023-04-23 19:57:27.497407 Sphinx-7.0.0/tests/roots/test-directive-code/target.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.497407 Sphinx-7.0.0/tests/roots/test-directive-csv-table/conf.py
--rw-r--r--   0        0        0       12 2023-04-23 19:57:27.498407 Sphinx-7.0.0/tests/roots/test-directive-csv-table/example.csv
--rw-r--r--   0        0        0       12 2023-04-23 19:57:27.498407 Sphinx-7.0.0/tests/roots/test-directive-csv-table/subdir/example.csv
--rw-r--r--   0        0        0       62 2023-04-23 19:57:27.498407 Sphinx-7.0.0/tests/roots/test-directive-only/conf.py
--rw-r--r--   0        0        0       63 2023-04-23 19:57:27.498407 Sphinx-7.0.0/tests/roots/test-directive-only/index.rst
--rw-r--r--   0        0        0     3063 2023-04-23 19:57:27.498407 Sphinx-7.0.0/tests/roots/test-directive-only/only.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.498407 Sphinx-7.0.0/tests/roots/test-directives-raw/conf.py
--rw-r--r--   0        0        0      404 2023-04-23 19:57:27.499407 Sphinx-7.0.0/tests/roots/test-directives-raw/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.499407 Sphinx-7.0.0/tests/roots/test-docutilsconf/conf.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.499407 Sphinx-7.0.0/tests/roots/test-docutilsconf/docutils.conf
--rw-r--r--   0        0        0       89 2023-04-23 19:57:27.499407 Sphinx-7.0.0/tests/roots/test-docutilsconf/index.rst
--rw-r--r--   0        0        0       74 2023-04-23 19:57:27.499407 Sphinx-7.0.0/tests/roots/test-domain-c-intersphinx/conf.py
--rw-r--r--   0        0        0     1146 2023-04-23 19:57:27.499407 Sphinx-7.0.0/tests/roots/test-domain-c-intersphinx/index.rst
--rw-r--r--   0        0        0      121 2023-04-23 19:57:27.499407 Sphinx-7.0.0/tests/roots/test-domain-c/anon-dup-decl.rst
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.500407 Sphinx-7.0.0/tests/roots/test-domain-c/conf.py
--rw-r--r--   0        0        0       70 2023-04-23 19:57:27.500407 Sphinx-7.0.0/tests/roots/test-domain-c/field-role.rst
--rw-r--r--   0        0        0      101 2023-04-23 19:57:27.500407 Sphinx-7.0.0/tests/roots/test-domain-c/function_param_target.rst
--rw-r--r--   0        0        0      785 2023-04-23 19:57:27.500407 Sphinx-7.0.0/tests/roots/test-domain-c/index.rst
--rw-r--r--   0        0        0      261 2023-04-23 19:57:27.500407 Sphinx-7.0.0/tests/roots/test-domain-c/namespace.rst
--rw-r--r--   0        0        0      163 2023-04-23 19:57:27.500407 Sphinx-7.0.0/tests/roots/test-domain-c/ns_lookup.rst
--rw-r--r--   0        0        0       74 2023-04-23 19:57:27.501407 Sphinx-7.0.0/tests/roots/test-domain-cpp-intersphinx/conf.py
--rw-r--r--   0        0        0     2444 2023-04-23 19:57:27.501407 Sphinx-7.0.0/tests/roots/test-domain-cpp-intersphinx/index.rst
--rw-r--r--   0        0        0       92 2023-04-23 19:57:27.501407 Sphinx-7.0.0/tests/roots/test-domain-cpp/anon-dup-decl.rst
--rw-r--r--   0        0        0      688 2023-04-23 19:57:27.501407 Sphinx-7.0.0/tests/roots/test-domain-cpp/any-role.rst
--rw-r--r--   0        0        0       27 2023-04-23 19:57:27.501407 Sphinx-7.0.0/tests/roots/test-domain-cpp/backslash.rst
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.501407 Sphinx-7.0.0/tests/roots/test-domain-cpp/conf.py
--rw-r--r--   0        0        0       59 2023-04-23 19:57:27.501407 Sphinx-7.0.0/tests/roots/test-domain-cpp/field-role.rst
--rw-r--r--   0        0        0     1136 2023-04-23 19:57:27.501407 Sphinx-7.0.0/tests/roots/test-domain-cpp/index.rst
--rw-r--r--   0        0        0      133 2023-04-23 19:57:27.502406 Sphinx-7.0.0/tests/roots/test-domain-cpp/lookup-key-overload.rst
--rw-r--r--   0        0        0      437 2023-04-23 19:57:27.502406 Sphinx-7.0.0/tests/roots/test-domain-cpp/multi-decl-lookup.rst
--rw-r--r--   0        0        0     2136 2023-04-23 19:57:27.502406 Sphinx-7.0.0/tests/roots/test-domain-cpp/roles-targets-ok.rst
--rw-r--r--   0        0        0     2406 2023-04-23 19:57:27.502406 Sphinx-7.0.0/tests/roots/test-domain-cpp/roles-targets-warn.rst
--rw-r--r--   0        0        0      697 2023-04-23 19:57:27.502406 Sphinx-7.0.0/tests/roots/test-domain-cpp/roles.rst
--rw-r--r--   0        0        0       90 2023-04-23 19:57:27.502406 Sphinx-7.0.0/tests/roots/test-domain-cpp/roles2.rst
--rw-r--r--   0        0        0      383 2023-04-23 19:57:27.502406 Sphinx-7.0.0/tests/roots/test-domain-cpp/semicolon.rst
--rw-r--r--   0        0        0      203 2023-04-23 19:57:27.503407 Sphinx-7.0.0/tests/roots/test-domain-cpp/warn-template-param-qualified-name.rst
--rw-r--r--   0        0        0      249 2023-04-23 19:57:27.503407 Sphinx-7.0.0/tests/roots/test-domain-cpp/xref_consistency.rst
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.503407 Sphinx-7.0.0/tests/roots/test-domain-js/conf.py
--rw-r--r--   0        0        0       66 2023-04-23 19:57:27.503407 Sphinx-7.0.0/tests/roots/test-domain-js/index.rst
--rw-r--r--   0        0        0      527 2023-04-23 19:57:27.503407 Sphinx-7.0.0/tests/roots/test-domain-js/module.rst
--rw-r--r--   0        0        0      886 2023-04-23 19:57:27.503407 Sphinx-7.0.0/tests/roots/test-domain-js/roles.rst
--rw-r--r--   0        0        0       41 2023-04-23 19:57:27.503407 Sphinx-7.0.0/tests/roots/test-domain-py-python_use_unqualified_type_names/conf.py
--rw-r--r--   0        0        0      240 2023-04-23 19:57:27.504407 Sphinx-7.0.0/tests/roots/test-domain-py-python_use_unqualified_type_names/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.504407 Sphinx-7.0.0/tests/roots/test-domain-py-xref-warning/conf.py
--rw-r--r--   0        0        0      116 2023-04-23 19:57:27.504407 Sphinx-7.0.0/tests/roots/test-domain-py-xref-warning/index.rst
--rw-r--r--   0        0        0      359 2023-04-23 19:57:27.504407 Sphinx-7.0.0/tests/roots/test-domain-py/abbr.rst
--rw-r--r--   0        0        0      174 2023-04-23 19:57:27.504407 Sphinx-7.0.0/tests/roots/test-domain-py/canonical.rst
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.504407 Sphinx-7.0.0/tests/roots/test-domain-py/conf.py
--rw-r--r--   0        0        0      107 2023-04-23 19:57:27.504407 Sphinx-7.0.0/tests/roots/test-domain-py/index.rst
--rw-r--r--   0        0        0     1040 2023-04-23 19:57:27.505407 Sphinx-7.0.0/tests/roots/test-domain-py/module.rst
--rw-r--r--   0        0        0      383 2023-04-23 19:57:27.505407 Sphinx-7.0.0/tests/roots/test-domain-py/module_option.rst
--rw-r--r--   0        0        0      872 2023-04-23 19:57:27.505407 Sphinx-7.0.0/tests/roots/test-domain-py/roles.rst
--rw-r--r--   0        0        0       24 2023-04-23 19:57:27.505407 Sphinx-7.0.0/tests/roots/test-double-inheriting-theme/base_themes_dir/base_theme1/theme.conf
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.505407 Sphinx-7.0.0/tests/roots/test-double-inheriting-theme/base_themes_dir/base_theme2/theme.conf
--rw-r--r--   0        0        0      127 2023-04-23 19:57:27.506407 Sphinx-7.0.0/tests/roots/test-double-inheriting-theme/conf.py
--rw-r--r--   0        0        0       87 2023-04-23 19:57:27.506407 Sphinx-7.0.0/tests/roots/test-double-inheriting-theme/index.rst
--rw-r--r--   0        0        0       40 2023-04-23 19:57:27.506407 Sphinx-7.0.0/tests/roots/test-environment-record-dependencies/api.rst
--rw-r--r--   0        0        0       99 2023-04-23 19:57:27.506407 Sphinx-7.0.0/tests/roots/test-environment-record-dependencies/conf.py
--rw-r--r--   0        0        0       38 2023-04-23 19:57:27.506407 Sphinx-7.0.0/tests/roots/test-environment-record-dependencies/example_module.py
--rw-r--r--   0        0        0       22 2023-04-23 19:57:27.506407 Sphinx-7.0.0/tests/roots/test-environment-record-dependencies/index.rst
--rw-r--r--   0        0        0       87 2023-04-23 19:57:27.507407 Sphinx-7.0.0/tests/roots/test-epub-anchor-id/conf.py
--rw-r--r--   0        0        0      191 2023-04-23 19:57:27.507407 Sphinx-7.0.0/tests/roots/test-epub-anchor-id/index.rst
--rw-r--r--   0        0        0      111 2023-04-23 19:57:27.507407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/autodoc_dummy_bar.py
--rw-r--r--   0        0        0       94 2023-04-23 19:57:27.507407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/autodoc_dummy_module.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.507407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/bug2437/__init__.py
--rw-r--r--   0        0        0       47 2023-04-23 19:57:27.507407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/bug2437/autodoc_dummy_foo.py
--rw-r--r--   0        0        0      215 2023-04-23 19:57:27.507407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/conf.py
--rw-r--r--   0        0        0      282 2023-04-23 19:57:27.508406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/index.rst
--rw-r--r--   0        0        0      149 2023-04-23 19:57:27.508406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/TYPE_CHECKING.py
--rw-r--r--   0        0        0     4363 2023-04-23 19:57:27.508406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/__init__.py
--rw-r--r--   0        0        0      187 2023-04-23 19:57:27.508406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/_functions_to_import.py
--rw-r--r--   0        0        0      428 2023-04-23 19:57:27.508406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/abstractmethods.py
--rw-r--r--   0        0        0      150 2023-04-23 19:57:27.509407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/annotated.py
--rw-r--r--   0        0        0      882 2023-04-23 19:57:27.509407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/autoclass_content.py
--rw-r--r--   0        0        0      665 2023-04-23 19:57:27.509407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/autodoc_type_aliases.py
--rw-r--r--   0        0        0      107 2023-04-23 19:57:27.509407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/bound_method.py
--rw-r--r--   0        0        0      219 2023-04-23 19:57:27.510406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/cached_property.py
--rw-r--r--   0        0        0      279 2023-04-23 19:57:27.510406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/callable.py
--rw-r--r--   0        0        0       47 2023-04-23 19:57:27.510406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/canonical/__init__.py
--rw-r--r--   0        0        0      158 2023-04-23 19:57:27.510406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/canonical/original.py
--rw-r--r--   0        0        0      684 2023-04-23 19:57:27.510406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/classes.py
--rw-r--r--   0        0        0      764 2023-04-23 19:57:27.510406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/coroutine.py
--rw-r--r--   0        0        0      245 2023-04-23 19:57:27.511406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/cython.pyx
--rw-r--r--   0        0        0      766 2023-04-23 19:57:27.511406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/decorator.py
--rw-r--r--   0        0        0      683 2023-04-23 19:57:27.511406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/descriptor.py
--rw-r--r--   0        0        0      643 2023-04-23 19:57:27.511406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/docstring_signature.py
--rw-r--r--   0        0        0      150 2023-04-23 19:57:27.511406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/empty_all.py
--rw-r--r--   0        0        0      384 2023-04-23 19:57:27.511406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/enums.py
--rw-r--r--   0        0        0      227 2023-04-23 19:57:27.511406 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/final.py
--rw-r--r--   0        0        0      268 2023-04-23 19:57:27.512418 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/functions.py
--rw-r--r--   0        0        0      278 2023-04-23 19:57:27.512418 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/generic_class.py
--rw-r--r--   0        0        0      262 2023-04-23 19:57:27.512418 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/genericalias.py
--rw-r--r--   0        0        0      260 2023-04-23 19:57:27.512418 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/hide_value.py
--rw-r--r--   0        0        0       42 2023-04-23 19:57:27.512418 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/imported_members.py
--rw-r--r--   0        0        0      458 2023-04-23 19:57:27.512418 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/inheritance.py
--rw-r--r--   0        0        0      279 2023-04-23 19:57:27.512418 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/instance_variable.py
--rw-r--r--   0        0        0       52 2023-04-23 19:57:27.513407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/metadata.py
--rw-r--r--   0        0        0      422 2023-04-23 19:57:27.513407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/methods.py
--rw-r--r--   0        0        0      155 2023-04-23 19:57:27.513407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/module.py
--rw-r--r--   0        0        0       93 2023-04-23 19:57:27.513407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/name_conflict/__init__.py
--rw-r--r--   0        0        0       65 2023-04-23 19:57:27.513407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/name_conflict/foo.py
--rw-r--r--   0        0        0      169 2023-04-23 19:57:27.513407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/name_mangling.py
--rw-r--r--   0        0        0      894 2023-04-23 19:57:27.513407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/need_mocks.py
--rw-r--r--   0        0        0     1345 2023-04-23 19:57:27.514407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/overload.py
--rw-r--r--   0        0        0       59 2023-04-23 19:57:27.514407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/overload2.py
--rw-r--r--   0        0        0      207 2023-04-23 19:57:27.514407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/partialfunction.py
--rw-r--r--   0        0        0      420 2023-04-23 19:57:27.514407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/partialmethod.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.514407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/pep570.py
--rw-r--r--   0        0        0      292 2023-04-23 19:57:27.514407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/pep604.py
--rw-r--r--   0        0        0      831 2023-04-23 19:57:27.514407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/preserve_defaults.py
--rw-r--r--   0        0        0      556 2023-04-23 19:57:27.515423 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/private.py
--rw-r--r--   0        0        0       90 2023-04-23 19:57:27.515423 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/process_docstring.py
--rw-r--r--   0        0        0      407 2023-04-23 19:57:27.515423 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/properties.py
--rw-r--r--   0        0        0      705 2023-04-23 19:57:27.515423 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/singledispatch.py
--rw-r--r--   0        0        0      628 2023-04-23 19:57:27.515423 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/singledispatchmethod.py
--rw-r--r--   0        0        0      396 2023-04-23 19:57:27.515423 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/slots.py
--rw-r--r--   0        0        0      168 2023-04-23 19:57:27.515423 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/sort_by_all.py
--rw-r--r--   0        0        0      551 2023-04-23 19:57:27.516407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/typed_vars.py
--rw-r--r--   0        0        0     2107 2023-04-23 19:57:27.516407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/typehints.py
--rw-r--r--   0        0        0      461 2023-04-23 19:57:27.516407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/typevar.py
--rw-r--r--   0        0        0      123 2023-04-23 19:57:27.516407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/uninitialized_attributes.py
--rw-r--r--   0        0        0      372 2023-04-23 19:57:27.516407 Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/wrappedfunction.py
--rw-r--r--   0        0        0       85 2023-04-23 19:57:27.516407 Sphinx-7.0.0/tests/roots/test-ext-autosectionlabel-prefix-document/conf.py
--rw-r--r--   0        0        0      591 2023-04-23 19:57:27.516407 Sphinx-7.0.0/tests/roots/test-ext-autosectionlabel-prefix-document/index.rst
--rw-r--r--   0        0        0       45 2023-04-23 19:57:27.517407 Sphinx-7.0.0/tests/roots/test-ext-autosectionlabel/conf.py
--rw-r--r--   0        0        0      535 2023-04-23 19:57:27.517407 Sphinx-7.0.0/tests/roots/test-ext-autosectionlabel/index.rst
--rw-r--r--   0        0        0      294 2023-04-23 19:57:27.517407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-filename-map/autosummary_dummy_module.py
--rw-r--r--   0        0        0      255 2023-04-23 19:57:27.517407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-filename-map/conf.py
--rw-r--r--   0        0        0      198 2023-04-23 19:57:27.517407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-filename-map/index.rst
--rw-r--r--   0        0        0       47 2023-04-23 19:57:27.517407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-imported_members/autosummary_dummy_package/__init__.py
--rw-r--r--   0        0        0       85 2023-04-23 19:57:27.518406 Sphinx-7.0.0/tests/roots/test-ext-autosummary-imported_members/autosummary_dummy_package/autosummary_dummy_module.py
--rw-r--r--   0        0        0      168 2023-04-23 19:57:27.518406 Sphinx-7.0.0/tests/roots/test-ext-autosummary-imported_members/conf.py
--rw-r--r--   0        0        0      147 2023-04-23 19:57:27.518406 Sphinx-7.0.0/tests/roots/test-ext-autosummary-imported_members/index.rst
--rw-r--r--   0        0        0      171 2023-04-23 19:57:27.518406 Sphinx-7.0.0/tests/roots/test-ext-autosummary-mock_imports/conf.py
--rw-r--r--   0        0        0       72 2023-04-23 19:57:27.518406 Sphinx-7.0.0/tests/roots/test-ext-autosummary-mock_imports/foo.py
--rw-r--r--   0        0        0      117 2023-04-23 19:57:27.518406 Sphinx-7.0.0/tests/roots/test-ext-autosummary-mock_imports/index.rst
--rw-r--r--   0        0        0      241 2023-04-23 19:57:27.519407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/__init__.py
--rw-r--r--   0        0        0      201 2023-04-23 19:57:27.519407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/autosummary_dummy_module.py
--rw-r--r--   0        0        0      201 2023-04-23 19:57:27.519407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/extra_dummy_module.py
--rw-r--r--   0        0        0      170 2023-04-23 19:57:27.519407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-module_all/conf.py
--rw-r--r--   0        0        0      154 2023-04-23 19:57:27.519407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-module_all/index.rst
--rw-r--r--   0        0        0      132 2023-04-23 19:57:27.519407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-recursive/conf.py
--rw-r--r--   0        0        0      174 2023-04-23 19:57:27.519407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-recursive/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.520407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-recursive/package2/__init__.py
--rw-r--r--   0        0        0      147 2023-04-23 19:57:27.520407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-recursive/package2/module.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.519407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-recursive/package/__init__.py
--rw-r--r--   0        0        0      147 2023-04-23 19:57:27.520407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-recursive/package/module.py
--rw-r--r--   0        0        0       63 2023-04-23 19:57:27.520407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-recursive/package/module_importfail.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.520407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-recursive/package/package/__init__.py
--rw-r--r--   0        0        0      147 2023-04-23 19:57:27.520407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-recursive/package/package/module.py
--rw-r--r--   0        0        0      404 2023-04-23 19:57:27.521407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-skip-member/conf.py
--rw-r--r--   0        0        0       54 2023-04-23 19:57:27.521407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-skip-member/index.rst
--rw-r--r--   0        0        0      264 2023-04-23 19:57:27.521407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-skip-member/target.py
--rw-r--r--   0        0        0        6 2023-04-23 19:57:27.521407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-template/_templates/empty.rst
--rw-r--r--   0        0        0      209 2023-04-23 19:57:27.521407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-template/conf.py
--rw-r--r--   0        0        0       78 2023-04-23 19:57:27.521407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-template/index.rst
--rw-r--r--   0        0        0       39 2023-04-23 19:57:27.521407 Sphinx-7.0.0/tests/roots/test-ext-autosummary-template/target.py
--rw-r--r--   0        0        0       22 2023-04-23 19:57:27.522407 Sphinx-7.0.0/tests/roots/test-ext-autosummary/autosummary_class_module.py
--rw-r--r--   0        0        0      232 2023-04-23 19:57:27.522407 Sphinx-7.0.0/tests/roots/test-ext-autosummary/autosummary_dummy_inherited_module.py
--rw-r--r--   0        0        0      932 2023-04-23 19:57:27.522407 Sphinx-7.0.0/tests/roots/test-ext-autosummary/autosummary_dummy_module.py
--rw-r--r--   0        0        0       63 2023-04-23 19:57:27.522407 Sphinx-7.0.0/tests/roots/test-ext-autosummary/autosummary_importfail.py
--rw-r--r--   0        0        0      190 2023-04-23 19:57:27.522407 Sphinx-7.0.0/tests/roots/test-ext-autosummary/conf.py
--rw-r--r--   0        0        0      499 2023-04-23 19:57:27.522407 Sphinx-7.0.0/tests/roots/test-ext-autosummary/index.rst
--rw-r--r--   0        0        0      242 2023-04-23 19:57:27.523407 Sphinx-7.0.0/tests/roots/test-ext-coverage/conf.py
--rw-r--r--   0        0        0      254 2023-04-23 19:57:27.523407 Sphinx-7.0.0/tests/roots/test-ext-coverage/coverage_ignored.py
--rw-r--r--   0        0        0      254 2023-04-23 19:57:27.523407 Sphinx-7.0.0/tests/roots/test-ext-coverage/coverage_not_ignored.py
--rw-r--r--   0        0        0       98 2023-04-23 19:57:27.523407 Sphinx-7.0.0/tests/roots/test-ext-coverage/index.rst
--rw-r--r--   0        0        0      371 2023-04-23 19:57:27.523407 Sphinx-7.0.0/tests/roots/test-ext-doctest-skipif/conf.py
--rw-r--r--   0        0        0     2052 2023-04-23 19:57:27.523407 Sphinx-7.0.0/tests/roots/test-ext-doctest-skipif/skipif.txt
--rw-r--r--   0        0        0      205 2023-04-23 19:57:27.523407 Sphinx-7.0.0/tests/roots/test-ext-doctest-with-autodoc/conf.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.524407 Sphinx-7.0.0/tests/roots/test-ext-doctest-with-autodoc/dir/__init__.py
--rw-r--r--   0        0        0       28 2023-04-23 19:57:27.524407 Sphinx-7.0.0/tests/roots/test-ext-doctest-with-autodoc/dir/bar.py
--rw-r--r--   0        0        0       60 2023-04-23 19:57:27.524407 Sphinx-7.0.0/tests/roots/test-ext-doctest-with-autodoc/dir/inner.rst
--rw-r--r--   0        0        0       25 2023-04-23 19:57:27.524407 Sphinx-7.0.0/tests/roots/test-ext-doctest-with-autodoc/foo.py
--rw-r--r--   0        0        0       52 2023-04-23 19:57:27.524407 Sphinx-7.0.0/tests/roots/test-ext-doctest-with-autodoc/index.rst
--rw-r--r--   0        0        0      148 2023-04-23 19:57:27.524407 Sphinx-7.0.0/tests/roots/test-ext-doctest/conf.py
--rw-r--r--   0        0        0     2147 2023-04-23 19:57:27.525407 Sphinx-7.0.0/tests/roots/test-ext-doctest/doctest.txt
--rw-r--r--   0        0        0      190 2023-04-23 19:57:27.525407 Sphinx-7.0.0/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/conf.py
--rw-r--r--   0        0        0      555 2023-04-23 19:57:27.525407 Sphinx-7.0.0/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/index.rst
--rw-r--r--   0        0        0      161 2023-04-23 19:57:27.525407 Sphinx-7.0.0/tests/roots/test-ext-extlinks-hardcoded-urls/conf.py
--rw-r--r--   0        0        0      703 2023-04-23 19:57:27.525407 Sphinx-7.0.0/tests/roots/test-ext-extlinks-hardcoded-urls/index.rst
--rw-r--r--   0        0        0       40 2023-04-23 19:57:27.525407 Sphinx-7.0.0/tests/roots/test-ext-githubpages/conf.py
--rw-r--r--   0        0        0       25 2023-04-23 19:57:27.525407 Sphinx-7.0.0/tests/roots/test-ext-githubpages/index.rst
--rw-r--r--   0        0        0       67 2023-04-23 19:57:27.526407 Sphinx-7.0.0/tests/roots/test-ext-graphviz/conf.py
--rw-r--r--   0        0        0       25 2023-04-23 19:57:27.526407 Sphinx-7.0.0/tests/roots/test-ext-graphviz/graph.dot
--rw-r--r--   0        0        0       25 2023-04-23 19:57:27.526407 Sphinx-7.0.0/tests/roots/test-ext-graphviz/graph.xx.dot
--rw-r--r--   0        0        0      389 2023-04-23 19:57:27.526407 Sphinx-7.0.0/tests/roots/test-ext-graphviz/index.rst
--rw-r--r--   0        0        0      256 2023-04-23 19:57:27.526407 Sphinx-7.0.0/tests/roots/test-ext-ifconfig/conf.py
--rw-r--r--   0        0        0      274 2023-04-23 19:57:27.526407 Sphinx-7.0.0/tests/roots/test-ext-ifconfig/index.rst
--rw-r--r--   0        0        0       41 2023-04-23 19:57:27.527407 Sphinx-7.0.0/tests/roots/test-ext-imgconverter/conf.py
--rw-r--r--   0        0        0   141783 2023-04-23 19:57:27.528407 Sphinx-7.0.0/tests/roots/test-ext-imgconverter/img.pdf
--rw-r--r--   0        0        0       86 2023-04-23 19:57:27.528407 Sphinx-7.0.0/tests/roots/test-ext-imgconverter/index.rst
--rw-r--r--   0        0        0      243 2023-04-23 19:57:27.528407 Sphinx-7.0.0/tests/roots/test-ext-imgconverter/svgimg.svg
--rw-r--r--   0        0        0      106 2023-04-23 19:57:27.528407 Sphinx-7.0.0/tests/roots/test-ext-imgmockconverter/1/svgimg.svg
--rw-r--r--   0        0        0      243 2023-04-23 19:57:27.528407 Sphinx-7.0.0/tests/roots/test-ext-imgmockconverter/2/svgimg.svg
--rw-r--r--   0        0        0       97 2023-04-23 19:57:27.529407 Sphinx-7.0.0/tests/roots/test-ext-imgmockconverter/conf.py
--rw-r--r--   0        0        0       98 2023-04-23 19:57:27.529407 Sphinx-7.0.0/tests/roots/test-ext-imgmockconverter/index.rst
--rw-r--r--   0        0        0      881 2023-04-23 19:57:27.529407 Sphinx-7.0.0/tests/roots/test-ext-imgmockconverter/mocksvgconverter.py
--rw-r--r--   0        0        0      112 2023-04-23 19:57:27.529407 Sphinx-7.0.0/tests/roots/test-ext-inheritance_diagram/conf.py
--rw-r--r--   0        0        0       13 2023-04-23 19:57:27.529407 Sphinx-7.0.0/tests/roots/test-ext-inheritance_diagram/example/__init__.py
--rw-r--r--   0        0        0       46 2023-04-23 19:57:27.529407 Sphinx-7.0.0/tests/roots/test-ext-inheritance_diagram/example/sphinx.py
--rw-r--r--   0        0        0      215 2023-04-23 19:57:27.529407 Sphinx-7.0.0/tests/roots/test-ext-inheritance_diagram/index.rst
--rw-r--r--   0        0        0      101 2023-04-23 19:57:27.530407 Sphinx-7.0.0/tests/roots/test-ext-inheritance_diagram/test.py
--rw-r--r--   0        0        0       40 2023-04-23 19:57:27.530407 Sphinx-7.0.0/tests/roots/test-ext-intersphinx-cppdomain/conf.py
--rw-r--r--   0        0        0      150 2023-04-23 19:57:27.530407 Sphinx-7.0.0/tests/roots/test-ext-intersphinx-cppdomain/index.rst
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.530407 Sphinx-7.0.0/tests/roots/test-ext-intersphinx-role/conf.py
--rw-r--r--   0        0        0     1211 2023-04-23 19:57:27.530407 Sphinx-7.0.0/tests/roots/test-ext-intersphinx-role/index.rst
--rw-r--r--   0        0        0      488 2023-04-23 19:57:27.530407 Sphinx-7.0.0/tests/roots/test-ext-math-compat/conf.py
--rw-r--r--   0        0        0      199 2023-04-23 19:57:27.531407 Sphinx-7.0.0/tests/roots/test-ext-math-compat/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.531407 Sphinx-7.0.0/tests/roots/test-ext-math-simple/conf.py
--rw-r--r--   0        0        0       43 2023-04-23 19:57:27.531407 Sphinx-7.0.0/tests/roots/test-ext-math-simple/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.531407 Sphinx-7.0.0/tests/roots/test-ext-math/conf.py
--rw-r--r--   0        0        0      239 2023-04-23 19:57:27.531407 Sphinx-7.0.0/tests/roots/test-ext-math/index.rst
--rw-r--r--   0        0        0      396 2023-04-23 19:57:27.531407 Sphinx-7.0.0/tests/roots/test-ext-math/math.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.531407 Sphinx-7.0.0/tests/roots/test-ext-math/nomath.rst
--rw-r--r--   0        0        0      128 2023-04-23 19:57:27.531407 Sphinx-7.0.0/tests/roots/test-ext-math/page.rst
--rw-r--r--   0        0        0      100 2023-04-23 19:57:27.532407 Sphinx-7.0.0/tests/roots/test-ext-napoleon/conf.py
--rw-r--r--   0        0        0       64 2023-04-23 19:57:27.532407 Sphinx-7.0.0/tests/roots/test-ext-napoleon/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.532407 Sphinx-7.0.0/tests/roots/test-ext-napoleon/mypackage/__init__.py
--rw-r--r--   0        0        0      194 2023-04-23 19:57:27.532407 Sphinx-7.0.0/tests/roots/test-ext-napoleon/mypackage/typehints.py
--rw-r--r--   0        0        0       70 2023-04-23 19:57:27.532407 Sphinx-7.0.0/tests/roots/test-ext-napoleon/typehints.rst
--rw-r--r--   0        0        0       31 2023-04-23 19:57:27.532407 Sphinx-7.0.0/tests/roots/test-ext-todo/bar.rst
--rw-r--r--   0        0        0       33 2023-04-23 19:57:27.533407 Sphinx-7.0.0/tests/roots/test-ext-todo/conf.py
--rw-r--r--   0        0        0      125 2023-04-23 19:57:27.533407 Sphinx-7.0.0/tests/roots/test-ext-todo/foo.rst
--rw-r--r--   0        0        0      109 2023-04-23 19:57:27.533407 Sphinx-7.0.0/tests/roots/test-ext-todo/index.rst
--rw-r--r--   0        0        0      108 2023-04-23 19:57:27.533407 Sphinx-7.0.0/tests/roots/test-ext-viewcode-find/conf.py
--rw-r--r--   0        0        0      636 2023-04-23 19:57:27.533407 Sphinx-7.0.0/tests/roots/test-ext-viewcode-find/index.rst
--rw-r--r--   0        0        0       37 2023-04-23 19:57:27.533407 Sphinx-7.0.0/tests/roots/test-ext-viewcode-find/not_a_package/__init__.py
--rw-r--r--   0        0        0      371 2023-04-23 19:57:27.533407 Sphinx-7.0.0/tests/roots/test-ext-viewcode-find/not_a_package/submodule.py
--rw-r--r--   0        0        0      745 2023-04-23 19:57:27.534407 Sphinx-7.0.0/tests/roots/test-ext-viewcode/conf.py
--rw-r--r--   0        0        0      550 2023-04-23 19:57:27.534407 Sphinx-7.0.0/tests/roots/test-ext-viewcode/index.rst
--rw-r--r--   0        0        0     3111 2023-04-23 19:57:27.534407 Sphinx-7.0.0/tests/roots/test-ext-viewcode/objects.rst
--rw-r--r--   0        0        0       64 2023-04-23 19:57:27.534407 Sphinx-7.0.0/tests/roots/test-ext-viewcode/spam/__init__.py
--rw-r--r--   0        0        0      308 2023-04-23 19:57:27.534407 Sphinx-7.0.0/tests/roots/test-ext-viewcode/spam/mod1.py
--rw-r--r--   0        0        0      188 2023-04-23 19:57:27.534407 Sphinx-7.0.0/tests/roots/test-ext-viewcode/spam/mod2.py
--rw-r--r--   0        0        0       52 2023-04-23 19:57:27.534407 Sphinx-7.0.0/tests/roots/test-ext-viewcode/spam/mod3.py
--rw-r--r--   0        0        0       63 2023-04-23 19:57:27.535407 Sphinx-7.0.0/tests/roots/test-extensions/conf.py
--rw-r--r--   0        0        0       70 2023-04-23 19:57:27.535407 Sphinx-7.0.0/tests/roots/test-extensions/read_parallel.py
--rw-r--r--   0        0        0       71 2023-04-23 19:57:27.535407 Sphinx-7.0.0/tests/roots/test-extensions/read_serial.py
--rw-r--r--   0        0        0       72 2023-04-23 19:57:27.535407 Sphinx-7.0.0/tests/roots/test-extensions/write_parallel.py
--rw-r--r--   0        0        0       72 2023-04-23 19:57:27.535407 Sphinx-7.0.0/tests/roots/test-extensions/write_serial.py
--rw-r--r--   0        0        0       70 2023-04-23 19:57:27.535407 Sphinx-7.0.0/tests/roots/test-footnotes/bar.rst
--rw-r--r--   0        0        0       70 2023-04-23 19:57:27.536407 Sphinx-7.0.0/tests/roots/test-footnotes/baz.rst
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.536407 Sphinx-7.0.0/tests/roots/test-footnotes/conf.py
--rw-r--r--   0        0        0     3385 2023-04-23 19:57:27.536407 Sphinx-7.0.0/tests/roots/test-footnotes/index.rst
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.536407 Sphinx-7.0.0/tests/roots/test-footnotes/rimg.png
--rw-r--r--   0        0        0      143 2023-04-23 19:57:27.536407 Sphinx-7.0.0/tests/roots/test-gettext-template/_templates/template1.html
--rw-r--r--   0        0        0      143 2023-04-23 19:57:27.536407 Sphinx-7.0.0/tests/roots/test-gettext-template/_templates/template2.html
--rw-r--r--   0        0        0       32 2023-04-23 19:57:27.536407 Sphinx-7.0.0/tests/roots/test-gettext-template/conf.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.536407 Sphinx-7.0.0/tests/roots/test-gettext-template/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.537407 Sphinx-7.0.0/tests/roots/test-glossary/conf.py
--rw-r--r--   0        0        0      260 2023-04-23 19:57:27.537407 Sphinx-7.0.0/tests/roots/test-glossary/index.rst
--rw-r--r--   0        0        0      103 2023-04-23 19:57:27.537407 Sphinx-7.0.0/tests/roots/test-highlight_options/conf.py
--rw-r--r--   0        0        0      166 2023-04-23 19:57:27.537407 Sphinx-7.0.0/tests/roots/test-highlight_options/index.rst
--rw-r--r--   0        0        0      468 2023-04-23 19:57:27.537407 Sphinx-7.0.0/tests/roots/test-html_assets/conf.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.537407 Sphinx-7.0.0/tests/roots/test-html_assets/extra/.htaccess
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.537407 Sphinx-7.0.0/tests/roots/test-html_assets/extra/.htpasswd
--rw-r--r--   0        0        0       28 2023-04-23 19:57:27.538407 Sphinx-7.0.0/tests/roots/test-html_assets/extra/API.html_t
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.538679 Sphinx-7.0.0/tests/roots/test-html_assets/extra/css/style.css
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.538679 Sphinx-7.0.0/tests/roots/test-html_assets/extra/index.rst
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.538679 Sphinx-7.0.0/tests/roots/test-html_assets/extra/rimg.png
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.538679 Sphinx-7.0.0/tests/roots/test-html_assets/extra/subdir/.htaccess
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.538679 Sphinx-7.0.0/tests/roots/test-html_assets/extra/subdir/.htpasswd
--rw-r--r--   0        0        0       65 2023-04-23 19:57:27.538679 Sphinx-7.0.0/tests/roots/test-html_assets/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.538679 Sphinx-7.0.0/tests/roots/test-html_assets/static/.htaccess
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.538679 Sphinx-7.0.0/tests/roots/test-html_assets/static/.htpasswd
--rw-r--r--   0        0        0       28 2023-04-23 19:57:27.539686 Sphinx-7.0.0/tests/roots/test-html_assets/static/API.html_t
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.539686 Sphinx-7.0.0/tests/roots/test-html_assets/static/css/style.css
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.539686 Sphinx-7.0.0/tests/roots/test-html_assets/static/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.539686 Sphinx-7.0.0/tests/roots/test-html_assets/static/js/custom.js
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.539686 Sphinx-7.0.0/tests/roots/test-html_assets/static/rimg.png
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.539686 Sphinx-7.0.0/tests/roots/test-html_assets/static/subdir/.htaccess
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.540686 Sphinx-7.0.0/tests/roots/test-html_assets/static/subdir/.htpasswd
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.540686 Sphinx-7.0.0/tests/roots/test-html_assets/subdir/_build/index.html
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.540686 Sphinx-7.0.0/tests/roots/test-html_assets/subdir/background.png
--rw-r--r--   0        0        0       53 2023-04-23 19:57:27.540686 Sphinx-7.0.0/tests/roots/test-html_entity/conf.py
--rw-r--r--   0        0        0      561 2023-04-23 19:57:27.540686 Sphinx-7.0.0/tests/roots/test-html_entity/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.541685 Sphinx-7.0.0/tests/roots/test-html_scaled_image_link/conf.py
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.541685 Sphinx-7.0.0/tests/roots/test-html_scaled_image_link/img.png
--rw-r--r--   0        0        0      172 2023-04-23 19:57:27.541685 Sphinx-7.0.0/tests/roots/test-html_scaled_image_link/index.rst
--rw-r--r--   0        0        0       36 2023-04-23 19:57:27.541685 Sphinx-7.0.0/tests/roots/test-html_signaturereturn_icon/conf.py
--rw-r--r--   0        0        0      108 2023-04-23 19:57:27.541685 Sphinx-7.0.0/tests/roots/test-html_signaturereturn_icon/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.541685 Sphinx-7.0.0/tests/roots/test-html_style/_static/default.css
--rw-r--r--   0        0        0       58 2023-04-23 19:57:27.542686 Sphinx-7.0.0/tests/roots/test-html_style/conf.py
--rw-r--r--   0        0        0       22 2023-04-23 19:57:27.542686 Sphinx-7.0.0/tests/roots/test-html_style/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.542686 Sphinx-7.0.0/tests/roots/test-image-escape/conf.py
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.542686 Sphinx-7.0.0/tests/roots/test-image-escape/img_#1.png
--rw-r--r--   0        0        0      145 2023-04-23 19:57:27.542686 Sphinx-7.0.0/tests/roots/test-image-escape/index.rst
--rw-r--r--   0        0        0      161 2023-04-23 19:57:27.542686 Sphinx-7.0.0/tests/roots/test-image-in-parsed-literal/conf.py
--rw-r--r--   0        0        0      113 2023-04-23 19:57:27.542686 Sphinx-7.0.0/tests/roots/test-image-in-parsed-literal/index.rst
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.543686 Sphinx-7.0.0/tests/roots/test-image-in-parsed-literal/pic.png
--rw-r--r--   0        0        0      143 2023-04-23 19:57:27.543886 Sphinx-7.0.0/tests/roots/test-image-in-section/conf.py
--rw-r--r--   0        0        0      287 2023-04-23 19:57:27.543886 Sphinx-7.0.0/tests/roots/test-image-in-section/index.rst
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.543886 Sphinx-7.0.0/tests/roots/test-image-in-section/pic.png
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.543886 Sphinx-7.0.0/tests/roots/test-images/conf.py
--rw-r--r--   0        0        0    24976 2023-04-23 19:57:27.543886 Sphinx-7.0.0/tests/roots/test-images/img.gif
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.543886 Sphinx-7.0.0/tests/roots/test-images/img.ja.png
--rw-r--r--   0        0        0   141783 2023-04-23 19:57:27.544893 Sphinx-7.0.0/tests/roots/test-images/img.pdf
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.545892 Sphinx-7.0.0/tests/roots/test-images/img.png
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.545892 Sphinx-7.0.0/tests/roots/test-images/img.zh.png
--rw-r--r--   0        0        0      466 2023-04-23 19:57:27.545892 Sphinx-7.0.0/tests/roots/test-images/index.rst
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.545892 Sphinx-7.0.0/tests/roots/test-images/rimg.png
--rw-r--r--   0        0        0      218 2023-04-23 19:57:27.545892 Sphinx-7.0.0/tests/roots/test-images/rimg.png.xx
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.545892 Sphinx-7.0.0/tests/roots/test-images/rimg.xx.png
--rw-r--r--   0        0        0      128 2023-04-23 19:57:27.546893 Sphinx-7.0.0/tests/roots/test-images/subdir/index.rst
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.546893 Sphinx-7.0.0/tests/roots/test-images/subdir/rimg.png
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.546893 Sphinx-7.0.0/tests/roots/test-images/subdir/rimg.xx.png
--rw-r--r--   0        0        0   141783 2023-04-23 19:57:27.547893 Sphinx-7.0.0/tests/roots/test-images/subdir/svgimg.pdf
--rw-r--r--   0        0        0      243 2023-04-23 19:57:27.547893 Sphinx-7.0.0/tests/roots/test-images/subdir/svgimg.svg
--rw-r--r--   0        0        0      243 2023-04-23 19:57:27.547893 Sphinx-7.0.0/tests/roots/test-images/subdir/svgimg.xx.svg
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.547893 Sphinx-7.0.0/tests/roots/test-images/testimäge.png
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.548892 Sphinx-7.0.0/tests/roots/test-index_on_title/conf.py
--rw-r--r--   0        0        0      117 2023-04-23 19:57:27.548892 Sphinx-7.0.0/tests/roots/test-index_on_title/contents.rst
--rw-r--r--   0        0        0       70 2023-04-23 19:57:27.548892 Sphinx-7.0.0/tests/roots/test-inheritance/basic_diagram.rst
--rw-r--r--   0        0        0      135 2023-04-23 19:57:27.548892 Sphinx-7.0.0/tests/roots/test-inheritance/conf.py
--rw-r--r--   0        0        0      166 2023-04-23 19:57:27.548892 Sphinx-7.0.0/tests/roots/test-inheritance/diagram_module_w_2_top_classes.rst
--rw-r--r--   0        0        0      125 2023-04-23 19:57:27.548892 Sphinx-7.0.0/tests/roots/test-inheritance/diagram_w_1_top_class.rst
--rw-r--r--   0        0        0      179 2023-04-23 19:57:27.548892 Sphinx-7.0.0/tests/roots/test-inheritance/diagram_w_2_top_classes.rst
--rw-r--r--   0        0        0      104 2023-04-23 19:57:27.549892 Sphinx-7.0.0/tests/roots/test-inheritance/diagram_w_nested_classes.rst
--rw-r--r--   0        0        0      118 2023-04-23 19:57:27.549892 Sphinx-7.0.0/tests/roots/test-inheritance/diagram_w_parts.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.549892 Sphinx-7.0.0/tests/roots/test-inheritance/dummy/__init__.py
--rw-r--r--   0        0        0      267 2023-04-23 19:57:27.549892 Sphinx-7.0.0/tests/roots/test-inheritance/dummy/test.py
--rw-r--r--   0        0        0       95 2023-04-23 19:57:27.549892 Sphinx-7.0.0/tests/roots/test-inheritance/dummy/test_nested.py
--rw-r--r--   0        0        0       31 2023-04-23 19:57:27.549892 Sphinx-7.0.0/tests/roots/test-inheritance/index.rst
--rw-r--r--   0        0        0      216 2023-04-23 19:57:27.549892 Sphinx-7.0.0/tests/roots/test-intl/_templates/contents.html
--rw-r--r--   0        0        0      599 2023-04-23 19:57:27.550892 Sphinx-7.0.0/tests/roots/test-intl/admonitions.txt
--rw-r--r--   0        0        0       74 2023-04-23 19:57:27.550892 Sphinx-7.0.0/tests/roots/test-intl/bom.txt
--rw-r--r--   0        0        0      262 2023-04-23 19:57:27.550892 Sphinx-7.0.0/tests/roots/test-intl/conf.py
--rw-r--r--   0        0        0      342 2023-04-23 19:57:27.550892 Sphinx-7.0.0/tests/roots/test-intl/definition_terms.txt
--rw-r--r--   0        0        0      704 2023-04-23 19:57:27.550892 Sphinx-7.0.0/tests/roots/test-intl/docfields.txt
--rw-r--r--   0        0        0      858 2023-04-23 19:57:27.550892 Sphinx-7.0.0/tests/roots/test-intl/external_links.txt
--rw-r--r--   0        0        0      747 2023-04-23 19:57:27.550892 Sphinx-7.0.0/tests/roots/test-intl/figure.txt
--rw-r--r--   0        0        0      407 2023-04-23 19:57:27.550892 Sphinx-7.0.0/tests/roots/test-intl/footnote.txt
--rw-r--r--   0        0        0      378 2023-04-23 19:57:27.551892 Sphinx-7.0.0/tests/roots/test-intl/glossary_terms.txt
--rw-r--r--   0        0        0      151 2023-04-23 19:57:27.551892 Sphinx-7.0.0/tests/roots/test-intl/glossary_terms_inconsistency.txt
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.551892 Sphinx-7.0.0/tests/roots/test-intl/i18n.png
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.551892 Sphinx-7.0.0/tests/roots/test-intl/img.png
--rw-r--r--   0        0        0      539 2023-04-23 19:57:27.551892 Sphinx-7.0.0/tests/roots/test-intl/index.txt
--rw-r--r--   0        0        0      530 2023-04-23 19:57:27.551892 Sphinx-7.0.0/tests/roots/test-intl/index_entries.txt
--rw-r--r--   0        0        0     1832 2023-04-23 19:57:27.552893 Sphinx-7.0.0/tests/roots/test-intl/label_target.txt
--rw-r--r--   0        0        0      943 2023-04-23 19:57:27.552893 Sphinx-7.0.0/tests/roots/test-intl/literalblock.txt
--rw-r--r--   0        0        0      278 2023-04-23 19:57:27.552893 Sphinx-7.0.0/tests/roots/test-intl/noqa.txt
--rw-r--r--   0        0        0      128 2023-04-23 19:57:27.552893 Sphinx-7.0.0/tests/roots/test-intl/only.txt
--rw-r--r--   0        0        0       78 2023-04-23 19:57:27.552893 Sphinx-7.0.0/tests/roots/test-intl/raw.txt
--rw-r--r--   0        0        0     1094 2023-04-23 19:57:27.552893 Sphinx-7.0.0/tests/roots/test-intl/refs.txt
--rw-r--r--   0        0        0      291 2023-04-23 19:57:27.552893 Sphinx-7.0.0/tests/roots/test-intl/refs_inconsistency.txt
--rw-r--r--   0        0        0      252 2023-04-23 19:57:27.552893 Sphinx-7.0.0/tests/roots/test-intl/refs_python_domain.txt
--rw-r--r--   0        0        0      738 2023-04-23 19:57:27.552893 Sphinx-7.0.0/tests/roots/test-intl/role_xref.txt
--rw-r--r--   0        0        0      152 2023-04-23 19:57:27.553892 Sphinx-7.0.0/tests/roots/test-intl/rubric.txt
--rw-r--r--   0        0        0       97 2023-04-23 19:57:27.553892 Sphinx-7.0.0/tests/roots/test-intl/section.txt
--rw-r--r--   0        0        0      210 2023-04-23 19:57:27.554190 Sphinx-7.0.0/tests/roots/test-intl/seealso.txt
--rw-r--r--   0        0        0       32 2023-04-23 19:57:27.554190 Sphinx-7.0.0/tests/roots/test-intl/subdir/index.txt
--rw-r--r--   0        0        0      263 2023-04-23 19:57:27.554190 Sphinx-7.0.0/tests/roots/test-intl/table.txt
--rw-r--r--   0        0        0      139 2023-04-23 19:57:27.554190 Sphinx-7.0.0/tests/roots/test-intl/toctree.txt
--rw-r--r--   0        0        0      135 2023-04-23 19:57:27.554190 Sphinx-7.0.0/tests/roots/test-intl/topic.txt
--rw-r--r--   0        0        0      337 2023-04-23 19:57:27.554190 Sphinx-7.0.0/tests/roots/test-intl/versionchange.txt
--rw-r--r--   0        0        0       79 2023-04-23 19:57:27.554190 Sphinx-7.0.0/tests/roots/test-intl/warnings.txt
--rw-r--r--   0        0        0     1513 2023-04-23 19:57:27.555196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/admonitions.po
--rw-r--r--   0        0        0      264 2023-04-23 19:57:27.555196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/bom.po
--rw-r--r--   0        0        0     1198 2023-04-25 10:59:46.885153 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/definition_terms.po
--rw-r--r--   0        0        0     1086 2023-04-23 19:57:27.555196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/docfields.po
--rw-r--r--   0        0        0     1691 2023-04-23 19:57:27.555196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/external_links.po
--rw-r--r--   0        0        0     1307 2023-04-23 19:57:27.556196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/figure.po
--rw-r--r--   0        0        0     1228 2023-04-23 19:57:27.556196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/footnote.po
--rw-r--r--   0        0        0     1327 2023-04-23 19:57:27.556196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms.po
--rw-r--r--   0        0        0      754 2023-04-25 10:59:46.885153 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms_inconsistency.po
--rw-r--r--   0        0        0      773 2023-04-23 19:57:27.556196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/index.po
--rw-r--r--   0        0        0     1318 2023-04-23 19:57:27.556196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/index_entries.po
--rw-r--r--   0        0        0     2159 2023-04-23 19:57:27.557196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/label_target.po
--rw-r--r--   0        0        0     2211 2023-04-23 19:57:27.557196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/literalblock.po
--rw-r--r--   0        0        0     1380 2023-04-23 19:57:27.557196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/noqa.po
--rw-r--r--   0        0        0      723 2023-04-23 19:57:27.557196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/only.po
--rw-r--r--   0        0        0      644 2023-04-23 19:57:27.557196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/raw.po
--rw-r--r--   0        0        0     2771 2023-04-23 19:57:27.557196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/refs.po
--rw-r--r--   0        0        0     1045 2023-04-23 19:57:27.557196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/refs_inconsistency.po
--rw-r--r--   0        0        0      675 2023-04-23 19:57:27.557196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/refs_python_domain.po
--rw-r--r--   0        0        0     1707 2023-04-23 19:57:27.558196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/role_xref.po
--rw-r--r--   0        0        0      744 2023-04-25 10:59:46.885153 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/rubric.po
--rw-r--r--   0        0        0      706 2023-04-23 19:57:27.558196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/section.po
--rw-r--r--   0        0        0      792 2023-04-23 19:57:27.558196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/seealso.po
--rw-r--r--   0        0        0      621 2023-04-23 19:57:27.558196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0      992 2023-04-23 19:57:27.558196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/table.po
--rw-r--r--   0        0        0      767 2023-04-23 19:57:27.558196 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/toctree.po
--rw-r--r--   0        0        0      750 2023-04-23 19:57:27.559195 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/topic.po
--rw-r--r--   0        0        0     1070 2023-04-23 19:57:27.559195 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/versionchange.po
--rw-r--r--   0        0        0      710 2023-04-23 19:57:27.559195 Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/warnings.po
--rw-r--r--   0        0        0       21 2023-04-23 19:57:27.559195 Sphinx-7.0.0/tests/roots/test-keep_warnings/conf.py
--rw-r--r--   0        0        0       20 2023-04-23 19:57:27.559195 Sphinx-7.0.0/tests/roots/test-keep_warnings/index.rst
--rw-r--r--   0        0        0       13 2023-04-23 19:57:27.559195 Sphinx-7.0.0/tests/roots/test-latex-babel/bar.rst
--rw-r--r--   0        0        0       98 2023-04-23 19:57:27.559195 Sphinx-7.0.0/tests/roots/test-latex-babel/conf.py
--rw-r--r--   0        0        0       13 2023-04-23 19:57:27.560196 Sphinx-7.0.0/tests/roots/test-latex-babel/foo.rst
--rw-r--r--   0        0        0       87 2023-04-23 19:57:27.560196 Sphinx-7.0.0/tests/roots/test-latex-babel/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.560196 Sphinx-7.0.0/tests/roots/test-latex-container/conf.py
--rw-r--r--   0        0        0       35 2023-04-23 19:57:27.560196 Sphinx-7.0.0/tests/roots/test-latex-container/index.rst
--rw-r--r--   0        0        0       59 2023-04-23 19:57:27.560196 Sphinx-7.0.0/tests/roots/test-latex-equations/conf.py
--rw-r--r--   0        0        0      256 2023-04-23 19:57:27.560196 Sphinx-7.0.0/tests/roots/test-latex-equations/equations.rst
--rw-r--r--   0        0        0      452 2023-04-23 19:57:27.560196 Sphinx-7.0.0/tests/roots/test-latex-equations/expects/latex-equations.tex
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.561196 Sphinx-7.0.0/tests/roots/test-latex-figure-in-admonition/conf.py
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.561196 Sphinx-7.0.0/tests/roots/test-latex-figure-in-admonition/img.png
--rw-r--r--   0        0        0      132 2023-04-23 19:57:27.561196 Sphinx-7.0.0/tests/roots/test-latex-figure-in-admonition/index.rst
--rw-r--r--   0        0        0     1573 2023-04-23 19:57:27.561196 Sphinx-7.0.0/tests/roots/test-latex-includegraphics/conf.py
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.561196 Sphinx-7.0.0/tests/roots/test-latex-includegraphics/img.png
--rw-r--r--   0        0        0      834 2023-04-23 19:57:27.561196 Sphinx-7.0.0/tests/roots/test-latex-includegraphics/index.rst
--rw-r--r--   0        0        0    34213 2023-04-23 19:57:27.562196 Sphinx-7.0.0/tests/roots/test-latex-includegraphics/sphinx.png
--rw-r--r--   0        0        0    38192 2023-04-23 19:57:27.562196 Sphinx-7.0.0/tests/roots/test-latex-includegraphics/tall.png
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.562196 Sphinx-7.0.0/tests/roots/test-latex-index/conf.py
--rw-r--r--   0        0        0      215 2023-04-23 19:57:27.562196 Sphinx-7.0.0/tests/roots/test-latex-index/index.rst
--rw-r--r--   0        0        0       17 2023-04-23 19:57:27.563195 Sphinx-7.0.0/tests/roots/test-latex-labels-before-module/automodule1.py
--rw-r--r--   0        0        0       17 2023-04-23 19:57:27.563195 Sphinx-7.0.0/tests/roots/test-latex-labels-before-module/automodule2a.py
--rw-r--r--   0        0        0       17 2023-04-23 19:57:27.563195 Sphinx-7.0.0/tests/roots/test-latex-labels-before-module/automodule2b.py
--rw-r--r--   0        0        0       17 2023-04-23 19:57:27.564197 Sphinx-7.0.0/tests/roots/test-latex-labels-before-module/automodule3.py
--rw-r--r--   0        0        0      117 2023-04-23 19:57:27.564197 Sphinx-7.0.0/tests/roots/test-latex-labels-before-module/conf.py
--rw-r--r--   0        0        0      464 2023-04-23 19:57:27.564197 Sphinx-7.0.0/tests/roots/test-latex-labels-before-module/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.564197 Sphinx-7.0.0/tests/roots/test-latex-labels/conf.py
--rw-r--r--   0        0        0      771 2023-04-23 19:57:27.565196 Sphinx-7.0.0/tests/roots/test-latex-labels/index.rst
--rw-r--r--   0        0        0       18 2023-04-23 19:57:27.565196 Sphinx-7.0.0/tests/roots/test-latex-labels/otherdoc.rst
--rw-r--r--   0        0        0      250 2023-04-23 19:57:27.565196 Sphinx-7.0.0/tests/roots/test-latex-numfig/conf.py
--rw-r--r--   0        0        0      112 2023-04-23 19:57:27.565196 Sphinx-7.0.0/tests/roots/test-latex-numfig/index.rst
--rw-r--r--   0        0        0      141 2023-04-23 19:57:27.565196 Sphinx-7.0.0/tests/roots/test-latex-numfig/indexhowto.rst
--rw-r--r--   0        0        0      165 2023-04-23 19:57:27.565196 Sphinx-7.0.0/tests/roots/test-latex-numfig/indexmanual.rst
--rw-r--r--   0        0        0       18 2023-04-23 19:57:27.566196 Sphinx-7.0.0/tests/roots/test-latex-table/_mytemplates/latex/longtable.tex_t
--rw-r--r--   0        0        0     1661 2023-04-23 19:57:27.566196 Sphinx-7.0.0/tests/roots/test-latex-table/complex.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.566196 Sphinx-7.0.0/tests/roots/test-latex-table/conf.py
--rw-r--r--   0        0        0     1933 2023-04-23 19:57:27.566196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/complex_spanning_cell.tex
--rw-r--r--   0        0        0     1752 2023-04-23 19:57:27.566196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/gridtable.tex
--rw-r--r--   0        0        0     1780 2023-04-23 19:57:27.566196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/gridtable_with_tabularcolumn.tex
--rw-r--r--   0        0        0     1323 2023-04-23 19:57:27.567196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable.tex
--rw-r--r--   0        0        0     1300 2023-04-23 19:57:27.567196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_align.tex
--rw-r--r--   0        0        0     1445 2023-04-23 19:57:27.567196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_caption.tex
--rw-r--r--   0        0        0     1384 2023-04-23 19:57:27.567196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_problematic_cell.tex
--rw-r--r--   0        0        0     1637 2023-04-23 19:57:27.568196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_stub_columns_and_problematic_cell.tex
--rw-r--r--   0        0        0     1386 2023-04-23 19:57:27.568196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_verbatim.tex
--rw-r--r--   0        0        0     1656 2023-04-23 19:57:27.568196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_widths.tex
--rw-r--r--   0        0        0     1409 2023-04-23 19:57:27.568196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_widths_and_problematic_cell.tex
--rw-r--r--   0        0        0     1341 2023-04-23 19:57:27.569196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_with_tabularcolumn.tex
--rw-r--r--   0        0        0      704 2023-04-23 19:57:27.569196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/simple_table.tex
--rw-r--r--   0        0        0      851 2023-04-23 19:57:27.569196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_caption.tex
--rw-r--r--   0        0        0      777 2023-04-23 19:57:27.569196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_problematic_cell.tex
--rw-r--r--   0        0        0      978 2023-04-23 19:57:27.569196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_stub_columns_and_problematic_cell.tex
--rw-r--r--   0        0        0      594 2023-04-23 19:57:27.569196 Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_threeparagraphs_cell_in_first_col.tex
--rw-r--r--   0        0        0      779 2023-04-23 19:57:27.570195 Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_verbatim.tex
--rw-r--r--   0        0        0     1093 2023-04-23 19:57:27.570195 Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_widths.tex
--rw-r--r--   0        0        0      802 2023-04-23 19:57:27.570358 Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_widths_and_problematic_cell.tex
--rw-r--r--   0        0        0      733 2023-04-23 19:57:27.570358 Sphinx-7.0.0/tests/roots/test-latex-table/expects/tabular_having_widths.tex
--rw-r--r--   0        0        0      747 2023-04-23 19:57:27.570358 Sphinx-7.0.0/tests/roots/test-latex-table/expects/tabularcolumn.tex
--rw-r--r--   0        0        0      727 2023-04-23 19:57:27.570358 Sphinx-7.0.0/tests/roots/test-latex-table/expects/tabulary_having_widths.tex
--rw-r--r--   0        0        0       84 2023-04-23 19:57:27.570358 Sphinx-7.0.0/tests/roots/test-latex-table/index.rst
--rw-r--r--   0        0        0     2516 2023-04-23 19:57:27.570358 Sphinx-7.0.0/tests/roots/test-latex-table/longtable.rst
--rw-r--r--   0        0        0     2770 2023-04-23 19:57:27.571364 Sphinx-7.0.0/tests/roots/test-latex-table/tabular.rst
--rw-r--r--   0        0        0       52 2023-04-23 19:57:27.571364 Sphinx-7.0.0/tests/roots/test-latex-theme/conf.py
--rw-r--r--   0        0        0       24 2023-04-23 19:57:27.571364 Sphinx-7.0.0/tests/roots/test-latex-theme/index.rst
--rw-r--r--   0        0        0      117 2023-04-23 19:57:27.571364 Sphinx-7.0.0/tests/roots/test-latex-theme/theme/custom/theme.conf
--rw-r--r--   0        0        0      160 2023-04-23 19:57:27.571364 Sphinx-7.0.0/tests/roots/test-latex-title/conf.py
--rw-r--r--   0        0        0      165 2023-04-23 19:57:27.572363 Sphinx-7.0.0/tests/roots/test-latex-title/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.572363 Sphinx-7.0.0/tests/roots/test-latex-unicode/conf.py
--rw-r--r--   0        0        0      142 2023-04-23 19:57:27.572363 Sphinx-7.0.0/tests/roots/test-latex-unicode/index.rst
--rw-r--r--   0        0        0       81 2023-04-23 19:57:27.572363 Sphinx-7.0.0/tests/roots/test-linkcheck-anchors-ignore/conf.py
--rw-r--r--   0        0        0      109 2023-04-23 19:57:27.572363 Sphinx-7.0.0/tests/roots/test-linkcheck-anchors-ignore/index.rst
--rw-r--r--   0        0        0      180 2023-04-23 19:57:27.572363 Sphinx-7.0.0/tests/roots/test-linkcheck-documents_exclude/br0ken_link.rst
--rw-r--r--   0        0        0      174 2023-04-23 19:57:27.573363 Sphinx-7.0.0/tests/roots/test-linkcheck-documents_exclude/broken_link.rst
--rw-r--r--   0        0        0      134 2023-04-23 19:57:27.573363 Sphinx-7.0.0/tests/roots/test-linkcheck-documents_exclude/conf.py
--rw-r--r--   0        0        0       40 2023-04-23 19:57:27.573363 Sphinx-7.0.0/tests/roots/test-linkcheck-documents_exclude/index.rst
--rw-r--r--   0        0        0       81 2023-04-23 19:57:27.573363 Sphinx-7.0.0/tests/roots/test-linkcheck-localserver-anchor/conf.py
--rw-r--r--   0        0        0       48 2023-04-23 19:57:27.573363 Sphinx-7.0.0/tests/roots/test-linkcheck-localserver-anchor/index.rst
--rw-r--r--   0        0        0       56 2023-04-23 19:57:27.573363 Sphinx-7.0.0/tests/roots/test-linkcheck-localserver-https/conf.py
--rw-r--r--   0        0        0       42 2023-04-23 19:57:27.574363 Sphinx-7.0.0/tests/roots/test-linkcheck-localserver-https/index.rst
--rw-r--r--   0        0        0       56 2023-04-23 19:57:27.574363 Sphinx-7.0.0/tests/roots/test-linkcheck-localserver-warn-redirects/conf.py
--rw-r--r--   0        0        0       95 2023-04-23 19:57:27.574363 Sphinx-7.0.0/tests/roots/test-linkcheck-localserver-warn-redirects/index.rst
--rw-r--r--   0        0        0       56 2023-04-23 19:57:27.574363 Sphinx-7.0.0/tests/roots/test-linkcheck-localserver/conf.py
--rw-r--r--   0        0        0       41 2023-04-23 19:57:27.574363 Sphinx-7.0.0/tests/roots/test-linkcheck-localserver/index.rst
--rw-r--r--   0        0        0       56 2023-04-23 19:57:27.574363 Sphinx-7.0.0/tests/roots/test-linkcheck-raw-node/conf.py
--rw-r--r--   0        0        0       46 2023-04-23 19:57:27.575363 Sphinx-7.0.0/tests/roots/test-linkcheck-raw-node/index.rst
--rw-r--r--   0        0        0       81 2023-04-23 19:57:27.575574 Sphinx-7.0.0/tests/roots/test-linkcheck-too-many-retries/conf.py
--rw-r--r--   0        0        0       73 2023-04-23 19:57:27.575574 Sphinx-7.0.0/tests/roots/test-linkcheck-too-many-retries/index.rst
--rw-r--r--   0        0        0      100 2023-04-23 19:57:27.575574 Sphinx-7.0.0/tests/roots/test-linkcheck/conf.py
--rw-r--r--   0        0        0      582 2023-04-23 19:57:27.575574 Sphinx-7.0.0/tests/roots/test-linkcheck/links.rst
--rw-r--r--   0        0        0      143 2023-04-23 19:57:27.575574 Sphinx-7.0.0/tests/roots/test-local-logo/conf.py
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.576581 Sphinx-7.0.0/tests/roots/test-local-logo/images/img.png
--rw-r--r--   0        0        0     1477 2023-04-27 00:31:27.936073 Sphinx-7.0.0/tests/roots/test-local-logo/index.rst
--rw-r--r--   0        0        0       80 2023-04-23 19:57:27.576581 Sphinx-7.0.0/tests/roots/test-locale/locale1/en/LC_MESSAGES/myext.mo
--rw-r--r--   0        0        0       41 2023-04-23 19:57:27.577582 Sphinx-7.0.0/tests/roots/test-locale/locale1/en/LC_MESSAGES/myext.po
--rw-r--r--   0        0        0       80 2023-04-23 19:57:27.577582 Sphinx-7.0.0/tests/roots/test-locale/locale1/et/LC_MESSAGES/myext.mo
--rw-r--r--   0        0        0       41 2023-04-23 19:57:27.577582 Sphinx-7.0.0/tests/roots/test-locale/locale1/et/LC_MESSAGES/myext.po
--rw-r--r--   0        0        0       82 2023-04-23 19:57:27.577582 Sphinx-7.0.0/tests/roots/test-locale/locale2/en/LC_MESSAGES/myext.mo
--rw-r--r--   0        0        0       43 2023-04-23 19:57:27.578581 Sphinx-7.0.0/tests/roots/test-locale/locale2/en/LC_MESSAGES/myext.po
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.578581 Sphinx-7.0.0/tests/roots/test-manpage_url/conf.py
--rw-r--r--   0        0        0       61 2023-04-23 19:57:27.578581 Sphinx-7.0.0/tests/roots/test-manpage_url/index.rst
--rw-r--r--   0        0        0      114 2023-04-23 19:57:27.578581 Sphinx-7.0.0/tests/roots/test-markup-citation/conf.py
--rw-r--r--   0        0        0      166 2023-04-23 19:57:27.578581 Sphinx-7.0.0/tests/roots/test-markup-citation/index.rst
--rw-r--r--   0        0        0      114 2023-04-23 19:57:27.578581 Sphinx-7.0.0/tests/roots/test-markup-rubric/conf.py
--rw-r--r--   0        0        0      112 2023-04-23 19:57:27.579581 Sphinx-7.0.0/tests/roots/test-markup-rubric/index.rst
--rw-r--r--   0        0        0       78 2023-04-23 19:57:27.579581 Sphinx-7.0.0/tests/roots/test-maxlistdepth/conf.py
--rw-r--r--   0        0        0      687 2023-04-23 19:57:27.579581 Sphinx-7.0.0/tests/roots/test-maxlistdepth/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.579581 Sphinx-7.0.0/tests/roots/test-metadata/conf.py
--rw-r--r--   0        0        0     1436 2023-04-23 19:57:27.579581 Sphinx-7.0.0/tests/roots/test-metadata/index.rst
--rw-r--r--   0        0        0        8 2023-04-23 19:57:27.579581 Sphinx-7.0.0/tests/roots/test-need-escaped/bar.rst
--rw-r--r--   0        0        0        8 2023-04-23 19:57:27.579581 Sphinx-7.0.0/tests/roots/test-need-escaped/baz.rst
--rw-r--r--   0        0        0       62 2023-04-23 19:57:27.580581 Sphinx-7.0.0/tests/roots/test-need-escaped/conf.py
--rw-r--r--   0        0        0       82 2023-04-23 19:57:27.580581 Sphinx-7.0.0/tests/roots/test-need-escaped/foo.rst
--rw-r--r--   0        0        0      574 2023-04-23 19:57:27.580581 Sphinx-7.0.0/tests/roots/test-need-escaped/index.rst
--rw-r--r--   0        0        0       10 2023-04-23 19:57:27.580581 Sphinx-7.0.0/tests/roots/test-need-escaped/quux.rst
--rw-r--r--   0        0        0       29 2023-04-23 19:57:27.580581 Sphinx-7.0.0/tests/roots/test-need-escaped/qux.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.580581 Sphinx-7.0.0/tests/roots/test-nested-enumerated-list/conf.py
--rw-r--r--   0        0        0      300 2023-04-23 19:57:27.580581 Sphinx-7.0.0/tests/roots/test-nested-enumerated-list/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.581582 Sphinx-7.0.0/tests/roots/test-nested-tables/conf.py
--rw-r--r--   0        0        0      248 2023-04-23 19:57:27.581582 Sphinx-7.0.0/tests/roots/test-nested-tables/index.rst
--rw-r--r--   0        0        0       16 2023-04-23 19:57:27.581582 Sphinx-7.0.0/tests/roots/test-nitpicky-warnings/conf.py
--rw-r--r--   0        0        0      176 2023-04-23 19:57:27.581582 Sphinx-7.0.0/tests/roots/test-nitpicky-warnings/index.rst
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.581582 Sphinx-7.0.0/tests/roots/test-numbered-circular/conf.py
--rw-r--r--   0        0        0       36 2023-04-23 19:57:27.581582 Sphinx-7.0.0/tests/roots/test-numbered-circular/index.rst
--rw-r--r--   0        0        0       23 2023-04-23 19:57:27.581582 Sphinx-7.0.0/tests/roots/test-numbered-circular/sub.rst
--rw-r--r--   0        0        0      710 2023-04-23 19:57:27.582581 Sphinx-7.0.0/tests/roots/test-numfig/bar.rst
--rw-r--r--   0        0        0      259 2023-04-23 19:57:27.582581 Sphinx-7.0.0/tests/roots/test-numfig/baz.rst
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.582581 Sphinx-7.0.0/tests/roots/test-numfig/conf.py
--rw-r--r--   0        0        0      912 2023-04-23 19:57:27.582581 Sphinx-7.0.0/tests/roots/test-numfig/foo.rst
--rw-r--r--   0        0        0     1024 2023-04-23 19:57:27.582581 Sphinx-7.0.0/tests/roots/test-numfig/index.rst
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.582581 Sphinx-7.0.0/tests/roots/test-numfig/rimg.png
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.582581 Sphinx-7.0.0/tests/roots/test-object-description-sections/conf.py
--rw-r--r--   0        0        0       80 2023-04-23 19:57:27.582581 Sphinx-7.0.0/tests/roots/test-object-description-sections/index.rst
--rw-r--r--   0        0        0       73 2023-04-23 19:57:27.583581 Sphinx-7.0.0/tests/roots/test-productionlist/Bare.rst
--rw-r--r--   0        0        0       58 2023-04-23 19:57:27.583581 Sphinx-7.0.0/tests/roots/test-productionlist/Dup1.rst
--rw-r--r--   0        0        0       58 2023-04-23 19:57:27.583581 Sphinx-7.0.0/tests/roots/test-productionlist/Dup2.rst
--rw-r--r--   0        0        0       94 2023-04-23 19:57:27.583581 Sphinx-7.0.0/tests/roots/test-productionlist/LineContinuation.rst
--rw-r--r--   0        0        0       72 2023-04-23 19:57:27.583581 Sphinx-7.0.0/tests/roots/test-productionlist/P1.rst
--rw-r--r--   0        0        0       72 2023-04-23 19:57:27.583581 Sphinx-7.0.0/tests/roots/test-productionlist/P2.rst
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.583581 Sphinx-7.0.0/tests/roots/test-productionlist/conf.py
--rw-r--r--   0        0        0       97 2023-04-23 19:57:27.583581 Sphinx-7.0.0/tests/roots/test-productionlist/firstLineRule.rst
--rw-r--r--   0        0        0      663 2023-04-23 19:57:27.584581 Sphinx-7.0.0/tests/roots/test-productionlist/index.rst
--rw-r--r--   0        0        0      177 2023-04-23 19:57:27.584581 Sphinx-7.0.0/tests/roots/test-prolog/conf.py
--rw-r--r--   0        0        0       83 2023-04-23 19:57:27.584581 Sphinx-7.0.0/tests/roots/test-prolog/index.rst
--rw-r--r--   0        0        0       57 2023-04-23 19:57:27.584581 Sphinx-7.0.0/tests/roots/test-prolog/markdown.md
--rw-r--r--   0        0        0      299 2023-04-23 19:57:27.584581 Sphinx-7.0.0/tests/roots/test-prolog/prolog_markdown_parser.py
--rw-r--r--   0        0        0       67 2023-04-23 19:57:27.584581 Sphinx-7.0.0/tests/roots/test-prolog/restructuredtext.rst
--rw-r--r--   0        0        0       75 2023-04-25 10:59:46.885153 Sphinx-7.0.0/tests/roots/test-pycode/cp_1251_coded.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.585581 Sphinx-7.0.0/tests/roots/test-reST-code-block/conf.py
--rw-r--r--   0        0        0       97 2023-04-23 19:57:27.585581 Sphinx-7.0.0/tests/roots/test-reST-code-block/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.585581 Sphinx-7.0.0/tests/roots/test-reST-code-role/conf.py
--rw-r--r--   0        0        0      194 2023-04-23 19:57:27.585581 Sphinx-7.0.0/tests/roots/test-reST-code-role/index.rst
--rw-r--r--   0        0        0       27 2023-04-23 19:57:27.585581 Sphinx-7.0.0/tests/roots/test-refonly_bullet_list/conf.py
--rw-r--r--   0        0        0      147 2023-04-23 19:57:27.585581 Sphinx-7.0.0/tests/roots/test-refonly_bullet_list/index.rst
--rw-r--r--   0        0        0      237 2023-04-23 19:57:27.586581 Sphinx-7.0.0/tests/roots/test-remote-logo/conf.py
--rw-r--r--   0        0        0     1477 2023-04-27 00:31:27.936073 Sphinx-7.0.0/tests/roots/test-remote-logo/index.rst
--rw-r--r--   0        0        0       32 2023-04-23 19:57:27.586581 Sphinx-7.0.0/tests/roots/test-roles-download/another/dummy.dat
--rw-r--r--   0        0        0      114 2023-04-23 19:57:27.586581 Sphinx-7.0.0/tests/roots/test-roles-download/conf.py
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.586581 Sphinx-7.0.0/tests/roots/test-roles-download/dummy.dat
--rw-r--r--   0        0        0      214 2023-04-23 19:57:27.586581 Sphinx-7.0.0/tests/roots/test-roles-download/index.rst
--rw-r--r--   0        0        0     2111 2023-04-23 19:57:27.586581 Sphinx-7.0.0/tests/roots/test-root/Makefile
--rw-r--r--   0        0        0       67 2023-04-23 19:57:27.587581 Sphinx-7.0.0/tests/roots/test-root/_templates/contentssb.html
--rw-r--r--   0        0        0       99 2023-04-23 19:57:27.587581 Sphinx-7.0.0/tests/roots/test-root/_templates/customsb.html
--rw-r--r--   0        0        0      428 2023-04-23 19:57:27.587581 Sphinx-7.0.0/tests/roots/test-root/_templates/layout.html
--rw-r--r--   0        0        0      578 2023-04-23 19:57:27.587581 Sphinx-7.0.0/tests/roots/test-root/autodoc.txt
--rw-r--r--   0        0        0     4587 2023-04-23 19:57:27.587581 Sphinx-7.0.0/tests/roots/test-root/autodoc_target.py
--rw-r--r--   0        0        0       74 2023-04-23 19:57:27.587581 Sphinx-7.0.0/tests/roots/test-root/bom.txt
--rw-r--r--   0        0        0     4257 2023-04-23 19:57:27.588581 Sphinx-7.0.0/tests/roots/test-root/conf.py
--rw-r--r--   0        0        0       87 2023-04-23 19:57:27.588581 Sphinx-7.0.0/tests/roots/test-root/extapi.txt
--rw-r--r--   0        0        0      365 2023-04-23 19:57:27.588581 Sphinx-7.0.0/tests/roots/test-root/extensions.txt
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.588581 Sphinx-7.0.0/tests/roots/test-root/file_with_special_#_chars.xyz
--rw-r--r--   0        0        0      826 2023-04-23 19:57:27.588581 Sphinx-7.0.0/tests/roots/test-root/footnote.txt
--rw-r--r--   0        0        0      575 2023-04-23 19:57:27.588581 Sphinx-7.0.0/tests/roots/test-root/images.txt
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.588581 Sphinx-7.0.0/tests/roots/test-root/img.foo.png
--rw-r--r--   0        0        0    24976 2023-04-23 19:57:27.589582 Sphinx-7.0.0/tests/roots/test-root/img.gif
--rw-r--r--   0        0        0   141783 2023-04-23 19:57:27.590582 Sphinx-7.0.0/tests/roots/test-root/img.pdf
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.590582 Sphinx-7.0.0/tests/roots/test-root/img.png
--rw-r--r--   0        0        0     2108 2023-04-23 19:57:27.590582 Sphinx-7.0.0/tests/roots/test-root/includes.txt
--rw-r--r--   0        0        0     1118 2023-04-23 19:57:27.590582 Sphinx-7.0.0/tests/roots/test-root/index.txt
--rw-r--r--   0        0        0      750 2023-04-23 19:57:27.590582 Sphinx-7.0.0/tests/roots/test-root/lists.txt
--rw-r--r--   0        0        0      200 2023-04-23 19:57:27.590582 Sphinx-7.0.0/tests/roots/test-root/literal.inc
--rw-r--r--   0        0        0      208 2023-04-23 19:57:27.591581 Sphinx-7.0.0/tests/roots/test-root/literal_orig.inc
--rw-r--r--   0        0        0     6919 2023-04-23 19:57:27.591581 Sphinx-7.0.0/tests/roots/test-root/markup.txt
--rw-r--r--   0        0        0      373 2023-04-23 19:57:27.591581 Sphinx-7.0.0/tests/roots/test-root/math.txt
--rw-r--r--   0        0        0     4561 2023-04-23 19:57:27.591581 Sphinx-7.0.0/tests/roots/test-root/objects.txt
--rw-r--r--   0        0        0      110 2023-04-23 19:57:27.591581 Sphinx-7.0.0/tests/roots/test-root/otherext.foo
--rw-r--r--   0        0        0      346 2023-04-23 19:57:27.591581 Sphinx-7.0.0/tests/roots/test-root/parsermod.py
--rw-r--r--   0        0        0       45 2023-04-23 19:57:27.591581 Sphinx-7.0.0/tests/roots/test-root/quotes.inc
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.591581 Sphinx-7.0.0/tests/roots/test-root/rimg.png
--rw-r--r--   0        0        0       40 2023-04-23 19:57:27.592581 Sphinx-7.0.0/tests/roots/test-root/special/api.h
--rw-r--r--   0        0        0       32 2023-04-23 19:57:27.592581 Sphinx-7.0.0/tests/roots/test-root/special/code.py
--rw-r--r--   0        0        0       96 2023-04-23 19:57:27.592581 Sphinx-7.0.0/tests/roots/test-root/subdir/excluded.txt
--rw-r--r--   0        0        0      106 2023-04-23 19:57:27.592581 Sphinx-7.0.0/tests/roots/test-root/subdir/images.txt
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.593582 Sphinx-7.0.0/tests/roots/test-root/subdir/img.png
--rw-r--r--   0        0        0      143 2023-04-23 19:57:27.593582 Sphinx-7.0.0/tests/roots/test-root/subdir/include.inc
--rw-r--r--   0        0        0      328 2023-04-23 19:57:27.593582 Sphinx-7.0.0/tests/roots/test-root/subdir/includes.txt
--rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.593582 Sphinx-7.0.0/tests/roots/test-root/subdir/simg.png
--rw-r--r--   0        0        0   141783 2023-04-23 19:57:27.594581 Sphinx-7.0.0/tests/roots/test-root/svgimg.pdf
--rw-r--r--   0        0        0      243 2023-04-23 19:57:27.594581 Sphinx-7.0.0/tests/roots/test-root/svgimg.svg
--rw-r--r--   0        0        0       78 2023-04-23 19:57:27.595582 Sphinx-7.0.0/tests/roots/test-root/tabs.inc
--rw-r--r--   0        0        0       77 2023-04-23 19:57:27.595582 Sphinx-7.0.0/tests/roots/test-root/test.inc
--rw-r--r--   0        0        0      107 2023-04-23 19:57:27.595582 Sphinx-7.0.0/tests/roots/test-root/wrongenc.inc
--rw-r--r--   0        0        0       58 2023-04-23 19:57:27.595582 Sphinx-7.0.0/tests/roots/test-search/conf.py
--rw-r--r--   0        0        0      381 2023-04-23 19:57:27.595582 Sphinx-7.0.0/tests/roots/test-search/index.rst
--rw-r--r--   0        0        0       41 2023-04-23 19:57:27.595582 Sphinx-7.0.0/tests/roots/test-search/nosearch.rst
--rw-r--r--   0        0        0      184 2023-04-23 19:57:27.595582 Sphinx-7.0.0/tests/roots/test-search/tocitem.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.596580 Sphinx-7.0.0/tests/roots/test-smartquotes/conf.py
--rw-r--r--   0        0        0      107 2023-04-23 19:57:27.596580 Sphinx-7.0.0/tests/roots/test-smartquotes/index.rst
--rw-r--r--   0        0        0      231 2023-04-23 19:57:27.596580 Sphinx-7.0.0/tests/roots/test-smartquotes/literals.rst
--rw-r--r--   0        0        0      453 2023-04-23 19:57:27.596580 Sphinx-7.0.0/tests/roots/test-stylesheets/_templates/layout.html
--rw-r--r--   0        0        0      318 2023-04-23 19:57:27.596580 Sphinx-7.0.0/tests/roots/test-stylesheets/conf.py
--rw-r--r--   0        0        0       53 2023-04-23 19:57:27.596580 Sphinx-7.0.0/tests/roots/test-stylesheets/index.rst
--rw-r--r--   0        0        0      182 2023-04-23 19:57:27.597580 Sphinx-7.0.0/tests/roots/test-templating/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      109 2023-04-23 19:57:27.597580 Sphinx-7.0.0/tests/roots/test-templating/_templates/layout.html
--rw-r--r--   0        0        0      135 2023-04-23 19:57:27.597580 Sphinx-7.0.0/tests/roots/test-templating/autosummary_templating.txt
--rw-r--r--   0        0        0      266 2023-04-23 19:57:27.597580 Sphinx-7.0.0/tests/roots/test-templating/conf.py
--rw-r--r--   0        0        0      124 2023-04-23 19:57:27.597580 Sphinx-7.0.0/tests/roots/test-templating/index.txt
--rw-r--r--   0        0        0      661 2023-04-23 19:57:27.598581 Sphinx-7.0.0/tests/roots/test-theming/child.zip
--rw-r--r--   0        0        0       94 2023-04-23 19:57:27.598581 Sphinx-7.0.0/tests/roots/test-theming/conf.py
--rw-r--r--   0        0        0       26 2023-04-23 19:57:27.598581 Sphinx-7.0.0/tests/roots/test-theming/index.rst
--rw-r--r--   0        0        0     1039 2023-04-23 19:57:27.599582 Sphinx-7.0.0/tests/roots/test-theming/parent.zip
--rw-r--r--   0        0        0       82 2023-04-23 19:57:27.599582 Sphinx-7.0.0/tests/roots/test-theming/test_theme/__init__.py
--rw-r--r--   0        0        0      139 2023-04-23 19:57:27.599582 Sphinx-7.0.0/tests/roots/test-theming/test_theme/staticfiles/layout.html
--rw-r--r--   0        0        0      120 2023-04-23 19:57:27.599582 Sphinx-7.0.0/tests/roots/test-theming/test_theme/staticfiles/static/staticimg.png
--rw-r--r--   0        0        0       82 2023-04-23 19:57:27.600582 Sphinx-7.0.0/tests/roots/test-theming/test_theme/staticfiles/static/statictmpl.html_t
--rw-r--r--   0        0        0      104 2023-04-23 19:57:27.600582 Sphinx-7.0.0/tests/roots/test-theming/test_theme/staticfiles/theme.conf
--rw-r--r--   0        0        0       98 2023-04-23 19:57:27.600582 Sphinx-7.0.0/tests/roots/test-theming/test_theme/test-theme/theme.conf
--rw-r--r--   0        0        0     1039 2023-04-23 19:57:27.600582 Sphinx-7.0.0/tests/roots/test-theming/ziptheme.zip
--rw-r--r--   0        0        0      150 2023-04-23 19:57:27.600582 Sphinx-7.0.0/tests/roots/test-tocdepth/bar.rst
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.601583 Sphinx-7.0.0/tests/roots/test-tocdepth/baz.rst
--rw-r--r--   0        0        0       53 2023-04-23 19:57:27.601583 Sphinx-7.0.0/tests/roots/test-tocdepth/conf.py
--rw-r--r--   0        0        0      146 2023-04-23 19:57:27.601583 Sphinx-7.0.0/tests/roots/test-tocdepth/foo.rst
--rw-r--r--   0        0        0       71 2023-04-23 19:57:27.601583 Sphinx-7.0.0/tests/roots/test-tocdepth/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.601583 Sphinx-7.0.0/tests/roots/test-toctree-domain-objects/conf.py
--rw-r--r--   0        0        0      731 2023-04-23 19:57:27.602583 Sphinx-7.0.0/tests/roots/test-toctree-domain-objects/domains.rst
--rw-r--r--   0        0        0       90 2023-04-23 19:57:27.602583 Sphinx-7.0.0/tests/roots/test-toctree-domain-objects/index.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.602583 Sphinx-7.0.0/tests/roots/test-toctree-duplicated/conf.py
--rw-r--r--   0        0        0        8 2023-04-23 19:57:27.602583 Sphinx-7.0.0/tests/roots/test-toctree-duplicated/foo.rst
--rw-r--r--   0        0        0       77 2023-04-23 19:57:27.602583 Sphinx-7.0.0/tests/roots/test-toctree-duplicated/index.rst
--rw-r--r--   0        0        0      101 2023-04-23 19:57:27.602583 Sphinx-7.0.0/tests/roots/test-toctree-empty/_templates/localtoc.html
--rw-r--r--   0        0        0       62 2023-04-23 19:57:27.603581 Sphinx-7.0.0/tests/roots/test-toctree-empty/conf.py
--rw-r--r--   0        0        0       52 2023-04-23 19:57:27.603581 Sphinx-7.0.0/tests/roots/test-toctree-empty/index.rst
--rw-r--r--   0        0        0       17 2023-04-23 19:57:27.603581 Sphinx-7.0.0/tests/roots/test-toctree-glob/bar/bar_1.rst
--rw-r--r--   0        0        0       17 2023-04-23 19:57:27.604581 Sphinx-7.0.0/tests/roots/test-toctree-glob/bar/bar_2.rst
--rw-r--r--   0        0        0       17 2023-04-23 19:57:27.604581 Sphinx-7.0.0/tests/roots/test-toctree-glob/bar/bar_3.rst
--rw-r--r--   0        0        0       17 2023-04-23 19:57:27.604581 Sphinx-7.0.0/tests/roots/test-toctree-glob/bar/bar_4/index.rst
--rw-r--r--   0        0        0       53 2023-04-23 19:57:27.604581 Sphinx-7.0.0/tests/roots/test-toctree-glob/bar/index.rst
--rw-r--r--   0        0        0       13 2023-04-23 19:57:27.604581 Sphinx-7.0.0/tests/roots/test-toctree-glob/baz.rst
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.604581 Sphinx-7.0.0/tests/roots/test-toctree-glob/conf.py
--rw-r--r--   0        0        0       13 2023-04-23 19:57:27.604581 Sphinx-7.0.0/tests/roots/test-toctree-glob/foo.rst
--rw-r--r--   0        0        0      303 2023-04-23 19:57:27.605581 Sphinx-7.0.0/tests/roots/test-toctree-glob/index.rst
--rw-r--r--   0        0        0       16 2023-04-23 19:57:27.605581 Sphinx-7.0.0/tests/roots/test-toctree-glob/quux.rst
--rw-r--r--   0        0        0       50 2023-04-23 19:57:27.605581 Sphinx-7.0.0/tests/roots/test-toctree-glob/qux/index.rst
--rw-r--r--   0        0        0       17 2023-04-23 19:57:27.605581 Sphinx-7.0.0/tests/roots/test-toctree-glob/qux/qux_1.rst
--rw-r--r--   0        0        0       17 2023-04-23 19:57:27.606581 Sphinx-7.0.0/tests/roots/test-toctree-glob/qux/qux_2.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.606581 Sphinx-7.0.0/tests/roots/test-toctree-index/conf.py
--rw-r--r--   0        0        0      105 2023-04-23 19:57:27.606581 Sphinx-7.0.0/tests/roots/test-toctree-index/foo.rst
--rw-r--r--   0        0        0      132 2023-04-23 19:57:27.606581 Sphinx-7.0.0/tests/roots/test-toctree-index/index.rst
--rw-r--r--   0        0        0      150 2023-04-23 19:57:27.606581 Sphinx-7.0.0/tests/roots/test-toctree-maxdepth/bar.rst
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.606581 Sphinx-7.0.0/tests/roots/test-toctree-maxdepth/baz.rst
--rw-r--r--   0        0        0       30 2023-04-23 19:57:27.607582 Sphinx-7.0.0/tests/roots/test-toctree-maxdepth/conf.py
--rw-r--r--   0        0        0      146 2023-04-23 19:57:27.607582 Sphinx-7.0.0/tests/roots/test-toctree-maxdepth/foo.rst
--rw-r--r--   0        0        0      105 2023-04-23 19:57:27.607582 Sphinx-7.0.0/tests/roots/test-toctree-maxdepth/index.rst
--rw-r--r--   0        0        0      105 2023-04-23 19:57:27.607582 Sphinx-7.0.0/tests/roots/test-toctree-maxdepth/qux.rst
--rw-r--r--   0        0        0        8 2023-04-23 19:57:27.607582 Sphinx-7.0.0/tests/roots/test-toctree/bar.rst
--rw-r--r--   0        0        0        8 2023-04-23 19:57:27.607582 Sphinx-7.0.0/tests/roots/test-toctree/baz.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.607582 Sphinx-7.0.0/tests/roots/test-toctree/conf.py
--rw-r--r--   0        0        0       74 2023-04-23 19:57:27.608580 Sphinx-7.0.0/tests/roots/test-toctree/foo.rst
--rw-r--r--   0        0        0      885 2023-04-23 19:57:27.608580 Sphinx-7.0.0/tests/roots/test-toctree/index.rst
--rw-r--r--   0        0        0       10 2023-04-23 19:57:27.608580 Sphinx-7.0.0/tests/roots/test-toctree/quux.rst
--rw-r--r--   0        0        0       29 2023-04-23 19:57:27.608580 Sphinx-7.0.0/tests/roots/test-toctree/qux.rst
--rw-r--r--   0        0        0       97 2023-04-23 19:57:27.608580 Sphinx-7.0.0/tests/roots/test-toctree/tocdepth.rst
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.608580 Sphinx-7.0.0/tests/roots/test-transforms-post_transforms-keyboard/conf.py
--rw-r--r--   0        0        0       94 2023-04-23 19:57:27.609582 Sphinx-7.0.0/tests/roots/test-transforms-post_transforms-keyboard/index.rst
--rw-r--r--   0        0        0       16 2023-04-23 19:57:27.609582 Sphinx-7.0.0/tests/roots/test-transforms-post_transforms-missing-reference/conf.py
--rw-r--r--   0        0        0      113 2023-04-23 19:57:27.609582 Sphinx-7.0.0/tests/roots/test-transforms-post_transforms-missing-reference/index.rst
--rw-r--r--   0        0        0       36 2023-04-23 19:57:27.609582 Sphinx-7.0.0/tests/roots/test-trim_doctest_flags/conf.py
--rw-r--r--   0        0        0      784 2023-04-23 19:57:27.609582 Sphinx-7.0.0/tests/roots/test-trim_doctest_flags/index.rst
--rw-r--r--   0        0        0     1012 2023-04-23 19:57:27.610582 Sphinx-7.0.0/tests/roots/test-versioning/added.txt
--rw-r--r--   0        0        0       86 2023-04-23 19:57:27.610582 Sphinx-7.0.0/tests/roots/test-versioning/conf.py
--rw-r--r--   0        0        0      584 2023-04-23 19:57:27.610582 Sphinx-7.0.0/tests/roots/test-versioning/deleted.txt
--rw-r--r--   0        0        0      490 2023-04-23 19:57:27.610582 Sphinx-7.0.0/tests/roots/test-versioning/deleted_end.txt
--rw-r--r--   0        0        0      164 2023-04-23 19:57:27.610582 Sphinx-7.0.0/tests/roots/test-versioning/index.txt
--rw-r--r--   0        0        0      864 2023-04-23 19:57:27.610582 Sphinx-7.0.0/tests/roots/test-versioning/insert.txt
--rw-r--r--   0        0        0      850 2023-04-23 19:57:27.611492 Sphinx-7.0.0/tests/roots/test-versioning/insert_beginning.txt
--rw-r--r--   0        0        0      735 2023-04-23 19:57:27.611492 Sphinx-7.0.0/tests/roots/test-versioning/insert_similar.txt
--rw-r--r--   0        0        0      867 2023-04-23 19:57:27.611492 Sphinx-7.0.0/tests/roots/test-versioning/modified.txt
--rw-r--r--   0        0        0      715 2023-04-23 19:57:27.611492 Sphinx-7.0.0/tests/roots/test-versioning/original.txt
--rw-r--r--   0        0        0      151 2023-04-23 19:57:27.611492 Sphinx-7.0.0/tests/roots/test-warnings/autodoc_fodder.py
--rw-r--r--   0        0        0       97 2023-04-23 19:57:27.611492 Sphinx-7.0.0/tests/roots/test-warnings/conf.py
--rw-r--r--   0        0        0      697 2023-04-23 19:57:27.612498 Sphinx-7.0.0/tests/roots/test-warnings/index.rst
--rw-r--r--   0        0        0   141783 2023-04-23 19:57:27.613498 Sphinx-7.0.0/tests/roots/test-warnings/svgimg.pdf
--rw-r--r--   0        0        0      243 2023-04-23 19:57:27.613498 Sphinx-7.0.0/tests/roots/test-warnings/svgimg.svg
--rw-r--r--   0        0        0       18 2023-04-23 19:57:27.613498 Sphinx-7.0.0/tests/roots/test-warnings/undecodable.rst
--rw-r--r--   0        0        0      107 2023-04-23 19:57:27.613498 Sphinx-7.0.0/tests/roots/test-warnings/wrongenc.inc
--rw-r--r--   0        0        0     3309 2023-04-23 19:57:27.613498 Sphinx-7.0.0/tests/test_api_translator.py
--rw-r--r--   0        0        0     5605 2023-04-23 19:57:27.614498 Sphinx-7.0.0/tests/test_application.py
--rw-r--r--   0        0        0     4771 2023-04-23 19:57:27.614498 Sphinx-7.0.0/tests/test_build.py
--rw-r--r--   0        0        0     1152 2023-04-23 19:57:27.614498 Sphinx-7.0.0/tests/test_build_changes.py
--rw-r--r--   0        0        0     1407 2023-04-23 19:57:27.614498 Sphinx-7.0.0/tests/test_build_dirhtml.py
--rw-r--r--   0        0        0    16623 2023-04-23 19:57:27.615497 Sphinx-7.0.0/tests/test_build_epub.py
--rw-r--r--   0        0        0     6660 2023-04-23 19:57:27.615497 Sphinx-7.0.0/tests/test_build_gettext.py
--rw-r--r--   0        0        0    80591 2023-04-28 10:59:41.037038 Sphinx-7.0.0/tests/test_build_html.py
--rw-r--r--   0        0        0    75378 2023-04-23 19:57:27.616498 Sphinx-7.0.0/tests/test_build_latex.py
--rw-r--r--   0        0        0    24262 2023-04-23 19:57:27.616498 Sphinx-7.0.0/tests/test_build_linkcheck.py
--rw-r--r--   0        0        0     2751 2023-04-23 19:57:27.616498 Sphinx-7.0.0/tests/test_build_manpage.py
--rw-r--r--   0        0        0     5910 2023-04-23 19:57:27.616498 Sphinx-7.0.0/tests/test_build_texinfo.py
--rw-r--r--   0        0        0     8996 2023-04-23 19:57:27.617498 Sphinx-7.0.0/tests/test_build_text.py
--rw-r--r--   0        0        0     1322 2023-04-23 19:57:27.617498 Sphinx-7.0.0/tests/test_builder.py
--rw-r--r--   0        0        0     2646 2023-04-23 19:57:27.617498 Sphinx-7.0.0/tests/test_catalogs.py
--rw-r--r--   0        0        0    15085 2023-04-26 16:05:03.832456 Sphinx-7.0.0/tests/test_config.py
--rw-r--r--   0        0        0      811 2023-04-23 19:57:27.617967 Sphinx-7.0.0/tests/test_correct_year.py
--rw-r--r--   0        0        0    23761 2023-04-23 19:57:27.617967 Sphinx-7.0.0/tests/test_directive_code.py
--rw-r--r--   0        0        0     2088 2023-04-23 19:57:27.617967 Sphinx-7.0.0/tests/test_directive_object_description.py
--rw-r--r--   0        0        0     1655 2023-04-23 19:57:27.618752 Sphinx-7.0.0/tests/test_directive_only.py
--rw-r--r--   0        0        0     5207 2023-04-23 19:57:27.618752 Sphinx-7.0.0/tests/test_directive_other.py
--rw-r--r--   0        0        0     4362 2023-04-23 19:57:27.619179 Sphinx-7.0.0/tests/test_directive_patch.py
--rw-r--r--   0        0        0     1084 2023-04-23 19:57:27.619179 Sphinx-7.0.0/tests/test_docutilsconf.py
--rw-r--r--   0        0        0    28522 2023-04-23 19:57:27.619179 Sphinx-7.0.0/tests/test_domain_c.py
--rw-r--r--   0        0        0    67113 2023-04-23 19:57:27.620191 Sphinx-7.0.0/tests/test_domain_cpp.py
--rw-r--r--   0        0        0    10933 2023-04-23 19:57:27.620393 Sphinx-7.0.0/tests/test_domain_js.py
--rw-r--r--   0        0        0    76403 2023-04-23 19:57:27.620829 Sphinx-7.0.0/tests/test_domain_py.py
--rw-r--r--   0        0        0     5896 2023-04-23 19:57:27.620829 Sphinx-7.0.0/tests/test_domain_rst.py
--rw-r--r--   0        0        0    19424 2023-04-23 19:57:27.620829 Sphinx-7.0.0/tests/test_domain_std.py
--rw-r--r--   0        0        0     5286 2023-04-23 19:57:27.620829 Sphinx-7.0.0/tests/test_environment.py
--rw-r--r--   0        0        0     8068 2023-04-23 19:57:27.621840 Sphinx-7.0.0/tests/test_environment_indexentries.py
--rw-r--r--   0        0        0      310 2023-04-23 19:57:27.621840 Sphinx-7.0.0/tests/test_environment_record_dependencies.py
--rw-r--r--   0        0        0    20508 2023-04-23 19:57:27.621840 Sphinx-7.0.0/tests/test_environment_toctree.py
--rw-r--r--   0        0        0      321 2023-04-23 19:57:27.621840 Sphinx-7.0.0/tests/test_errors.py
--rw-r--r--   0        0        0     1826 2023-04-23 19:57:27.621840 Sphinx-7.0.0/tests/test_events.py
--rw-r--r--   0        0        0    23255 2023-04-23 19:57:27.621840 Sphinx-7.0.0/tests/test_ext_apidoc.py
--rw-r--r--   0        0        0    76880 2023-04-23 19:57:27.622839 Sphinx-7.0.0/tests/test_ext_autodoc.py
--rw-r--r--   0        0        0     4801 2023-04-23 19:57:27.622839 Sphinx-7.0.0/tests/test_ext_autodoc_autoattribute.py
--rw-r--r--   0        0        0    14272 2023-04-23 19:57:27.622839 Sphinx-7.0.0/tests/test_ext_autodoc_autoclass.py
--rw-r--r--   0        0        0     2631 2023-04-23 19:57:27.622839 Sphinx-7.0.0/tests/test_ext_autodoc_autodata.py
--rw-r--r--   0        0        0     5647 2023-04-23 19:57:27.623839 Sphinx-7.0.0/tests/test_ext_autodoc_autofunction.py
--rw-r--r--   0        0        0     5355 2023-04-23 19:57:27.624010 Sphinx-7.0.0/tests/test_ext_autodoc_automodule.py
--rw-r--r--   0        0        0     2501 2023-04-23 19:57:27.624010 Sphinx-7.0.0/tests/test_ext_autodoc_autoproperty.py
--rw-r--r--   0        0        0    55422 2023-04-23 19:57:27.624010 Sphinx-7.0.0/tests/test_ext_autodoc_configs.py
--rw-r--r--   0        0        0     3335 2023-04-23 19:57:27.625016 Sphinx-7.0.0/tests/test_ext_autodoc_events.py
--rw-r--r--   0        0        0     3963 2023-04-23 19:57:27.625016 Sphinx-7.0.0/tests/test_ext_autodoc_mock.py
--rw-r--r--   0        0        0     1666 2023-04-23 19:57:27.625016 Sphinx-7.0.0/tests/test_ext_autodoc_preserve_defaults.py
--rw-r--r--   0        0        0     4415 2023-04-23 19:57:27.625016 Sphinx-7.0.0/tests/test_ext_autodoc_private_members.py
--rw-r--r--   0        0        0     3145 2023-04-23 19:57:27.625016 Sphinx-7.0.0/tests/test_ext_autosectionlabel.py
--rw-r--r--   0        0        0    27705 2023-04-23 19:57:27.626128 Sphinx-7.0.0/tests/test_ext_autosummary.py
--rw-r--r--   0        0        0     3158 2023-04-23 19:57:27.626507 Sphinx-7.0.0/tests/test_ext_coverage.py
--rw-r--r--   0        0        0     5524 2023-04-23 19:57:27.626635 Sphinx-7.0.0/tests/test_ext_doctest.py
--rw-r--r--   0        0        0      378 2023-04-23 19:57:27.626635 Sphinx-7.0.0/tests/test_ext_duration.py
--rw-r--r--   0        0        0     2104 2023-04-23 19:57:27.626635 Sphinx-7.0.0/tests/test_ext_extlinks.py
--rw-r--r--   0        0        0      958 2023-04-23 19:57:27.626635 Sphinx-7.0.0/tests/test_ext_githubpages.py
--rw-r--r--   0        0        0     7667 2023-04-23 19:57:27.626635 Sphinx-7.0.0/tests/test_ext_graphviz.py
--rw-r--r--   0        0        0      850 2023-04-23 19:57:27.626635 Sphinx-7.0.0/tests/test_ext_ifconfig.py
--rw-r--r--   0        0        0     1038 2023-04-23 19:57:27.627705 Sphinx-7.0.0/tests/test_ext_imgconverter.py
--rw-r--r--   0        0        0      609 2023-04-23 19:57:27.627705 Sphinx-7.0.0/tests/test_ext_imgmockconverter.py
--rw-r--r--   0        0        0    10579 2023-04-23 19:57:27.627705 Sphinx-7.0.0/tests/test_ext_inheritance_diagram.py
--rw-r--r--   0        0        0    21393 2023-04-23 19:57:27.627705 Sphinx-7.0.0/tests/test_ext_intersphinx.py
--rw-r--r--   0        0        0    13142 2023-04-23 19:57:27.628705 Sphinx-7.0.0/tests/test_ext_math.py
--rw-r--r--   0        0        0     6912 2023-04-23 19:57:27.628705 Sphinx-7.0.0/tests/test_ext_napoleon.py
--rw-r--r--   0        0        0    70796 2023-04-23 19:57:27.628705 Sphinx-7.0.0/tests/test_ext_napoleon_docstring.py
--rw-r--r--   0        0        0     3878 2023-04-23 19:57:27.629705 Sphinx-7.0.0/tests/test_ext_todo.py
--rw-r--r--   0        0        0     5467 2023-04-23 19:57:27.629705 Sphinx-7.0.0/tests/test_ext_viewcode.py
--rw-r--r--   0        0        0      857 2023-04-23 19:57:27.629705 Sphinx-7.0.0/tests/test_extension.py
--rw-r--r--   0        0        0     3563 2023-04-23 19:57:27.629705 Sphinx-7.0.0/tests/test_highlighting.py
--rw-r--r--   0        0        0    49439 2023-04-23 19:57:27.629705 Sphinx-7.0.0/tests/test_intl.py
--rw-r--r--   0        0        0     2551 2023-04-23 19:57:27.630705 Sphinx-7.0.0/tests/test_locale.py
--rw-r--r--   0        0        0    22328 2023-04-23 19:57:27.630705 Sphinx-7.0.0/tests/test_markup.py
--rw-r--r--   0        0        0     1931 2023-04-23 19:57:27.630705 Sphinx-7.0.0/tests/test_metadata.py
--rw-r--r--   0        0        0     2459 2023-04-23 19:57:27.631706 Sphinx-7.0.0/tests/test_parser.py
--rw-r--r--   0        0        0     2573 2023-04-23 19:57:27.631706 Sphinx-7.0.0/tests/test_project.py
--rw-r--r--   0        0        0     6918 2023-04-23 19:57:27.631706 Sphinx-7.0.0/tests/test_pycode.py
--rw-r--r--   0        0        0     2835 2023-04-23 19:57:27.631706 Sphinx-7.0.0/tests/test_pycode_ast.py
--rw-r--r--   0        0        0    18264 2023-04-23 19:57:27.632705 Sphinx-7.0.0/tests/test_pycode_parser.py
--rw-r--r--   0        0        0     7347 2023-04-23 19:57:27.632705 Sphinx-7.0.0/tests/test_quickstart.py
--rw-r--r--   0        0        0     2570 2023-04-23 19:57:27.632705 Sphinx-7.0.0/tests/test_roles.py
--rw-r--r--   0        0        0    11627 2023-04-23 19:57:27.632705 Sphinx-7.0.0/tests/test_search.py
--rw-r--r--   0        0        0     3747 2023-04-23 19:57:27.632705 Sphinx-7.0.0/tests/test_smartquotes.py
--rw-r--r--   0        0        0     1435 2023-04-23 19:57:27.633705 Sphinx-7.0.0/tests/test_templating.py
--rw-r--r--   0        0        0     4312 2023-04-26 16:05:03.832456 Sphinx-7.0.0/tests/test_theming.py
--rw-r--r--   0        0        0     1843 2023-04-23 19:57:27.633705 Sphinx-7.0.0/tests/test_toctree.py
--rw-r--r--   0        0        0     2231 2023-04-23 19:57:27.633705 Sphinx-7.0.0/tests/test_transforms_post_transforms.py
--rw-r--r--   0        0        0     1324 2023-04-23 19:57:27.633705 Sphinx-7.0.0/tests/test_transforms_post_transforms_code.py
--rw-r--r--   0        0        0     2799 2023-04-23 19:57:27.634705 Sphinx-7.0.0/tests/test_util.py
--rw-r--r--   0        0        0     3065 2023-04-23 19:57:27.634705 Sphinx-7.0.0/tests/test_util_display.py
--rw-r--r--   0        0        0     3032 2023-04-23 19:57:27.634705 Sphinx-7.0.0/tests/test_util_docstrings.py
--rw-r--r--   0        0        0     2647 2023-04-23 19:57:27.635341 Sphinx-7.0.0/tests/test_util_docutils.py
--rw-r--r--   0        0        0     3800 2023-04-23 19:57:27.635341 Sphinx-7.0.0/tests/test_util_fileutil.py
--rw-r--r--   0        0        0     8627 2023-04-27 00:28:57.465794 Sphinx-7.0.0/tests/test_util_i18n.py
--rw-r--r--   0        0        0     2653 2023-04-23 19:57:27.635341 Sphinx-7.0.0/tests/test_util_images.py
--rw-r--r--   0        0        0    26901 2023-04-23 19:57:27.636377 Sphinx-7.0.0/tests/test_util_inspect.py
--rw-r--r--   0        0        0     4032 2023-04-23 19:57:27.636377 Sphinx-7.0.0/tests/test_util_inventory.py
--rw-r--r--   0        0        0    13459 2023-04-23 19:57:27.636377 Sphinx-7.0.0/tests/test_util_logging.py
--rw-r--r--   0        0        0     7180 2023-04-23 19:57:27.637384 Sphinx-7.0.0/tests/test_util_matching.py
--rw-r--r--   0        0        0     7464 2023-04-23 19:57:27.637384 Sphinx-7.0.0/tests/test_util_nodes.py
--rw-r--r--   0        0        0     4556 2023-04-23 19:57:27.637384 Sphinx-7.0.0/tests/test_util_rst.py
--rw-r--r--   0        0        0      952 2023-04-23 19:57:27.637384 Sphinx-7.0.0/tests/test_util_template.py
--rw-r--r--   0        0        0    22811 2023-04-23 19:57:27.637384 Sphinx-7.0.0/tests/test_util_typing.py
--rw-r--r--   0        0        0     3561 2023-04-23 19:57:27.638376 Sphinx-7.0.0/tests/test_versioning.py
--rw-r--r--   0        0        0     1065 2023-04-23 19:57:27.638376 Sphinx-7.0.0/tests/test_writer_latex.py
--rw-r--r--   0        0        0     1859 2023-04-23 19:57:27.638376 Sphinx-7.0.0/tests/typing_test_data.py
--rw-r--r--   0        0        0     1654 2023-04-23 19:57:27.638376 Sphinx-7.0.0/tests/utils.py
--rw-r--r--   0        0        0      992 2023-04-23 19:57:27.639377 Sphinx-7.0.0/tox.ini
--rw-r--r--   0        0        0      227 2023-04-23 19:57:27.639377 Sphinx-7.0.0/utils/CHANGES_template
--rw-r--r--   0        0        0        0 2023-04-23 19:57:27.639377 Sphinx-7.0.0/utils/__init__.py
--rw-r--r--   0        0        0     8282 2023-04-23 19:57:27.640377 Sphinx-7.0.0/utils/babel_runner.py
--rw-r--r--   0        0        0      296 2023-04-25 10:59:46.885153 Sphinx-7.0.0/utils/bump_docker.sh
--rw-r--r--   0        0        0     5808 2023-04-28 21:01:36.713260 Sphinx-7.0.0/utils/bump_version.py
--rw-r--r--   0        0        0     1730 2023-04-23 19:57:27.640377 Sphinx-7.0.0/utils/release-checklist
--rw-r--r--   0        0        0     6138 1970-01-01 00:00:00.000000 Sphinx-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4070 2023-04-23 19:57:27.290387 Sphinx-7.0.0rc1/AUTHORS
+-rw-r--r--   0        0        0   369722 2023-04-28 11:31:18.602669 Sphinx-7.0.0rc1/CHANGES
+-rw-r--r--   0        0        0     3530 2023-04-23 19:57:27.292374 Sphinx-7.0.0rc1/CODE_OF_CONDUCT
+-rw-r--r--   0        0        0    26647 2023-04-23 19:57:27.293375 Sphinx-7.0.0rc1/EXAMPLES
+-rw-r--r--   0        0        0     3135 2023-04-23 19:57:27.293375 Sphinx-7.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     2654 2023-04-23 19:57:27.294379 Sphinx-7.0.0rc1/README.rst
+-rw-r--r--   0        0        0      607 2023-04-23 19:57:27.294379 Sphinx-7.0.0rc1/doc/Makefile
+-rw-r--r--   0        0        0      152 2023-04-23 19:57:27.294379 Sphinx-7.0.0rc1/doc/_static/Makefile
+-rw-r--r--   0        0        0    27523 2023-04-23 19:57:27.294379 Sphinx-7.0.0rc1/doc/_static/bookcover.png
+-rw-r--r--   0        0        0     9875 2023-04-23 19:57:27.295374 Sphinx-7.0.0rc1/doc/_static/conf.py.txt
+-rw-r--r--   0        0        0     3307 2023-04-23 19:57:27.295374 Sphinx-7.0.0rc1/doc/_static/favicon.svg
+-rw-r--r--   0        0        0     1351 2023-04-23 19:57:27.295374 Sphinx-7.0.0rc1/doc/_static/more.png
+-rw-r--r--   0        0        0    34213 2023-04-23 19:57:27.295374 Sphinx-7.0.0rc1/doc/_static/sphinx.png
+-rw-r--r--   0        0        0    25792 2023-04-23 19:57:27.296374 Sphinx-7.0.0rc1/doc/_static/themes/agogo.png
+-rw-r--r--   0        0        0    32356 2023-04-23 19:57:27.296374 Sphinx-7.0.0rc1/doc/_static/themes/alabaster.png
+-rw-r--r--   0        0        0    27139 2023-04-23 19:57:27.296374 Sphinx-7.0.0rc1/doc/_static/themes/bizstyle.png
+-rw-r--r--   0        0        0    39927 2023-04-23 19:57:27.297375 Sphinx-7.0.0rc1/doc/_static/themes/classic.png
+-rw-r--r--   0        0        0    56954 2023-04-23 19:57:27.297375 Sphinx-7.0.0rc1/doc/_static/themes/fullsize/agogo.png
+-rw-r--r--   0        0        0    40248 2023-04-23 19:57:27.297375 Sphinx-7.0.0rc1/doc/_static/themes/fullsize/alabaster.png
+-rw-r--r--   0        0        0    75192 2023-04-23 19:57:27.298374 Sphinx-7.0.0rc1/doc/_static/themes/fullsize/bizstyle.png
+-rw-r--r--   0        0        0    72597 2023-04-23 19:57:27.299374 Sphinx-7.0.0rc1/doc/_static/themes/fullsize/classic.png
+-rw-r--r--   0        0        0    84200 2023-04-23 19:57:27.299374 Sphinx-7.0.0rc1/doc/_static/themes/fullsize/haiku.png
+-rw-r--r--   0        0        0    32266 2023-04-23 19:57:27.300375 Sphinx-7.0.0rc1/doc/_static/themes/fullsize/nature.png
+-rw-r--r--   0        0        0   102717 2023-04-23 19:57:27.300375 Sphinx-7.0.0rc1/doc/_static/themes/fullsize/pyramid.png
+-rw-r--r--   0        0        0    88111 2023-04-23 19:57:27.301375 Sphinx-7.0.0rc1/doc/_static/themes/fullsize/scrolls.png
+-rw-r--r--   0        0        0    39411 2023-04-23 19:57:27.302374 Sphinx-7.0.0rc1/doc/_static/themes/fullsize/sphinx_rtd_theme.png
+-rw-r--r--   0        0        0    84439 2023-04-23 19:57:27.302374 Sphinx-7.0.0rc1/doc/_static/themes/fullsize/sphinxdoc.png
+-rw-r--r--   0        0        0    91744 2023-04-23 19:57:27.303374 Sphinx-7.0.0rc1/doc/_static/themes/fullsize/traditional.png
+-rw-r--r--   0        0        0    43184 2023-04-23 19:57:27.303374 Sphinx-7.0.0rc1/doc/_static/themes/haiku.png
+-rw-r--r--   0        0        0    28536 2023-04-23 19:57:27.303374 Sphinx-7.0.0rc1/doc/_static/themes/nature.png
+-rw-r--r--   0        0        0    38805 2023-04-23 19:57:27.304374 Sphinx-7.0.0rc1/doc/_static/themes/pyramid.png
+-rw-r--r--   0        0        0    27800 2023-04-23 19:57:27.304374 Sphinx-7.0.0rc1/doc/_static/themes/scrolls.png
+-rw-r--r--   0        0        0    29138 2023-04-23 19:57:27.304374 Sphinx-7.0.0rc1/doc/_static/themes/sphinx_rtd_theme.png
+-rw-r--r--   0        0        0    30225 2023-04-23 19:57:27.304374 Sphinx-7.0.0rc1/doc/_static/themes/sphinxdoc.png
+-rw-r--r--   0        0        0    32258 2023-04-23 19:57:27.305374 Sphinx-7.0.0rc1/doc/_static/themes/traditional.png
+-rw-r--r--   0        0        0    16371 2023-04-23 19:57:27.305374 Sphinx-7.0.0rc1/doc/_static/translation.png
+-rw-r--r--   0        0        0      342 2023-04-23 19:57:27.305374 Sphinx-7.0.0rc1/doc/_static/translation.puml
+-rw-r--r--   0        0        0     8232 2023-04-25 10:59:46.881271 Sphinx-7.0.0rc1/doc/_static/translation.svg
+-rw-r--r--   0        0        0    26500 2023-04-23 19:57:27.306374 Sphinx-7.0.0rc1/doc/_static/tutorial/lumache-autosummary.png
+-rw-r--r--   0        0        0    52126 2023-04-23 19:57:27.306374 Sphinx-7.0.0rc1/doc/_static/tutorial/lumache-first-light.png
+-rw-r--r--   0        0        0    51223 2023-04-23 19:57:27.307374 Sphinx-7.0.0rc1/doc/_static/tutorial/lumache-furo.png
+-rw-r--r--   0        0        0    71741 2023-04-23 19:57:27.308375 Sphinx-7.0.0rc1/doc/_static/tutorial/lumache-py-function-full.png
+-rw-r--r--   0        0        0    41828 2023-04-23 19:57:27.308375 Sphinx-7.0.0rc1/doc/_static/tutorial/lumache-py-function.png
+-rw-r--r--   0        0        0      225 2023-04-23 19:57:27.308375 Sphinx-7.0.0rc1/doc/_templates/contents.html
+-rw-r--r--   0        0        0     1968 2023-04-23 19:57:27.309374 Sphinx-7.0.0rc1/doc/_themes/sphinx13/layout.html
+-rw-r--r--   0        0        0     6552 2023-04-23 19:57:27.309374 Sphinx-7.0.0rc1/doc/_themes/sphinx13/static/sphinx13.css
+-rw-r--r--   0        0        0    11719 2023-04-23 19:57:27.309374 Sphinx-7.0.0rc1/doc/_themes/sphinx13/static/sphinxheader.png
+-rw-r--r--   0        0        0       60 2023-04-23 19:57:27.310374 Sphinx-7.0.0rc1/doc/_themes/sphinx13/theme.conf
+-rw-r--r--   0        0        0       98 2023-04-23 19:57:27.310374 Sphinx-7.0.0rc1/doc/authors.rst
+-rw-r--r--   0        0        0      400 2023-04-23 19:57:27.310374 Sphinx-7.0.0rc1/doc/changes.rst
+-rw-r--r--   0        0        0     9004 2023-04-27 00:31:27.920451 Sphinx-7.0.0rc1/doc/conf.py
+-rw-r--r--   0        0        0     1151 2023-04-23 19:57:27.311375 Sphinx-7.0.0rc1/doc/development/builders.rst
+-rw-r--r--   0        0        0      649 2023-04-23 19:57:27.311375 Sphinx-7.0.0rc1/doc/development/index.rst
+-rw-r--r--   0        0        0     1051 2023-04-23 19:57:27.311375 Sphinx-7.0.0rc1/doc/development/overview.rst
+-rw-r--r--   0        0        0    15048 2023-04-28 09:32:47.966025 Sphinx-7.0.0rc1/doc/development/templating.rst
+-rw-r--r--   0        0        0    12324 2023-04-23 19:57:27.312375 Sphinx-7.0.0rc1/doc/development/theming.rst
+-rw-r--r--   0        0        0     4020 2023-04-23 19:57:27.312375 Sphinx-7.0.0rc1/doc/development/tutorials/autodoc_ext.rst
+-rw-r--r--   0        0        0      438 2023-04-23 19:57:27.312375 Sphinx-7.0.0rc1/doc/development/tutorials/examples/README.rst
+-rw-r--r--   0        0        0     1802 2023-04-23 19:57:27.312375 Sphinx-7.0.0rc1/doc/development/tutorials/examples/autodoc_intenum.py
+-rw-r--r--   0        0        0      400 2023-04-23 19:57:27.312375 Sphinx-7.0.0rc1/doc/development/tutorials/examples/helloworld.py
+-rw-r--r--   0        0        0     5030 2023-04-23 19:57:27.313375 Sphinx-7.0.0rc1/doc/development/tutorials/examples/recipe.py
+-rw-r--r--   0        0        0     3942 2023-04-23 19:57:27.313375 Sphinx-7.0.0rc1/doc/development/tutorials/examples/todo.py
+-rw-r--r--   0        0        0     5289 2023-04-23 19:57:27.313375 Sphinx-7.0.0rc1/doc/development/tutorials/helloworld.rst
+-rw-r--r--   0        0        0      262 2023-04-23 19:57:27.313375 Sphinx-7.0.0rc1/doc/development/tutorials/index.rst
+-rw-r--r--   0        0        0     8216 2023-04-23 19:57:27.313375 Sphinx-7.0.0rc1/doc/development/tutorials/recipe.rst
+-rw-r--r--   0        0        0    13435 2023-04-23 19:57:27.313375 Sphinx-7.0.0rc1/doc/development/tutorials/todo.rst
+-rw-r--r--   0        0        0       54 2023-04-23 19:57:27.313375 Sphinx-7.0.0rc1/doc/examples.rst
+-rw-r--r--   0        0        0    14235 2023-04-23 19:57:27.314375 Sphinx-7.0.0rc1/doc/extdev/appapi.rst
+-rw-r--r--   0        0        0     1103 2023-04-23 19:57:27.314375 Sphinx-7.0.0rc1/doc/extdev/builderapi.rst
+-rw-r--r--   0        0        0      165 2023-04-23 19:57:27.314375 Sphinx-7.0.0rc1/doc/extdev/collectorapi.rst
+-rw-r--r--   0        0        0    40815 2023-04-27 00:31:27.920451 Sphinx-7.0.0rc1/doc/extdev/deprecated.rst
+-rw-r--r--   0        0        0      518 2023-04-23 19:57:27.315375 Sphinx-7.0.0rc1/doc/extdev/domainapi.rst
+-rw-r--r--   0        0        0     1043 2023-04-23 19:57:27.315375 Sphinx-7.0.0rc1/doc/extdev/envapi.rst
+-rw-r--r--   0        0        0     2817 2023-04-23 19:57:27.315375 Sphinx-7.0.0rc1/doc/extdev/i18n.rst
+-rw-r--r--   0        0        0     8597 2023-04-23 19:57:27.315375 Sphinx-7.0.0rc1/doc/extdev/index.rst
+-rw-r--r--   0        0        0     2384 2023-04-23 19:57:27.316375 Sphinx-7.0.0rc1/doc/extdev/logging.rst
+-rw-r--r--   0        0        0     4787 2023-04-23 19:57:27.316375 Sphinx-7.0.0rc1/doc/extdev/markupapi.rst
+-rw-r--r--   0        0        0     1563 2023-04-23 19:57:27.316375 Sphinx-7.0.0rc1/doc/extdev/nodes.rst
+-rw-r--r--   0        0        0     1243 2023-04-23 19:57:27.316375 Sphinx-7.0.0rc1/doc/extdev/parserapi.rst
+-rw-r--r--   0        0        0      114 2023-04-23 19:57:27.316375 Sphinx-7.0.0rc1/doc/extdev/projectapi.rst
+-rw-r--r--   0        0        0      943 2023-04-23 19:57:27.316375 Sphinx-7.0.0rc1/doc/extdev/utils.rst
+-rw-r--r--   0        0        0    13329 2023-04-23 19:57:27.316375 Sphinx-7.0.0rc1/doc/faq.rst
+-rw-r--r--   0        0        0     4173 2023-04-23 19:57:27.317375 Sphinx-7.0.0rc1/doc/glossary.rst
+-rw-r--r--   0        0        0     3539 2023-04-23 19:57:27.317375 Sphinx-7.0.0rc1/doc/index.rst
+-rw-r--r--   0        0        0       71 2023-04-23 19:57:27.317375 Sphinx-7.0.0rc1/doc/internals/code-of-conduct.rst
+-rw-r--r--   0        0        0    11482 2023-04-23 19:57:27.317375 Sphinx-7.0.0rc1/doc/internals/contributing.rst
+-rw-r--r--   0        0        0      353 2023-04-23 19:57:27.317375 Sphinx-7.0.0rc1/doc/internals/index.rst
+-rw-r--r--   0        0        0     1964 2023-04-23 19:57:27.317375 Sphinx-7.0.0rc1/doc/internals/organization.rst
+-rw-r--r--   0        0        0     4395 2023-04-23 19:57:27.318375 Sphinx-7.0.0rc1/doc/internals/release-process.rst
+-rw-r--r--   0        0        0    68725 2023-04-23 19:57:27.318375 Sphinx-7.0.0rc1/doc/latex.rst
+-rwxr-xr-x   0        0        0      784 2023-04-25 10:59:46.881271 Sphinx-7.0.0rc1/doc/make.bat
+-rw-r--r--   0        0        0      314 2023-04-23 19:57:27.319375 Sphinx-7.0.0rc1/doc/man/index.rst
+-rw-r--r--   0        0        0     4508 2023-04-23 19:57:27.319375 Sphinx-7.0.0rc1/doc/man/sphinx-apidoc.rst
+-rw-r--r--   0        0        0     2122 2023-04-23 19:57:27.319375 Sphinx-7.0.0rc1/doc/man/sphinx-autogen.rst
+-rw-r--r--   0        0        0    10497 2023-04-23 19:57:27.319375 Sphinx-7.0.0rc1/doc/man/sphinx-build.rst
+-rw-r--r--   0        0        0     3692 2023-04-23 19:57:27.319375 Sphinx-7.0.0rc1/doc/man/sphinx-quickstart.rst
+-rw-r--r--   0        0        0      806 2023-04-23 19:57:27.319375 Sphinx-7.0.0rc1/doc/support.rst
+-rw-r--r--   0        0        0     4981 2023-04-23 19:57:27.320375 Sphinx-7.0.0rc1/doc/tutorial/automatic-doc-generation.rst
+-rw-r--r--   0        0        0    11036 2023-04-23 19:57:27.320375 Sphinx-7.0.0rc1/doc/tutorial/deploying.rst
+-rw-r--r--   0        0        0     9134 2023-04-23 19:57:27.320375 Sphinx-7.0.0rc1/doc/tutorial/describing-code.rst
+-rw-r--r--   0        0        0      240 2023-04-23 19:57:27.320375 Sphinx-7.0.0rc1/doc/tutorial/end.rst
+-rw-r--r--   0        0        0     3450 2023-04-23 19:57:27.320375 Sphinx-7.0.0rc1/doc/tutorial/first-steps.rst
+-rw-r--r--   0        0        0     3723 2023-04-23 19:57:27.321380 Sphinx-7.0.0rc1/doc/tutorial/getting-started.rst
+-rw-r--r--   0        0        0     1433 2023-04-23 19:57:27.321380 Sphinx-7.0.0rc1/doc/tutorial/index.rst
+-rw-r--r--   0        0        0     2528 2023-04-23 19:57:27.321380 Sphinx-7.0.0rc1/doc/tutorial/more-sphinx-customization.rst
+-rw-r--r--   0        0        0     4177 2023-04-23 19:57:27.321380 Sphinx-7.0.0rc1/doc/tutorial/narrative-documentation.rst
+-rw-r--r--   0        0        0    11259 2023-04-23 19:57:27.322375 Sphinx-7.0.0rc1/doc/usage/advanced/intl.rst
+-rw-r--r--   0        0        0     2670 2023-04-23 19:57:27.322375 Sphinx-7.0.0rc1/doc/usage/advanced/websupport/api.rst
+-rw-r--r--   0        0        0      302 2023-04-23 19:57:27.322375 Sphinx-7.0.0rc1/doc/usage/advanced/websupport/index.rst
+-rw-r--r--   0        0        0     9640 2023-04-23 19:57:27.323375 Sphinx-7.0.0rc1/doc/usage/advanced/websupport/quickstart.rst
+-rw-r--r--   0        0        0     1368 2023-04-23 19:57:27.323375 Sphinx-7.0.0rc1/doc/usage/advanced/websupport/searchadapters.rst
+-rw-r--r--   0        0        0     1231 2023-04-23 19:57:27.323375 Sphinx-7.0.0rc1/doc/usage/advanced/websupport/storagebackends.rst
+-rw-r--r--   0        0        0    17742 2023-04-23 19:57:27.323375 Sphinx-7.0.0rc1/doc/usage/builders/index.rst
+-rw-r--r--   0        0        0    99806 2023-04-23 19:57:27.324375 Sphinx-7.0.0rc1/doc/usage/configuration.rst
+-rw-r--r--   0        0        0    29861 2023-04-23 19:57:27.324375 Sphinx-7.0.0rc1/doc/usage/extensions/autodoc.rst
+-rw-r--r--   0        0        0     1899 2023-04-23 19:57:27.325374 Sphinx-7.0.0rc1/doc/usage/extensions/autosectionlabel.rst
+-rw-r--r--   0        0        0    11098 2023-04-23 19:57:27.325374 Sphinx-7.0.0rc1/doc/usage/extensions/autosummary.rst
+-rw-r--r--   0        0        0     1584 2023-04-23 19:57:27.325374 Sphinx-7.0.0rc1/doc/usage/extensions/coverage.rst
+-rw-r--r--   0        0        0    11838 2023-04-23 19:57:27.325374 Sphinx-7.0.0rc1/doc/usage/extensions/doctest.rst
+-rw-r--r--   0        0        0      404 2023-04-23 19:57:27.325374 Sphinx-7.0.0rc1/doc/usage/extensions/duration.rst
+-rw-r--r--   0        0        0     9665 2023-04-23 19:57:27.326376 Sphinx-7.0.0rc1/doc/usage/extensions/example_google.py
+-rw-r--r--   0        0        0      296 2023-04-23 19:57:27.326376 Sphinx-7.0.0rc1/doc/usage/extensions/example_google.rst
+-rw-r--r--   0        0        0     9714 2023-04-23 19:57:27.326376 Sphinx-7.0.0rc1/doc/usage/extensions/example_numpy.py
+-rw-r--r--   0        0        0      292 2023-04-23 19:57:27.326376 Sphinx-7.0.0rc1/doc/usage/extensions/example_numpy.rst
+-rw-r--r--   0        0        0     2781 2023-04-23 19:57:27.326376 Sphinx-7.0.0rc1/doc/usage/extensions/extlinks.rst
+-rw-r--r--   0        0        0      491 2023-04-23 19:57:27.326376 Sphinx-7.0.0rc1/doc/usage/extensions/githubpages.rst
+-rw-r--r--   0        0        0     6292 2023-04-23 19:57:27.327375 Sphinx-7.0.0rc1/doc/usage/extensions/graphviz.rst
+-rw-r--r--   0        0        0     1329 2023-04-23 19:57:27.327375 Sphinx-7.0.0rc1/doc/usage/extensions/ifconfig.rst
+-rw-r--r--   0        0        0     1705 2023-04-23 19:57:27.327375 Sphinx-7.0.0rc1/doc/usage/extensions/imgconverter.rst
+-rw-r--r--   0        0        0     2410 2023-04-23 19:57:27.327375 Sphinx-7.0.0rc1/doc/usage/extensions/index.rst
+-rw-r--r--   0        0        0     5594 2023-04-23 19:57:27.327375 Sphinx-7.0.0rc1/doc/usage/extensions/inheritance.rst
+-rw-r--r--   0        0        0     9934 2023-04-23 19:57:27.328374 Sphinx-7.0.0rc1/doc/usage/extensions/intersphinx.rst
+-rw-r--r--   0        0        0     1756 2023-04-23 19:57:27.328374 Sphinx-7.0.0rc1/doc/usage/extensions/linkcode.rst
+-rw-r--r--   0        0        0    11756 2023-04-23 19:57:27.328374 Sphinx-7.0.0rc1/doc/usage/extensions/math.rst
+-rw-r--r--   0        0        0    15980 2023-04-23 19:57:27.328374 Sphinx-7.0.0rc1/doc/usage/extensions/napoleon.rst
+-rw-r--r--   0        0        0     1644 2023-04-23 19:57:27.328374 Sphinx-7.0.0rc1/doc/usage/extensions/todo.rst
+-rw-r--r--   0        0        0     3748 2023-04-23 19:57:27.328374 Sphinx-7.0.0rc1/doc/usage/extensions/viewcode.rst
+-rw-r--r--   0        0        0      537 2023-04-27 00:31:27.920451 Sphinx-7.0.0rc1/doc/usage/index.rst
+-rw-r--r--   0        0        0     7146 2023-04-23 19:57:27.329374 Sphinx-7.0.0rc1/doc/usage/installation.rst
+-rw-r--r--   0        0        0     1584 2023-04-23 19:57:27.329374 Sphinx-7.0.0rc1/doc/usage/markdown.rst
+-rw-r--r--   0        0        0    13150 2023-04-27 00:31:27.920451 Sphinx-7.0.0rc1/doc/usage/quickstart.rst
+-rw-r--r--   0        0        0    20508 2023-04-23 19:57:27.330375 Sphinx-7.0.0rc1/doc/usage/restructuredtext/basics.rst
+-rw-r--r--   0        0        0    45004 2023-04-23 19:57:27.330375 Sphinx-7.0.0rc1/doc/usage/restructuredtext/directives.rst
+-rw-r--r--   0        0        0    62364 2023-04-23 19:57:27.330375 Sphinx-7.0.0rc1/doc/usage/restructuredtext/domains.rst
+-rw-r--r--   0        0        0     1967 2023-04-23 19:57:27.331375 Sphinx-7.0.0rc1/doc/usage/restructuredtext/field-lists.rst
+-rw-r--r--   0        0        0      574 2023-04-23 19:57:27.331375 Sphinx-7.0.0rc1/doc/usage/restructuredtext/index.rst
+-rw-r--r--   0        0        0    18187 2023-04-23 19:57:27.331375 Sphinx-7.0.0rc1/doc/usage/restructuredtext/roles.rst
+-rw-r--r--   0        0        0    14326 2023-04-23 19:57:27.331375 Sphinx-7.0.0rc1/doc/usage/theming.rst
+-rw-r--r--   0        0        0    12593 2023-04-27 00:31:27.920451 Sphinx-7.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1829 2023-04-28 11:31:28.415866 Sphinx-7.0.0rc1/sphinx/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-23 19:57:27.333374 Sphinx-7.0.0rc1/sphinx/__main__.py
+-rw-r--r--   0        0        0    17579 2023-04-23 19:57:27.334375 Sphinx-7.0.0rc1/sphinx/addnodes.py
+-rw-r--r--   0        0        0    55683 2023-04-28 09:26:30.898486 Sphinx-7.0.0rc1/sphinx/application.py
+-rw-r--r--   0        0        0    26838 2023-04-28 09:26:30.898486 Sphinx-7.0.0rc1/sphinx/builders/__init__.py
+-rw-r--r--   0        0        0    28999 2023-04-23 19:57:27.335380 Sphinx-7.0.0rc1/sphinx/builders/_epub_base.py
+-rw-r--r--   0        0        0     6474 2023-04-23 19:57:27.335380 Sphinx-7.0.0rc1/sphinx/builders/changes.py
+-rw-r--r--   0        0        0     1504 2023-04-23 19:57:27.335380 Sphinx-7.0.0rc1/sphinx/builders/dirhtml.py
+-rw-r--r--   0        0        0      982 2023-04-23 19:57:27.335380 Sphinx-7.0.0rc1/sphinx/builders/dummy.py
+-rw-r--r--   0        0        0    11284 2023-04-23 19:57:27.336375 Sphinx-7.0.0rc1/sphinx/builders/epub3.py
+-rw-r--r--   0        0        0    11407 2023-04-23 19:57:27.336375 Sphinx-7.0.0rc1/sphinx/builders/gettext.py
+-rw-r--r--   0        0        0    58281 2023-04-28 10:59:56.013366 Sphinx-7.0.0rc1/sphinx/builders/html/__init__.py
+-rw-r--r--   0        0        0     2525 2023-04-23 19:57:27.337375 Sphinx-7.0.0rc1/sphinx/builders/html/transforms.py
+-rw-r--r--   0        0        0    24143 2023-04-23 19:57:27.338035 Sphinx-7.0.0rc1/sphinx/builders/latex/__init__.py
+-rw-r--r--   0        0        0     7365 2023-04-23 19:57:27.338035 Sphinx-7.0.0rc1/sphinx/builders/latex/constants.py
+-rw-r--r--   0        0        0      866 2023-04-23 19:57:27.338035 Sphinx-7.0.0rc1/sphinx/builders/latex/nodes.py
+-rw-r--r--   0        0        0     4445 2023-04-23 19:57:27.338035 Sphinx-7.0.0rc1/sphinx/builders/latex/theming.py
+-rw-r--r--   0        0        0    20998 2023-04-23 19:57:27.338961 Sphinx-7.0.0rc1/sphinx/builders/latex/transforms.py
+-rw-r--r--   0        0        0     1703 2023-04-23 19:57:27.338961 Sphinx-7.0.0rc1/sphinx/builders/latex/util.py
+-rw-r--r--   0        0        0    23404 2023-04-23 19:57:27.338961 Sphinx-7.0.0rc1/sphinx/builders/linkcheck.py
+-rw-r--r--   0        0        0     4511 2023-04-23 19:57:27.338961 Sphinx-7.0.0rc1/sphinx/builders/manpage.py
+-rw-r--r--   0        0        0     7425 2023-04-23 19:57:27.338961 Sphinx-7.0.0rc1/sphinx/builders/singlehtml.py
+-rw-r--r--   0        0        0     9634 2023-04-23 19:57:27.339975 Sphinx-7.0.0rc1/sphinx/builders/texinfo.py
+-rw-r--r--   0        0        0     2870 2023-04-23 19:57:27.339975 Sphinx-7.0.0rc1/sphinx/builders/text.py
+-rw-r--r--   0        0        0     3726 2023-04-23 19:57:27.339975 Sphinx-7.0.0rc1/sphinx/builders/xml.py
+-rw-r--r--   0        0        0       44 2023-04-23 19:57:27.339975 Sphinx-7.0.0rc1/sphinx/cmd/__init__.py
+-rw-r--r--   0        0        0    13411 2023-04-23 19:57:27.339975 Sphinx-7.0.0rc1/sphinx/cmd/build.py
+-rw-r--r--   0        0        0     6552 2023-04-23 19:57:27.340974 Sphinx-7.0.0rc1/sphinx/cmd/make_mode.py
+-rw-r--r--   0        0        0    23835 2023-04-23 19:57:27.340974 Sphinx-7.0.0rc1/sphinx/cmd/quickstart.py
+-rw-r--r--   0        0        0    21519 2023-04-26 16:05:03.832456 Sphinx-7.0.0rc1/sphinx/config.py
+-rw-r--r--   0        0        0     1816 2023-04-28 11:10:33.021919 Sphinx-7.0.0rc1/sphinx/deprecation.py
+-rw-r--r--   0        0        0    13518 2023-04-23 19:57:27.341975 Sphinx-7.0.0rc1/sphinx/directives/__init__.py
+-rw-r--r--   0        0        0    18354 2023-04-23 19:57:27.341975 Sphinx-7.0.0rc1/sphinx/directives/code.py
+-rw-r--r--   0        0        0    14672 2023-04-23 19:57:27.341975 Sphinx-7.0.0rc1/sphinx/directives/other.py
+-rw-r--r--   0        0        0     6781 2023-04-23 19:57:27.342974 Sphinx-7.0.0rc1/sphinx/directives/patches.py
+-rw-r--r--   0        0        0    15320 2023-04-23 19:57:27.342974 Sphinx-7.0.0rc1/sphinx/domains/__init__.py
+-rw-r--r--   0        0        0   150745 2023-04-27 00:29:16.230978 Sphinx-7.0.0rc1/sphinx/domains/c.py
+-rw-r--r--   0        0        0     5524 2023-04-23 19:57:27.343975 Sphinx-7.0.0rc1/sphinx/domains/changeset.py
+-rw-r--r--   0        0        0     5676 2023-04-23 19:57:27.343975 Sphinx-7.0.0rc1/sphinx/domains/citation.py
+-rw-r--r--   0        0        0   329631 2023-04-23 19:57:27.344974 Sphinx-7.0.0rc1/sphinx/domains/cpp.py
+-rw-r--r--   0        0        0     4086 2023-04-23 19:57:27.344974 Sphinx-7.0.0rc1/sphinx/domains/index.py
+-rw-r--r--   0        0        0    18294 2023-04-27 00:29:16.230978 Sphinx-7.0.0rc1/sphinx/domains/javascript.py
+-rw-r--r--   0        0        0     5459 2023-04-23 19:57:27.345974 Sphinx-7.0.0rc1/sphinx/domains/math.py
+-rw-r--r--   0        0        0    59777 2023-04-27 00:29:16.230978 Sphinx-7.0.0rc1/sphinx/domains/python.py
+-rw-r--r--   0        0        0    10292 2023-04-27 00:29:16.230978 Sphinx-7.0.0rc1/sphinx/domains/rst.py
+-rw-r--r--   0        0        0    45842 2023-04-27 00:29:16.230978 Sphinx-7.0.0rc1/sphinx/domains/std.py
+-rw-r--r--   0        0        0    29692 2023-04-23 19:57:27.347974 Sphinx-7.0.0rc1/sphinx/environment/__init__.py
+-rw-r--r--   0        0        0       34 2023-04-23 19:57:27.347974 Sphinx-7.0.0rc1/sphinx/environment/adapters/__init__.py
+-rw-r--r--   0        0        0      418 2023-04-23 19:57:27.347974 Sphinx-7.0.0rc1/sphinx/environment/adapters/asset.py
+-rw-r--r--   0        0        0     7509 2023-04-23 19:57:27.347974 Sphinx-7.0.0rc1/sphinx/environment/adapters/indexentries.py
+-rw-r--r--   0        0        0    16449 2023-04-23 19:57:27.348974 Sphinx-7.0.0rc1/sphinx/environment/adapters/toctree.py
+-rw-r--r--   0        0        0     2784 2023-04-23 19:57:27.348974 Sphinx-7.0.0rc1/sphinx/environment/collectors/__init__.py
+-rw-r--r--   0        0        0     6161 2023-04-23 19:57:27.348974 Sphinx-7.0.0rc1/sphinx/environment/collectors/asset.py
+-rw-r--r--   0        0        0     1887 2023-04-23 19:57:27.348974 Sphinx-7.0.0rc1/sphinx/environment/collectors/dependencies.py
+-rw-r--r--   0        0        0     2609 2023-04-23 19:57:27.349974 Sphinx-7.0.0rc1/sphinx/environment/collectors/metadata.py
+-rw-r--r--   0        0        0     2144 2023-04-23 19:57:27.349974 Sphinx-7.0.0rc1/sphinx/environment/collectors/title.py
+-rw-r--r--   0        0        0    15869 2023-04-23 19:57:27.349974 Sphinx-7.0.0rc1/sphinx/environment/collectors/toctree.py
+-rw-r--r--   0        0        0     3388 2023-04-23 19:57:27.349974 Sphinx-7.0.0rc1/sphinx/errors.py
+-rw-r--r--   0        0        0     4230 2023-04-23 19:57:27.349974 Sphinx-7.0.0rc1/sphinx/events.py
+-rw-r--r--   0        0        0       57 2023-04-23 19:57:27.349974 Sphinx-7.0.0rc1/sphinx/ext/__init__.py
+-rw-r--r--   0        0        0    19197 2023-04-23 19:57:27.350974 Sphinx-7.0.0rc1/sphinx/ext/apidoc.py
+-rw-r--r--   0        0        0   114236 2023-04-23 19:57:27.350974 Sphinx-7.0.0rc1/sphinx/ext/autodoc/__init__.py
+-rw-r--r--   0        0        0     5925 2023-04-23 19:57:27.351975 Sphinx-7.0.0rc1/sphinx/ext/autodoc/directive.py
+-rw-r--r--   0        0        0    11371 2023-04-23 19:57:27.351975 Sphinx-7.0.0rc1/sphinx/ext/autodoc/importer.py
+-rw-r--r--   0        0        0     5900 2023-04-23 19:57:27.351975 Sphinx-7.0.0rc1/sphinx/ext/autodoc/mock.py
+-rw-r--r--   0        0        0     4588 2023-04-23 19:57:27.351975 Sphinx-7.0.0rc1/sphinx/ext/autodoc/preserve_defaults.py
+-rw-r--r--   0        0        0     5292 2023-04-23 19:57:27.351975 Sphinx-7.0.0rc1/sphinx/ext/autodoc/type_comment.py
+-rw-r--r--   0        0        0     7789 2023-04-23 19:57:27.352974 Sphinx-7.0.0rc1/sphinx/ext/autodoc/typehints.py
+-rw-r--r--   0        0        0     2292 2023-04-23 19:57:27.352974 Sphinx-7.0.0rc1/sphinx/ext/autosectionlabel.py
+-rw-r--r--   0        0        0    31056 2023-04-28 09:21:04.216236 Sphinx-7.0.0rc1/sphinx/ext/autosummary/__init__.py
+-rw-r--r--   0        0        0    26212 2023-04-23 19:57:27.353975 Sphinx-7.0.0rc1/sphinx/ext/autosummary/generate.py
+-rw-r--r--   0        0        0      106 2023-04-23 19:57:27.353975 Sphinx-7.0.0rc1/sphinx/ext/autosummary/templates/autosummary/base.rst
+-rw-r--r--   0        0        0      553 2023-04-23 19:57:27.353975 Sphinx-7.0.0rc1/sphinx/ext/autosummary/templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1071 2023-04-23 19:57:27.353975 Sphinx-7.0.0rc1/sphinx/ext/autosummary/templates/autosummary/module.rst
+-rw-r--r--   0        0        0    14065 2023-04-23 19:57:27.354974 Sphinx-7.0.0rc1/sphinx/ext/coverage.py
+-rw-r--r--   0        0        0    22423 2023-04-23 19:57:27.354974 Sphinx-7.0.0rc1/sphinx/ext/doctest.py
+-rw-r--r--   0        0        0     2887 2023-04-23 19:57:27.354974 Sphinx-7.0.0rc1/sphinx/ext/duration.py
+-rw-r--r--   0        0        0     4523 2023-04-23 19:57:27.354974 Sphinx-7.0.0rc1/sphinx/ext/extlinks.py
+-rw-r--r--   0        0        0     1962 2023-04-23 19:57:27.355975 Sphinx-7.0.0rc1/sphinx/ext/githubpages.py
+-rw-r--r--   0        0        0    15864 2023-04-23 19:57:27.355975 Sphinx-7.0.0rc1/sphinx/ext/graphviz.py
+-rw-r--r--   0        0        0     2517 2023-04-23 19:57:27.355975 Sphinx-7.0.0rc1/sphinx/ext/ifconfig.py
+-rw-r--r--   0        0        0     3582 2023-04-23 19:57:27.355975 Sphinx-7.0.0rc1/sphinx/ext/imgconverter.py
+-rw-r--r--   0        0        0    15117 2023-04-23 19:57:27.355975 Sphinx-7.0.0rc1/sphinx/ext/imgmath.py
+-rw-r--r--   0        0        0    17031 2023-04-23 19:57:27.356974 Sphinx-7.0.0rc1/sphinx/ext/inheritance_diagram.py
+-rw-r--r--   0        0        0    28440 2023-04-27 00:29:16.230978 Sphinx-7.0.0rc1/sphinx/ext/intersphinx.py
+-rw-r--r--   0        0        0     2203 2023-04-23 19:57:27.356974 Sphinx-7.0.0rc1/sphinx/ext/linkcode.py
+-rw-r--r--   0        0        0     5182 2023-04-23 19:57:27.356974 Sphinx-7.0.0rc1/sphinx/ext/mathjax.py
+-rw-r--r--   0        0        0    17936 2023-04-23 19:57:27.357974 Sphinx-7.0.0rc1/sphinx/ext/napoleon/__init__.py
+-rw-r--r--   0        0        0    48417 2023-04-23 19:57:27.357974 Sphinx-7.0.0rc1/sphinx/ext/napoleon/docstring.py
+-rw-r--r--   0        0        0     8017 2023-04-23 19:57:27.357974 Sphinx-7.0.0rc1/sphinx/ext/todo.py
+-rw-r--r--   0        0        0    12900 2023-04-23 19:57:27.358974 Sphinx-7.0.0rc1/sphinx/ext/viewcode.py
+-rw-r--r--   0        0        0     2995 2023-04-23 19:57:27.358974 Sphinx-7.0.0rc1/sphinx/extension.py
+-rw-r--r--   0        0        0     6986 2023-04-23 19:57:27.358974 Sphinx-7.0.0rc1/sphinx/highlighting.py
+-rw-r--r--   0        0        0     6190 2023-04-27 15:02:05.988638 Sphinx-7.0.0rc1/sphinx/io.py
+-rw-r--r--   0        0        0     7107 2023-04-23 19:57:27.358974 Sphinx-7.0.0rc1/sphinx/jinja2glue.py
+-rw-r--r--   0        0        0      165 2023-04-25 10:59:46.881271 Sphinx-7.0.0rc1/sphinx/locale/.tx/config
+-rw-r--r--   0        0        0     7316 2023-04-23 19:57:27.359974 Sphinx-7.0.0rc1/sphinx/locale/__init__.py
+-rw-r--r--   0        0        0     3735 2023-04-23 19:57:27.359974 Sphinx-7.0.0rc1/sphinx/locale/ar/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     7947 2023-04-23 19:57:27.360974 Sphinx-7.0.0rc1/sphinx/locale/ar/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    87617 2023-04-23 19:57:27.361975 Sphinx-7.0.0rc1/sphinx/locale/ar/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2361 2023-04-23 19:57:27.362172 Sphinx-7.0.0rc1/sphinx/locale/bg/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      492 2023-04-23 19:57:27.362172 Sphinx-7.0.0rc1/sphinx/locale/bg/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84994 2023-04-23 19:57:27.362172 Sphinx-7.0.0rc1/sphinx/locale/bg/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     6038 2023-04-23 19:57:27.363207 Sphinx-7.0.0rc1/sphinx/locale/bn/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     7976 2023-04-23 19:57:27.363207 Sphinx-7.0.0rc1/sphinx/locale/bn/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    89077 2023-04-23 19:57:27.364207 Sphinx-7.0.0rc1/sphinx/locale/bn/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3259 2023-04-23 19:57:27.364207 Sphinx-7.0.0rc1/sphinx/locale/ca/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     5587 2023-04-23 19:57:27.364207 Sphinx-7.0.0rc1/sphinx/locale/ca/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86709 2023-04-23 19:57:27.364207 Sphinx-7.0.0rc1/sphinx/locale/ca/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2446 2023-04-23 19:57:27.365207 Sphinx-7.0.0rc1/sphinx/locale/cak/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     2424 2023-04-23 19:57:27.365207 Sphinx-7.0.0rc1/sphinx/locale/cak/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85717 2023-04-23 19:57:27.365207 Sphinx-7.0.0rc1/sphinx/locale/cak/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4037 2023-04-23 19:57:27.366207 Sphinx-7.0.0rc1/sphinx/locale/cs/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     8265 2023-04-23 19:57:27.366207 Sphinx-7.0.0rc1/sphinx/locale/cs/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    87804 2023-04-23 19:57:27.366207 Sphinx-7.0.0rc1/sphinx/locale/cs/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3472 2023-04-23 19:57:27.366207 Sphinx-7.0.0rc1/sphinx/locale/cy/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6214 2023-04-23 19:57:27.367207 Sphinx-7.0.0rc1/sphinx/locale/cy/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    87070 2023-04-23 19:57:27.367425 Sphinx-7.0.0rc1/sphinx/locale/cy/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3726 2023-04-23 19:57:27.367425 Sphinx-7.0.0rc1/sphinx/locale/da/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    13099 2023-04-23 19:57:27.367425 Sphinx-7.0.0rc1/sphinx/locale/da/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    89619 2023-04-23 19:57:27.367425 Sphinx-7.0.0rc1/sphinx/locale/da/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3594 2023-04-23 19:57:27.368431 Sphinx-7.0.0rc1/sphinx/locale/de/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    11216 2023-04-23 19:57:27.368431 Sphinx-7.0.0rc1/sphinx/locale/de/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    89151 2023-04-23 19:57:27.368431 Sphinx-7.0.0rc1/sphinx/locale/de/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     8904 2023-04-23 19:57:27.369431 Sphinx-7.0.0rc1/sphinx/locale/el/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    81979 2023-04-23 19:57:27.369431 Sphinx-7.0.0rc1/sphinx/locale/el/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   133241 2023-04-23 19:57:27.370445 Sphinx-7.0.0rc1/sphinx/locale/el/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2363 2023-04-23 19:57:27.370445 Sphinx-7.0.0rc1/sphinx/locale/en_FR/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      462 2023-04-23 19:57:27.370445 Sphinx-7.0.0rc1/sphinx/locale/en_FR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84193 2023-04-23 19:57:27.371431 Sphinx-7.0.0rc1/sphinx/locale/en_FR/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2364 2023-04-23 19:57:27.371431 Sphinx-7.0.0rc1/sphinx/locale/en_GB/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    13825 2023-04-23 19:57:27.371431 Sphinx-7.0.0rc1/sphinx/locale/en_GB/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    89843 2023-04-23 19:57:27.373431 Sphinx-7.0.0rc1/sphinx/locale/en_GB/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2364 2023-04-23 19:57:27.373431 Sphinx-7.0.0rc1/sphinx/locale/en_HK/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      508 2023-04-23 19:57:27.374431 Sphinx-7.0.0rc1/sphinx/locale/en_HK/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84196 2023-04-23 19:57:27.374431 Sphinx-7.0.0rc1/sphinx/locale/en_HK/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2518 2023-04-23 19:57:27.374431 Sphinx-7.0.0rc1/sphinx/locale/eo/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     1864 2023-04-23 19:57:27.374431 Sphinx-7.0.0rc1/sphinx/locale/eo/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84676 2023-04-23 19:57:27.374431 Sphinx-7.0.0rc1/sphinx/locale/eo/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4319 2023-04-23 19:57:27.375430 Sphinx-7.0.0rc1/sphinx/locale/es/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    82560 2023-04-23 19:57:27.375430 Sphinx-7.0.0rc1/sphinx/locale/es/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   122518 2023-04-23 19:57:27.376438 Sphinx-7.0.0rc1/sphinx/locale/es/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3781 2023-04-23 19:57:27.376438 Sphinx-7.0.0rc1/sphinx/locale/et/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    33706 2023-04-23 19:57:27.377431 Sphinx-7.0.0rc1/sphinx/locale/et/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    97950 2023-04-23 19:57:27.377431 Sphinx-7.0.0rc1/sphinx/locale/et/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3163 2023-04-23 19:57:27.377431 Sphinx-7.0.0rc1/sphinx/locale/eu/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6727 2023-04-23 19:57:27.378430 Sphinx-7.0.0rc1/sphinx/locale/eu/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86399 2023-04-23 19:57:27.378510 Sphinx-7.0.0rc1/sphinx/locale/eu/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     7742 2023-04-23 19:57:27.378510 Sphinx-7.0.0rc1/sphinx/locale/fa/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    98774 2023-04-23 19:57:27.379515 Sphinx-7.0.0rc1/sphinx/locale/fa/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   140105 2023-04-23 19:57:27.379515 Sphinx-7.0.0rc1/sphinx/locale/fa/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2848 2023-04-23 19:57:27.380514 Sphinx-7.0.0rc1/sphinx/locale/fi/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     2912 2023-04-23 19:57:27.380514 Sphinx-7.0.0rc1/sphinx/locale/fi/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84980 2023-04-23 19:57:27.380514 Sphinx-7.0.0rc1/sphinx/locale/fi/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4309 2023-04-23 19:57:27.381514 Sphinx-7.0.0rc1/sphinx/locale/fr/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    85079 2023-04-23 19:57:27.381514 Sphinx-7.0.0rc1/sphinx/locale/fr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   125547 2023-04-23 19:57:27.381514 Sphinx-7.0.0rc1/sphinx/locale/fr/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2415 2023-04-23 19:57:27.381514 Sphinx-7.0.0rc1/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      555 2023-04-23 19:57:27.381514 Sphinx-7.0.0rc1/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84243 2023-04-23 19:57:27.382515 Sphinx-7.0.0rc1/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4946 2023-04-23 19:57:27.382515 Sphinx-7.0.0rc1/sphinx/locale/he/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     4947 2023-04-23 19:57:27.382515 Sphinx-7.0.0rc1/sphinx/locale/he/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86015 2023-04-23 19:57:27.382515 Sphinx-7.0.0rc1/sphinx/locale/he/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     7677 2023-04-23 19:57:27.383515 Sphinx-7.0.0rc1/sphinx/locale/hi/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    98543 2023-04-23 19:57:27.383515 Sphinx-7.0.0rc1/sphinx/locale/hi/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   147260 2023-04-23 19:57:27.384515 Sphinx-7.0.0rc1/sphinx/locale/hi/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2364 2023-04-23 19:57:27.384515 Sphinx-7.0.0rc1/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      502 2023-04-23 19:57:27.384515 Sphinx-7.0.0rc1/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84190 2023-04-23 19:57:27.385517 Sphinx-7.0.0rc1/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3797 2023-04-23 19:57:27.385517 Sphinx-7.0.0rc1/sphinx/locale/hr/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    17189 2023-04-23 19:57:27.385517 Sphinx-7.0.0rc1/sphinx/locale/hr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    90656 2023-04-23 19:57:27.386515 Sphinx-7.0.0rc1/sphinx/locale/hr/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4041 2023-04-23 19:57:27.386515 Sphinx-7.0.0rc1/sphinx/locale/hu/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    11533 2023-04-23 19:57:27.386515 Sphinx-7.0.0rc1/sphinx/locale/hu/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88685 2023-04-23 19:57:27.386515 Sphinx-7.0.0rc1/sphinx/locale/hu/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3613 2023-04-23 19:57:27.387514 Sphinx-7.0.0rc1/sphinx/locale/id/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    60590 2023-04-23 19:57:27.387514 Sphinx-7.0.0rc1/sphinx/locale/id/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   109933 2023-04-23 19:57:27.387514 Sphinx-7.0.0rc1/sphinx/locale/id/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2886 2023-04-23 19:57:27.388515 Sphinx-7.0.0rc1/sphinx/locale/is/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     3082 2023-04-23 19:57:27.388515 Sphinx-7.0.0rc1/sphinx/locale/is/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85100 2023-04-23 19:57:27.388515 Sphinx-7.0.0rc1/sphinx/locale/is/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3727 2023-04-23 19:57:27.388515 Sphinx-7.0.0rc1/sphinx/locale/it/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    10819 2023-04-23 19:57:27.389514 Sphinx-7.0.0rc1/sphinx/locale/it/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88216 2023-04-23 19:57:27.389514 Sphinx-7.0.0rc1/sphinx/locale/it/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     5105 2023-04-23 19:57:27.389514 Sphinx-7.0.0rc1/sphinx/locale/ja/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    87432 2023-04-23 19:57:27.390514 Sphinx-7.0.0rc1/sphinx/locale/ja/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   129215 2023-04-23 19:57:27.390514 Sphinx-7.0.0rc1/sphinx/locale/ja/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4973 2023-04-23 19:57:27.391515 Sphinx-7.0.0rc1/sphinx/locale/ko/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    83942 2023-04-23 19:57:27.391515 Sphinx-7.0.0rc1/sphinx/locale/ko/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   123556 2023-04-23 19:57:27.392514 Sphinx-7.0.0rc1/sphinx/locale/ko/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3534 2023-04-23 19:57:27.392514 Sphinx-7.0.0rc1/sphinx/locale/lt/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     7104 2023-04-23 19:57:27.392514 Sphinx-7.0.0rc1/sphinx/locale/lt/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86600 2023-04-23 19:57:27.392514 Sphinx-7.0.0rc1/sphinx/locale/lt/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3506 2023-04-23 19:57:27.393514 Sphinx-7.0.0rc1/sphinx/locale/lv/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6786 2023-04-23 19:57:27.393514 Sphinx-7.0.0rc1/sphinx/locale/lv/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86319 2023-04-23 19:57:27.393514 Sphinx-7.0.0rc1/sphinx/locale/lv/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2476 2023-04-23 19:57:27.393514 Sphinx-7.0.0rc1/sphinx/locale/mk/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     2011 2023-04-23 19:57:27.394514 Sphinx-7.0.0rc1/sphinx/locale/mk/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84870 2023-04-23 19:57:27.394514 Sphinx-7.0.0rc1/sphinx/locale/mk/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3169 2023-04-23 19:57:27.394514 Sphinx-7.0.0rc1/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6766 2023-04-23 19:57:27.394514 Sphinx-7.0.0rc1/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86123 2023-04-23 19:57:27.394514 Sphinx-7.0.0rc1/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     6284 2023-04-23 19:57:27.395514 Sphinx-7.0.0rc1/sphinx/locale/ne/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     8869 2023-04-23 19:57:27.395514 Sphinx-7.0.0rc1/sphinx/locale/ne/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88391 2023-04-23 19:57:27.395514 Sphinx-7.0.0rc1/sphinx/locale/ne/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3637 2023-04-23 19:57:27.396514 Sphinx-7.0.0rc1/sphinx/locale/nl/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    19426 2023-04-23 19:57:27.396514 Sphinx-7.0.0rc1/sphinx/locale/nl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    91992 2023-04-23 19:57:27.396514 Sphinx-7.0.0rc1/sphinx/locale/nl/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3967 2023-04-23 19:57:27.397514 Sphinx-7.0.0rc1/sphinx/locale/pl/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    29754 2023-04-23 19:57:27.397514 Sphinx-7.0.0rc1/sphinx/locale/pl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    96611 2023-04-23 19:57:27.397514 Sphinx-7.0.0rc1/sphinx/locale/pl/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2412 2023-04-23 19:57:27.397514 Sphinx-7.0.0rc1/sphinx/locale/pt/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      544 2023-04-23 19:57:27.397514 Sphinx-7.0.0rc1/sphinx/locale/pt/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84232 2023-04-23 19:57:27.398514 Sphinx-7.0.0rc1/sphinx/locale/pt/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4325 2023-04-23 19:57:27.398514 Sphinx-7.0.0rc1/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    80235 2023-04-23 19:57:27.399515 Sphinx-7.0.0rc1/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   120545 2023-04-23 19:57:27.400031 Sphinx-7.0.0rc1/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3806 2023-04-23 19:57:27.400031 Sphinx-7.0.0rc1/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     8035 2023-04-23 19:57:27.400031 Sphinx-7.0.0rc1/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86961 2023-04-23 19:57:27.401036 Sphinx-7.0.0rc1/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3761 2023-04-23 19:57:27.401036 Sphinx-7.0.0rc1/sphinx/locale/ro/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     8822 2023-04-23 19:57:27.401036 Sphinx-7.0.0rc1/sphinx/locale/ro/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    87272 2023-04-23 19:57:27.401036 Sphinx-7.0.0rc1/sphinx/locale/ro/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     8313 2023-04-23 19:57:27.402036 Sphinx-7.0.0rc1/sphinx/locale/ru/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    16339 2023-04-23 19:57:27.402036 Sphinx-7.0.0rc1/sphinx/locale/ru/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    92408 2023-04-23 19:57:27.402036 Sphinx-7.0.0rc1/sphinx/locale/ru/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3877 2023-04-23 19:57:27.403036 Sphinx-7.0.0rc1/sphinx/locale/si/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     3602 2023-04-23 19:57:27.403036 Sphinx-7.0.0rc1/sphinx/locale/si/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85680 2023-04-23 19:57:27.403036 Sphinx-7.0.0rc1/sphinx/locale/si/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4265 2023-04-23 19:57:27.404037 Sphinx-7.0.0rc1/sphinx/locale/sk/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    67619 2023-04-23 19:57:27.404037 Sphinx-7.0.0rc1/sphinx/locale/sk/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   113547 2023-04-23 19:57:27.404037 Sphinx-7.0.0rc1/sphinx/locale/sk/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3246 2023-04-23 19:57:27.405036 Sphinx-7.0.0rc1/sphinx/locale/sl/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     5417 2023-04-23 19:57:27.405036 Sphinx-7.0.0rc1/sphinx/locale/sl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85800 2023-04-23 19:57:27.405036 Sphinx-7.0.0rc1/sphinx/locale/sl/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0    84162 2023-04-23 19:57:27.405036 Sphinx-7.0.0rc1/sphinx/locale/sphinx.pot
+-rw-r--r--   0        0        0     4390 2023-04-23 19:57:27.406036 Sphinx-7.0.0rc1/sphinx/locale/sq/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    78940 2023-04-23 19:57:27.406036 Sphinx-7.0.0rc1/sphinx/locale/sq/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   120398 2023-04-23 19:57:27.407039 Sphinx-7.0.0rc1/sphinx/locale/sq/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2441 2023-04-23 19:57:27.408036 Sphinx-7.0.0rc1/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      584 2023-04-23 19:57:27.408036 Sphinx-7.0.0rc1/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84272 2023-04-23 19:57:27.408036 Sphinx-7.0.0rc1/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4161 2023-04-23 19:57:27.407039 Sphinx-7.0.0rc1/sphinx/locale/sr/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     9426 2023-04-23 19:57:27.407039 Sphinx-7.0.0rc1/sphinx/locale/sr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88404 2023-04-23 19:57:27.408036 Sphinx-7.0.0rc1/sphinx/locale/sr/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2443 2023-04-23 19:57:27.408036 Sphinx-7.0.0rc1/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      579 2023-04-23 19:57:27.409036 Sphinx-7.0.0rc1/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84267 2023-04-23 19:57:27.409036 Sphinx-7.0.0rc1/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3342 2023-04-23 19:57:27.409036 Sphinx-7.0.0rc1/sphinx/locale/sv/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6754 2023-04-23 19:57:27.409036 Sphinx-7.0.0rc1/sphinx/locale/sv/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86142 2023-04-23 19:57:27.410038 Sphinx-7.0.0rc1/sphinx/locale/sv/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2361 2023-04-23 19:57:27.410038 Sphinx-7.0.0rc1/sphinx/locale/ta/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      647 2023-04-23 19:57:27.410038 Sphinx-7.0.0rc1/sphinx/locale/ta/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84340 2023-04-23 19:57:27.410038 Sphinx-7.0.0rc1/sphinx/locale/ta/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2361 2023-04-23 19:57:27.411036 Sphinx-7.0.0rc1/sphinx/locale/te/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      489 2023-04-23 19:57:27.411036 Sphinx-7.0.0rc1/sphinx/locale/te/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84177 2023-04-23 19:57:27.411036 Sphinx-7.0.0rc1/sphinx/locale/te/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4099 2023-04-23 19:57:27.411036 Sphinx-7.0.0rc1/sphinx/locale/tr/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    58138 2023-04-23 19:57:27.412036 Sphinx-7.0.0rc1/sphinx/locale/tr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   109922 2023-04-23 19:57:27.412036 Sphinx-7.0.0rc1/sphinx/locale/tr/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     6344 2023-04-23 19:57:27.413036 Sphinx-7.0.0rc1/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6693 2023-04-23 19:57:27.413036 Sphinx-7.0.0rc1/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    87195 2023-04-23 19:57:27.413036 Sphinx-7.0.0rc1/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2361 2023-04-23 19:57:27.413036 Sphinx-7.0.0rc1/sphinx/locale/ur/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      487 2023-04-23 19:57:27.413036 Sphinx-7.0.0rc1/sphinx/locale/ur/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84175 2023-04-23 19:57:27.414036 Sphinx-7.0.0rc1/sphinx/locale/ur/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3581 2023-04-23 19:57:27.414036 Sphinx-7.0.0rc1/sphinx/locale/vi/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     5971 2023-04-23 19:57:27.414036 Sphinx-7.0.0rc1/sphinx/locale/vi/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86239 2023-04-23 19:57:27.414036 Sphinx-7.0.0rc1/sphinx/locale/vi/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2355 2023-04-23 19:57:27.415036 Sphinx-7.0.0rc1/sphinx/locale/yue/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      487 2023-04-23 19:57:27.415036 Sphinx-7.0.0rc1/sphinx/locale/yue/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84175 2023-04-23 19:57:27.415036 Sphinx-7.0.0rc1/sphinx/locale/yue/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4455 2023-04-23 19:57:27.415036 Sphinx-7.0.0rc1/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    76383 2023-04-23 19:57:27.416271 Sphinx-7.0.0rc1/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   116078 2023-04-23 19:57:27.416725 Sphinx-7.0.0rc1/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2362 2023-04-23 19:57:27.416725 Sphinx-7.0.0rc1/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      501 2023-04-23 19:57:27.416725 Sphinx-7.0.0rc1/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84189 2023-04-23 19:57:27.417852 Sphinx-7.0.0rc1/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2362 2023-04-23 19:57:27.417852 Sphinx-7.0.0rc1/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      516 2023-04-23 19:57:27.417852 Sphinx-7.0.0rc1/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84204 2023-04-23 19:57:27.417852 Sphinx-7.0.0rc1/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4639 2023-04-23 19:57:27.418852 Sphinx-7.0.0rc1/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    75797 2023-04-23 19:57:27.418852 Sphinx-7.0.0rc1/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   115249 2023-04-23 19:57:27.419852 Sphinx-7.0.0rc1/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3098 2023-04-23 19:57:27.419852 Sphinx-7.0.0rc1/sphinx/parsers.py
+-rw-r--r--   0        0        0     3432 2023-04-23 19:57:27.420852 Sphinx-7.0.0rc1/sphinx/project.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.420852 Sphinx-7.0.0rc1/sphinx/py.typed
+-rw-r--r--   0        0        0     5581 2023-04-23 19:57:27.420852 Sphinx-7.0.0rc1/sphinx/pycode/__init__.py
+-rw-r--r--   0        0        0     6648 2023-04-27 13:52:14.963498 Sphinx-7.0.0rc1/sphinx/pycode/ast.py
+-rw-r--r--   0        0        0    21072 2023-04-23 19:57:27.420852 Sphinx-7.0.0rc1/sphinx/pycode/parser.py
+-rw-r--r--   0        0        0     2861 2023-04-23 19:57:27.421852 Sphinx-7.0.0rc1/sphinx/pygments_styles.py
+-rw-r--r--   0        0        0    21983 2023-04-28 09:26:30.898486 Sphinx-7.0.0rc1/sphinx/registry.py
+-rw-r--r--   0        0        0    15975 2023-04-23 19:57:27.421852 Sphinx-7.0.0rc1/sphinx/roles.py
+-rw-r--r--   0        0        0    23064 2023-04-27 00:29:16.230978 Sphinx-7.0.0rc1/sphinx/search/__init__.py
+-rw-r--r--   0        0        0     3561 2023-04-23 19:57:27.422852 Sphinx-7.0.0rc1/sphinx/search/da.py
+-rw-r--r--   0        0        0     4637 2023-04-23 19:57:27.422852 Sphinx-7.0.0rc1/sphinx/search/de.py
+-rw-r--r--   0        0        0     4899 2023-04-23 19:57:27.422852 Sphinx-7.0.0rc1/sphinx/search/en.py
+-rw-r--r--   0        0        0     5723 2023-04-23 19:57:27.422852 Sphinx-7.0.0rc1/sphinx/search/es.py
+-rw-r--r--   0        0        0     3207 2023-04-23 19:57:27.423852 Sphinx-7.0.0rc1/sphinx/search/fi.py
+-rw-r--r--   0        0        0     3438 2023-04-23 19:57:27.423852 Sphinx-7.0.0rc1/sphinx/search/fr.py
+-rw-r--r--   0        0        0     1949 2023-04-23 19:57:27.423852 Sphinx-7.0.0rc1/sphinx/search/hu.py
+-rw-r--r--   0        0        0     5089 2023-04-23 19:57:27.424852 Sphinx-7.0.0rc1/sphinx/search/it.py
+-rw-r--r--   0        0        0    30997 2023-04-27 00:29:16.230978 Sphinx-7.0.0rc1/sphinx/search/ja.py
+-rw-r--r--   0        0        0     3594 2023-04-23 19:57:27.424852 Sphinx-7.0.0rc1/sphinx/search/minified-js/base-stemmer.js
+-rw-r--r--   0        0        0     3123 2023-04-23 19:57:27.424852 Sphinx-7.0.0rc1/sphinx/search/minified-js/danish-stemmer.js
+-rw-r--r--   0        0        0     5529 2023-04-23 19:57:27.425852 Sphinx-7.0.0rc1/sphinx/search/minified-js/dutch-stemmer.js
+-rw-r--r--   0        0        0     7529 2023-04-23 19:57:27.425852 Sphinx-7.0.0rc1/sphinx/search/minified-js/finnish-stemmer.js
+-rw-r--r--   0        0        0    11571 2023-04-23 19:57:27.426185 Sphinx-7.0.0rc1/sphinx/search/minified-js/french-stemmer.js
+-rw-r--r--   0        0        0     4669 2023-04-23 19:57:27.426185 Sphinx-7.0.0rc1/sphinx/search/minified-js/german-stemmer.js
+-rw-r--r--   0        0        0     6614 2023-04-23 19:57:27.426185 Sphinx-7.0.0rc1/sphinx/search/minified-js/hungarian-stemmer.js
+-rw-r--r--   0        0        0     9100 2023-04-23 19:57:27.426185 Sphinx-7.0.0rc1/sphinx/search/minified-js/italian-stemmer.js
+-rw-r--r--   0        0        0     2594 2023-04-23 19:57:27.426185 Sphinx-7.0.0rc1/sphinx/search/minified-js/norwegian-stemmer.js
+-rw-r--r--   0        0        0     6439 2023-04-23 19:57:27.427191 Sphinx-7.0.0rc1/sphinx/search/minified-js/porter-stemmer.js
+-rw-r--r--   0        0        0     8373 2023-04-23 19:57:27.427191 Sphinx-7.0.0rc1/sphinx/search/minified-js/portuguese-stemmer.js
+-rw-r--r--   0        0        0     8333 2023-04-23 19:57:27.427191 Sphinx-7.0.0rc1/sphinx/search/minified-js/romanian-stemmer.js
+-rw-r--r--   0        0        0     5735 2023-04-23 19:57:27.427191 Sphinx-7.0.0rc1/sphinx/search/minified-js/russian-stemmer.js
+-rw-r--r--   0        0        0     9121 2023-04-23 19:57:27.427191 Sphinx-7.0.0rc1/sphinx/search/minified-js/spanish-stemmer.js
+-rw-r--r--   0        0        0     2654 2023-04-23 19:57:27.427191 Sphinx-7.0.0rc1/sphinx/search/minified-js/swedish-stemmer.js
+-rw-r--r--   0        0        0    19972 2023-04-23 19:57:27.428192 Sphinx-7.0.0rc1/sphinx/search/minified-js/turkish-stemmer.js
+-rw-r--r--   0        0        0     4571 2023-04-23 19:57:27.428192 Sphinx-7.0.0rc1/sphinx/search/nl.py
+-rw-r--r--   0        0        0     4893 2023-04-23 19:57:27.428192 Sphinx-7.0.0rc1/sphinx/search/no.py
+-rw-r--r--   0        0        0     8133 2023-04-23 19:57:27.428192 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/base-stemmer.js
+-rw-r--r--   0        0        0     8134 2023-04-23 19:57:27.429191 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/danish-stemmer.js
+-rw-r--r--   0        0        0    19495 2023-04-23 19:57:27.429191 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/dutch-stemmer.js
+-rw-r--r--   0        0        0    21286 2023-04-23 19:57:27.429191 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/finnish-stemmer.js
+-rw-r--r--   0        0        0    42080 2023-04-23 19:57:27.429191 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/french-stemmer.js
+-rw-r--r--   0        0        0    17647 2023-04-23 19:57:27.430191 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/german-stemmer.js
+-rw-r--r--   0        0        0    17564 2023-04-23 19:57:27.430191 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/hungarian-stemmer.js
+-rw-r--r--   0        0        0    29065 2023-04-23 19:57:27.430191 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/italian-stemmer.js
+-rw-r--r--   0        0        0     6870 2023-04-23 19:57:27.430191 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/norwegian-stemmer.js
+-rw-r--r--   0        0        0    20391 2023-04-23 19:57:27.431192 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/porter-stemmer.js
+-rw-r--r--   0        0        0    26718 2023-04-23 19:57:27.431192 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/portuguese-stemmer.js
+-rw-r--r--   0        0        0    25006 2023-04-23 19:57:27.431192 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/romanian-stemmer.js
+-rw-r--r--   0        0        0    17996 2023-04-23 19:57:27.431192 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/russian-stemmer.js
+-rw-r--r--   0        0        0    28534 2023-04-23 19:57:27.431192 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/spanish-stemmer.js
+-rw-r--r--   0        0        0     6851 2023-04-23 19:57:27.432192 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/swedish-stemmer.js
+-rw-r--r--   0        0        0    77511 2023-04-23 19:57:27.432192 Sphinx-7.0.0rc1/sphinx/search/non-minified-js/turkish-stemmer.js
+-rw-r--r--   0        0        0     4648 2023-04-23 19:57:27.432192 Sphinx-7.0.0rc1/sphinx/search/pt.py
+-rw-r--r--   0        0        0      557 2023-04-23 19:57:27.432192 Sphinx-7.0.0rc1/sphinx/search/ro.py
+-rw-r--r--   0        0        0     7905 2023-04-23 19:57:27.433192 Sphinx-7.0.0rc1/sphinx/search/ru.py
+-rw-r--r--   0        0        0     3436 2023-04-23 19:57:27.433192 Sphinx-7.0.0rc1/sphinx/search/sv.py
+-rw-r--r--   0        0        0      551 2023-04-23 19:57:27.433192 Sphinx-7.0.0rc1/sphinx/search/tr.py
+-rw-r--r--   0        0        0     6146 2023-04-23 19:57:27.433192 Sphinx-7.0.0rc1/sphinx/search/zh.py
+-rw-r--r--   0        0        0      196 2023-04-23 19:57:27.434192 Sphinx-7.0.0rc1/sphinx/templates/apidoc/module.rst_t
+-rw-r--r--   0        0        0     1173 2023-04-23 19:57:27.434192 Sphinx-7.0.0rc1/sphinx/templates/apidoc/package.rst_t
+-rw-r--r--   0        0        0      128 2023-04-23 19:57:27.434192 Sphinx-7.0.0rc1/sphinx/templates/apidoc/toc.rst_t
+-rw-r--r--   0        0        0      246 2023-04-23 19:57:27.434192 Sphinx-7.0.0rc1/sphinx/templates/epub3/container.xml
+-rw-r--r--   0        0        0     2127 2023-04-23 19:57:27.434192 Sphinx-7.0.0rc1/sphinx/templates/epub3/content.opf_t
+-rw-r--r--   0        0        0       20 2023-04-23 19:57:27.434192 Sphinx-7.0.0rc1/sphinx/templates/epub3/mimetype
+-rw-r--r--   0        0        0      629 2023-04-23 19:57:27.435192 Sphinx-7.0.0rc1/sphinx/templates/epub3/nav.xhtml_t
+-rw-r--r--   0        0        0      743 2023-04-23 19:57:27.435192 Sphinx-7.0.0rc1/sphinx/templates/epub3/toc.ncx_t
+-rw-r--r--   0        0        0      875 2023-04-23 19:57:27.435192 Sphinx-7.0.0rc1/sphinx/templates/gettext/message.pot_t
+-rw-r--r--   0        0        0      299 2023-04-23 19:57:27.435192 Sphinx-7.0.0rc1/sphinx/templates/graphviz/graphviz.css
+-rw-r--r--   0        0        0      864 2023-04-23 19:57:27.435192 Sphinx-7.0.0rc1/sphinx/templates/htmlhelp/project.hhc
+-rw-r--r--   0        0        0      570 2023-04-23 19:57:27.436192 Sphinx-7.0.0rc1/sphinx/templates/htmlhelp/project.hhp
+-rw-r--r--   0        0        0      165 2023-04-25 10:59:46.881271 Sphinx-7.0.0rc1/sphinx/templates/htmlhelp/project.stp
+-rw-r--r--   0        0        0      397 2023-04-23 19:57:27.436192 Sphinx-7.0.0rc1/sphinx/templates/imgmath/preview.tex_t
+-rw-r--r--   0        0        0      321 2023-04-23 19:57:27.436192 Sphinx-7.0.0rc1/sphinx/templates/imgmath/template.tex_t
+-rw-r--r--   0        0        0     2986 2023-04-23 19:57:27.436192 Sphinx-7.0.0rc1/sphinx/templates/latex/latex.tex_t
+-rw-r--r--   0        0        0     2156 2023-04-23 19:57:27.437192 Sphinx-7.0.0rc1/sphinx/templates/latex/longtable.tex_t
+-rw-r--r--   0        0        0      944 2023-04-23 19:57:27.437192 Sphinx-7.0.0rc1/sphinx/templates/latex/sphinxmessages.sty_t
+-rw-r--r--   0        0        0     1406 2023-04-23 19:57:27.437192 Sphinx-7.0.0rc1/sphinx/templates/latex/tabular.tex_t
+-rw-r--r--   0        0        0     1420 2023-04-23 19:57:27.437192 Sphinx-7.0.0rc1/sphinx/templates/latex/tabulary.tex_t
+-rw-r--r--   0        0        0      656 2023-04-23 19:57:27.437192 Sphinx-7.0.0rc1/sphinx/templates/quickstart/Makefile.new_t
+-rw-r--r--   0        0        0     4031 2023-04-23 19:57:27.437192 Sphinx-7.0.0rc1/sphinx/templates/quickstart/Makefile_t
+-rw-r--r--   0        0        0     2129 2023-04-23 19:57:27.438192 Sphinx-7.0.0rc1/sphinx/templates/quickstart/conf.py_t
+-rw-r--r--   0        0        0      787 2023-04-23 19:57:27.438192 Sphinx-7.0.0rc1/sphinx/templates/quickstart/make.bat.new_t
+-rw-r--r--   0        0        0     3293 2023-04-23 19:57:27.438192 Sphinx-7.0.0rc1/sphinx/templates/quickstart/make.bat_t
+-rw-r--r--   0        0        0      492 2023-04-23 19:57:27.438192 Sphinx-7.0.0rc1/sphinx/templates/quickstart/root_doc.rst_t
+-rw-r--r--   0        0        0     1423 2023-04-23 19:57:27.438192 Sphinx-7.0.0rc1/sphinx/templates/texinfo/Makefile
+-rw-r--r--   0        0        0      171 2023-04-23 19:57:27.439192 Sphinx-7.0.0rc1/sphinx/testing/__init__.py
+-rw-r--r--   0        0        0     2710 2023-04-23 19:57:27.439192 Sphinx-7.0.0rc1/sphinx/testing/comparer.py
+-rw-r--r--   0        0        0     7508 2023-04-23 19:57:27.439192 Sphinx-7.0.0rc1/sphinx/testing/fixtures.py
+-rw-r--r--   0        0        0     6317 2023-04-25 10:53:02.931530 Sphinx-7.0.0rc1/sphinx/testing/path.py
+-rw-r--r--   0        0        0     1029 2023-04-23 19:57:27.439192 Sphinx-7.0.0rc1/sphinx/testing/restructuredtext.py
+-rw-r--r--   0        0        0     7297 2023-04-23 19:57:27.439192 Sphinx-7.0.0rc1/sphinx/testing/util.py
+-rw-r--r--   0        0        0     4366 2023-04-23 19:57:27.440192 Sphinx-7.0.0rc1/sphinx/texinputs/LICRcyr2utf8.xdy
+-rw-r--r--   0        0        0    10188 2023-04-23 19:57:27.440192 Sphinx-7.0.0rc1/sphinx/texinputs/LICRlatin2utf8.xdy
+-rw-r--r--   0        0        0    18890 2023-04-23 19:57:27.440192 Sphinx-7.0.0rc1/sphinx/texinputs/LatinRules.xdy
+-rw-r--r--   0        0        0     2401 2023-04-23 19:57:27.440192 Sphinx-7.0.0rc1/sphinx/texinputs/Makefile_t
+-rw-r--r--   0        0        0      695 2023-04-23 19:57:27.440192 Sphinx-7.0.0rc1/sphinx/texinputs/latexmkjarc_t
+-rw-r--r--   0        0        0     1104 2023-04-23 19:57:27.441192 Sphinx-7.0.0rc1/sphinx/texinputs/latexmkrc_t
+-rw-r--r--   0        0        0     1041 2023-04-23 19:57:27.441192 Sphinx-7.0.0rc1/sphinx/texinputs/make.bat_t
+-rw-r--r--   0        0        0      392 2023-04-23 19:57:27.441192 Sphinx-7.0.0rc1/sphinx/texinputs/python.ist
+-rw-r--r--   0        0        0    44560 2023-04-23 19:57:27.441192 Sphinx-7.0.0rc1/sphinx/texinputs/sphinx.sty
+-rw-r--r--   0        0        0     9474 2023-04-23 19:57:27.442192 Sphinx-7.0.0rc1/sphinx/texinputs/sphinx.xdy
+-rw-r--r--   0        0        0     3256 2023-04-23 19:57:27.442510 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxhowto.cls
+-rw-r--r--   0        0        0    10989 2023-04-23 19:57:27.442791 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexadmonitions.sty
+-rw-r--r--   0        0        0      901 2023-04-23 19:57:27.442999 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexcontainers.sty
+-rw-r--r--   0        0        0     4840 2023-04-23 19:57:27.443155 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexgraphics.sty
+-rw-r--r--   0        0        0     2066 2023-04-23 19:57:27.443155 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexindbibtoc.sty
+-rw-r--r--   0        0        0     5139 2023-04-23 19:57:27.443523 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexlists.sty
+-rw-r--r--   0        0        0    46048 2023-04-23 19:57:27.443889 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexliterals.sty
+-rw-r--r--   0        0        0     4532 2023-04-23 19:57:27.444274 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexnumfig.sty
+-rw-r--r--   0        0        0     9067 2023-04-23 19:57:27.444274 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexobjects.sty
+-rw-r--r--   0        0        0     5066 2023-04-23 19:57:27.444274 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexshadowbox.sty
+-rw-r--r--   0        0        0     3445 2023-04-23 19:57:27.444274 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexstyleheadings.sty
+-rw-r--r--   0        0        0     3064 2023-04-23 19:57:27.445286 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexstylepage.sty
+-rw-r--r--   0        0        0     8232 2023-04-23 19:57:27.445286 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexstyletext.sty
+-rw-r--r--   0        0        0    57830 2023-04-23 19:57:27.445286 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatextables.sty
+-rw-r--r--   0        0        0     4241 2023-04-23 19:57:27.445286 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxmanual.cls
+-rw-r--r--   0        0        0     2061 2023-04-23 19:57:27.446286 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxoptionsgeometry.sty
+-rw-r--r--   0        0        0     1094 2023-04-23 19:57:27.446286 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxoptionshyperref.sty
+-rw-r--r--   0        0        0    36615 2023-04-23 19:57:27.446286 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxpackageboxes.sty
+-rw-r--r--   0        0        0     2590 2023-04-23 19:57:27.446286 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxpackagecyrillic.sty
+-rw-r--r--   0        0        0    15254 2023-04-23 19:57:27.447286 Sphinx-7.0.0rc1/sphinx/texinputs/sphinxpackagefootnote.sty
+-rw-r--r--   0        0        0     2503 2023-04-23 19:57:27.447286 Sphinx-7.0.0rc1/sphinx/texinputs_win/Makefile_t
+-rw-r--r--   0        0        0     3321 2023-04-23 19:57:27.447286 Sphinx-7.0.0rc1/sphinx/themes/agogo/layout.html
+-rw-r--r--   0        0        0     9144 2023-04-23 19:57:27.448286 Sphinx-7.0.0rc1/sphinx/themes/agogo/static/agogo.css_t
+-rw-r--r--   0        0        0      276 2023-04-23 19:57:27.448286 Sphinx-7.0.0rc1/sphinx/themes/agogo/static/bgfooter.png
+-rw-r--r--   0        0        0      266 2023-04-23 19:57:27.448286 Sphinx-7.0.0rc1/sphinx/themes/agogo/static/bgtop.png
+-rw-r--r--   0        0        0      477 2023-04-23 19:57:27.448286 Sphinx-7.0.0rc1/sphinx/themes/agogo/theme.conf
+-rw-r--r--   0        0        0      466 2023-04-23 19:57:27.448286 Sphinx-7.0.0rc1/sphinx/themes/basic/changes/frameset.html
+-rw-r--r--   0        0        0      485 2023-04-23 19:57:27.448286 Sphinx-7.0.0rc1/sphinx/themes/basic/changes/rstsource.html
+-rw-r--r--   0        0        0     1306 2023-04-23 19:57:27.449286 Sphinx-7.0.0rc1/sphinx/themes/basic/changes/versionchanges.html
+-rw-r--r--   0        0        0     1636 2023-04-23 19:57:27.449286 Sphinx-7.0.0rc1/sphinx/themes/basic/defindex.html
+-rw-r--r--   0        0        0     1892 2023-04-23 19:57:27.449286 Sphinx-7.0.0rc1/sphinx/themes/basic/domainindex.html
+-rw-r--r--   0        0        0     1804 2023-04-23 19:57:27.449286 Sphinx-7.0.0rc1/sphinx/themes/basic/genindex-single.html
+-rw-r--r--   0        0        0     1210 2023-04-23 19:57:27.449286 Sphinx-7.0.0rc1/sphinx/themes/basic/genindex-split.html
+-rw-r--r--   0        0        0     2069 2023-04-23 19:57:27.449286 Sphinx-7.0.0rc1/sphinx/themes/basic/genindex.html
+-rw-r--r--   0        0        0      432 2023-04-23 19:57:27.450286 Sphinx-7.0.0rc1/sphinx/themes/basic/globaltoc.html
+-rw-r--r--   0        0        0     7128 2023-04-28 10:59:41.037038 Sphinx-7.0.0rc1/sphinx/themes/basic/layout.html
+-rw-r--r--   0        0        0      370 2023-04-23 19:57:27.450286 Sphinx-7.0.0rc1/sphinx/themes/basic/localtoc.html
+-rw-r--r--   0        0        0      679 2023-04-23 19:57:27.450286 Sphinx-7.0.0rc1/sphinx/themes/basic/opensearch.xml
+-rw-r--r--   0        0        0      273 2023-04-23 19:57:27.450286 Sphinx-7.0.0rc1/sphinx/themes/basic/page.html
+-rw-r--r--   0        0        0      652 2023-04-23 19:57:27.450286 Sphinx-7.0.0rc1/sphinx/themes/basic/relations.html
+-rw-r--r--   0        0        0     2039 2023-04-23 19:57:27.450286 Sphinx-7.0.0rc1/sphinx/themes/basic/search.html
+-rw-r--r--   0        0        0      809 2023-04-23 19:57:27.451286 Sphinx-7.0.0rc1/sphinx/themes/basic/searchbox.html
+-rw-r--r--   0        0        0      947 2023-04-23 19:57:27.451286 Sphinx-7.0.0rc1/sphinx/themes/basic/searchfield.html
+-rw-r--r--   0        0        0      544 2023-04-23 19:57:27.451286 Sphinx-7.0.0rc1/sphinx/themes/basic/sourcelink.html
+-rw-r--r--   0        0        0    14893 2023-04-23 19:57:27.451286 Sphinx-7.0.0rc1/sphinx/themes/basic/static/basic.css_t
+-rw-r--r--   0        0        0     4472 2023-04-23 19:57:27.452286 Sphinx-7.0.0rc1/sphinx/themes/basic/static/doctools.js
+-rw-r--r--   0        0        0      673 2023-04-23 19:57:27.452286 Sphinx-7.0.0rc1/sphinx/themes/basic/static/documentation_options.js_t
+-rw-r--r--   0        0        0      286 2023-04-23 19:57:27.452286 Sphinx-7.0.0rc1/sphinx/themes/basic/static/file.png
+-rw-r--r--   0        0        0      676 2023-04-23 19:57:27.452286 Sphinx-7.0.0rc1/sphinx/themes/basic/static/language_data.js_t
+-rw-r--r--   0        0        0       90 2023-04-23 19:57:27.452286 Sphinx-7.0.0rc1/sphinx/themes/basic/static/minus.png
+-rw-r--r--   0        0        0       90 2023-04-23 19:57:27.452286 Sphinx-7.0.0rc1/sphinx/themes/basic/static/plus.png
+-rw-r--r--   0        0        0    18215 2023-04-23 19:57:27.453287 Sphinx-7.0.0rc1/sphinx/themes/basic/static/searchtools.js
+-rw-r--r--   0        0        0     4712 2023-04-23 19:57:27.453287 Sphinx-7.0.0rc1/sphinx/themes/basic/static/sphinx_highlight.js
+-rw-r--r--   0        0        0      371 2023-04-23 19:57:27.453287 Sphinx-7.0.0rc1/sphinx/themes/basic/theme.conf
+-rw-r--r--   0        0        0      664 2023-04-23 19:57:27.454287 Sphinx-7.0.0rc1/sphinx/themes/bizstyle/layout.html
+-rw-r--r--   0        0        0       78 2023-04-23 19:57:27.454287 Sphinx-7.0.0rc1/sphinx/themes/bizstyle/static/background_b01.png
+-rw-r--r--   0        0        0    10314 2023-04-23 19:57:27.454287 Sphinx-7.0.0rc1/sphinx/themes/bizstyle/static/bizstyle.css_t
+-rw-r--r--   0        0        0     1129 2023-04-23 19:57:27.454287 Sphinx-7.0.0rc1/sphinx/themes/bizstyle/static/bizstyle.js_t
+-rw-r--r--   0        0        0    14940 2023-04-23 19:57:27.455286 Sphinx-7.0.0rc1/sphinx/themes/bizstyle/static/css3-mediaqueries.js
+-rw-r--r--   0        0        0    28634 2023-04-23 19:57:27.455286 Sphinx-7.0.0rc1/sphinx/themes/bizstyle/static/css3-mediaqueries_src.js
+-rw-r--r--   0        0        0      148 2023-04-23 19:57:27.455286 Sphinx-7.0.0rc1/sphinx/themes/bizstyle/theme.conf
+-rw-r--r--   0        0        0      661 2023-04-23 19:57:27.455286 Sphinx-7.0.0rc1/sphinx/themes/classic/layout.html
+-rw-r--r--   0        0        0     6635 2023-04-23 19:57:27.456285 Sphinx-7.0.0rc1/sphinx/themes/classic/static/classic.css_t
+-rw-r--r--   0        0        0     2659 2023-04-23 19:57:27.456285 Sphinx-7.0.0rc1/sphinx/themes/classic/static/sidebar.js_t
+-rw-r--r--   0        0        0      719 2023-04-23 19:57:27.456285 Sphinx-7.0.0rc1/sphinx/themes/classic/theme.conf
+-rw-r--r--   0        0        0       28 2023-04-23 19:57:27.456285 Sphinx-7.0.0rc1/sphinx/themes/default/static/default.css
+-rw-r--r--   0        0        0       26 2023-04-23 19:57:27.457285 Sphinx-7.0.0rc1/sphinx/themes/default/theme.conf
+-rw-r--r--   0        0        0      693 2023-04-23 19:57:27.457285 Sphinx-7.0.0rc1/sphinx/themes/epub/epub-cover.html
+-rw-r--r--   0        0        0      543 2023-04-23 19:57:27.457285 Sphinx-7.0.0rc1/sphinx/themes/epub/layout.html
+-rw-r--r--   0        0        0    12262 2023-04-23 19:57:27.457285 Sphinx-7.0.0rc1/sphinx/themes/epub/static/epub.css_t
+-rw-r--r--   0        0        0      108 2023-04-23 19:57:27.457285 Sphinx-7.0.0rc1/sphinx/themes/epub/theme.conf
+-rw-r--r--   0        0        0     2012 2023-04-23 19:57:27.458401 Sphinx-7.0.0rc1/sphinx/themes/haiku/layout.html
+-rw-r--r--   0        0        0     1128 2023-04-23 19:57:27.458401 Sphinx-7.0.0rc1/sphinx/themes/haiku/static/alert_info_32.png
+-rw-r--r--   0        0        0      944 2023-04-23 19:57:27.458401 Sphinx-7.0.0rc1/sphinx/themes/haiku/static/alert_warning_32.png
+-rw-r--r--   0        0        0       82 2023-04-23 19:57:27.458401 Sphinx-7.0.0rc1/sphinx/themes/haiku/static/bg-page.png
+-rw-r--r--   0        0        0      165 2023-04-23 19:57:27.458401 Sphinx-7.0.0rc1/sphinx/themes/haiku/static/bullet_orange.png
+-rw-r--r--   0        0        0     7059 2023-04-23 19:57:27.458401 Sphinx-7.0.0rc1/sphinx/themes/haiku/static/haiku.css_t
+-rw-r--r--   0        0        0      298 2023-04-23 19:57:27.458401 Sphinx-7.0.0rc1/sphinx/themes/haiku/theme.conf
+-rw-r--r--   0        0        0     4234 2023-04-23 19:57:27.459407 Sphinx-7.0.0rc1/sphinx/themes/nature/static/nature.css_t
+-rw-r--r--   0        0        0       71 2023-04-23 19:57:27.459407 Sphinx-7.0.0rc1/sphinx/themes/nature/theme.conf
+-rw-r--r--   0        0        0      642 2023-04-23 19:57:27.459407 Sphinx-7.0.0rc1/sphinx/themes/nonav/layout.html
+-rw-r--r--   0        0        0     9636 2023-04-23 19:57:27.460407 Sphinx-7.0.0rc1/sphinx/themes/nonav/static/nonav.css_t
+-rw-r--r--   0        0        0      109 2023-04-23 19:57:27.460407 Sphinx-7.0.0rc1/sphinx/themes/nonav/theme.conf
+-rw-r--r--   0        0        0      875 2023-04-23 19:57:27.460407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/layout.html
+-rw-r--r--   0        0        0     1394 2023-04-23 19:57:27.460407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/dialog-note.png
+-rw-r--r--   0        0        0     1351 2023-04-23 19:57:27.460407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/dialog-seealso.png
+-rw-r--r--   0        0        0     1186 2023-04-23 19:57:27.461407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/dialog-todo.png
+-rw-r--r--   0        0        0     1798 2023-04-23 19:57:27.461407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/dialog-topic.png
+-rw-r--r--   0        0        0     1280 2023-04-23 19:57:27.461407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/dialog-warning.png
+-rw-r--r--   0        0        0     5629 2023-04-23 19:57:27.461407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/epub.css_t
+-rw-r--r--   0        0        0      333 2023-04-23 19:57:27.461407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/footerbg.png
+-rw-r--r--   0        0        0      190 2023-04-23 19:57:27.461407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/headerbg.png
+-rw-r--r--   0        0        0      726 2023-04-23 19:57:27.461407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/ie6.css
+-rw-r--r--   0        0        0      101 2023-04-23 19:57:27.462407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/middlebg.png
+-rw-r--r--   0        0        0     6301 2023-04-23 19:57:27.462407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/pyramid.css_t
+-rw-r--r--   0        0        0       49 2023-04-23 19:57:27.462407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/transparent.gif
+-rw-r--r--   0        0        0      102 2023-04-23 19:57:27.462407 Sphinx-7.0.0rc1/sphinx/themes/pyramid/theme.conf
+-rw-r--r--   0        0        0     5775 2023-04-23 19:57:27.462407 Sphinx-7.0.0rc1/sphinx/themes/scrolls/artwork/logo.svg
+-rw-r--r--   0        0        0     1661 2023-04-23 19:57:27.463407 Sphinx-7.0.0rc1/sphinx/themes/scrolls/layout.html
+-rw-r--r--   0        0        0    25238 2023-04-23 19:57:27.463407 Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/darkmetal.png
+-rw-r--r--   0        0        0      172 2023-04-23 19:57:27.463407 Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/headerbg.png
+-rw-r--r--   0        0        0     8305 2023-04-23 19:57:27.463407 Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/logo.png
+-rw-r--r--   0        0        0     7547 2023-04-23 19:57:27.463407 Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/metal.png
+-rw-r--r--   0        0        0      124 2023-04-23 19:57:27.464407 Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/navigation.png
+-rw-r--r--   0        0        0      303 2023-04-23 19:57:27.464407 Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/print.css
+-rw-r--r--   0        0        0     7977 2023-04-23 19:57:27.464407 Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/scrolls.css_t
+-rw-r--r--   0        0        0      527 2023-04-23 19:57:27.464407 Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/theme_extras.js
+-rw-r--r--   0        0        0    44483 2023-04-23 19:57:27.465407 Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/watermark.png
+-rw-r--r--   0        0        0     8049 2023-04-23 19:57:27.465407 Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/watermark_blur.png
+-rw-r--r--   0        0        0      260 2023-04-23 19:57:27.465407 Sphinx-7.0.0rc1/sphinx/themes/scrolls/theme.conf
+-rw-r--r--   0        0        0      107 2023-04-23 19:57:27.465407 Sphinx-7.0.0rc1/sphinx/themes/sphinxdoc/static/contents.png
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.465407 Sphinx-7.0.0rc1/sphinx/themes/sphinxdoc/static/navigation.png
+-rw-r--r--   0        0        0     6314 2023-04-23 19:57:27.465407 Sphinx-7.0.0rc1/sphinx/themes/sphinxdoc/static/sphinxdoc.css_t
+-rw-r--r--   0        0        0       77 2023-04-23 19:57:27.466407 Sphinx-7.0.0rc1/sphinx/themes/sphinxdoc/theme.conf
+-rw-r--r--   0        0        0    12162 2023-04-23 19:57:27.466407 Sphinx-7.0.0rc1/sphinx/themes/traditional/static/traditional.css_t
+-rw-r--r--   0        0        0      105 2023-04-23 19:57:27.466407 Sphinx-7.0.0rc1/sphinx/themes/traditional/theme.conf
+-rw-r--r--   0        0        0     7937 2023-04-23 19:57:27.466407 Sphinx-7.0.0rc1/sphinx/theming.py
+-rw-r--r--   0        0        0    14420 2023-04-23 19:57:27.467407 Sphinx-7.0.0rc1/sphinx/transforms/__init__.py
+-rw-r--r--   0        0        0     2768 2023-04-23 19:57:27.467407 Sphinx-7.0.0rc1/sphinx/transforms/compact_bullet_list.py
+-rw-r--r--   0        0        0    23400 2023-04-23 19:57:27.467407 Sphinx-7.0.0rc1/sphinx/transforms/i18n.py
+-rw-r--r--   0        0        0    12011 2023-04-23 19:57:27.467407 Sphinx-7.0.0rc1/sphinx/transforms/post_transforms/__init__.py
+-rw-r--r--   0        0        0     4486 2023-04-23 19:57:27.468408 Sphinx-7.0.0rc1/sphinx/transforms/post_transforms/code.py
+-rw-r--r--   0        0        0    10043 2023-04-23 19:57:27.468408 Sphinx-7.0.0rc1/sphinx/transforms/post_transforms/images.py
+-rw-r--r--   0        0        0     1361 2023-04-23 19:57:27.468408 Sphinx-7.0.0rc1/sphinx/transforms/references.py
+-rw-r--r--   0        0        0    12535 2023-04-27 14:47:43.282341 Sphinx-7.0.0rc1/sphinx/util/__init__.py
+-rw-r--r--   0        0        0      240 2023-04-23 19:57:27.468408 Sphinx-7.0.0rc1/sphinx/util/build_phase.py
+-rw-r--r--   0        0        0    15290 2023-04-23 19:57:27.469407 Sphinx-7.0.0rc1/sphinx/util/cfamily.py
+-rw-r--r--   0        0        0     3218 2023-04-23 19:57:27.469407 Sphinx-7.0.0rc1/sphinx/util/console.py
+-rw-r--r--   0        0        0     2281 2023-04-23 19:57:27.469407 Sphinx-7.0.0rc1/sphinx/util/display.py
+-rw-r--r--   0        0        0    16330 2023-04-23 19:57:27.469407 Sphinx-7.0.0rc1/sphinx/util/docfields.py
+-rw-r--r--   0        0        0     2930 2023-04-23 19:57:27.470407 Sphinx-7.0.0rc1/sphinx/util/docstrings.py
+-rw-r--r--   0        0        0    22713 2023-04-28 09:03:22.692472 Sphinx-7.0.0rc1/sphinx/util/docutils.py
+-rw-r--r--   0        0        0     1960 2023-04-23 19:57:27.470407 Sphinx-7.0.0rc1/sphinx/util/exceptions.py
+-rw-r--r--   0        0        0     3722 2023-04-23 19:57:27.470407 Sphinx-7.0.0rc1/sphinx/util/fileutil.py
+-rw-r--r--   0        0        0      513 2023-04-23 19:57:27.470407 Sphinx-7.0.0rc1/sphinx/util/http_date.py
+-rw-r--r--   0        0        0     9598 2023-04-27 00:28:57.465794 Sphinx-7.0.0rc1/sphinx/util/i18n.py
+-rw-r--r--   0        0        0     3451 2023-04-23 19:57:27.471407 Sphinx-7.0.0rc1/sphinx/util/images.py
+-rw-r--r--   0        0        0    28244 2023-04-23 19:57:27.471407 Sphinx-7.0.0rc1/sphinx/util/inspect.py
+-rw-r--r--   0        0        0     6311 2023-04-23 19:57:27.472407 Sphinx-7.0.0rc1/sphinx/util/inventory.py
+-rw-r--r--   0        0        0    18103 2023-04-23 19:57:27.472407 Sphinx-7.0.0rc1/sphinx/util/logging.py
+-rw-r--r--   0        0        0     5274 2023-04-23 19:57:27.472407 Sphinx-7.0.0rc1/sphinx/util/matching.py
+-rw-r--r--   0        0        0     1816 2023-04-23 19:57:27.473407 Sphinx-7.0.0rc1/sphinx/util/math.py
+-rw-r--r--   0        0        0    22872 2023-04-23 19:57:27.473407 Sphinx-7.0.0rc1/sphinx/util/nodes.py
+-rw-r--r--   0        0        0     6973 2023-04-23 19:57:27.473407 Sphinx-7.0.0rc1/sphinx/util/osutil.py
+-rw-r--r--   0        0        0     5023 2023-04-23 19:57:27.473407 Sphinx-7.0.0rc1/sphinx/util/parallel.py
+-rw-r--r--   0        0        0     1445 2023-04-23 19:57:27.474408 Sphinx-7.0.0rc1/sphinx/util/png.py
+-rw-r--r--   0        0        0     2870 2023-04-23 19:57:27.474408 Sphinx-7.0.0rc1/sphinx/util/requests.py
+-rw-r--r--   0        0        0     3330 2023-04-23 19:57:27.474408 Sphinx-7.0.0rc1/sphinx/util/rst.py
+-rw-r--r--   0        0        0     2651 2023-04-23 19:57:27.475407 Sphinx-7.0.0rc1/sphinx/util/tags.py
+-rw-r--r--   0        0        0     4691 2023-04-23 19:57:27.475407 Sphinx-7.0.0rc1/sphinx/util/template.py
+-rw-r--r--   0        0        0     5442 2023-04-23 19:57:27.475407 Sphinx-7.0.0rc1/sphinx/util/texescape.py
+-rw-r--r--   0        0        0    14984 2023-04-23 19:57:27.475407 Sphinx-7.0.0rc1/sphinx/util/typing.py
+-rw-r--r--   0        0        0     5801 2023-04-23 19:57:27.475407 Sphinx-7.0.0rc1/sphinx/versioning.py
+-rw-r--r--   0        0        0       31 2023-04-23 19:57:27.476407 Sphinx-7.0.0rc1/sphinx/writers/__init__.py
+-rw-r--r--   0        0        0     1605 2023-04-28 10:59:41.037038 Sphinx-7.0.0rc1/sphinx/writers/html.py
+-rw-r--r--   0        0        0    31991 2023-04-23 19:57:27.477407 Sphinx-7.0.0rc1/sphinx/writers/html5.py
+-rw-r--r--   0        0        0    84706 2023-04-28 09:42:17.461902 Sphinx-7.0.0rc1/sphinx/writers/latex.py
+-rw-r--r--   0        0        0    15475 2023-04-23 19:57:27.478407 Sphinx-7.0.0rc1/sphinx/writers/manpage.py
+-rw-r--r--   0        0        0    52823 2023-04-23 19:57:27.478407 Sphinx-7.0.0rc1/sphinx/writers/texinfo.py
+-rw-r--r--   0        0        0    37916 2023-04-23 19:57:27.479408 Sphinx-7.0.0rc1/sphinx/writers/text.py
+-rw-r--r--   0        0        0     1457 2023-04-23 19:57:27.479408 Sphinx-7.0.0rc1/sphinx/writers/xml.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.479408 Sphinx-7.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     3054 2023-04-23 19:57:27.479408 Sphinx-7.0.0rc1/tests/certs/cert.pem
+-rw-r--r--   0        0        0     1574 2023-04-23 19:57:27.480407 Sphinx-7.0.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0      363 2023-04-23 19:57:27.480407 Sphinx-7.0.0rc1/tests/ext_napoleon_pep526_data_google.py
+-rw-r--r--   0        0        0      385 2023-04-23 19:57:27.480407 Sphinx-7.0.0rc1/tests/ext_napoleon_pep526_data_numpy.py
+-rw-r--r--   0        0        0       34 2023-04-23 19:57:27.480407 Sphinx-7.0.0rc1/tests/js/documentation_options.js
+-rw-r--r--   0        0        0     1694 2023-04-23 19:57:27.480407 Sphinx-7.0.0rc1/tests/js/searchtools.js
+-rw-r--r--   0        0        0     1985 2023-04-23 19:57:27.481407 Sphinx-7.0.0rc1/tests/js/sphinx_highlight.js
+-rw-r--r--   0        0        0      111 2023-04-23 19:57:27.481407 Sphinx-7.0.0rc1/tests/roots/test-add_enumerable_node/conf.py
+-rw-r--r--   0        0        0     1464 2023-04-23 19:57:27.481407 Sphinx-7.0.0rc1/tests/roots/test-add_enumerable_node/enumerable_node.py
+-rw-r--r--   0        0        0      763 2023-04-23 19:57:27.481407 Sphinx-7.0.0rc1/tests/roots/test-add_enumerable_node/index.rst
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.481407 Sphinx-7.0.0rc1/tests/roots/test-add_enumerable_node/rimg.png
+-rw-r--r--   0        0        0      277 2023-04-23 19:57:27.481407 Sphinx-7.0.0rc1/tests/roots/test-add_source_parser-conflicts-with-users-setting/conf.py
+-rw-r--r--   0        0        0      201 2023-04-23 19:57:27.482407 Sphinx-7.0.0rc1/tests/roots/test-add_source_parser-conflicts-with-users-setting/source_parser.py
+-rw-r--r--   0        0        0      121 2023-04-23 19:57:27.482407 Sphinx-7.0.0rc1/tests/roots/test-add_source_parser/conf.py
+-rw-r--r--   0        0        0      201 2023-04-23 19:57:27.482407 Sphinx-7.0.0rc1/tests/roots/test-add_source_parser/source_parser.py
+-rw-r--r--   0        0        0     1659 2023-04-23 19:57:27.482407 Sphinx-7.0.0rc1/tests/roots/test-api-set-translator/conf.py
+-rw-r--r--   0        0        0       72 2023-04-23 19:57:27.482407 Sphinx-7.0.0rc1/tests/roots/test-api-set-translator/index.rst
+-rw-r--r--   0        0        0       98 2023-04-23 19:57:27.483407 Sphinx-7.0.0rc1/tests/roots/test-api-set-translator/nonext/conf.py
+-rw-r--r--   0        0        0      101 2023-04-23 19:57:27.483407 Sphinx-7.0.0rc1/tests/roots/test-api-set-translator/translator.py
+-rw-r--r--   0        0        0        0 2023-04-25 10:59:46.881271 Sphinx-7.0.0rc1/tests/roots/test-apidoc-duplicates/fish_licence/halibut.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.483407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-duplicates/fish_licence/halibut.pyx
+-rw-r--r--   0        0        0       12 2023-04-23 19:57:27.484407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-pep420/a/b/c/__init__.py
+-rw-r--r--   0        0        0       11 2023-04-23 19:57:27.484407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-pep420/a/b/c/d.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.484407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-pep420/a/b/e/__init__.py
+-rw-r--r--   0        0        0       11 2023-04-23 19:57:27.484407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-pep420/a/b/e/f.py
+-rw-r--r--   0        0        0       11 2023-04-23 19:57:27.484407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-pep420/a/b/x/y.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.484407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-subpackage-in-toc/parent/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.485407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-subpackage-in-toc/parent/child/__init__.py
+-rw-r--r--   0        0        0        6 2023-04-23 19:57:27.485407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-subpackage-in-toc/parent/child/foo.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.485407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-toc/mypackage/__init__.py
+-rw-r--r--   0        0        0      404 2023-04-25 10:59:46.885153 Sphinx-7.0.0rc1/tests/roots/test-apidoc-toc/mypackage/main.py
+-rw-r--r--   0        0        0       79 2023-04-23 19:57:27.485407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-toc/mypackage/no_init/foo.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.485407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-toc/mypackage/resource/__init__.py
+-rw-r--r--   0        0        0       96 2023-04-23 19:57:27.486407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-toc/mypackage/resource/resource.txt
+-rw-r--r--   0        0        0       23 2023-04-23 19:57:27.486407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-toc/mypackage/something/__init__.py
+-rw-r--r--   0        0        0       44 2023-04-23 19:57:27.486407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-trailing-underscore/package_/__init__.py
+-rw-r--r--   0        0        0      215 2023-04-23 19:57:27.486407 Sphinx-7.0.0rc1/tests/roots/test-apidoc-trailing-underscore/package_/module_.py
+-rw-r--r--   0        0        0      221 2023-04-23 19:57:27.486407 Sphinx-7.0.0rc1/tests/roots/test-autosummary/conf.py
+-rw-r--r--   0        0        0     1335 2023-04-23 19:57:27.487407 Sphinx-7.0.0rc1/tests/roots/test-autosummary/dummy_module.py
+-rw-r--r--   0        0        0       98 2023-04-23 19:57:27.487407 Sphinx-7.0.0rc1/tests/roots/test-autosummary/index.rst
+-rw-r--r--   0        0        0      507 2023-04-23 19:57:27.487407 Sphinx-7.0.0rc1/tests/roots/test-autosummary/sphinx.rst
+-rw-r--r--   0        0        0      198 2023-04-23 19:57:27.487407 Sphinx-7.0.0rc1/tests/roots/test-autosummary/underscore_module_.py
+-rw-r--r--   0        0        0      114 2023-04-23 19:57:27.487407 Sphinx-7.0.0rc1/tests/roots/test-basic/conf.py
+-rw-r--r--   0        0        0     1477 2023-04-27 00:31:27.920451 Sphinx-7.0.0rc1/tests/roots/test-basic/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.488407 Sphinx-7.0.0rc1/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/_static/extra.css
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.488407 Sphinx-7.0.0rc1/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/_static/mytheme.css
+-rw-r--r--   0        0        0       60 2023-04-23 19:57:27.488407 Sphinx-7.0.0rc1/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/theme.conf
+-rw-r--r--   0        0        0       53 2023-04-23 19:57:27.488407 Sphinx-7.0.0rc1/tests/roots/test-build-html-theme-having-multiple-stylesheets/conf.py
+-rw-r--r--   0        0        0      100 2023-04-23 19:57:27.488407 Sphinx-7.0.0rc1/tests/roots/test-build-html-theme-having-multiple-stylesheets/index.rst
+-rw-r--r--   0        0        0      372 2023-04-23 19:57:27.488407 Sphinx-7.0.0rc1/tests/roots/test-build-html-translator/conf.py
+-rw-r--r--   0        0        0      252 2023-04-23 19:57:27.489407 Sphinx-7.0.0rc1/tests/roots/test-build-html-translator/index.rst
+-rw-r--r--   0        0        0       53 2023-04-23 19:57:27.489407 Sphinx-7.0.0rc1/tests/roots/test-build-text/conf.py
+-rw-r--r--   0        0        0       20 2023-04-23 19:57:27.489407 Sphinx-7.0.0rc1/tests/roots/test-build-text/doc1.txt
+-rw-r--r--   0        0        0       51 2023-04-23 19:57:27.489407 Sphinx-7.0.0rc1/tests/roots/test-build-text/doc2.txt
+-rw-r--r--   0        0        0      135 2023-04-23 19:57:27.489407 Sphinx-7.0.0rc1/tests/roots/test-build-text/index.txt
+-rw-r--r--   0        0        0       62 2023-04-23 19:57:27.489407 Sphinx-7.0.0rc1/tests/roots/test-build-text/lineblock.txt
+-rw-r--r--   0        0        0       40 2023-04-23 19:57:27.489407 Sphinx-7.0.0rc1/tests/roots/test-build-text/listitems.txt
+-rw-r--r--   0        0        0      388 2023-04-23 19:57:27.489407 Sphinx-7.0.0rc1/tests/roots/test-build-text/maxwidth.txt
+-rw-r--r--   0        0        0      478 2023-04-23 19:57:27.490407 Sphinx-7.0.0rc1/tests/roots/test-build-text/nonascii_maxwidth.txt
+-rw-r--r--   0        0        0       75 2023-04-23 19:57:27.490407 Sphinx-7.0.0rc1/tests/roots/test-build-text/nonascii_table.txt
+-rw-r--r--   0        0        0       17 2023-04-23 19:57:27.490407 Sphinx-7.0.0rc1/tests/roots/test-build-text/nonascii_title.txt
+-rw-r--r--   0        0        0       98 2023-04-23 19:57:27.490407 Sphinx-7.0.0rc1/tests/roots/test-build-text/table.txt
+-rw-r--r--   0        0        0       98 2023-04-23 19:57:27.490407 Sphinx-7.0.0rc1/tests/roots/test-build-text/table_colspan.txt
+-rw-r--r--   0        0        0      140 2023-04-23 19:57:27.490407 Sphinx-7.0.0rc1/tests/roots/test-build-text/table_colspan_and_rowspan.txt
+-rw-r--r--   0        0        0       98 2023-04-23 19:57:27.490407 Sphinx-7.0.0rc1/tests/roots/test-build-text/table_colspan_left.txt
+-rw-r--r--   0        0        0       98 2023-04-23 19:57:27.490407 Sphinx-7.0.0rc1/tests/roots/test-build-text/table_rowspan.txt
+-rw-r--r--   0        0        0       18 2023-04-23 19:57:27.491407 Sphinx-7.0.0rc1/tests/roots/test-builder-dirhtml/bar.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.491407 Sphinx-7.0.0rc1/tests/roots/test-builder-dirhtml/conf.py
+-rw-r--r--   0        0        0       32 2023-04-23 19:57:27.491407 Sphinx-7.0.0rc1/tests/roots/test-builder-dirhtml/foo/foo_1.rst
+-rw-r--r--   0        0        0       32 2023-04-23 19:57:27.491407 Sphinx-7.0.0rc1/tests/roots/test-builder-dirhtml/foo/foo_2.rst
+-rw-r--r--   0        0        0       63 2023-04-23 19:57:27.491407 Sphinx-7.0.0rc1/tests/roots/test-builder-dirhtml/foo/index.rst
+-rw-r--r--   0        0        0       59 2023-04-23 19:57:27.491407 Sphinx-7.0.0rc1/tests/roots/test-builder-dirhtml/index.rst
+-rw-r--r--   0        0        0       74 2023-04-23 19:57:27.491407 Sphinx-7.0.0rc1/tests/roots/test-builder-gettext-dont-rebuild-mo/bom.rst
+-rw-r--r--   0        0        0       16 2023-04-23 19:57:27.492406 Sphinx-7.0.0rc1/tests/roots/test-builder-gettext-dont-rebuild-mo/conf.py
+-rw-r--r--   0        0        0      108 2023-04-23 19:57:27.492406 Sphinx-7.0.0rc1/tests/roots/test-builder-gettext-dont-rebuild-mo/index.rst
+-rw-r--r--   0        0        0      264 2023-04-23 19:57:27.492406 Sphinx-7.0.0rc1/tests/roots/test-builder-gettext-dont-rebuild-mo/xx/LC_MESSAGES/bom.po
+-rw-r--r--   0        0        0      330 2023-04-23 19:57:27.492406 Sphinx-7.0.0rc1/tests/roots/test-changes/base.rst
+-rw-r--r--   0        0        0      371 2023-04-23 19:57:27.492406 Sphinx-7.0.0rc1/tests/roots/test-changes/c-api.rst
+-rw-r--r--   0        0        0      134 2023-04-23 19:57:27.492406 Sphinx-7.0.0rc1/tests/roots/test-changes/conf.py
+-rw-r--r--   0        0        0      189 2023-04-23 19:57:27.493407 Sphinx-7.0.0rc1/tests/roots/test-changes/contents.rst
+-rw-r--r--   0        0        0      443 2023-04-23 19:57:27.493407 Sphinx-7.0.0rc1/tests/roots/test-changes/library/utils.rst
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.493407 Sphinx-7.0.0rc1/tests/roots/test-circular/conf.py
+-rw-r--r--   0        0        0       22 2023-04-23 19:57:27.493407 Sphinx-7.0.0rc1/tests/roots/test-circular/index.rst
+-rw-r--r--   0        0        0       23 2023-04-23 19:57:27.493407 Sphinx-7.0.0rc1/tests/roots/test-circular/sub.rst
+-rw-r--r--   0        0        0       81 2023-04-23 19:57:27.494407 Sphinx-7.0.0rc1/tests/roots/test-config/conf.py
+-rw-r--r--   0        0        0       32 2023-04-23 19:57:27.494407 Sphinx-7.0.0rc1/tests/roots/test-correct-year/conf.py
+-rw-r--r--   0        0        0       55 2023-04-23 19:57:27.494407 Sphinx-7.0.0rc1/tests/roots/test-correct-year/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.494407 Sphinx-7.0.0rc1/tests/roots/test-default_role/conf.py
+-rw-r--r--   0        0        0       29 2023-04-23 19:57:27.494407 Sphinx-7.0.0rc1/tests/roots/test-default_role/foo.rst
+-rw-r--r--   0        0        0       54 2023-04-23 19:57:27.494407 Sphinx-7.0.0rc1/tests/roots/test-default_role/index.rst
+-rw-r--r--   0        0        0      762 2023-04-23 19:57:27.495407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/caption.rst
+-rw-r--r--   0        0        0      263 2023-04-23 19:57:27.495407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/classes.rst
+-rw-r--r--   0        0        0       44 2023-04-23 19:57:27.495407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/conf.py
+-rw-r--r--   0        0        0     1434 2023-04-23 19:57:27.495407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/dedent.rst
+-rw-r--r--   0        0        0      170 2023-04-23 19:57:27.495407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/emphasize.rst
+-rw-r--r--   0        0        0        3 2023-04-23 19:57:27.495407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/empty.inc
+-rw-r--r--   0        0        0       21 2023-04-23 19:57:27.496407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/error.inc
+-rw-r--r--   0        0        0      203 2023-04-23 19:57:27.496407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/force.rst
+-rw-r--r--   0        0        0      345 2023-04-23 19:57:27.496407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/highlight.rst
+-rw-r--r--   0        0        0      267 2023-04-23 19:57:27.496407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/index.rst
+-rw-r--r--   0        0        0      349 2023-04-23 19:57:27.496407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/linenos.rst
+-rw-r--r--   0        0        0      396 2023-04-23 19:57:27.496407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/linenothreshold.rst
+-rw-r--r--   0        0        0      206 2023-04-23 19:57:27.497407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/literal-diff.inc
+-rw-r--r--   0        0        0       67 2023-04-23 19:57:27.497407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/literal-short.inc
+-rw-r--r--   0        0        0      213 2023-04-23 19:57:27.497407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/literal.inc
+-rw-r--r--   0        0        0      421 2023-04-23 19:57:27.497407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/namedblocks.rst
+-rw-r--r--   0        0        0      263 2023-04-23 19:57:27.497407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/py-decorators.inc
+-rw-r--r--   0        0        0      391 2023-04-23 19:57:27.497407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/py-decorators.rst
+-rw-r--r--   0        0        0      305 2023-04-25 10:59:46.885153 Sphinx-7.0.0rc1/tests/roots/test-directive-code/python.rst
+-rw-r--r--   0        0        0      355 2023-04-23 19:57:27.497407 Sphinx-7.0.0rc1/tests/roots/test-directive-code/target.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.497407 Sphinx-7.0.0rc1/tests/roots/test-directive-csv-table/conf.py
+-rw-r--r--   0        0        0       12 2023-04-23 19:57:27.498407 Sphinx-7.0.0rc1/tests/roots/test-directive-csv-table/example.csv
+-rw-r--r--   0        0        0       12 2023-04-23 19:57:27.498407 Sphinx-7.0.0rc1/tests/roots/test-directive-csv-table/subdir/example.csv
+-rw-r--r--   0        0        0       62 2023-04-23 19:57:27.498407 Sphinx-7.0.0rc1/tests/roots/test-directive-only/conf.py
+-rw-r--r--   0        0        0       63 2023-04-23 19:57:27.498407 Sphinx-7.0.0rc1/tests/roots/test-directive-only/index.rst
+-rw-r--r--   0        0        0     3063 2023-04-23 19:57:27.498407 Sphinx-7.0.0rc1/tests/roots/test-directive-only/only.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.498407 Sphinx-7.0.0rc1/tests/roots/test-directives-raw/conf.py
+-rw-r--r--   0        0        0      404 2023-04-23 19:57:27.499407 Sphinx-7.0.0rc1/tests/roots/test-directives-raw/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.499407 Sphinx-7.0.0rc1/tests/roots/test-docutilsconf/conf.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.499407 Sphinx-7.0.0rc1/tests/roots/test-docutilsconf/docutils.conf
+-rw-r--r--   0        0        0       89 2023-04-23 19:57:27.499407 Sphinx-7.0.0rc1/tests/roots/test-docutilsconf/index.rst
+-rw-r--r--   0        0        0       74 2023-04-23 19:57:27.499407 Sphinx-7.0.0rc1/tests/roots/test-domain-c-intersphinx/conf.py
+-rw-r--r--   0        0        0     1146 2023-04-23 19:57:27.499407 Sphinx-7.0.0rc1/tests/roots/test-domain-c-intersphinx/index.rst
+-rw-r--r--   0        0        0      121 2023-04-23 19:57:27.499407 Sphinx-7.0.0rc1/tests/roots/test-domain-c/anon-dup-decl.rst
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.500407 Sphinx-7.0.0rc1/tests/roots/test-domain-c/conf.py
+-rw-r--r--   0        0        0       70 2023-04-23 19:57:27.500407 Sphinx-7.0.0rc1/tests/roots/test-domain-c/field-role.rst
+-rw-r--r--   0        0        0      101 2023-04-23 19:57:27.500407 Sphinx-7.0.0rc1/tests/roots/test-domain-c/function_param_target.rst
+-rw-r--r--   0        0        0      785 2023-04-23 19:57:27.500407 Sphinx-7.0.0rc1/tests/roots/test-domain-c/index.rst
+-rw-r--r--   0        0        0      261 2023-04-23 19:57:27.500407 Sphinx-7.0.0rc1/tests/roots/test-domain-c/namespace.rst
+-rw-r--r--   0        0        0      163 2023-04-23 19:57:27.500407 Sphinx-7.0.0rc1/tests/roots/test-domain-c/ns_lookup.rst
+-rw-r--r--   0        0        0       74 2023-04-23 19:57:27.501407 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp-intersphinx/conf.py
+-rw-r--r--   0        0        0     2444 2023-04-23 19:57:27.501407 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp-intersphinx/index.rst
+-rw-r--r--   0        0        0       92 2023-04-23 19:57:27.501407 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/anon-dup-decl.rst
+-rw-r--r--   0        0        0      688 2023-04-23 19:57:27.501407 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/any-role.rst
+-rw-r--r--   0        0        0       27 2023-04-23 19:57:27.501407 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/backslash.rst
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.501407 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/conf.py
+-rw-r--r--   0        0        0       59 2023-04-23 19:57:27.501407 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/field-role.rst
+-rw-r--r--   0        0        0     1136 2023-04-23 19:57:27.501407 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/index.rst
+-rw-r--r--   0        0        0      133 2023-04-23 19:57:27.502406 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/lookup-key-overload.rst
+-rw-r--r--   0        0        0      437 2023-04-23 19:57:27.502406 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/multi-decl-lookup.rst
+-rw-r--r--   0        0        0     2136 2023-04-23 19:57:27.502406 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/roles-targets-ok.rst
+-rw-r--r--   0        0        0     2406 2023-04-23 19:57:27.502406 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/roles-targets-warn.rst
+-rw-r--r--   0        0        0      697 2023-04-23 19:57:27.502406 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/roles.rst
+-rw-r--r--   0        0        0       90 2023-04-23 19:57:27.502406 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/roles2.rst
+-rw-r--r--   0        0        0      383 2023-04-23 19:57:27.502406 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/semicolon.rst
+-rw-r--r--   0        0        0      203 2023-04-23 19:57:27.503407 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/warn-template-param-qualified-name.rst
+-rw-r--r--   0        0        0      249 2023-04-23 19:57:27.503407 Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/xref_consistency.rst
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.503407 Sphinx-7.0.0rc1/tests/roots/test-domain-js/conf.py
+-rw-r--r--   0        0        0       66 2023-04-23 19:57:27.503407 Sphinx-7.0.0rc1/tests/roots/test-domain-js/index.rst
+-rw-r--r--   0        0        0      527 2023-04-23 19:57:27.503407 Sphinx-7.0.0rc1/tests/roots/test-domain-js/module.rst
+-rw-r--r--   0        0        0      886 2023-04-23 19:57:27.503407 Sphinx-7.0.0rc1/tests/roots/test-domain-js/roles.rst
+-rw-r--r--   0        0        0       41 2023-04-23 19:57:27.503407 Sphinx-7.0.0rc1/tests/roots/test-domain-py-python_use_unqualified_type_names/conf.py
+-rw-r--r--   0        0        0      240 2023-04-23 19:57:27.504407 Sphinx-7.0.0rc1/tests/roots/test-domain-py-python_use_unqualified_type_names/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.504407 Sphinx-7.0.0rc1/tests/roots/test-domain-py-xref-warning/conf.py
+-rw-r--r--   0        0        0      116 2023-04-23 19:57:27.504407 Sphinx-7.0.0rc1/tests/roots/test-domain-py-xref-warning/index.rst
+-rw-r--r--   0        0        0      359 2023-04-23 19:57:27.504407 Sphinx-7.0.0rc1/tests/roots/test-domain-py/abbr.rst
+-rw-r--r--   0        0        0      174 2023-04-23 19:57:27.504407 Sphinx-7.0.0rc1/tests/roots/test-domain-py/canonical.rst
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.504407 Sphinx-7.0.0rc1/tests/roots/test-domain-py/conf.py
+-rw-r--r--   0        0        0      107 2023-04-23 19:57:27.504407 Sphinx-7.0.0rc1/tests/roots/test-domain-py/index.rst
+-rw-r--r--   0        0        0     1040 2023-04-23 19:57:27.505407 Sphinx-7.0.0rc1/tests/roots/test-domain-py/module.rst
+-rw-r--r--   0        0        0      383 2023-04-23 19:57:27.505407 Sphinx-7.0.0rc1/tests/roots/test-domain-py/module_option.rst
+-rw-r--r--   0        0        0      872 2023-04-23 19:57:27.505407 Sphinx-7.0.0rc1/tests/roots/test-domain-py/roles.rst
+-rw-r--r--   0        0        0       24 2023-04-23 19:57:27.505407 Sphinx-7.0.0rc1/tests/roots/test-double-inheriting-theme/base_themes_dir/base_theme1/theme.conf
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.505407 Sphinx-7.0.0rc1/tests/roots/test-double-inheriting-theme/base_themes_dir/base_theme2/theme.conf
+-rw-r--r--   0        0        0      127 2023-04-23 19:57:27.506407 Sphinx-7.0.0rc1/tests/roots/test-double-inheriting-theme/conf.py
+-rw-r--r--   0        0        0       87 2023-04-23 19:57:27.506407 Sphinx-7.0.0rc1/tests/roots/test-double-inheriting-theme/index.rst
+-rw-r--r--   0        0        0       40 2023-04-23 19:57:27.506407 Sphinx-7.0.0rc1/tests/roots/test-environment-record-dependencies/api.rst
+-rw-r--r--   0        0        0       99 2023-04-23 19:57:27.506407 Sphinx-7.0.0rc1/tests/roots/test-environment-record-dependencies/conf.py
+-rw-r--r--   0        0        0       38 2023-04-23 19:57:27.506407 Sphinx-7.0.0rc1/tests/roots/test-environment-record-dependencies/example_module.py
+-rw-r--r--   0        0        0       22 2023-04-23 19:57:27.506407 Sphinx-7.0.0rc1/tests/roots/test-environment-record-dependencies/index.rst
+-rw-r--r--   0        0        0       87 2023-04-23 19:57:27.507407 Sphinx-7.0.0rc1/tests/roots/test-epub-anchor-id/conf.py
+-rw-r--r--   0        0        0      191 2023-04-23 19:57:27.507407 Sphinx-7.0.0rc1/tests/roots/test-epub-anchor-id/index.rst
+-rw-r--r--   0        0        0      111 2023-04-23 19:57:27.507407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/autodoc_dummy_bar.py
+-rw-r--r--   0        0        0       94 2023-04-23 19:57:27.507407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/autodoc_dummy_module.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.507407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/bug2437/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-23 19:57:27.507407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/bug2437/autodoc_dummy_foo.py
+-rw-r--r--   0        0        0      215 2023-04-23 19:57:27.507407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/conf.py
+-rw-r--r--   0        0        0      282 2023-04-23 19:57:27.508406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/index.rst
+-rw-r--r--   0        0        0      149 2023-04-23 19:57:27.508406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/TYPE_CHECKING.py
+-rw-r--r--   0        0        0     4363 2023-04-23 19:57:27.508406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-23 19:57:27.508406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/_functions_to_import.py
+-rw-r--r--   0        0        0      428 2023-04-23 19:57:27.508406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/abstractmethods.py
+-rw-r--r--   0        0        0      150 2023-04-23 19:57:27.509407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/annotated.py
+-rw-r--r--   0        0        0      882 2023-04-23 19:57:27.509407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/autoclass_content.py
+-rw-r--r--   0        0        0      665 2023-04-23 19:57:27.509407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/autodoc_type_aliases.py
+-rw-r--r--   0        0        0      107 2023-04-23 19:57:27.509407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/bound_method.py
+-rw-r--r--   0        0        0      219 2023-04-23 19:57:27.510406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/cached_property.py
+-rw-r--r--   0        0        0      279 2023-04-23 19:57:27.510406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/callable.py
+-rw-r--r--   0        0        0       47 2023-04-23 19:57:27.510406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/canonical/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-23 19:57:27.510406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/canonical/original.py
+-rw-r--r--   0        0        0      684 2023-04-23 19:57:27.510406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/classes.py
+-rw-r--r--   0        0        0      764 2023-04-23 19:57:27.510406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/coroutine.py
+-rw-r--r--   0        0        0      245 2023-04-23 19:57:27.511406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/cython.pyx
+-rw-r--r--   0        0        0      766 2023-04-23 19:57:27.511406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/decorator.py
+-rw-r--r--   0        0        0      683 2023-04-23 19:57:27.511406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/descriptor.py
+-rw-r--r--   0        0        0      643 2023-04-23 19:57:27.511406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/docstring_signature.py
+-rw-r--r--   0        0        0      150 2023-04-23 19:57:27.511406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/empty_all.py
+-rw-r--r--   0        0        0      384 2023-04-23 19:57:27.511406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/enums.py
+-rw-r--r--   0        0        0      227 2023-04-23 19:57:27.511406 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/final.py
+-rw-r--r--   0        0        0      268 2023-04-23 19:57:27.512418 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/functions.py
+-rw-r--r--   0        0        0      278 2023-04-23 19:57:27.512418 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/generic_class.py
+-rw-r--r--   0        0        0      262 2023-04-23 19:57:27.512418 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/genericalias.py
+-rw-r--r--   0        0        0      260 2023-04-23 19:57:27.512418 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/hide_value.py
+-rw-r--r--   0        0        0       42 2023-04-23 19:57:27.512418 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/imported_members.py
+-rw-r--r--   0        0        0      458 2023-04-23 19:57:27.512418 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/inheritance.py
+-rw-r--r--   0        0        0      279 2023-04-23 19:57:27.512418 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/instance_variable.py
+-rw-r--r--   0        0        0       52 2023-04-23 19:57:27.513407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/metadata.py
+-rw-r--r--   0        0        0      422 2023-04-23 19:57:27.513407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/methods.py
+-rw-r--r--   0        0        0      155 2023-04-23 19:57:27.513407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/module.py
+-rw-r--r--   0        0        0       93 2023-04-23 19:57:27.513407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/name_conflict/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-23 19:57:27.513407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/name_conflict/foo.py
+-rw-r--r--   0        0        0      169 2023-04-23 19:57:27.513407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/name_mangling.py
+-rw-r--r--   0        0        0      894 2023-04-23 19:57:27.513407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/need_mocks.py
+-rw-r--r--   0        0        0     1345 2023-04-23 19:57:27.514407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/overload.py
+-rw-r--r--   0        0        0       59 2023-04-23 19:57:27.514407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/overload2.py
+-rw-r--r--   0        0        0      207 2023-04-23 19:57:27.514407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/partialfunction.py
+-rw-r--r--   0        0        0      420 2023-04-23 19:57:27.514407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/partialmethod.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.514407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/pep570.py
+-rw-r--r--   0        0        0      292 2023-04-23 19:57:27.514407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/pep604.py
+-rw-r--r--   0        0        0      831 2023-04-23 19:57:27.514407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/preserve_defaults.py
+-rw-r--r--   0        0        0      556 2023-04-23 19:57:27.515423 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/private.py
+-rw-r--r--   0        0        0       90 2023-04-23 19:57:27.515423 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/process_docstring.py
+-rw-r--r--   0        0        0      407 2023-04-23 19:57:27.515423 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/properties.py
+-rw-r--r--   0        0        0      705 2023-04-23 19:57:27.515423 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/singledispatch.py
+-rw-r--r--   0        0        0      628 2023-04-23 19:57:27.515423 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/singledispatchmethod.py
+-rw-r--r--   0        0        0      396 2023-04-23 19:57:27.515423 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/slots.py
+-rw-r--r--   0        0        0      168 2023-04-23 19:57:27.515423 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/sort_by_all.py
+-rw-r--r--   0        0        0      551 2023-04-23 19:57:27.516407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/typed_vars.py
+-rw-r--r--   0        0        0     2107 2023-04-23 19:57:27.516407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/typehints.py
+-rw-r--r--   0        0        0      461 2023-04-23 19:57:27.516407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/typevar.py
+-rw-r--r--   0        0        0      123 2023-04-23 19:57:27.516407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/uninitialized_attributes.py
+-rw-r--r--   0        0        0      372 2023-04-23 19:57:27.516407 Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/wrappedfunction.py
+-rw-r--r--   0        0        0       85 2023-04-23 19:57:27.516407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosectionlabel-prefix-document/conf.py
+-rw-r--r--   0        0        0      591 2023-04-23 19:57:27.516407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosectionlabel-prefix-document/index.rst
+-rw-r--r--   0        0        0       45 2023-04-23 19:57:27.517407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosectionlabel/conf.py
+-rw-r--r--   0        0        0      535 2023-04-23 19:57:27.517407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosectionlabel/index.rst
+-rw-r--r--   0        0        0      294 2023-04-23 19:57:27.517407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-filename-map/autosummary_dummy_module.py
+-rw-r--r--   0        0        0      255 2023-04-23 19:57:27.517407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-filename-map/conf.py
+-rw-r--r--   0        0        0      198 2023-04-23 19:57:27.517407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-filename-map/index.rst
+-rw-r--r--   0        0        0       47 2023-04-23 19:57:27.517407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-imported_members/autosummary_dummy_package/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-23 19:57:27.518406 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-imported_members/autosummary_dummy_package/autosummary_dummy_module.py
+-rw-r--r--   0        0        0      168 2023-04-23 19:57:27.518406 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-imported_members/conf.py
+-rw-r--r--   0        0        0      147 2023-04-23 19:57:27.518406 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-imported_members/index.rst
+-rw-r--r--   0        0        0      171 2023-04-23 19:57:27.518406 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-mock_imports/conf.py
+-rw-r--r--   0        0        0       72 2023-04-23 19:57:27.518406 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-mock_imports/foo.py
+-rw-r--r--   0        0        0      117 2023-04-23 19:57:27.518406 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-mock_imports/index.rst
+-rw-r--r--   0        0        0      241 2023-04-23 19:57:27.519407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/__init__.py
+-rw-r--r--   0        0        0      201 2023-04-23 19:57:27.519407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/autosummary_dummy_module.py
+-rw-r--r--   0        0        0      201 2023-04-23 19:57:27.519407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/extra_dummy_module.py
+-rw-r--r--   0        0        0      170 2023-04-23 19:57:27.519407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-module_all/conf.py
+-rw-r--r--   0        0        0      154 2023-04-23 19:57:27.519407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-module_all/index.rst
+-rw-r--r--   0        0        0      132 2023-04-23 19:57:27.519407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-recursive/conf.py
+-rw-r--r--   0        0        0      174 2023-04-23 19:57:27.519407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-recursive/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.520407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-recursive/package2/__init__.py
+-rw-r--r--   0        0        0      147 2023-04-23 19:57:27.520407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-recursive/package2/module.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.519407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-recursive/package/__init__.py
+-rw-r--r--   0        0        0      147 2023-04-23 19:57:27.520407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-recursive/package/module.py
+-rw-r--r--   0        0        0       63 2023-04-23 19:57:27.520407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-recursive/package/module_importfail.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.520407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-recursive/package/package/__init__.py
+-rw-r--r--   0        0        0      147 2023-04-23 19:57:27.520407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-recursive/package/package/module.py
+-rw-r--r--   0        0        0      404 2023-04-23 19:57:27.521407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-skip-member/conf.py
+-rw-r--r--   0        0        0       54 2023-04-23 19:57:27.521407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-skip-member/index.rst
+-rw-r--r--   0        0        0      264 2023-04-23 19:57:27.521407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-skip-member/target.py
+-rw-r--r--   0        0        0        6 2023-04-23 19:57:27.521407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-template/_templates/empty.rst
+-rw-r--r--   0        0        0      209 2023-04-23 19:57:27.521407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-template/conf.py
+-rw-r--r--   0        0        0       78 2023-04-23 19:57:27.521407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-template/index.rst
+-rw-r--r--   0        0        0       39 2023-04-23 19:57:27.521407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary-template/target.py
+-rw-r--r--   0        0        0       22 2023-04-23 19:57:27.522407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary/autosummary_class_module.py
+-rw-r--r--   0        0        0      232 2023-04-23 19:57:27.522407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary/autosummary_dummy_inherited_module.py
+-rw-r--r--   0        0        0      932 2023-04-23 19:57:27.522407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary/autosummary_dummy_module.py
+-rw-r--r--   0        0        0       63 2023-04-23 19:57:27.522407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary/autosummary_importfail.py
+-rw-r--r--   0        0        0      190 2023-04-23 19:57:27.522407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary/conf.py
+-rw-r--r--   0        0        0      499 2023-04-23 19:57:27.522407 Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary/index.rst
+-rw-r--r--   0        0        0      242 2023-04-23 19:57:27.523407 Sphinx-7.0.0rc1/tests/roots/test-ext-coverage/conf.py
+-rw-r--r--   0        0        0      254 2023-04-23 19:57:27.523407 Sphinx-7.0.0rc1/tests/roots/test-ext-coverage/coverage_ignored.py
+-rw-r--r--   0        0        0      254 2023-04-23 19:57:27.523407 Sphinx-7.0.0rc1/tests/roots/test-ext-coverage/coverage_not_ignored.py
+-rw-r--r--   0        0        0       98 2023-04-23 19:57:27.523407 Sphinx-7.0.0rc1/tests/roots/test-ext-coverage/index.rst
+-rw-r--r--   0        0        0      371 2023-04-23 19:57:27.523407 Sphinx-7.0.0rc1/tests/roots/test-ext-doctest-skipif/conf.py
+-rw-r--r--   0        0        0     2052 2023-04-23 19:57:27.523407 Sphinx-7.0.0rc1/tests/roots/test-ext-doctest-skipif/skipif.txt
+-rw-r--r--   0        0        0      205 2023-04-23 19:57:27.523407 Sphinx-7.0.0rc1/tests/roots/test-ext-doctest-with-autodoc/conf.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.524407 Sphinx-7.0.0rc1/tests/roots/test-ext-doctest-with-autodoc/dir/__init__.py
+-rw-r--r--   0        0        0       28 2023-04-23 19:57:27.524407 Sphinx-7.0.0rc1/tests/roots/test-ext-doctest-with-autodoc/dir/bar.py
+-rw-r--r--   0        0        0       60 2023-04-23 19:57:27.524407 Sphinx-7.0.0rc1/tests/roots/test-ext-doctest-with-autodoc/dir/inner.rst
+-rw-r--r--   0        0        0       25 2023-04-23 19:57:27.524407 Sphinx-7.0.0rc1/tests/roots/test-ext-doctest-with-autodoc/foo.py
+-rw-r--r--   0        0        0       52 2023-04-23 19:57:27.524407 Sphinx-7.0.0rc1/tests/roots/test-ext-doctest-with-autodoc/index.rst
+-rw-r--r--   0        0        0      148 2023-04-23 19:57:27.524407 Sphinx-7.0.0rc1/tests/roots/test-ext-doctest/conf.py
+-rw-r--r--   0        0        0     2147 2023-04-23 19:57:27.525407 Sphinx-7.0.0rc1/tests/roots/test-ext-doctest/doctest.txt
+-rw-r--r--   0        0        0      190 2023-04-23 19:57:27.525407 Sphinx-7.0.0rc1/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/conf.py
+-rw-r--r--   0        0        0      555 2023-04-23 19:57:27.525407 Sphinx-7.0.0rc1/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/index.rst
+-rw-r--r--   0        0        0      161 2023-04-23 19:57:27.525407 Sphinx-7.0.0rc1/tests/roots/test-ext-extlinks-hardcoded-urls/conf.py
+-rw-r--r--   0        0        0      703 2023-04-23 19:57:27.525407 Sphinx-7.0.0rc1/tests/roots/test-ext-extlinks-hardcoded-urls/index.rst
+-rw-r--r--   0        0        0       40 2023-04-23 19:57:27.525407 Sphinx-7.0.0rc1/tests/roots/test-ext-githubpages/conf.py
+-rw-r--r--   0        0        0       25 2023-04-23 19:57:27.525407 Sphinx-7.0.0rc1/tests/roots/test-ext-githubpages/index.rst
+-rw-r--r--   0        0        0       67 2023-04-23 19:57:27.526407 Sphinx-7.0.0rc1/tests/roots/test-ext-graphviz/conf.py
+-rw-r--r--   0        0        0       25 2023-04-23 19:57:27.526407 Sphinx-7.0.0rc1/tests/roots/test-ext-graphviz/graph.dot
+-rw-r--r--   0        0        0       25 2023-04-23 19:57:27.526407 Sphinx-7.0.0rc1/tests/roots/test-ext-graphviz/graph.xx.dot
+-rw-r--r--   0        0        0      389 2023-04-23 19:57:27.526407 Sphinx-7.0.0rc1/tests/roots/test-ext-graphviz/index.rst
+-rw-r--r--   0        0        0      256 2023-04-23 19:57:27.526407 Sphinx-7.0.0rc1/tests/roots/test-ext-ifconfig/conf.py
+-rw-r--r--   0        0        0      274 2023-04-23 19:57:27.526407 Sphinx-7.0.0rc1/tests/roots/test-ext-ifconfig/index.rst
+-rw-r--r--   0        0        0       41 2023-04-23 19:57:27.527407 Sphinx-7.0.0rc1/tests/roots/test-ext-imgconverter/conf.py
+-rw-r--r--   0        0        0   141783 2023-04-23 19:57:27.528407 Sphinx-7.0.0rc1/tests/roots/test-ext-imgconverter/img.pdf
+-rw-r--r--   0        0        0       86 2023-04-23 19:57:27.528407 Sphinx-7.0.0rc1/tests/roots/test-ext-imgconverter/index.rst
+-rw-r--r--   0        0        0      243 2023-04-23 19:57:27.528407 Sphinx-7.0.0rc1/tests/roots/test-ext-imgconverter/svgimg.svg
+-rw-r--r--   0        0        0      106 2023-04-23 19:57:27.528407 Sphinx-7.0.0rc1/tests/roots/test-ext-imgmockconverter/1/svgimg.svg
+-rw-r--r--   0        0        0      243 2023-04-23 19:57:27.528407 Sphinx-7.0.0rc1/tests/roots/test-ext-imgmockconverter/2/svgimg.svg
+-rw-r--r--   0        0        0       97 2023-04-23 19:57:27.529407 Sphinx-7.0.0rc1/tests/roots/test-ext-imgmockconverter/conf.py
+-rw-r--r--   0        0        0       98 2023-04-23 19:57:27.529407 Sphinx-7.0.0rc1/tests/roots/test-ext-imgmockconverter/index.rst
+-rw-r--r--   0        0        0      881 2023-04-23 19:57:27.529407 Sphinx-7.0.0rc1/tests/roots/test-ext-imgmockconverter/mocksvgconverter.py
+-rw-r--r--   0        0        0      112 2023-04-23 19:57:27.529407 Sphinx-7.0.0rc1/tests/roots/test-ext-inheritance_diagram/conf.py
+-rw-r--r--   0        0        0       13 2023-04-23 19:57:27.529407 Sphinx-7.0.0rc1/tests/roots/test-ext-inheritance_diagram/example/__init__.py
+-rw-r--r--   0        0        0       46 2023-04-23 19:57:27.529407 Sphinx-7.0.0rc1/tests/roots/test-ext-inheritance_diagram/example/sphinx.py
+-rw-r--r--   0        0        0      215 2023-04-23 19:57:27.529407 Sphinx-7.0.0rc1/tests/roots/test-ext-inheritance_diagram/index.rst
+-rw-r--r--   0        0        0      101 2023-04-23 19:57:27.530407 Sphinx-7.0.0rc1/tests/roots/test-ext-inheritance_diagram/test.py
+-rw-r--r--   0        0        0       40 2023-04-23 19:57:27.530407 Sphinx-7.0.0rc1/tests/roots/test-ext-intersphinx-cppdomain/conf.py
+-rw-r--r--   0        0        0      150 2023-04-23 19:57:27.530407 Sphinx-7.0.0rc1/tests/roots/test-ext-intersphinx-cppdomain/index.rst
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.530407 Sphinx-7.0.0rc1/tests/roots/test-ext-intersphinx-role/conf.py
+-rw-r--r--   0        0        0     1211 2023-04-23 19:57:27.530407 Sphinx-7.0.0rc1/tests/roots/test-ext-intersphinx-role/index.rst
+-rw-r--r--   0        0        0      488 2023-04-23 19:57:27.530407 Sphinx-7.0.0rc1/tests/roots/test-ext-math-compat/conf.py
+-rw-r--r--   0        0        0      199 2023-04-23 19:57:27.531407 Sphinx-7.0.0rc1/tests/roots/test-ext-math-compat/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.531407 Sphinx-7.0.0rc1/tests/roots/test-ext-math-simple/conf.py
+-rw-r--r--   0        0        0       43 2023-04-23 19:57:27.531407 Sphinx-7.0.0rc1/tests/roots/test-ext-math-simple/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.531407 Sphinx-7.0.0rc1/tests/roots/test-ext-math/conf.py
+-rw-r--r--   0        0        0      239 2023-04-23 19:57:27.531407 Sphinx-7.0.0rc1/tests/roots/test-ext-math/index.rst
+-rw-r--r--   0        0        0      396 2023-04-23 19:57:27.531407 Sphinx-7.0.0rc1/tests/roots/test-ext-math/math.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.531407 Sphinx-7.0.0rc1/tests/roots/test-ext-math/nomath.rst
+-rw-r--r--   0        0        0      128 2023-04-23 19:57:27.531407 Sphinx-7.0.0rc1/tests/roots/test-ext-math/page.rst
+-rw-r--r--   0        0        0      100 2023-04-23 19:57:27.532407 Sphinx-7.0.0rc1/tests/roots/test-ext-napoleon/conf.py
+-rw-r--r--   0        0        0       64 2023-04-23 19:57:27.532407 Sphinx-7.0.0rc1/tests/roots/test-ext-napoleon/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.532407 Sphinx-7.0.0rc1/tests/roots/test-ext-napoleon/mypackage/__init__.py
+-rw-r--r--   0        0        0      194 2023-04-23 19:57:27.532407 Sphinx-7.0.0rc1/tests/roots/test-ext-napoleon/mypackage/typehints.py
+-rw-r--r--   0        0        0       70 2023-04-23 19:57:27.532407 Sphinx-7.0.0rc1/tests/roots/test-ext-napoleon/typehints.rst
+-rw-r--r--   0        0        0       31 2023-04-23 19:57:27.532407 Sphinx-7.0.0rc1/tests/roots/test-ext-todo/bar.rst
+-rw-r--r--   0        0        0       33 2023-04-23 19:57:27.533407 Sphinx-7.0.0rc1/tests/roots/test-ext-todo/conf.py
+-rw-r--r--   0        0        0      125 2023-04-23 19:57:27.533407 Sphinx-7.0.0rc1/tests/roots/test-ext-todo/foo.rst
+-rw-r--r--   0        0        0      109 2023-04-23 19:57:27.533407 Sphinx-7.0.0rc1/tests/roots/test-ext-todo/index.rst
+-rw-r--r--   0        0        0      108 2023-04-23 19:57:27.533407 Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode-find/conf.py
+-rw-r--r--   0        0        0      636 2023-04-23 19:57:27.533407 Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode-find/index.rst
+-rw-r--r--   0        0        0       37 2023-04-23 19:57:27.533407 Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode-find/not_a_package/__init__.py
+-rw-r--r--   0        0        0      371 2023-04-23 19:57:27.533407 Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode-find/not_a_package/submodule.py
+-rw-r--r--   0        0        0      745 2023-04-23 19:57:27.534407 Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode/conf.py
+-rw-r--r--   0        0        0      550 2023-04-23 19:57:27.534407 Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode/index.rst
+-rw-r--r--   0        0        0     3111 2023-04-23 19:57:27.534407 Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode/objects.rst
+-rw-r--r--   0        0        0       64 2023-04-23 19:57:27.534407 Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode/spam/__init__.py
+-rw-r--r--   0        0        0      308 2023-04-23 19:57:27.534407 Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode/spam/mod1.py
+-rw-r--r--   0        0        0      188 2023-04-23 19:57:27.534407 Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode/spam/mod2.py
+-rw-r--r--   0        0        0       52 2023-04-23 19:57:27.534407 Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode/spam/mod3.py
+-rw-r--r--   0        0        0       63 2023-04-23 19:57:27.535407 Sphinx-7.0.0rc1/tests/roots/test-extensions/conf.py
+-rw-r--r--   0        0        0       70 2023-04-23 19:57:27.535407 Sphinx-7.0.0rc1/tests/roots/test-extensions/read_parallel.py
+-rw-r--r--   0        0        0       71 2023-04-23 19:57:27.535407 Sphinx-7.0.0rc1/tests/roots/test-extensions/read_serial.py
+-rw-r--r--   0        0        0       72 2023-04-23 19:57:27.535407 Sphinx-7.0.0rc1/tests/roots/test-extensions/write_parallel.py
+-rw-r--r--   0        0        0       72 2023-04-23 19:57:27.535407 Sphinx-7.0.0rc1/tests/roots/test-extensions/write_serial.py
+-rw-r--r--   0        0        0       70 2023-04-23 19:57:27.535407 Sphinx-7.0.0rc1/tests/roots/test-footnotes/bar.rst
+-rw-r--r--   0        0        0       70 2023-04-23 19:57:27.536407 Sphinx-7.0.0rc1/tests/roots/test-footnotes/baz.rst
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.536407 Sphinx-7.0.0rc1/tests/roots/test-footnotes/conf.py
+-rw-r--r--   0        0        0     3385 2023-04-23 19:57:27.536407 Sphinx-7.0.0rc1/tests/roots/test-footnotes/index.rst
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.536407 Sphinx-7.0.0rc1/tests/roots/test-footnotes/rimg.png
+-rw-r--r--   0        0        0      143 2023-04-23 19:57:27.536407 Sphinx-7.0.0rc1/tests/roots/test-gettext-template/_templates/template1.html
+-rw-r--r--   0        0        0      143 2023-04-23 19:57:27.536407 Sphinx-7.0.0rc1/tests/roots/test-gettext-template/_templates/template2.html
+-rw-r--r--   0        0        0       32 2023-04-23 19:57:27.536407 Sphinx-7.0.0rc1/tests/roots/test-gettext-template/conf.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.536407 Sphinx-7.0.0rc1/tests/roots/test-gettext-template/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.537407 Sphinx-7.0.0rc1/tests/roots/test-glossary/conf.py
+-rw-r--r--   0        0        0      260 2023-04-23 19:57:27.537407 Sphinx-7.0.0rc1/tests/roots/test-glossary/index.rst
+-rw-r--r--   0        0        0      103 2023-04-23 19:57:27.537407 Sphinx-7.0.0rc1/tests/roots/test-highlight_options/conf.py
+-rw-r--r--   0        0        0      166 2023-04-23 19:57:27.537407 Sphinx-7.0.0rc1/tests/roots/test-highlight_options/index.rst
+-rw-r--r--   0        0        0      468 2023-04-23 19:57:27.537407 Sphinx-7.0.0rc1/tests/roots/test-html_assets/conf.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.537407 Sphinx-7.0.0rc1/tests/roots/test-html_assets/extra/.htaccess
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.537407 Sphinx-7.0.0rc1/tests/roots/test-html_assets/extra/.htpasswd
+-rw-r--r--   0        0        0       28 2023-04-23 19:57:27.538407 Sphinx-7.0.0rc1/tests/roots/test-html_assets/extra/API.html_t
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.538679 Sphinx-7.0.0rc1/tests/roots/test-html_assets/extra/css/style.css
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.538679 Sphinx-7.0.0rc1/tests/roots/test-html_assets/extra/index.rst
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.538679 Sphinx-7.0.0rc1/tests/roots/test-html_assets/extra/rimg.png
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.538679 Sphinx-7.0.0rc1/tests/roots/test-html_assets/extra/subdir/.htaccess
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.538679 Sphinx-7.0.0rc1/tests/roots/test-html_assets/extra/subdir/.htpasswd
+-rw-r--r--   0        0        0       65 2023-04-23 19:57:27.538679 Sphinx-7.0.0rc1/tests/roots/test-html_assets/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.538679 Sphinx-7.0.0rc1/tests/roots/test-html_assets/static/.htaccess
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.538679 Sphinx-7.0.0rc1/tests/roots/test-html_assets/static/.htpasswd
+-rw-r--r--   0        0        0       28 2023-04-23 19:57:27.539686 Sphinx-7.0.0rc1/tests/roots/test-html_assets/static/API.html_t
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.539686 Sphinx-7.0.0rc1/tests/roots/test-html_assets/static/css/style.css
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.539686 Sphinx-7.0.0rc1/tests/roots/test-html_assets/static/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.539686 Sphinx-7.0.0rc1/tests/roots/test-html_assets/static/js/custom.js
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.539686 Sphinx-7.0.0rc1/tests/roots/test-html_assets/static/rimg.png
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.539686 Sphinx-7.0.0rc1/tests/roots/test-html_assets/static/subdir/.htaccess
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.540686 Sphinx-7.0.0rc1/tests/roots/test-html_assets/static/subdir/.htpasswd
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.540686 Sphinx-7.0.0rc1/tests/roots/test-html_assets/subdir/_build/index.html
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.540686 Sphinx-7.0.0rc1/tests/roots/test-html_assets/subdir/background.png
+-rw-r--r--   0        0        0       53 2023-04-23 19:57:27.540686 Sphinx-7.0.0rc1/tests/roots/test-html_entity/conf.py
+-rw-r--r--   0        0        0      561 2023-04-23 19:57:27.540686 Sphinx-7.0.0rc1/tests/roots/test-html_entity/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.541685 Sphinx-7.0.0rc1/tests/roots/test-html_scaled_image_link/conf.py
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.541685 Sphinx-7.0.0rc1/tests/roots/test-html_scaled_image_link/img.png
+-rw-r--r--   0        0        0      172 2023-04-23 19:57:27.541685 Sphinx-7.0.0rc1/tests/roots/test-html_scaled_image_link/index.rst
+-rw-r--r--   0        0        0       36 2023-04-23 19:57:27.541685 Sphinx-7.0.0rc1/tests/roots/test-html_signaturereturn_icon/conf.py
+-rw-r--r--   0        0        0      108 2023-04-23 19:57:27.541685 Sphinx-7.0.0rc1/tests/roots/test-html_signaturereturn_icon/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.541685 Sphinx-7.0.0rc1/tests/roots/test-html_style/_static/default.css
+-rw-r--r--   0        0        0       58 2023-04-23 19:57:27.542686 Sphinx-7.0.0rc1/tests/roots/test-html_style/conf.py
+-rw-r--r--   0        0        0       22 2023-04-23 19:57:27.542686 Sphinx-7.0.0rc1/tests/roots/test-html_style/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.542686 Sphinx-7.0.0rc1/tests/roots/test-image-escape/conf.py
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.542686 Sphinx-7.0.0rc1/tests/roots/test-image-escape/img_#1.png
+-rw-r--r--   0        0        0      145 2023-04-23 19:57:27.542686 Sphinx-7.0.0rc1/tests/roots/test-image-escape/index.rst
+-rw-r--r--   0        0        0      161 2023-04-23 19:57:27.542686 Sphinx-7.0.0rc1/tests/roots/test-image-in-parsed-literal/conf.py
+-rw-r--r--   0        0        0      113 2023-04-23 19:57:27.542686 Sphinx-7.0.0rc1/tests/roots/test-image-in-parsed-literal/index.rst
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.543686 Sphinx-7.0.0rc1/tests/roots/test-image-in-parsed-literal/pic.png
+-rw-r--r--   0        0        0      143 2023-04-23 19:57:27.543886 Sphinx-7.0.0rc1/tests/roots/test-image-in-section/conf.py
+-rw-r--r--   0        0        0      287 2023-04-23 19:57:27.543886 Sphinx-7.0.0rc1/tests/roots/test-image-in-section/index.rst
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.543886 Sphinx-7.0.0rc1/tests/roots/test-image-in-section/pic.png
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.543886 Sphinx-7.0.0rc1/tests/roots/test-images/conf.py
+-rw-r--r--   0        0        0    24976 2023-04-23 19:57:27.543886 Sphinx-7.0.0rc1/tests/roots/test-images/img.gif
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.543886 Sphinx-7.0.0rc1/tests/roots/test-images/img.ja.png
+-rw-r--r--   0        0        0   141783 2023-04-23 19:57:27.544893 Sphinx-7.0.0rc1/tests/roots/test-images/img.pdf
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.545892 Sphinx-7.0.0rc1/tests/roots/test-images/img.png
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.545892 Sphinx-7.0.0rc1/tests/roots/test-images/img.zh.png
+-rw-r--r--   0        0        0      466 2023-04-23 19:57:27.545892 Sphinx-7.0.0rc1/tests/roots/test-images/index.rst
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.545892 Sphinx-7.0.0rc1/tests/roots/test-images/rimg.png
+-rw-r--r--   0        0        0      218 2023-04-23 19:57:27.545892 Sphinx-7.0.0rc1/tests/roots/test-images/rimg.png.xx
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.545892 Sphinx-7.0.0rc1/tests/roots/test-images/rimg.xx.png
+-rw-r--r--   0        0        0      128 2023-04-23 19:57:27.546893 Sphinx-7.0.0rc1/tests/roots/test-images/subdir/index.rst
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.546893 Sphinx-7.0.0rc1/tests/roots/test-images/subdir/rimg.png
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.546893 Sphinx-7.0.0rc1/tests/roots/test-images/subdir/rimg.xx.png
+-rw-r--r--   0        0        0   141783 2023-04-23 19:57:27.547893 Sphinx-7.0.0rc1/tests/roots/test-images/subdir/svgimg.pdf
+-rw-r--r--   0        0        0      243 2023-04-23 19:57:27.547893 Sphinx-7.0.0rc1/tests/roots/test-images/subdir/svgimg.svg
+-rw-r--r--   0        0        0      243 2023-04-23 19:57:27.547893 Sphinx-7.0.0rc1/tests/roots/test-images/subdir/svgimg.xx.svg
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.547893 Sphinx-7.0.0rc1/tests/roots/test-images/testimäge.png
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.548892 Sphinx-7.0.0rc1/tests/roots/test-index_on_title/conf.py
+-rw-r--r--   0        0        0      117 2023-04-23 19:57:27.548892 Sphinx-7.0.0rc1/tests/roots/test-index_on_title/contents.rst
+-rw-r--r--   0        0        0       70 2023-04-23 19:57:27.548892 Sphinx-7.0.0rc1/tests/roots/test-inheritance/basic_diagram.rst
+-rw-r--r--   0        0        0      135 2023-04-23 19:57:27.548892 Sphinx-7.0.0rc1/tests/roots/test-inheritance/conf.py
+-rw-r--r--   0        0        0      166 2023-04-23 19:57:27.548892 Sphinx-7.0.0rc1/tests/roots/test-inheritance/diagram_module_w_2_top_classes.rst
+-rw-r--r--   0        0        0      125 2023-04-23 19:57:27.548892 Sphinx-7.0.0rc1/tests/roots/test-inheritance/diagram_w_1_top_class.rst
+-rw-r--r--   0        0        0      179 2023-04-23 19:57:27.548892 Sphinx-7.0.0rc1/tests/roots/test-inheritance/diagram_w_2_top_classes.rst
+-rw-r--r--   0        0        0      104 2023-04-23 19:57:27.549892 Sphinx-7.0.0rc1/tests/roots/test-inheritance/diagram_w_nested_classes.rst
+-rw-r--r--   0        0        0      118 2023-04-23 19:57:27.549892 Sphinx-7.0.0rc1/tests/roots/test-inheritance/diagram_w_parts.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.549892 Sphinx-7.0.0rc1/tests/roots/test-inheritance/dummy/__init__.py
+-rw-r--r--   0        0        0      267 2023-04-23 19:57:27.549892 Sphinx-7.0.0rc1/tests/roots/test-inheritance/dummy/test.py
+-rw-r--r--   0        0        0       95 2023-04-23 19:57:27.549892 Sphinx-7.0.0rc1/tests/roots/test-inheritance/dummy/test_nested.py
+-rw-r--r--   0        0        0       31 2023-04-23 19:57:27.549892 Sphinx-7.0.0rc1/tests/roots/test-inheritance/index.rst
+-rw-r--r--   0        0        0      216 2023-04-23 19:57:27.549892 Sphinx-7.0.0rc1/tests/roots/test-intl/_templates/contents.html
+-rw-r--r--   0        0        0      599 2023-04-23 19:57:27.550892 Sphinx-7.0.0rc1/tests/roots/test-intl/admonitions.txt
+-rw-r--r--   0        0        0       74 2023-04-23 19:57:27.550892 Sphinx-7.0.0rc1/tests/roots/test-intl/bom.txt
+-rw-r--r--   0        0        0      262 2023-04-23 19:57:27.550892 Sphinx-7.0.0rc1/tests/roots/test-intl/conf.py
+-rw-r--r--   0        0        0      342 2023-04-23 19:57:27.550892 Sphinx-7.0.0rc1/tests/roots/test-intl/definition_terms.txt
+-rw-r--r--   0        0        0      704 2023-04-23 19:57:27.550892 Sphinx-7.0.0rc1/tests/roots/test-intl/docfields.txt
+-rw-r--r--   0        0        0      858 2023-04-23 19:57:27.550892 Sphinx-7.0.0rc1/tests/roots/test-intl/external_links.txt
+-rw-r--r--   0        0        0      747 2023-04-23 19:57:27.550892 Sphinx-7.0.0rc1/tests/roots/test-intl/figure.txt
+-rw-r--r--   0        0        0      407 2023-04-23 19:57:27.550892 Sphinx-7.0.0rc1/tests/roots/test-intl/footnote.txt
+-rw-r--r--   0        0        0      378 2023-04-23 19:57:27.551892 Sphinx-7.0.0rc1/tests/roots/test-intl/glossary_terms.txt
+-rw-r--r--   0        0        0      151 2023-04-23 19:57:27.551892 Sphinx-7.0.0rc1/tests/roots/test-intl/glossary_terms_inconsistency.txt
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.551892 Sphinx-7.0.0rc1/tests/roots/test-intl/i18n.png
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.551892 Sphinx-7.0.0rc1/tests/roots/test-intl/img.png
+-rw-r--r--   0        0        0      539 2023-04-23 19:57:27.551892 Sphinx-7.0.0rc1/tests/roots/test-intl/index.txt
+-rw-r--r--   0        0        0      530 2023-04-23 19:57:27.551892 Sphinx-7.0.0rc1/tests/roots/test-intl/index_entries.txt
+-rw-r--r--   0        0        0     1832 2023-04-23 19:57:27.552893 Sphinx-7.0.0rc1/tests/roots/test-intl/label_target.txt
+-rw-r--r--   0        0        0      943 2023-04-23 19:57:27.552893 Sphinx-7.0.0rc1/tests/roots/test-intl/literalblock.txt
+-rw-r--r--   0        0        0      278 2023-04-23 19:57:27.552893 Sphinx-7.0.0rc1/tests/roots/test-intl/noqa.txt
+-rw-r--r--   0        0        0      128 2023-04-23 19:57:27.552893 Sphinx-7.0.0rc1/tests/roots/test-intl/only.txt
+-rw-r--r--   0        0        0       78 2023-04-23 19:57:27.552893 Sphinx-7.0.0rc1/tests/roots/test-intl/raw.txt
+-rw-r--r--   0        0        0     1094 2023-04-23 19:57:27.552893 Sphinx-7.0.0rc1/tests/roots/test-intl/refs.txt
+-rw-r--r--   0        0        0      291 2023-04-23 19:57:27.552893 Sphinx-7.0.0rc1/tests/roots/test-intl/refs_inconsistency.txt
+-rw-r--r--   0        0        0      252 2023-04-23 19:57:27.552893 Sphinx-7.0.0rc1/tests/roots/test-intl/refs_python_domain.txt
+-rw-r--r--   0        0        0      738 2023-04-23 19:57:27.552893 Sphinx-7.0.0rc1/tests/roots/test-intl/role_xref.txt
+-rw-r--r--   0        0        0      152 2023-04-23 19:57:27.553892 Sphinx-7.0.0rc1/tests/roots/test-intl/rubric.txt
+-rw-r--r--   0        0        0       97 2023-04-23 19:57:27.553892 Sphinx-7.0.0rc1/tests/roots/test-intl/section.txt
+-rw-r--r--   0        0        0      210 2023-04-23 19:57:27.554190 Sphinx-7.0.0rc1/tests/roots/test-intl/seealso.txt
+-rw-r--r--   0        0        0       32 2023-04-23 19:57:27.554190 Sphinx-7.0.0rc1/tests/roots/test-intl/subdir/index.txt
+-rw-r--r--   0        0        0      263 2023-04-23 19:57:27.554190 Sphinx-7.0.0rc1/tests/roots/test-intl/table.txt
+-rw-r--r--   0        0        0      139 2023-04-23 19:57:27.554190 Sphinx-7.0.0rc1/tests/roots/test-intl/toctree.txt
+-rw-r--r--   0        0        0      135 2023-04-23 19:57:27.554190 Sphinx-7.0.0rc1/tests/roots/test-intl/topic.txt
+-rw-r--r--   0        0        0      337 2023-04-23 19:57:27.554190 Sphinx-7.0.0rc1/tests/roots/test-intl/versionchange.txt
+-rw-r--r--   0        0        0       79 2023-04-23 19:57:27.554190 Sphinx-7.0.0rc1/tests/roots/test-intl/warnings.txt
+-rw-r--r--   0        0        0     1513 2023-04-23 19:57:27.555196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/admonitions.po
+-rw-r--r--   0        0        0      264 2023-04-23 19:57:27.555196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/bom.po
+-rw-r--r--   0        0        0     1198 2023-04-25 10:59:46.885153 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/definition_terms.po
+-rw-r--r--   0        0        0     1086 2023-04-23 19:57:27.555196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/docfields.po
+-rw-r--r--   0        0        0     1691 2023-04-23 19:57:27.555196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/external_links.po
+-rw-r--r--   0        0        0     1307 2023-04-23 19:57:27.556196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/figure.po
+-rw-r--r--   0        0        0     1228 2023-04-23 19:57:27.556196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/footnote.po
+-rw-r--r--   0        0        0     1327 2023-04-23 19:57:27.556196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms.po
+-rw-r--r--   0        0        0      754 2023-04-25 10:59:46.885153 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms_inconsistency.po
+-rw-r--r--   0        0        0      773 2023-04-23 19:57:27.556196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/index.po
+-rw-r--r--   0        0        0     1318 2023-04-23 19:57:27.556196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/index_entries.po
+-rw-r--r--   0        0        0     2159 2023-04-23 19:57:27.557196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/label_target.po
+-rw-r--r--   0        0        0     2211 2023-04-23 19:57:27.557196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/literalblock.po
+-rw-r--r--   0        0        0     1380 2023-04-23 19:57:27.557196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/noqa.po
+-rw-r--r--   0        0        0      723 2023-04-23 19:57:27.557196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/only.po
+-rw-r--r--   0        0        0      644 2023-04-23 19:57:27.557196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/raw.po
+-rw-r--r--   0        0        0     2771 2023-04-23 19:57:27.557196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/refs.po
+-rw-r--r--   0        0        0     1045 2023-04-23 19:57:27.557196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/refs_inconsistency.po
+-rw-r--r--   0        0        0      675 2023-04-23 19:57:27.557196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/refs_python_domain.po
+-rw-r--r--   0        0        0     1707 2023-04-23 19:57:27.558196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/role_xref.po
+-rw-r--r--   0        0        0      744 2023-04-25 10:59:46.885153 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/rubric.po
+-rw-r--r--   0        0        0      706 2023-04-23 19:57:27.558196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/section.po
+-rw-r--r--   0        0        0      792 2023-04-23 19:57:27.558196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/seealso.po
+-rw-r--r--   0        0        0      621 2023-04-23 19:57:27.558196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0      992 2023-04-23 19:57:27.558196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/table.po
+-rw-r--r--   0        0        0      767 2023-04-23 19:57:27.558196 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/toctree.po
+-rw-r--r--   0        0        0      750 2023-04-23 19:57:27.559195 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/topic.po
+-rw-r--r--   0        0        0     1070 2023-04-23 19:57:27.559195 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/versionchange.po
+-rw-r--r--   0        0        0      710 2023-04-23 19:57:27.559195 Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/warnings.po
+-rw-r--r--   0        0        0       21 2023-04-23 19:57:27.559195 Sphinx-7.0.0rc1/tests/roots/test-keep_warnings/conf.py
+-rw-r--r--   0        0        0       20 2023-04-23 19:57:27.559195 Sphinx-7.0.0rc1/tests/roots/test-keep_warnings/index.rst
+-rw-r--r--   0        0        0       13 2023-04-23 19:57:27.559195 Sphinx-7.0.0rc1/tests/roots/test-latex-babel/bar.rst
+-rw-r--r--   0        0        0       98 2023-04-23 19:57:27.559195 Sphinx-7.0.0rc1/tests/roots/test-latex-babel/conf.py
+-rw-r--r--   0        0        0       13 2023-04-23 19:57:27.560196 Sphinx-7.0.0rc1/tests/roots/test-latex-babel/foo.rst
+-rw-r--r--   0        0        0       87 2023-04-23 19:57:27.560196 Sphinx-7.0.0rc1/tests/roots/test-latex-babel/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.560196 Sphinx-7.0.0rc1/tests/roots/test-latex-container/conf.py
+-rw-r--r--   0        0        0       35 2023-04-23 19:57:27.560196 Sphinx-7.0.0rc1/tests/roots/test-latex-container/index.rst
+-rw-r--r--   0        0        0       59 2023-04-23 19:57:27.560196 Sphinx-7.0.0rc1/tests/roots/test-latex-equations/conf.py
+-rw-r--r--   0        0        0      256 2023-04-23 19:57:27.560196 Sphinx-7.0.0rc1/tests/roots/test-latex-equations/equations.rst
+-rw-r--r--   0        0        0      452 2023-04-23 19:57:27.560196 Sphinx-7.0.0rc1/tests/roots/test-latex-equations/expects/latex-equations.tex
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.561196 Sphinx-7.0.0rc1/tests/roots/test-latex-figure-in-admonition/conf.py
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.561196 Sphinx-7.0.0rc1/tests/roots/test-latex-figure-in-admonition/img.png
+-rw-r--r--   0        0        0      132 2023-04-23 19:57:27.561196 Sphinx-7.0.0rc1/tests/roots/test-latex-figure-in-admonition/index.rst
+-rw-r--r--   0        0        0     1573 2023-04-23 19:57:27.561196 Sphinx-7.0.0rc1/tests/roots/test-latex-includegraphics/conf.py
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.561196 Sphinx-7.0.0rc1/tests/roots/test-latex-includegraphics/img.png
+-rw-r--r--   0        0        0      834 2023-04-23 19:57:27.561196 Sphinx-7.0.0rc1/tests/roots/test-latex-includegraphics/index.rst
+-rw-r--r--   0        0        0    34213 2023-04-23 19:57:27.562196 Sphinx-7.0.0rc1/tests/roots/test-latex-includegraphics/sphinx.png
+-rw-r--r--   0        0        0    38192 2023-04-23 19:57:27.562196 Sphinx-7.0.0rc1/tests/roots/test-latex-includegraphics/tall.png
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.562196 Sphinx-7.0.0rc1/tests/roots/test-latex-index/conf.py
+-rw-r--r--   0        0        0      215 2023-04-23 19:57:27.562196 Sphinx-7.0.0rc1/tests/roots/test-latex-index/index.rst
+-rw-r--r--   0        0        0       17 2023-04-23 19:57:27.563195 Sphinx-7.0.0rc1/tests/roots/test-latex-labels-before-module/automodule1.py
+-rw-r--r--   0        0        0       17 2023-04-23 19:57:27.563195 Sphinx-7.0.0rc1/tests/roots/test-latex-labels-before-module/automodule2a.py
+-rw-r--r--   0        0        0       17 2023-04-23 19:57:27.563195 Sphinx-7.0.0rc1/tests/roots/test-latex-labels-before-module/automodule2b.py
+-rw-r--r--   0        0        0       17 2023-04-23 19:57:27.564197 Sphinx-7.0.0rc1/tests/roots/test-latex-labels-before-module/automodule3.py
+-rw-r--r--   0        0        0      117 2023-04-23 19:57:27.564197 Sphinx-7.0.0rc1/tests/roots/test-latex-labels-before-module/conf.py
+-rw-r--r--   0        0        0      464 2023-04-23 19:57:27.564197 Sphinx-7.0.0rc1/tests/roots/test-latex-labels-before-module/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.564197 Sphinx-7.0.0rc1/tests/roots/test-latex-labels/conf.py
+-rw-r--r--   0        0        0      771 2023-04-23 19:57:27.565196 Sphinx-7.0.0rc1/tests/roots/test-latex-labels/index.rst
+-rw-r--r--   0        0        0       18 2023-04-23 19:57:27.565196 Sphinx-7.0.0rc1/tests/roots/test-latex-labels/otherdoc.rst
+-rw-r--r--   0        0        0      250 2023-04-23 19:57:27.565196 Sphinx-7.0.0rc1/tests/roots/test-latex-numfig/conf.py
+-rw-r--r--   0        0        0      112 2023-04-23 19:57:27.565196 Sphinx-7.0.0rc1/tests/roots/test-latex-numfig/index.rst
+-rw-r--r--   0        0        0      141 2023-04-23 19:57:27.565196 Sphinx-7.0.0rc1/tests/roots/test-latex-numfig/indexhowto.rst
+-rw-r--r--   0        0        0      165 2023-04-23 19:57:27.565196 Sphinx-7.0.0rc1/tests/roots/test-latex-numfig/indexmanual.rst
+-rw-r--r--   0        0        0       18 2023-04-23 19:57:27.566196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/_mytemplates/latex/longtable.tex_t
+-rw-r--r--   0        0        0     1661 2023-04-23 19:57:27.566196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/complex.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.566196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/conf.py
+-rw-r--r--   0        0        0     1933 2023-04-23 19:57:27.566196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/complex_spanning_cell.tex
+-rw-r--r--   0        0        0     1752 2023-04-23 19:57:27.566196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/gridtable.tex
+-rw-r--r--   0        0        0     1780 2023-04-23 19:57:27.566196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/gridtable_with_tabularcolumn.tex
+-rw-r--r--   0        0        0     1323 2023-04-23 19:57:27.567196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable.tex
+-rw-r--r--   0        0        0     1300 2023-04-23 19:57:27.567196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_align.tex
+-rw-r--r--   0        0        0     1445 2023-04-23 19:57:27.567196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_caption.tex
+-rw-r--r--   0        0        0     1384 2023-04-23 19:57:27.567196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_problematic_cell.tex
+-rw-r--r--   0        0        0     1637 2023-04-23 19:57:27.568196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_stub_columns_and_problematic_cell.tex
+-rw-r--r--   0        0        0     1386 2023-04-23 19:57:27.568196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_verbatim.tex
+-rw-r--r--   0        0        0     1656 2023-04-23 19:57:27.568196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_widths.tex
+-rw-r--r--   0        0        0     1409 2023-04-23 19:57:27.568196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_widths_and_problematic_cell.tex
+-rw-r--r--   0        0        0     1341 2023-04-23 19:57:27.569196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_with_tabularcolumn.tex
+-rw-r--r--   0        0        0      704 2023-04-23 19:57:27.569196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/simple_table.tex
+-rw-r--r--   0        0        0      851 2023-04-23 19:57:27.569196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_caption.tex
+-rw-r--r--   0        0        0      777 2023-04-23 19:57:27.569196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_problematic_cell.tex
+-rw-r--r--   0        0        0      978 2023-04-23 19:57:27.569196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_stub_columns_and_problematic_cell.tex
+-rw-r--r--   0        0        0      594 2023-04-23 19:57:27.569196 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_threeparagraphs_cell_in_first_col.tex
+-rw-r--r--   0        0        0      779 2023-04-23 19:57:27.570195 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_verbatim.tex
+-rw-r--r--   0        0        0     1093 2023-04-23 19:57:27.570195 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_widths.tex
+-rw-r--r--   0        0        0      802 2023-04-23 19:57:27.570358 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_widths_and_problematic_cell.tex
+-rw-r--r--   0        0        0      733 2023-04-23 19:57:27.570358 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/tabular_having_widths.tex
+-rw-r--r--   0        0        0      747 2023-04-23 19:57:27.570358 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/tabularcolumn.tex
+-rw-r--r--   0        0        0      727 2023-04-23 19:57:27.570358 Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/tabulary_having_widths.tex
+-rw-r--r--   0        0        0       84 2023-04-23 19:57:27.570358 Sphinx-7.0.0rc1/tests/roots/test-latex-table/index.rst
+-rw-r--r--   0        0        0     2516 2023-04-23 19:57:27.570358 Sphinx-7.0.0rc1/tests/roots/test-latex-table/longtable.rst
+-rw-r--r--   0        0        0     2770 2023-04-23 19:57:27.571364 Sphinx-7.0.0rc1/tests/roots/test-latex-table/tabular.rst
+-rw-r--r--   0        0        0       52 2023-04-23 19:57:27.571364 Sphinx-7.0.0rc1/tests/roots/test-latex-theme/conf.py
+-rw-r--r--   0        0        0       24 2023-04-23 19:57:27.571364 Sphinx-7.0.0rc1/tests/roots/test-latex-theme/index.rst
+-rw-r--r--   0        0        0      117 2023-04-23 19:57:27.571364 Sphinx-7.0.0rc1/tests/roots/test-latex-theme/theme/custom/theme.conf
+-rw-r--r--   0        0        0      160 2023-04-23 19:57:27.571364 Sphinx-7.0.0rc1/tests/roots/test-latex-title/conf.py
+-rw-r--r--   0        0        0      165 2023-04-23 19:57:27.572363 Sphinx-7.0.0rc1/tests/roots/test-latex-title/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.572363 Sphinx-7.0.0rc1/tests/roots/test-latex-unicode/conf.py
+-rw-r--r--   0        0        0      142 2023-04-23 19:57:27.572363 Sphinx-7.0.0rc1/tests/roots/test-latex-unicode/index.rst
+-rw-r--r--   0        0        0       81 2023-04-23 19:57:27.572363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-anchors-ignore/conf.py
+-rw-r--r--   0        0        0      109 2023-04-23 19:57:27.572363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-anchors-ignore/index.rst
+-rw-r--r--   0        0        0      180 2023-04-23 19:57:27.572363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-documents_exclude/br0ken_link.rst
+-rw-r--r--   0        0        0      174 2023-04-23 19:57:27.573363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-documents_exclude/broken_link.rst
+-rw-r--r--   0        0        0      134 2023-04-23 19:57:27.573363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-documents_exclude/conf.py
+-rw-r--r--   0        0        0       40 2023-04-23 19:57:27.573363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-documents_exclude/index.rst
+-rw-r--r--   0        0        0       81 2023-04-23 19:57:27.573363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-localserver-anchor/conf.py
+-rw-r--r--   0        0        0       48 2023-04-23 19:57:27.573363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-localserver-anchor/index.rst
+-rw-r--r--   0        0        0       56 2023-04-23 19:57:27.573363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-localserver-https/conf.py
+-rw-r--r--   0        0        0       42 2023-04-23 19:57:27.574363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-localserver-https/index.rst
+-rw-r--r--   0        0        0       56 2023-04-23 19:57:27.574363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-localserver-warn-redirects/conf.py
+-rw-r--r--   0        0        0       95 2023-04-23 19:57:27.574363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-localserver-warn-redirects/index.rst
+-rw-r--r--   0        0        0       56 2023-04-23 19:57:27.574363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-localserver/conf.py
+-rw-r--r--   0        0        0       41 2023-04-23 19:57:27.574363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-localserver/index.rst
+-rw-r--r--   0        0        0       56 2023-04-23 19:57:27.574363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-raw-node/conf.py
+-rw-r--r--   0        0        0       46 2023-04-23 19:57:27.575363 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-raw-node/index.rst
+-rw-r--r--   0        0        0       81 2023-04-23 19:57:27.575574 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-too-many-retries/conf.py
+-rw-r--r--   0        0        0       73 2023-04-23 19:57:27.575574 Sphinx-7.0.0rc1/tests/roots/test-linkcheck-too-many-retries/index.rst
+-rw-r--r--   0        0        0      100 2023-04-23 19:57:27.575574 Sphinx-7.0.0rc1/tests/roots/test-linkcheck/conf.py
+-rw-r--r--   0        0        0      582 2023-04-23 19:57:27.575574 Sphinx-7.0.0rc1/tests/roots/test-linkcheck/links.rst
+-rw-r--r--   0        0        0      143 2023-04-23 19:57:27.575574 Sphinx-7.0.0rc1/tests/roots/test-local-logo/conf.py
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.576581 Sphinx-7.0.0rc1/tests/roots/test-local-logo/images/img.png
+-rw-r--r--   0        0        0     1477 2023-04-27 00:31:27.936073 Sphinx-7.0.0rc1/tests/roots/test-local-logo/index.rst
+-rw-r--r--   0        0        0       80 2023-04-23 19:57:27.576581 Sphinx-7.0.0rc1/tests/roots/test-locale/locale1/en/LC_MESSAGES/myext.mo
+-rw-r--r--   0        0        0       41 2023-04-23 19:57:27.577582 Sphinx-7.0.0rc1/tests/roots/test-locale/locale1/en/LC_MESSAGES/myext.po
+-rw-r--r--   0        0        0       80 2023-04-23 19:57:27.577582 Sphinx-7.0.0rc1/tests/roots/test-locale/locale1/et/LC_MESSAGES/myext.mo
+-rw-r--r--   0        0        0       41 2023-04-23 19:57:27.577582 Sphinx-7.0.0rc1/tests/roots/test-locale/locale1/et/LC_MESSAGES/myext.po
+-rw-r--r--   0        0        0       82 2023-04-23 19:57:27.577582 Sphinx-7.0.0rc1/tests/roots/test-locale/locale2/en/LC_MESSAGES/myext.mo
+-rw-r--r--   0        0        0       43 2023-04-23 19:57:27.578581 Sphinx-7.0.0rc1/tests/roots/test-locale/locale2/en/LC_MESSAGES/myext.po
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.578581 Sphinx-7.0.0rc1/tests/roots/test-manpage_url/conf.py
+-rw-r--r--   0        0        0       61 2023-04-23 19:57:27.578581 Sphinx-7.0.0rc1/tests/roots/test-manpage_url/index.rst
+-rw-r--r--   0        0        0      114 2023-04-23 19:57:27.578581 Sphinx-7.0.0rc1/tests/roots/test-markup-citation/conf.py
+-rw-r--r--   0        0        0      166 2023-04-23 19:57:27.578581 Sphinx-7.0.0rc1/tests/roots/test-markup-citation/index.rst
+-rw-r--r--   0        0        0      114 2023-04-23 19:57:27.578581 Sphinx-7.0.0rc1/tests/roots/test-markup-rubric/conf.py
+-rw-r--r--   0        0        0      112 2023-04-23 19:57:27.579581 Sphinx-7.0.0rc1/tests/roots/test-markup-rubric/index.rst
+-rw-r--r--   0        0        0       78 2023-04-23 19:57:27.579581 Sphinx-7.0.0rc1/tests/roots/test-maxlistdepth/conf.py
+-rw-r--r--   0        0        0      687 2023-04-23 19:57:27.579581 Sphinx-7.0.0rc1/tests/roots/test-maxlistdepth/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.579581 Sphinx-7.0.0rc1/tests/roots/test-metadata/conf.py
+-rw-r--r--   0        0        0     1436 2023-04-23 19:57:27.579581 Sphinx-7.0.0rc1/tests/roots/test-metadata/index.rst
+-rw-r--r--   0        0        0        8 2023-04-23 19:57:27.579581 Sphinx-7.0.0rc1/tests/roots/test-need-escaped/bar.rst
+-rw-r--r--   0        0        0        8 2023-04-23 19:57:27.579581 Sphinx-7.0.0rc1/tests/roots/test-need-escaped/baz.rst
+-rw-r--r--   0        0        0       62 2023-04-23 19:57:27.580581 Sphinx-7.0.0rc1/tests/roots/test-need-escaped/conf.py
+-rw-r--r--   0        0        0       82 2023-04-23 19:57:27.580581 Sphinx-7.0.0rc1/tests/roots/test-need-escaped/foo.rst
+-rw-r--r--   0        0        0      574 2023-04-23 19:57:27.580581 Sphinx-7.0.0rc1/tests/roots/test-need-escaped/index.rst
+-rw-r--r--   0        0        0       10 2023-04-23 19:57:27.580581 Sphinx-7.0.0rc1/tests/roots/test-need-escaped/quux.rst
+-rw-r--r--   0        0        0       29 2023-04-23 19:57:27.580581 Sphinx-7.0.0rc1/tests/roots/test-need-escaped/qux.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.580581 Sphinx-7.0.0rc1/tests/roots/test-nested-enumerated-list/conf.py
+-rw-r--r--   0        0        0      300 2023-04-23 19:57:27.580581 Sphinx-7.0.0rc1/tests/roots/test-nested-enumerated-list/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.581582 Sphinx-7.0.0rc1/tests/roots/test-nested-tables/conf.py
+-rw-r--r--   0        0        0      248 2023-04-23 19:57:27.581582 Sphinx-7.0.0rc1/tests/roots/test-nested-tables/index.rst
+-rw-r--r--   0        0        0       16 2023-04-23 19:57:27.581582 Sphinx-7.0.0rc1/tests/roots/test-nitpicky-warnings/conf.py
+-rw-r--r--   0        0        0      176 2023-04-23 19:57:27.581582 Sphinx-7.0.0rc1/tests/roots/test-nitpicky-warnings/index.rst
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.581582 Sphinx-7.0.0rc1/tests/roots/test-numbered-circular/conf.py
+-rw-r--r--   0        0        0       36 2023-04-23 19:57:27.581582 Sphinx-7.0.0rc1/tests/roots/test-numbered-circular/index.rst
+-rw-r--r--   0        0        0       23 2023-04-23 19:57:27.581582 Sphinx-7.0.0rc1/tests/roots/test-numbered-circular/sub.rst
+-rw-r--r--   0        0        0      710 2023-04-23 19:57:27.582581 Sphinx-7.0.0rc1/tests/roots/test-numfig/bar.rst
+-rw-r--r--   0        0        0      259 2023-04-23 19:57:27.582581 Sphinx-7.0.0rc1/tests/roots/test-numfig/baz.rst
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.582581 Sphinx-7.0.0rc1/tests/roots/test-numfig/conf.py
+-rw-r--r--   0        0        0      912 2023-04-23 19:57:27.582581 Sphinx-7.0.0rc1/tests/roots/test-numfig/foo.rst
+-rw-r--r--   0        0        0     1024 2023-04-23 19:57:27.582581 Sphinx-7.0.0rc1/tests/roots/test-numfig/index.rst
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.582581 Sphinx-7.0.0rc1/tests/roots/test-numfig/rimg.png
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.582581 Sphinx-7.0.0rc1/tests/roots/test-object-description-sections/conf.py
+-rw-r--r--   0        0        0       80 2023-04-23 19:57:27.582581 Sphinx-7.0.0rc1/tests/roots/test-object-description-sections/index.rst
+-rw-r--r--   0        0        0       73 2023-04-23 19:57:27.583581 Sphinx-7.0.0rc1/tests/roots/test-productionlist/Bare.rst
+-rw-r--r--   0        0        0       58 2023-04-23 19:57:27.583581 Sphinx-7.0.0rc1/tests/roots/test-productionlist/Dup1.rst
+-rw-r--r--   0        0        0       58 2023-04-23 19:57:27.583581 Sphinx-7.0.0rc1/tests/roots/test-productionlist/Dup2.rst
+-rw-r--r--   0        0        0       94 2023-04-23 19:57:27.583581 Sphinx-7.0.0rc1/tests/roots/test-productionlist/LineContinuation.rst
+-rw-r--r--   0        0        0       72 2023-04-23 19:57:27.583581 Sphinx-7.0.0rc1/tests/roots/test-productionlist/P1.rst
+-rw-r--r--   0        0        0       72 2023-04-23 19:57:27.583581 Sphinx-7.0.0rc1/tests/roots/test-productionlist/P2.rst
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.583581 Sphinx-7.0.0rc1/tests/roots/test-productionlist/conf.py
+-rw-r--r--   0        0        0       97 2023-04-23 19:57:27.583581 Sphinx-7.0.0rc1/tests/roots/test-productionlist/firstLineRule.rst
+-rw-r--r--   0        0        0      663 2023-04-23 19:57:27.584581 Sphinx-7.0.0rc1/tests/roots/test-productionlist/index.rst
+-rw-r--r--   0        0        0      177 2023-04-23 19:57:27.584581 Sphinx-7.0.0rc1/tests/roots/test-prolog/conf.py
+-rw-r--r--   0        0        0       83 2023-04-23 19:57:27.584581 Sphinx-7.0.0rc1/tests/roots/test-prolog/index.rst
+-rw-r--r--   0        0        0       57 2023-04-23 19:57:27.584581 Sphinx-7.0.0rc1/tests/roots/test-prolog/markdown.md
+-rw-r--r--   0        0        0      299 2023-04-23 19:57:27.584581 Sphinx-7.0.0rc1/tests/roots/test-prolog/prolog_markdown_parser.py
+-rw-r--r--   0        0        0       67 2023-04-23 19:57:27.584581 Sphinx-7.0.0rc1/tests/roots/test-prolog/restructuredtext.rst
+-rw-r--r--   0        0        0       75 2023-04-25 10:59:46.885153 Sphinx-7.0.0rc1/tests/roots/test-pycode/cp_1251_coded.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.585581 Sphinx-7.0.0rc1/tests/roots/test-reST-code-block/conf.py
+-rw-r--r--   0        0        0       97 2023-04-23 19:57:27.585581 Sphinx-7.0.0rc1/tests/roots/test-reST-code-block/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.585581 Sphinx-7.0.0rc1/tests/roots/test-reST-code-role/conf.py
+-rw-r--r--   0        0        0      194 2023-04-23 19:57:27.585581 Sphinx-7.0.0rc1/tests/roots/test-reST-code-role/index.rst
+-rw-r--r--   0        0        0       27 2023-04-23 19:57:27.585581 Sphinx-7.0.0rc1/tests/roots/test-refonly_bullet_list/conf.py
+-rw-r--r--   0        0        0      147 2023-04-23 19:57:27.585581 Sphinx-7.0.0rc1/tests/roots/test-refonly_bullet_list/index.rst
+-rw-r--r--   0        0        0      237 2023-04-23 19:57:27.586581 Sphinx-7.0.0rc1/tests/roots/test-remote-logo/conf.py
+-rw-r--r--   0        0        0     1477 2023-04-27 00:31:27.936073 Sphinx-7.0.0rc1/tests/roots/test-remote-logo/index.rst
+-rw-r--r--   0        0        0       32 2023-04-23 19:57:27.586581 Sphinx-7.0.0rc1/tests/roots/test-roles-download/another/dummy.dat
+-rw-r--r--   0        0        0      114 2023-04-23 19:57:27.586581 Sphinx-7.0.0rc1/tests/roots/test-roles-download/conf.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.586581 Sphinx-7.0.0rc1/tests/roots/test-roles-download/dummy.dat
+-rw-r--r--   0        0        0      214 2023-04-23 19:57:27.586581 Sphinx-7.0.0rc1/tests/roots/test-roles-download/index.rst
+-rw-r--r--   0        0        0     2111 2023-04-23 19:57:27.586581 Sphinx-7.0.0rc1/tests/roots/test-root/Makefile
+-rw-r--r--   0        0        0       67 2023-04-23 19:57:27.587581 Sphinx-7.0.0rc1/tests/roots/test-root/_templates/contentssb.html
+-rw-r--r--   0        0        0       99 2023-04-23 19:57:27.587581 Sphinx-7.0.0rc1/tests/roots/test-root/_templates/customsb.html
+-rw-r--r--   0        0        0      428 2023-04-23 19:57:27.587581 Sphinx-7.0.0rc1/tests/roots/test-root/_templates/layout.html
+-rw-r--r--   0        0        0      578 2023-04-23 19:57:27.587581 Sphinx-7.0.0rc1/tests/roots/test-root/autodoc.txt
+-rw-r--r--   0        0        0     4587 2023-04-23 19:57:27.587581 Sphinx-7.0.0rc1/tests/roots/test-root/autodoc_target.py
+-rw-r--r--   0        0        0       74 2023-04-23 19:57:27.587581 Sphinx-7.0.0rc1/tests/roots/test-root/bom.txt
+-rw-r--r--   0        0        0     4257 2023-04-23 19:57:27.588581 Sphinx-7.0.0rc1/tests/roots/test-root/conf.py
+-rw-r--r--   0        0        0       87 2023-04-23 19:57:27.588581 Sphinx-7.0.0rc1/tests/roots/test-root/extapi.txt
+-rw-r--r--   0        0        0      365 2023-04-23 19:57:27.588581 Sphinx-7.0.0rc1/tests/roots/test-root/extensions.txt
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.588581 Sphinx-7.0.0rc1/tests/roots/test-root/file_with_special_#_chars.xyz
+-rw-r--r--   0        0        0      826 2023-04-23 19:57:27.588581 Sphinx-7.0.0rc1/tests/roots/test-root/footnote.txt
+-rw-r--r--   0        0        0      575 2023-04-23 19:57:27.588581 Sphinx-7.0.0rc1/tests/roots/test-root/images.txt
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.588581 Sphinx-7.0.0rc1/tests/roots/test-root/img.foo.png
+-rw-r--r--   0        0        0    24976 2023-04-23 19:57:27.589582 Sphinx-7.0.0rc1/tests/roots/test-root/img.gif
+-rw-r--r--   0        0        0   141783 2023-04-23 19:57:27.590582 Sphinx-7.0.0rc1/tests/roots/test-root/img.pdf
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.590582 Sphinx-7.0.0rc1/tests/roots/test-root/img.png
+-rw-r--r--   0        0        0     2108 2023-04-23 19:57:27.590582 Sphinx-7.0.0rc1/tests/roots/test-root/includes.txt
+-rw-r--r--   0        0        0     1118 2023-04-23 19:57:27.590582 Sphinx-7.0.0rc1/tests/roots/test-root/index.txt
+-rw-r--r--   0        0        0      750 2023-04-23 19:57:27.590582 Sphinx-7.0.0rc1/tests/roots/test-root/lists.txt
+-rw-r--r--   0        0        0      200 2023-04-23 19:57:27.590582 Sphinx-7.0.0rc1/tests/roots/test-root/literal.inc
+-rw-r--r--   0        0        0      208 2023-04-23 19:57:27.591581 Sphinx-7.0.0rc1/tests/roots/test-root/literal_orig.inc
+-rw-r--r--   0        0        0     6919 2023-04-23 19:57:27.591581 Sphinx-7.0.0rc1/tests/roots/test-root/markup.txt
+-rw-r--r--   0        0        0      373 2023-04-23 19:57:27.591581 Sphinx-7.0.0rc1/tests/roots/test-root/math.txt
+-rw-r--r--   0        0        0     4561 2023-04-23 19:57:27.591581 Sphinx-7.0.0rc1/tests/roots/test-root/objects.txt
+-rw-r--r--   0        0        0      110 2023-04-23 19:57:27.591581 Sphinx-7.0.0rc1/tests/roots/test-root/otherext.foo
+-rw-r--r--   0        0        0      346 2023-04-23 19:57:27.591581 Sphinx-7.0.0rc1/tests/roots/test-root/parsermod.py
+-rw-r--r--   0        0        0       45 2023-04-23 19:57:27.591581 Sphinx-7.0.0rc1/tests/roots/test-root/quotes.inc
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.591581 Sphinx-7.0.0rc1/tests/roots/test-root/rimg.png
+-rw-r--r--   0        0        0       40 2023-04-23 19:57:27.592581 Sphinx-7.0.0rc1/tests/roots/test-root/special/api.h
+-rw-r--r--   0        0        0       32 2023-04-23 19:57:27.592581 Sphinx-7.0.0rc1/tests/roots/test-root/special/code.py
+-rw-r--r--   0        0        0       96 2023-04-23 19:57:27.592581 Sphinx-7.0.0rc1/tests/roots/test-root/subdir/excluded.txt
+-rw-r--r--   0        0        0      106 2023-04-23 19:57:27.592581 Sphinx-7.0.0rc1/tests/roots/test-root/subdir/images.txt
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.593582 Sphinx-7.0.0rc1/tests/roots/test-root/subdir/img.png
+-rw-r--r--   0        0        0      143 2023-04-23 19:57:27.593582 Sphinx-7.0.0rc1/tests/roots/test-root/subdir/include.inc
+-rw-r--r--   0        0        0      328 2023-04-23 19:57:27.593582 Sphinx-7.0.0rc1/tests/roots/test-root/subdir/includes.txt
+-rw-r--r--   0        0        0    66247 2023-04-23 19:57:27.593582 Sphinx-7.0.0rc1/tests/roots/test-root/subdir/simg.png
+-rw-r--r--   0        0        0   141783 2023-04-23 19:57:27.594581 Sphinx-7.0.0rc1/tests/roots/test-root/svgimg.pdf
+-rw-r--r--   0        0        0      243 2023-04-23 19:57:27.594581 Sphinx-7.0.0rc1/tests/roots/test-root/svgimg.svg
+-rw-r--r--   0        0        0       78 2023-04-23 19:57:27.595582 Sphinx-7.0.0rc1/tests/roots/test-root/tabs.inc
+-rw-r--r--   0        0        0       77 2023-04-23 19:57:27.595582 Sphinx-7.0.0rc1/tests/roots/test-root/test.inc
+-rw-r--r--   0        0        0      107 2023-04-23 19:57:27.595582 Sphinx-7.0.0rc1/tests/roots/test-root/wrongenc.inc
+-rw-r--r--   0        0        0       58 2023-04-23 19:57:27.595582 Sphinx-7.0.0rc1/tests/roots/test-search/conf.py
+-rw-r--r--   0        0        0      381 2023-04-23 19:57:27.595582 Sphinx-7.0.0rc1/tests/roots/test-search/index.rst
+-rw-r--r--   0        0        0       41 2023-04-23 19:57:27.595582 Sphinx-7.0.0rc1/tests/roots/test-search/nosearch.rst
+-rw-r--r--   0        0        0      184 2023-04-23 19:57:27.595582 Sphinx-7.0.0rc1/tests/roots/test-search/tocitem.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.596580 Sphinx-7.0.0rc1/tests/roots/test-smartquotes/conf.py
+-rw-r--r--   0        0        0      107 2023-04-23 19:57:27.596580 Sphinx-7.0.0rc1/tests/roots/test-smartquotes/index.rst
+-rw-r--r--   0        0        0      231 2023-04-23 19:57:27.596580 Sphinx-7.0.0rc1/tests/roots/test-smartquotes/literals.rst
+-rw-r--r--   0        0        0      453 2023-04-23 19:57:27.596580 Sphinx-7.0.0rc1/tests/roots/test-stylesheets/_templates/layout.html
+-rw-r--r--   0        0        0      318 2023-04-23 19:57:27.596580 Sphinx-7.0.0rc1/tests/roots/test-stylesheets/conf.py
+-rw-r--r--   0        0        0       53 2023-04-23 19:57:27.596580 Sphinx-7.0.0rc1/tests/roots/test-stylesheets/index.rst
+-rw-r--r--   0        0        0      182 2023-04-23 19:57:27.597580 Sphinx-7.0.0rc1/tests/roots/test-templating/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      109 2023-04-23 19:57:27.597580 Sphinx-7.0.0rc1/tests/roots/test-templating/_templates/layout.html
+-rw-r--r--   0        0        0      135 2023-04-23 19:57:27.597580 Sphinx-7.0.0rc1/tests/roots/test-templating/autosummary_templating.txt
+-rw-r--r--   0        0        0      266 2023-04-23 19:57:27.597580 Sphinx-7.0.0rc1/tests/roots/test-templating/conf.py
+-rw-r--r--   0        0        0      124 2023-04-23 19:57:27.597580 Sphinx-7.0.0rc1/tests/roots/test-templating/index.txt
+-rw-r--r--   0        0        0      661 2023-04-23 19:57:27.598581 Sphinx-7.0.0rc1/tests/roots/test-theming/child.zip
+-rw-r--r--   0        0        0       94 2023-04-23 19:57:27.598581 Sphinx-7.0.0rc1/tests/roots/test-theming/conf.py
+-rw-r--r--   0        0        0       26 2023-04-23 19:57:27.598581 Sphinx-7.0.0rc1/tests/roots/test-theming/index.rst
+-rw-r--r--   0        0        0     1039 2023-04-23 19:57:27.599582 Sphinx-7.0.0rc1/tests/roots/test-theming/parent.zip
+-rw-r--r--   0        0        0       82 2023-04-23 19:57:27.599582 Sphinx-7.0.0rc1/tests/roots/test-theming/test_theme/__init__.py
+-rw-r--r--   0        0        0      139 2023-04-23 19:57:27.599582 Sphinx-7.0.0rc1/tests/roots/test-theming/test_theme/staticfiles/layout.html
+-rw-r--r--   0        0        0      120 2023-04-23 19:57:27.599582 Sphinx-7.0.0rc1/tests/roots/test-theming/test_theme/staticfiles/static/staticimg.png
+-rw-r--r--   0        0        0       82 2023-04-23 19:57:27.600582 Sphinx-7.0.0rc1/tests/roots/test-theming/test_theme/staticfiles/static/statictmpl.html_t
+-rw-r--r--   0        0        0      104 2023-04-23 19:57:27.600582 Sphinx-7.0.0rc1/tests/roots/test-theming/test_theme/staticfiles/theme.conf
+-rw-r--r--   0        0        0       98 2023-04-23 19:57:27.600582 Sphinx-7.0.0rc1/tests/roots/test-theming/test_theme/test-theme/theme.conf
+-rw-r--r--   0        0        0     1039 2023-04-23 19:57:27.600582 Sphinx-7.0.0rc1/tests/roots/test-theming/ziptheme.zip
+-rw-r--r--   0        0        0      150 2023-04-23 19:57:27.600582 Sphinx-7.0.0rc1/tests/roots/test-tocdepth/bar.rst
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.601583 Sphinx-7.0.0rc1/tests/roots/test-tocdepth/baz.rst
+-rw-r--r--   0        0        0       53 2023-04-23 19:57:27.601583 Sphinx-7.0.0rc1/tests/roots/test-tocdepth/conf.py
+-rw-r--r--   0        0        0      146 2023-04-23 19:57:27.601583 Sphinx-7.0.0rc1/tests/roots/test-tocdepth/foo.rst
+-rw-r--r--   0        0        0       71 2023-04-23 19:57:27.601583 Sphinx-7.0.0rc1/tests/roots/test-tocdepth/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.601583 Sphinx-7.0.0rc1/tests/roots/test-toctree-domain-objects/conf.py
+-rw-r--r--   0        0        0      731 2023-04-23 19:57:27.602583 Sphinx-7.0.0rc1/tests/roots/test-toctree-domain-objects/domains.rst
+-rw-r--r--   0        0        0       90 2023-04-23 19:57:27.602583 Sphinx-7.0.0rc1/tests/roots/test-toctree-domain-objects/index.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.602583 Sphinx-7.0.0rc1/tests/roots/test-toctree-duplicated/conf.py
+-rw-r--r--   0        0        0        8 2023-04-23 19:57:27.602583 Sphinx-7.0.0rc1/tests/roots/test-toctree-duplicated/foo.rst
+-rw-r--r--   0        0        0       77 2023-04-23 19:57:27.602583 Sphinx-7.0.0rc1/tests/roots/test-toctree-duplicated/index.rst
+-rw-r--r--   0        0        0      101 2023-04-23 19:57:27.602583 Sphinx-7.0.0rc1/tests/roots/test-toctree-empty/_templates/localtoc.html
+-rw-r--r--   0        0        0       62 2023-04-23 19:57:27.603581 Sphinx-7.0.0rc1/tests/roots/test-toctree-empty/conf.py
+-rw-r--r--   0        0        0       52 2023-04-23 19:57:27.603581 Sphinx-7.0.0rc1/tests/roots/test-toctree-empty/index.rst
+-rw-r--r--   0        0        0       17 2023-04-23 19:57:27.603581 Sphinx-7.0.0rc1/tests/roots/test-toctree-glob/bar/bar_1.rst
+-rw-r--r--   0        0        0       17 2023-04-23 19:57:27.604581 Sphinx-7.0.0rc1/tests/roots/test-toctree-glob/bar/bar_2.rst
+-rw-r--r--   0        0        0       17 2023-04-23 19:57:27.604581 Sphinx-7.0.0rc1/tests/roots/test-toctree-glob/bar/bar_3.rst
+-rw-r--r--   0        0        0       17 2023-04-23 19:57:27.604581 Sphinx-7.0.0rc1/tests/roots/test-toctree-glob/bar/bar_4/index.rst
+-rw-r--r--   0        0        0       53 2023-04-23 19:57:27.604581 Sphinx-7.0.0rc1/tests/roots/test-toctree-glob/bar/index.rst
+-rw-r--r--   0        0        0       13 2023-04-23 19:57:27.604581 Sphinx-7.0.0rc1/tests/roots/test-toctree-glob/baz.rst
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.604581 Sphinx-7.0.0rc1/tests/roots/test-toctree-glob/conf.py
+-rw-r--r--   0        0        0       13 2023-04-23 19:57:27.604581 Sphinx-7.0.0rc1/tests/roots/test-toctree-glob/foo.rst
+-rw-r--r--   0        0        0      303 2023-04-23 19:57:27.605581 Sphinx-7.0.0rc1/tests/roots/test-toctree-glob/index.rst
+-rw-r--r--   0        0        0       16 2023-04-23 19:57:27.605581 Sphinx-7.0.0rc1/tests/roots/test-toctree-glob/quux.rst
+-rw-r--r--   0        0        0       50 2023-04-23 19:57:27.605581 Sphinx-7.0.0rc1/tests/roots/test-toctree-glob/qux/index.rst
+-rw-r--r--   0        0        0       17 2023-04-23 19:57:27.605581 Sphinx-7.0.0rc1/tests/roots/test-toctree-glob/qux/qux_1.rst
+-rw-r--r--   0        0        0       17 2023-04-23 19:57:27.606581 Sphinx-7.0.0rc1/tests/roots/test-toctree-glob/qux/qux_2.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.606581 Sphinx-7.0.0rc1/tests/roots/test-toctree-index/conf.py
+-rw-r--r--   0        0        0      105 2023-04-23 19:57:27.606581 Sphinx-7.0.0rc1/tests/roots/test-toctree-index/foo.rst
+-rw-r--r--   0        0        0      132 2023-04-23 19:57:27.606581 Sphinx-7.0.0rc1/tests/roots/test-toctree-index/index.rst
+-rw-r--r--   0        0        0      150 2023-04-23 19:57:27.606581 Sphinx-7.0.0rc1/tests/roots/test-toctree-maxdepth/bar.rst
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.606581 Sphinx-7.0.0rc1/tests/roots/test-toctree-maxdepth/baz.rst
+-rw-r--r--   0        0        0       30 2023-04-23 19:57:27.607582 Sphinx-7.0.0rc1/tests/roots/test-toctree-maxdepth/conf.py
+-rw-r--r--   0        0        0      146 2023-04-23 19:57:27.607582 Sphinx-7.0.0rc1/tests/roots/test-toctree-maxdepth/foo.rst
+-rw-r--r--   0        0        0      105 2023-04-23 19:57:27.607582 Sphinx-7.0.0rc1/tests/roots/test-toctree-maxdepth/index.rst
+-rw-r--r--   0        0        0      105 2023-04-23 19:57:27.607582 Sphinx-7.0.0rc1/tests/roots/test-toctree-maxdepth/qux.rst
+-rw-r--r--   0        0        0        8 2023-04-23 19:57:27.607582 Sphinx-7.0.0rc1/tests/roots/test-toctree/bar.rst
+-rw-r--r--   0        0        0        8 2023-04-23 19:57:27.607582 Sphinx-7.0.0rc1/tests/roots/test-toctree/baz.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.607582 Sphinx-7.0.0rc1/tests/roots/test-toctree/conf.py
+-rw-r--r--   0        0        0       74 2023-04-23 19:57:27.608580 Sphinx-7.0.0rc1/tests/roots/test-toctree/foo.rst
+-rw-r--r--   0        0        0      885 2023-04-23 19:57:27.608580 Sphinx-7.0.0rc1/tests/roots/test-toctree/index.rst
+-rw-r--r--   0        0        0       10 2023-04-23 19:57:27.608580 Sphinx-7.0.0rc1/tests/roots/test-toctree/quux.rst
+-rw-r--r--   0        0        0       29 2023-04-23 19:57:27.608580 Sphinx-7.0.0rc1/tests/roots/test-toctree/qux.rst
+-rw-r--r--   0        0        0       97 2023-04-23 19:57:27.608580 Sphinx-7.0.0rc1/tests/roots/test-toctree/tocdepth.rst
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.608580 Sphinx-7.0.0rc1/tests/roots/test-transforms-post_transforms-keyboard/conf.py
+-rw-r--r--   0        0        0       94 2023-04-23 19:57:27.609582 Sphinx-7.0.0rc1/tests/roots/test-transforms-post_transforms-keyboard/index.rst
+-rw-r--r--   0        0        0       16 2023-04-23 19:57:27.609582 Sphinx-7.0.0rc1/tests/roots/test-transforms-post_transforms-missing-reference/conf.py
+-rw-r--r--   0        0        0      113 2023-04-23 19:57:27.609582 Sphinx-7.0.0rc1/tests/roots/test-transforms-post_transforms-missing-reference/index.rst
+-rw-r--r--   0        0        0       36 2023-04-23 19:57:27.609582 Sphinx-7.0.0rc1/tests/roots/test-trim_doctest_flags/conf.py
+-rw-r--r--   0        0        0      784 2023-04-23 19:57:27.609582 Sphinx-7.0.0rc1/tests/roots/test-trim_doctest_flags/index.rst
+-rw-r--r--   0        0        0     1012 2023-04-23 19:57:27.610582 Sphinx-7.0.0rc1/tests/roots/test-versioning/added.txt
+-rw-r--r--   0        0        0       86 2023-04-23 19:57:27.610582 Sphinx-7.0.0rc1/tests/roots/test-versioning/conf.py
+-rw-r--r--   0        0        0      584 2023-04-23 19:57:27.610582 Sphinx-7.0.0rc1/tests/roots/test-versioning/deleted.txt
+-rw-r--r--   0        0        0      490 2023-04-23 19:57:27.610582 Sphinx-7.0.0rc1/tests/roots/test-versioning/deleted_end.txt
+-rw-r--r--   0        0        0      164 2023-04-23 19:57:27.610582 Sphinx-7.0.0rc1/tests/roots/test-versioning/index.txt
+-rw-r--r--   0        0        0      864 2023-04-23 19:57:27.610582 Sphinx-7.0.0rc1/tests/roots/test-versioning/insert.txt
+-rw-r--r--   0        0        0      850 2023-04-23 19:57:27.611492 Sphinx-7.0.0rc1/tests/roots/test-versioning/insert_beginning.txt
+-rw-r--r--   0        0        0      735 2023-04-23 19:57:27.611492 Sphinx-7.0.0rc1/tests/roots/test-versioning/insert_similar.txt
+-rw-r--r--   0        0        0      867 2023-04-23 19:57:27.611492 Sphinx-7.0.0rc1/tests/roots/test-versioning/modified.txt
+-rw-r--r--   0        0        0      715 2023-04-23 19:57:27.611492 Sphinx-7.0.0rc1/tests/roots/test-versioning/original.txt
+-rw-r--r--   0        0        0      151 2023-04-23 19:57:27.611492 Sphinx-7.0.0rc1/tests/roots/test-warnings/autodoc_fodder.py
+-rw-r--r--   0        0        0       97 2023-04-23 19:57:27.611492 Sphinx-7.0.0rc1/tests/roots/test-warnings/conf.py
+-rw-r--r--   0        0        0      697 2023-04-23 19:57:27.612498 Sphinx-7.0.0rc1/tests/roots/test-warnings/index.rst
+-rw-r--r--   0        0        0   141783 2023-04-23 19:57:27.613498 Sphinx-7.0.0rc1/tests/roots/test-warnings/svgimg.pdf
+-rw-r--r--   0        0        0      243 2023-04-23 19:57:27.613498 Sphinx-7.0.0rc1/tests/roots/test-warnings/svgimg.svg
+-rw-r--r--   0        0        0       18 2023-04-23 19:57:27.613498 Sphinx-7.0.0rc1/tests/roots/test-warnings/undecodable.rst
+-rw-r--r--   0        0        0      107 2023-04-23 19:57:27.613498 Sphinx-7.0.0rc1/tests/roots/test-warnings/wrongenc.inc
+-rw-r--r--   0        0        0     3309 2023-04-23 19:57:27.613498 Sphinx-7.0.0rc1/tests/test_api_translator.py
+-rw-r--r--   0        0        0     5605 2023-04-23 19:57:27.614498 Sphinx-7.0.0rc1/tests/test_application.py
+-rw-r--r--   0        0        0     4771 2023-04-23 19:57:27.614498 Sphinx-7.0.0rc1/tests/test_build.py
+-rw-r--r--   0        0        0     1152 2023-04-23 19:57:27.614498 Sphinx-7.0.0rc1/tests/test_build_changes.py
+-rw-r--r--   0        0        0     1407 2023-04-23 19:57:27.614498 Sphinx-7.0.0rc1/tests/test_build_dirhtml.py
+-rw-r--r--   0        0        0    16623 2023-04-23 19:57:27.615497 Sphinx-7.0.0rc1/tests/test_build_epub.py
+-rw-r--r--   0        0        0     6660 2023-04-23 19:57:27.615497 Sphinx-7.0.0rc1/tests/test_build_gettext.py
+-rw-r--r--   0        0        0    80591 2023-04-28 10:59:41.037038 Sphinx-7.0.0rc1/tests/test_build_html.py
+-rw-r--r--   0        0        0    75378 2023-04-23 19:57:27.616498 Sphinx-7.0.0rc1/tests/test_build_latex.py
+-rw-r--r--   0        0        0    24262 2023-04-23 19:57:27.616498 Sphinx-7.0.0rc1/tests/test_build_linkcheck.py
+-rw-r--r--   0        0        0     2751 2023-04-23 19:57:27.616498 Sphinx-7.0.0rc1/tests/test_build_manpage.py
+-rw-r--r--   0        0        0     5910 2023-04-23 19:57:27.616498 Sphinx-7.0.0rc1/tests/test_build_texinfo.py
+-rw-r--r--   0        0        0     8996 2023-04-23 19:57:27.617498 Sphinx-7.0.0rc1/tests/test_build_text.py
+-rw-r--r--   0        0        0     1322 2023-04-23 19:57:27.617498 Sphinx-7.0.0rc1/tests/test_builder.py
+-rw-r--r--   0        0        0     2646 2023-04-23 19:57:27.617498 Sphinx-7.0.0rc1/tests/test_catalogs.py
+-rw-r--r--   0        0        0    15085 2023-04-26 16:05:03.832456 Sphinx-7.0.0rc1/tests/test_config.py
+-rw-r--r--   0        0        0      811 2023-04-23 19:57:27.617967 Sphinx-7.0.0rc1/tests/test_correct_year.py
+-rw-r--r--   0        0        0    23761 2023-04-23 19:57:27.617967 Sphinx-7.0.0rc1/tests/test_directive_code.py
+-rw-r--r--   0        0        0     2088 2023-04-23 19:57:27.617967 Sphinx-7.0.0rc1/tests/test_directive_object_description.py
+-rw-r--r--   0        0        0     1655 2023-04-23 19:57:27.618752 Sphinx-7.0.0rc1/tests/test_directive_only.py
+-rw-r--r--   0        0        0     5207 2023-04-23 19:57:27.618752 Sphinx-7.0.0rc1/tests/test_directive_other.py
+-rw-r--r--   0        0        0     4362 2023-04-23 19:57:27.619179 Sphinx-7.0.0rc1/tests/test_directive_patch.py
+-rw-r--r--   0        0        0     1084 2023-04-23 19:57:27.619179 Sphinx-7.0.0rc1/tests/test_docutilsconf.py
+-rw-r--r--   0        0        0    28522 2023-04-23 19:57:27.619179 Sphinx-7.0.0rc1/tests/test_domain_c.py
+-rw-r--r--   0        0        0    67113 2023-04-23 19:57:27.620191 Sphinx-7.0.0rc1/tests/test_domain_cpp.py
+-rw-r--r--   0        0        0    10933 2023-04-23 19:57:27.620393 Sphinx-7.0.0rc1/tests/test_domain_js.py
+-rw-r--r--   0        0        0    76403 2023-04-23 19:57:27.620829 Sphinx-7.0.0rc1/tests/test_domain_py.py
+-rw-r--r--   0        0        0     5896 2023-04-23 19:57:27.620829 Sphinx-7.0.0rc1/tests/test_domain_rst.py
+-rw-r--r--   0        0        0    19424 2023-04-23 19:57:27.620829 Sphinx-7.0.0rc1/tests/test_domain_std.py
+-rw-r--r--   0        0        0     5286 2023-04-23 19:57:27.620829 Sphinx-7.0.0rc1/tests/test_environment.py
+-rw-r--r--   0        0        0     8068 2023-04-23 19:57:27.621840 Sphinx-7.0.0rc1/tests/test_environment_indexentries.py
+-rw-r--r--   0        0        0      310 2023-04-23 19:57:27.621840 Sphinx-7.0.0rc1/tests/test_environment_record_dependencies.py
+-rw-r--r--   0        0        0    20508 2023-04-23 19:57:27.621840 Sphinx-7.0.0rc1/tests/test_environment_toctree.py
+-rw-r--r--   0        0        0      321 2023-04-23 19:57:27.621840 Sphinx-7.0.0rc1/tests/test_errors.py
+-rw-r--r--   0        0        0     1826 2023-04-23 19:57:27.621840 Sphinx-7.0.0rc1/tests/test_events.py
+-rw-r--r--   0        0        0    23255 2023-04-23 19:57:27.621840 Sphinx-7.0.0rc1/tests/test_ext_apidoc.py
+-rw-r--r--   0        0        0    76880 2023-04-23 19:57:27.622839 Sphinx-7.0.0rc1/tests/test_ext_autodoc.py
+-rw-r--r--   0        0        0     4801 2023-04-23 19:57:27.622839 Sphinx-7.0.0rc1/tests/test_ext_autodoc_autoattribute.py
+-rw-r--r--   0        0        0    14272 2023-04-23 19:57:27.622839 Sphinx-7.0.0rc1/tests/test_ext_autodoc_autoclass.py
+-rw-r--r--   0        0        0     2631 2023-04-23 19:57:27.622839 Sphinx-7.0.0rc1/tests/test_ext_autodoc_autodata.py
+-rw-r--r--   0        0        0     5647 2023-04-23 19:57:27.623839 Sphinx-7.0.0rc1/tests/test_ext_autodoc_autofunction.py
+-rw-r--r--   0        0        0     5355 2023-04-23 19:57:27.624010 Sphinx-7.0.0rc1/tests/test_ext_autodoc_automodule.py
+-rw-r--r--   0        0        0     2501 2023-04-23 19:57:27.624010 Sphinx-7.0.0rc1/tests/test_ext_autodoc_autoproperty.py
+-rw-r--r--   0        0        0    55422 2023-04-23 19:57:27.624010 Sphinx-7.0.0rc1/tests/test_ext_autodoc_configs.py
+-rw-r--r--   0        0        0     3335 2023-04-23 19:57:27.625016 Sphinx-7.0.0rc1/tests/test_ext_autodoc_events.py
+-rw-r--r--   0        0        0     3963 2023-04-23 19:57:27.625016 Sphinx-7.0.0rc1/tests/test_ext_autodoc_mock.py
+-rw-r--r--   0        0        0     1666 2023-04-23 19:57:27.625016 Sphinx-7.0.0rc1/tests/test_ext_autodoc_preserve_defaults.py
+-rw-r--r--   0        0        0     4415 2023-04-23 19:57:27.625016 Sphinx-7.0.0rc1/tests/test_ext_autodoc_private_members.py
+-rw-r--r--   0        0        0     3145 2023-04-23 19:57:27.625016 Sphinx-7.0.0rc1/tests/test_ext_autosectionlabel.py
+-rw-r--r--   0        0        0    27705 2023-04-23 19:57:27.626128 Sphinx-7.0.0rc1/tests/test_ext_autosummary.py
+-rw-r--r--   0        0        0     3158 2023-04-23 19:57:27.626507 Sphinx-7.0.0rc1/tests/test_ext_coverage.py
+-rw-r--r--   0        0        0     5524 2023-04-23 19:57:27.626635 Sphinx-7.0.0rc1/tests/test_ext_doctest.py
+-rw-r--r--   0        0        0      378 2023-04-23 19:57:27.626635 Sphinx-7.0.0rc1/tests/test_ext_duration.py
+-rw-r--r--   0        0        0     2104 2023-04-23 19:57:27.626635 Sphinx-7.0.0rc1/tests/test_ext_extlinks.py
+-rw-r--r--   0        0        0      958 2023-04-23 19:57:27.626635 Sphinx-7.0.0rc1/tests/test_ext_githubpages.py
+-rw-r--r--   0        0        0     7667 2023-04-23 19:57:27.626635 Sphinx-7.0.0rc1/tests/test_ext_graphviz.py
+-rw-r--r--   0        0        0      850 2023-04-23 19:57:27.626635 Sphinx-7.0.0rc1/tests/test_ext_ifconfig.py
+-rw-r--r--   0        0        0     1038 2023-04-23 19:57:27.627705 Sphinx-7.0.0rc1/tests/test_ext_imgconverter.py
+-rw-r--r--   0        0        0      609 2023-04-23 19:57:27.627705 Sphinx-7.0.0rc1/tests/test_ext_imgmockconverter.py
+-rw-r--r--   0        0        0    10579 2023-04-23 19:57:27.627705 Sphinx-7.0.0rc1/tests/test_ext_inheritance_diagram.py
+-rw-r--r--   0        0        0    21393 2023-04-23 19:57:27.627705 Sphinx-7.0.0rc1/tests/test_ext_intersphinx.py
+-rw-r--r--   0        0        0    13142 2023-04-23 19:57:27.628705 Sphinx-7.0.0rc1/tests/test_ext_math.py
+-rw-r--r--   0        0        0     6912 2023-04-23 19:57:27.628705 Sphinx-7.0.0rc1/tests/test_ext_napoleon.py
+-rw-r--r--   0        0        0    70796 2023-04-23 19:57:27.628705 Sphinx-7.0.0rc1/tests/test_ext_napoleon_docstring.py
+-rw-r--r--   0        0        0     3878 2023-04-23 19:57:27.629705 Sphinx-7.0.0rc1/tests/test_ext_todo.py
+-rw-r--r--   0        0        0     5467 2023-04-23 19:57:27.629705 Sphinx-7.0.0rc1/tests/test_ext_viewcode.py
+-rw-r--r--   0        0        0      857 2023-04-23 19:57:27.629705 Sphinx-7.0.0rc1/tests/test_extension.py
+-rw-r--r--   0        0        0     3563 2023-04-23 19:57:27.629705 Sphinx-7.0.0rc1/tests/test_highlighting.py
+-rw-r--r--   0        0        0    49439 2023-04-23 19:57:27.629705 Sphinx-7.0.0rc1/tests/test_intl.py
+-rw-r--r--   0        0        0     2551 2023-04-23 19:57:27.630705 Sphinx-7.0.0rc1/tests/test_locale.py
+-rw-r--r--   0        0        0    22328 2023-04-23 19:57:27.630705 Sphinx-7.0.0rc1/tests/test_markup.py
+-rw-r--r--   0        0        0     1931 2023-04-23 19:57:27.630705 Sphinx-7.0.0rc1/tests/test_metadata.py
+-rw-r--r--   0        0        0     2459 2023-04-23 19:57:27.631706 Sphinx-7.0.0rc1/tests/test_parser.py
+-rw-r--r--   0        0        0     2573 2023-04-23 19:57:27.631706 Sphinx-7.0.0rc1/tests/test_project.py
+-rw-r--r--   0        0        0     6918 2023-04-23 19:57:27.631706 Sphinx-7.0.0rc1/tests/test_pycode.py
+-rw-r--r--   0        0        0     2835 2023-04-23 19:57:27.631706 Sphinx-7.0.0rc1/tests/test_pycode_ast.py
+-rw-r--r--   0        0        0    18264 2023-04-23 19:57:27.632705 Sphinx-7.0.0rc1/tests/test_pycode_parser.py
+-rw-r--r--   0        0        0     7347 2023-04-23 19:57:27.632705 Sphinx-7.0.0rc1/tests/test_quickstart.py
+-rw-r--r--   0        0        0     2570 2023-04-23 19:57:27.632705 Sphinx-7.0.0rc1/tests/test_roles.py
+-rw-r--r--   0        0        0    11627 2023-04-23 19:57:27.632705 Sphinx-7.0.0rc1/tests/test_search.py
+-rw-r--r--   0        0        0     3747 2023-04-23 19:57:27.632705 Sphinx-7.0.0rc1/tests/test_smartquotes.py
+-rw-r--r--   0        0        0     1435 2023-04-23 19:57:27.633705 Sphinx-7.0.0rc1/tests/test_templating.py
+-rw-r--r--   0        0        0     4312 2023-04-26 16:05:03.832456 Sphinx-7.0.0rc1/tests/test_theming.py
+-rw-r--r--   0        0        0     1843 2023-04-23 19:57:27.633705 Sphinx-7.0.0rc1/tests/test_toctree.py
+-rw-r--r--   0        0        0     2231 2023-04-23 19:57:27.633705 Sphinx-7.0.0rc1/tests/test_transforms_post_transforms.py
+-rw-r--r--   0        0        0     1324 2023-04-23 19:57:27.633705 Sphinx-7.0.0rc1/tests/test_transforms_post_transforms_code.py
+-rw-r--r--   0        0        0     2799 2023-04-23 19:57:27.634705 Sphinx-7.0.0rc1/tests/test_util.py
+-rw-r--r--   0        0        0     3065 2023-04-23 19:57:27.634705 Sphinx-7.0.0rc1/tests/test_util_display.py
+-rw-r--r--   0        0        0     3032 2023-04-23 19:57:27.634705 Sphinx-7.0.0rc1/tests/test_util_docstrings.py
+-rw-r--r--   0        0        0     2647 2023-04-23 19:57:27.635341 Sphinx-7.0.0rc1/tests/test_util_docutils.py
+-rw-r--r--   0        0        0     3800 2023-04-23 19:57:27.635341 Sphinx-7.0.0rc1/tests/test_util_fileutil.py
+-rw-r--r--   0        0        0     8627 2023-04-27 00:28:57.465794 Sphinx-7.0.0rc1/tests/test_util_i18n.py
+-rw-r--r--   0        0        0     2653 2023-04-23 19:57:27.635341 Sphinx-7.0.0rc1/tests/test_util_images.py
+-rw-r--r--   0        0        0    26901 2023-04-23 19:57:27.636377 Sphinx-7.0.0rc1/tests/test_util_inspect.py
+-rw-r--r--   0        0        0     4032 2023-04-23 19:57:27.636377 Sphinx-7.0.0rc1/tests/test_util_inventory.py
+-rw-r--r--   0        0        0    13459 2023-04-23 19:57:27.636377 Sphinx-7.0.0rc1/tests/test_util_logging.py
+-rw-r--r--   0        0        0     7180 2023-04-23 19:57:27.637384 Sphinx-7.0.0rc1/tests/test_util_matching.py
+-rw-r--r--   0        0        0     7464 2023-04-23 19:57:27.637384 Sphinx-7.0.0rc1/tests/test_util_nodes.py
+-rw-r--r--   0        0        0     4556 2023-04-23 19:57:27.637384 Sphinx-7.0.0rc1/tests/test_util_rst.py
+-rw-r--r--   0        0        0      952 2023-04-23 19:57:27.637384 Sphinx-7.0.0rc1/tests/test_util_template.py
+-rw-r--r--   0        0        0    22811 2023-04-23 19:57:27.637384 Sphinx-7.0.0rc1/tests/test_util_typing.py
+-rw-r--r--   0        0        0     3561 2023-04-23 19:57:27.638376 Sphinx-7.0.0rc1/tests/test_versioning.py
+-rw-r--r--   0        0        0     1065 2023-04-23 19:57:27.638376 Sphinx-7.0.0rc1/tests/test_writer_latex.py
+-rw-r--r--   0        0        0     1859 2023-04-23 19:57:27.638376 Sphinx-7.0.0rc1/tests/typing_test_data.py
+-rw-r--r--   0        0        0     1654 2023-04-23 19:57:27.638376 Sphinx-7.0.0rc1/tests/utils.py
+-rw-r--r--   0        0        0      992 2023-04-23 19:57:27.639377 Sphinx-7.0.0rc1/tox.ini
+-rw-r--r--   0        0        0      227 2023-04-23 19:57:27.639377 Sphinx-7.0.0rc1/utils/CHANGES_template
+-rw-r--r--   0        0        0        0 2023-04-23 19:57:27.639377 Sphinx-7.0.0rc1/utils/__init__.py
+-rw-r--r--   0        0        0     8282 2023-04-23 19:57:27.640377 Sphinx-7.0.0rc1/utils/babel_runner.py
+-rw-r--r--   0        0        0      296 2023-04-25 10:59:46.885153 Sphinx-7.0.0rc1/utils/bump_docker.sh
+-rw-r--r--   0        0        0     5808 2023-04-28 11:31:18.602669 Sphinx-7.0.0rc1/utils/bump_version.py
+-rw-r--r--   0        0        0     1730 2023-04-23 19:57:27.640377 Sphinx-7.0.0rc1/utils/release-checklist
+-rw-r--r--   0        0        0     6141 1970-01-01 00:00:00.000000 Sphinx-7.0.0rc1/PKG-INFO
```

### Comparing `Sphinx-7.0.0/AUTHORS` & `Sphinx-7.0.0rc1/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -89,7 +89,16 @@
 * Thomas Waldmann -- apidoc module fixes
 * Tim Hoffmann -- theme improvements
 * Vince Salvino -- JavaScript search improvements
 * Will Maier -- directory HTML builder
 * Zac Hatfield-Dodds -- doctest reporting improvements, intersphinx performance
 
 Many thanks for all contributions!
+
+Included software
+=================
+
+There are also a few modules or functions incorporated from other
+authors and projects:
+
+* sphinx.util.jsdump uses the basestring encoding from simplejson,
+  written by Bob Ippolito, released under the MIT license
```

### Comparing `Sphinx-7.0.0/CHANGES` & `Sphinx-7.0.0rc1/CHANGES`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-Release 7.0.0 (released Apr 29, 2023)
-=====================================
+Release 7.0.0 (in development)
+==============================
+
+Dependencies
+------------
 
 Incompatible changes
 --------------------
 
 * #11359: Remove long-deprecated aliases for ``MecabSplitter`` and
   ``DefaultSplitter`` in ``sphinx.search.ja``.
 * #11360: Remove deprecated ``make_old_id`` functions in domain object
@@ -25,14 +28,26 @@
 * #11381: Remove deprecated ``style`` key for HTML templates.
 * #11382: Remove deprecated ``sphinx.writers.latex.LaTeXTranslator.docclasses``
   attribute.
 * #11383: Remove deprecated ``sphinx.builders.html.html5_ready`` and
   ``sphinx.builders.html.HTMLTranslator`` attributes.
 * #11385: Remove support for HTML 4 output.
 
+Deprecated
+----------
+
+Features added
+--------------
+
+Bugs fixed
+----------
+
+Testing
+--------
+
 Release 6.2.1 (released Apr 25, 2023)
 =====================================
 
 Bugs fixed
 ----------
 
 * #11355: Revert the default type of :confval:`nitpick_ignore` and
```

### Comparing `Sphinx-7.0.0/CODE_OF_CONDUCT` & `Sphinx-7.0.0rc1/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/EXAMPLES` & `Sphinx-7.0.0rc1/EXAMPLES`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/LICENSE` & `Sphinx-7.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/README.rst` & `Sphinx-7.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/Makefile` & `Sphinx-7.0.0rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/bookcover.png` & `Sphinx-7.0.0rc1/doc/_static/bookcover.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/conf.py.txt` & `Sphinx-7.0.0rc1/doc/_static/conf.py.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/favicon.svg` & `Sphinx-7.0.0rc1/doc/_static/favicon.svg`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/more.png` & `Sphinx-7.0.0rc1/doc/_static/more.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/sphinx.png` & `Sphinx-7.0.0rc1/doc/_static/sphinx.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/agogo.png` & `Sphinx-7.0.0rc1/doc/_static/themes/agogo.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/alabaster.png` & `Sphinx-7.0.0rc1/doc/_static/themes/alabaster.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/bizstyle.png` & `Sphinx-7.0.0rc1/doc/_static/themes/bizstyle.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/classic.png` & `Sphinx-7.0.0rc1/doc/_static/themes/classic.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/fullsize/agogo.png` & `Sphinx-7.0.0rc1/doc/_static/themes/fullsize/agogo.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/fullsize/alabaster.png` & `Sphinx-7.0.0rc1/doc/_static/themes/fullsize/alabaster.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/fullsize/bizstyle.png` & `Sphinx-7.0.0rc1/doc/_static/themes/fullsize/bizstyle.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/fullsize/classic.png` & `Sphinx-7.0.0rc1/doc/_static/themes/fullsize/classic.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/fullsize/haiku.png` & `Sphinx-7.0.0rc1/doc/_static/themes/fullsize/haiku.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/fullsize/nature.png` & `Sphinx-7.0.0rc1/doc/_static/themes/fullsize/nature.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/fullsize/pyramid.png` & `Sphinx-7.0.0rc1/doc/_static/themes/fullsize/pyramid.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/fullsize/scrolls.png` & `Sphinx-7.0.0rc1/doc/_static/themes/fullsize/scrolls.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/fullsize/sphinx_rtd_theme.png` & `Sphinx-7.0.0rc1/doc/_static/themes/fullsize/sphinx_rtd_theme.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/fullsize/sphinxdoc.png` & `Sphinx-7.0.0rc1/doc/_static/themes/fullsize/sphinxdoc.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/fullsize/traditional.png` & `Sphinx-7.0.0rc1/doc/_static/themes/fullsize/traditional.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/haiku.png` & `Sphinx-7.0.0rc1/doc/_static/themes/haiku.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/nature.png` & `Sphinx-7.0.0rc1/doc/_static/themes/nature.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/pyramid.png` & `Sphinx-7.0.0rc1/doc/_static/themes/pyramid.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/scrolls.png` & `Sphinx-7.0.0rc1/doc/_static/themes/scrolls.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/sphinx_rtd_theme.png` & `Sphinx-7.0.0rc1/doc/_static/themes/sphinx_rtd_theme.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/sphinxdoc.png` & `Sphinx-7.0.0rc1/doc/_static/themes/sphinxdoc.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/themes/traditional.png` & `Sphinx-7.0.0rc1/doc/_static/themes/traditional.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/translation.png` & `Sphinx-7.0.0rc1/doc/_static/translation.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/translation.svg` & `Sphinx-7.0.0rc1/doc/_static/translation.svg`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/tutorial/lumache-autosummary.png` & `Sphinx-7.0.0rc1/doc/_static/tutorial/lumache-autosummary.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/tutorial/lumache-first-light.png` & `Sphinx-7.0.0rc1/doc/_static/tutorial/lumache-first-light.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/tutorial/lumache-furo.png` & `Sphinx-7.0.0rc1/doc/_static/tutorial/lumache-furo.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/tutorial/lumache-py-function-full.png` & `Sphinx-7.0.0rc1/doc/_static/tutorial/lumache-py-function-full.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_static/tutorial/lumache-py-function.png` & `Sphinx-7.0.0rc1/doc/_static/tutorial/lumache-py-function.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_themes/sphinx13/layout.html` & `Sphinx-7.0.0rc1/doc/_themes/sphinx13/layout.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_themes/sphinx13/static/sphinx13.css` & `Sphinx-7.0.0rc1/doc/_themes/sphinx13/static/sphinx13.css`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/_themes/sphinx13/static/sphinxheader.png` & `Sphinx-7.0.0rc1/doc/_themes/sphinx13/static/sphinxheader.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/conf.py` & `Sphinx-7.0.0rc1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/development/builders.rst` & `Sphinx-7.0.0rc1/doc/development/builders.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/development/index.rst` & `Sphinx-7.0.0rc1/doc/development/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/development/overview.rst` & `Sphinx-7.0.0rc1/doc/development/overview.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/development/templating.rst` & `Sphinx-7.0.0rc1/doc/development/templating.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/development/theming.rst` & `Sphinx-7.0.0rc1/doc/development/theming.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/development/tutorials/autodoc_ext.rst` & `Sphinx-7.0.0rc1/doc/development/tutorials/autodoc_ext.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/development/tutorials/examples/autodoc_intenum.py` & `Sphinx-7.0.0rc1/doc/development/tutorials/examples/autodoc_intenum.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/development/tutorials/examples/recipe.py` & `Sphinx-7.0.0rc1/doc/development/tutorials/examples/recipe.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/development/tutorials/examples/todo.py` & `Sphinx-7.0.0rc1/doc/development/tutorials/examples/todo.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/development/tutorials/helloworld.rst` & `Sphinx-7.0.0rc1/doc/development/tutorials/helloworld.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/development/tutorials/recipe.rst` & `Sphinx-7.0.0rc1/doc/development/tutorials/recipe.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/development/tutorials/todo.rst` & `Sphinx-7.0.0rc1/doc/development/tutorials/todo.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/extdev/appapi.rst` & `Sphinx-7.0.0rc1/doc/extdev/appapi.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/extdev/builderapi.rst` & `Sphinx-7.0.0rc1/doc/extdev/builderapi.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/extdev/deprecated.rst` & `Sphinx-7.0.0rc1/doc/extdev/deprecated.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/extdev/domainapi.rst` & `Sphinx-7.0.0rc1/doc/extdev/domainapi.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/extdev/envapi.rst` & `Sphinx-7.0.0rc1/doc/extdev/envapi.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/extdev/i18n.rst` & `Sphinx-7.0.0rc1/doc/extdev/i18n.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/extdev/index.rst` & `Sphinx-7.0.0rc1/doc/extdev/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/extdev/logging.rst` & `Sphinx-7.0.0rc1/doc/extdev/logging.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/extdev/markupapi.rst` & `Sphinx-7.0.0rc1/doc/extdev/markupapi.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/extdev/nodes.rst` & `Sphinx-7.0.0rc1/doc/extdev/nodes.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/extdev/parserapi.rst` & `Sphinx-7.0.0rc1/doc/extdev/parserapi.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/extdev/utils.rst` & `Sphinx-7.0.0rc1/doc/extdev/utils.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/faq.rst` & `Sphinx-7.0.0rc1/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/glossary.rst` & `Sphinx-7.0.0rc1/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/index.rst` & `Sphinx-7.0.0rc1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/internals/contributing.rst` & `Sphinx-7.0.0rc1/doc/internals/contributing.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/internals/organization.rst` & `Sphinx-7.0.0rc1/doc/internals/organization.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/internals/release-process.rst` & `Sphinx-7.0.0rc1/doc/internals/release-process.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/latex.rst` & `Sphinx-7.0.0rc1/doc/latex.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/make.bat` & `Sphinx-7.0.0rc1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/man/sphinx-apidoc.rst` & `Sphinx-7.0.0rc1/doc/man/sphinx-apidoc.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/man/sphinx-autogen.rst` & `Sphinx-7.0.0rc1/doc/man/sphinx-autogen.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/man/sphinx-build.rst` & `Sphinx-7.0.0rc1/doc/man/sphinx-build.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/man/sphinx-quickstart.rst` & `Sphinx-7.0.0rc1/doc/man/sphinx-quickstart.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/support.rst` & `Sphinx-7.0.0rc1/doc/support.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/tutorial/automatic-doc-generation.rst` & `Sphinx-7.0.0rc1/doc/tutorial/automatic-doc-generation.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/tutorial/deploying.rst` & `Sphinx-7.0.0rc1/doc/tutorial/deploying.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/tutorial/describing-code.rst` & `Sphinx-7.0.0rc1/doc/tutorial/describing-code.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/tutorial/first-steps.rst` & `Sphinx-7.0.0rc1/doc/tutorial/first-steps.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/tutorial/getting-started.rst` & `Sphinx-7.0.0rc1/doc/tutorial/getting-started.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/tutorial/index.rst` & `Sphinx-7.0.0rc1/doc/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/tutorial/more-sphinx-customization.rst` & `Sphinx-7.0.0rc1/doc/tutorial/more-sphinx-customization.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/tutorial/narrative-documentation.rst` & `Sphinx-7.0.0rc1/doc/tutorial/narrative-documentation.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/advanced/intl.rst` & `Sphinx-7.0.0rc1/doc/usage/advanced/intl.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/advanced/websupport/api.rst` & `Sphinx-7.0.0rc1/doc/usage/advanced/websupport/api.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/advanced/websupport/quickstart.rst` & `Sphinx-7.0.0rc1/doc/usage/advanced/websupport/quickstart.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/advanced/websupport/searchadapters.rst` & `Sphinx-7.0.0rc1/doc/usage/advanced/websupport/searchadapters.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/advanced/websupport/storagebackends.rst` & `Sphinx-7.0.0rc1/doc/usage/advanced/websupport/storagebackends.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/builders/index.rst` & `Sphinx-7.0.0rc1/doc/usage/builders/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/configuration.rst` & `Sphinx-7.0.0rc1/doc/usage/configuration.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/autodoc.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/autodoc.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/autosectionlabel.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/autosectionlabel.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/autosummary.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/autosummary.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/coverage.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/coverage.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/doctest.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/doctest.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/example_google.py` & `Sphinx-7.0.0rc1/doc/usage/extensions/example_google.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/example_numpy.py` & `Sphinx-7.0.0rc1/doc/usage/extensions/example_numpy.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/extlinks.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/extlinks.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/graphviz.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/graphviz.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/ifconfig.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/ifconfig.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/imgconverter.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/imgconverter.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/index.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/inheritance.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/inheritance.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/intersphinx.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/intersphinx.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/linkcode.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/linkcode.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/math.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/math.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/napoleon.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/napoleon.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/todo.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/todo.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/extensions/viewcode.rst` & `Sphinx-7.0.0rc1/doc/usage/extensions/viewcode.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/index.rst` & `Sphinx-7.0.0rc1/doc/usage/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/installation.rst` & `Sphinx-7.0.0rc1/doc/usage/installation.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/markdown.rst` & `Sphinx-7.0.0rc1/doc/usage/markdown.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/quickstart.rst` & `Sphinx-7.0.0rc1/doc/usage/quickstart.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/restructuredtext/basics.rst` & `Sphinx-7.0.0rc1/doc/usage/restructuredtext/basics.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/restructuredtext/directives.rst` & `Sphinx-7.0.0rc1/doc/usage/restructuredtext/directives.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/restructuredtext/domains.rst` & `Sphinx-7.0.0rc1/doc/usage/restructuredtext/domains.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/restructuredtext/field-lists.rst` & `Sphinx-7.0.0rc1/doc/usage/restructuredtext/field-lists.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/restructuredtext/index.rst` & `Sphinx-7.0.0rc1/doc/usage/restructuredtext/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/restructuredtext/roles.rst` & `Sphinx-7.0.0rc1/doc/usage/restructuredtext/roles.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/doc/usage/theming.rst` & `Sphinx-7.0.0rc1/doc/usage/theming.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/pyproject.toml` & `Sphinx-7.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/__init__.py` & `Sphinx-7.0.0rc1/sphinx/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,26 +15,26 @@
     warnings.filterwarnings('default', category=RemovedInNextVersionWarning)
 # docutils.io using mode='rU' for open
 warnings.filterwarnings('ignore', "'U' mode is deprecated",
                         DeprecationWarning, module='docutils.io')
 warnings.filterwarnings('ignore', 'The frontend.Option class .*',
                         DeprecationWarning, module='docutils.frontend')
 
-__version__ = '7.0.0'
+__version__ = '7.0.0rc1'
 __display_version__ = __version__  # used for command line version
 
 #: Version info for better programmatic use.
 #:
 #: A tuple of five elements; for Sphinx version 1.2.1 beta 3 this would be
 #: ``(1, 2, 1, 'beta', 3)``. The fourth element can be one of: ``alpha``,
 #: ``beta``, ``rc``, ``final``. ``final`` always has 0 as the last element.
 #:
 #: .. versionadded:: 1.2
 #:    Before version 1.2, check the string ``sphinx.__version__``.
-version_info = (7, 0, 0, 'final', 0)
+version_info = (7, 0, 0, 'rc', 1)
 
 package_dir = path.abspath(path.dirname(__file__))
 
 _in_development = False
 if _in_development:
     # Only import subprocess if needed
     import subprocess
```

### Comparing `Sphinx-7.0.0/sphinx/addnodes.py` & `Sphinx-7.0.0rc1/sphinx/addnodes.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/application.py` & `Sphinx-7.0.0rc1/sphinx/application.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/__init__.py` & `Sphinx-7.0.0rc1/sphinx/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/_epub_base.py` & `Sphinx-7.0.0rc1/sphinx/builders/_epub_base.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/changes.py` & `Sphinx-7.0.0rc1/sphinx/builders/changes.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/dirhtml.py` & `Sphinx-7.0.0rc1/sphinx/builders/dirhtml.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/dummy.py` & `Sphinx-7.0.0rc1/sphinx/builders/dummy.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/epub3.py` & `Sphinx-7.0.0rc1/sphinx/builders/epub3.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/gettext.py` & `Sphinx-7.0.0rc1/sphinx/builders/gettext.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/html/__init__.py` & `Sphinx-7.0.0rc1/sphinx/builders/html/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/html/transforms.py` & `Sphinx-7.0.0rc1/sphinx/builders/html/transforms.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/latex/__init__.py` & `Sphinx-7.0.0rc1/sphinx/builders/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/latex/constants.py` & `Sphinx-7.0.0rc1/sphinx/builders/latex/constants.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/latex/nodes.py` & `Sphinx-7.0.0rc1/sphinx/builders/latex/nodes.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/latex/theming.py` & `Sphinx-7.0.0rc1/sphinx/builders/latex/theming.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/latex/transforms.py` & `Sphinx-7.0.0rc1/sphinx/builders/latex/transforms.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/latex/util.py` & `Sphinx-7.0.0rc1/sphinx/builders/latex/util.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/linkcheck.py` & `Sphinx-7.0.0rc1/sphinx/builders/linkcheck.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/manpage.py` & `Sphinx-7.0.0rc1/sphinx/builders/manpage.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/singlehtml.py` & `Sphinx-7.0.0rc1/sphinx/builders/singlehtml.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/texinfo.py` & `Sphinx-7.0.0rc1/sphinx/builders/texinfo.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/text.py` & `Sphinx-7.0.0rc1/sphinx/builders/text.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/builders/xml.py` & `Sphinx-7.0.0rc1/sphinx/builders/xml.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/cmd/build.py` & `Sphinx-7.0.0rc1/sphinx/cmd/build.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/cmd/make_mode.py` & `Sphinx-7.0.0rc1/sphinx/cmd/make_mode.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/cmd/quickstart.py` & `Sphinx-7.0.0rc1/sphinx/cmd/quickstart.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/config.py` & `Sphinx-7.0.0rc1/sphinx/config.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/deprecation.py` & `Sphinx-7.0.0rc1/sphinx/deprecation.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/directives/__init__.py` & `Sphinx-7.0.0rc1/sphinx/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/directives/code.py` & `Sphinx-7.0.0rc1/sphinx/directives/code.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/directives/other.py` & `Sphinx-7.0.0rc1/sphinx/directives/other.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/directives/patches.py` & `Sphinx-7.0.0rc1/sphinx/directives/patches.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/domains/__init__.py` & `Sphinx-7.0.0rc1/sphinx/domains/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/domains/c.py` & `Sphinx-7.0.0rc1/sphinx/domains/c.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/domains/changeset.py` & `Sphinx-7.0.0rc1/sphinx/domains/changeset.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/domains/citation.py` & `Sphinx-7.0.0rc1/sphinx/domains/citation.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/domains/cpp.py` & `Sphinx-7.0.0rc1/sphinx/domains/cpp.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/domains/index.py` & `Sphinx-7.0.0rc1/sphinx/domains/index.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/domains/javascript.py` & `Sphinx-7.0.0rc1/sphinx/domains/javascript.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/domains/math.py` & `Sphinx-7.0.0rc1/sphinx/domains/math.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/domains/python.py` & `Sphinx-7.0.0rc1/sphinx/domains/python.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/domains/rst.py` & `Sphinx-7.0.0rc1/sphinx/domains/rst.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/domains/std.py` & `Sphinx-7.0.0rc1/sphinx/domains/std.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/environment/__init__.py` & `Sphinx-7.0.0rc1/sphinx/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/environment/adapters/indexentries.py` & `Sphinx-7.0.0rc1/sphinx/environment/adapters/indexentries.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/environment/adapters/toctree.py` & `Sphinx-7.0.0rc1/sphinx/environment/adapters/toctree.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/environment/collectors/__init__.py` & `Sphinx-7.0.0rc1/sphinx/environment/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/environment/collectors/asset.py` & `Sphinx-7.0.0rc1/sphinx/environment/collectors/asset.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/environment/collectors/dependencies.py` & `Sphinx-7.0.0rc1/sphinx/environment/collectors/dependencies.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/environment/collectors/metadata.py` & `Sphinx-7.0.0rc1/sphinx/environment/collectors/metadata.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/environment/collectors/title.py` & `Sphinx-7.0.0rc1/sphinx/environment/collectors/title.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/environment/collectors/toctree.py` & `Sphinx-7.0.0rc1/sphinx/environment/collectors/toctree.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/errors.py` & `Sphinx-7.0.0rc1/sphinx/errors.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/events.py` & `Sphinx-7.0.0rc1/sphinx/events.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/apidoc.py` & `Sphinx-7.0.0rc1/sphinx/ext/apidoc.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/autodoc/__init__.py` & `Sphinx-7.0.0rc1/sphinx/ext/autodoc/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/autodoc/directive.py` & `Sphinx-7.0.0rc1/sphinx/ext/autodoc/directive.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/autodoc/importer.py` & `Sphinx-7.0.0rc1/sphinx/ext/autodoc/importer.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/autodoc/mock.py` & `Sphinx-7.0.0rc1/sphinx/ext/autodoc/mock.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/autodoc/preserve_defaults.py` & `Sphinx-7.0.0rc1/sphinx/ext/autodoc/preserve_defaults.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/autodoc/type_comment.py` & `Sphinx-7.0.0rc1/sphinx/ext/autodoc/type_comment.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/autodoc/typehints.py` & `Sphinx-7.0.0rc1/sphinx/ext/autodoc/typehints.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/autosectionlabel.py` & `Sphinx-7.0.0rc1/sphinx/ext/autosectionlabel.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/autosummary/__init__.py` & `Sphinx-7.0.0rc1/sphinx/ext/autosummary/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/autosummary/generate.py` & `Sphinx-7.0.0rc1/sphinx/ext/autosummary/generate.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/autosummary/templates/autosummary/class.rst` & `Sphinx-7.0.0rc1/sphinx/ext/autosummary/templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/autosummary/templates/autosummary/module.rst` & `Sphinx-7.0.0rc1/sphinx/ext/autosummary/templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/coverage.py` & `Sphinx-7.0.0rc1/sphinx/ext/coverage.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/doctest.py` & `Sphinx-7.0.0rc1/sphinx/ext/doctest.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/duration.py` & `Sphinx-7.0.0rc1/sphinx/ext/duration.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/extlinks.py` & `Sphinx-7.0.0rc1/sphinx/ext/extlinks.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/githubpages.py` & `Sphinx-7.0.0rc1/sphinx/ext/githubpages.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/graphviz.py` & `Sphinx-7.0.0rc1/sphinx/ext/graphviz.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/ifconfig.py` & `Sphinx-7.0.0rc1/sphinx/ext/ifconfig.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/imgconverter.py` & `Sphinx-7.0.0rc1/sphinx/ext/imgconverter.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/imgmath.py` & `Sphinx-7.0.0rc1/sphinx/ext/imgmath.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/inheritance_diagram.py` & `Sphinx-7.0.0rc1/sphinx/ext/inheritance_diagram.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/intersphinx.py` & `Sphinx-7.0.0rc1/sphinx/ext/intersphinx.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/linkcode.py` & `Sphinx-7.0.0rc1/sphinx/ext/linkcode.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/mathjax.py` & `Sphinx-7.0.0rc1/sphinx/ext/mathjax.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/napoleon/__init__.py` & `Sphinx-7.0.0rc1/sphinx/ext/napoleon/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/napoleon/docstring.py` & `Sphinx-7.0.0rc1/sphinx/ext/napoleon/docstring.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/todo.py` & `Sphinx-7.0.0rc1/sphinx/ext/todo.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/ext/viewcode.py` & `Sphinx-7.0.0rc1/sphinx/ext/viewcode.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/extension.py` & `Sphinx-7.0.0rc1/sphinx/extension.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/highlighting.py` & `Sphinx-7.0.0rc1/sphinx/highlighting.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/io.py` & `Sphinx-7.0.0rc1/sphinx/io.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/jinja2glue.py` & `Sphinx-7.0.0rc1/sphinx/jinja2glue.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/__init__.py` & `Sphinx-7.0.0rc1/sphinx/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ar/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/ar/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ar/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/ar/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ar/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/ar/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/bg/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/bg/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/bg/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/bg/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/bn/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/bn/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/bn/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/bn/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/bn/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/bn/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ca/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/ca/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ca/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/ca/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ca/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/ca/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/cak/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/cak/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/cak/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/cak/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/cak/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/cak/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/cs/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/cs/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/cs/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/cs/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/cs/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/cs/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/cy/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/cy/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/cy/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/cy/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/cy/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/cy/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/da/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/da/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/da/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/da/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/da/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/da/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/de/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/de/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/de/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/de/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/de/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/de/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/el/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/el/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/el/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/el/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/el/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/el/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/en_FR/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/en_FR/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/en_FR/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/en_FR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/en_GB/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/en_GB/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/en_GB/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/en_GB/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/en_GB/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/en_GB/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/en_HK/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/en_HK/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/en_HK/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/en_HK/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/eo/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/eo/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/eo/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/eo/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/eo/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/eo/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/es/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/es/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/es/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/es/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/es/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/es/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/et/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/et/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/et/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/et/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/et/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/et/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/eu/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/eu/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/eu/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/eu/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/eu/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/eu/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/fa/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/fa/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/fa/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/fa/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/fa/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/fa/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/fi/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/fi/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/fi/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/fi/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/fi/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/fi/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/fr/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/fr/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/fr/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/fr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/fr/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/fr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/he/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/he/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/he/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/he/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/he/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/he/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/hi/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/hi/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/hi/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/hi/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/hi/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/hi/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/hr/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/hr/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/hr/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/hr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/hr/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/hr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/hu/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/hu/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/hu/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/hu/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/hu/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/hu/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/id/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/id/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/id/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/id/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/id/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/id/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/is/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/is/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/is/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/is/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/is/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/is/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/it/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/it/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/it/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/it/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/it/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/it/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ja/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/ja/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ja/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/ja/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ja/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/ja/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ko/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/ko/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ko/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/ko/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ko/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/ko/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/lt/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/lt/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/lt/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/lt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/lt/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/lt/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/lv/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/lv/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/lv/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/lv/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/lv/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/lv/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/mk/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/mk/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/mk/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/mk/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/mk/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/mk/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ne/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/ne/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ne/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/ne/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ne/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/ne/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/nl/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/nl/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/nl/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/nl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/nl/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/nl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/pl/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/pl/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/pl/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/pl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/pl/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/pl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/pt/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/pt/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/pt/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/pt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/pt/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/pt/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ro/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/ro/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ro/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/ro/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ro/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/ro/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ru/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/ru/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ru/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/ru/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ru/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/ru/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/si/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/si/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/si/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/si/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/si/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/si/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sk/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/sk/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sk/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/sk/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sk/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/sk/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sl/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/sl/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sl/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/sl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sl/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/sl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sphinx.pot` & `Sphinx-7.0.0rc1/sphinx/locale/sphinx.pot`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sq/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/sq/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sq/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/sq/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sq/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/sq/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sr/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/sr/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sr/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/sr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sr/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/sr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sv/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/sv/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sv/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/sv/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/sv/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/sv/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ta/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/ta/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ta/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/ta/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ta/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/ta/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/te/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/te/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/te/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/te/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/tr/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/tr/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/tr/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/tr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/tr/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/tr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ur/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/ur/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/ur/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/ur/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/vi/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/vi/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/vi/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/vi/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/vi/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/vi/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/yue/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/yue/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/yue/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/yue/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.js` & `Sphinx-7.0.0rc1/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.mo` & `Sphinx-7.0.0rc1/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/parsers.py` & `Sphinx-7.0.0rc1/sphinx/parsers.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/project.py` & `Sphinx-7.0.0rc1/sphinx/project.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/pycode/__init__.py` & `Sphinx-7.0.0rc1/sphinx/pycode/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/pycode/ast.py` & `Sphinx-7.0.0rc1/sphinx/pycode/ast.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/pycode/parser.py` & `Sphinx-7.0.0rc1/sphinx/pycode/parser.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/pygments_styles.py` & `Sphinx-7.0.0rc1/sphinx/pygments_styles.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/registry.py` & `Sphinx-7.0.0rc1/sphinx/registry.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/roles.py` & `Sphinx-7.0.0rc1/sphinx/roles.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/__init__.py` & `Sphinx-7.0.0rc1/sphinx/search/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/da.py` & `Sphinx-7.0.0rc1/sphinx/search/da.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/de.py` & `Sphinx-7.0.0rc1/sphinx/search/de.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/en.py` & `Sphinx-7.0.0rc1/sphinx/search/en.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/es.py` & `Sphinx-7.0.0rc1/sphinx/search/es.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/fi.py` & `Sphinx-7.0.0rc1/sphinx/search/fi.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/fr.py` & `Sphinx-7.0.0rc1/sphinx/search/fr.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/hu.py` & `Sphinx-7.0.0rc1/sphinx/search/hu.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/it.py` & `Sphinx-7.0.0rc1/sphinx/search/it.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/ja.py` & `Sphinx-7.0.0rc1/sphinx/search/ja.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/base-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/base-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/danish-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/danish-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/dutch-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/dutch-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/finnish-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/finnish-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/french-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/french-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/german-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/german-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/hungarian-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/hungarian-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/italian-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/italian-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/norwegian-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/norwegian-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/porter-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/porter-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/portuguese-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/portuguese-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/romanian-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/romanian-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/russian-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/russian-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/spanish-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/spanish-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/swedish-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/swedish-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/minified-js/turkish-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/minified-js/turkish-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/nl.py` & `Sphinx-7.0.0rc1/sphinx/search/nl.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/no.py` & `Sphinx-7.0.0rc1/sphinx/search/no.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/base-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/base-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/danish-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/danish-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/dutch-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/dutch-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/finnish-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/finnish-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/french-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/french-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/german-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/german-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/hungarian-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/hungarian-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/italian-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/italian-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/norwegian-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/norwegian-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/porter-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/porter-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/portuguese-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/portuguese-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/romanian-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/romanian-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/russian-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/russian-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/spanish-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/spanish-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/swedish-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/swedish-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/non-minified-js/turkish-stemmer.js` & `Sphinx-7.0.0rc1/sphinx/search/non-minified-js/turkish-stemmer.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/pt.py` & `Sphinx-7.0.0rc1/sphinx/search/pt.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/ro.py` & `Sphinx-7.0.0rc1/sphinx/search/ro.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/ru.py` & `Sphinx-7.0.0rc1/sphinx/search/ru.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/sv.py` & `Sphinx-7.0.0rc1/sphinx/search/sv.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/tr.py` & `Sphinx-7.0.0rc1/sphinx/search/tr.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/search/zh.py` & `Sphinx-7.0.0rc1/sphinx/search/zh.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/apidoc/package.rst_t` & `Sphinx-7.0.0rc1/sphinx/templates/apidoc/package.rst_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/epub3/content.opf_t` & `Sphinx-7.0.0rc1/sphinx/templates/epub3/content.opf_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/epub3/nav.xhtml_t` & `Sphinx-7.0.0rc1/sphinx/templates/epub3/nav.xhtml_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/epub3/toc.ncx_t` & `Sphinx-7.0.0rc1/sphinx/templates/epub3/toc.ncx_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/gettext/message.pot_t` & `Sphinx-7.0.0rc1/sphinx/templates/gettext/message.pot_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/htmlhelp/project.hhc` & `Sphinx-7.0.0rc1/sphinx/templates/htmlhelp/project.hhc`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/htmlhelp/project.hhp` & `Sphinx-7.0.0rc1/sphinx/templates/htmlhelp/project.hhp`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/latex/latex.tex_t` & `Sphinx-7.0.0rc1/sphinx/templates/latex/latex.tex_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/latex/longtable.tex_t` & `Sphinx-7.0.0rc1/sphinx/templates/latex/longtable.tex_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/latex/sphinxmessages.sty_t` & `Sphinx-7.0.0rc1/sphinx/templates/latex/sphinxmessages.sty_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/latex/tabular.tex_t` & `Sphinx-7.0.0rc1/sphinx/templates/latex/tabular.tex_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/latex/tabulary.tex_t` & `Sphinx-7.0.0rc1/sphinx/templates/latex/tabulary.tex_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/quickstart/Makefile.new_t` & `Sphinx-7.0.0rc1/sphinx/templates/quickstart/Makefile.new_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/quickstart/Makefile_t` & `Sphinx-7.0.0rc1/sphinx/templates/quickstart/Makefile_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/quickstart/conf.py_t` & `Sphinx-7.0.0rc1/sphinx/templates/quickstart/conf.py_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/quickstart/make.bat.new_t` & `Sphinx-7.0.0rc1/sphinx/templates/quickstart/make.bat.new_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/quickstart/make.bat_t` & `Sphinx-7.0.0rc1/sphinx/templates/quickstart/make.bat_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/templates/texinfo/Makefile` & `Sphinx-7.0.0rc1/sphinx/templates/texinfo/Makefile`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/testing/comparer.py` & `Sphinx-7.0.0rc1/sphinx/testing/comparer.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/testing/fixtures.py` & `Sphinx-7.0.0rc1/sphinx/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/testing/path.py` & `Sphinx-7.0.0rc1/sphinx/testing/path.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/testing/restructuredtext.py` & `Sphinx-7.0.0rc1/sphinx/testing/restructuredtext.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/testing/util.py` & `Sphinx-7.0.0rc1/sphinx/testing/util.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/LICRcyr2utf8.xdy` & `Sphinx-7.0.0rc1/sphinx/texinputs/LICRcyr2utf8.xdy`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/LICRlatin2utf8.xdy` & `Sphinx-7.0.0rc1/sphinx/texinputs/LICRlatin2utf8.xdy`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/LatinRules.xdy` & `Sphinx-7.0.0rc1/sphinx/texinputs/LatinRules.xdy`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/Makefile_t` & `Sphinx-7.0.0rc1/sphinx/texinputs/Makefile_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/latexmkjarc_t` & `Sphinx-7.0.0rc1/sphinx/texinputs/latexmkjarc_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/latexmkrc_t` & `Sphinx-7.0.0rc1/sphinx/texinputs/latexmkrc_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/make.bat_t` & `Sphinx-7.0.0rc1/sphinx/texinputs/make.bat_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinx.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinx.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinx.xdy` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinx.xdy`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxhowto.cls` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxhowto.cls`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxlatexadmonitions.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexadmonitions.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxlatexcontainers.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexcontainers.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxlatexgraphics.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexgraphics.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxlatexindbibtoc.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexindbibtoc.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxlatexlists.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexlists.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxlatexliterals.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexliterals.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxlatexnumfig.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexnumfig.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxlatexobjects.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexobjects.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxlatexshadowbox.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexshadowbox.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxlatexstyleheadings.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexstyleheadings.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxlatexstylepage.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexstylepage.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxlatexstyletext.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatexstyletext.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxlatextables.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxlatextables.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxmanual.cls` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxmanual.cls`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxoptionsgeometry.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxoptionsgeometry.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxoptionshyperref.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxoptionshyperref.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxpackageboxes.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxpackageboxes.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxpackagecyrillic.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxpackagecyrillic.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs/sphinxpackagefootnote.sty` & `Sphinx-7.0.0rc1/sphinx/texinputs/sphinxpackagefootnote.sty`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/texinputs_win/Makefile_t` & `Sphinx-7.0.0rc1/sphinx/texinputs_win/Makefile_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/agogo/layout.html` & `Sphinx-7.0.0rc1/sphinx/themes/agogo/layout.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/agogo/static/agogo.css_t` & `Sphinx-7.0.0rc1/sphinx/themes/agogo/static/agogo.css_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/changes/versionchanges.html` & `Sphinx-7.0.0rc1/sphinx/themes/basic/changes/versionchanges.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/defindex.html` & `Sphinx-7.0.0rc1/sphinx/themes/basic/defindex.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/domainindex.html` & `Sphinx-7.0.0rc1/sphinx/themes/basic/domainindex.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/genindex-single.html` & `Sphinx-7.0.0rc1/sphinx/themes/basic/genindex-single.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/genindex-split.html` & `Sphinx-7.0.0rc1/sphinx/themes/basic/genindex-split.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/genindex.html` & `Sphinx-7.0.0rc1/sphinx/themes/basic/genindex.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/layout.html` & `Sphinx-7.0.0rc1/sphinx/themes/basic/layout.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/opensearch.xml` & `Sphinx-7.0.0rc1/sphinx/themes/basic/opensearch.xml`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/relations.html` & `Sphinx-7.0.0rc1/sphinx/themes/basic/relations.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/search.html` & `Sphinx-7.0.0rc1/sphinx/themes/basic/search.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/searchbox.html` & `Sphinx-7.0.0rc1/sphinx/themes/basic/searchbox.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/searchfield.html` & `Sphinx-7.0.0rc1/sphinx/themes/basic/searchfield.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/sourcelink.html` & `Sphinx-7.0.0rc1/sphinx/themes/basic/sourcelink.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/static/basic.css_t` & `Sphinx-7.0.0rc1/sphinx/themes/basic/static/basic.css_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/static/doctools.js` & `Sphinx-7.0.0rc1/sphinx/themes/basic/static/doctools.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/static/documentation_options.js_t` & `Sphinx-7.0.0rc1/sphinx/themes/basic/static/documentation_options.js_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/static/language_data.js_t` & `Sphinx-7.0.0rc1/sphinx/themes/basic/static/language_data.js_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/static/searchtools.js` & `Sphinx-7.0.0rc1/sphinx/themes/basic/static/searchtools.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/basic/static/sphinx_highlight.js` & `Sphinx-7.0.0rc1/sphinx/themes/basic/static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/bizstyle/layout.html` & `Sphinx-7.0.0rc1/sphinx/themes/bizstyle/layout.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/bizstyle/static/bizstyle.css_t` & `Sphinx-7.0.0rc1/sphinx/themes/bizstyle/static/bizstyle.css_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/bizstyle/static/bizstyle.js_t` & `Sphinx-7.0.0rc1/sphinx/themes/bizstyle/static/bizstyle.js_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/bizstyle/static/css3-mediaqueries.js` & `Sphinx-7.0.0rc1/sphinx/themes/bizstyle/static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/bizstyle/static/css3-mediaqueries_src.js` & `Sphinx-7.0.0rc1/sphinx/themes/bizstyle/static/css3-mediaqueries_src.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/classic/layout.html` & `Sphinx-7.0.0rc1/sphinx/themes/classic/layout.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/classic/static/classic.css_t` & `Sphinx-7.0.0rc1/sphinx/themes/classic/static/classic.css_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/classic/static/sidebar.js_t` & `Sphinx-7.0.0rc1/sphinx/themes/classic/static/sidebar.js_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/classic/theme.conf` & `Sphinx-7.0.0rc1/sphinx/themes/classic/theme.conf`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/epub/epub-cover.html` & `Sphinx-7.0.0rc1/sphinx/themes/epub/epub-cover.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/epub/layout.html` & `Sphinx-7.0.0rc1/sphinx/themes/epub/layout.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/epub/static/epub.css_t` & `Sphinx-7.0.0rc1/sphinx/themes/epub/static/epub.css_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/haiku/layout.html` & `Sphinx-7.0.0rc1/sphinx/themes/haiku/layout.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/haiku/static/alert_info_32.png` & `Sphinx-7.0.0rc1/sphinx/themes/haiku/static/alert_info_32.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/haiku/static/alert_warning_32.png` & `Sphinx-7.0.0rc1/sphinx/themes/haiku/static/alert_warning_32.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/haiku/static/haiku.css_t` & `Sphinx-7.0.0rc1/sphinx/themes/haiku/static/haiku.css_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/nature/static/nature.css_t` & `Sphinx-7.0.0rc1/sphinx/themes/nature/static/nature.css_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/nonav/layout.html` & `Sphinx-7.0.0rc1/sphinx/themes/nonav/layout.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/nonav/static/nonav.css_t` & `Sphinx-7.0.0rc1/sphinx/themes/nonav/static/nonav.css_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/pyramid/layout.html` & `Sphinx-7.0.0rc1/sphinx/themes/pyramid/layout.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/pyramid/static/dialog-note.png` & `Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/dialog-note.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/pyramid/static/dialog-seealso.png` & `Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/dialog-seealso.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/pyramid/static/dialog-todo.png` & `Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/dialog-todo.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/pyramid/static/dialog-topic.png` & `Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/dialog-topic.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/pyramid/static/dialog-warning.png` & `Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/dialog-warning.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/pyramid/static/epub.css_t` & `Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/epub.css_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/pyramid/static/ie6.css` & `Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/ie6.css`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/pyramid/static/pyramid.css_t` & `Sphinx-7.0.0rc1/sphinx/themes/pyramid/static/pyramid.css_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/scrolls/artwork/logo.svg` & `Sphinx-7.0.0rc1/sphinx/themes/scrolls/artwork/logo.svg`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/scrolls/layout.html` & `Sphinx-7.0.0rc1/sphinx/themes/scrolls/layout.html`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/scrolls/static/darkmetal.png` & `Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/darkmetal.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/scrolls/static/logo.png` & `Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/logo.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/scrolls/static/metal.png` & `Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/metal.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/scrolls/static/scrolls.css_t` & `Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/scrolls.css_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/scrolls/static/theme_extras.js` & `Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/theme_extras.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/scrolls/static/watermark.png` & `Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/watermark.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/scrolls/static/watermark_blur.png` & `Sphinx-7.0.0rc1/sphinx/themes/scrolls/static/watermark_blur.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/sphinxdoc/static/sphinxdoc.css_t` & `Sphinx-7.0.0rc1/sphinx/themes/sphinxdoc/static/sphinxdoc.css_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/themes/traditional/static/traditional.css_t` & `Sphinx-7.0.0rc1/sphinx/themes/traditional/static/traditional.css_t`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/theming.py` & `Sphinx-7.0.0rc1/sphinx/theming.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/transforms/__init__.py` & `Sphinx-7.0.0rc1/sphinx/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/transforms/compact_bullet_list.py` & `Sphinx-7.0.0rc1/sphinx/transforms/compact_bullet_list.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/transforms/i18n.py` & `Sphinx-7.0.0rc1/sphinx/transforms/i18n.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/transforms/post_transforms/__init__.py` & `Sphinx-7.0.0rc1/sphinx/transforms/post_transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/transforms/post_transforms/code.py` & `Sphinx-7.0.0rc1/sphinx/transforms/post_transforms/code.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/transforms/post_transforms/images.py` & `Sphinx-7.0.0rc1/sphinx/transforms/post_transforms/images.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/transforms/references.py` & `Sphinx-7.0.0rc1/sphinx/transforms/references.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/__init__.py` & `Sphinx-7.0.0rc1/sphinx/util/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/cfamily.py` & `Sphinx-7.0.0rc1/sphinx/util/cfamily.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/console.py` & `Sphinx-7.0.0rc1/sphinx/util/console.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/display.py` & `Sphinx-7.0.0rc1/sphinx/util/display.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/docfields.py` & `Sphinx-7.0.0rc1/sphinx/util/docfields.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/docstrings.py` & `Sphinx-7.0.0rc1/sphinx/util/docstrings.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/docutils.py` & `Sphinx-7.0.0rc1/sphinx/util/docutils.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/exceptions.py` & `Sphinx-7.0.0rc1/sphinx/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/fileutil.py` & `Sphinx-7.0.0rc1/sphinx/util/fileutil.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/http_date.py` & `Sphinx-7.0.0rc1/sphinx/util/http_date.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/i18n.py` & `Sphinx-7.0.0rc1/sphinx/util/i18n.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/images.py` & `Sphinx-7.0.0rc1/sphinx/util/images.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/inspect.py` & `Sphinx-7.0.0rc1/sphinx/util/inspect.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/inventory.py` & `Sphinx-7.0.0rc1/sphinx/util/inventory.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/logging.py` & `Sphinx-7.0.0rc1/sphinx/util/logging.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/matching.py` & `Sphinx-7.0.0rc1/sphinx/util/matching.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/math.py` & `Sphinx-7.0.0rc1/sphinx/util/math.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/nodes.py` & `Sphinx-7.0.0rc1/sphinx/util/nodes.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/osutil.py` & `Sphinx-7.0.0rc1/sphinx/util/osutil.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/parallel.py` & `Sphinx-7.0.0rc1/sphinx/util/parallel.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/png.py` & `Sphinx-7.0.0rc1/sphinx/util/png.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/requests.py` & `Sphinx-7.0.0rc1/sphinx/util/requests.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/rst.py` & `Sphinx-7.0.0rc1/sphinx/util/rst.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/tags.py` & `Sphinx-7.0.0rc1/sphinx/util/tags.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/template.py` & `Sphinx-7.0.0rc1/sphinx/util/template.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/texescape.py` & `Sphinx-7.0.0rc1/sphinx/util/texescape.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/util/typing.py` & `Sphinx-7.0.0rc1/sphinx/util/typing.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/versioning.py` & `Sphinx-7.0.0rc1/sphinx/versioning.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/writers/html.py` & `Sphinx-7.0.0rc1/sphinx/writers/html.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/writers/html5.py` & `Sphinx-7.0.0rc1/sphinx/writers/html5.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/writers/latex.py` & `Sphinx-7.0.0rc1/sphinx/writers/latex.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/writers/manpage.py` & `Sphinx-7.0.0rc1/sphinx/writers/manpage.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/writers/texinfo.py` & `Sphinx-7.0.0rc1/sphinx/writers/texinfo.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/writers/text.py` & `Sphinx-7.0.0rc1/sphinx/writers/text.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/sphinx/writers/xml.py` & `Sphinx-7.0.0rc1/sphinx/writers/xml.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/certs/cert.pem` & `Sphinx-7.0.0rc1/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/conftest.py` & `Sphinx-7.0.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/js/searchtools.js` & `Sphinx-7.0.0rc1/tests/js/searchtools.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/js/sphinx_highlight.js` & `Sphinx-7.0.0rc1/tests/js/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-add_enumerable_node/enumerable_node.py` & `Sphinx-7.0.0rc1/tests/roots/test-add_enumerable_node/enumerable_node.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-add_enumerable_node/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-add_enumerable_node/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-api-set-translator/conf.py` & `Sphinx-7.0.0rc1/tests/roots/test-api-set-translator/conf.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-autosummary/dummy_module.py` & `Sphinx-7.0.0rc1/tests/roots/test-autosummary/dummy_module.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-basic/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-basic/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-directive-code/caption.rst` & `Sphinx-7.0.0rc1/tests/roots/test-directive-code/caption.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-directive-code/dedent.rst` & `Sphinx-7.0.0rc1/tests/roots/test-directive-code/dedent.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-directive-only/only.rst` & `Sphinx-7.0.0rc1/tests/roots/test-directive-only/only.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-domain-c-intersphinx/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-domain-c-intersphinx/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-domain-c/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-domain-c/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-domain-cpp-intersphinx/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-domain-cpp-intersphinx/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-domain-cpp/any-role.rst` & `Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/any-role.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-domain-cpp/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-domain-cpp/roles-targets-ok.rst` & `Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/roles-targets-ok.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-domain-cpp/roles-targets-warn.rst` & `Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/roles-targets-warn.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-domain-cpp/roles.rst` & `Sphinx-7.0.0rc1/tests/roots/test-domain-cpp/roles.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-domain-js/module.rst` & `Sphinx-7.0.0rc1/tests/roots/test-domain-js/module.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-domain-js/roles.rst` & `Sphinx-7.0.0rc1/tests/roots/test-domain-js/roles.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-domain-py/module.rst` & `Sphinx-7.0.0rc1/tests/roots/test-domain-py/module.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-domain-py/roles.rst` & `Sphinx-7.0.0rc1/tests/roots/test-domain-py/roles.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/__init__.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/__init__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/autoclass_content.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/autoclass_content.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/autodoc_type_aliases.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/autodoc_type_aliases.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/classes.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/classes.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/coroutine.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/coroutine.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/decorator.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/decorator.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/descriptor.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/descriptor.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/docstring_signature.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/docstring_signature.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/need_mocks.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/need_mocks.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/overload.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/overload.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/preserve_defaults.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/preserve_defaults.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/private.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/private.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/singledispatch.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/singledispatch.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/singledispatchmethod.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/singledispatchmethod.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/typed_vars.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/typed_vars.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autodoc/target/typehints.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autodoc/target/typehints.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autosectionlabel-prefix-document/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autosectionlabel-prefix-document/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autosectionlabel/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autosectionlabel/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-autosummary/autosummary_dummy_module.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-autosummary/autosummary_dummy_module.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-doctest-skipif/skipif.txt` & `Sphinx-7.0.0rc1/tests/roots/test-ext-doctest-skipif/skipif.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-doctest/doctest.txt` & `Sphinx-7.0.0rc1/tests/roots/test-ext-doctest/doctest.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-extlinks-hardcoded-urls/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-ext-extlinks-hardcoded-urls/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-imgconverter/img.pdf` & `Sphinx-7.0.0rc1/tests/roots/test-ext-imgconverter/img.pdf`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-imgmockconverter/mocksvgconverter.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-imgmockconverter/mocksvgconverter.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-intersphinx-role/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-ext-intersphinx-role/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-viewcode-find/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode-find/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-viewcode/conf.py` & `Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode/conf.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-viewcode/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-ext-viewcode/objects.rst` & `Sphinx-7.0.0rc1/tests/roots/test-ext-viewcode/objects.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-footnotes/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-footnotes/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-html_entity/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-html_entity/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-html_scaled_image_link/img.png` & `Sphinx-7.0.0rc1/tests/roots/test-html_scaled_image_link/img.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-image-escape/img_#1.png` & `Sphinx-7.0.0rc1/tests/roots/test-image-escape/img_#1.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-images/img.gif` & `Sphinx-7.0.0rc1/tests/roots/test-images/img.gif`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-images/img.ja.png` & `Sphinx-7.0.0rc1/tests/roots/test-images/img.ja.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-images/img.pdf` & `Sphinx-7.0.0rc1/tests/roots/test-images/img.pdf`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-images/img.png` & `Sphinx-7.0.0rc1/tests/roots/test-images/img.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-images/img.zh.png` & `Sphinx-7.0.0rc1/tests/roots/test-images/img.zh.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-images/subdir/svgimg.pdf` & `Sphinx-7.0.0rc1/tests/roots/test-images/subdir/svgimg.pdf`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-images/testimäge.png` & `Sphinx-7.0.0rc1/tests/roots/test-images/testimäge.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/admonitions.txt` & `Sphinx-7.0.0rc1/tests/roots/test-intl/admonitions.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/docfields.txt` & `Sphinx-7.0.0rc1/tests/roots/test-intl/docfields.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/external_links.txt` & `Sphinx-7.0.0rc1/tests/roots/test-intl/external_links.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/figure.txt` & `Sphinx-7.0.0rc1/tests/roots/test-intl/figure.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/i18n.png` & `Sphinx-7.0.0rc1/tests/roots/test-intl/i18n.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/img.png` & `Sphinx-7.0.0rc1/tests/roots/test-intl/img.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/index.txt` & `Sphinx-7.0.0rc1/tests/roots/test-intl/index.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/index_entries.txt` & `Sphinx-7.0.0rc1/tests/roots/test-intl/index_entries.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/label_target.txt` & `Sphinx-7.0.0rc1/tests/roots/test-intl/label_target.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/literalblock.txt` & `Sphinx-7.0.0rc1/tests/roots/test-intl/literalblock.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/refs.txt` & `Sphinx-7.0.0rc1/tests/roots/test-intl/refs.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/role_xref.txt` & `Sphinx-7.0.0rc1/tests/roots/test-intl/role_xref.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/admonitions.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/admonitions.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/definition_terms.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/definition_terms.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/docfields.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/docfields.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/external_links.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/external_links.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/figure.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/figure.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/footnote.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/footnote.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms_inconsistency.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms_inconsistency.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/index.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/index_entries.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/index_entries.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/label_target.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/label_target.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/literalblock.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/literalblock.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/noqa.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/noqa.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/only.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/only.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/raw.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/raw.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/refs.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/refs.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/refs_inconsistency.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/refs_inconsistency.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/refs_python_domain.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/refs_python_domain.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/role_xref.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/role_xref.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/rubric.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/rubric.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/section.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/section.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/seealso.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/seealso.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/sphinx.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/table.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/table.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/toctree.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/toctree.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/topic.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/topic.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/versionchange.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/versionchange.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-intl/xx/LC_MESSAGES/warnings.po` & `Sphinx-7.0.0rc1/tests/roots/test-intl/xx/LC_MESSAGES/warnings.po`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-figure-in-admonition/img.png` & `Sphinx-7.0.0rc1/tests/roots/test-latex-figure-in-admonition/img.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-includegraphics/conf.py` & `Sphinx-7.0.0rc1/tests/roots/test-latex-includegraphics/conf.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-includegraphics/img.png` & `Sphinx-7.0.0rc1/tests/roots/test-latex-includegraphics/img.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-includegraphics/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-latex-includegraphics/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-includegraphics/sphinx.png` & `Sphinx-7.0.0rc1/tests/roots/test-latex-includegraphics/sphinx.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-includegraphics/tall.png` & `Sphinx-7.0.0rc1/tests/roots/test-latex-includegraphics/tall.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-labels/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-latex-labels/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/complex.rst` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/complex.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/complex_spanning_cell.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/complex_spanning_cell.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/gridtable.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/gridtable.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/gridtable_with_tabularcolumn.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/gridtable_with_tabularcolumn.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_align.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_align.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_caption.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_caption.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_problematic_cell.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_stub_columns_and_problematic_cell.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_stub_columns_and_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_verbatim.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_verbatim.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_widths.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_widths.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_having_widths_and_problematic_cell.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_having_widths_and_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/longtable_with_tabularcolumn.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/longtable_with_tabularcolumn.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/simple_table.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/simple_table.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_caption.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_caption.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_problematic_cell.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_stub_columns_and_problematic_cell.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_stub_columns_and_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_threeparagraphs_cell_in_first_col.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_threeparagraphs_cell_in_first_col.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_verbatim.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_verbatim.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_widths.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_widths.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/table_having_widths_and_problematic_cell.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/table_having_widths_and_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/tabular_having_widths.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/tabular_having_widths.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/tabularcolumn.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/tabularcolumn.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/expects/tabulary_having_widths.tex` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/expects/tabulary_having_widths.tex`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/longtable.rst` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/longtable.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-latex-table/tabular.rst` & `Sphinx-7.0.0rc1/tests/roots/test-latex-table/tabular.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-linkcheck/links.rst` & `Sphinx-7.0.0rc1/tests/roots/test-linkcheck/links.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-local-logo/images/img.png` & `Sphinx-7.0.0rc1/tests/roots/test-local-logo/images/img.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-local-logo/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-local-logo/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-maxlistdepth/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-maxlistdepth/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-metadata/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-metadata/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-need-escaped/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-need-escaped/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-numfig/bar.rst` & `Sphinx-7.0.0rc1/tests/roots/test-numfig/bar.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-numfig/foo.rst` & `Sphinx-7.0.0rc1/tests/roots/test-numfig/foo.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-numfig/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-numfig/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-productionlist/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-productionlist/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-remote-logo/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-remote-logo/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/Makefile` & `Sphinx-7.0.0rc1/tests/roots/test-root/Makefile`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/autodoc.txt` & `Sphinx-7.0.0rc1/tests/roots/test-root/autodoc.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/autodoc_target.py` & `Sphinx-7.0.0rc1/tests/roots/test-root/autodoc_target.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/conf.py` & `Sphinx-7.0.0rc1/tests/roots/test-root/conf.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/footnote.txt` & `Sphinx-7.0.0rc1/tests/roots/test-root/footnote.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/images.txt` & `Sphinx-7.0.0rc1/tests/roots/test-root/images.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/img.foo.png` & `Sphinx-7.0.0rc1/tests/roots/test-root/img.foo.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/img.gif` & `Sphinx-7.0.0rc1/tests/roots/test-root/img.gif`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/img.pdf` & `Sphinx-7.0.0rc1/tests/roots/test-root/img.pdf`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/img.png` & `Sphinx-7.0.0rc1/tests/roots/test-root/img.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/includes.txt` & `Sphinx-7.0.0rc1/tests/roots/test-root/includes.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/index.txt` & `Sphinx-7.0.0rc1/tests/roots/test-root/index.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/lists.txt` & `Sphinx-7.0.0rc1/tests/roots/test-root/lists.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/markup.txt` & `Sphinx-7.0.0rc1/tests/roots/test-root/markup.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/objects.txt` & `Sphinx-7.0.0rc1/tests/roots/test-root/objects.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/subdir/img.png` & `Sphinx-7.0.0rc1/tests/roots/test-root/subdir/img.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/subdir/simg.png` & `Sphinx-7.0.0rc1/tests/roots/test-root/subdir/simg.png`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-root/svgimg.pdf` & `Sphinx-7.0.0rc1/tests/roots/test-root/svgimg.pdf`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-theming/child.zip` & `Sphinx-7.0.0rc1/tests/roots/test-theming/child.zip`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-theming/parent.zip` & `Sphinx-7.0.0rc1/tests/roots/test-theming/parent.zip`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-theming/ziptheme.zip` & `Sphinx-7.0.0rc1/tests/roots/test-theming/ziptheme.zip`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-toctree-domain-objects/domains.rst` & `Sphinx-7.0.0rc1/tests/roots/test-toctree-domain-objects/domains.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-toctree/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-toctree/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-trim_doctest_flags/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-trim_doctest_flags/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-versioning/added.txt` & `Sphinx-7.0.0rc1/tests/roots/test-versioning/added.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-versioning/deleted.txt` & `Sphinx-7.0.0rc1/tests/roots/test-versioning/deleted.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-versioning/insert.txt` & `Sphinx-7.0.0rc1/tests/roots/test-versioning/insert.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-versioning/insert_beginning.txt` & `Sphinx-7.0.0rc1/tests/roots/test-versioning/insert_beginning.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-versioning/insert_similar.txt` & `Sphinx-7.0.0rc1/tests/roots/test-versioning/insert_similar.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-versioning/modified.txt` & `Sphinx-7.0.0rc1/tests/roots/test-versioning/modified.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-versioning/original.txt` & `Sphinx-7.0.0rc1/tests/roots/test-versioning/original.txt`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-warnings/index.rst` & `Sphinx-7.0.0rc1/tests/roots/test-warnings/index.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/roots/test-warnings/svgimg.pdf` & `Sphinx-7.0.0rc1/tests/roots/test-warnings/svgimg.pdf`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_api_translator.py` & `Sphinx-7.0.0rc1/tests/test_api_translator.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_application.py` & `Sphinx-7.0.0rc1/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_build.py` & `Sphinx-7.0.0rc1/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_build_changes.py` & `Sphinx-7.0.0rc1/tests/test_build_changes.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_build_dirhtml.py` & `Sphinx-7.0.0rc1/tests/test_build_dirhtml.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_build_epub.py` & `Sphinx-7.0.0rc1/tests/test_build_epub.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_build_gettext.py` & `Sphinx-7.0.0rc1/tests/test_build_gettext.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_build_html.py` & `Sphinx-7.0.0rc1/tests/test_build_html.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_build_latex.py` & `Sphinx-7.0.0rc1/tests/test_build_latex.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_build_linkcheck.py` & `Sphinx-7.0.0rc1/tests/test_build_linkcheck.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_build_manpage.py` & `Sphinx-7.0.0rc1/tests/test_build_manpage.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_build_texinfo.py` & `Sphinx-7.0.0rc1/tests/test_build_texinfo.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_build_text.py` & `Sphinx-7.0.0rc1/tests/test_build_text.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_builder.py` & `Sphinx-7.0.0rc1/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_catalogs.py` & `Sphinx-7.0.0rc1/tests/test_catalogs.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_config.py` & `Sphinx-7.0.0rc1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_correct_year.py` & `Sphinx-7.0.0rc1/tests/test_correct_year.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_directive_code.py` & `Sphinx-7.0.0rc1/tests/test_directive_code.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_directive_object_description.py` & `Sphinx-7.0.0rc1/tests/test_directive_object_description.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_directive_only.py` & `Sphinx-7.0.0rc1/tests/test_directive_only.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_directive_other.py` & `Sphinx-7.0.0rc1/tests/test_directive_other.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_directive_patch.py` & `Sphinx-7.0.0rc1/tests/test_directive_patch.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_docutilsconf.py` & `Sphinx-7.0.0rc1/tests/test_docutilsconf.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_domain_c.py` & `Sphinx-7.0.0rc1/tests/test_domain_c.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_domain_cpp.py` & `Sphinx-7.0.0rc1/tests/test_domain_cpp.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_domain_js.py` & `Sphinx-7.0.0rc1/tests/test_domain_js.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_domain_py.py` & `Sphinx-7.0.0rc1/tests/test_domain_py.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_domain_rst.py` & `Sphinx-7.0.0rc1/tests/test_domain_rst.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_domain_std.py` & `Sphinx-7.0.0rc1/tests/test_domain_std.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_environment.py` & `Sphinx-7.0.0rc1/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_environment_indexentries.py` & `Sphinx-7.0.0rc1/tests/test_environment_indexentries.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_environment_toctree.py` & `Sphinx-7.0.0rc1/tests/test_environment_toctree.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_events.py` & `Sphinx-7.0.0rc1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_apidoc.py` & `Sphinx-7.0.0rc1/tests/test_ext_apidoc.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autodoc.py` & `Sphinx-7.0.0rc1/tests/test_ext_autodoc.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autodoc_autoattribute.py` & `Sphinx-7.0.0rc1/tests/test_ext_autodoc_autoattribute.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autodoc_autoclass.py` & `Sphinx-7.0.0rc1/tests/test_ext_autodoc_autoclass.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autodoc_autodata.py` & `Sphinx-7.0.0rc1/tests/test_ext_autodoc_autodata.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autodoc_autofunction.py` & `Sphinx-7.0.0rc1/tests/test_ext_autodoc_autofunction.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autodoc_automodule.py` & `Sphinx-7.0.0rc1/tests/test_ext_autodoc_automodule.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autodoc_autoproperty.py` & `Sphinx-7.0.0rc1/tests/test_ext_autodoc_autoproperty.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autodoc_configs.py` & `Sphinx-7.0.0rc1/tests/test_ext_autodoc_configs.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autodoc_events.py` & `Sphinx-7.0.0rc1/tests/test_ext_autodoc_events.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autodoc_mock.py` & `Sphinx-7.0.0rc1/tests/test_ext_autodoc_mock.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autodoc_preserve_defaults.py` & `Sphinx-7.0.0rc1/tests/test_ext_autodoc_preserve_defaults.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autodoc_private_members.py` & `Sphinx-7.0.0rc1/tests/test_ext_autodoc_private_members.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autosectionlabel.py` & `Sphinx-7.0.0rc1/tests/test_ext_autosectionlabel.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_autosummary.py` & `Sphinx-7.0.0rc1/tests/test_ext_autosummary.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_coverage.py` & `Sphinx-7.0.0rc1/tests/test_ext_coverage.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_doctest.py` & `Sphinx-7.0.0rc1/tests/test_ext_doctest.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_extlinks.py` & `Sphinx-7.0.0rc1/tests/test_ext_extlinks.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_githubpages.py` & `Sphinx-7.0.0rc1/tests/test_ext_githubpages.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_graphviz.py` & `Sphinx-7.0.0rc1/tests/test_ext_graphviz.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_ifconfig.py` & `Sphinx-7.0.0rc1/tests/test_ext_ifconfig.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_imgconverter.py` & `Sphinx-7.0.0rc1/tests/test_ext_imgconverter.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_imgmockconverter.py` & `Sphinx-7.0.0rc1/tests/test_ext_imgmockconverter.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_inheritance_diagram.py` & `Sphinx-7.0.0rc1/tests/test_ext_inheritance_diagram.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_intersphinx.py` & `Sphinx-7.0.0rc1/tests/test_ext_intersphinx.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_math.py` & `Sphinx-7.0.0rc1/tests/test_ext_math.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_napoleon.py` & `Sphinx-7.0.0rc1/tests/test_ext_napoleon.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_napoleon_docstring.py` & `Sphinx-7.0.0rc1/tests/test_ext_napoleon_docstring.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_todo.py` & `Sphinx-7.0.0rc1/tests/test_ext_todo.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_ext_viewcode.py` & `Sphinx-7.0.0rc1/tests/test_ext_viewcode.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_extension.py` & `Sphinx-7.0.0rc1/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_highlighting.py` & `Sphinx-7.0.0rc1/tests/test_highlighting.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_intl.py` & `Sphinx-7.0.0rc1/tests/test_intl.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_locale.py` & `Sphinx-7.0.0rc1/tests/test_locale.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_markup.py` & `Sphinx-7.0.0rc1/tests/test_markup.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_metadata.py` & `Sphinx-7.0.0rc1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_parser.py` & `Sphinx-7.0.0rc1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_project.py` & `Sphinx-7.0.0rc1/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_pycode.py` & `Sphinx-7.0.0rc1/tests/test_pycode.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_pycode_ast.py` & `Sphinx-7.0.0rc1/tests/test_pycode_ast.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_pycode_parser.py` & `Sphinx-7.0.0rc1/tests/test_pycode_parser.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_quickstart.py` & `Sphinx-7.0.0rc1/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_roles.py` & `Sphinx-7.0.0rc1/tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_search.py` & `Sphinx-7.0.0rc1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_smartquotes.py` & `Sphinx-7.0.0rc1/tests/test_smartquotes.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_templating.py` & `Sphinx-7.0.0rc1/tests/test_templating.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_theming.py` & `Sphinx-7.0.0rc1/tests/test_theming.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_toctree.py` & `Sphinx-7.0.0rc1/tests/test_toctree.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_transforms_post_transforms.py` & `Sphinx-7.0.0rc1/tests/test_transforms_post_transforms.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_transforms_post_transforms_code.py` & `Sphinx-7.0.0rc1/tests/test_transforms_post_transforms_code.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util.py` & `Sphinx-7.0.0rc1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_display.py` & `Sphinx-7.0.0rc1/tests/test_util_display.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_docstrings.py` & `Sphinx-7.0.0rc1/tests/test_util_docstrings.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_docutils.py` & `Sphinx-7.0.0rc1/tests/test_util_docutils.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_fileutil.py` & `Sphinx-7.0.0rc1/tests/test_util_fileutil.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_i18n.py` & `Sphinx-7.0.0rc1/tests/test_util_i18n.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_images.py` & `Sphinx-7.0.0rc1/tests/test_util_images.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_inspect.py` & `Sphinx-7.0.0rc1/tests/test_util_inspect.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_inventory.py` & `Sphinx-7.0.0rc1/tests/test_util_inventory.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_logging.py` & `Sphinx-7.0.0rc1/tests/test_util_logging.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_matching.py` & `Sphinx-7.0.0rc1/tests/test_util_matching.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_nodes.py` & `Sphinx-7.0.0rc1/tests/test_util_nodes.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_rst.py` & `Sphinx-7.0.0rc1/tests/test_util_rst.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_template.py` & `Sphinx-7.0.0rc1/tests/test_util_template.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_util_typing.py` & `Sphinx-7.0.0rc1/tests/test_util_typing.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_versioning.py` & `Sphinx-7.0.0rc1/tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/test_writer_latex.py` & `Sphinx-7.0.0rc1/tests/test_writer_latex.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/typing_test_data.py` & `Sphinx-7.0.0rc1/tests/typing_test_data.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tests/utils.py` & `Sphinx-7.0.0rc1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/tox.ini` & `Sphinx-7.0.0rc1/tox.ini`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/utils/babel_runner.py` & `Sphinx-7.0.0rc1/utils/babel_runner.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/utils/bump_version.py` & `Sphinx-7.0.0rc1/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/utils/release-checklist` & `Sphinx-7.0.0rc1/utils/release-checklist`

 * *Files identical despite different names*

### Comparing `Sphinx-7.0.0/PKG-INFO` & `Sphinx-7.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sphinx
-Version: 7.0.0
+Version: 7.0.0rc1
 Summary: Python documentation generator
 Author-email: Georg Brandl <georg@python.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

