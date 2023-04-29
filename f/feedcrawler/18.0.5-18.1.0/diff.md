# Comparing `tmp/feedcrawler-18.0.5.tar.gz` & `tmp/feedcrawler-18.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedcrawler-18.0.5.tar", last modified: Mon Apr 17 19:30:00 2023, max compression
+gzip compressed data, was "feedcrawler-18.1.0.tar", last modified: Sat Apr 29 16:52:10 2023, max compression
```

## Comparing `feedcrawler-18.0.5.tar` & `feedcrawler-18.1.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.604563 feedcrawler-18.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-17 19:30:00.604563 feedcrawler-18.0.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7047 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/external_sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    20326 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/external_sites/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/metadata/imdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_nx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/external_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42357 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_tools/myjd_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_tools/ombi_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_tools/overseerr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_tools/plex_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/jobs/feed_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/jobs/package_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20929 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/providers/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/http_requests/cache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/http_requests/cloudflare_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/http_requests/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    44206 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/myjd_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/url_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/web_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/web_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.604563 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    82113 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js
--rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js
--rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js
--rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
--rw-r--r--   0 runner    (1001) docker     (123)    60695 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
--rw-r--r--   0 runner    (1001) docker     (123)   194314 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
--rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
--rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    79982 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
--rw-r--r--   0 runner    (1001) docker     (123)   144900 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-ffd92ad0.js
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
--rw-r--r--   0 runner    (1001) docker     (123)    50726 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js
--rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-17 19:29:59.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    82956 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/web_interface/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 19:30:00.604563 feedcrawler-18.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.757878 feedcrawler-18.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-04-29 16:52:10.757878 feedcrawler-18.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6931 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.741878 feedcrawler-18.1.0/feedcrawler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.741878 feedcrawler-18.1.0/feedcrawler/external_sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.741878 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20326 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.745878 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.745878 feedcrawler-18.1.0/feedcrawler/external_sites/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/metadata/imdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.745878 feedcrawler-18.1.0/feedcrawler/external_sites/web_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/web_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/web_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/web_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/web_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.745878 feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/content_all_nx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.745878 feedcrawler-18.1.0/feedcrawler/external_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42357 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_tools/myjd_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_tools/ombi_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_tools/overseerr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/external_tools/plex_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.749879 feedcrawler-18.1.0/feedcrawler/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/jobs/feed_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/jobs/package_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.749879 feedcrawler-18.1.0/feedcrawler/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.749879 feedcrawler-18.1.0/feedcrawler/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/http_requests/cache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/http_requests/cloudflare_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44221 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/myjd_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/url_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/providers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.749879 feedcrawler-18.1.0/feedcrawler/web_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/web_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.737878 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.753878 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.757878 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    82113 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
+-rw-r--r--   0 runner    (1001) docker     (123)    60695 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194314 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
+-rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    79982 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
+-rw-r--r--   0 runner    (1001) docker     (123)   144900 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-ffd92ad0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
+-rw-r--r--   0 runner    (1001) docker     (123)    50726 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-29 16:52:09.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    82969 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/feedcrawler/web_interface/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:52:10.741878 feedcrawler-18.1.0/feedcrawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 16:52:10.000000 feedcrawler-18.1.0/feedcrawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 16:52:10.757878 feedcrawler-18.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-29 16:51:33.000000 feedcrawler-18.1.0/setup.py
```

### Comparing `feedcrawler-18.0.5/LICENSE.md` & `feedcrawler-18.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/PKG-INFO` & `feedcrawler-18.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedcrawler
-Version: 18.0.5
+Version: 18.1.0
 Summary: Automate downloads using predefined sites and the My JDownloader API
 Home-page: https://github.com/rix1337/FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -44,30 +44,24 @@
 
 ## Installation
 
 ## Manuelle Installation
 
 ### Voraussetzungen
 
-* [Python 3.8](https://www.python.org/downloads/) oder neuer (nur 3 [externe Abhängigkeiten](https://github.com/rix1337/FeedCrawler/blob/main/requirements.txt)!)
+* [Python 3.8](https://www.python.org/downloads/) oder neuer (nur 4 [externe Abhängigkeiten](https://github.com/rix1337/FeedCrawler/blob/main/requirements.txt)!)
 * [JDownloader 2](http://www.jdownloader.org/jdownloader2) mit aktivem [My JDownloader-Konto](https://my.jdownloader.org)
 * _optional: [FlareSolverr 3](https://github.com/FlareSolverr/FlareSolverr) um Cloudflare-Blockaden zu umgehen_
 
 ### Installation / Update durch [pip](https://pip.pypa.io/en/stable/installation/)
 
 ```pip install -U feedcrawler```
 
 Hinweise zur manuellen Installation und Einrichtung finden sich im [Wiki](https://github.com/rix1337/FeedCrawler/wiki)!
 
-### GUI aktivieren
-
-```pip install -U PySimpleGUI psgtray```
-
-Dieser Schritt ist optional und ist nur auf Desktop-Systemen sinnvoll. Windows-Builds beinhalten die GUI bereits.
-
 ### Lokaler Build
 Benötigt [Node.js](https://nodejs.org/en/download/), [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) und [pip](https://pip.pypa.io/en/stable/installation/):
 
 1. Frontend-Pfad aufrufen: `cd feedcrawler/web_interface/vuejs_frontend`
 2. Dependencies installieren: `npm ci`
 3. [Vue.js 3](https://vuejs.org/) Frontend kompilieren: `npm run build`
 4. Zurück in das Hauptverzeichnis wechseln: `cd ../../..`
@@ -110,14 +104,15 @@
 | ```--log-level=<LOGLEVEL>```   | Legt fest, wie genau geloggt wird (`CRITICAL`, `ERROR`, `WARNING`, `INFO`, `DEBUG`, `NOTSET`) |
 | ```--config="<PFAD>"```        | Legt den Ablageort für Einstellungen und Logs fest |
 | ```--port=<PORT>```            | Legt den Port des Webservers fest |
 | ```--jd-user=<NUTZERNAME>```   | Legt den Nutzernamen für My JDownloader fest |
 | ```--jd-pass=<PASSWORT>```     | Legt das Passwort für My JDownloader fest |
 | ```--jd-device=<GERÄTENAME>``` | Legt den Gerätenamen für My JDownloader fest (optional, wenn nur ein Gerät vorhanden ist) |
 | ```--delay=<SEKUNDEN>``` | Verzögere Suchlauf nach Start um ganze Zahl in Sekunden (optional) |
+| ```--no-gui``` | Startet FeedCrawler ohne GUI (optional) |
 
 ## Sicherheitshinweis
 
 Der Webserver sollte nie ohne Absicherung im Internet freigegeben werden. Dazu lassen sich im Webinterface Nutzername
 und Passwort festlegen.
 
 Es empfiehlt sich, zusätzlich einen Reverse-Proxy mit HTTPs-Zertifikat,
```

### Comparing `feedcrawler-18.0.5/README.md` & `feedcrawler-18.1.0/feedcrawler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: feedcrawler
+Version: 18.1.0
+Summary: Automate downloads using predefined sites and the My JDownloader API
+Home-page: https://github.com/rix1337/FeedCrawler
+Author: rix1337
+Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # FeedCrawler
 
 <img src="https://raw.githubusercontent.com/rix1337/FeedCrawler/main/feedcrawler/web_interface/vuejs_frontend/public/favicon.ico" data-canonical-src="https://raw.githubusercontent.com/rix1337/FeedCrawler/main/feedcrawler/web_interface/vuejs_frontend/public/favicon.ico" width="64" height="64" />
 
 FeedCrawler automatisiert bequem das Hinzufügen von Links für den JDownloader.
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rix1337/FeedCrawler/CreateRelease.yml?branch=main)](https://github.com/rix1337/FeedCrawler/actions/workflows/CreateRelease.yml)
@@ -29,30 +44,24 @@
 
 ## Installation
 
 ## Manuelle Installation
 
 ### Voraussetzungen
 
-* [Python 3.8](https://www.python.org/downloads/) oder neuer (nur 3 [externe Abhängigkeiten](https://github.com/rix1337/FeedCrawler/blob/main/requirements.txt)!)
+* [Python 3.8](https://www.python.org/downloads/) oder neuer (nur 4 [externe Abhängigkeiten](https://github.com/rix1337/FeedCrawler/blob/main/requirements.txt)!)
 * [JDownloader 2](http://www.jdownloader.org/jdownloader2) mit aktivem [My JDownloader-Konto](https://my.jdownloader.org)
 * _optional: [FlareSolverr 3](https://github.com/FlareSolverr/FlareSolverr) um Cloudflare-Blockaden zu umgehen_
 
 ### Installation / Update durch [pip](https://pip.pypa.io/en/stable/installation/)
 
 ```pip install -U feedcrawler```
 
 Hinweise zur manuellen Installation und Einrichtung finden sich im [Wiki](https://github.com/rix1337/FeedCrawler/wiki)!
 
-### GUI aktivieren
-
-```pip install -U PySimpleGUI psgtray```
-
-Dieser Schritt ist optional und ist nur auf Desktop-Systemen sinnvoll. Windows-Builds beinhalten die GUI bereits.
-
 ### Lokaler Build
 Benötigt [Node.js](https://nodejs.org/en/download/), [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) und [pip](https://pip.pypa.io/en/stable/installation/):
 
 1. Frontend-Pfad aufrufen: `cd feedcrawler/web_interface/vuejs_frontend`
 2. Dependencies installieren: `npm ci`
 3. [Vue.js 3](https://vuejs.org/) Frontend kompilieren: `npm run build`
 4. Zurück in das Hauptverzeichnis wechseln: `cd ../../..`
@@ -95,20 +104,23 @@
 | ```--log-level=<LOGLEVEL>```   | Legt fest, wie genau geloggt wird (`CRITICAL`, `ERROR`, `WARNING`, `INFO`, `DEBUG`, `NOTSET`) |
 | ```--config="<PFAD>"```        | Legt den Ablageort für Einstellungen und Logs fest |
 | ```--port=<PORT>```            | Legt den Port des Webservers fest |
 | ```--jd-user=<NUTZERNAME>```   | Legt den Nutzernamen für My JDownloader fest |
 | ```--jd-pass=<PASSWORT>```     | Legt das Passwort für My JDownloader fest |
 | ```--jd-device=<GERÄTENAME>``` | Legt den Gerätenamen für My JDownloader fest (optional, wenn nur ein Gerät vorhanden ist) |
 | ```--delay=<SEKUNDEN>``` | Verzögere Suchlauf nach Start um ganze Zahl in Sekunden (optional) |
+| ```--no-gui``` | Startet FeedCrawler ohne GUI (optional) |
 
 ## Sicherheitshinweis
 
 Der Webserver sollte nie ohne Absicherung im Internet freigegeben werden. Dazu lassen sich im Webinterface Nutzername
 und Passwort festlegen.
 
 Es empfiehlt sich, zusätzlich einen Reverse-Proxy mit HTTPs-Zertifikat,
 bspw. [kostenlos von letsencrypt](https://letsencrypt.org/), zu verwenden.
 
 ## Credits
 
 * [mmarquezs](https://github.com/mmarquezs/) (My JDownloader-API für Python)
 * [JetBrains PyCharm](https://www.jetbrains.com/?from=FeedCrawler) (Open-Source-Lizenz für dieses Projekt)
+
+
```

### Comparing `feedcrawler-18.0.5/feedcrawler/crawler.py` & `feedcrawler-18.1.0/feedcrawler/crawler.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,46 +28,50 @@
 
 def start_feedcrawler():
     with multiprocessing.Manager() as manager:
         shared_state_dict = manager.dict()
         shared_state_lock = manager.Lock()
         shared_state.set_state(shared_state_dict, shared_state_lock)
 
-        if gui.enabled:
-            window = gui.create_main_window()
-            sys.stdout = gui.PrintToConsoleAndGui(window)
-        else:
-            window = False
-            sys.stdout = Unbuffered(sys.stdout)
-
         parser = argparse.ArgumentParser()
         parser.add_argument("--log-level", help="Legt fest, wie genau geloggt wird (INFO, DEBUG)")
         parser.add_argument("--config", help="Legt den Ablageort für Einstellungen und Logs fest")
         parser.add_argument("--port", help="Legt den Port des Webservers fest")
         parser.add_argument("--jd-user", help="Legt den Nutzernamen für My JDownloader fest")
         parser.add_argument("--jd-pass", help="Legt das Passwort für My JDownloader fest")
         parser.add_argument("--jd-device", help="Legt den Gerätenamen für My JDownloader fest")
         parser.add_argument("--delay", help="Verzögere Suchlauf nach Start um ganze Zahl in Sekunden")
+        parser.add_argument("--no-gui", action='store_true', help="Startet FeedCrawler ohne GUI")
         parser.add_argument("--keep-cdc", action='store_true',
                             help="Intern: Vergisst 'Feed ab hier bereits gecrawlt' nicht vor dem ersten Suchlauf")
         parser.add_argument("--remove_cloudflare_time", action='store_true',
                             help="Intern: Leere die Zeit des letzten Cloudflare-Umgehungs-Laufes vor dem ersten Suchlauf")
         parser.add_argument("--test_run", action='store_true', help="Intern: Führt einen Testlauf durch")
         parser.add_argument("--docker", action='store_true',
                             help="Intern: Sperre Pfad und Port auf Docker-Standardwerte")
         arguments = parser.parse_args()
 
-        shared_state.set_initial_values(arguments.test_run, arguments.remove_cloudflare_time)
+        shared_state.set_initial_values(arguments.docker,
+                                        arguments.no_gui,
+                                        arguments.test_run,
+                                        arguments.remove_cloudflare_time
+                                        )
+
+        if shared_state.values["gui"]:
+            window, icon = gui.create_main_window()
+            sys.stdout = gui.PrintToConsoleAndGui(window)
+        else:
+            sys.stdout = Unbuffered(sys.stdout)
 
         print("┌──────────────────────────────────────────────┐")
         print("  FeedCrawler " + version + " von RiX")
         print("  https://github.com/rix1337/FeedCrawler")
         print("└──────────────────────────────────────────────┘")
 
-        if arguments.docker:
+        if shared_state.values["docker"]:
             config_path = "/config"
         else:
             config_path = configpath(arguments.config)
 
         shared_state.set_files(config_path)
 
         print('Nutze das Verzeichnis "' + config_path + '" für Einstellungen/Logs')
@@ -96,24 +100,24 @@
         for name in shared_state.values["sites"]:
             name = name.lower()
             hostname = clean_up_hostname(name, hostnames.get(name))
             if hostname:
                 set_hostnames[name] = hostname
 
         if not shared_state.values["test_run"] and not set_hostnames:
-            if gui.enabled:
+            if shared_state.values["gui"]:
                 gui.no_hostnames_gui(shared_state.values["configfile"])
             else:
                 print('Keine Hostnamen in der FeedCrawler.ini gefunden! Beende FeedCrawler!')
                 time.sleep(10)
             sys.exit(1)
 
         if not shared_state.values["test_run"]:
             if not os.path.exists(shared_state.values["configfile"]):
-                if arguments.docker:
+                if shared_state.values["docker"]:
                     if arguments.jd_user and arguments.jd_pass:
                         myjd_input(arguments.port, arguments.jd_user, arguments.jd_pass, arguments.jd_device)
                 else:
                     myjd_input(arguments.port, arguments.jd_user, arguments.jd_pass, arguments.jd_device)
             else:
                 feedcrawler = CrawlerConfig('FeedCrawler')
                 user = feedcrawler.get('myjd_user')
@@ -165,26 +169,26 @@
             else:
                 print('My JDownloader Zugangsversuche nicht erfolgreich! Beende FeedCrawler!')
                 sys.exit(1)
 
         feedcrawler = CrawlerConfig('FeedCrawler')
         port = int(feedcrawler.get("port"))
         docker = False
-        if arguments.docker:
+        if shared_state.values["docker"]:
             port = int('9090')
             docker = True
         elif arguments.port:
             port = int(arguments.port)
 
         if feedcrawler.get("prefix"):
             prefix = '/' + feedcrawler.get("prefix")
         else:
             prefix = ''
         local_address = 'http://' + check_ip() + ':' + str(port) + prefix
-        if not arguments.docker:
+        if not shared_state.values["docker"]:
             print('Der Webserver ist erreichbar unter "' + local_address + '"')
 
         shared_state.set_connection_info(local_address, port, prefix, docker)
 
         CrawlerConfig("FeedCrawler").remove_redundant_entries()
         remove_redundant_db_tables(shared_state.values["dbfile"])
 
@@ -206,16 +210,16 @@
                                                            args=(shared_state_dict, shared_state_lock,))
             process_feed_crawler.start()
 
             process_watch_packages = multiprocessing.Process(target=watch_packages,
                                                              args=(shared_state_dict, shared_state_lock,))
             process_watch_packages.start()
 
-            if not arguments.docker and gui.enabled:
-                gui.main_gui(window, shared_state_dict, shared_state_lock)
+            if shared_state.values["gui"]:
+                gui.main_gui(window, icon, shared_state_dict, shared_state_lock)
 
                 sys.stdout = sys.__stdout__
                 process_web_server.terminate()
                 process_feed_crawler.terminate()
                 process_watch_packages.terminate()
                 sys.exit(0)
```

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/content_all.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/content_all.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/content_shows.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/content_shows.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/shared.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_by.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_dw.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_dw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_ff.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_ff.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_fx.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_fx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_hw.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_hw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_nk.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_nx.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_nx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_ww.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_all_ww.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/metadata/imdb.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/metadata/imdb.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/content_all.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/web_search/content_all.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/content_shows.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/web_search/content_shows.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/shared.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/web_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_by.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_dw.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/content_all_dw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_fx.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/content_all_fx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_hw.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/content_all_hw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_nk.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_nx.py` & `feedcrawler-18.1.0/feedcrawler/external_sites/web_search/sites/content_all_nx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_tools/myjd_api.py` & `feedcrawler-18.1.0/feedcrawler/external_tools/myjd_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_tools/ombi_api.py` & `feedcrawler-18.1.0/feedcrawler/external_tools/ombi_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_tools/overseerr_api.py` & `feedcrawler-18.1.0/feedcrawler/external_tools/overseerr_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/external_tools/plex_api.py` & `feedcrawler-18.1.0/feedcrawler/external_tools/plex_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/jobs/feed_search.py` & `feedcrawler-18.1.0/feedcrawler/jobs/feed_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         DJ(filename='List_CustomDJ_Documentaries'),
         DJ(filename='List_CustomDJ_Documentaries_Regex'),
         DD(filename='List_CustomDD_Feeds')
     ]
 
 
 def feed_crawler(shared_state_dict, shared_state_lock):
-    if gui.enabled:
+    if shared_state_dict["gui"]:
         sys.stdout = gui.AppendToPrintQueue(shared_state_dict, shared_state_lock)
     else:
         sys.stdout = Unbuffered(sys.stdout)
 
     shared_state.set_state(shared_state_dict, shared_state_lock)
     shared_state.set_logger()
     logger = shared_state.logger
```

### Comparing `feedcrawler-18.0.5/feedcrawler/jobs/package_watcher.py` & `feedcrawler-18.1.0/feedcrawler/jobs/package_watcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from feedcrawler.providers.myjd_connection import retry_decrypt
 from feedcrawler.providers.myjd_connection import set_device_from_config
 from feedcrawler.providers.notifications import notify
 from feedcrawler.providers.sqlite_database import FeedDb
 
 
 def watch_packages(shared_state_dict, shared_state_lock):
-    if gui.enabled:
+    if shared_state_dict["gui"]:
         sys.stdout = gui.AppendToPrintQueue(shared_state_dict, shared_state_lock)
     else:
         sys.stdout = Unbuffered(sys.stdout)
 
     shared_state.set_state(shared_state_dict, shared_state_lock)
     shared_state.set_logger()
```

### Comparing `feedcrawler-18.0.5/feedcrawler/providers/common_functions.py` & `feedcrawler-18.1.0/feedcrawler/providers/common_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -495,15 +495,15 @@
         f = open(pathfile, "w")
         f.write(configpath)
         f.close()
     elif os.path.exists(pathfile):
         f = open(pathfile, "r")
         configpath = f.readline()
     else:
-        if gui.enabled:
+        if shared_state.values["gui"]:
             configpath = gui.configpath_gui(current_path)
         else:
             print("Wo sollen Einstellungen und Logs abgelegt werden? Leer lassen, um den aktuellen Pfad zu nutzen.")
             configpath = input("Pfad angeben:")
         if len(configpath) > 0:
             f = open(pathfile, "w")
             f.write(configpath)
```

### Comparing `feedcrawler-18.0.5/feedcrawler/providers/config.py` & `feedcrawler-18.1.0/feedcrawler/providers/config.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/providers/http_requests/cache_handler.py` & `feedcrawler-18.1.0/feedcrawler/providers/http_requests/cache_handler.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/providers/http_requests/cloudflare_handlers.py` & `feedcrawler-18.1.0/feedcrawler/providers/http_requests/cloudflare_handlers.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/providers/http_requests/request_handler.py` & `feedcrawler-18.1.0/feedcrawler/providers/http_requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/providers/myjd_connection.py` & `feedcrawler-18.1.0/feedcrawler/providers/myjd_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1064,15 +1064,15 @@
     if user and password and device:
         print("Zugangsdaten aus den Parametern übernommen.")
     elif user and password and not device:
         one_device = get_if_one_device(user, password)
         if one_device:
             print("Gerätename " + one_device + " automatisch ermittelt.")
     else:
-        if gui.enabled:
+        if shared_state.values["gui"]:
             user, password, device = gui.myjd_credentials_gui()
         else:
             print("Bitte die Zugangsdaten für My JDownloader angeben:")
             user = input("Nutzername/Email:")
             password = input("Passwort:")
             one_device = get_if_one_device(user, password)
             if one_device:
```

### Comparing `feedcrawler-18.0.5/feedcrawler/providers/notifications.py` & `feedcrawler-18.1.0/feedcrawler/providers/notifications.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/providers/shared_state.py` & `feedcrawler-18.1.0/feedcrawler/providers/shared_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 # FeedCrawler
 # Projekt von https://github.com/rix1337
 # Dieses Modul stellt alle globalen Parameter für die verschiedenen parallel laufenden Threads bereit.
 
 import logging
 import os
+import platform
 import sys
 import time
 from logging import handlers
 
 from feedcrawler.external_tools.myjd_api import Jddevice, Myjdapi
 from feedcrawler.external_tools.myjd_api import TokenExpiredException, RequestTimeoutException, MYJDException
 from feedcrawler.providers.config import CrawlerConfig
@@ -31,15 +32,21 @@
     lock.acquire()
     try:
         values[key] = value
     finally:
         lock.release()
 
 
-def set_initial_values(test_run, remove_cloudflare_time):
+def set_initial_values(docker, no_gui, test_run, remove_cloudflare_time):
+    update("docker", docker)
+    if docker or no_gui or (not platform.system() == 'Windows' and not os.environ.get('DISPLAY')):
+        gui_enabled = False
+    else:
+        gui_enabled = True
+    update("gui", gui_enabled)
     update("test_run", test_run)
     update("remove_cloudflare_time", remove_cloudflare_time)
     update("ww_blocked", False)
     update("sf_blocked", False)
     update("user_agent", 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) ' \
                          'Chrome/111.0.0.0 Safari/537.36')
```

### Comparing `feedcrawler-18.0.5/feedcrawler/providers/sqlite_database.py` & `feedcrawler-18.1.0/feedcrawler/providers/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/providers/url_functions.py` & `feedcrawler-18.1.0/feedcrawler/providers/url_functions.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/providers/version.py` & `feedcrawler-18.1.0/feedcrawler/providers/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import re
 from distutils.version import StrictVersion
 from urllib.request import urlopen
 
 
 def get_version():
-    return "18.0.5"
+    return "18.1.0"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub('[^\d\.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-ffd92ad0.js` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-ffd92ad0.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/index.html` & `feedcrawler-18.1.0/feedcrawler/web_interface/vuejs_frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/feedcrawler/web_interface/web_server.py` & `feedcrawler-18.1.0/feedcrawler/web_interface/web_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -2020,15 +2020,15 @@
         print('Update steht bereit (' + updateversion +
               ')! Weitere Informationen unter https://github.com/rix1337/FeedCrawler/releases/latest')
 
     app_container()
 
 
 def web_server(shared_state_dict, shared_state_lock):
-    if gui.enabled:
+    if shared_state_dict["gui"]:
         sys.stdout = gui.AppendToPrintQueue(shared_state_dict, shared_state_lock)
     else:
         sys.stdout = Unbuffered(sys.stdout)
 
     shared_state.set_state(shared_state_dict, shared_state_lock)
     shared_state.set_logger()
```

### Comparing `feedcrawler-18.0.5/feedcrawler.egg-info/PKG-INFO` & `feedcrawler-18.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: feedcrawler
-Version: 18.0.5
-Summary: Automate downloads using predefined sites and the My JDownloader API
-Home-page: https://github.com/rix1337/FeedCrawler
-Author: rix1337
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # FeedCrawler
 
 <img src="https://raw.githubusercontent.com/rix1337/FeedCrawler/main/feedcrawler/web_interface/vuejs_frontend/public/favicon.ico" data-canonical-src="https://raw.githubusercontent.com/rix1337/FeedCrawler/main/feedcrawler/web_interface/vuejs_frontend/public/favicon.ico" width="64" height="64" />
 
 FeedCrawler automatisiert bequem das Hinzufügen von Links für den JDownloader.
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rix1337/FeedCrawler/CreateRelease.yml?branch=main)](https://github.com/rix1337/FeedCrawler/actions/workflows/CreateRelease.yml)
@@ -44,30 +29,24 @@
 
 ## Installation
 
 ## Manuelle Installation
 
 ### Voraussetzungen
 
-* [Python 3.8](https://www.python.org/downloads/) oder neuer (nur 3 [externe Abhängigkeiten](https://github.com/rix1337/FeedCrawler/blob/main/requirements.txt)!)
+* [Python 3.8](https://www.python.org/downloads/) oder neuer (nur 4 [externe Abhängigkeiten](https://github.com/rix1337/FeedCrawler/blob/main/requirements.txt)!)
 * [JDownloader 2](http://www.jdownloader.org/jdownloader2) mit aktivem [My JDownloader-Konto](https://my.jdownloader.org)
 * _optional: [FlareSolverr 3](https://github.com/FlareSolverr/FlareSolverr) um Cloudflare-Blockaden zu umgehen_
 
 ### Installation / Update durch [pip](https://pip.pypa.io/en/stable/installation/)
 
 ```pip install -U feedcrawler```
 
 Hinweise zur manuellen Installation und Einrichtung finden sich im [Wiki](https://github.com/rix1337/FeedCrawler/wiki)!
 
-### GUI aktivieren
-
-```pip install -U PySimpleGUI psgtray```
-
-Dieser Schritt ist optional und ist nur auf Desktop-Systemen sinnvoll. Windows-Builds beinhalten die GUI bereits.
-
 ### Lokaler Build
 Benötigt [Node.js](https://nodejs.org/en/download/), [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) und [pip](https://pip.pypa.io/en/stable/installation/):
 
 1. Frontend-Pfad aufrufen: `cd feedcrawler/web_interface/vuejs_frontend`
 2. Dependencies installieren: `npm ci`
 3. [Vue.js 3](https://vuejs.org/) Frontend kompilieren: `npm run build`
 4. Zurück in das Hauptverzeichnis wechseln: `cd ../../..`
@@ -110,22 +89,21 @@
 | ```--log-level=<LOGLEVEL>```   | Legt fest, wie genau geloggt wird (`CRITICAL`, `ERROR`, `WARNING`, `INFO`, `DEBUG`, `NOTSET`) |
 | ```--config="<PFAD>"```        | Legt den Ablageort für Einstellungen und Logs fest |
 | ```--port=<PORT>```            | Legt den Port des Webservers fest |
 | ```--jd-user=<NUTZERNAME>```   | Legt den Nutzernamen für My JDownloader fest |
 | ```--jd-pass=<PASSWORT>```     | Legt das Passwort für My JDownloader fest |
 | ```--jd-device=<GERÄTENAME>``` | Legt den Gerätenamen für My JDownloader fest (optional, wenn nur ein Gerät vorhanden ist) |
 | ```--delay=<SEKUNDEN>``` | Verzögere Suchlauf nach Start um ganze Zahl in Sekunden (optional) |
+| ```--no-gui``` | Startet FeedCrawler ohne GUI (optional) |
 
 ## Sicherheitshinweis
 
 Der Webserver sollte nie ohne Absicherung im Internet freigegeben werden. Dazu lassen sich im Webinterface Nutzername
 und Passwort festlegen.
 
 Es empfiehlt sich, zusätzlich einen Reverse-Proxy mit HTTPs-Zertifikat,
 bspw. [kostenlos von letsencrypt](https://letsencrypt.org/), zu verwenden.
 
 ## Credits
 
 * [mmarquezs](https://github.com/mmarquezs/) (My JDownloader-API für Python)
 * [JetBrains PyCharm](https://www.jetbrains.com/?from=FeedCrawler) (Open-Source-Lizenz für dieses Projekt)
-
-
```

### Comparing `feedcrawler-18.0.5/feedcrawler.egg-info/SOURCES.txt` & `feedcrawler-18.1.0/feedcrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.5/setup.py` & `feedcrawler-18.1.0/setup.py`

 * *Files identical despite different names*

