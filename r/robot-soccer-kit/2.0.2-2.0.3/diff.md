# Comparing `tmp/robot-soccer-kit-2.0.2.tar.gz` & `tmp/robot-soccer-kit-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot-soccer-kit-2.0.2.tar", last modified: Fri Apr  7 12:46:35 2023, max compression
+gzip compressed data, was "robot-soccer-kit-2.0.3.tar", last modified: Sat Apr 29 10:42:48 2023, max compression
```

## Comparing `robot-soccer-kit-2.0.2.tar` & `robot-soccer-kit-2.0.3.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.935875 robot-soccer-kit-2.0.2/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      262 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/LICENSE
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-04-07 12:46:35.935875 robot-soccer-kit-2.0.2/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      588 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/README.md
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.895876 robot-soccer-kit-2.0.2/robot_soccer_kit.egg-info/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-04-07 12:46:35.000000 robot-soccer-kit-2.0.2/robot_soccer_kit.egg-info/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4847 2023-04-07 12:46:35.000000 robot-soccer-kit-2.0.2/robot_soccer_kit.egg-info/SOURCES.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-04-07 12:46:35.000000 robot-soccer-kit-2.0.2/robot_soccer_kit.egg-info/dependency_links.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       86 2023-04-07 12:46:35.000000 robot-soccer-kit-2.0.2/robot_soccer_kit.egg-info/requires.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        4 2023-04-07 12:46:35.000000 robot-soccer-kit-2.0.2/robot_soccer_kit.egg-info/top_level.txt
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.899875 robot-soccer-kit-2.0.2/rsk/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      102 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/__init__.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/api.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5422 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/backend.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10948 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/client.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      277 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/config.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3225 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/constants.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13513 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/control.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       35 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/debug.sh
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    17821 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/detection.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1058 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/dumb_ia.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/dump_referee.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       73 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/em.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10173 2022-11-27 19:47:15.000000 robot-soccer-kit-2.0.2/rsk/field.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2379 2023-04-07 11:09:06.000000 robot-soccer-kit-2.0.2/rsk/game_controller.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-04-07 11:09:06.000000 robot-soccer-kit-2.0.2/rsk/kinematics.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      445 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/logger.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      602 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/place.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    23541 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/referee.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2362 2023-04-07 11:09:06.000000 robot-soccer-kit-2.0.2/rsk/robot.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11752 2023-04-07 11:09:07.000000 robot-soccer-kit-2.0.2/rsk/robot_serial.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6030 2023-04-07 11:09:06.000000 robot-soccer-kit-2.0.2/rsk/robots.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10231 2023-04-07 11:17:58.000000 robot-soccer-kit-2.0.2/rsk/simulator.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2317 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/state.py
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.903875 robot-soccer-kit-2.0.2/rsk/static/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.895876 robot-soccer-kit-2.0.2/rsk/static/bootstrap/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.911875 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75616 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226018 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56464 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142342 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75690 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226022 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56539 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142419 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11735 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126626 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9817 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    51406 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11728 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126641 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9889 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    63643 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96254 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250681 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74887 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163881 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96121 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250622 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74815 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163716 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267476 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658460 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220780 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   568408 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267055 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658305 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220887 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   567947 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.915875 robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   208288 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.bundle.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   448884 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80599 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   333974 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   136243 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.esm.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   305274 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.esm.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74135 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.esm.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   222070 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.esm.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   145819 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   306458 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    60554 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   217885 2023-04-07 08:27:16.000000 robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      215 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/camera-setting.html
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.919875 robot-soccer-kit-2.0.2/rsk/static/css/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2566 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/css/app.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1150 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/favicon.ico
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.923875 robot-soccer-kit-2.0.2/rsk/static/icons/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.browserslistrc
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      167 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.editorconfig
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       40 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.eslintignore
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      375 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.eslintrc.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      922 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.fantasticonrc.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       43 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.gitattributes
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.923875 robot-soccer-kit-2.0.2/rsk/static/icons/.github/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.923875 robot-soccer-kit-2.0.2/rsk/static/icons/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      583 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.github/ISSUE_TEMPLATE/icon-request.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      433 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.github/dependabot.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   248086 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.github/preview.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      572 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.github/release-drafter.yml
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.923875 robot-soccer-kit-2.0.2/rsk/static/icons/.github/workflows/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      662 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.github/workflows/codeql.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1190 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.github/workflows/deploy.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      243 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.github/workflows/release-notes.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      575 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.github/workflows/test.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       63 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.gitignore
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      125 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/.stylelintrc
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1093 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/LICENSE.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3312 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/README.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   881772 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/bootstrap-icons.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      425 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/composer.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2052 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/config.yml
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.923875 robot-soccer-kit-2.0.2/rsk/static/icons/font/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80510 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/font/bootstrap-icons.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    42897 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/font/bootstrap-icons.json
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.927875 robot-soccer-kit-2.0.2/rsk/static/icons/font/fonts/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   137124 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/font/fonts/bootstrap-icons.woff
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   102536 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/font/fonts/bootstrap-icons.woff2
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   200995 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/font/index.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   643115 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/package-lock.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3152 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/package.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3085 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/svg-sprite.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/icons/svgo.config.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.931875 robot-soccer-kit-2.0.2/rsk/static/imgs/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3287 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/imgs/ball.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1251 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/imgs/ball_16x16.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1856 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/imgs/ball_24x24.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    43069 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/imgs/ball_256x256.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/imgs/ball_32x32.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4470 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/imgs/ball_48x48.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19402 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/imgs/field.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    17815 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/imgs/field.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   249649 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/imgs/robot.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   507520 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/imgs/robotblue1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   524385 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/imgs/robotblue2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   498488 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/imgs/robotgreen1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   522425 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/imgs/robotgreen2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    26782 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/index.html
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.931875 robot-soccer-kit-2.0.2/rsk/static/jquery/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   288580 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/jquery/jquery.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.935875 robot-soccer-kit-2.0.2/rsk/static/js/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1614 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/js/app.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1567 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/js/control.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    24647 2023-04-07 12:46:19.000000 robot-soccer-kit-2.0.2/rsk/static/js/referee.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6005 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/js/robots.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      426 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/js/tabs.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      329 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/js/utils.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6015 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/js/video.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-07 12:46:35.935875 robot-soccer-kit-2.0.2/rsk/static/markers/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6021 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/markers/blue1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6023 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/markers/blue2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6009 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/markers/green1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5098 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/markers/green2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      337 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/referee_event_neutral.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      632 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/referee_event_team.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1029 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/static/robot.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      569 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.2/rsk/static/team.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3865 2022-11-27 19:47:15.000000 robot-soccer-kit-2.0.2/rsk/tasks.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4154 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/utils.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9469 2023-04-07 11:08:46.000000 robot-soccer-kit-2.0.2/rsk/video.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-04-07 12:46:35.935875 robot-soccer-kit-2.0.2/setup.cfg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1395 2023-04-07 12:46:25.000000 robot-soccer-kit-2.0.2/setup.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.028063 robot-soccer-kit-2.0.3/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      262 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/LICENSE
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-04-29 10:42:48.028063 robot-soccer-kit-2.0.3/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      588 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/README.md
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.008063 robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-04-29 10:42:47.000000 robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4847 2023-04-29 10:42:47.000000 robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-04-29 10:42:47.000000 robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       82 2023-04-29 10:42:47.000000 robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/requires.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        4 2023-04-29 10:42:47.000000 robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/top_level.txt
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.008063 robot-soccer-kit-2.0.3/rsk/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      102 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/__init__.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/api.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5422 2023-04-29 10:15:19.000000 robot-soccer-kit-2.0.3/rsk/backend.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10937 2023-04-29 10:28:28.000000 robot-soccer-kit-2.0.3/rsk/client.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      277 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/config.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3225 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/constants.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13513 2023-04-29 10:23:15.000000 robot-soccer-kit-2.0.3/rsk/control.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       35 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/debug.sh
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    18552 2023-04-29 10:39:09.000000 robot-soccer-kit-2.0.3/rsk/detection.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1058 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/dumb_ia.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/dump_referee.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       73 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/em.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10173 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/field.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2379 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/game_controller.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/kinematics.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      445 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/logger.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      602 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/place.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    23541 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/referee.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2362 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/robot.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11752 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/robot_serial.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6030 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/robots.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10231 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/simulator.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2321 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/state.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.008063 robot-soccer-kit-2.0.3/rsk/static/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.008063 robot-soccer-kit-2.0.3/rsk/static/bootstrap/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.016063 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75616 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226018 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56464 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142342 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75690 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226022 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56539 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142419 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11735 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126626 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9817 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    51406 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11728 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126641 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9889 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    63643 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96254 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250681 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163881 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96121 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250622 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163716 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267476 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658460 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220780 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   568408 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267055 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658305 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   567947 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.020063 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   208288 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   448884 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80599 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   333974 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   136243 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   305274 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74135 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   222070 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   145819 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   306458 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    60554 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   217885 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      215 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/camera-setting.html
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.020063 robot-soccer-kit-2.0.3/rsk/static/css/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2566 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/css/app.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1150 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/favicon.ico
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.020063 robot-soccer-kit-2.0.3/rsk/static/icons/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.browserslistrc
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      167 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.editorconfig
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       40 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.eslintignore
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      375 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.eslintrc.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      922 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.fantasticonrc.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       43 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.gitattributes
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.024063 robot-soccer-kit-2.0.3/rsk/static/icons/.github/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.024063 robot-soccer-kit-2.0.3/rsk/static/icons/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      583 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/ISSUE_TEMPLATE/icon-request.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      433 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/dependabot.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   248086 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/preview.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      572 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/release-drafter.yml
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.024063 robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      662 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/codeql.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1190 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/deploy.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      243 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/release-notes.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      575 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/test.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       63 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.gitignore
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      125 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.stylelintrc
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1093 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/LICENSE.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3312 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/README.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   881772 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/bootstrap-icons.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      425 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/composer.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2052 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/config.yml
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.024063 robot-soccer-kit-2.0.3/rsk/static/icons/font/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80510 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/font/bootstrap-icons.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    42897 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/font/bootstrap-icons.json
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.024063 robot-soccer-kit-2.0.3/rsk/static/icons/font/fonts/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   137124 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/font/fonts/bootstrap-icons.woff
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   102536 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/font/fonts/bootstrap-icons.woff2
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   200995 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/font/index.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   643115 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/package-lock.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3152 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/package.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3085 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/svg-sprite.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/svgo.config.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.024063 robot-soccer-kit-2.0.3/rsk/static/imgs/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3287 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/ball.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1251 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/ball_16x16.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1856 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/ball_24x24.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    43069 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/ball_256x256.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/ball_32x32.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4470 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/ball_48x48.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19402 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/field.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    17815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/field.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   249649 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/robot.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   507520 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/robotblue1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   524385 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/robotblue2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   498488 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/robotgreen1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   522425 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/robotgreen2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    26782 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/index.html
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.028063 robot-soccer-kit-2.0.3/rsk/static/jquery/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   288580 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/jquery/jquery.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.028063 robot-soccer-kit-2.0.3/rsk/static/js/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1614 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/js/app.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1567 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/js/control.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    24647 2023-04-29 10:29:12.000000 robot-soccer-kit-2.0.3/rsk/static/js/referee.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6005 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/js/robots.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      426 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/js/tabs.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      329 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/js/utils.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5996 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/js/video.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.028063 robot-soccer-kit-2.0.3/rsk/static/markers/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6021 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/markers/blue1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6023 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/markers/blue2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6009 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/markers/green1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5098 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/markers/green2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      337 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/referee_event_neutral.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      632 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/referee_event_team.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1029 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/robot.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      569 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/team.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3865 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/tasks.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4154 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/utils.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9469 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/video.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-04-29 10:42:48.028063 robot-soccer-kit-2.0.3/setup.cfg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1391 2023-04-29 10:42:22.000000 robot-soccer-kit-2.0.3/setup.py
```

### Comparing `robot-soccer-kit-2.0.2/PKG-INFO` & `robot-soccer-kit-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-soccer-kit
-Version: 2.0.2
+Version: 2.0.3
 Summary: Robot Soccer Kit
 Home-page: https://github.com/rhoban/robot-soccer-kit/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: robot holonomic omniwheel ssl robocup junior soccer standard localized tracking
 Platform: UNKNOWN
```

### Comparing `robot-soccer-kit-2.0.2/README.md` & `robot-soccer-kit-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/robot_soccer_kit.egg-info/PKG-INFO` & `robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-soccer-kit
-Version: 2.0.2
+Version: 2.0.3
 Summary: Robot Soccer Kit
 Home-page: https://github.com/rhoban/robot-soccer-kit/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: robot holonomic omniwheel ssl robocup junior soccer standard localized tracking
 Platform: UNKNOWN
```

### Comparing `robot-soccer-kit-2.0.2/robot_soccer_kit.egg-info/SOURCES.txt` & `robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/api.py` & `robot-soccer-kit-2.0.3/rsk/api.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/backend.py` & `robot-soccer-kit-2.0.3/rsk/backend.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/client.py` & `robot-soccer-kit-2.0.3/rsk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,15 @@
         tracked.last_update = time.time()
 
     def sub_process(self):
         self.sub.RCVTIMEO = 1000
         last_t = time.time()
         while self.running:
             try:
-                json = self.sub.recv_json(zmq.NOBLOCK)
+                json = self.sub.recv_json()
                 ts = time.time()
                 dt = ts - last_t
                 last_t = ts
 
                 if "ball" in json:
                     self.ball = None if json["ball"] is None else np.array(json["ball"])
```

### Comparing `robot-soccer-kit-2.0.2/rsk/constants.py` & `robot-soccer-kit-2.0.3/rsk/constants.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/control.py` & `robot-soccer-kit-2.0.3/rsk/control.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/detection.py` & `robot-soccer-kit-2.0.3/rsk/detection.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,37 +13,37 @@
     def __init__(self):
         # Video attribute
         self.detection = self
         self.capture = None
         self.period = None
 
         self.referee = None
+
         # Publishing server
         self.context = zmq.Context()
         self.socket = self.context.socket(zmq.PUB)
         self.socket.set_hwm(1)
         self.socket.bind("tcp://*:7557")
 
         self.field = Field()
 
 
 class Detection:
     def __init__(self):
         self.state = None
         self.referee = None
 
-        # Publishing server
-        # self.context = zmq.Context()
-        # self.socket = self.context.socket(zmq.PUB)
-        # self.socket.set_hwm(1)
-        # self.socket.bind("tcp://*:7557")
-
         # ArUco parameters
-        self.arucoDict = cv2.aruco.Dictionary_get(cv2.aruco.DICT_4X4_50)
-        self.arucoParams = cv2.aruco.DetectorParameters_create()
+        if self.is_new_aruco_api():
+            dictionary = cv2.aruco.getPredefinedDictionary(cv2.aruco.DICT_4X4_50)
+            parameters = cv2.aruco.DetectorParameters()
+            self.detector = cv2.aruco.ArucoDetector(dictionary, parameters)
+        else:
+            self.arucoDict = cv2.aruco.Dictionary_get(cv2.aruco.DICT_4X4_50)
+            self.arucoParams = cv2.aruco.DetectorParameters_create()
         # arucoParams.cornerRefinementMethod = cv2.aruco.CORNER_REFINE_APRILTAG
 
         # Goals Colors
         self.team_colors = {"green": (0, 255, 0), "blue": (255, 0, 0)}
 
         self.canceled_goal_side = None
 
@@ -93,14 +93,30 @@
         # Detection output
         self.markers = {}
         self.last_updates = {}
         self.ball = None
         self.no_ball = 0
         self.field = Field()
 
+    def is_new_aruco_api(self) -> bool:
+        """
+        Aruco API changed slightly in opencv >= 4.7, see:
+        https://stackoverflow.com/questions/74964527/attributeerror-module-cv2-aruco-has-no-attribute-dictionary-get
+
+        We check OpenCV version and assume
+        """
+        (major, minor, _) = cv2.__version__.split(".")
+
+        if int(major) < 4 or (int(major) == 4 and int(minor) <= 6):
+            # OpenCV <= 4.6
+            return False
+        else:
+            # OpenCV > 4.6
+            return True
+
     def should_display(self, entry: list) -> bool:
         return self.displaySettings[entry]["value"]
 
     def set_display_setting(self, entry: str, value: bool):
         self.displaySettings[entry]["value"] = value
         self.save_display_settings()
 
@@ -301,15 +317,19 @@
                     16,
                 )
 
     def detect_markers(self, image, image_debug=None):
         """
         Detect the fiducial markers on the image, they are passed to the field for calibration
         """
-        (corners, ids, rejected) = cv2.aruco.detectMarkers(image, self.arucoDict, parameters=self.arucoParams)
+        if self.is_new_aruco_api():
+            (corners, ids, rejected) = self.detector.detectMarkers(image)
+        else:
+            (corners, ids, rejected) = cv2.aruco.detectMarkers(image, self.arucoDict, parameters=self.arucoParams)
+
         new_markers = {}
 
         if len(corners) > 0:
             for markerCorner, markerID in zip(corners, ids.flatten()):
                 if markerID not in self.arucoItems:
                     continue
```

### Comparing `robot-soccer-kit-2.0.2/rsk/dumb_ia.py` & `robot-soccer-kit-2.0.3/rsk/dumb_ia.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/dump_referee.py` & `robot-soccer-kit-2.0.3/rsk/dump_referee.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/field.py` & `robot-soccer-kit-2.0.3/rsk/field.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/game_controller.py` & `robot-soccer-kit-2.0.3/rsk/game_controller.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/kinematics.py` & `robot-soccer-kit-2.0.3/rsk/kinematics.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/place.py` & `robot-soccer-kit-2.0.3/rsk/place.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/referee.py` & `robot-soccer-kit-2.0.3/rsk/referee.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/robot.py` & `robot-soccer-kit-2.0.3/rsk/robot.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/robot_serial.py` & `robot-soccer-kit-2.0.3/rsk/robot_serial.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/robots.py` & `robot-soccer-kit-2.0.3/rsk/robots.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/simulator.py` & `robot-soccer-kit-2.0.3/rsk/simulator.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/state.py` & `robot-soccer-kit-2.0.3/rsk/state.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.socket.send_json(info, flags=zmq.NOBLOCK)
 
     def _refresh(function):
         def inner_publish(self, *args, **kwargs):
             function(self, *args, **kwargs)
 
             if self.context is not None:
-                if self.last_time is None or time.time() - self.last_time > 1 / self.frequency_pub:
+                if self.last_time is None or (time.time() - self.last_time) > (1 / self.frequency_pub):
                     self.last_time = time.time()
                     self.publish()
 
         return inner_publish
 
     @_refresh
     def set_markers(self, markers):
```

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.min.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.min.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.rtl.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.min.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.min.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.min.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.min.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.rtl.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.rtl.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.rtl.min.css` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.bundle.js` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.bundle.js.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.bundle.min.js` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.esm.js` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.esm.js.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.esm.min.js` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.esm.min.js.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.js` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.js.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.min.js` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/bootstrap/js/bootstrap.min.js.map` & `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/css/app.css` & `robot-soccer-kit-2.0.3/rsk/static/css/app.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/favicon.ico` & `robot-soccer-kit-2.0.3/rsk/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/.fantasticonrc.js` & `robot-soccer-kit-2.0.3/rsk/static/icons/.fantasticonrc.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md` & `robot-soccer-kit-2.0.3/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/.github/preview.png` & `robot-soccer-kit-2.0.3/rsk/static/icons/.github/preview.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/.github/release-drafter.yml` & `robot-soccer-kit-2.0.3/rsk/static/icons/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/.github/workflows/codeql.yml` & `robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/.github/workflows/deploy.yml` & `robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/.github/workflows/test.yml` & `robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/LICENSE.md` & `robot-soccer-kit-2.0.3/rsk/static/icons/LICENSE.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/README.md` & `robot-soccer-kit-2.0.3/rsk/static/icons/README.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/bootstrap-icons.svg` & `robot-soccer-kit-2.0.3/rsk/static/icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/config.yml` & `robot-soccer-kit-2.0.3/rsk/static/icons/config.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/font/bootstrap-icons.css` & `robot-soccer-kit-2.0.3/rsk/static/icons/font/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/font/bootstrap-icons.json` & `robot-soccer-kit-2.0.3/rsk/static/icons/font/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/font/fonts/bootstrap-icons.woff` & `robot-soccer-kit-2.0.3/rsk/static/icons/font/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/font/fonts/bootstrap-icons.woff2` & `robot-soccer-kit-2.0.3/rsk/static/icons/font/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/font/index.html` & `robot-soccer-kit-2.0.3/rsk/static/icons/font/index.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/package-lock.json` & `robot-soccer-kit-2.0.3/rsk/static/icons/package-lock.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/package.json` & `robot-soccer-kit-2.0.3/rsk/static/icons/package.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/svg-sprite.json` & `robot-soccer-kit-2.0.3/rsk/static/icons/svg-sprite.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/icons/svgo.config.js` & `robot-soccer-kit-2.0.3/rsk/static/icons/svgo.config.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/imgs/ball.png` & `robot-soccer-kit-2.0.3/rsk/static/imgs/ball.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/imgs/ball_16x16.png` & `robot-soccer-kit-2.0.3/rsk/static/imgs/ball_16x16.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/imgs/ball_24x24.png` & `robot-soccer-kit-2.0.3/rsk/static/imgs/ball_24x24.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/imgs/ball_256x256.png` & `robot-soccer-kit-2.0.3/rsk/static/imgs/ball_256x256.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/imgs/ball_32x32.png` & `robot-soccer-kit-2.0.3/rsk/static/imgs/ball_32x32.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/imgs/ball_48x48.png` & `robot-soccer-kit-2.0.3/rsk/static/imgs/ball_48x48.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/imgs/field.png` & `robot-soccer-kit-2.0.3/rsk/static/imgs/field.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/imgs/field.svg` & `robot-soccer-kit-2.0.3/rsk/static/imgs/field.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/imgs/robot.svg` & `robot-soccer-kit-2.0.3/rsk/static/imgs/robot.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/imgs/robotblue1.svg` & `robot-soccer-kit-2.0.3/rsk/static/imgs/robotblue1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/imgs/robotblue2.svg` & `robot-soccer-kit-2.0.3/rsk/static/imgs/robotblue2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/imgs/robotgreen1.svg` & `robot-soccer-kit-2.0.3/rsk/static/imgs/robotgreen1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/imgs/robotgreen2.svg` & `robot-soccer-kit-2.0.3/rsk/static/imgs/robotgreen2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/index.html` & `robot-soccer-kit-2.0.3/rsk/static/index.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/jquery/jquery.js` & `robot-soccer-kit-2.0.3/rsk/static/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/js/app.js` & `robot-soccer-kit-2.0.3/rsk/static/js/app.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/js/control.js` & `robot-soccer-kit-2.0.3/rsk/static/js/control.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/js/referee.js` & `robot-soccer-kit-2.0.3/rsk/static/js/referee.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/js/robots.js` & `robot-soccer-kit-2.0.3/rsk/static/js/robots.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/js/video.js` & `robot-soccer-kit-2.0.3/rsk/static/js/video.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -102,15 +102,15 @@
     // Retrieving the images
     setInterval(function() {
 
         is_vision = current_tab == 'vision' || 'referee';
         backend.enableVideoDebug(is_vision);
 
         backend.get_video(is_vision, function(video) {
-            if (video.image && !simulated_view) {
+            if (video.image) {
                 $('.camera-image').attr('src', 'data:image/jpeg;base64,' + video.image);
             }
 
             if (video.running) {
                 $('body').addClass('vision-running');
             } else {
                 $('body').removeClass('vision-running');
```

### Comparing `robot-soccer-kit-2.0.2/rsk/static/markers/blue1.svg` & `robot-soccer-kit-2.0.3/rsk/static/markers/blue1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/markers/blue2.svg` & `robot-soccer-kit-2.0.3/rsk/static/markers/blue2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/markers/green1.svg` & `robot-soccer-kit-2.0.3/rsk/static/markers/green1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/markers/green2.svg` & `robot-soccer-kit-2.0.3/rsk/static/markers/green2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/referee_event_team.html` & `robot-soccer-kit-2.0.3/rsk/static/referee_event_team.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/robot.html` & `robot-soccer-kit-2.0.3/rsk/static/robot.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/static/team.html` & `robot-soccer-kit-2.0.3/rsk/static/team.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/tasks.py` & `robot-soccer-kit-2.0.3/rsk/tasks.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/utils.py` & `robot-soccer-kit-2.0.3/rsk/utils.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/rsk/video.py` & `robot-soccer-kit-2.0.3/rsk/video.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.2/setup.py` & `robot-soccer-kit-2.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         for filename in filenames:
             if '__pycache__' not in path:
                 paths.append(os.path.join('..', path, filename))
     return paths
 
 setuptools.setup(
     name="robot-soccer-kit",
-    version="2.0.2",
+    version="2.0.3",
     author="Rhoban team",
     author_email="team@rhoban.com",
     description="Robot Soccer Kit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rhoban/robot-soccer-kit/",
     packages=setuptools.find_packages(),
@@ -35,14 +35,14 @@
     ],
     extras_require={
         'gc': [ # Game controller extra requirements
             "pyserial",
             "flask",
             "flask-cors",
             "waitress",
-            "opencv-contrib-python<4.7"
+            "opencv-contrib-python"
         ]
     },
     include_package_data=True,
     package_data={"": package_files("rsk")},
     python_requires='>=3.6',
 )
```

