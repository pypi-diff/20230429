# Comparing `tmp/pyunifiprotect-4.8.2.tar.gz` & `tmp/pyunifiprotect-4.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyunifiprotect-4.8.2.tar", last modified: Sat Apr 22 15:33:02 2023, max compression
+gzip compressed data, was "pyunifiprotect-4.8.3.tar", last modified: Sat Apr 29 16:01:30 2023, max compression
```

## Comparing `pyunifiprotect-4.8.2.tar` & `pyunifiprotect-4.8.3.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.412003 pyunifiprotect-4.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.392002 pyunifiprotect-4.8.2/.bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      300 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.bin/format-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.bin/install-requirements
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.392002 pyunifiprotect-4.8.2/.bin/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.bin/lib/common.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.bin/lint-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.bin/test-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.bin/update-requirements
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.392002 pyunifiprotect-4.8.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.392002 pyunifiprotect-4.8.2/.docker/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.docker/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.388002 pyunifiprotect-4.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.392002 pyunifiprotect-4.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.github/workflows/test-live-AngellusMortis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.392002 pyunifiprotect-4.8.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/LIVE_DATA_CI.md
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-22 15:33:02.412003 pyunifiprotect-4.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/TESTDATA.md
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.396002 pyunifiprotect-4.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/docs/dev.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.396002 pyunifiprotect-4.8.2/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.396002 pyunifiprotect-4.8.2/docs/overrides/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/docs/overrides/partials/toc-item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.396002 pyunifiprotect-4.8.2/pyunifiprotect/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47822 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.400002 pyunifiprotect-4.8.2/pyunifiprotect/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/chimes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/doorlocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/lights.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/liveviews.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.400002 pyunifiprotect-4.8.2/pyunifiprotect/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34837 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    72566 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    33277 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/release_cache.json
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.404003 pyunifiprotect-4.8.2/pyunifiprotect/test_util/
--rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/test_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/test_util/anonymize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.396002 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-22 15:33:02.000000 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-22 15:33:02.000000 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 15:33:02.000000 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-22 15:33:02.000000 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-22 15:33:02.000000 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-22 15:33:02.000000 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 15:33:02.412003 pyunifiprotect-4.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.404003 pyunifiprotect-4.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22173 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.404003 pyunifiprotect-4.8.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29621 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_chime.py
--rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_doorlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_light.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.412003 pyunifiprotect-4.8.2/tests/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)   239461 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_bootstrap.json
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_bridge.json
--rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_camera.json
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_camera_heatmap.png
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_camera_snapshot.png
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_camera_thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (123)    50760 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_camera_video.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_chime.json
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_constants.json
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_doorlock.json
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_event_smart_track.json
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_light.json
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_liveview.json
--rw-r--r--   0 runner    (1001) docker     (123)   854579 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_raw_events.json
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_sensor.json
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_viewport.json
--rw-r--r--   0 runner    (1001) docker     (123)   159864 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_ws_messages.json
--rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/test_api_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/test_api_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.774006 pyunifiprotect-4.8.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/.bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      300 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.bin/format-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.bin/install-requirements
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/.bin/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.bin/lib/common.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.bin/lint-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.bin/test-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.bin/update-requirements
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/.docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.docker/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.758006 pyunifiprotect-4.8.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.github/workflows/test-live-AngellusMortis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/LIVE_DATA_CI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-29 16:01:30.774006 pyunifiprotect-4.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/TESTDATA.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/docs/dev.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/docs/overrides/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/docs/overrides/partials/toc-item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.762006 pyunifiprotect-4.8.3/pyunifiprotect/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47822 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.766006 pyunifiprotect-4.8.3/pyunifiprotect/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/chimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/doorlocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/lights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/liveviews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/cli/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.766006 pyunifiprotect-4.8.3/pyunifiprotect/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35653 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73235 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33721 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/data/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/release_cache.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.766006 pyunifiprotect-4.8.3/pyunifiprotect/test_util/
+-rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/test_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/test_util/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/pyunifiprotect/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.766006 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-29 16:01:30.000000 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-29 16:01:30.000000 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:01:30.000000 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-29 16:01:30.000000 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-29 16:01:30.000000 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 16:01:30.000000 pyunifiprotect-4.8.3/pyunifiprotect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 16:01:30.774006 pyunifiprotect-4.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.770006 pyunifiprotect-4.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22173 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.770006 pyunifiprotect-4.8.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27759 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_chime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24435 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_doorlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/data/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:30.774006 pyunifiprotect-4.8.3/tests/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239461 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_bootstrap.json
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_bridge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_camera.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_camera_heatmap.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_camera_snapshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_camera_thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50760 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_camera_video.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_chime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_constants.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_doorlock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_event_smart_track.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_light.json
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_liveview.json
+-rw-r--r--   0 runner    (1001) docker     (123)   854579 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_raw_events.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_sensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_viewport.json
+-rw-r--r--   0 runner    (1001) docker     (123)   159864 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/sample_data/sample_ws_messages.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/test_api_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/test_api_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-29 16:01:18.000000 pyunifiprotect-4.8.3/tests/test_utils.py
```

### Comparing `pyunifiprotect-4.8.2/.bin/lib/common.sh` & `pyunifiprotect-4.8.3/.bin/lib/common.sh`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/.bin/lint-code` & `pyunifiprotect-4.8.3/.bin/lint-code`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/.bin/update-requirements` & `pyunifiprotect-4.8.3/.bin/update-requirements`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/.devcontainer/devcontainer.json` & `pyunifiprotect-4.8.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/.github/workflows/ci.yaml` & `pyunifiprotect-4.8.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/.github/workflows/docker.yml` & `pyunifiprotect-4.8.3/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/.github/workflows/docs.yml` & `pyunifiprotect-4.8.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/.github/workflows/pypi.yml` & `pyunifiprotect-4.8.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/.github/workflows/test-live-AngellusMortis.yml` & `pyunifiprotect-4.8.3/.github/workflows/test-live-AngellusMortis.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/.gitignore` & `pyunifiprotect-4.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/.vscode/launch.json` & `pyunifiprotect-4.8.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/.vscode/tasks.json` & `pyunifiprotect-4.8.3/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/Dockerfile` & `pyunifiprotect-4.8.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/LICENSE` & `pyunifiprotect-4.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/LIVE_DATA_CI.md` & `pyunifiprotect-4.8.3/LIVE_DATA_CI.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/PKG-INFO` & `pyunifiprotect-4.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunifiprotect
-Version: 4.8.2
+Version: 4.8.3
 Summary: Unofficial UniFi Protect Python API and CLI
 Author-email: Bjarne Riis <bjarne@briis.com>, Christopher Bailey <cbailey@mort.is>
 Maintainer-email: Christopher Bailey <cbailey@mort.is>, "J. Nick Koston" <nick@koston.org>
 License: MIT
 Project-URL: Source Code, https://github.com/AngellusMortis/pyunifiprotect/
 Project-URL: Documentation, https://angellusmortis.github.io/pyunifiprotect/latest/
 Project-URL: Bug Reports, https://github.com/AngellusMortis/pyunifiprotect/issues/
```

### Comparing `pyunifiprotect-4.8.2/README.md` & `pyunifiprotect-4.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/TESTDATA.md` & `pyunifiprotect-4.8.3/TESTDATA.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/dev-requirements.txt` & `pyunifiprotect-4.8.3/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/docs/api.md` & `pyunifiprotect-4.8.3/docs/api.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/docs/cli.md` & `pyunifiprotect-4.8.3/docs/cli.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/docs/dev.md` & `pyunifiprotect-4.8.3/docs/dev.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/mkdocs.yml` & `pyunifiprotect-4.8.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyproject.toml` & `pyunifiprotect-4.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/api.py` & `pyunifiprotect-4.8.3/pyunifiprotect/api.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/cli/__init__.py` & `pyunifiprotect-4.8.3/pyunifiprotect/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/cli/backup.py` & `pyunifiprotect-4.8.3/pyunifiprotect/cli/backup.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/cli/base.py` & `pyunifiprotect-4.8.3/pyunifiprotect/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/cli/cameras.py` & `pyunifiprotect-4.8.3/pyunifiprotect/cli/cameras.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,16 +266,17 @@
             raise typer.Exit(1)
 
     if add:
         values = list(set(obj.smart_detect_settings.object_types) | set(values))
     elif remove:
         values = list(set(obj.smart_detect_settings.object_types) - set(values))
 
+    data_before_changes = obj.dict_with_excludes()
     obj.smart_detect_settings.object_types = values
-    base.run(ctx, obj.save_device())
+    base.run(ctx, obj.save_device(data_before_changes))
 
 
 @app.command()
 def smart_audio_detects(
     ctx: typer.Context,
     values: list[d.SmartDetectAudioType] = typer.Argument(None, help="Set to [] to empty list of detect types."),
     add: bool = typer.Option(False, "-a", "--add", help="Add values instead of set"),
@@ -317,16 +318,17 @@
             raise typer.Exit(1)
 
     if add:
         values = list(set(obj.smart_detect_settings.audio_types) | set(values))
     elif remove:
         values = list(set(obj.smart_detect_settings.audio_types) - set(values))
 
+    data_before_changes = obj.dict_with_excludes()
     obj.smart_detect_settings.audio_types = values
-    base.run(ctx, obj.save_device())
+    base.run(ctx, obj.save_device(data_before_changes))
 
 
 @app.command()
 def set_motion_detection(ctx: typer.Context, enabled: bool) -> None:
     """Sets motion detection on camera"""
 
     base.require_device_id(ctx)
```

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/cli/chimes.py` & `pyunifiprotect-4.8.3/pyunifiprotect/cli/chimes.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,17 @@
             raise typer.Exit(1)
 
     if add:
         camera_ids = list(set(obj.camera_ids) | set(camera_ids))
     elif remove:
         camera_ids = list(set(obj.camera_ids) - set(camera_ids))
 
+    data_before_changes = obj.dict_with_excludes()
     obj.camera_ids = camera_ids
-    base.run(ctx, obj.save_device())
+    base.run(ctx, obj.save_device(data_before_changes))
 
 
 @app.command()
 def play(ctx: typer.Context) -> None:
     """Plays chime tone."""
 
     base.require_device_id(ctx)
```

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/cli/doorlocks.py` & `pyunifiprotect-4.8.3/pyunifiprotect/cli/doorlocks.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/cli/events.py` & `pyunifiprotect-4.8.3/pyunifiprotect/cli/events.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/cli/lights.py` & `pyunifiprotect-4.8.3/pyunifiprotect/cli/lights.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/cli/liveviews.py` & `pyunifiprotect-4.8.3/pyunifiprotect/cli/liveviews.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/cli/nvr.py` & `pyunifiprotect-4.8.3/pyunifiprotect/cli/nvr.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/cli/sensors.py` & `pyunifiprotect-4.8.3/pyunifiprotect/cli/sensors.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/cli/viewers.py` & `pyunifiprotect-4.8.3/pyunifiprotect/cli/viewers.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/data/__init__.py` & `pyunifiprotect-4.8.3/pyunifiprotect/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/data/base.py` & `pyunifiprotect-4.8.3/pyunifiprotect/data/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 
     * Provides `.unifi_dict_to_dict` to convert UFP JSON to a more Pythonic formatted dict (camel case to snake case)
     * Add attrs with matching Pyhonic name and they will automatically be populated from the UFP JSON if passed in to the constructer
     * Provides `.unifi_dict` to convert object back into UFP JSON
     """
 
     _api: Optional[ProtectApiClient] = PrivateAttr(None)
-    _initial_data: Dict[str, Any] = PrivateAttr()
 
     _protect_objs: ClassVar[Optional[Dict[str, Type[ProtectBaseObject]]]] = None
     _protect_objs_set: ClassVar[Optional[SetStr]] = None
     _protect_lists: ClassVar[Optional[Dict[str, Type[ProtectBaseObject]]]] = None
     _protect_lists_set: ClassVar[Optional[SetStr]] = None
     _protect_dicts: ClassVar[Optional[Dict[str, Type[ProtectBaseObject]]]] = None
     _protect_dicts_set: ClassVar[Optional[SetStr]] = None
@@ -92,17 +91,14 @@
     def __init__(self, api: Optional[ProtectApiClient] = None, **data: Any) -> None:
         """
         Base class for creating Python objects from UFP JSON data.
 
         Use the static method `.from_unifi_dict()` to create objects from UFP JSON data from then the main class constructor.
         """
         super().__init__(**data)
-
-        excludes = self.__class__._get_excluded_changed_fields()  # pylint: disable=protected-access
-        self._initial_data = self.dict(exclude=excludes)
         self._api = api
 
     @classmethod
     def from_unifi_dict(cls, api: Optional[ProtectApiClient] = None, **data: Any) -> Self:
         """
         Main constructor for `ProtectBaseObject`
 
@@ -145,25 +141,24 @@
         for key in cls._get_protect_dicts_set().intersection(values_set):
             if isinstance(values[key], dict):
                 values[key] = {
                     k: unifi_dicts[key].construct(**v) if isinstance(v, dict) else v for k, v in values[key].items()
                 }
 
         obj = super().construct(_fields_set=_fields_set, **values)
-        obj._initial_data = obj.dict(exclude=cls._get_excluded_changed_fields())  # pylint: disable=protected-access
         obj._api = api  # pylint: disable=protected-access
 
         return obj
 
     @classmethod
     @cache
     def _get_excluded_changed_fields(cls) -> Set[str]:
         """
         Helper method for override in child classes for fields that excluded from calculating "changed" state for a
-        model (`.initial_data` and `.get_changed()`)
+        model (`.get_changed()`)
         """
         return set()
 
     @classmethod
     @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         """
@@ -497,20 +492,23 @@
 
         # Always injected above
         del data["api"]
 
         for key in data:
             setattr(self, key, convert_unifi_data(data[key], self.__fields__[key]))
 
-        excludes = self.__class__._get_excluded_changed_fields()  # pylint: disable=protected-access
-        self._initial_data = {k: v for k, v in self.__dict__.items() if k not in excludes}
         return self
 
-    def get_changed(self) -> Dict[str, Any]:
-        return dict_diff(self._initial_data, self.dict())
+    def dict_with_excludes(self) -> Dict[str, Any]:
+        """Returns a dict of the current object without any UFP objects converted to dicts."""
+        excludes = self.__class__._get_excluded_changed_fields()  # pylint: disable=protected-access
+        return self.dict(exclude=excludes)
+
+    def get_changed(self, data_before_changes: Dict[str, Any]) -> Dict[str, Any]:
+        return dict_diff(data_before_changes, self.dict())
 
     @property
     def api(self) -> ProtectApiClient:
         """
         ProtectApiClient that the UFP object was created with. If no API Client was passed in time of
         creation, will raise `BadRequest`
         """
@@ -573,20 +571,19 @@
     @classmethod
     def _get_read_only_fields(cls) -> Set[str]:
         return set()
 
     async def _api_update(self, data: Dict[str, Any]) -> None:
         raise NotImplementedError()
 
-    def revert_changes(self) -> None:
+    def revert_changes(self, data_before_changes: Dict[str, Any]) -> None:
         """Reverts current changes to device and resets it back to initial state"""
-
-        changed = self.get_changed()
+        changed = self.get_changed(data_before_changes)
         for key in changed.keys():
-            setattr(self, key, self._initial_data[key])
+            setattr(self, key, data_before_changes[key])
 
     def can_create(self, user: User) -> bool:
         if self.model is None:
             return True
 
         return user.can(self.model, PermissionNode.CREATE, self)
 
@@ -625,76 +622,97 @@
         try:
             async with timeout(0.05):
                 await self._update_event.wait()
             self._update_event.clear()
             return
         except asyncio.TimeoutError:
             async with self._update_lock:
+                # Important! Now that we have the lock, we yield to the event loop so any
+                # updates from the websocket are processed before we generate the diff
+                await asyncio.sleep(0)
+                # Save the initial data before we generate the diff
+                data_before_changes = self.dict_with_excludes()
                 while not self._update_queue.empty():
                     callback = self._update_queue.get_nowait()
                     callback()
-                await self.save_device()
-
-    async def save_device(self, force_emit: bool = False, revert_on_fail: bool = True) -> None:
+                # Important, do not yield to the event loop before generating the diff
+                # otherwise we may miss updates from the websocket
+                await self._save_device_changes(
+                    data_before_changes, self.unifi_dict(data=self.get_changed(data_before_changes))
+                )
+
+    async def save_device(
+        self, data_before_changes: Dict[str, Any], force_emit: bool = False, revert_on_fail: bool = True
+    ) -> None:
         """
         Generates a diff for unsaved changed on the device and sends them back to UFP
 
         USE WITH CAUTION, updates _all_ fields for the current object that have been changed.
         May have unexpected side effects.
 
         Tested updates have been added a methods on applicable devices.
 
         Args:
             force_emit: Emit a fake UFP WS message. Should only be use for when UFP does not properly emit a WS message
         """
-
         # do not allow multiple save_device calls at once
         release_lock = False
         if not self._update_lock.locked():
             await self._update_lock.acquire()
             release_lock = True
 
         try:
-            if self.model is None:
-                raise BadRequest("Unknown model type")
-
-            if not self.api.bootstrap.auth_user.can(self.model, PermissionNode.WRITE, self):
-                if revert_on_fail:
-                    self.revert_changes()
-                raise NotAuthorized(f"Do not have write permission for obj: {self.id}")
-
-            excludes = self.__class__._get_excluded_changed_fields()  # pylint: disable=protected-access
-            new_data = self.dict(exclude=excludes)
-            updated = self.unifi_dict(data=self.get_changed())
-
-            # do not patch when there are no updates
-            if updated == {}:
-                return
-
-            read_only_keys = self.__class__._get_read_only_fields().intersection(  # pylint: disable=protected-access
-                updated.keys()
+            await self._save_device_changes(
+                data_before_changes,
+                self.unifi_dict(data=self.get_changed(data_before_changes)),
+                force_emit=force_emit,
+                revert_on_fail=revert_on_fail,
             )
-            if len(read_only_keys) > 0:
-                self.revert_changes()
-                raise BadRequest(f"The following key(s) are read only: {read_only_keys}")
-
-            try:
-                await self._api_update(updated)
-            except ClientError:
-                if revert_on_fail:
-                    self.revert_changes()
-                raise
-            self._initial_data = new_data
-
-            if force_emit:
-                await self.emit_message(updated)
         finally:
             if release_lock:
                 self._update_lock.release()
 
+    async def _save_device_changes(
+        self,
+        data_before_changes: Dict[str, Any],
+        updated: Dict[str, Any],
+        force_emit: bool = False,
+        revert_on_fail: bool = True,
+    ) -> None:
+        """Saves the current device changes to UFP."""
+        assert self._update_lock.locked(), "save_device_changes should only be called when the update lock is held"
+        read_only_fields = self.__class__._get_read_only_fields()  # pylint: disable=protected-access
+
+        if self.model is None:
+            raise BadRequest("Unknown model type")
+
+        if not self.api.bootstrap.auth_user.can(self.model, PermissionNode.WRITE, self):
+            if revert_on_fail:
+                self.revert_changes(data_before_changes)
+            raise NotAuthorized(f"Do not have write permission for obj: {self.id}")
+
+        # do not patch when there are no updates
+        if updated == {}:
+            return
+
+        read_only_keys = read_only_fields.intersection(updated.keys())
+        if len(read_only_keys) > 0:
+            self.revert_changes(data_before_changes)
+            raise BadRequest(f"{type(self)} The following key(s) are read only: {read_only_keys}, updated: {updated}")
+
+        try:
+            await self._api_update(updated)
+        except ClientError:
+            if revert_on_fail:
+                self.revert_changes(data_before_changes)
+            raise
+
+        if force_emit:
+            await self.emit_message(updated)
+
     async def emit_message(self, updated: Dict[str, Any]) -> None:
         """Emites fake WS message for ProtectApiClient to process."""
 
         if updated == {}:
             _LOGGER.debug("Event ping callback started for %s", self.id)
 
         if self.model is None:
@@ -774,33 +792,33 @@
         def callback() -> None:
             self.name = name
 
         await self.queue_update(callback)
 
 
 class WiredConnectionState(ProtectBaseObject):
-    phy_rate: Optional[int]
+    phy_rate: Optional[float]
 
 
 class WirelessConnectionState(ProtectBaseObject):
     signal_quality: Optional[int]
     signal_strength: Optional[int]
 
 
 class BluetoothConnectionState(WirelessConnectionState):
     experience_score: Optional[PercentFloat] = None
 
 
 class WifiConnectionState(WirelessConnectionState):
-    phy_rate: Optional[int]
+    phy_rate: Optional[float]
     channel: Optional[int]
     frequency: Optional[int]
     ssid: Optional[str]
     bssid: Optional[str] = None
-    tx_rate: Optional[int] = None
+    tx_rate: Optional[float] = None
     # requires 2.7.5+
     ap_name: Optional[str] = None
     experience: Optional[str] = None
     # requires 2.7.15+
     connectivity: Optional[str] = None
 
 
@@ -906,22 +924,17 @@
 
     @property
     def is_adopted_by_us(self) -> bool:
         """Verifies device is adopted and controlled by this NVR."""
 
         return self.is_adopted and not self.is_adopted_by_other
 
-    def get_changed(self) -> Dict[str, Any]:
+    def get_changed(self, data_before_changes: Dict[str, Any]) -> Dict[str, Any]:
         """Gets dictionary of all changed fields"""
-
-        excludes = self.__class__._get_excluded_changed_fields()  # pylint: disable=protected-access
-        new_data = self.dict(exclude=excludes)
-        updated = dict_diff(self._initial_data, new_data)
-
-        return updated
+        return dict_diff(data_before_changes, self.dict_with_excludes())
 
     async def set_ssh(self, enabled: bool) -> None:
         """Sets ssh status for protect device"""
 
         def callback() -> None:
             self.is_ssh_enabled = enabled
```

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/data/bootstrap.py` & `pyunifiprotect-4.8.3/pyunifiprotect/data/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/data/convert.py` & `pyunifiprotect-4.8.3/pyunifiprotect/data/convert.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/data/devices.py` & `pyunifiprotect-4.8.3/pyunifiprotect/data/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """UniFi Protect Data."""
 from __future__ import annotations
 
+import asyncio
 from collections.abc import Iterable
 from datetime import datetime, timedelta
 from functools import cache
 from ipaddress import IPv4Address
 import logging
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Tuple, Union
@@ -133,19 +134,21 @@
 
         return self.api.bootstrap.cameras[self.camera_id]
 
     async def set_paired_camera(self, camera: Optional[Camera]) -> None:
         """Sets the camera paired with the light"""
 
         async with self._update_lock:
+            await asyncio.sleep(0)  # yield to the event loop once we have the lock to process any pending updates
+            data_before_changes = self.dict_with_excludes()
             if camera is None:
                 self.camera_id = None
             else:
                 self.camera_id = camera.id
-            await self.save_device(force_emit=True)
+            await self.save_device(data_before_changes, force_emit=True)
 
     async def set_status_light(self, enabled: bool) -> None:
         """Sets the status indicator light for the light"""
 
         def callback() -> None:
             self.light_device_settings.is_indicator_enabled = enabled
 
@@ -747,15 +750,15 @@
     is_deleting: bool
     # Microphone Sensitivity
     mic_volume: PercentInt
     is_mic_enabled: bool
     is_recording: bool
     is_motion_detected: bool
     is_smart_detected: bool
-    phy_rate: Optional[int]
+    phy_rate: Optional[float]
     hdr_mode: bool
     # Recording Quality -> High Frame
     video_mode: VideoMode
     is_probing_for_wifi: bool
     chime_duration: timedelta
     last_ring: Optional[datetime]
     is_live_heatmap_enabled: bool
@@ -893,16 +896,16 @@
         if "talkbackStream" in data:
             del data["talkbackStream"]
         if "lcdMessage" in data and data["lcdMessage"] is None:
             data["lcdMessage"] = {}
 
         return data
 
-    def get_changed(self) -> Dict[str, Any]:
-        updated = super().get_changed()
+    def get_changed(self, data_before_changes: Dict[str, Any]) -> Dict[str, Any]:
+        updated = super().get_changed(data_before_changes)
 
         if "lcd_message" in updated:
             lcd_message = updated["lcd_message"]
             # to "clear" LCD message, set reset_at to a time in the past
             if lcd_message is None:
                 updated["lcd_message"] = {"reset_at": utc_now() - timedelta(seconds=10)}
             # otherwise, pass full LCD message to prevent issues
@@ -1527,17 +1530,19 @@
         """Sets doorbell LCD text. Requires camera to be doorbell"""
 
         if not self.feature_flags.has_lcd_screen:
             raise BadRequest("Camera does not have an LCD screen")
 
         if text_type is None:
             async with self._update_lock:
+                await asyncio.sleep(0)  # yield to the event loop once we have the lock to process any pending updates
+                data_before_changes = self.dict_with_excludes()
                 self.lcd_message = None
                 # UniFi Protect bug: clearing LCD text message does _not_ emit a WS message
-                await self.save_device(force_emit=True)
+                await self.save_device(data_before_changes, force_emit=True)
                 return
 
         if text_type != DoorbellMessageType.CUSTOM_MESSAGE:
             if text is not None:
                 raise BadRequest("Can only set text if text_type is CUSTOM_MESSAGE")
             text = text_type.value.replace("_", " ")
 
@@ -1677,17 +1682,19 @@
         """
 
         if self._api is not None:
             if liveview.id not in self._api.bootstrap.liveviews:
                 raise BadRequest("Unknown liveview")
 
         async with self._update_lock:
+            await asyncio.sleep(0)  # yield to the event loop once we have the lock to process any pending updates
+            data_before_changes = self.dict_with_excludes()
             self.liveview_id = liveview.id
             # UniFi Protect bug: changing the liveview does _not_ emit a WS message
-            await self.save_device(force_emit=True)
+            await self.save_device(data_before_changes, force_emit=True)
 
 
 class Bridge(ProtectAdoptableDeviceModel):
     platform: str
 
 
 class SensorSettingsBase(ProtectBaseObject):
```

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/data/nvr.py` & `pyunifiprotect-4.8.3/pyunifiprotect/data/nvr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """UniFi Protect Data."""
 from __future__ import annotations
 
+import asyncio
 from datetime import datetime, timedelta, tzinfo
 from functools import cache
 from ipaddress import IPv4Address
 import logging
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
@@ -883,15 +884,14 @@
                 DoorbellMessage(
                     type=DoorbellMessageType.CUSTOM_MESSAGE,
                     text=message,
                 )
                 for message in messages
             ),
         ]
-        self._initial_data = self.dict()
 
     async def set_insights(self, enabled: bool) -> None:
         """Sets analytics collection for NVR"""
 
         def callback() -> None:
             self.is_insights_enabled = enabled
 
@@ -935,27 +935,35 @@
         if len(message) > 30:
             raise BadRequest("Message length over 30 characters")
 
         if message in self.doorbell_settings.custom_messages:
             raise BadRequest("Custom doorbell message already exists")
 
         async with self._update_lock:
+            await asyncio.sleep(
+                0
+            )  # yield to the event loop once we have the look to ensure websocket updates are processed
+            data_before_changes = self.dict_with_excludes()
             self.doorbell_settings.custom_messages.append(DoorbellText(message))
-            await self.save_device()
+            await self.save_device(data_before_changes)
             self.update_all_messages()
 
     async def remove_custom_doorbell_message(self, message: str) -> None:
         """Removes custom doorbell message"""
 
         if message not in self.doorbell_settings.custom_messages:
             raise BadRequest("Custom doorbell message does not exists")
 
         async with self._update_lock:
+            await asyncio.sleep(
+                0
+            )  # yield to the event loop once we have the look to ensure websocket updates are processed
+            data_before_changes = self.dict_with_excludes()
             self.doorbell_settings.custom_messages.remove(DoorbellText(message))
-            await self.save_device()
+            await self.save_device(data_before_changes)
             self.update_all_messages()
 
     async def reboot(self) -> None:
         """Reboots the NVR"""
 
         await self.api.reboot_nvr()
```

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/data/types.py` & `pyunifiprotect-4.8.3/pyunifiprotect/data/types.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/data/user.py` & `pyunifiprotect-4.8.3/pyunifiprotect/data/user.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/data/websocket.py` & `pyunifiprotect-4.8.3/pyunifiprotect/data/websocket.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/exceptions.py` & `pyunifiprotect-4.8.3/pyunifiprotect/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/stream.py` & `pyunifiprotect-4.8.3/pyunifiprotect/stream.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/test_util/__init__.py` & `pyunifiprotect-4.8.3/pyunifiprotect/test_util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/test_util/anonymize.py` & `pyunifiprotect-4.8.3/pyunifiprotect/test_util/anonymize.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/utils.py` & `pyunifiprotect-4.8.3/pyunifiprotect/utils.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect/websocket.py` & `pyunifiprotect-4.8.3/pyunifiprotect/websocket.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect.egg-info/PKG-INFO` & `pyunifiprotect-4.8.3/pyunifiprotect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunifiprotect
-Version: 4.8.2
+Version: 4.8.3
 Summary: Unofficial UniFi Protect Python API and CLI
 Author-email: Bjarne Riis <bjarne@briis.com>, Christopher Bailey <cbailey@mort.is>
 Maintainer-email: Christopher Bailey <cbailey@mort.is>, "J. Nick Koston" <nick@koston.org>
 License: MIT
 Project-URL: Source Code, https://github.com/AngellusMortis/pyunifiprotect/
 Project-URL: Documentation, https://angellusmortis.github.io/pyunifiprotect/latest/
 Project-URL: Bug Reports, https://github.com/AngellusMortis/pyunifiprotect/issues/
```

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect.egg-info/SOURCES.txt` & `pyunifiprotect-4.8.3/pyunifiprotect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/pyunifiprotect.egg-info/requires.txt` & `pyunifiprotect-4.8.3/pyunifiprotect.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/requirements.txt` & `pyunifiprotect-4.8.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/conftest.py` & `pyunifiprotect-4.8.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/data/test_camera.py` & `pyunifiprotect-4.8.3/tests/data/test_camera.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 async def test_camera_set_motion_detection(camera_obj: Optional[Camera], status: bool):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.recording_settings.enable_motion_detection = not status
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_motion_detection(status)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={"recordingSettings": {"enableMotionDetection": status}},
@@ -51,15 +50,14 @@
 async def test_camera_set_recording_mode(camera_obj: Optional[Camera], mode: RecordingMode):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.recording_settings.mode = RecordingMode.NEVER
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_recording_mode(mode)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={"recordingSettings": {"mode": mode.value}},
@@ -71,15 +69,14 @@
 async def test_camera_set_ir_led_model_no_ir(camera_obj: Optional[Camera]):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_led_ir = False
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_ir_led_model(IRLEDMode.AUTO)
 
     assert not camera_obj.api.api_request.called
 
 
@@ -90,15 +87,14 @@
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_led_ir = True
     camera_obj.isp_settings.ir_led_mode = IRLEDMode.OFF
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_ir_led_model(mode)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={"ispSettings": {"irLedMode": mode.value}},
@@ -110,15 +106,14 @@
 async def test_camera_set_status_light_no_status(camera_obj: Optional[Camera]):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_led_status = False
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_status_light(True)
 
     assert not camera_obj.api.api_request.called
 
 
@@ -130,15 +125,14 @@
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_led_status = True
     camera_obj.led_settings.is_enabled = not status
     camera_obj.led_settings.blink_rate = 10
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_status_light(status)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={"ledSettings": {"isEnabled": status, "blinkRate": 0}},
@@ -150,15 +144,14 @@
 async def test_camera_set_hdr_no_hdr(camera_obj: Optional[Camera]):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_hdr = False
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_hdr(True)
 
     assert not camera_obj.api.api_request.called
 
 
@@ -169,15 +162,14 @@
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_hdr = True
     camera_obj.hdr_mode = not status
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_hdr(status)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={"hdrMode": status},
@@ -190,15 +182,14 @@
 async def test_camera_set_ssh(camera_obj: Optional[Camera], status: bool):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.is_ssh_enabled = not status
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_ssh(status)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={"isSshEnabled": status},
@@ -211,15 +202,14 @@
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.video_modes = [VideoMode.DEFAULT]
     camera_obj.video_mode = VideoMode.DEFAULT
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_video_mode(VideoMode.HIGH_FPS)
 
     assert not camera_obj.api.api_request.called
 
 
@@ -229,15 +219,14 @@
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.video_modes = [VideoMode.DEFAULT, VideoMode.HIGH_FPS]
     camera_obj.video_mode = VideoMode.DEFAULT
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_video_mode(VideoMode.HIGH_FPS)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={"videoMode": VideoMode.HIGH_FPS.value},
@@ -249,15 +238,14 @@
 async def test_camera_set_camera_zoom_no_zoom(camera_obj: Optional[Camera]):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.can_optical_zoom = False
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_camera_zoom(True)
 
     assert not camera_obj.api.api_request.called
 
 
@@ -268,15 +256,14 @@
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.can_optical_zoom = True
     camera_obj.isp_settings.zoom_position = 10
-    camera_obj._initial_data = camera_obj.dict()
 
     if level in (-1, 200):
         with pytest.raises(ValidationError):
             await camera_obj.set_camera_zoom(level)
 
         assert not camera_obj.api.api_request.called
     else:
@@ -296,15 +283,14 @@
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_hdr = False
     camera_obj.isp_settings.wdr = 2
-    camera_obj._initial_data = camera_obj.dict()
 
     if level in (-1, 4):
         with pytest.raises(ValidationError):
             await camera_obj.set_wdr_level(level)
 
             assert not camera_obj.api.api_request.called
     else:
@@ -322,15 +308,14 @@
 async def test_camera_set_wdr_level_hdr(camera_obj: Optional[Camera]):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_hdr = True
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_wdr_level(1)
 
     assert not camera_obj.api.api_request.called
 
 
@@ -339,15 +324,14 @@
 async def test_camera_set_mic_volume_no_mic(camera_obj: Optional[Camera]):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_mic = False
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_mic_volume(True)
 
     assert not camera_obj.api.api_request.called
 
 
@@ -358,15 +342,14 @@
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_mic = True
     camera_obj.mic_volume = 10
-    camera_obj._initial_data = camera_obj.dict()
 
     if level in (-1, 200):
         with pytest.raises(ValidationError):
             await camera_obj.set_mic_volume(level)
 
         assert not camera_obj.api.api_request.called
     else:
@@ -384,15 +367,14 @@
 async def test_camera_set_speaker_volume_no_speaker(camera_obj: Optional[Camera]):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_speaker = False
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_speaker_volume(True)
 
     assert not camera_obj.api.api_request.called
 
 
@@ -403,15 +385,14 @@
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_speaker = True
     camera_obj.speaker_settings.volume = 10
-    camera_obj._initial_data = camera_obj.dict()
 
     if level in (-1, 200):
         with pytest.raises(ValidationError):
             await camera_obj.set_speaker_volume(level)
 
         assert not camera_obj.api.api_request.called
     else:
@@ -429,15 +410,14 @@
 async def test_camera_set_chime_duration_no_chime(camera_obj: Optional[Camera]):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_chime = False
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_chime_duration(1000)
 
     assert not camera_obj.api.api_request.called
 
 
@@ -449,15 +429,14 @@
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_chime = True
     camera_obj.chime_duration = 300
     camera_obj.mic_volume = 10
-    camera_obj._initial_data = camera_obj.dict()
 
     if duration in (-1, 20):
         with pytest.raises(BadRequest):
             await camera_obj.set_chime_duration(duration)
 
         assert not camera_obj.api.api_request.called
     else:
@@ -475,15 +454,14 @@
 async def test_camera_set_system_sounds_no_speaker(camera_obj: Optional[Camera]):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_speaker = False
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_system_sounds(True)
 
     assert not camera_obj.api.api_request.called
 
 
@@ -494,15 +472,14 @@
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_speaker = True
     camera_obj.speaker_settings.are_system_sounds_enabled = not status
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_system_sounds(status)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={"speakerSettings": {"areSystemSoundsEnabled": status}},
@@ -515,15 +492,14 @@
 async def test_camera_set_osd_name(camera_obj: Optional[Camera], status: bool):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.osd_settings.is_name_enabled = not status
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_osd_name(status)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={"osdSettings": {"isNameEnabled": status}},
@@ -536,15 +512,14 @@
 async def test_camera_set_osd_date(camera_obj: Optional[Camera], status: bool):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.osd_settings.is_date_enabled = not status
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_osd_date(status)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={"osdSettings": {"isDateEnabled": status}},
@@ -557,15 +532,14 @@
 async def test_camera_set_osd_logo(camera_obj: Optional[Camera], status: bool):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.osd_settings.is_logo_enabled = not status
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_osd_logo(status)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={"osdSettings": {"isLogoEnabled": status}},
@@ -578,15 +552,14 @@
 async def test_camera_set_osd_bitrate(camera_obj: Optional[Camera], status: bool):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.osd_settings.is_debug_enabled = not status
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_osd_bitrate(status)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={"osdSettings": {"isDebugEnabled": status}},
@@ -598,15 +571,14 @@
 async def test_camera_set_smart_detect_types_no_smart(camera_obj: Optional[Camera]):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_smart_detect = False
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_smart_detect_types([])
 
     assert not camera_obj.api.api_request.called
 
 
@@ -616,15 +588,14 @@
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_smart_detect = True
     camera_obj.smart_detect_settings.object_types = []
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_smart_detect_types([SmartDetectObjectType.PERSON])
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={"smartDetectSettings": {"objectTypes": ["person"]}},
@@ -636,15 +607,14 @@
 async def test_camera_set_lcd_text_no_lcd(camera_obj: Optional[Camera]):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_lcd_screen = False
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_lcd_text(DoorbellMessageType.DO_NOT_DISTURB)
 
     assert not camera_obj.api.api_request.called
 
 
@@ -655,15 +625,14 @@
 
     camera_obj.feature_flags.has_lcd_screen = True
     camera_obj.lcd_message = LCDMessage(
         type=DoorbellMessageType.DO_NOT_DISTURB,
         text=DoorbellMessageType.DO_NOT_DISTURB.value.replace("_", " "),
         reset_at=None,
     )
-    camera_obj._initial_data = camera_obj.dict()
 
     now = datetime.utcnow()
     await camera_obj.set_lcd_text(DoorbellMessageType.CUSTOM_MESSAGE, "Test", now)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
@@ -684,15 +653,14 @@
 
     camera_obj.feature_flags.has_lcd_screen = True
     camera_obj.lcd_message = LCDMessage(
         type=DoorbellMessageType.CUSTOM_MESSAGE,
         text="Welcome",
         reset_at=None,
     )
-    camera_obj._initial_data = camera_obj.dict()
 
     now = datetime.utcnow()
     await camera_obj.set_lcd_text(DoorbellMessageType.CUSTOM_MESSAGE, "Test", now)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
@@ -711,15 +679,14 @@
 async def test_camera_set_lcd_text_invalid_text(camera_obj: Optional[Camera]):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_lcd_screen = True
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_lcd_text(DoorbellMessageType.DO_NOT_DISTURB, "Test")
 
     assert not camera_obj.api.api_request.called
 
 
@@ -733,15 +700,14 @@
 
     camera_obj.feature_flags.has_lcd_screen = True
     camera_obj.lcd_message = LCDMessage(
         type=DoorbellMessageType.DO_NOT_DISTURB,
         text=DoorbellMessageType.DO_NOT_DISTURB.value.replace("_", " "),
         reset_at=None,
     )
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_lcd_text(DoorbellMessageType.LEAVE_PACKAGE_AT_DOOR)
 
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
         json={
@@ -768,15 +734,14 @@
 
     camera_obj.feature_flags.has_lcd_screen = True
     camera_obj.lcd_message = LCDMessage(
         type=DoorbellMessageType.DO_NOT_DISTURB,
         text=DoorbellMessageType.DO_NOT_DISTURB.value.replace("_", " "),
         reset_at=None,
     )
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_lcd_text(None)
 
     expected_dt = now - timedelta(seconds=10)
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
@@ -813,15 +778,14 @@
 
     camera_obj.feature_flags.has_lcd_screen = True
     camera_obj.lcd_message = LCDMessage(
         type=DoorbellMessageType.DO_NOT_DISTURB,
         text=DoorbellMessageType.DO_NOT_DISTURB.value.replace("_", " "),
         reset_at=None,
     )
-    camera_obj._initial_data = camera_obj.dict()
 
     await camera_obj.set_lcd_text(DoorbellMessageType.LEAVE_PACKAGE_AT_DOOR, reset_at=DEFAULT)
 
     expected_dt = now + camera_obj.api.bootstrap.nvr.doorbell_settings.default_message_reset_timeout
     camera_obj.api.api_request.assert_called_with(
         f"cameras/{camera_obj.id}",
         method="patch",
@@ -840,15 +804,14 @@
 async def test_camera_set_privacy_no_privacy(camera_obj: Optional[Camera]):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     camera_obj.api.api_request.reset_mock()
 
     camera_obj.feature_flags.has_privacy_mask = False
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.set_privacy(True)
 
     assert not camera_obj.api.api_request.called
 
 
@@ -872,15 +835,14 @@
 
     camera_obj.feature_flags.has_privacy_mask = True
     camera_obj.privacy_zones = []
     if actual_enabled:
         camera_obj.add_privacy_zone()
     camera_obj.mic_volume = 10
     camera_obj.recording_settings.mode = RecordingMode.NEVER
-    camera_obj._initial_data = camera_obj.dict()
 
     if level in (-1, 200):
         with pytest.raises(ValidationError):
             await camera_obj.set_privacy(enabled, level, mode)
 
         assert not camera_obj.api.api_request.called
     else:
```

### Comparing `pyunifiprotect-4.8.2/tests/data/test_chime.py` & `pyunifiprotect-4.8.3/tests/data/test_chime.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 @pytest.mark.asyncio
 async def test_chime_set_volume(chime_obj: Optional[Chime], level: int):
     if chime_obj is None:
         pytest.skip("No chime_obj obj found")
 
     chime_obj.api.api_request.reset_mock()
     chime_obj.volume = 20
-    chime_obj._initial_data = chime_obj.dict()
 
     if level in (-1, 200):
         with pytest.raises(ValidationError):
             await chime_obj.set_volume(level)
 
         assert not chime_obj.api.api_request.called
     else:
@@ -72,19 +71,17 @@
     if chime_obj is None:
         pytest.skip("No chime_obj obj found")
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     chime_obj.api.api_request.reset_mock()
     chime_obj.camera_ids = []
-    chime_obj._initial_data = chime_obj.dict()
 
     camera_obj.api.api_request.reset_mock()
     camera_obj.feature_flags.is_doorbell = True
-    camera_obj._initial_data = chime_obj.dict()
 
     await chime_obj.add_camera(camera_obj)
 
     chime_obj.api.api_request.assert_called_with(
         f"chimes/{chime_obj.id}",
         method="patch",
         json={"cameraIds": [camera_obj.id]},
@@ -97,19 +94,17 @@
     if chime_obj is None:
         pytest.skip("No chime_obj obj found")
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     chime_obj.api.api_request.reset_mock()
     chime_obj.camera_ids = []
-    chime_obj._initial_data = chime_obj.dict()
 
     camera_obj.api.api_request.reset_mock()
     camera_obj.feature_flags.is_doorbell = False
-    camera_obj._initial_data = chime_obj.dict()
 
     with pytest.raises(BadRequest):
         await chime_obj.add_camera(camera_obj)
 
     assert not chime_obj.api.api_request.called
 
 
@@ -119,19 +114,17 @@
     if chime_obj is None:
         pytest.skip("No chime_obj obj found")
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     chime_obj.api.api_request.reset_mock()
     chime_obj.camera_ids = [camera_obj.id]
-    chime_obj._initial_data = chime_obj.dict()
 
     camera_obj.api.api_request.reset_mock()
     camera_obj.feature_flags.is_doorbell = True
-    camera_obj._initial_data = chime_obj.dict()
 
     with pytest.raises(BadRequest):
         await chime_obj.add_camera(camera_obj)
 
     assert not chime_obj.api.api_request.called
 
 
@@ -141,19 +134,17 @@
     if chime_obj is None:
         pytest.skip("No chime_obj obj found")
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     chime_obj.api.api_request.reset_mock()
     chime_obj.camera_ids = [camera_obj.id]
-    chime_obj._initial_data = chime_obj.dict()
 
     camera_obj.api.api_request.reset_mock()
     camera_obj.feature_flags.is_doorbell = True
-    camera_obj._initial_data = chime_obj.dict()
 
     await chime_obj.remove_camera(camera_obj)
 
     chime_obj.api.api_request.assert_called_with(
         f"chimes/{chime_obj.id}",
         method="patch",
         json={"cameraIds": []},
@@ -166,17 +157,15 @@
     if chime_obj is None:
         pytest.skip("No chime_obj obj found")
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     chime_obj.api.api_request.reset_mock()
     chime_obj.camera_ids = []
-    chime_obj._initial_data = chime_obj.dict()
 
     camera_obj.api.api_request.reset_mock()
     camera_obj.feature_flags.is_doorbell = True
-    camera_obj._initial_data = chime_obj.dict()
 
     with pytest.raises(BadRequest):
         await chime_obj.remove_camera(camera_obj)
 
     assert not chime_obj.api.api_request.called
```

### Comparing `pyunifiprotect-4.8.2/tests/data/test_common.py` & `pyunifiprotect-4.8.3/tests/data/test_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -289,39 +289,36 @@
     assert VideoMode("highFps") == VideoMode.HIGH_FPS
     assert RecordingType("roTating") == RecordingType.CONTINUOUS
 
 
 @pytest.mark.asyncio
 async def test_play_audio_no_speaker(camera_obj: Camera):
     camera_obj.feature_flags.has_speaker = False
-    camera_obj._initial_data = camera_obj.dict()
 
     with pytest.raises(BadRequest):
         await camera_obj.play_audio("test")
 
 
 @pytest.mark.asyncio
 @pytest.mark.usefixtures("disable_camera_validation")
 async def test_play_audio_already_playing(camera_obj: Camera):
     camera_obj.feature_flags.has_speaker = True
-    camera_obj._initial_data = camera_obj.dict()
 
     camera_obj.talkback_stream = Mock()
     camera_obj.talkback_stream.is_running = True
 
     with pytest.raises(BadRequest):
         await camera_obj.play_audio("test")
 
 
 @pytest.mark.asyncio
 @pytest.mark.usefixtures("disable_camera_validation")
 @patch("pyunifiprotect.data.devices.TalkbackStream")
 async def test_play_audio(mock_talkback, camera_obj: Camera):
     camera_obj.feature_flags.has_speaker = True
-    camera_obj._initial_data = camera_obj.dict()
 
     mock_instance = MockTalkback()
     mock_talkback.return_value = mock_instance
 
     await camera_obj.play_audio("test")
 
     mock_talkback.assert_called_with(camera_obj, "test", None)
@@ -330,15 +327,14 @@
 
 
 @pytest.mark.asyncio
 @pytest.mark.usefixtures("disable_camera_validation")
 @patch("pyunifiprotect.data.devices.TalkbackStream")
 async def test_play_audio_no_blocking(mock_talkback, camera_obj: Camera):
     camera_obj.feature_flags.has_speaker = True
-    camera_obj._initial_data = camera_obj.dict()
 
     mock_instance = MockTalkback()
     mock_talkback.return_value = mock_instance
 
     await camera_obj.play_audio("test", blocking=False)
 
     mock_talkback.assert_called_with(camera_obj, "test", None)
@@ -350,15 +346,14 @@
 
 
 @pytest.mark.asyncio
 @pytest.mark.usefixtures("disable_camera_validation")
 @patch("pyunifiprotect.data.devices.TalkbackStream")
 async def test_play_audio_stop(mock_talkback, camera_obj: Camera):
     camera_obj.feature_flags.has_speaker = True
-    camera_obj._initial_data = camera_obj.dict()
 
     mock_instance = MockTalkback()
     mock_talkback.return_value = mock_instance
 
     await camera_obj.play_audio("test", blocking=False)
 
     mock_talkback.assert_called_with(camera_obj, "test", None)
@@ -370,15 +365,14 @@
 
 
 @pytest.mark.asyncio
 @pytest.mark.usefixtures("disable_camera_validation")
 @patch("pyunifiprotect.data.devices.TalkbackStream")
 async def test_play_audio_error(mock_talkback, camera_obj: Camera):
     camera_obj.feature_flags.has_speaker = True
-    camera_obj._initial_data = camera_obj.dict()
 
     mock_instance = MockTalkback()
     mock_instance.is_error = True
     mock_talkback.return_value = mock_instance
 
     with pytest.raises(StreamError):
         await camera_obj.play_audio("test")
@@ -468,15 +462,17 @@
 
 
 @pytest.mark.skipif(not TEST_CAMERA_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_save_device_no_changes(camera_obj: Camera):
     camera_obj.api.api_request.reset_mock()  # type: ignore
 
-    await camera_obj.save_device()
+    data_before_changes = camera_obj.dict_with_excludes()
+
+    await camera_obj.save_device(data_before_changes)
 
     assert not camera_obj.api.api_request.called  # type: ignore
 
 
 @pytest.mark.skipif(not TEST_CAMERA_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_device_reboot(camera_obj: Camera):
@@ -519,17 +515,15 @@
     can_delete_media: bool,
 ):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     api = user_obj.api
     user_obj.all_permissions = [Permission.from_unifi_dict(rawPermission=p, api=api) for p in permissions]
-    user_obj._initial_data = user_obj.dict()
     camera_obj.id = "test_id_1"
-    camera_obj._initial_data = camera_obj.dict()
     api.bootstrap.cameras[camera_obj.id] = camera_obj
 
     assert camera_obj.can_create(user_obj) is can_create
     assert camera_obj.can_read(user_obj) is can_read
     assert camera_obj.can_write(user_obj) is can_write
     assert camera_obj.can_delete(user_obj) is can_delete
     assert camera_obj.can_read_media(user_obj) is can_read_media
@@ -559,15 +553,14 @@
     can_delete: bool,
 ):
     api = user_obj.api
 
     user1 = user_obj.copy()
     user1.id = "test_id_1"
     user1.all_permissions = [Permission.from_unifi_dict(rawPermission=p, api=api) for p in permissions]
-    user1._initial_data = user1.dict()
 
     api.bootstrap.auth_user_id = user1.id
     api.bootstrap.users = {user1.id: user1}
 
     assert user1.can_create(user1) is can_create
     assert user1.can_read(user1) is can_read
     assert user1.can_write(user1) is can_write
@@ -597,19 +590,17 @@
     can_delete: bool,
 ):
     api = user_obj.api
 
     user1 = user_obj.copy()
     user1.id = "test_id_1"
     user1.all_permissions = [Permission.from_unifi_dict(rawPermission=p, api=api) for p in permissions]
-    user1._initial_data = user1.dict()
 
     user2 = user_obj.copy()
     user2.id = "test_id_2"
-    user2._initial_data = user2.dict()
 
     api.bootstrap.auth_user_id = user1.id
     api.bootstrap.users = {user1.id: user1, user2.id: user2}
 
     assert user2.can_create(user1) is can_create
     assert user2.can_read(user1) is can_read
     assert user2.can_write(user1) is can_write
@@ -622,41 +613,38 @@
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     api = user_obj.api
     camera_obj.id = "test_id_1"
     camera_obj.add_privacy_zone()
     camera_obj.recording_settings.mode = RecordingMode.NEVER
-    camera_obj._initial_data = camera_obj.dict()
     api.bootstrap.cameras[camera_obj.id] = camera_obj
 
     user_obj.all_permissions = [Permission.from_unifi_dict(rawPermission="camera:read:*", api=api)]
-    user_obj._initial_data = user_obj.dict()
 
     camera_before = camera_obj.dict()
 
     camera_obj.remove_privacy_zone()
     camera_obj.recording_settings.mode = RecordingMode.ALWAYS
     with pytest.raises(NotAuthorized):
-        await camera_obj.save_device()
+        await camera_obj.save_device(camera_before)
 
     assert camera_before == camera_obj.dict()
 
 
 @pytest.mark.skipif(not TEST_CAMERA_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_multiple_updates(user_obj: User, camera_obj: Camera):
     if camera_obj is None:
         pytest.skip("No camera_obj obj found")
 
     api = user_obj.api
     camera_obj.id = "test_id_1"
     camera_obj.recording_settings.enable_motion_detection = False
     camera_obj.smart_detect_settings.object_types = []
-    camera_obj._initial_data = camera_obj.dict()
     api.bootstrap.cameras[camera_obj.id] = camera_obj
 
     await asyncio.gather(
         camera_obj.set_motion_detection(True),
         camera_obj.set_person_detection(True),
         camera_obj.set_vehicle_detection(True),
     )
```

### Comparing `pyunifiprotect-4.8.2/tests/data/test_doorlock.py` & `pyunifiprotect-4.8.3/tests/data/test_doorlock.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 @pytest.mark.skipif(not TEST_DOORLOCK_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_doorlock_set_paired_camera_none(doorlock_obj: Doorlock):
     doorlock_obj.api.api_request.reset_mock()
 
     doorlock_obj.camera_id = "bad_id"
-    doorlock_obj._initial_data = doorlock_obj.dict()
 
     await doorlock_obj.set_paired_camera(None)
 
     doorlock_obj.api.api_request.assert_called_with(
         f"doorlocks/{doorlock_obj.id}",
         method="patch",
         json={"camera": None},
@@ -32,15 +31,14 @@
 
 @pytest.mark.skipif(not TEST_DOORLOCK_EXISTS or not TEST_CAMERA_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_doorlock_set_paired_camera(doorlock_obj: Light, camera_obj: Camera):
     doorlock_obj.api.api_request.reset_mock()
 
     doorlock_obj.camera_id = None
-    doorlock_obj._initial_data = doorlock_obj.dict()
 
     await doorlock_obj.set_paired_camera(camera_obj)
 
     doorlock_obj.api.api_request.assert_called_with(
         f"doorlocks/{doorlock_obj.id}",
         method="patch",
         json={"camera": camera_obj.id},
@@ -50,15 +48,14 @@
 @pytest.mark.skipif(not TEST_DOORLOCK_EXISTS, reason="Missing testdata")
 @pytest.mark.parametrize("status", [True, False])
 @pytest.mark.asyncio
 async def test_doorlock_set_status_light(doorlock_obj: Doorlock, status: bool):
     doorlock_obj.api.api_request.reset_mock()
 
     doorlock_obj.led_settings.is_enabled = not status
-    doorlock_obj._initial_data = doorlock_obj.dict()
 
     await doorlock_obj.set_status_light(status)
 
     doorlock_obj.api.api_request.assert_called_with(
         f"doorlocks/{doorlock_obj.id}",
         method="patch",
         json={"ledSettings": {"isEnabled": status}},
@@ -79,15 +76,14 @@
 async def test_doorlock_set_auto_close_time(
     doorlock_obj: Doorlock,
     duration: timedelta,
 ):
     doorlock_obj.api.api_request.reset_mock()
 
     doorlock_obj.auto_close_time = timedelta(seconds=30)
-    doorlock_obj._initial_data = doorlock_obj.dict()
 
     duration_invalid = duration is not None and int(duration.total_seconds()) == 3601
     if duration_invalid:
         with pytest.raises(BadRequest):
             await doorlock_obj.set_auto_close_time(duration)
 
             assert not doorlock_obj.api.api_request.called
@@ -105,15 +101,14 @@
 
 @pytest.mark.skipif(not TEST_DOORLOCK_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_doorlock_close(doorlock_obj: Doorlock):
     doorlock_obj.api.api_request.reset_mock()
 
     doorlock_obj.lock_status = LockStatusType.OPEN
-    doorlock_obj._initial_data = doorlock_obj.dict()
 
     await doorlock_obj.close_lock()
 
     doorlock_obj.api.api_request.assert_called_with(
         f"doorlocks/{doorlock_obj.id}/close",
         method="post",
     )
@@ -121,29 +116,27 @@
 
 @pytest.mark.skipif(not TEST_DOORLOCK_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_doorlock_close_invalid(doorlock_obj: Doorlock):
     doorlock_obj.api.api_request.reset_mock()
 
     doorlock_obj.lock_status = LockStatusType.CLOSED
-    doorlock_obj._initial_data = doorlock_obj.dict()
 
     with pytest.raises(BadRequest):
         await doorlock_obj.close_lock()
 
     assert not doorlock_obj.api.api_request.called
 
 
 @pytest.mark.skipif(not TEST_DOORLOCK_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_doorlock_open(doorlock_obj: Doorlock):
     doorlock_obj.api.api_request.reset_mock()
 
     doorlock_obj.lock_status = LockStatusType.CLOSED
-    doorlock_obj._initial_data = doorlock_obj.dict()
 
     await doorlock_obj.open_lock()
 
     doorlock_obj.api.api_request.assert_called_with(
         f"doorlocks/{doorlock_obj.id}/open",
         method="post",
     )
@@ -151,13 +144,12 @@
 
 @pytest.mark.skipif(not TEST_DOORLOCK_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_doorlock_open_invalid(doorlock_obj: Doorlock):
     doorlock_obj.api.api_request.reset_mock()
 
     doorlock_obj.lock_status = LockStatusType.OPEN
-    doorlock_obj._initial_data = doorlock_obj.dict()
 
     with pytest.raises(BadRequest):
         await doorlock_obj.open_lock()
 
     assert not doorlock_obj.api.api_request.called
```

### Comparing `pyunifiprotect-4.8.2/tests/data/test_light.py` & `pyunifiprotect-4.8.3/tests/data/test_light.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 @pytest.mark.skipif(not TEST_LIGHT_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_light_set_paired_camera_none(light_obj: Light):
     light_obj.api.api_request.reset_mock()
 
     light_obj.camera_id = "bad_id"
-    light_obj._initial_data = light_obj.dict()
 
     await light_obj.set_paired_camera(None)
 
     light_obj.api.api_request.assert_called_with(
         f"lights/{light_obj.id}",
         method="patch",
         json={"camera": None},
@@ -33,15 +32,14 @@
 
 @pytest.mark.skipif(not TEST_LIGHT_EXISTS or not TEST_CAMERA_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_light_set_paired_camera(light_obj: Light, camera_obj: Camera):
     light_obj.api.api_request.reset_mock()
 
     light_obj.camera_id = None
-    light_obj._initial_data = light_obj.dict()
 
     await light_obj.set_paired_camera(camera_obj)
 
     light_obj.api.api_request.assert_called_with(
         f"lights/{light_obj.id}",
         method="patch",
         json={"camera": camera_obj.id},
@@ -51,15 +49,14 @@
 @pytest.mark.skipif(not TEST_LIGHT_EXISTS, reason="Missing testdata")
 @pytest.mark.parametrize("status", [True, False])
 @pytest.mark.asyncio
 async def test_light_set_status_light(light_obj: Light, status: bool):
     light_obj.api.api_request.reset_mock()
 
     light_obj.light_device_settings.is_indicator_enabled = not status
-    light_obj._initial_data = light_obj.dict()
 
     await light_obj.set_status_light(status)
 
     light_obj.api.api_request.assert_called_with(
         f"lights/{light_obj.id}",
         method="patch",
         json={"lightDeviceSettings": {"isIndicatorEnabled": status}},
@@ -69,15 +66,14 @@
 @pytest.mark.skipif(not TEST_LIGHT_EXISTS, reason="Missing testdata")
 @pytest.mark.parametrize("level", [-1, 1, 3, 6, 7])
 @pytest.mark.asyncio
 async def test_light_set_led_level(light_obj: Light, level: int):
     light_obj.api.api_request.reset_mock()
 
     light_obj.light_device_settings.led_level = 2
-    light_obj._initial_data = light_obj.dict()
 
     if level in (-1, 7):
         with pytest.raises(ValidationError):
             await light_obj.set_led_level(level)
 
             assert not light_obj.api.api_request.called
     else:
@@ -96,15 +92,14 @@
 @pytest.mark.asyncio
 async def test_light_set_light(light_obj: Light, status: bool, level: Optional[int]):
     light_obj.api.api_request.reset_mock()
 
     light_obj.light_on_settings.is_led_force_on = not status
     if level is not None:
         light_obj.light_device_settings.led_level = 2
-    light_obj._initial_data = light_obj.dict()
 
     if level in (-1, 7):
         with pytest.raises(ValidationError):
             await light_obj.set_light(status, level)
 
             assert not light_obj.api.api_request.called
     else:
@@ -128,15 +123,14 @@
 async def test_light_set_sensitivity(
     light_obj: Light,
     sensitivity: int,
 ):
     light_obj.api.api_request.reset_mock()
 
     light_obj.light_device_settings.pir_sensitivity = 50
-    light_obj._initial_data = light_obj.dict()
 
     if sensitivity == -10:
         with pytest.raises(ValidationError):
             await light_obj.set_sensitivity(sensitivity)
 
             assert not light_obj.api.api_request.called
     else:
@@ -165,15 +159,14 @@
 async def test_light_set_duration(
     light_obj: Light,
     duration: timedelta,
 ):
     light_obj.api.api_request.reset_mock()
 
     light_obj.light_device_settings.pir_duration = timedelta(seconds=30)
-    light_obj._initial_data = light_obj.dict()
 
     duration_invalid = duration is not None and int(duration.total_seconds()) in (1, 1000)
     if duration_invalid:
         with pytest.raises(BadRequest):
             await light_obj.set_duration(duration)
 
             assert not light_obj.api.api_request.called
@@ -213,15 +206,14 @@
 ):
     light_obj.api.api_request.reset_mock()
 
     light_obj.light_mode_settings.mode = LightModeType.MOTION
     light_obj.light_mode_settings.enable_at = LightModeEnableType.DARK
     light_obj.light_device_settings.pir_duration = timedelta(seconds=30)
     light_obj.light_device_settings.pir_sensitivity = 50
-    light_obj._initial_data = light_obj.dict()
 
     duration_invalid = duration is not None and int(duration.total_seconds()) in (1, 1000)
     if duration_invalid:
         with pytest.raises(BadRequest):
             await light_obj.set_light_settings(mode, enable_at=enable_at, duration=duration, sensitivity=sensitivity)
 
             assert not light_obj.api.api_request.called
```

### Comparing `pyunifiprotect-4.8.2/tests/data/test_nvr.py` & `pyunifiprotect-4.8.3/tests/data/test_nvr.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 @pytest.mark.parametrize("status", [True, False])
 @pytest.mark.asyncio
 async def test_nvr_set_insights(nvr_obj: NVR, status: bool):
     nvr_obj.api.api_request.reset_mock()
 
     nvr_obj.is_insights_enabled = not status
-    nvr_obj._initial_data = nvr_obj.dict()
 
     await nvr_obj.set_insights(status)
 
     nvr_obj.api.api_request.assert_called_with(
         "nvr",
         method="patch",
         json={"isInsightsEnabled": status},
@@ -34,15 +33,14 @@
 
 
 @pytest.mark.asyncio
 async def test_nvr_set_anonymous_analytics(nvr_obj: NVR):
     nvr_obj.api.api_request.reset_mock()
 
     nvr_obj.analytics_data = AnalyticsOption.ANONYMOUS
-    nvr_obj._initial_data = nvr_obj.dict()
 
     await nvr_obj.set_anonymous_analytics(False)
 
     nvr_obj.api.api_request.assert_called_with(
         "nvr",
         method="patch",
         json={"analyticsData": "none"},
@@ -85,15 +83,14 @@
 
 @pytest.mark.parametrize("message", ["Welcome", "Test", "fqthpqBgVMKXp9jXX2VeuGeXYfx2mMjB"])
 @pytest.mark.asyncio
 async def test_nvr_add_custom_doorbell_message(nvr_obj: NVR, message: str):
     nvr_obj.api.api_request.reset_mock()
 
     nvr_obj.doorbell_settings.custom_messages = ["Welcome"]
-    nvr_obj._initial_data = nvr_obj.dict()
 
     if message != "Test":
         with pytest.raises(BadRequest):
             await nvr_obj.add_custom_doorbell_message(message)
 
         assert not nvr_obj.api.api_request.called
     else:
@@ -125,15 +122,14 @@
 
 @pytest.mark.parametrize("message", ["Welcome", "Test"])
 @pytest.mark.asyncio
 async def test_nvr_remove_custom_doorbell_message(nvr_obj: NVR, message: str):
     nvr_obj.api.api_request.reset_mock()
 
     nvr_obj.doorbell_settings.custom_messages = ["Welcome"]
-    nvr_obj._initial_data = nvr_obj.dict()
 
     if message == "Test":
         with pytest.raises(BadRequest):
             await nvr_obj.remove_custom_doorbell_message(message)
 
         assert not nvr_obj.api.api_request.called
     else:
```

### Comparing `pyunifiprotect-4.8.2/tests/data/test_sensor.py` & `pyunifiprotect-4.8.3/tests/data/test_sensor.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 @pytest.mark.skipif(not TEST_SENSOR_EXISTS, reason="Missing testdata")
 @pytest.mark.parametrize("status", [True, False])
 @pytest.mark.asyncio
 async def test_sensor_set_status_light(sensor_obj: Sensor, status: bool):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.led_settings.is_enabled = not status
-    sensor_obj._initial_data = sensor_obj.dict()
 
     await sensor_obj.set_status_light(status)
 
     sensor_obj.api.api_request.assert_called_with(
         f"sensors/{sensor_obj.id}",
         method="patch",
         json={"ledSettings": {"isEnabled": status}},
@@ -32,15 +31,14 @@
 @pytest.mark.skipif(not TEST_SENSOR_EXISTS, reason="Missing testdata")
 @pytest.mark.parametrize("mount_type", [MountType.DOOR, MountType.NONE])
 @pytest.mark.asyncio
 async def test_sensor_set_mount_type(sensor_obj: Sensor, mount_type: MountType):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.mount_type = MountType.LEAK
-    sensor_obj._initial_data = sensor_obj.dict()
 
     await sensor_obj.set_mount_type(mount_type)
 
     sensor_obj.api.api_request.assert_called_with(
         f"sensors/{sensor_obj.id}",
         method="patch",
         json={"mountType": mount_type.value},
@@ -50,15 +48,14 @@
 @pytest.mark.skipif(not TEST_SENSOR_EXISTS, reason="Missing testdata")
 @pytest.mark.parametrize("status", [True, False])
 @pytest.mark.asyncio
 async def test_sensor_set_motion_status(sensor_obj: Sensor, status: bool):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.motion_settings.is_enabled = not status
-    sensor_obj._initial_data = sensor_obj.dict()
 
     await sensor_obj.set_motion_status(status)
 
     sensor_obj.api.api_request.assert_called_with(
         f"sensors/{sensor_obj.id}",
         method="patch",
         json={"motionSettings": {"isEnabled": status}},
@@ -68,15 +65,14 @@
 @pytest.mark.skipif(not TEST_SENSOR_EXISTS, reason="Missing testdata")
 @pytest.mark.parametrize("status", [True, False])
 @pytest.mark.asyncio
 async def test_sensor_set_temperature_status(sensor_obj: Sensor, status: bool):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.temperature_settings.is_enabled = not status
-    sensor_obj._initial_data = sensor_obj.dict()
 
     await sensor_obj.set_temperature_status(status)
 
     sensor_obj.api.api_request.assert_called_with(
         f"sensors/{sensor_obj.id}",
         method="patch",
         json={"temperatureSettings": {"isEnabled": status}},
@@ -86,15 +82,14 @@
 @pytest.mark.skipif(not TEST_SENSOR_EXISTS, reason="Missing testdata")
 @pytest.mark.parametrize("status", [True, False])
 @pytest.mark.asyncio
 async def test_sensor_set_humidity_status(sensor_obj: Sensor, status: bool):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.humidity_settings.is_enabled = not status
-    sensor_obj._initial_data = sensor_obj.dict()
 
     await sensor_obj.set_humidity_status(status)
 
     sensor_obj.api.api_request.assert_called_with(
         f"sensors/{sensor_obj.id}",
         method="patch",
         json={"humiditySettings": {"isEnabled": status}},
@@ -104,15 +99,14 @@
 @pytest.mark.skipif(not TEST_SENSOR_EXISTS, reason="Missing testdata")
 @pytest.mark.parametrize("status", [True, False])
 @pytest.mark.asyncio
 async def test_sensor_set_light_status(sensor_obj: Sensor, status: bool):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.light_settings.is_enabled = not status
-    sensor_obj._initial_data = sensor_obj.dict()
 
     await sensor_obj.set_light_status(status)
 
     sensor_obj.api.api_request.assert_called_with(
         f"sensors/{sensor_obj.id}",
         method="patch",
         json={"lightSettings": {"isEnabled": status}},
@@ -122,15 +116,14 @@
 @pytest.mark.skipif(not TEST_SENSOR_EXISTS, reason="Missing testdata")
 @pytest.mark.parametrize("status", [True, False])
 @pytest.mark.asyncio
 async def test_sensor_set_alarm_status(sensor_obj: Sensor, status: bool):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.alarm_settings.is_enabled = not status
-    sensor_obj._initial_data = sensor_obj.dict()
 
     await sensor_obj.set_alarm_status(status)
 
     sensor_obj.api.api_request.assert_called_with(
         f"sensors/{sensor_obj.id}",
         method="patch",
         json={"alarmSettings": {"isEnabled": status}},
@@ -143,15 +136,14 @@
 async def test_sensor_set_motion_sensitivity(
     sensor_obj: Sensor,
     sensitivity: int,
 ):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.motion_settings.sensitivity = 50
-    sensor_obj._initial_data = sensor_obj.dict()
 
     if sensitivity == -10:
         with pytest.raises(ValidationError):
             await sensor_obj.set_motion_sensitivity(sensitivity)
 
             assert not sensor_obj.api.api_request.called
     else:
@@ -169,15 +161,14 @@
 @pytest.mark.parametrize("high", [20.0, 45.0, 50.0])
 @pytest.mark.asyncio
 async def test_sensor_set_temperature_safe_range(sensor_obj: Sensor, low: float, high: float):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.temperature_settings.low_threshold = None
     sensor_obj.temperature_settings.high_threshold = None
-    sensor_obj._initial_data = sensor_obj.dict()
 
     if low == -1.0 or high == 50.0 or low > high:
         with pytest.raises(BadRequest):
             await sensor_obj.set_temperature_safe_range(low, high)
 
             assert not sensor_obj.api.api_request.called
     else:
@@ -195,15 +186,14 @@
 @pytest.mark.parametrize("high", [45.0, 99.0, 100.0])
 @pytest.mark.asyncio
 async def test_sensor_set_humidity_safe_range(sensor_obj: Sensor, low: float, high: float):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.humidity_settings.low_threshold = None
     sensor_obj.humidity_settings.high_threshold = None
-    sensor_obj._initial_data = sensor_obj.dict()
 
     if low == 0.0 or high == 100.0 or low > high:
         with pytest.raises(BadRequest):
             await sensor_obj.set_humidity_safe_range(low, high)
 
             assert not sensor_obj.api.api_request.called
     else:
@@ -221,15 +211,14 @@
 @pytest.mark.parametrize("high", [400.0, 1000.0, 1001.0])
 @pytest.mark.asyncio
 async def test_sensor_set_light_safe_range(sensor_obj: Sensor, low: float, high: float):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.light_settings.low_threshold = None
     sensor_obj.light_settings.high_threshold = None
-    sensor_obj._initial_data = sensor_obj.dict()
 
     if low == 0.0 or high == 1001.0 or low > high:
         with pytest.raises(BadRequest):
             await sensor_obj.set_light_safe_range(low, high)
 
             assert not sensor_obj.api.api_request.called
     else:
@@ -245,15 +234,14 @@
 @pytest.mark.skipif(not TEST_SENSOR_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_sensor_remove_temperature_safe_range(sensor_obj: Sensor):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.temperature_settings.low_threshold = 10
     sensor_obj.temperature_settings.high_threshold = 20
-    sensor_obj._initial_data = sensor_obj.dict()
 
     await sensor_obj.remove_temperature_safe_range()
 
     sensor_obj.api.api_request.assert_called_with(
         f"sensors/{sensor_obj.id}",
         method="patch",
         json={"temperatureSettings": {"lowThreshold": None, "highThreshold": None}},
@@ -263,15 +251,14 @@
 @pytest.mark.skipif(not TEST_SENSOR_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_sensor_remove_humidity_safe_range(sensor_obj: Sensor):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.humidity_settings.low_threshold = 10
     sensor_obj.humidity_settings.high_threshold = 20
-    sensor_obj._initial_data = sensor_obj.dict()
 
     await sensor_obj.remove_humidity_safe_range()
 
     sensor_obj.api.api_request.assert_called_with(
         f"sensors/{sensor_obj.id}",
         method="patch",
         json={"humiditySettings": {"lowThreshold": None, "highThreshold": None}},
@@ -281,15 +268,14 @@
 @pytest.mark.skipif(not TEST_SENSOR_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_sensor_remove_light_safe_range(sensor_obj: Sensor):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.light_settings.low_threshold = 10
     sensor_obj.light_settings.high_threshold = 20
-    sensor_obj._initial_data = sensor_obj.dict()
 
     await sensor_obj.remove_light_safe_range()
 
     sensor_obj.api.api_request.assert_called_with(
         f"sensors/{sensor_obj.id}",
         method="patch",
         json={"lightSettings": {"lowThreshold": None, "highThreshold": None}},
@@ -298,15 +284,14 @@
 
 @pytest.mark.skipif(not TEST_SENSOR_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_sensor_set_paired_camera_none(sensor_obj: Sensor):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.camera_id = "bad_id"
-    sensor_obj._initial_data = sensor_obj.dict()
 
     await sensor_obj.set_paired_camera(None)
 
     sensor_obj.api.api_request.assert_called_with(
         f"sensors/{sensor_obj.id}",
         method="patch",
         json={"camera": None},
@@ -315,15 +300,14 @@
 
 @pytest.mark.skipif(not TEST_SENSOR_EXISTS or not TEST_CAMERA_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_sensor_set_paired_camera(sensor_obj: Light, camera_obj: Camera):
     sensor_obj.api.api_request.reset_mock()
 
     sensor_obj.camera_id = None
-    sensor_obj._initial_data = sensor_obj.dict()
 
     await sensor_obj.set_paired_camera(camera_obj)
 
     sensor_obj.api.api_request.assert_called_with(
         f"sensors/{sensor_obj.id}",
         method="patch",
         json={"camera": camera_obj.id},
```

### Comparing `pyunifiprotect-4.8.2/tests/data/test_viewer.py` & `pyunifiprotect-4.8.3/tests/data/test_viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 @pytest.mark.skipif(not TEST_VIEWPORT_EXISTS, reason="Missing testdata")
 @pytest.mark.asyncio
 async def test_viewer_set_liveview_valid(viewer_obj: Viewer, liveview_obj: Liveview):
     viewer_obj.api.api_request.reset_mock()
     viewer_obj.api.emit_message = Mock()
 
     viewer_obj.liveview_id = "bad_id"
-    viewer_obj._initial_data = viewer_obj.dict()
 
     await viewer_obj.set_liveview(liveview_obj)
     viewer_obj.api.api_request.assert_called_with(
         f"viewers/{viewer_obj.id}",
         method="patch",
         json={"liveview": liveview_obj.id},
     )
```

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/constants.py` & `pyunifiprotect-4.8.3/tests/sample_data/constants.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_bootstrap.json` & `pyunifiprotect-4.8.3/tests/sample_data/sample_bootstrap.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_bridge.json` & `pyunifiprotect-4.8.3/tests/sample_data/sample_bridge.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_camera.json` & `pyunifiprotect-4.8.3/tests/sample_data/sample_camera.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_camera_heatmap.png` & `pyunifiprotect-4.8.3/tests/sample_data/sample_camera_heatmap.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_camera_snapshot.png` & `pyunifiprotect-4.8.3/tests/sample_data/sample_camera_snapshot.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_camera_thumbnail.png` & `pyunifiprotect-4.8.3/tests/sample_data/sample_camera_thumbnail.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_camera_video.mp4` & `pyunifiprotect-4.8.3/tests/sample_data/sample_camera_video.mp4`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_chime.json` & `pyunifiprotect-4.8.3/tests/sample_data/sample_chime.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_constants.json` & `pyunifiprotect-4.8.3/tests/sample_data/sample_constants.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_doorlock.json` & `pyunifiprotect-4.8.3/tests/sample_data/sample_doorlock.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_event_smart_track.json` & `pyunifiprotect-4.8.3/tests/sample_data/sample_event_smart_track.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_light.json` & `pyunifiprotect-4.8.3/tests/sample_data/sample_light.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_liveview.json` & `pyunifiprotect-4.8.3/tests/sample_data/sample_liveview.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_raw_events.json` & `pyunifiprotect-4.8.3/tests/sample_data/sample_raw_events.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_sensor.json` & `pyunifiprotect-4.8.3/tests/sample_data/sample_sensor.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_viewport.json` & `pyunifiprotect-4.8.3/tests/sample_data/sample_viewport.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/sample_data/sample_ws_messages.json` & `pyunifiprotect-4.8.3/tests/sample_data/sample_ws_messages.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/test_api.py` & `pyunifiprotect-4.8.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/test_api_polling.py` & `pyunifiprotect-4.8.3/tests/test_api_polling.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/test_api_ws.py` & `pyunifiprotect-4.8.3/tests/test_api_ws.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.2/tests/test_utils.py` & `pyunifiprotect-4.8.3/tests/test_utils.py`

 * *Files identical despite different names*

