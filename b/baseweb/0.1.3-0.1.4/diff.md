# Comparing `tmp/baseweb-0.1.3.tar.gz` & `tmp/baseweb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseweb-0.1.3.tar", last modified: Tue Feb 14 13:15:31 2023, max compression
+gzip compressed data, was "baseweb-0.1.4.tar", last modified: Sat Apr 29 12:07:29 2023, max compression
```

## Comparing `baseweb-0.1.3.tar` & `baseweb-0.1.4.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.513841 baseweb-0.1.3/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.487280 baseweb-0.1.3/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     1028 2022-08-27 16:31:13.000000 baseweb-0.1.3/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1072 2022-08-27 15:15:58.000000 baseweb-0.1.3/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)     1072 2022-08-27 14:55:53.000000 baseweb-0.1.3/LICENSE.txt.backup
--rw-r--r--   0 xtof       (501) staff       (20)      189 2022-11-26 16:31:09.000000 baseweb-0.1.3/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     1718 2023-02-14 13:15:31.513711 baseweb-0.1.3/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.488652 baseweb-0.1.3/baseweb/
--rw-r--r--   0 xtof       (501) staff       (20)      230 2023-01-13 12:15:42.000000 baseweb-0.1.3/baseweb/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1469 2023-01-11 09:45:50.000000 baseweb-0.1.3/baseweb/config.py
--rw-r--r--   0 xtof       (501) staff       (20)     2024 2023-01-17 18:19:27.000000 baseweb-0.1.3/baseweb/interface.py
--rw-r--r--   0 xtof       (501) staff       (20)      347 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/rest.py
--rw-r--r--   0 xtof       (501) staff       (20)      836 2022-08-27 16:28:54.000000 baseweb-0.1.3/baseweb/security.py
--rw-r--r--   0 xtof       (501) staff       (20)      551 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/socketio.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.492541 baseweb-0.1.3/baseweb/static/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.493280 baseweb-0.1.3/baseweb/static/css/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/css/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      287 2022-12-29 15:36:28.000000 baseweb-0.1.3/baseweb/static/css/main.css
--rw-rw-rw-   0 xtof       (501) staff       (20)     4773 2022-10-28 08:40:23.000000 baseweb-0.1.3/baseweb/static/css/process_diagram.css
--rw-rw-rw-   0 xtof       (501) staff       (20)     6510 2022-10-28 08:40:23.000000 baseweb-0.1.3/baseweb/static/css/table.css
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.494275 baseweb-0.1.3/baseweb/static/js/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/js/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      861 2022-12-29 15:53:40.000000 baseweb-0.1.3/baseweb/static/js/app.js
--rw-r--r--   0 xtof       (501) staff       (20)      925 2022-12-29 15:52:31.000000 baseweb-0.1.3/baseweb/static/js/common.js
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.495890 baseweb-0.1.3/baseweb/static/js/components/
--rw-rw-rw-   0 xtof       (501) staff       (20)     8465 2023-01-12 13:14:07.000000 baseweb-0.1.3/baseweb/static/js/components/CollectionView.js
--rw-rw-rw-   0 xtof       (501) staff       (20)      615 2022-10-28 08:40:23.000000 baseweb-0.1.3/baseweb/static/js/components/LineChart.js
--rw-r--r--   0 xtof       (501) staff       (20)     4814 2022-12-29 15:51:31.000000 baseweb-0.1.3/baseweb/static/js/components/NavigationDrawer.js
--rw-r--r--   0 xtof       (501) staff       (20)      150 2022-12-28 10:56:49.000000 baseweb-0.1.3/baseweb/static/js/components/Page.js
--rw-r--r--   0 xtof       (501) staff       (20)      660 2022-12-28 11:19:05.000000 baseweb-0.1.3/baseweb/static/js/components/PageWithBanner.js
--rw-rw-rw-   0 xtof       (501) staff       (20)     5213 2022-12-25 15:23:36.000000 baseweb-0.1.3/baseweb/static/js/components/ProcessDiagram.js
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/js/components/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)       88 2022-12-28 12:15:48.000000 baseweb-0.1.3/baseweb/static/js/router.js
--rw-r--r--   0 xtof       (501) staff       (20)      571 2022-12-25 17:12:00.000000 baseweb-0.1.3/baseweb/static/js/socketio.js
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.495989 baseweb-0.1.3/baseweb/static/vendor/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.497357 baseweb-0.1.3/baseweb/static/vendor/css/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/css/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    13490 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/css/bootstrap-datetimepicker.css
--rw-r--r--   0 xtof       (501) staff       (20)     1571 2022-11-30 17:41:16.000000 baseweb-0.1.3/baseweb/static/vendor/css/highlight.js.github.css
--rw-r--r--   0 xtof       (501) staff       (20)     1363 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/css/roboto-material-icons.css
--rw-r--r--   0 xtof       (501) staff       (20)     9800 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/css/vfg.css
--rw-r--r--   0 xtof       (501) staff       (20)     7238 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/css/vue-multiselect.min.css
--rw-r--r--   0 xtof       (501) staff       (20)   210148 2022-12-25 18:19:16.000000 baseweb-0.1.3/baseweb/static/vendor/css/vuetify.min.css
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.499562 baseweb-0.1.3/baseweb/static/vendor/fonts/
--rw-r--r--   0 xtof       (501) staff       (20)    35588 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmEU9fBBc9.ttf
--rw-r--r--   0 xtof       (501) staff       (20)    35468 2022-12-28 19:16:33.000000 baseweb-0.1.3/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmSU5fBBc9.ttf
--rw-r--r--   0 xtof       (501) staff       (20)    35236 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmWUlfBBc9.ttf
--rw-r--r--   0 xtof       (501) staff       (20)    35408 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/fonts/KFOmCnqEu92Fr1Mu4mxP.ttf
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/fonts/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    49168 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.512264 baseweb-0.1.3/baseweb/static/vendor/js/
--rw-r--r--   0 xtof       (501) staff       (20)   157843 2022-12-29 15:35:01.000000 baseweb-0.1.3/baseweb/static/vendor/js/Chart.min.js
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/js/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    39239 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/js/bootstrap-datetimepicker.min.js
--rwxr-xr-x   0 xtof       (501) staff       (20)    37045 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/js/bootstrap.min.js
--rw-r--r--   0 xtof       (501) staff       (20)   120762 2022-11-30 17:19:12.000000 baseweb-0.1.3/baseweb/static/vendor/js/highlight.min.js
--rw-r--r--   0 xtof       (501) staff       (20)     2730 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/js/html5shiv.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    40413 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/js/index.js.map
--rwxr-xr-x   0 xtof       (501) staff       (20)    97163 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/js/jquery.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    51465 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/js/moment.min.js
--rw-r--r--   0 xtof       (501) staff       (20)     4377 2022-08-27 14:55:53.000000 baseweb-0.1.3/baseweb/static/vendor/js/respond.min.js
--rw-r--r--   0 xtof       (501) staff       (20)   146329 2022-08-27 16:18:42.000000 baseweb-0.1.3/baseweb/static/vendor/js/socket.io.min.js.map
--rw-r--r--   0 xtof       (501) staff       (20)    43622 2022-08-27 16:18:54.000000 baseweb-0.1.3/baseweb/static/vendor/js/socket.io.slim.js
--rw-r--r--   0 xtof       (501) staff       (20)     3526 2022-08-27 14:55:54.000000 baseweb-0.1.3/baseweb/static/vendor/js/vue-chartjs.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    24240 2022-08-27 14:55:54.000000 baseweb-0.1.3/baseweb/static/vendor/js/vue-chartjs.min.js.map
--rw-r--r--   0 xtof       (501) staff       (20)   115645 2022-08-27 14:55:54.000000 baseweb-0.1.3/baseweb/static/vendor/js/vue-form-generator.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    43084 2022-08-27 14:55:54.000000 baseweb-0.1.3/baseweb/static/vendor/js/vue-multiselect.min.js
--rw-r--r--   0 xtof       (501) staff       (20)    30139 2022-08-27 14:55:54.000000 baseweb-0.1.3/baseweb/static/vendor/js/vue-notification.js
--rw-r--r--   0 xtof       (501) staff       (20)    65289 2022-11-26 16:27:44.000000 baseweb-0.1.3/baseweb/static/vendor/js/vue-router.js
--rw-r--r--   0 xtof       (501) staff       (20)   433738 2022-12-25 18:21:14.000000 baseweb-0.1.3/baseweb/static/vendor/js/vue.js
--rw-r--r--   0 xtof       (501) staff       (20)  1101513 2022-12-25 18:34:51.000000 baseweb-0.1.3/baseweb/static/vendor/js/vuetify.js
--rw-r--r--   0 xtof       (501) staff       (20)  1102711 2022-12-25 18:34:51.000000 baseweb-0.1.3/baseweb/static/vendor/js/vuetify.js.map
--rw-r--r--   0 xtof       (501) staff       (20)    25628 2022-11-26 16:27:44.000000 baseweb-0.1.3/baseweb/static/vendor/js/vuex.js
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.513419 baseweb-0.1.3/baseweb/templates/
--rw-r--r--   0 xtof       (501) staff       (20)      270 2022-08-27 14:55:54.000000 baseweb-0.1.3/baseweb/templates/404.html
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:54.000000 baseweb-0.1.3/baseweb/templates/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     5515 2023-01-09 08:48:06.000000 baseweb-0.1.3/baseweb/templates/main.html
--rw-r--r--   0 xtof       (501) staff       (20)     1099 2022-12-28 10:02:38.000000 baseweb-0.1.3/baseweb/templates/manifest.json
--rw-r--r--   0 xtof       (501) staff       (20)      145 2022-12-28 11:17:50.000000 baseweb-0.1.3/baseweb/templates/store.js
--rw-r--r--   0 xtof       (501) staff       (20)      240 2023-01-11 09:31:30.000000 baseweb-0.1.3/baseweb/web.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.488893 baseweb-0.1.3/baseweb-demo/
--rw-r--r--   0 xtof       (501) staff       (20)     2332 2023-01-17 18:36:29.000000 baseweb-0.1.3/baseweb-demo/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.489139 baseweb-0.1.3/baseweb-demo/pages/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-11-26 16:32:12.000000 baseweb-0.1.3/baseweb-demo/pages/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.489255 baseweb-0.1.3/baseweb-demo/pages/components/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.489371 baseweb-0.1.3/baseweb-demo/pages/components/CollectionView/
--rw-r--r--   0 xtof       (501) staff       (20)     1924 2022-12-28 10:51:57.000000 baseweb-0.1.3/baseweb-demo/pages/components/CollectionView/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.489768 baseweb-0.1.3/baseweb-demo/pages/components/PageWithBanner/
--rw-r--r--   0 xtof       (501) staff       (20)      169 2022-12-28 10:58:50.000000 baseweb-0.1.3/baseweb-demo/pages/components/PageWithBanner/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-12-28 10:55:34.000000 baseweb-0.1.3/baseweb-demo/pages/components/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.490031 baseweb-0.1.3/baseweb-demo/pages/index/
--rw-r--r--   0 xtof       (501) staff       (20)     1610 2023-01-09 08:46:29.000000 baseweb-0.1.3/baseweb-demo/pages/index/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.490279 baseweb-0.1.3/baseweb-demo/pages/page1/
--rw-r--r--   0 xtof       (501) staff       (20)      160 2022-11-26 16:32:12.000000 baseweb-0.1.3/baseweb-demo/pages/page1/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.490546 baseweb-0.1.3/baseweb-demo/pages/page2/
--rw-r--r--   0 xtof       (501) staff       (20)      160 2022-11-26 16:32:12.000000 baseweb-0.1.3/baseweb-demo/pages/page2/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.490739 baseweb-0.1.3/baseweb-demo/pages/page3/
--rw-r--r--   0 xtof       (501) staff       (20)      160 2022-12-28 10:25:32.000000 baseweb-0.1.3/baseweb-demo/pages/page3/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.491039 baseweb-0.1.3/baseweb-demo/pages/page4/
--rw-r--r--   0 xtof       (501) staff       (20)      160 2022-12-28 13:04:06.000000 baseweb-0.1.3/baseweb-demo/pages/page4/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.491292 baseweb-0.1.3/baseweb-demo/pages/page5/
--rw-r--r--   0 xtof       (501) staff       (20)      160 2022-12-29 15:06:11.000000 baseweb-0.1.3/baseweb-demo/pages/page5/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.491549 baseweb-0.1.3/baseweb-demo/pages/process/
--rw-r--r--   0 xtof       (501) staff       (20)     2825 2022-12-25 15:24:02.000000 baseweb-0.1.3/baseweb-demo/pages/process/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.491815 baseweb-0.1.3/baseweb-demo/static/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-12-25 18:52:18.000000 baseweb-0.1.3/baseweb-demo/static/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-02-14 13:15:31.492421 baseweb-0.1.3/baseweb.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     1718 2023-02-14 13:15:31.000000 baseweb-0.1.3/baseweb.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)     3214 2023-02-14 13:15:31.000000 baseweb-0.1.3/baseweb.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2023-02-14 13:15:31.000000 baseweb-0.1.3/baseweb.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)      114 2023-02-14 13:15:31.000000 baseweb-0.1.3/baseweb.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       21 2023-02-14 13:15:31.000000 baseweb-0.1.3/baseweb.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2023-02-14 13:15:31.513877 baseweb-0.1.3/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1698 2023-01-13 12:16:18.000000 baseweb-0.1.3/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.564617 baseweb-0.1.4/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.551794 baseweb-0.1.4/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     1028 2022-08-27 16:31:13.000000 baseweb-0.1.4/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1072 2022-08-27 15:15:58.000000 baseweb-0.1.4/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)     1072 2022-08-27 14:55:53.000000 baseweb-0.1.4/LICENSE.txt.backup
+-rw-r--r--   0 xtof       (501) staff       (20)      189 2022-11-26 16:31:09.000000 baseweb-0.1.4/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     1718 2023-04-29 12:07:29.564489 baseweb-0.1.4/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.552763 baseweb-0.1.4/baseweb/
+-rw-r--r--   0 xtof       (501) staff       (20)      230 2023-04-29 07:10:09.000000 baseweb-0.1.4/baseweb/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1469 2023-01-11 09:45:50.000000 baseweb-0.1.4/baseweb/config.py
+-rw-r--r--   0 xtof       (501) staff       (20)     2024 2023-01-17 18:19:27.000000 baseweb-0.1.4/baseweb/interface.py
+-rw-r--r--   0 xtof       (501) staff       (20)      347 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/rest.py
+-rw-r--r--   0 xtof       (501) staff       (20)      836 2022-08-27 16:28:54.000000 baseweb-0.1.4/baseweb/security.py
+-rw-r--r--   0 xtof       (501) staff       (20)      551 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/socketio.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.555050 baseweb-0.1.4/baseweb/static/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.555429 baseweb-0.1.4/baseweb/static/css/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/css/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      287 2022-12-29 15:36:28.000000 baseweb-0.1.4/baseweb/static/css/main.css
+-rw-rw-rw-   0 xtof       (501) staff       (20)     4773 2022-10-28 08:40:23.000000 baseweb-0.1.4/baseweb/static/css/process_diagram.css
+-rw-rw-rw-   0 xtof       (501) staff       (20)     6510 2022-10-28 08:40:23.000000 baseweb-0.1.4/baseweb/static/css/table.css
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.555916 baseweb-0.1.4/baseweb/static/js/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/js/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      839 2023-04-29 07:16:33.000000 baseweb-0.1.4/baseweb/static/js/app.js
+-rw-r--r--   0 xtof       (501) staff       (20)      925 2022-12-29 15:52:31.000000 baseweb-0.1.4/baseweb/static/js/common.js
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.556818 baseweb-0.1.4/baseweb/static/js/components/
+-rw-rw-rw-   0 xtof       (501) staff       (20)     8465 2023-01-12 13:14:07.000000 baseweb-0.1.4/baseweb/static/js/components/CollectionView.js
+-rw-rw-rw-   0 xtof       (501) staff       (20)      615 2022-10-28 08:40:23.000000 baseweb-0.1.4/baseweb/static/js/components/LineChart.js
+-rw-r--r--   0 xtof       (501) staff       (20)     4814 2022-12-29 15:51:31.000000 baseweb-0.1.4/baseweb/static/js/components/NavigationDrawer.js
+-rw-r--r--   0 xtof       (501) staff       (20)      150 2022-12-28 10:56:49.000000 baseweb-0.1.4/baseweb/static/js/components/Page.js
+-rw-r--r--   0 xtof       (501) staff       (20)      660 2022-12-28 11:19:05.000000 baseweb-0.1.4/baseweb/static/js/components/PageWithBanner.js
+-rw-rw-rw-   0 xtof       (501) staff       (20)     5213 2022-12-25 15:23:36.000000 baseweb-0.1.4/baseweb/static/js/components/ProcessDiagram.js
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/js/components/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)       88 2022-12-28 12:15:48.000000 baseweb-0.1.4/baseweb/static/js/router.js
+-rw-r--r--   0 xtof       (501) staff       (20)      571 2022-12-25 17:12:00.000000 baseweb-0.1.4/baseweb/static/js/socketio.js
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.556918 baseweb-0.1.4/baseweb/static/vendor/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.557702 baseweb-0.1.4/baseweb/static/vendor/css/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/css/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    13490 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/css/bootstrap-datetimepicker.css
+-rw-r--r--   0 xtof       (501) staff       (20)     1571 2022-11-30 17:41:16.000000 baseweb-0.1.4/baseweb/static/vendor/css/highlight.js.github.css
+-rw-r--r--   0 xtof       (501) staff       (20)     1363 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/css/roboto-material-icons.css
+-rw-r--r--   0 xtof       (501) staff       (20)     9800 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/css/vfg.css
+-rw-r--r--   0 xtof       (501) staff       (20)     7238 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/css/vue-multiselect.min.css
+-rw-r--r--   0 xtof       (501) staff       (20)   210148 2022-12-25 18:19:16.000000 baseweb-0.1.4/baseweb/static/vendor/css/vuetify.min.css
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.558864 baseweb-0.1.4/baseweb/static/vendor/fonts/
+-rw-r--r--   0 xtof       (501) staff       (20)    35588 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmEU9fBBc9.ttf
+-rw-r--r--   0 xtof       (501) staff       (20)    35468 2022-12-28 19:16:33.000000 baseweb-0.1.4/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmSU5fBBc9.ttf
+-rw-r--r--   0 xtof       (501) staff       (20)    35236 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmWUlfBBc9.ttf
+-rw-r--r--   0 xtof       (501) staff       (20)    35408 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/fonts/KFOmCnqEu92Fr1Mu4mxP.ttf
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/fonts/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    49168 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.563349 baseweb-0.1.4/baseweb/static/vendor/js/
+-rw-r--r--   0 xtof       (501) staff       (20)   157843 2022-12-29 15:35:01.000000 baseweb-0.1.4/baseweb/static/vendor/js/Chart.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/js/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    39239 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/js/bootstrap-datetimepicker.min.js
+-rwxr-xr-x   0 xtof       (501) staff       (20)    37045 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/js/bootstrap.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)   120762 2022-11-30 17:19:12.000000 baseweb-0.1.4/baseweb/static/vendor/js/highlight.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)     2730 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/js/html5shiv.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    40413 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/js/index.js.map
+-rwxr-xr-x   0 xtof       (501) staff       (20)    97163 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/js/jquery.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    51465 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/js/moment.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)     4377 2022-08-27 14:55:53.000000 baseweb-0.1.4/baseweb/static/vendor/js/respond.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)   146329 2022-08-27 16:18:42.000000 baseweb-0.1.4/baseweb/static/vendor/js/socket.io.min.js.map
+-rw-r--r--   0 xtof       (501) staff       (20)    43622 2022-08-27 16:18:54.000000 baseweb-0.1.4/baseweb/static/vendor/js/socket.io.slim.js
+-rw-r--r--   0 xtof       (501) staff       (20)     3526 2022-08-27 14:55:54.000000 baseweb-0.1.4/baseweb/static/vendor/js/vue-chartjs.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    24240 2022-08-27 14:55:54.000000 baseweb-0.1.4/baseweb/static/vendor/js/vue-chartjs.min.js.map
+-rw-r--r--   0 xtof       (501) staff       (20)   115645 2022-08-27 14:55:54.000000 baseweb-0.1.4/baseweb/static/vendor/js/vue-form-generator.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    43084 2022-08-27 14:55:54.000000 baseweb-0.1.4/baseweb/static/vendor/js/vue-multiselect.min.js
+-rw-r--r--   0 xtof       (501) staff       (20)    30139 2022-08-27 14:55:54.000000 baseweb-0.1.4/baseweb/static/vendor/js/vue-notification.js
+-rw-r--r--   0 xtof       (501) staff       (20)    65289 2022-11-26 16:27:44.000000 baseweb-0.1.4/baseweb/static/vendor/js/vue-router.js
+-rw-r--r--   0 xtof       (501) staff       (20)   433738 2022-12-25 18:21:14.000000 baseweb-0.1.4/baseweb/static/vendor/js/vue.js
+-rw-r--r--   0 xtof       (501) staff       (20)  1101513 2022-12-25 18:34:51.000000 baseweb-0.1.4/baseweb/static/vendor/js/vuetify.js
+-rw-r--r--   0 xtof       (501) staff       (20)  1102711 2022-12-25 18:34:51.000000 baseweb-0.1.4/baseweb/static/vendor/js/vuetify.js.map
+-rw-r--r--   0 xtof       (501) staff       (20)    25628 2022-11-26 16:27:44.000000 baseweb-0.1.4/baseweb/static/vendor/js/vuex.js
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.564311 baseweb-0.1.4/baseweb/templates/
+-rw-r--r--   0 xtof       (501) staff       (20)      270 2022-08-27 14:55:54.000000 baseweb-0.1.4/baseweb/templates/404.html
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-08-27 14:55:54.000000 baseweb-0.1.4/baseweb/templates/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     5515 2023-04-29 07:17:17.000000 baseweb-0.1.4/baseweb/templates/main.html
+-rw-r--r--   0 xtof       (501) staff       (20)     1099 2022-12-28 10:02:38.000000 baseweb-0.1.4/baseweb/templates/manifest.json
+-rw-r--r--   0 xtof       (501) staff       (20)      145 2022-12-28 11:17:50.000000 baseweb-0.1.4/baseweb/templates/store.js
+-rw-r--r--   0 xtof       (501) staff       (20)      240 2023-01-11 09:31:30.000000 baseweb-0.1.4/baseweb/web.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.552967 baseweb-0.1.4/baseweb-demo/
+-rw-r--r--   0 xtof       (501) staff       (20)     1982 2023-04-29 12:06:06.000000 baseweb-0.1.4/baseweb-demo/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.553067 baseweb-0.1.4/baseweb-demo/pages/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-11-26 16:32:12.000000 baseweb-0.1.4/baseweb-demo/pages/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.553151 baseweb-0.1.4/baseweb-demo/pages/components/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.553236 baseweb-0.1.4/baseweb-demo/pages/components/CollectionView/
+-rw-r--r--   0 xtof       (501) staff       (20)     1924 2022-12-28 10:51:57.000000 baseweb-0.1.4/baseweb-demo/pages/components/CollectionView/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.553338 baseweb-0.1.4/baseweb-demo/pages/components/PageWithBanner/
+-rw-r--r--   0 xtof       (501) staff       (20)      169 2022-12-28 10:58:50.000000 baseweb-0.1.4/baseweb-demo/pages/components/PageWithBanner/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-12-28 10:55:34.000000 baseweb-0.1.4/baseweb-demo/pages/components/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.553578 baseweb-0.1.4/baseweb-demo/pages/index/
+-rw-r--r--   0 xtof       (501) staff       (20)     1313 2023-04-29 06:53:02.000000 baseweb-0.1.4/baseweb-demo/pages/index/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.553681 baseweb-0.1.4/baseweb-demo/pages/page1/
+-rw-r--r--   0 xtof       (501) staff       (20)      160 2022-11-26 16:32:12.000000 baseweb-0.1.4/baseweb-demo/pages/page1/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.553889 baseweb-0.1.4/baseweb-demo/pages/page2/
+-rw-r--r--   0 xtof       (501) staff       (20)      160 2022-11-26 16:32:12.000000 baseweb-0.1.4/baseweb-demo/pages/page2/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.554059 baseweb-0.1.4/baseweb-demo/pages/page3/
+-rw-r--r--   0 xtof       (501) staff       (20)      311 2023-04-29 12:05:47.000000 baseweb-0.1.4/baseweb-demo/pages/page3/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.554158 baseweb-0.1.4/baseweb-demo/pages/page4/
+-rw-r--r--   0 xtof       (501) staff       (20)      160 2022-12-28 13:04:06.000000 baseweb-0.1.4/baseweb-demo/pages/page4/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.554266 baseweb-0.1.4/baseweb-demo/pages/page5/
+-rw-r--r--   0 xtof       (501) staff       (20)      160 2022-12-29 15:06:11.000000 baseweb-0.1.4/baseweb-demo/pages/page5/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.554365 baseweb-0.1.4/baseweb-demo/pages/protected_page/
+-rw-r--r--   0 xtof       (501) staff       (20)     1229 2023-04-29 12:06:06.000000 baseweb-0.1.4/baseweb-demo/pages/protected_page/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.554463 baseweb-0.1.4/baseweb-demo/static/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-12-25 18:52:18.000000 baseweb-0.1.4/baseweb-demo/static/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-29 12:07:29.554946 baseweb-0.1.4/baseweb.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     1718 2023-04-29 12:07:29.000000 baseweb-0.1.4/baseweb.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)     3221 2023-04-29 12:07:29.000000 baseweb-0.1.4/baseweb.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-04-29 12:07:29.000000 baseweb-0.1.4/baseweb.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      114 2023-04-29 12:07:29.000000 baseweb-0.1.4/baseweb.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       21 2023-04-29 12:07:29.000000 baseweb-0.1.4/baseweb.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-04-29 12:07:29.564660 baseweb-0.1.4/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1698 2023-01-13 12:16:18.000000 baseweb-0.1.4/setup.py
```

### Comparing `baseweb-0.1.3/.github/README.md` & `baseweb-0.1.4/.github/README.md`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/LICENSE.txt` & `baseweb-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/LICENSE.txt.backup` & `baseweb-0.1.4/LICENSE.txt.backup`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/PKG-INFO` & `baseweb-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseweb
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Pythonic base for building interactive web applications
 Home-page: https://github.com/christophevg/baseweb
 Author: Christophe VG
 License: MIT
 Keywords: Flask Vue REST SocketIO
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 4 - Beta
```

### Comparing `baseweb-0.1.3/baseweb/config.py` & `baseweb-0.1.4/baseweb/config.py`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/interface.py` & `baseweb-0.1.4/baseweb/interface.py`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/security.py` & `baseweb-0.1.4/baseweb/security.py`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/socketio.py` & `baseweb-0.1.4/baseweb/socketio.py`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/css/process_diagram.css` & `baseweb-0.1.4/baseweb/static/css/process_diagram.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/css/table.css` & `baseweb-0.1.4/baseweb/static/css/table.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/js/app.js` & `baseweb-0.1.4/baseweb/static/js/app.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,8 @@
 var app = new Vue({
-    el: "#app",
     delimiters: ['${', '}'],
     router: router,
     components: {
         multiselect: VueMultiselect.Multiselect,
         navigationdrawer: NavigationDrawer
     },
     data: {
```

### Comparing `baseweb-0.1.3/baseweb/static/js/common.js` & `baseweb-0.1.4/baseweb/static/js/common.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/js/components/CollectionView.js` & `baseweb-0.1.4/baseweb/static/js/components/CollectionView.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/js/components/LineChart.js` & `baseweb-0.1.4/baseweb/static/js/components/LineChart.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/js/components/NavigationDrawer.js` & `baseweb-0.1.4/baseweb/static/js/components/NavigationDrawer.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/js/components/PageWithBanner.js` & `baseweb-0.1.4/baseweb/static/js/components/PageWithBanner.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/js/components/ProcessDiagram.js` & `baseweb-0.1.4/baseweb/static/js/components/ProcessDiagram.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/js/socketio.js` & `baseweb-0.1.4/baseweb/static/js/socketio.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/css/bootstrap-datetimepicker.css` & `baseweb-0.1.4/baseweb/static/vendor/css/bootstrap-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/css/highlight.js.github.css` & `baseweb-0.1.4/baseweb/static/vendor/css/highlight.js.github.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/css/roboto-material-icons.css` & `baseweb-0.1.4/baseweb/static/vendor/css/roboto-material-icons.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/css/vfg.css` & `baseweb-0.1.4/baseweb/static/vendor/css/vfg.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/css/vue-multiselect.min.css` & `baseweb-0.1.4/baseweb/static/vendor/css/vue-multiselect.min.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/css/vuetify.min.css` & `baseweb-0.1.4/baseweb/static/vendor/css/vuetify.min.css`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmEU9fBBc9.ttf` & `baseweb-0.1.4/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmEU9fBBc9.ttf`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmSU5fBBc9.ttf` & `baseweb-0.1.4/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmSU5fBBc9.ttf`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmWUlfBBc9.ttf` & `baseweb-0.1.4/baseweb/static/vendor/fonts/KFOlCnqEu92Fr1MmWUlfBBc9.ttf`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/fonts/KFOmCnqEu92Fr1Mu4mxP.ttf` & `baseweb-0.1.4/baseweb/static/vendor/fonts/KFOmCnqEu92Fr1Mu4mxP.ttf`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `baseweb-0.1.4/baseweb/static/vendor/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/Chart.min.js` & `baseweb-0.1.4/baseweb/static/vendor/js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/bootstrap-datetimepicker.min.js` & `baseweb-0.1.4/baseweb/static/vendor/js/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/bootstrap.min.js` & `baseweb-0.1.4/baseweb/static/vendor/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/highlight.min.js` & `baseweb-0.1.4/baseweb/static/vendor/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/html5shiv.min.js` & `baseweb-0.1.4/baseweb/static/vendor/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/index.js.map` & `baseweb-0.1.4/baseweb/static/vendor/js/index.js.map`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/jquery.min.js` & `baseweb-0.1.4/baseweb/static/vendor/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/moment.min.js` & `baseweb-0.1.4/baseweb/static/vendor/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/respond.min.js` & `baseweb-0.1.4/baseweb/static/vendor/js/respond.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/socket.io.min.js.map` & `baseweb-0.1.4/baseweb/static/vendor/js/socket.io.min.js.map`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/socket.io.slim.js` & `baseweb-0.1.4/baseweb/static/vendor/js/socket.io.slim.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/vue-chartjs.min.js` & `baseweb-0.1.4/baseweb/static/vendor/js/vue-chartjs.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/vue-chartjs.min.js.map` & `baseweb-0.1.4/baseweb/static/vendor/js/vue-chartjs.min.js.map`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/vue-form-generator.min.js` & `baseweb-0.1.4/baseweb/static/vendor/js/vue-form-generator.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/vue-multiselect.min.js` & `baseweb-0.1.4/baseweb/static/vendor/js/vue-multiselect.min.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/vue-notification.js` & `baseweb-0.1.4/baseweb/static/vendor/js/vue-notification.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/vue-router.js` & `baseweb-0.1.4/baseweb/static/vendor/js/vue-router.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/vue.js` & `baseweb-0.1.4/baseweb/static/vendor/js/vue.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/vuetify.js` & `baseweb-0.1.4/baseweb/static/vendor/js/vuetify.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/vuetify.js.map` & `baseweb-0.1.4/baseweb/static/vendor/js/vuetify.js.map`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/static/vendor/js/vuex.js` & `baseweb-0.1.4/baseweb/static/vendor/js/vuex.js`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/templates/main.html` & `baseweb-0.1.4/baseweb/templates/main.html`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb/templates/manifest.json` & `baseweb-0.1.4/baseweb/templates/manifest.json`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb-demo/__init__.py` & `baseweb-0.1.4/baseweb-demo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 logger = logging.getLogger(__name__)
 
 import os
 
 # load the environment variables for this setup
 from dotenv import load_dotenv, find_dotenv
 load_dotenv(find_dotenv())
+load_dotenv(find_dotenv(".env.local"))
 
 LOG_LEVEL = os.environ.get("LOG_LEVEL") or "INFO"
 
 # setup logging infrastructure
 
 # logging.getLogger("urllib3").setLevel(logging.WARN)
 
@@ -25,48 +26,34 @@
 logging.getLogger("engineio.client").setLevel(logging.WARN)
 logging.getLogger("engineio.server").setLevel(logging.WARN)
 logging.getLogger("socketio.client").setLevel(logging.WARN)
 logging.getLogger("socketio.server").setLevel(logging.WARN)
 
 logging.getLogger().handlers[0].setFormatter(formatter)
 
-from baseweb.config import app
-
-app["baseweb-demo"] = {
-  "a few" : "app specific",
-  "configuration" : "settings",
-}
-
-app.recaptcha = "6LcbsOEjAAAAAABrd1kwa0eciF8AZK2v6vSTxRzZ"
-
 # import baseweb server object to expose it from this application
 from baseweb.web import server
 
 from baseweb.security import add_authenticator
 
 def authenticator(scope, request, *args, **kwargs):
   logger.debug("AUTH: scope:{} / request:{} / args:{} / kwargs:{}".format(
     scope, str(request), str(args), str(kwargs)
   ))
   return True
 
 add_authenticator(authenticator)
 
 from baseweb.interface import register_component, register_static_folder
-from baseweb.interface import register_external_script, register_stylesheet
 
 HERE       = os.path.dirname(__file__)
-STATIC     = os.path.join(HERE, "static")
 COMPONENTS = os.path.join(HERE, "components")
 
-register_static_folder(STATIC)
-
-register_stylesheet("style.css", STATIC)
+register_static_folder(os.path.join(HERE, "static"))
 
 register_component("app.js",        HERE)
 register_component("SourceView.js", COMPONENTS)
 register_component("logo.js",       COMPONENTS)
 
-register_external_script("https://www.google.com/recaptcha/api.js?render=6LcbsOEjAAAAAABrd1kwa0eciF8AZK2v6vSTxRzZ")
-
 from .pages            import index, page1, page2, page3, page4, page5
+from .pages            import protected_page
 from .pages.components import CollectionView, PageWithBanner
```

### Comparing `baseweb-0.1.3/baseweb-demo/pages/components/CollectionView/__init__.py` & `baseweb-0.1.4/baseweb-demo/pages/components/CollectionView/__init__.py`

 * *Files identical despite different names*

### Comparing `baseweb-0.1.3/baseweb-demo/pages/index/__init__.py` & `baseweb-0.1.4/baseweb-demo/pages/index/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 
 register_component("index.js", os.path.dirname(__file__))
 
 from flask import request
 
 from flask_restful import Resource
 
-import requests
-
 from baseweb.rest     import api
 from baseweb.socketio import socketio
 from baseweb.security import authenticated
 
 # log all messages both to logging infrastructure and connected clients
 
 def log(msg):
@@ -35,19 +33,14 @@
 
 # set up a REST resource to handle requests from the UI
 
 class Hello(Resource):
   @authenticated("app.hello.get")
   def get(self):
     name = request.args["name"]
-    token = request.args["token"]
-    if token:
-      log(f"got token: {token}")
-      resp = requests.post("https://www.google.com/recaptcha/api/siteverify", {"secret": "6LcbsOEjAAAAAAk4rRljsrXMntrd5m2vIs32VbsF", "response" : token})
-      log(f"interpretation : {resp.json()}")
     log("received hello from {0} via rest/get".format(name))
     return "Hello {0} from REST/GET".format(name)
     
   @authenticated("app.hello.post")
   def post(self):
     name = request.get_json()["name"]
     log("received hello from {0} via rest/post".format(name))
```

### Comparing `baseweb-0.1.3/baseweb.egg-info/PKG-INFO` & `baseweb-0.1.4/baseweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseweb
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Pythonic base for building interactive web applications
 Home-page: https://github.com/christophevg/baseweb
 Author: Christophe VG
 License: MIT
 Keywords: Flask Vue REST SocketIO
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 4 - Beta
```

### Comparing `baseweb-0.1.3/baseweb.egg-info/SOURCES.txt` & `baseweb-0.1.4/baseweb.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 baseweb-demo/pages/components/PageWithBanner/__init__.py
 baseweb-demo/pages/index/__init__.py
 baseweb-demo/pages/page1/__init__.py
 baseweb-demo/pages/page2/__init__.py
 baseweb-demo/pages/page3/__init__.py
 baseweb-demo/pages/page4/__init__.py
 baseweb-demo/pages/page5/__init__.py
-baseweb-demo/pages/process/__init__.py
+baseweb-demo/pages/protected_page/__init__.py
 baseweb-demo/static/__init__.py
 baseweb.egg-info/PKG-INFO
 baseweb.egg-info/SOURCES.txt
 baseweb.egg-info/dependency_links.txt
 baseweb.egg-info/requires.txt
 baseweb.egg-info/top_level.txt
 baseweb/static/__init__.py
```

### Comparing `baseweb-0.1.3/setup.py` & `baseweb-0.1.4/setup.py`

 * *Files identical despite different names*

