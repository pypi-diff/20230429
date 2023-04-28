# Comparing `tmp/ark-3.0.1.tar.gz` & `tmp/ark-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ark-3.0.1.tar", last modified: Tue Sep  6 09:17:25 2016, max compression
+gzip compressed data, was "ark-7.0.0.tar", last modified: Fri Apr 28 23:31:16 2023, max compression
```

## Comparing `ark-3.0.1.tar` & `ark-7.0.0.tar`

### file list

```diff
@@ -1,168 +1,111 @@
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     2025 2016-09-05 22:24:48.000000 ark-3.0.1/ark/__init__.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      714 2016-08-19 17:03:23.000000 ark-3.0.1/ark/__main__.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     2847 2016-09-05 22:24:48.000000 ark-3.0.1/ark/build.py
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/cli/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     2800 2016-09-05 22:24:48.000000 ark-3.0.1/ark/cli/__init__.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1960 2016-09-05 22:24:48.000000 ark-3.0.1/ark/cli/build.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      730 2016-09-05 22:24:48.000000 ark-3.0.1/ark/cli/clear.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1141 2016-09-05 22:24:48.000000 ark-3.0.1/ark/cli/init.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     2482 2016-09-05 22:24:48.000000 ark-3.0.1/ark/cli/serve.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     3843 2016-09-05 22:24:48.000000 ark-3.0.1/ark/cli/watch.py
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ext/
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ext/__pycache__/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1392 2016-09-05 22:38:19.000000 ark-3.0.1/ark/ext/__pycache__/ark_breadcrumbs.cpython-35.pyc
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      503 2016-09-05 22:38:19.000000 ark-3.0.1/ark/ext/__pycache__/ark_classes.cpython-35.pyc
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1204 2016-09-06 09:16:22.000000 ark-3.0.1/ark/ext/__pycache__/ark_ibis.cpython-35.pyc
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1304 2016-09-06 09:16:22.000000 ark-3.0.1/ark/ext/__pycache__/ark_jinja.cpython-35.pyc
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      512 2016-09-05 22:38:19.000000 ark-3.0.1/ark/ext/__pycache__/ark_markdown.cpython-35.pyc
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1961 2016-09-05 22:38:19.000000 ark-3.0.1/ark/ext/__pycache__/ark_paging.cpython-35.pyc
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1241 2016-09-05 22:38:19.000000 ark-3.0.1/ark/ext/__pycache__/ark_pygmentize.cpython-35.pyc
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      971 2016-09-06 09:16:22.000000 ark-3.0.1/ark/ext/__pycache__/ark_shortcodes.cpython-35.pyc
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      588 2016-09-05 22:38:19.000000 ark-3.0.1/ark/ext/__pycache__/ark_stats.cpython-35.pyc
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      414 2016-09-05 22:38:19.000000 ark-3.0.1/ark/ext/__pycache__/ark_syntex.cpython-35.pyc
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     3122 2016-09-05 22:38:19.000000 ark-3.0.1/ark/ext/__pycache__/ark_tags.cpython-35.pyc
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      667 2016-09-05 22:38:19.000000 ark-3.0.1/ark/ext/__pycache__/ark_yaml.cpython-35.pyc
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     2084 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ext/ark_breadcrumbs.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      676 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ext/ark_classes.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1403 2016-09-06 09:15:26.000000 ark-3.0.1/ark/ext/ark_ibis.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1767 2016-09-06 09:15:48.000000 ark-3.0.1/ark/ext/ark_jinja.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      801 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ext/ark_markdown.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     4071 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ext/ark_paging.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1912 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ext/ark_pygmentize.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1361 2016-09-06 09:15:53.000000 ark-3.0.1/ark/ext/ark_shortcodes.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      877 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ext/ark_stats.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      587 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ext/ark_syntex.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     3455 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ext/ark_tags.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1134 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ext/ark_yaml.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1417 2016-09-05 22:24:48.000000 ark-3.0.1/ark/extensions.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     2297 2016-08-21 01:43:02.000000 ark-3.0.1/ark/hashes.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1426 2016-09-05 22:24:48.000000 ark-3.0.1/ark/hooks.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      867 2016-08-05 16:18:29.000000 ark-3.0.1/ark/includes.py
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1956 2016-08-05 15:47:59.000000 ark-3.0.1/ark/ini/ark.py
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/inc/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      950 2016-07-01 18:16:27.000000 ark-3.0.1/ark/ini/inc/footer.stx
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      115 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/inc/menu.md
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      248 2015-09-08 15:14:12.000000 ark-3.0.1/ark/ini/inc/sidebar.md
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/debug/
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/debug/extensions/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      849 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/debug/extensions/debug_dedup.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1212 2015-05-20 17:06:35.000000 ark-3.0.1/ark/ini/lib/debug/license.txt
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      234 2016-07-01 17:44:01.000000 ark-3.0.1/ark/ini/lib/debug/readme.md
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/debug/resources/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     4840 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/debug/resources/pygments.css
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1737 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/debug/resources/theme.css
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/debug/templates/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      538 2016-07-01 17:40:55.000000 ark-3.0.1/ark/ini/lib/debug/templates/base.ibis
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1144 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/debug/templates/index.ibis
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      397 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/debug/templates/single.ibis
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/phoenix/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1212 2016-07-01 17:18:54.000000 ark-3.0.1/ark/ini/lib/phoenix/license.txt
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1321 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/readme.md
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/css/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     4210 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/css/pygments.css
--rw-r--r--   0 dmlhllnd   (501) staff       (20)    14839 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/css/theme.css
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/css/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)    35134 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/css/font-awesome.css
--rw-r--r--   0 dmlhllnd   (501) staff       (20)    29063 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/css/font-awesome.min.css
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/fonts/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)    76518 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/fonts/fontawesome-webfont.eot
--rw-r--r--   0 dmlhllnd   (501) staff       (20)   391622 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/fonts/fontawesome-webfont.svg
--rw-r--r--   0 dmlhllnd   (501) staff       (20)   152796 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 dmlhllnd   (501) staff       (20)    90412 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/fonts/fontawesome-webfont.woff
--rw-r--r--   0 dmlhllnd   (501) staff       (20)    71896 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 dmlhllnd   (501) staff       (20)   124988 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/fonts/FontAwesome.otf
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      713 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/animated.less
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      585 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/bordered-pulled.less
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      452 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/core.less
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      119 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/fixed-width.less
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      495 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/font-awesome.less
--rw-r--r--   0 dmlhllnd   (501) staff       (20)    46249 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/icons.less
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      370 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/larger.less
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      377 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/list.less
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1603 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/mixins.less
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      771 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/path.less
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      622 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/rotated-flipped.less
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      118 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/screen-reader.less
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      476 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/stacked.less
--rw-r--r--   0 dmlhllnd   (501) staff       (20)    20890 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/less/variables.less
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      715 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/_animated.scss
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      592 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/_bordered-pulled.scss
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      459 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/_core.scss
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      120 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/_fixed-width.scss
--rw-r--r--   0 dmlhllnd   (501) staff       (20)    46979 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/_icons.scss
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      375 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/_larger.scss
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      378 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/_list.scss
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1637 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/_mixins.scss
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      783 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/_path.scss
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      672 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/_rotated-flipped.scss
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      134 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/_screen-reader.scss
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      482 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/_stacked.scss
--rw-r--r--   0 dmlhllnd   (501) staff       (20)    20971 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/_variables.scss
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      430 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/fa/scss/font-awesome.scss
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/images/
--rwxr-xr-x   0 dmlhllnd   (501) staff       (20)      167 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/images/background-dark-grey.png
--rwxr-xr-x   0 dmlhllnd   (501) staff       (20)      167 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/images/background-dark-red.png
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      170 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/images/background-dark-yellow.png
--rwxr-xr-x   0 dmlhllnd   (501) staff       (20)      178 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/images/background-image-border.png
--rwxr-xr-x   0 dmlhllnd   (501) staff       (20)      167 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/images/background-light-grey.png
--rwxr-xr-x   0 dmlhllnd   (501) staff       (20)      168 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/images/background-light-red.png
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      172 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/images/background-light-yellow.png
--rwxr-xr-x   0 dmlhllnd   (501) staff       (20)     6664 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/images/linen.jpg
--rwxr-xr-x   0 dmlhllnd   (501) staff       (20)      165 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/images/shaded-50.png
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/js/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     2731 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/phoenix/resources/js/html5shiv.js
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/phoenix/templates/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1976 2016-07-02 08:29:16.000000 ark-3.0.1/ark/ini/lib/phoenix/templates/base.ibis
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     2161 2016-08-04 22:24:43.000000 ark-3.0.1/ark/ini/lib/phoenix/templates/index.ibis
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      196 2016-07-01 01:48:00.000000 ark-3.0.1/ark/ini/lib/phoenix/templates/pages-single.ibis
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1280 2016-08-04 22:25:30.000000 ark-3.0.1/ark/ini/lib/phoenix/templates/single.ibis
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/vanilla/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1212 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/vanilla/license.txt
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      430 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/vanilla/readme.md
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/vanilla/resources/
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/vanilla/resources/css/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     4840 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/vanilla/resources/css/pygments.css
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     8115 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/vanilla/resources/css/theme.css
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/vanilla/resources/js/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     2731 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/vanilla/resources/js/html5shiv.js
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/lib/vanilla/templates/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      925 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/vanilla/templates/base.ibis
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      244 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/vanilla/templates/index.ibis
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      338 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/lib/vanilla/templates/single.ibis
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/src/
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/src/pages/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     4297 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/src/pages/about.stx
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1090 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/src/pages/index.md
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark/ini/src/posts/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1157 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/src/posts/post-one.md
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1158 2016-09-05 22:24:48.000000 ark-3.0.1/ark/ini/src/posts/post-two.md
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1121 2016-08-05 10:56:44.000000 ark-3.0.1/ark/loader.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      228 2016-09-06 09:10:42.000000 ark-3.0.1/ark/meta.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     8744 2016-09-05 22:24:48.000000 ark-3.0.1/ark/pages.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     2486 2016-08-05 16:18:39.000000 ark-3.0.1/ark/records.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1351 2016-08-13 09:25:45.000000 ark-3.0.1/ark/renderers.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     7237 2016-09-05 22:24:48.000000 ark-3.0.1/ark/site.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1759 2016-09-05 22:24:48.000000 ark-3.0.1/ark/templates.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      436 2016-09-05 22:24:48.000000 ark-3.0.1/ark/theme.py
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     4190 2016-09-05 22:24:48.000000 ark-3.0.1/ark/utils.py
-drwxr-xr-x   0 dmlhllnd   (501) staff       (20)        0 2016-09-06 09:17:25.000000 ark-3.0.1/ark.egg-info/
--rw-r--r--   0 dmlhllnd   (501) staff       (20)        1 2016-09-06 09:17:24.000000 ark-3.0.1/ark.egg-info/dependency_links.txt
--rw-r--r--   0 dmlhllnd   (501) staff       (20)       34 2016-09-06 09:17:24.000000 ark-3.0.1/ark.egg-info/entry_points.txt
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      807 2016-09-06 09:17:24.000000 ark-3.0.1/ark.egg-info/PKG-INFO
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      202 2016-09-06 09:17:24.000000 ark-3.0.1/ark.egg-info/requires.txt
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     5068 2016-09-06 09:17:25.000000 ark-3.0.1/ark.egg-info/SOURCES.txt
--rw-r--r--   0 dmlhllnd   (501) staff       (20)        4 2016-09-06 09:17:24.000000 ark-3.0.1/ark.egg-info/top_level.txt
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1212 2016-01-31 21:45:53.000000 ark-3.0.1/license.txt
--rw-r--r--   0 dmlhllnd   (501) staff       (20)       86 2016-09-06 09:17:24.000000 ark-3.0.1/MANIFEST.in
--rw-r--r--   0 dmlhllnd   (501) staff       (20)      807 2016-09-06 09:17:25.000000 ark-3.0.1/PKG-INFO
--rw-r--r--   0 dmlhllnd   (501) staff       (20)     1079 2016-09-05 22:24:48.000000 ark-3.0.1/readme.md
--rw-r--r--   0 dmlhllnd   (501) staff       (20)       59 2016-09-06 09:17:25.000000 ark-3.0.1/setup.cfg
--rwxr-xr-x   0 dmlhllnd   (501) staff       (20)     2122 2016-09-05 22:24:48.000000 ark-3.0.1/setup.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.687283 ark-7.0.0/
+-rw-r--r--   0 dmulholl   (501) staff       (20)       96 2023-04-28 23:31:16.000000 ark-7.0.0/MANIFEST.in
+-rw-r--r--   0 dmulholl   (501) staff       (20)      667 2023-04-28 23:31:16.686889 ark-7.0.0/PKG-INFO
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.651821 ark-7.0.0/ark/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1798 2023-04-28 21:56:21.000000 ark-7.0.0/ark/__init__.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      630 2023-04-28 22:09:04.000000 ark-7.0.0/ark/__main__.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.654314 ark-7.0.0/ark/bundle/
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.654734 ark-7.0.0/ark/bundle/inc/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      162 2021-11-15 13:56:09.000000 ark-7.0.0/ark/bundle/inc/menu.md
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.646541 ark-7.0.0/ark/bundle/lib/
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.655495 ark-7.0.0/ark/bundle/lib/debug/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      607 2022-03-04 18:57:03.000000 ark-7.0.0/ark/bundle/lib/debug/license.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)      217 2023-04-28 22:12:12.000000 ark-7.0.0/ark/bundle/lib/debug/readme.md
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.656223 ark-7.0.0/ark/bundle/lib/debug/resources/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1760 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/debug/resources/debug.css
+-rw-r--r--   0 dmulholl   (501) staff       (20)     4840 2020-12-13 21:19:09.000000 ark-7.0.0/ark/bundle/lib/debug/resources/pygments.css
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.656664 ark-7.0.0/ark/bundle/lib/debug/templates/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2486 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/debug/templates/node.ibis
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.657507 ark-7.0.0/ark/bundle/lib/graphite/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      607 2022-03-04 18:57:03.000000 ark-7.0.0/ark/bundle/lib/graphite/license.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1245 2023-04-28 22:13:18.000000 ark-7.0.0/ark/bundle/lib/graphite/readme.md
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.646766 ark-7.0.0/ark/bundle/lib/graphite/resources/
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.658954 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.666831 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    93768 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    13172 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Bold.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    75680 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    14196 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-BoldItalic.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    99800 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    14648 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Italic.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)   189596 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    13612 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-Regular.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    77596 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    14200 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBold.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)    75580 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.ttf
+-rw-r--r--   0 dmulholl   (501) staff       (20)    14388 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/CrimsonText-SemiBoldItalic.woff2
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)     4512 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts/OFL.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2047 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/fonts.css
+-rw-r--r--   0 dmulholl   (501) staff       (20)    11077 2023-04-07 20:56:01.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/graphite.css
+-rw-r--r--   0 dmulholl   (501) staff       (20)     5027 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/resources/assets/pygments.css
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.667194 ark-7.0.0/ark/bundle/lib/graphite/templates/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1800 2021-11-04 12:14:28.000000 ark-7.0.0/ark/bundle/lib/graphite/templates/node.ibis
+-rw-r--r--   0 dmulholl   (501) staff       (20)      448 2023-04-28 22:18:55.000000 ark-7.0.0/ark/bundle/site.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.668336 ark-7.0.0/ark/bundle/src/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      551 2020-12-13 21:19:09.000000 ark-7.0.0/ark/bundle/src/about.md
+-rw-r--r--   0 dmulholl   (501) staff       (20)     4349 2021-11-13 17:10:33.000000 ark-7.0.0/ark/bundle/src/index.stx
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.669079 ark-7.0.0/ark/bundle/src/parent/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1095 2020-12-13 21:19:09.000000 ark-7.0.0/ark/bundle/src/parent/child-one.md
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1095 2020-12-13 21:19:09.000000 ark-7.0.0/ark/bundle/src/parent/child-two.md
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1097 2020-12-13 21:19:09.000000 ark-7.0.0/ark/bundle/src/parent.md
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.672855 ark-7.0.0/ark/cli/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1831 2023-04-28 22:15:02.000000 ark-7.0.0/ark/cli/__init__.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2704 2023-04-28 22:16:17.000000 ark-7.0.0/ark/cli/add.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3091 2023-04-28 22:16:49.000000 ark-7.0.0/ark/cli/build.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      903 2023-04-28 22:15:53.000000 ark-7.0.0/ark/cli/clear.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1375 2023-04-28 22:16:35.000000 ark-7.0.0/ark/cli/deploy.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1244 2023-04-28 22:10:48.000000 ark-7.0.0/ark/cli/init.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1313 2023-04-28 22:11:19.000000 ark-7.0.0/ark/cli/open.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2904 2023-04-28 22:15:41.000000 ark-7.0.0/ark/cli/serve.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2319 2023-04-28 22:16:28.000000 ark-7.0.0/ark/cli/tree.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     4019 2023-04-28 22:12:43.000000 ark-7.0.0/ark/cli/watch.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2882 2023-04-28 22:19:16.000000 ark-7.0.0/ark/events.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.675524 ark-7.0.0/ark/extensions/
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.686367 ark-7.0.0/ark/extensions/__pycache__/
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3625 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_automenu.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1256 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_ibis.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1556 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_jinja.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      935 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_markdown.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1600 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_shortcodes.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      828 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_syntext.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1267 2023-04-28 22:46:26.000000 ark-7.0.0/ark/extensions/__pycache__/ark_yaml.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1817 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_automenu.cpython-310.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3625 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_automenu.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      692 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_ibis.cpython-310.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1256 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_ibis.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      842 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_jinja.cpython-310.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1556 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_jinja.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      538 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_markdown.cpython-310.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      935 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_markdown.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      885 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_shortcodes.cpython-310.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1600 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_shortcodes.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      510 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_syntext.cpython-310.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      828 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_syntext.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)      663 2022-04-16 08:41:29.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_yaml.cpython-310.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1267 2023-03-31 17:08:54.000000 ark-7.0.0/ark/extensions/__pycache__/ivy_yaml.cpython-311.pyc
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3038 2023-04-28 22:02:17.000000 ark-7.0.0/ark/extensions/ark_automenu.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      484 2023-04-28 22:03:31.000000 ark-7.0.0/ark/extensions/ark_ibis.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      731 2023-04-28 22:03:48.000000 ark-7.0.0/ark/extensions/ark_jinja.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      368 2023-04-28 22:04:06.000000 ark-7.0.0/ark/extensions/ark_markdown.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1057 2023-04-28 22:04:30.000000 ark-7.0.0/ark/extensions/ark_shortcodes.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      335 2023-04-28 22:04:44.000000 ark-7.0.0/ark/extensions/ark_syntext.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)      541 2023-04-28 22:05:00.000000 ark-7.0.0/ark/extensions/ark_yaml.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1658 2023-04-28 22:18:34.000000 ark-7.0.0/ark/extensions.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3051 2023-04-28 22:17:38.000000 ark-7.0.0/ark/filters.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2604 2023-04-28 22:08:26.000000 ark-7.0.0/ark/hashes.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)    11019 2023-04-28 22:17:50.000000 ark-7.0.0/ark/nodes.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1880 2023-04-28 22:09:28.000000 ark-7.0.0/ark/renderers.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     7623 2023-04-28 22:00:03.000000 ark-7.0.0/ark/site.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     2606 2023-04-28 22:07:18.000000 ark-7.0.0/ark/templates.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)     6549 2022-04-15 14:06:24.000000 ark-7.0.0/ark/utils.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-28 23:31:16.653890 ark-7.0.0/ark.egg-info/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      667 2023-04-28 23:31:16.000000 ark-7.0.0/ark.egg-info/PKG-INFO
+-rw-r--r--   0 dmulholl   (501) staff       (20)     3475 2023-04-28 23:31:16.000000 ark-7.0.0/ark.egg-info/SOURCES.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)        1 2023-04-28 23:31:16.000000 ark-7.0.0/ark.egg-info/dependency_links.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)       33 2023-04-28 23:31:16.000000 ark-7.0.0/ark.egg-info/entry_points.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)      118 2023-04-28 23:31:16.000000 ark-7.0.0/ark.egg-info/requires.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)        4 2023-04-28 23:31:16.000000 ark-7.0.0/ark.egg-info/top_level.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)     1212 2016-08-25 13:09:14.000000 ark-7.0.0/license.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)      208 2023-04-28 21:54:32.000000 ark-7.0.0/readme.md
+-rw-r--r--   0 dmulholl   (501) staff       (20)       38 2023-04-28 23:31:16.687413 ark-7.0.0/setup.cfg
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)     2084 2023-04-28 21:51:45.000000 ark-7.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ark-3.0.1/ark/cli/serve.py` & `ark-7.0.0/ark/cli/serve.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,93 @@
-# --------------------------------------------------------------------------
-# Logic for the 'serve' command.
-# --------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
+# This module contains the logic for the 'serve' command.
+# ------------------------------------------------------------------------------
 
 import sys
 import os
 import http.server
 import webbrowser
 
 from .. import site
+from .. import utils
+from .. import events
 
 
-# Command help text.
 helptext = """
-Usage: %s serve [FLAGS] [OPTIONS]
+Usage: ark serve
 
   Serve the site's output directory using Python's builtin web server. The
   default web browser is automatically launched to view the site.
 
   Host IP defaults to localhost (127.0.0.1). Specify an IP address to serve
-  only on that address or '0.0.0.0' to serve on all available IPs.
+  only on that address or 0.0.0.0 to serve on all available IPs.
 
-  Port number defaults to 0 which randomly selects an available port. Note
-  that port numbers below 1024 require root authorization.
+  Port number defaults to 8080. Setting the port number to 0 will randomly
+  select an available port above 1024. Note that port numbers below 1024
+  require root authorization.
 
 Options:
   -d, --directory <path>    Specify a custom directory to serve.
-  -h, --host <str>          Host IP address. Defaults to localhost.
-  -p, --port <int>          Port number. Defaults to 0, i.e. random.
+  -h, --host <addr>         Host IP address. Defaults to localhost.
+  -p, --port <int>          Port number. Defaults to 8080.
 
 Flags:
       --help                Print this command's help text and exit.
-      --no-browser          Do not launch the default web browser.
+"""
 
-""" % os.path.basename(sys.argv[0])
 
-
-# Command callback.
-def callback(parser):
-
-    if parser['directory']:
-        if not os.path.exists(parser['directory']):
-            sys.exit("Error: '%s' does not exist." % parser['directory'])
-        os.chdir(parser['directory'])
+@events.register(events.Event.CLI)
+def register_command(argparser):
+    cmd_parser = argparser.command("serve", helptext, cmd_callback)
+    cmd_parser.option("directory d")
+    cmd_parser.option("browser b")
+    cmd_parser.option("host h", default="localhost")
+    cmd_parser.option("port p", type=int, default=8080)
+
+
+def cmd_callback(cmd_name, cmd_parser):
+    if cmd_parser.found('directory'):
+        dirpath = os.path.abspath(cmd_parser.value('directory'))
+        if not os.path.exists(dirpath):
+            sys.exit(f"Error: directory '{dirpath}' does not exist.")
     else:
         if not site.home():
             sys.exit("Error: cannot locate the site's home directory.")
         if not os.path.exists(site.out()):
             sys.exit("Error: cannot locate the site's output directory.")
-        os.chdir(site.out())
+        dirpath = site.out()
+
+    os.chdir(dirpath)
+
+    req_host = cmd_parser.value('host')
+    req_port = cmd_parser.value('port')
+
+    server_class = http.server.ThreadingHTTPServer
+    handler_class = http.server.SimpleHTTPRequestHandler
 
     try:
-        server = http.server.HTTPServer(
-            (parser['host'], parser['port']),
-            http.server.SimpleHTTPRequestHandler
-        )
+        server = server_class((req_host, req_port), handler_class)
     except PermissionError:
         sys.exit("Error: use 'sudo' to run on a port below 1024.")
     except OSError:
-        sys.exit("Error: address already in use. Choose a different port.")
+        sys.exit("Error: port already in use. Choose a different port.")
 
-    address = server.socket.getsockname()
+    host, port = server.socket.getsockname()
 
-    print("-" * 80)
-    print("Root: %s" % site.out())
-    print("Host: %s"  % address[0])
-    print("Port: %s" % address[1])
-    print("Stop: Ctrl-C")
-    print("-" * 80)
+    url = f"http://{req_host}:{port}"
+    webbrowser.open(url)
 
-    if not parser['no-browser']:
-        webbrowser.open("http://%s:%s" % (parser['host'], address[1]))
+    utils.termline()
+    print("Root: %s" % dirpath)
+    print("Host: %s"  % host)
+    print("Port: %s" % port)
+    print("Stop: Ctrl-C")
+    utils.termline()
 
     try:
         server.serve_forever()
     except KeyboardInterrupt:
-        print("\n" + "-" * 80 + "Stopping server...\n" + "-" * 80)
+        print()
+        utils.termline()
+        print("Stopping server...")
+        utils.termline()
         server.server_close()
```

### Comparing `ark-3.0.1/ark/cli/watch.py` & `ark-7.0.0/ark/cli/watch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,121 +1,131 @@
-# --------------------------------------------------------------------------
-# Logic for the 'watch' command.
-# --------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
+# This module contains the logic for the 'watch' command.
+# ------------------------------------------------------------------------------
 
 import sys
 import os
 import hashlib
 import time
 import subprocess
 import hashlib
 
 from .. import site
 from .. import utils
+from .. import events
 
 
-# Command help text.
 helptext = """
-Usage: %s watch [FLAGS] [ARGUMENTS]
+Usage: ark watch
 
-  Monitor the site directory and automatically rebuild when file changes are
-  detected.
+  Monitor the site directory and automatically rebuild the site when file
+  changes are detected.
+
+  The test server is automatically launched to view the site.
 
 Options:
-  -i, --inc <path>      Override the default 'inc' directory.
-  -l, --lib <path>      Override the default 'lib' directory.
-  -o, --out <path>      Override the default 'out' directory.
-  -r, --res <path>      Override the default 'res' directory.
-  -s, --src <path>      Override the default 'src' directory.
+  -p, --port <int>      Port number to serve on. Defaults to 8080.
   -t, --theme <name>    Override the default theme.
 
 Flags:
   -c, --clear           Clear the output directory before each build.
-      --help            Print this command's help text and exit.
+  -h, --help            Print this command's help text and exit.
+"""
+
 
-""" % os.path.basename(sys.argv[0])
+@events.register(events.Event.CLI)
+def register_command(argparser):
+    cmd_parser = argparser.command("watch", helptext, cmd_callback)
+    cmd_parser.flag("clear c")
+    cmd_parser.option("theme t")
+    cmd_parser.option("port p", type=int, default=8080)
 
 
 # Callback for the watch command. Python doesn't have a builtin file system
 # watcher so we hack together one of our own.
-def callback(parser):
-
+def cmd_callback(cmd_name, cmd_parser):
     home = site.home()
     if not home:
         sys.exit("Error: cannot locate the site's home directory.")
 
-    # Assemble a list of arguments for the subprocess call.
-    args = []
-
-    # We need to check if the `ark` package has been executed:
-    # 1. Directly, as `python3 /path/to/ark/package`.
-    # 2. As an installed package on the import path, `python3 -m ark`.
-    # 3. Via an entry script, `ark`.
+    # We want to reinvoke the currently active Ark package when we call the
+    # build command. This package may have been invoked in one of three ways:
+    # 1. Directly: `python /path/to/ark/directory`.
+    # 2. As an installed package on the import path: `python -m ark`.
+    # 3. Via an entry script or Windows executable.
     if os.path.isdir(sys.argv[0]):
-        args += ['python3', sys.argv[0]]
-    elif os.path.isfile(sys.argv[0]) and sys.argv[0].endswith('__main__.py'):
-        args += ['python3', sys.argv[0]]
-    elif os.path.isfile(sys.argv[0]):
-        args.append(sys.argv[0])
+        base = ['python3', sys.argv[0]]
+    elif sys.argv[0].endswith('__main__.py'):
+        base = ['python3', sys.argv[0]]
+    else:
+        base = [sys.argv[0]]
 
     # Append the 'build' command, a 'watching' flag, and any user arguments.
-    args += ['build', 'watching'] + parser.get_args()
+    args = base + ['build', 'watching'] + cmd_parser.args
 
     # Add direct support for the 'build' command's options and flags.
-    if parser['out']: args += ['--out', parser['out']]
-    if parser['src']: args += ['--src', parser['src']]
-    if parser['lib']: args += ['--lib', parser['lib']]
-    if parser['inc']: args += ['--inc', parser['inc']]
-    if parser['res']: args += ['--res', parser['res']]
-    if parser['theme']: args += ['--theme', parser['theme']]
-    if parser['clear']: args += ['--clear']
+    if cmd_parser.found('theme'):
+        args += ['--theme', cmd_parser.value('theme')]
+    if cmd_parser.found('clear'):
+        args += ['--clear']
 
     # Print a header showing the site location.
-    print("-" * 80)
+    utils.termline()
     print("Site: %s" % home)
     print("Stop: Ctrl-C")
-    print("-" * 80)
+    utils.termline()
 
     # Build the site with the 'firstwatch' flag.
     subprocess.call(args + ['firstwatch'])
-    print("-" * 80)
+    utils.termline()
 
     # Create a hash digest of the site directory.
     oldhash = hashsite(home)
 
+    # Run the webserver in a child process. It should run silently in the
+    # background and automatically shut down when the watch process exits.
+    subprocess.Popen(
+        base + ['serve', '--port', str(cmd_parser.value('port'))],
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE
+    )
+
     # Loop until the user hits Ctrl-C.
     try:
         while True:
             newhash = hashsite(home)
             if newhash != oldhash:
                 subprocess.call(args)
                 newhash = hashsite(home)
             oldhash = newhash
             time.sleep(0.5)
     except KeyboardInterrupt:
         pass
 
     # Build the site with the 'lastwatch' flag.
-    print("\n" + "-" * 80)
+    print()
+    utils.termline()
     subprocess.call(args + ['lastwatch'])
-    print("-" * 80)
+    utils.termline()
 
 
-# Returns a hash digest of the site directory.
+# Return a hash digest of the site directory.
 def hashsite(sitepath):
-    hash = hashlib.sha256()
+    hasher = hashlib.sha256()
 
     def hashdir(dirpath, is_home):
-        for fileinfo in utils.files(dirpath):
-            if fileinfo.name.endswith('~'):
+        for entry in os.scandir(dirpath):
+            if entry.name.startswith('.') or entry.name.endswith('~'):
                 continue
-            mtime = os.path.getmtime(fileinfo.path)
-            hash.update(str(mtime).encode())
-            hash.update(fileinfo.name.encode())
+            if entry.is_file():
+                mtime = os.path.getmtime(entry.path)
+                hasher.update(str(mtime).encode())
+                hasher.update(entry.name.encode())
+            if entry.is_dir():
+                hashdir(entry.path, False)
 
-        for dirinfo in utils.subdirs(dirpath):
-            if is_home and dirinfo.name == 'out':
-                continue
-            hashdir(dirinfo.path, False)
+    try:
+        hashdir(sitepath, True)
+    except FileNotFoundError:
+        pass
 
-    hashdir(sitepath, True)
-    return hash.digest()
+    return hasher.digest()
```

### Comparing `ark-3.0.1/ark/ext/ark_shortcodes.py` & `ark-7.0.0/ark/extensions/ark_shortcodes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# --------------------------------------------------------------------------
-# This extension adds support for shortcodes.
-# --------------------------------------------------------------------------
+# Add support for shortcodes in node content.
 
 import ark
 import sys
 
 try:
     import shortcodes
 except ImportError:
     shortcodes = None
 
 
+# We parse all shortcodes using this single Parser instance.
+parser = None
+
+
 # The shortcodes package is an optional dependency.
 if shortcodes:
 
-    # Check the site's config file for customized settings for the shortcode
-    # parser.
-    settings = ark.site.config.get('shortcodes', {})
-
-    # Initialize a single parser instance.
-    parser = shortcodes.Parser(**settings)
-
-    # Filter each record's content on the 'record_text' filter hook and
-    # render any shortcodes contained in it.
-    @ark.hooks.register('record_text')
-    def render(text, node):
+    # We process and replace shortcodes in the node's text content just before
+    # that text is rendered into HTML.
+    @ark.filters.register(ark.filters.Filter.NODE_TEXT)
+    def render_shortcodes(text, node):
+        global parser
+        if parser is None:
+            settings = ark.site.config.get('shortcode_settings') or {}
+            parser = shortcodes.Parser(**settings)
+
         try:
             return parser.parse(text, node)
         except shortcodes.ShortcodeError as err:
-            msg =  "-------------------\n"
-            msg += "  Shortcode Error  \n"
-            msg += "-------------------\n\n"
-            msg += "  Node: %s\n\n" % node.path()
-            msg += "  %s: %s" % (err.__class__.__name__, err)
-            if err.__context__:
-                cause = err.__context__
-                msg += "\n\nThe following cause was reported:\n\n"
-                msg += "%s: %s" % (cause.__class__.__name__, cause)
+            msg = "Shortcode Error\n"
+            msg += f">> Node: {node.url}\n"
+            msg += f">> {err.__class__.__name__}: {err}"
+            if (cause := err.__cause__):
+                msg += f"\n>> Cause: {cause.__class__.__name__}: {cause}"
             sys.exit(msg)
```

### Comparing `ark-3.0.1/ark/extensions.py` & `ark-7.0.0/ark/extensions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,53 @@
-# --------------------------------------------------------------------------
-# Loads extension modules.
-# --------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
+# This module loads extensions, i.e. Python modules and packages which use Ark's
+# plugin architecture to extend its functionality.
+# ------------------------------------------------------------------------------
 
 import os
 import sys
 import importlib
-
 from . import site
-from . import cli
-
-
-# Dictionary of loaded extension modules indexed by name.
-loaded = {}
 
 
-# Load the named module from the specified directory.
-def load_module(directory, name):
-    sys.path.insert(0, directory)
-    loaded[name] = importlib.import_module(name)
+# Load the named Python module from the specified directory.
+def load_module(dirpath: str, name: str):
+    sys.path.insert(0, dirpath)
+    importlib.import_module(name)
     sys.path.pop(0)
 
 
-# Load a directory of modules.
-def load_directory(directory):
-    for item in os.listdir(directory):
-        if item.startswith('.'):
+# Load a directory of Python modules.
+def load_directory(dirpath: str):
+    for name in os.listdir(dirpath):
+        if name.startswith('.'):
             continue
-        itembase = os.path.splitext(item)[0]
-        load_module(directory, itembase)
+        path = os.path.join(dirpath, name)
+        if os.path.isfile(path):
+            base, ext = os.path.splitext(name)
+            if ext == '.py':
+                load_module(dirpath, base)
+        elif os.path.isdir(path):
+            load_module(dirpath, name)
 
 
-# Load Ark's default set of extensions.
+# Load the default set of bundled extensions.
 def load_bundled_extensions():
-    load_directory(os.path.join(os.path.dirname(__file__), 'ext'))
+    load_directory(os.path.join(os.path.dirname(__file__), 'extensions'))
 
 
 # Load extensions from the site directory.
 def load_site_extensions():
     if os.path.isdir(site.ext()):
         load_directory(site.ext())
 
 
 # Load installed extensions listed in the site's configuration file.
 def load_installed_extensions():
     for name in site.config.get('extensions', []):
-        loaded[name] = importlib.import_module(name)
+        importlib.import_module(name)
 
 
-# Load bundled, installed, and site-directory extensions.
-def load():
-    load_bundled_extensions()
-    load_installed_extensions()
-    load_site_extensions()
+# Load extensions bundled with the active theme.
+def load_theme_extensions():
+    if site.theme() and os.path.isdir(site.theme('extensions')):
+        load_directory(site.theme('extensions'))
```

### Comparing `ark-3.0.1/ark/hashes.py` & `ark-7.0.0/ark/hashes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,87 @@
-# --------------------------------------------------------------------------
-# Handles the file hashing mechanism.
+# ------------------------------------------------------------------------------
+# This module handles Ark's file hashing mechanism.
 #
-# Before writing a page file to disk we check if there is an existing
-# file of the same name left over from a previous build. If there is,
-# we compare the hash of the new page's content with the cached hash
-# of the old page's content. If they are identical, we skip writing the
-# new page to disk.
+# Before writing a page file to disk we check if there is an existing file of
+# the same name left over from a previous build. If there is, we compare the
+# hash of the new page's content with the cached hash of the old page's
+# content. If they are identical, we skip writing the new page to disk.
 #
 # This has two effects:
 #
 #   * We save on disk IO, which is more expensive than comparing hashes.
 #   * We avoid unnecessarily bumping the file modification time.
-# --------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 
 import os
 import hashlib
 import pickle
 
 from . import site
-from . import hooks
+from . import events
 
 
-# Stores page hashes from the previous and current build runs.
-_hashes = { 'old': {}, 'new': {} }
+# Stores page-content hashes.
+_hashes = {}
 
 
-# Returns the name of the cachefile for the curent site.
-def cachefile():
-    if not 'cachefile' in _hashes:
-        name = hashlib.sha1(site.home().encode()).hexdigest() + '.pickle'
-        user = os.path.expanduser('~')
-        _hashes['cachefile'] = os.path.join(user, '.cache', 'ark', name)
-    return _hashes['cachefile']
-
-
-# Load cached page hashes from the last build run.
-@hooks.register('init')
-def load():
-    if os.path.isfile(cachefile()):
-        with open(cachefile(), 'rb') as file:
-            _hashes['old'] = pickle.load(file)
+# Update flag. True if we've added new hashes.
+_updated = False
 
 
-# Cache page hashes to disk for the next build run.
-@hooks.register('exit')
-def save():
-    if _hashes['new'] and _hashes['new'] != _hashes['old']:
-        if not os.path.isdir(os.path.dirname(cachefile())):
-            os.makedirs(os.path.dirname(cachefile()))
-        with open(cachefile(), 'wb') as file:
-            pickle.dump(_hashes['new'], file)
+# Stores the filepath for the cached-hashes file.
+_file = None
 
 
-# Returns true if filepath is an existing file whose hash matches that of
-# the content string. We use the relative filepath as the key to avoid
-# leaking potentially sensitive information (e.g. usernames) if the hash
-# file is checked into a public version control repository.
-def match(filepath, content):
+# Returns true if `filepath` is an existing file whose hash matches that of
+# the content string.
+def match(filepath: str, content: str) -> bool:
     key = os.path.relpath(filepath, site.out())
-    _hashes['new'][key] = hashlib.sha1(content.encode()).hexdigest()
-    if os.path.exists(filepath):
-        return _hashes['old'].get(key) == _hashes['new'][key]
+    old_hash = _hashes.get(key)
+    new_hash = hashlib.sha1(content.encode()).hexdigest()
+    if new_hash == old_hash:
+        return os.path.exists(filepath)
     else:
+        global _updated
+        _updated = True
+        _hashes[key] = new_hash
         return False
+
+
+# Clear the cache and delete any existing cache file.
+def clear():
+    _hashes.clear()
+    if os.path.isfile(_cachefile()):
+        os.remove(_cachefile())
+
+
+# Returns the name of the cache file for the curent site.
+def _cachefile() -> str:
+    global _file
+    if _file is None:
+        name = hashlib.sha1(site.home().encode()).hexdigest() + '.pickle'
+        if os.name == 'nt':
+            root = os.getenv('LOCALAPPDATA', os.path.expanduser('~'))
+            root = os.path.join(root, 'Ark')
+        else:
+            root = os.path.expanduser('~/.cache/ark')
+        _file = os.path.join(root, name)
+    return _file
+
+
+# Load cached page hashes from the last build run.
+@events.register(events.Event.INIT)
+def _load():
+    if os.path.isfile(_cachefile()):
+        with open(_cachefile(), 'rb') as file:
+            global _hashes
+            _hashes = pickle.load(file)
+
+
+# Cache page hashes to disk for the next build run.
+@events.register(events.Event.EXIT)
+def _save():
+    if _updated:
+        if not os.path.isdir(os.path.dirname(_cachefile())):
+            os.makedirs(os.path.dirname(_cachefile()))
+        with open(_cachefile(), 'wb') as file:
+            pickle.dump(_hashes, file)
```

### Comparing `ark-3.0.1/ark/ini/lib/debug/license.txt` & `ark-7.0.0/license.txt`

 * *Files identical despite different names*

### Comparing `ark-3.0.1/ark/ini/lib/debug/resources/pygments.css` & `ark-7.0.0/ark/bundle/lib/debug/resources/pygments.css`

 * *Files identical despite different names*

### Comparing `ark-3.0.1/ark/ini/lib/vanilla/resources/css/pygments.css` & `ark-7.0.0/ark/bundle/lib/graphite/resources/assets/pygments.css`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,70 @@
-/*
-    Syntax highlighting styles for Pygmentized code samples.
-*/
+/**
+ * -------------------------------------------------------------------------
+ *  Pygments Theme
+ * -------------------------------------------------------------------------
+ */
 
 pre .bp { color: #3465a4 }                      /* Name.Builtin.Pseudo */
-pre .c  { color: #8f5902; font-style: italic }  /* Comment */
-pre .c1 { color: #8f5902; font-style: italic }  /* Comment.Single */
-pre .cm { color: #8f5902; font-style: italic }  /* Comment.Multiline */
-pre .cp { color: #8f5902 }                      /* Comment.Preproc */
-pre .cs { color: #8f5902; font-style: italic }  /* Comment.Special */
+pre .c  { color: #8f5902 }                      /* Comment */
+pre .c1 { color: #8f5902 }                      /* Comment.Single */
+pre .cm { color: #8f5902 }                      /* Comment.Multiline */
+pre .cp { color: #540e8a; font-weight: bold }   /* Comment.Preproc */
+pre .cs { color: #8f5902 }                      /* Comment.Special */
 pre .g  { color: #222222 }                      /* Generic */
 pre .gd { color: #a40000 }                      /* Generic.Deleted */
-pre .ge { color: #222222; font-style: italic }  /* Generic.Emph */
+pre .ge { color: #222222 }                      /* Generic.Emph */
 pre .gr { color: #ef2929 }                      /* Generic.Error */
 pre .gh { color: #000080; font-weight: bold }   /* Generic.Heading */
 pre .gi { color: #00A000 }                      /* Generic.Inserted */
-pre .go { color: #222222; font-style: italic }  /* Generic.Output */
+pre .go { color: #222222 }                      /* Generic.Output */
 pre .gp { color: #8f5902 }                      /* Generic.Prompt */
 pre .gs { color: #222222; font-weight: bold }   /* Generic.Strong */
 pre .gu { color: #800080; font-weight: bold }   /* Generic.Subheading */
 pre .gt { color: #a40000; font-weight: bold }   /* Generic.Traceback */
 pre .il { color: #000088 }                      /* Literal.Number.Integer.Long */
 pre .k  { color: #204a87; font-weight: bold }   /* Keyword */
 pre .kc { color: #204a87; font-weight: bold }   /* Keyword.Constant */
 pre .kd { color: #204a87; font-weight: bold }   /* Keyword.Declaration */
-pre .kn { color: #204a87; font-weight: bold }   /* Keyword.Namespace */
+pre .kn { color: #540e8a; font-weight: bold }   /* Keyword.Namespace */
 pre .kp { color: #204a87; font-weight: bold }   /* Keyword.Pseudo */
 pre .kr { color: #204a87; font-weight: bold }   /* Keyword.Reserved */
 pre .kt { color: #204a87; font-weight: bold }   /* Keyword.Type */
 pre .l  { color: #222222 }                      /* Literal */
 pre .ld { color: #222222 }                      /* Literal.Date */
 pre .m  { color: #000088 }                      /* Literal.Number */
 pre .mf { color: #000088 }                      /* Literal.Number.Float */
 pre .mh { color: #000088 }                      /* Literal.Number.Hex */
 pre .mi { color: #000088 }                      /* Literal.Number.Integer */
 pre .mo { color: #000088 }                      /* Literal.Number.Oct */
+pre .mb { color: #000088 }                      /* Literal.Number.Bin */
 pre .n  { color: #222222 }                      /* Name */
 pre .na { color: #8f5902 }                      /* Name.Attribute */
 pre .nb { color: #204a87 }                      /* Name.Builtin */
 pre .nc { color: #222222 }                      /* Name.Class */
 pre .no { color: #222222 }                      /* Name.Constant */
 pre .nd { color: #000088 }                      /* Name.Decorator */
 pre .ni { color: #ce5c00 }                      /* Name.Entity */
 pre .ne { color: #cc0000; font-weight: bold }   /* Name.Exception */
 pre .nf { color: #222222 }                      /* Name.Function */
-pre .nl { color: #f57900 }                      /* Name.Label */
+pre .nl { color: #880000 }                      /* Name.Label */
 pre .nn { color: #222222 }                      /* Name.Namespace */
 pre .nt { color: #204a87; font-weight: bold }   /* Name.Tag */
 pre .nv { color: #222222 }                      /* Name.Variable */
 pre .nx { color: #222222 }                      /* Name.Other */
 pre .o  { color: #000088 }                      /* Operator */
 pre .ow { color: #204a87; font-weight: bold }   /* Operator.Word */
 pre .p  { color: #222222 }                      /* Punctuation */
 pre .py { color: #222222 }                      /* Name.Property */
 pre .s  { color: #880000 }                      /* Literal.String */
 pre .s1 { color: #880000 }                      /* Literal.String.Single */
 pre .s2 { color: #880000 }                      /* Literal.String.Double */
 pre .sb { color: #880000 }                      /* Literal.String.Backtick */
 pre .sc { color: #880000 }                      /* Literal.String.Char */
-pre .sd { color: #880000; font-style: italic }  /* Literal.String.Doc */
+pre .sd { color: #880000 }                      /* Literal.String.Doc */
 pre .se { color: #880000 }                      /* Literal.String.Escape */
 pre .sh { color: #880000 }                      /* Literal.String.Heredoc */
 pre .si { color: #880000 }                      /* Literal.String.Interpol */
 pre .sr { color: #880000 }                      /* Literal.String.Regex */
 pre .ss { color: #880000 }                      /* Literal.String.Symbol */
 pre .sx { color: #880000 }                      /* Literal.String.Other */
 pre .vc { color: #222222 }                      /* Name.Variable.Class */
```

### Comparing `ark-3.0.1/ark/ini/src/pages/about.stx` & `ark-7.0.0/ark/bundle/src/index.stx`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 ---
-title: About
+title: Page Title
+subtitle: This page has a subtitle.
 ---
 
-Lorem ipsum dolor sit amet, consectetur [adipisicing elit](#), sed do eiusmod
+Lorem ipsum dolor sit amet, consectetur [adipiscing elit](#), sed do eiusmod
 *tempor incididunt* ut labore et **dolore magna** aliqua. Ut enim ad minim
 veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
-`commodo consequat`.
+`commodo consequat`.[^1]
 
 Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore
 eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident,
-sunt in culpa qui officia deserunt mollit anim id est laborum.
+sunt in culpa qui officia deserunt mollit anim id est laborum [fn:2].
+
+::: footnote 1
+    Gallia est omnis divisa in partes tres, quarum unam incolunt Belgae,
+    aliam Aquitani, tertiam qui ipsorum lingua Celtae, nostra Galli
+    appellantur.
+
+::: footnote 2
+    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum
+    dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
+    proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
+
+
 
 ## Heading H2
 
 Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat.
 
+
+
 ### Heading H3
 
 Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat.
 
@@ -34,31 +49,29 @@
     }
 
 Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat.
 
-::: c
-
+::: code c
     #include <stdio.h>
 
     int main(int argc, char *argv[])
     {
         printf("hello world\n");
         return 0;
     }
 
 Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat.
 
-:>>
-
+::: quote
     Gallia est omnis divisa in partes tres, quarum unam incolunt Belgae,
     aliam Aquitani, tertiam qui ipsorum lingua Celtae, nostra Galli
     appellantur.
 
 Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
@@ -78,55 +91,44 @@
 3. Pears
 
 Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat.
 
-||  First Definition  ||
+[[  First Definition  ]]
 
     Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
     eiusmod tempor incididunt ut labore et dolore magna aliqua.
 
-||  Second Definition  ||
+[[  Second Definition  ]]
 
     Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
     eiusmod tempor incididunt ut labore et dolore magna aliqua.
 
 Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat.
 
-* * *
+::: hr
 
 Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat.
 
-:!! info
-
-    This is an alert box of type: *info*.
+::: infobox
+    Gallia est omnis divisa in partes tres, quarum unam incolunt Belgae,
+    aliam Aquitani, tertiam qui ipsorum lingua Celtae, nostra Galli
+    appellantur.
 
 Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat.
 
-:!! warning
-
-    This is an alert box of type: *warning*.
-
-Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
-tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
-quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
-consequat.
 
-:!! error
 
-    This is an alert box of type: *error*.
+### Notes
 
-Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
-tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
-quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
-consequat.
+::: insert footnotes
```

### Comparing `ark-3.0.1/ark/ini/src/pages/index.md` & `ark-7.0.0/ark/bundle/src/parent/child-one.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-title: Home
+title: Child One
 ---
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat.
```

### Comparing `ark-3.0.1/ark/ini/src/posts/post-one.md` & `ark-7.0.0/ark/bundle/src/parent/child-two.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 ---
-title: First Sample Post
-author: John Doe
-date: 2015-01-01
-tags: foo, bar, baz
+title: Child Two
 ---
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat.
```

### Comparing `ark-3.0.1/ark/ini/src/posts/post-two.md` & `ark-7.0.0/ark/bundle/src/parent.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 ---
-title: Second Sample Post
-author: John Doe
-date: 2015-01-02
-tags: bar, baz, bam
+title: Parent Page
 ---
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat.
```

