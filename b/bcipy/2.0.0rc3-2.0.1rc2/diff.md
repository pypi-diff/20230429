# Comparing `tmp/bcipy-2.0.0rc3.tar.gz` & `tmp/bcipy-2.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcipy-2.0.0rc3.tar", last modified: Fri Apr 28 23:57:05 2023, max compression
+gzip compressed data, was "bcipy-2.0.1rc2.tar", last modified: Fri Oct 14 22:23:29 2022, max compression
```

## Comparing `bcipy-2.0.0rc3.tar` & `bcipy-2.0.1rc2.tar`

### file list

```diff
@@ -1,195 +1,183 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.708856 bcipy-2.0.0rc3/
--rw-rw-rw-   0        0        0     8419 2022-07-22 17:37:41.000000 bcipy-2.0.0rc3/LICENSE.md
--rw-rw-rw-   0        0        0      815 2023-04-28 23:57:05.708856 bcipy-2.0.0rc3/PKG-INFO
--rw-rw-rw-   0        0        0    11813 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.503052 bcipy-2.0.0rc3/bcipy/
--rw-rw-rw-   0        0        0        0 2022-07-22 17:37:41.000000 bcipy-2.0.0rc3/bcipy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.541096 bcipy-2.0.0rc3/bcipy/acquisition/
--rw-rw-rw-   0        0        0      418 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/acquisition/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.549098 bcipy-2.0.0rc3/bcipy/acquisition/datastream/
--rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/acquisition/datastream/__init__.py
--rw-rw-rw-   0        0        0     3510 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/acquisition/datastream/generator.py
--rw-rw-rw-   0        0        0     8335 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/acquisition/datastream/lsl_server.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.554098 bcipy-2.0.0rc3/bcipy/acquisition/datastream/mock/
--rw-rw-rw-   0        0        0       88 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/acquisition/datastream/mock/__init__.py
--rw-rw-rw-   0        0        0     2268 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/acquisition/datastream/mock/eye_tracker_server.py
--rw-rw-rw-   0        0        0     2650 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/acquisition/datastream/mock/switch.py
--rw-rw-rw-   0        0        0     3520 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/acquisition/datastream/producer.py
--rw-rw-rw-   0        0        0     8515 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/acquisition/devices.py
--rw-rw-rw-   0        0        0      106 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/acquisition/exceptions.py
--rw-rw-rw-   0        0        0     2674 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/acquisition/marker_writer.py
--rw-rw-rw-   0        0        0     2912 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/acquisition/multimodal.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.556097 bcipy-2.0.0rc3/bcipy/acquisition/protocols/
--rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/acquisition/protocols/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.560099 bcipy-2.0.0rc3/bcipy/acquisition/protocols/lsl/
--rw-rw-rw-   0        0        0        0 2022-09-26 17:58:56.000000 bcipy-2.0.0rc3/bcipy/acquisition/protocols/lsl/__init__.py
--rw-rw-rw-   0        0        0    12264 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/acquisition/protocols/lsl/lsl_client.py
--rw-rw-rw-   0        0        0     3138 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/acquisition/protocols/lsl/lsl_connector.py
--rw-rw-rw-   0        0        0     8760 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/acquisition/protocols/lsl/lsl_recorder.py
--rw-rw-rw-   0        0        0      344 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/acquisition/record.py
--rw-rw-rw-   0        0        0     3092 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/acquisition/util.py
--rw-rw-rw-   0        0        0     1681 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/config.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.562100 bcipy-2.0.0rc3/bcipy/display/
--rw-rw-rw-   0        0        0      621 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/display/__init__.py
--rw-rw-rw-   0        0        0    11119 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/display/main.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.564100 bcipy-2.0.0rc3/bcipy/display/paradigm/
--rw-rw-rw-   0        0        0        0 2022-09-26 21:47:42.000000 bcipy-2.0.0rc3/bcipy/display/paradigm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.566098 bcipy-2.0.0rc3/bcipy/display/paradigm/matrix/
--rw-rw-rw-   0        0        0       85 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/display/paradigm/matrix/__init__.py
--rw-rw-rw-   0        0        0    13364 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/display/paradigm/matrix/display.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.568570 bcipy-2.0.0rc3/bcipy/display/paradigm/rsvp/
--rw-rw-rw-   0        0        0       81 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/display/paradigm/rsvp/__init__.py
--rw-rw-rw-   0        0        0    18083 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/display/paradigm/rsvp/display.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.572577 bcipy-2.0.0rc3/bcipy/display/paradigm/rsvp/mode/
--rw-rw-rw-   0        0        0        0 2022-09-26 21:47:57.000000 bcipy-2.0.0rc3/bcipy/display/paradigm/rsvp/mode/__init__.py
--rw-rw-rw-   0        0        0      976 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/display/paradigm/rsvp/mode/calibration.py
--rw-rw-rw-   0        0        0     3331 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/display/paradigm/rsvp/mode/copy_phrase.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.573578 bcipy-2.0.0rc3/bcipy/display/paradigm/vep/
--rw-rw-rw-   0        0        0        0 2022-10-03 21:54:59.000000 bcipy-2.0.0rc3/bcipy/display/paradigm/vep/__init__.py
--rw-rw-rw-   0        0        0    19046 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/display/paradigm/vep/display.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.575578 bcipy-2.0.0rc3/bcipy/feedback/
--rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/feedback/__init__.py
--rw-rw-rw-   0        0        0      555 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/feedback/feedback.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.578579 bcipy-2.0.0rc3/bcipy/feedback/sound/
--rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/feedback/sound/__init__.py
--rw-rw-rw-   0        0        0      989 2023-03-25 00:09:57.000000 bcipy-2.0.0rc3/bcipy/feedback/sound/auditory_feedback.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.582578 bcipy-2.0.0rc3/bcipy/feedback/visual/
--rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/feedback/visual/__init__.py
--rw-rw-rw-   0        0        0     4934 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/feedback/visual/level_feedback.py
--rw-rw-rw-   0        0        0     2861 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/feedback/visual/visual_feedback.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.588592 bcipy-2.0.0rc3/bcipy/gui/
--rw-rw-rw-   0        0        0    16780 2022-10-03 21:56:01.000000 bcipy-2.0.0rc3/bcipy/gui/BCInterface.py
--rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/gui/__init__.py
--rw-rw-rw-   0        0        0      811 2022-10-03 21:49:48.000000 bcipy-2.0.0rc3/bcipy/gui/alert.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.593619 bcipy-2.0.0rc3/bcipy/gui/experiments/
--rw-rw-rw-   0        0        0    10650 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/gui/experiments/ExperimentField.py
--rw-rw-rw-   0        0        0    16717 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/gui/experiments/ExperimentRegistry.py
--rw-rw-rw-   0        0        0     9569 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/gui/experiments/FieldRegistry.py
--rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/gui/experiments/__init__.py
--rw-rw-rw-   0        0        0     3418 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/gui/file_dialog.py
--rw-rw-rw-   0        0        0    32852 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/gui/main.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.596728 bcipy-2.0.0rc3/bcipy/gui/viewer/
--rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/gui/viewer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.601010 bcipy-2.0.0rc3/bcipy/gui/viewer/data_source/
--rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/gui/viewer/data_source/__init__.py
--rw-rw-rw-   0        0        0     1593 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/gui/viewer/data_source/data_source.py
--rw-rw-rw-   0        0        0     1294 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/gui/viewer/data_source/file_streamer.py
--rw-rw-rw-   0        0        0     2768 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/gui/viewer/data_source/lsl_data_source.py
--rw-rw-rw-   0        0        0    27424 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/gui/viewer/data_viewer.py
--rw-rw-rw-   0        0        0     1741 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/gui/viewer/ring_buffer.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.623274 bcipy-2.0.0rc3/bcipy/helpers/
--rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/helpers/__init__.py
--rw-rw-rw-   0        0        0    10180 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/acquisition.py
--rw-rw-rw-   0        0        0     1760 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/helpers/clock.py
--rw-rw-rw-   0        0        0    24026 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/convert.py
--rw-rw-rw-   0        0        0    13530 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/copy_phrase_wrapper.py
--rw-rw-rw-   0        0        0     2373 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/exceptions.py
--rw-rw-rw-   0        0        0     4696 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/language_model.py
--rw-rw-rw-   0        0        0     1297 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/helpers/list.py
--rw-rw-rw-   0        0        0     9624 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/load.py
--rw-rw-rw-   0        0        0    10253 2023-03-24 18:50:45.000000 bcipy-2.0.0rc3/bcipy/helpers/parameters.py
--rw-rw-rw-   0        0        0    14118 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/raw_data.py
--rw-rw-rw-   0        0        0     5441 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/save.py
--rw-rw-rw-   0        0        0    11524 2022-10-03 21:52:15.000000 bcipy-2.0.0rc3/bcipy/helpers/session.py
--rw-rw-rw-   0        0        0    32111 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/stimuli.py
--rw-rw-rw-   0        0        0     1161 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/symbols.py
--rw-rw-rw-   0        0        0     9876 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/system_utils.py
--rw-rw-rw-   0        0        0    11841 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/task.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.647855 bcipy-2.0.0rc3/bcipy/helpers/tests/
--rw-rw-rw-   0        0        0       77 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/__init__.py
--rw-rw-rw-   0        0        0     7013 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_acquisition.py
--rw-rw-rw-   0        0        0     1624 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_clock.py
--rw-rw-rw-   0        0        0    27612 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_convert.py
--rw-rw-rw-   0        0        0     8185 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_copy_phrase_wrapper.py
--rw-rw-rw-   0        0        0     9156 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_language_model.py
--rw-rw-rw-   0        0        0     2222 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_list.py
--rw-rw-rw-   0        0        0     7600 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_load.py
--rw-rw-rw-   0        0        0    20012 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_parameters.py
--rw-rw-rw-   0        0        0    15291 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_raw_data.py
--rw-rw-rw-   0        0        0     2887 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_save.py
--rw-rw-rw-   0        0        0     1742 2022-10-03 21:51:01.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_session.py
--rw-rw-rw-   0        0        0    34583 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_stimuli.py
--rw-rw-rw-   0        0        0      959 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_symbols.py
--rw-rw-rw-   0        0        0     3518 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_system_utils.py
--rw-rw-rw-   0        0        0    13974 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_task.py
--rw-rw-rw-   0        0        0    13540 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_triggers.py
--rw-rw-rw-   0        0        0     5670 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_validate.py
--rw-rw-rw-   0        0        0     5527 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/tests/test_visualization.py
--rw-rw-rw-   0        0        0    13462 2023-04-27 04:17:52.000000 bcipy-2.0.0rc3/bcipy/helpers/triggers.py
--rw-rw-rw-   0        0        0     4897 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/validate.py
--rw-rw-rw-   0        0        0     9263 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/helpers/visualization.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.650856 bcipy-2.0.0rc3/bcipy/language/
--rw-rw-rw-   0        0        0      108 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/language/__init__.py
--rw-rw-rw-   0        0        0     2820 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/language/main.py
--rw-rw-rw-   0        0        0     9516 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/main.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.651857 bcipy-2.0.0rc3/bcipy/parameters/
--rw-rw-rw-   0        0        0        0 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/parameters/__init__.py
--rw-rw-rw-   0        0        0     2851 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/preferences.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.652855 bcipy-2.0.0rc3/bcipy/signal/
--rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/signal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.654858 bcipy-2.0.0rc3/bcipy/signal/evaluate/
--rw-rw-rw-   0        0        0       90 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/signal/evaluate/__init__.py
--rw-rw-rw-   0        0        0     1365 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/signal/evaluate/evaluator.py
--rw-rw-rw-   0        0        0     2397 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/signal/evaluate/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.656855 bcipy-2.0.0rc3/bcipy/signal/generator/
--rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/signal/generator/__init__.py
--rw-rw-rw-   0        0        0      279 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/signal/generator/generator.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.667856 bcipy-2.0.0rc3/bcipy/signal/model/
--rw-rw-rw-   0        0        0      320 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/model/__init__.py
--rw-rw-rw-   0        0        0     1683 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/signal/model/base_model.py
--rw-rw-rw-   0        0        0     7095 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/model/classifier.py
--rw-rw-rw-   0        0        0     5837 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/model/cross_validation.py
--rw-rw-rw-   0        0        0     2984 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/model/density_estimation.py
--rw-rw-rw-   0        0        0     3655 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/model/dimensionality_reduction.py
--rw-rw-rw-   0        0        0     4552 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/signal/model/inquiry_preview.py
--rw-rw-rw-   0        0        0    10208 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/model/offline_analysis.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.669855 bcipy-2.0.0rc3/bcipy/signal/model/pca_rda_kde/
--rw-rw-rw-   0        0        0       82 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/signal/model/pca_rda_kde/__init__.py
--rw-rw-rw-   0        0        0     7772 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/model/pca_rda_kde/pca_rda_kde.py
--rw-rw-rw-   0        0        0     2381 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/model/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.670854 bcipy-2.0.0rc3/bcipy/signal/model/rda_kde/
--rw-rw-rw-   0        0        0        0 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/model/rda_kde/__init__.py
--rw-rw-rw-   0        0        0     7502 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/model/rda_kde/rda_kde.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.673855 bcipy-2.0.0rc3/bcipy/signal/process/
--rw-rw-rw-   0        0        0      251 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/signal/process/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.676854 bcipy-2.0.0rc3/bcipy/signal/process/decomposition/
--rw-rw-rw-   0        0        0      241 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/process/decomposition/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/process/decomposition/cwt.py
--rw-rw-rw-   0        0        0     3495 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/process/decomposition/psd.py
--rw-rw-rw-   0        0        0     1812 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/signal/process/filter.py
--rw-rw-rw-   0        0        0     1322 2022-07-22 17:37:42.000000 bcipy-2.0.0rc3/bcipy/signal/process/transform.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.686857 bcipy-2.0.0rc3/bcipy/task/
--rw-rw-rw-   0        0        0      186 2022-07-22 17:37:43.000000 bcipy-2.0.0rc3/bcipy/task/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.691858 bcipy-2.0.0rc3/bcipy/task/control/
--rw-rw-rw-   0        0        0        0 2022-09-26 21:52:17.000000 bcipy-2.0.0rc3/bcipy/task/control/__init__.py
--rw-rw-rw-   0        0        0     8149 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/task/control/criteria.py
--rw-rw-rw-   0        0        0    11068 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/task/control/handler.py
--rw-rw-rw-   0        0        0     2989 2022-07-22 17:37:43.000000 bcipy-2.0.0rc3/bcipy/task/control/query.py
--rw-rw-rw-   0        0        0    12442 2022-10-03 21:31:16.000000 bcipy-2.0.0rc3/bcipy/task/data.py
--rw-rw-rw-   0        0        0      521 2022-07-22 17:37:43.000000 bcipy-2.0.0rc3/bcipy/task/exceptions.py
--rw-rw-rw-   0        0        0      409 2022-07-22 17:37:43.000000 bcipy-2.0.0rc3/bcipy/task/main.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.693857 bcipy-2.0.0rc3/bcipy/task/paradigm/
--rw-rw-rw-   0        0        0        0 2022-09-26 21:52:24.000000 bcipy-2.0.0rc3/bcipy/task/paradigm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.699857 bcipy-2.0.0rc3/bcipy/task/paradigm/matrix/
--rw-rw-rw-   0        0        0        0 2022-09-26 21:52:26.000000 bcipy-2.0.0rc3/bcipy/task/paradigm/matrix/__init__.py
--rw-rw-rw-   0        0        0    11026 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/task/paradigm/matrix/calibration.py
--rw-rw-rw-   0        0        0     3550 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/task/paradigm/matrix/copy_phrase.py
--rw-rw-rw-   0        0        0     2647 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/task/paradigm/matrix/timing_verification.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.702857 bcipy-2.0.0rc3/bcipy/task/paradigm/rsvp/
--rw-rw-rw-   0        0        0        0 2022-09-26 21:52:34.000000 bcipy-2.0.0rc3/bcipy/task/paradigm/rsvp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.707859 bcipy-2.0.0rc3/bcipy/task/paradigm/rsvp/calibration/
--rw-rw-rw-   0        0        0        0 2022-09-26 21:52:59.000000 bcipy-2.0.0rc3/bcipy/task/paradigm/rsvp/calibration/__init__.py
--rw-rw-rw-   0        0        0    11597 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/task/paradigm/rsvp/calibration/calibration.py
--rw-rw-rw-   0        0        0     2683 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/task/paradigm/rsvp/calibration/timing_verification.py
--rw-rw-rw-   0        0        0    36251 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/task/paradigm/rsvp/copy_phrase.py
--rw-rw-rw-   0        0        0     2766 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/task/start_task.py
--rw-rw-rw-   0        0        0     2527 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/bcipy/task/task_registry.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:57:05.531097 bcipy-2.0.0rc3/bcipy.egg-info/
--rw-rw-rw-   0        0        0      815 2023-04-28 23:57:05.000000 bcipy-2.0.0rc3/bcipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5222 2023-04-28 23:57:05.000000 bcipy-2.0.0rc3/bcipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 23:57:05.000000 bcipy-2.0.0rc3/bcipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-28 23:57:05.000000 bcipy-2.0.0rc3/bcipy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      432 2023-04-28 23:57:05.000000 bcipy-2.0.0rc3/bcipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-28 23:57:05.000000 bcipy-2.0.0rc3/bcipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      205 2023-04-28 23:57:05.718856 bcipy-2.0.0rc3/setup.cfg
--rw-rw-rw-   0        0        0     3434 2023-04-28 23:54:53.000000 bcipy-2.0.0rc3/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.232950 bcipy-2.0.1rc2/
+-rw-rw-rw-   0        0        0     8419 2022-07-22 17:37:41.000000 bcipy-2.0.1rc2/LICENSE.md
+-rw-rw-rw-   0        0        0      814 2022-10-14 22:23:29.232950 bcipy-2.0.1rc2/PKG-INFO
+-rw-rw-rw-   0        0        0    10971 2022-10-03 21:49:31.000000 bcipy-2.0.1rc2/README.md
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.048746 bcipy-2.0.1rc2/bcipy/
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:41.000000 bcipy-2.0.1rc2/bcipy/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.076125 bcipy-2.0.1rc2/bcipy/acquisition/
+-rw-rw-rw-   0        0        0      245 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/acquisition/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.080124 bcipy-2.0.1rc2/bcipy/acquisition/datastream/
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/acquisition/datastream/__init__.py
+-rw-rw-rw-   0        0        0     3510 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/acquisition/datastream/generator.py
+-rw-rw-rw-   0        0        0     8308 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/acquisition/datastream/lsl_server.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.083419 bcipy-2.0.1rc2/bcipy/acquisition/datastream/mock/
+-rw-rw-rw-   0        0        0       88 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/acquisition/datastream/mock/__init__.py
+-rw-rw-rw-   0        0        0     2268 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/acquisition/datastream/mock/eye_tracker_server.py
+-rw-rw-rw-   0        0        0     2650 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/acquisition/datastream/mock/switch.py
+-rw-rw-rw-   0        0        0     3520 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/acquisition/datastream/producer.py
+-rw-rw-rw-   0        0        0     7170 2022-10-03 21:53:09.000000 bcipy-2.0.1rc2/bcipy/acquisition/devices.py
+-rw-rw-rw-   0        0        0      106 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/acquisition/exceptions.py
+-rw-rw-rw-   0        0        0     2674 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/acquisition/marker_writer.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.084422 bcipy-2.0.1rc2/bcipy/acquisition/protocols/
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/acquisition/protocols/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.089675 bcipy-2.0.1rc2/bcipy/acquisition/protocols/lsl/
+-rw-rw-rw-   0        0        0        0 2022-09-26 17:58:56.000000 bcipy-2.0.1rc2/bcipy/acquisition/protocols/lsl/__init__.py
+-rw-rw-rw-   0        0        0    11340 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/acquisition/protocols/lsl/lsl_client.py
+-rw-rw-rw-   0        0        0     3138 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/acquisition/protocols/lsl/lsl_connector.py
+-rw-rw-rw-   0        0        0     8760 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/acquisition/protocols/lsl/lsl_recorder.py
+-rw-rw-rw-   0        0        0      344 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/acquisition/record.py
+-rw-rw-rw-   0        0        0     3092 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/acquisition/util.py
+-rw-rw-rw-   0        0        0     1451 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/config.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.092032 bcipy-2.0.1rc2/bcipy/display/
+-rw-rw-rw-   0        0        0      680 2022-10-03 21:54:57.000000 bcipy-2.0.1rc2/bcipy/display/__init__.py
+-rw-rw-rw-   0        0        0    12544 2022-10-03 21:54:58.000000 bcipy-2.0.1rc2/bcipy/display/main.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.093032 bcipy-2.0.1rc2/bcipy/display/paradigm/
+-rw-rw-rw-   0        0        0        0 2022-09-26 21:47:42.000000 bcipy-2.0.1rc2/bcipy/display/paradigm/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.096029 bcipy-2.0.1rc2/bcipy/display/paradigm/matrix/
+-rw-rw-rw-   0        0        0       85 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/display/paradigm/matrix/__init__.py
+-rw-rw-rw-   0        0        0    12971 2022-10-03 21:56:01.000000 bcipy-2.0.1rc2/bcipy/display/paradigm/matrix/display.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.098494 bcipy-2.0.1rc2/bcipy/display/paradigm/matrix/mode/
+-rw-rw-rw-   0        0        0        0 2022-09-26 21:47:51.000000 bcipy-2.0.1rc2/bcipy/display/paradigm/matrix/mode/__init__.py
+-rw-rw-rw-   0        0        0      892 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/display/paradigm/matrix/mode/calibration.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.101006 bcipy-2.0.1rc2/bcipy/display/paradigm/rsvp/
+-rw-rw-rw-   0        0        0       81 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/display/paradigm/rsvp/__init__.py
+-rw-rw-rw-   0        0        0    18008 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/display/paradigm/rsvp/display.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.105008 bcipy-2.0.1rc2/bcipy/display/paradigm/rsvp/mode/
+-rw-rw-rw-   0        0        0        0 2022-09-26 21:47:57.000000 bcipy-2.0.1rc2/bcipy/display/paradigm/rsvp/mode/__init__.py
+-rw-rw-rw-   0        0        0      816 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/display/paradigm/rsvp/mode/calibration.py
+-rw-rw-rw-   0        0        0     4271 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/display/paradigm/rsvp/mode/copy_phrase.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.107629 bcipy-2.0.1rc2/bcipy/display/paradigm/vep/
+-rw-rw-rw-   0        0        0        0 2022-10-03 21:54:59.000000 bcipy-2.0.1rc2/bcipy/display/paradigm/vep/__init__.py
+-rw-rw-rw-   0        0        0    18549 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/display/paradigm/vep/display.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.109647 bcipy-2.0.1rc2/bcipy/feedback/
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/feedback/__init__.py
+-rw-rw-rw-   0        0        0      555 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/feedback/feedback.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.111644 bcipy-2.0.1rc2/bcipy/feedback/sound/
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/feedback/sound/__init__.py
+-rw-rw-rw-   0        0        0      989 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/feedback/sound/auditory_feedback.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.114914 bcipy-2.0.1rc2/bcipy/feedback/visual/
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/feedback/visual/__init__.py
+-rw-rw-rw-   0        0        0     4934 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/feedback/visual/level_feedback.py
+-rw-rw-rw-   0        0        0     2861 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/feedback/visual/visual_feedback.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.119914 bcipy-2.0.1rc2/bcipy/gui/
+-rw-rw-rw-   0        0        0    16780 2022-10-03 21:56:01.000000 bcipy-2.0.1rc2/bcipy/gui/BCInterface.py
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/gui/__init__.py
+-rw-rw-rw-   0        0        0      811 2022-10-03 21:49:48.000000 bcipy-2.0.1rc2/bcipy/gui/alert.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.124929 bcipy-2.0.1rc2/bcipy/gui/experiments/
+-rw-rw-rw-   0        0        0    10650 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/gui/experiments/ExperimentField.py
+-rw-rw-rw-   0        0        0    16717 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/gui/experiments/ExperimentRegistry.py
+-rw-rw-rw-   0        0        0     9569 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/gui/experiments/FieldRegistry.py
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/gui/experiments/__init__.py
+-rw-rw-rw-   0        0        0     2739 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/gui/file_dialog.py
+-rw-rw-rw-   0        0        0    31611 2022-10-03 21:53:53.000000 bcipy-2.0.1rc2/bcipy/gui/main.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.128119 bcipy-2.0.1rc2/bcipy/gui/viewer/
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/gui/viewer/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.133125 bcipy-2.0.1rc2/bcipy/gui/viewer/data_source/
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/gui/viewer/data_source/__init__.py
+-rw-rw-rw-   0        0        0     1593 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/gui/viewer/data_source/data_source.py
+-rw-rw-rw-   0        0        0     1294 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/gui/viewer/data_source/file_streamer.py
+-rw-rw-rw-   0        0        0     2768 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/gui/viewer/data_source/lsl_data_source.py
+-rw-rw-rw-   0        0        0    27424 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/gui/viewer/data_viewer.py
+-rw-rw-rw-   0        0        0     1741 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/gui/viewer/ring_buffer.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.156361 bcipy-2.0.1rc2/bcipy/helpers/
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/helpers/__init__.py
+-rw-rw-rw-   0        0        0     6147 2022-10-03 21:50:08.000000 bcipy-2.0.1rc2/bcipy/helpers/acquisition.py
+-rw-rw-rw-   0        0        0     1760 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/helpers/clock.py
+-rw-rw-rw-   0        0        0    20184 2022-10-13 23:09:21.000000 bcipy-2.0.1rc2/bcipy/helpers/convert.py
+-rw-rw-rw-   0        0        0    13292 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/helpers/copy_phrase_wrapper.py
+-rw-rw-rw-   0        0        0     1739 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/helpers/exceptions.py
+-rw-rw-rw-   0        0        0     4352 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/helpers/language_model.py
+-rw-rw-rw-   0        0        0     1297 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/helpers/list.py
+-rw-rw-rw-   0        0        0     9071 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/helpers/load.py
+-rw-rw-rw-   0        0        0    10253 2022-10-14 22:21:25.000000 bcipy-2.0.1rc2/bcipy/helpers/parameters.py
+-rw-rw-rw-   0        0        0    13494 2022-10-03 21:51:34.000000 bcipy-2.0.1rc2/bcipy/helpers/raw_data.py
+-rw-rw-rw-   0        0        0     5091 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/helpers/save.py
+-rw-rw-rw-   0        0        0    11524 2022-10-03 21:52:15.000000 bcipy-2.0.1rc2/bcipy/helpers/session.py
+-rw-rw-rw-   0        0        0    30448 2022-10-13 23:09:21.000000 bcipy-2.0.1rc2/bcipy/helpers/stimuli.py
+-rw-rw-rw-   0        0        0     8851 2022-10-03 21:56:01.000000 bcipy-2.0.1rc2/bcipy/helpers/system_utils.py
+-rw-rw-rw-   0        0        0    12896 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/helpers/task.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.179240 bcipy-2.0.1rc2/bcipy/helpers/tests/
+-rw-rw-rw-   0        0        0       77 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/__init__.py
+-rw-rw-rw-   0        0        0     2721 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_acquisition.py
+-rw-rw-rw-   0        0        0     1624 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_clock.py
+-rw-rw-rw-   0        0        0    19932 2022-10-03 21:51:41.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_convert.py
+-rw-rw-rw-   0        0        0     8342 2022-10-03 21:53:30.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_copy_phrase_wrapper.py
+-rw-rw-rw-   0        0        0     9156 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_language_model.py
+-rw-rw-rw-   0        0        0     2222 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_list.py
+-rw-rw-rw-   0        0        0     7600 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_load.py
+-rw-rw-rw-   0        0        0    20012 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_parameters.py
+-rw-rw-rw-   0        0        0    14606 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_raw_data.py
+-rw-rw-rw-   0        0        0     2887 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_save.py
+-rw-rw-rw-   0        0        0     1742 2022-10-03 21:51:01.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_session.py
+-rw-rw-rw-   0        0        0    31270 2022-10-03 21:53:34.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_stimuli.py
+-rw-rw-rw-   0        0        0    14529 2022-10-03 21:53:22.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_task.py
+-rw-rw-rw-   0        0        0    13540 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_triggers.py
+-rw-rw-rw-   0        0        0     5670 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/helpers/tests/test_validate.py
+-rw-rw-rw-   0        0        0    13462 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/helpers/triggers.py
+-rw-rw-rw-   0        0        0     4642 2022-10-03 21:54:47.000000 bcipy-2.0.1rc2/bcipy/helpers/validate.py
+-rw-rw-rw-   0        0        0     6062 2022-10-03 21:51:46.000000 bcipy-2.0.1rc2/bcipy/helpers/visualization.py
+-rw-rw-rw-   0        0        0     8019 2022-10-03 21:53:03.000000 bcipy-2.0.1rc2/bcipy/main.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.181480 bcipy-2.0.1rc2/bcipy/signal/
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.185513 bcipy-2.0.1rc2/bcipy/signal/evaluate/
+-rw-rw-rw-   0        0        0       90 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/evaluate/__init__.py
+-rw-rw-rw-   0        0        0     1365 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/evaluate/evaluator.py
+-rw-rw-rw-   0        0        0     2397 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/evaluate/rules.py
+-rw-rw-rw-   0        0        0      244 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.187497 bcipy-2.0.1rc2/bcipy/signal/generator/
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/generator/__init__.py
+-rw-rw-rw-   0        0        0      279 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/generator/generator.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.192925 bcipy-2.0.1rc2/bcipy/signal/model/
+-rw-rw-rw-   0        0        0      192 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/model/__init__.py
+-rw-rw-rw-   0        0        0     1683 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/model/base_model.py
+-rw-rw-rw-   0        0        0     4552 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/model/inquiry_preview.py
+-rw-rw-rw-   0        0        0     8779 2022-10-03 21:53:58.000000 bcipy-2.0.1rc2/bcipy/signal/model/offline_analysis.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.202003 bcipy-2.0.1rc2/bcipy/signal/model/pca_rda_kde/
+-rw-rw-rw-   0        0        0       82 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/model/pca_rda_kde/__init__.py
+-rw-rw-rw-   0        0        0     7095 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/model/pca_rda_kde/classifier.py
+-rw-rw-rw-   0        0        0     5935 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/model/pca_rda_kde/cross_validation.py
+-rw-rw-rw-   0        0        0     2984 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/model/pca_rda_kde/density_estimation.py
+-rw-rw-rw-   0        0        0     2542 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/model/pca_rda_kde/dimensionality_reduction.py
+-rw-rw-rw-   0        0        0     7592 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/model/pca_rda_kde/pca_rda_kde.py
+-rw-rw-rw-   0        0        0     2381 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/model/pca_rda_kde/pipeline.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.206210 bcipy-2.0.1rc2/bcipy/signal/process/
+-rw-rw-rw-   0        0        0      251 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/signal/process/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.208223 bcipy-2.0.1rc2/bcipy/signal/process/decomposition/
+-rw-rw-rw-   0        0        0        0 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/process/decomposition/__init__.py
+-rw-rw-rw-   0        0        0     3532 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/process/decomposition/psd.py
+-rw-rw-rw-   0        0        0     1804 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/process/filter.py
+-rw-rw-rw-   0        0        0     1322 2022-07-22 17:37:42.000000 bcipy-2.0.1rc2/bcipy/signal/process/transform.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.215509 bcipy-2.0.1rc2/bcipy/task/
+-rw-rw-rw-   0        0        0      186 2022-07-22 17:37:43.000000 bcipy-2.0.1rc2/bcipy/task/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.220706 bcipy-2.0.1rc2/bcipy/task/control/
+-rw-rw-rw-   0        0        0        0 2022-09-26 21:52:17.000000 bcipy-2.0.1rc2/bcipy/task/control/__init__.py
+-rw-rw-rw-   0        0        0     8149 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/task/control/criteria.py
+-rw-rw-rw-   0        0        0    10792 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/task/control/handler.py
+-rw-rw-rw-   0        0        0     2989 2022-07-22 17:37:43.000000 bcipy-2.0.1rc2/bcipy/task/control/query.py
+-rw-rw-rw-   0        0        0    12442 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/task/data.py
+-rw-rw-rw-   0        0        0      521 2022-07-22 17:37:43.000000 bcipy-2.0.1rc2/bcipy/task/exceptions.py
+-rw-rw-rw-   0        0        0      409 2022-07-22 17:37:43.000000 bcipy-2.0.1rc2/bcipy/task/main.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.221710 bcipy-2.0.1rc2/bcipy/task/paradigm/
+-rw-rw-rw-   0        0        0        0 2022-09-26 21:52:24.000000 bcipy-2.0.1rc2/bcipy/task/paradigm/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.224949 bcipy-2.0.1rc2/bcipy/task/paradigm/matrix/
+-rw-rw-rw-   0        0        0        0 2022-09-26 21:52:26.000000 bcipy-2.0.1rc2/bcipy/task/paradigm/matrix/__init__.py
+-rw-rw-rw-   0        0        0    10897 2022-10-03 21:49:31.000000 bcipy-2.0.1rc2/bcipy/task/paradigm/matrix/calibration.py
+-rw-rw-rw-   0        0        0     2855 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/task/paradigm/matrix/timing_verification.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.227951 bcipy-2.0.1rc2/bcipy/task/paradigm/rsvp/
+-rw-rw-rw-   0        0        0        0 2022-09-26 21:52:34.000000 bcipy-2.0.1rc2/bcipy/task/paradigm/rsvp/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.231947 bcipy-2.0.1rc2/bcipy/task/paradigm/rsvp/calibration/
+-rw-rw-rw-   0        0        0        0 2022-09-26 21:52:59.000000 bcipy-2.0.1rc2/bcipy/task/paradigm/rsvp/calibration/__init__.py
+-rw-rw-rw-   0        0        0    10723 2022-10-03 21:31:16.000000 bcipy-2.0.1rc2/bcipy/task/paradigm/rsvp/calibration/calibration.py
+-rw-rw-rw-   0        0        0     2540 2022-09-06 16:14:12.000000 bcipy-2.0.1rc2/bcipy/task/paradigm/rsvp/calibration/timing_verification.py
+-rw-rw-rw-   0        0        0    37268 2022-10-03 21:53:41.000000 bcipy-2.0.1rc2/bcipy/task/paradigm/rsvp/copy_phrase.py
+-rw-rw-rw-   0        0        0     2435 2022-09-06 16:14:12.000000 bcipy-2.0.1rc2/bcipy/task/start_task.py
+-rw-rw-rw-   0        0        0     2412 2022-09-06 16:14:12.000000 bcipy-2.0.1rc2/bcipy/task/task_registry.py
+drwxrwxrwx   0        0        0        0 2022-10-14 22:23:29.069130 bcipy-2.0.1rc2/bcipy.egg-info/
+-rw-rw-rw-   0        0        0      814 2022-10-14 22:23:28.000000 bcipy-2.0.1rc2/bcipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4969 2022-10-14 22:23:28.000000 bcipy-2.0.1rc2/bcipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-14 22:23:28.000000 bcipy-2.0.1rc2/bcipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2022-10-14 22:23:28.000000 bcipy-2.0.1rc2/bcipy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      341 2022-10-14 22:23:28.000000 bcipy-2.0.1rc2/bcipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2022-10-14 22:23:28.000000 bcipy-2.0.1rc2/bcipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      205 2022-10-14 22:23:29.234948 bcipy-2.0.1rc2/setup.cfg
+-rw-rw-rw-   0        0        0     3203 2022-10-14 22:21:25.000000 bcipy-2.0.1rc2/setup.py
```

### Comparing `bcipy-2.0.0rc3/LICENSE.md` & `bcipy-2.0.1rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/PKG-INFO` & `bcipy-2.0.1rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bcipy
-Version: 2.0.0rc3
+Version: 2.0.1rc2
 Summary: Python Software for Brain-Computer Interface.
 Home-page: https://github.com/CAMBI-tech/BciPy
 Author: CAMBI
 Author-email: cambi_support@googlegroups.com
 License: Hippocratic License 2.1
 Description: Python Brain-Computer Interface Software
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >3.7,<3.10
+Requires-Python: >3.6,<3.9
 Description-Content-Type: text/markdown
```

### Comparing `bcipy-2.0.0rc3/README.md` & `bcipy-2.0.1rc2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,244 +1,233 @@
-# BciPy: Brain-Computer Interface Software in Python
-
-
-[![BciPy](https://github.com/CAMBI-tech/BciPy/actions/workflows/main.yml/badge.svg)](https://github.com/CAMBI-tech/BciPy/actions/workflows/main.yml)
-[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](https://github.com/CAMBI-tech/BciPy/fork)
-[![Follow on Twitter](https://img.shields.io/twitter/follow/cambi_tech?label=Follow&style=social)](https://twitter.com/cambi_tech)
-
-
-BciPy is a library for conducting Brain-Computer Interface experiments in Python. It functions as a standalone application for experimental data collection or you can take the tools you need and start coding your own system. See our official BciPy documentation including affiliations and more context information [here](https://bcipy.github.io/) (in progress).
-
-It will run on the latest windows (7, 10, 11), linux (ubuntu 22.04) and macos (Big Sur). Other versions may work as well, but are not guaranteed. To see supported versions and operating systems as of this release see here: [BciPy Builds](https://github.com/CAMBI-tech/BciPy/actions/workflows/main.yml).
-
-*Please cite us when using!*
-
-```
-Memmott, T., Koçanaoğulları, A., Lawhead, M., Klee, D., Dudy, S., Fried-Oken, M., & Oken, B. (2021). BciPy: brain–computer interface software in Python. Brain-Computer Interfaces, 1-18.
-```
-
-## Dependencies
----------------
-This project requires Python 3.8 or 3.9. Please see notes below for additional OS specific dependencies before installation can be completed.
-
-### Linux
-
-You will need to install the prerequisites defined in `scripts\shell\linux_requirements.sh` as well as `pip install attrdict3`.
-
-### Windows
-
-If you are using a Windows machine, you will need to install the [Microsoft Visual C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/).
-
-*python 3.9 only!*
-You will need to install pyWinhook manually. See [here](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pywinhook) for the appropriate wheel file (`pyWinhook‑1.6.2‑cp39‑cp39‑win_amd64.whl`). Then run `pip install <path_to_wheel_file>`. We also include the 64-bit wheel file in the `.bcipy/downloads/` directory.
-
-### Mac
-
-If you are using a Mac, you will need to install XCode and enable command line tools. `xcode-select --install`. 
-
-## Installation
----------------
-
-#### BciPy Setup
-
-In order to run BciPy on your computer, after following the dependencies above, you will need to install the BciPy package.
-
-To install for use locally,
-1. Git clone https://github.com/BciPy/BciPy.git
-2. Change directory in your terminal to the repo
-3. Run `pip install -e .`
-4. To use the KenLMLanguageModel class, you must manually install the kenlm package. `pip install kenlm==0.1 --global-option="--max_order=12"`.
-
-
-If wanting the latest version from PyPi:
-1. `pip install bcipy`
-
-Alternately, if [Make](http://www.mingw.org/) is installed, you may run the follow command to install:
-
-```sh
-# install in development mode
-make dev-install
-```
-
-#### Usage Locally
-
-Two ways to get started using BciPy for data collection:
-	1. Run `python bcipy/gui/BCInterface.py` in your command prompt or terminal from from base BciPy directory. This will execute the main BCI GUI. You may also use the command `make bci-gui`. 
-	2. Invoke the experiment directly using command line utility `bcipy`.
-		- You can pass it attributes with flags, if desired.
-				Ex. `bcipy --user "bci_user" --task "RSVP Calibration"`
-		- Use the help flag to see other available input options: `bcipy --help`
-
-##### Example usage as a package
-
-```python
-from bcipy.helpers import system_utils
-system_utils.get_system_info()
-```
-
-## Glossary
------------
-
-***Stimuli***: A single letter, tone or image shown (generally in an inquiry). Singular = stimulus, plural = stimuli.
-
-***Trial***: A collection of data after a stimuli is shown. A----
-
-***Inquiry***: The set of stimuli after a fixation cross in a spelling task to gather user intent. A ---- B --- C ----
-
-***Series***: Each series contains at least one inquiry. A letter/icon decision is made after a series in a spelling task.
-
-***Session***: Data collected for a task. Comprised of metadata about the task and a list of Series.
-
-***Task***: An experimental design with stimuli, trials, inquiries and series for use in BCI. For instance, "RSVP Calibration" is a task.
-
-***Mode***: Common design elements between task types. For instance, Calibration and Free Spelling are modes.
-
-***Paradigm***: Display paradigm with unique properties and modes. Ex. Rapid-Serial Visual Presentation (RSVP), Matrix Speller, Steady-State Visual Evoked Potential (SSVEP).
-
-
-## Core Modules
----------------
-
-This a list of the major modules and their functionality. Each module will contain its own README, demo and tests. Please check them out for more information!
-
-- `acquisition`: acquires data, gives back desired time series, saves to file at end of session.
-- `display`: handles display of stimuli on screen and passes back stimuli timing.
-- `signal`: eeg signal models, filters, processing, evaluators and viewers.
-- `gui`: end-user interface into registered bci tasks and parameter editing. See BCInterface.py.
-- `helpers`: helpful functions needed for interactions between modules, basic I/O, and data visualization.
-- `language`: gives probabilities of next symbols during typing.
-- `parameters`: location of json parameters. This includes parameters.json (main experiment / app configuration) and device.json (device registry and configuration).
-- `static`: image and sound stimuli, misc manuals, and readable texts for gui.
-- `task`: bcipy implemented user tasks. Main collection of bci modules for use during various experimentation. Ex. RSVP Calibration.
-- `feedback`: feedback mechanisms for sound and visual stimuli.
-- `main`: executor of experiments. Main entry point into the application
-- `config`: configuration parameters for the application, including paths and data filenames.
-
-
-## Paradigms
-------------
-
-
-> RSVPKeyboard
-
-
-```
-*RSVP KeyboardTM* is an EEG (electroencephalography) based BCI (brain computer interface) typing system. It utilizes a visual presentation technique called rapid serial visual presentation (RSVP). In RSVP, the options are presented rapidly at a single location with a temporal separation. Similarly in RSVP KeyboardTM, the symbols (the letters and additional symbols) are shown at the center of screen. When the subject wants to select a symbol, they await the intended symbol during the presentation and elicit a p300 response to a target symbol.
-```
-
-Citation: 
-```
-Orhan, U., Hild, K. E., 2nd, Erdogmus, D., Roark, B., Oken, B., & Fried-Oken, M. (2012). RSVP Keyboard: An EEG Based Typing Interface. Proceedings of the ... IEEE International Conference on Acoustics, Speech, and Signal Processing. ICASSP (Conference), 10.1109/ICASSP.2012.6287966. https://doi.org/10.1109/ICASSP.2012.6287966
-```
-
-> Matrix Speller
-
-```
-Matrix Speller is an EEG (electroencephalography) based BCI (brain computer interface) typing system. It utilizes a visual presentation technique called Single Character Presentation (SCP). In matrix speller, the symbols are arranged in a matrix with fixed number of rows and columns. Using SCP, subsets of these symbols are intensified (i.e. highlighted) usually in pseudorandom order to produce an odd ball paradigm to induce p300 responses. 
-```
-
-Citation:
-```
-Farwell, L. A., & Donchin, E. (1988). Talking off the top of your head: toward a mental prosthesis utilizing event-related brain potentials. Electroencephalography and clinical Neurophysiology, 70(6), 510-523.
-
-Ahani A, Moghadamfalahi M, Erdogmus D. Language-Model Assisted And Icon-based Communication Through a Brain Computer Interface With Different Presentation Paradigms. IEEE Trans Neural Syst Rehabil Eng. 2018 Jul 25. doi: 10.1109/TNSRE.2018.2859432.
-```
-
-## Demo
---------
-
-All major functions and modules have demo and test files associated with them which may be run locally. This should help orient you to the functionality as well as serve as documentation. *If you add to the repo, you should be adding tests and fixing any test that fail when you change the code.*
-
-For example, you may run the main BciPy demo by:
-
-`python demo/bci_main_demo.py`
-
-This demo will load in parameters and execute a demo task defined in the file. There are demo files for all modules listed above except helpers and utils. Run them as a python script!
-
-
-## Testing
-----------
-
-When writing tests, put them in the correct module, in a tests folder, and prefix the file and test itself with `test_` in order for pytest to discover it. See other module tests for examples!
-
-Development requirements must be installed before running: `pip install -r dev_requirements.txt`
-
-To run all tests, in the command line:
-
-```python
-py.test
-```
-
-
-To run a single modules tests (ex. acquisition), in the command line:
-
-```python
-py.test acquisition
-```
-
-To generate test coverage metrics, in the command line:
-
-```bash
-coverage run --branch --source=bcipy -m pytest --mpl -k "not slow"
-
-#Generate a command line report
-coverage report
-
-# Generate html doc in the bci folder. Navigate to index.html and click.
-coverage html
-```
-
-Alternately, if Make is installed, you may run the follow command to run coverage/pytest and generate the html:
-
-```sh
-make coverage-html
-```
-
-## Linting
-----------
-
-This project enforces `PEP` style guidelines using [flake8](http://flake8.pycqa.org/en/latest/).
-
-To avoid spending unnecessary time on formatting, we recommend using `autopep8`. You can specify a file or directory to auto format. When ready to push your code, you may run the following commands to format your code:
-
-```sh
-# autoformat all files in bcipy
-autopep8 --in-place --aggressive -r bcipy
-
-# autoformat only the processor file
-autopep8 --in-place --aggressive bcipy/acquisition/processor.py
-```
-
-Finally, run the lint check: `flake8 bcipy`.
-
-Alternately, if Make is installed, you may run the follow command to run autopep8 and flake8:
-
-```sh
-make lint
-```
-
-### Contributions Welcome!
-
-If you want to be added to the development team slack or have additional questions, please reach out to us at support@cambi.tech!
-
-### Contribution Guidelines
-
-We follow and will enforce the contributor's covenant to foster a safe and inclusive environment for this open source software, please reference this link for more information: https://www.contributor-covenant.org/
-
-Other guidelines:
-- All features require tests and a demo.
-- All tests must pass to merge, even if they are seemingly unrelated to your work.
-- Use Spaces, not Tabs.
-- Use informative names for functions and classes.
-- Document the input and output of your functions / classes in the code. eg in-line commenting and typing.
-- Do not push IDE or other local configuration files.
-- All new modules or major functionality should be documented outside of the code with a README.md.
-	See README.md in repo or go to this site for inspiration: https://github.com/matiassingers/awesome-readme. Always use a Markdown interpreter before pushing. There are many free online or your IDE may come with one.
-
-See this resource for examples: http://docs.python-guide.org/en/latest/writing/style/
-
-## Contributors
----------------
-
-All contributions are greatly appreciated!
-
-[![image of contributors generated by https://contributors-img.web.app/ pulling from https://github.com/CAMBI-tech/BciPy/graphs/contributors](https://contrib.rocks/image?repo=CAMBI-tech/BciPy)](https://github.com/CAMBI-tech/BciPy/graphs/contributors)
+# BciPy: Brain-Computer Interface Software in Python
+
+
+[![BciPy](https://github.com/CAMBI-tech/BciPy/actions/workflows/main.yml/badge.svg)](https://github.com/CAMBI-tech/BciPy/actions/workflows/main.yml)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](https://github.com/CAMBI-tech/BciPy/fork)
+[![Follow on Twitter](https://img.shields.io/twitter/follow/cambi_tech?label=Follow&style=social)](https://twitter.com/cambi_tech)
+
+
+BciPy is a library for conducting Brain-Computer Interface experiments in Python. It functions as a standalone application for experimental data collection or you can take the tools you need and start coding your own system. See our official BciPy documentation including affiliations and more context information [here](https://bcipy.github.io/) (in progress).
+
+It will run on the latest windows (7, 10, 11), linux (ubuntu 22.04) and macos (Big Sur). Other versions may work as well, but are not guaranteed. To see supported versions and operating systems as of this release see here: [BciPy Builds](https://github.com/CAMBI-tech/BciPy/actions/workflows/main.yml).
+
+*Please cite us when using!*
+
+```
+Memmott, T., Koçanaoğulları, A., Lawhead, M., Klee, D., Dudy, S., Fried-Oken, M., & Oken, B. (2021). BciPy: brain–computer interface software in Python. Brain-Computer Interfaces, 1-18.
+```
+
+## Dependencies
+---------------
+This project requires Python 3.7 or 3.8. All other dependencies defined in the requirements.txt.
+
+
+## Installation
+---------------
+
+#### BciPy Setup
+
+In order to run BciPy on your computer, first install **Python 3** [from here.](https://www.python.org/downloads/)
+
+To use all the goodies locally (including the GUI and demo scripts)
+1. Git clone https://github.com/BciPy/BciPy.git
+2. Change directory in your terminal to the repo
+3. Run `pip install -e .`
+4. If using Mac, you will need to install XCode and enable command line tools. `xcode-select --install`
+5. If you're on Windows, you may need to uninstall pygame (`pip uninstall pygame`). Psychopy, for historical reasons, keeps pygame but it just spams your console logs if you only want to use pyglet (which we use in this repository!)
+
+If wanting the latest version from PyPi:
+1. `pip install bcipy`
+
+Alternately, if [Make](http://www.mingw.org/) is installed, you may run the follow command to install:
+
+```sh
+# install in development mode
+make dev-install
+```
+
+#### Usage Locally
+
+Start by running `python bcipy/gui/BCInterface.py` in your command prompt or terminal. This will run the GUI. You may also use the command `make bci-gui`. You may also invoke the experiment directly using command line tools from bcipy.
+
+Ex. `bcipy` *this will use default parameters, user, experiment and task*
+
+You can pass it attributes with flags, if desired.
+
+Ex. `bcipy --user "bci_user" --task "RSVP Calibration"`
+
+Use the help flag to see other available input options: `bcipy --help`
+
+##### Example usage as a package
+
+```python
+from bcipy.helpers import system_utils
+system_utils.get_system_info()
+```
+
+## Glossary
+-----------
+
+***Stimuli***: A single letter, tone or image shown (generally in an inquiry). Singular = stimulus, plural = stimuli.
+
+***Trial***: A collection of data after a stimuli is shown. A----
+
+***Inquiry***: The set of stimuli after a fixation cross in a spelling task to gather user intent. A ---- B --- C ----
+
+***Series***: Each series contains at least one inquiry. A letter/icon decision is made after a series in a spelling task.
+
+***Session***: Data collected for a task. Comprised of metadata about the task and a list of Series.
+
+***Task***: An experimental design with stimuli, trials, inquiries and series for use in BCI. For instance, "RSVP Calibration" is a task.
+
+***Mode***: Common design elements between task types. For instance, Calibration and Free Spelling are modes.
+
+***Paradigm***: Display paradigm with unique properties and modes. Ex. Rapid-Serial Visual Presentation (RSVP), Matrix Speller, Steady-State Visual Evoked Potential (SSVEP).
+
+
+## Core Modules
+---------------
+
+This a list of the major modules and their functionality. Each module will contain its own README, demo and tests. Please check them out for more information!
+
+- `acquisition`: acquires data, gives back desired time series, saves to file at end of session.
+- `display`: handles display of stimuli on screen and passes back stimuli timing.
+- `signal`: eeg signal models, filters, processing, evaluators and viewers.
+- `gui`: end-user interface into registered bci tasks and parameter editing. See BCInterface.py.
+- `helpers`: helpful functions needed for interactions between modules, basic I/O, and data visualization.
+- `language`: gives probabilities of next symbols during typing.
+- `parameters`: location of json parameters. This includes parameters.json (main experiment / app configuration) and device.json (device registry and configuration).
+- `static`: image and sound stimuli, misc manuals, and readable texts for gui.
+- `task`: bcipy implemented user tasks. Main collection of bci modules for use during various experimentation. Ex. RSVP Calibration.
+- `feedback`: feedback mechanisms for sound and visual stimuli.
+- `main`: executor of experiments. Main entry point into the application
+- `config`: configuration parameters for the application, including paths and data filenames.
+
+
+## Paradigms
+------------
+
+
+> RSVPKeyboard
+
+
+```
+*RSVP KeyboardTM* is an EEG (electroencephalography) based BCI (brain computer interface) typing system. It utilizes a visual presentation technique called rapid serial visual presentation (RSVP). In RSVP, the options are presented rapidly at a single location with a temporal separation. Similarly in RSVP KeyboardTM, the symbols (the letters and additional symbols) are shown at the center of screen. When the subject wants to select a symbol, they await the intended symbol during the presentation and elicit a p300 response to a target symbol.
+```
+
+Citation: 
+```
+Orhan, U., Hild, K. E., 2nd, Erdogmus, D., Roark, B., Oken, B., & Fried-Oken, M. (2012). RSVP Keyboard: An EEG Based Typing Interface. Proceedings of the ... IEEE International Conference on Acoustics, Speech, and Signal Processing. ICASSP (Conference), 10.1109/ICASSP.2012.6287966. https://doi.org/10.1109/ICASSP.2012.6287966
+```
+
+> Matrix Speller
+
+```
+Matrix Speller is an EEG (electroencephalography) based BCI (brain computer interface) typing system. It utilizes a visual presentation technique called Single Character Presentation (SCP). In matrix speller, the symbols are arranged in a matrix with fixed number of rows and columns. Using SCP, subsets of these symbols are intensified (i.e. highlighted) usually in pseudorandom order to produce an odd ball paradigm to induce p300 responses. 
+```
+
+Citation:
+```
+Farwell, L. A., & Donchin, E. (1988). Talking off the top of your head: toward a mental prosthesis utilizing event-related brain potentials. Electroencephalography and clinical Neurophysiology, 70(6), 510-523.
+
+Ahani A, Moghadamfalahi M, Erdogmus D. Language-Model Assisted And Icon-based Communication Through a Brain Computer Interface With Different Presentation Paradigms. IEEE Trans Neural Syst Rehabil Eng. 2018 Jul 25. doi: 10.1109/TNSRE.2018.2859432.
+```
+
+## Demo
+--------
+
+All major functions and modules have demo and test files associated with them which may be run locally. This should help orient you to the functionality as well as serve as documentation. *If you add to the repo, you should be adding tests and fixing any test that fail when you change the code.*
+
+For example, you may run the main BciPy demo by:
+
+`python demo/bci_main_demo.py`
+
+This demo will load in parameters and execute a demo task defined in the file. There are demo files for all modules listed above except language_model, helpers, and utils. Run them as a python script!
+
+
+## Testing
+----------
+
+When writing tests, put them in the correct module, in a tests folder, and prefix the file and test itself with `test_` in order for pytest to discover it. See other module tests for examples!
+
+Development requirements must be installed before running: `pip install dev_requirements.txt`
+
+To run all tests, in the command line:
+
+```python
+py.test
+```
+
+
+To run a single modules tests (ex. acquisition), in the command line:
+
+```python
+py.test acquisition
+```
+
+To generate test coverage metrics, in the command line:
+
+```bash
+coverage run --branch --source=bcipy -m pytest --mpl -k "not slow"
+
+#Generate a command line report
+coverage report
+
+# Generate html doc in the bci folder. Navigate to index.html and click.
+coverage html
+```
+
+Alternately, if Make is installed, you may run the follow command to run coverage/pytest and generate the html:
+
+```sh
+make coverage-html
+```
+
+## Linting
+----------
+
+This project enforces `PEP` style guidelines using [flake8](http://flake8.pycqa.org/en/latest/).
+
+To avoid spending unnecessary time on formatting, we recommend using `autopep8`. You can specify a file or directory to auto format. When ready to push your code, you may run the following commands to format your code:
+
+```sh
+# autoformat all files in bcipy
+autopep8 --in-place --aggressive -r bcipy
+
+# autoformat only the processor file
+autopep8 --in-place --aggressive bcipy/acquisition/processor.py
+```
+
+Finally, run the lint check: `flake8 bcipy`.
+
+Alternately, if Make is installed, you may run the follow command to run autopep8 and flake8:
+
+```sh
+make lint
+```
+
+### Contributions Welcome!
+
+If you want to be added to the development team slack or have additional questions, please reach out to us at support@cambi.tech!
+
+### Contribution Guidelines
+
+We follow and will enforce the contributor's covenant to foster a safe and inclusive environment for this open source software, please reference this link for more information: https://www.contributor-covenant.org/
+
+Other guidelines:
+- All features require tests and a demo.
+- All tests must pass to merge, even if they are seemingly unrelated to your work.
+- Use Spaces, not Tabs.
+- Use informative names for functions and classes.
+- Document the input and output of your functions / classes in the code. eg in-line commenting and typing.
+- Do not push IDE or other local configuration files.
+- All new modules or major functionality should be documented outside of the code with a README.md.
+	See README.md in repo or go to this site for inspiration: https://github.com/matiassingers/awesome-readme. Always use a Markdown interpreter before pushing. There are many free online or your IDE may come with one.
+
+See this resource for examples: http://docs.python-guide.org/en/latest/writing/style/
+
+## Contributors
+---------------
+
+All contributions are greatly appreciated!
+
+[![image of contributors generated by https://contributors-img.web.app/ pulling from https://github.com/CAMBI-tech/BciPy/graphs/contributors](https://contrib.rocks/image?repo=CAMBI-tech/BciPy)](https://github.com/CAMBI-tech/BciPy/graphs/contributors)
```

### Comparing `bcipy-2.0.0rc3/bcipy/acquisition/datastream/generator.py` & `bcipy-2.0.1rc2/bcipy/acquisition/datastream/generator.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/acquisition/datastream/lsl_server.py` & `bcipy-2.0.1rc2/bcipy/acquisition/datastream/lsl_server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,209 +1,213 @@
-"""Data server that streams EEG data over a LabStreamingLayer StreamOutlet
-using pylsl."""
-import logging
-from queue import Empty, Queue
-from typing import Generator
-import time
-import uuid
-
-from pylsl import StreamInfo, StreamOutlet
-
-from bcipy.config import DEFAULT_ENCODING
-from bcipy.acquisition.datastream.generator import random_data_generator
-from bcipy.acquisition.datastream.producer import Producer
-from bcipy.acquisition.devices import DeviceSpec
-from bcipy.acquisition.util import StoppableThread
-
-log = logging.getLogger(__name__)
-
-# pylint: disable=too-many-arguments
-
-MARKER_STREAM_NAME = 'TRG_device_stream'
-
-
-class LslDataServer(StoppableThread):
-    """Data server that streams EEG data over a LabStreamingLayer StreamOutlet
-    using pylsl. See https://github.com/sccn/labstreaminglayer/wiki.
-
-    In parameters.json, if the fake_data parameter is set to true and the
-    device is set to DSI-24, this server will be used to mock data. Alternatively,
-    fake_data can be set to false and this module can be run standalone in its
-    own python instance.
-
-    Parameters
-    ----------
-        device_spec : DeviceSpec
-            parameters used to configure the server. Should have at least
-            a list of channels and the sample frequency.
-        generator : optional Generator (see generator.py for options)
-            used to generate the data to be served. Uses random_data_generator
-            by default.
-        include_meta: bool, optional
-            if True, writes metadata to the outlet stream.
-        add_markers: bool, optional
-            if True, creates a the marker channel and streams data to this
-            channel at a fixed frequency.
-        marker_stream_name: str, optional
-            name of the sample marker stream
-    """
-
-    def __init__(self, device_spec: DeviceSpec, generator: Generator = None, include_meta: bool = True,
-                 add_markers: bool = False, marker_stream_name: str = MARKER_STREAM_NAME):
-        super(LslDataServer, self).__init__()
-
-        self.device_spec = device_spec
-        self.generator = generator or random_data_generator(channel_count=device_spec.channel_count)
-
-        log.debug("Starting LSL server for device: %s", device_spec.name)
-        print(f"Serving: {device_spec}")
-        info = StreamInfo(device_spec.name,
-                          device_spec.content_type, device_spec.channel_count,
-                          device_spec.sample_rate,
-                          device_spec.data_type,
-                          f'{device_spec.content_type.lower()}_{uuid.uuid1()}')
-
-        if include_meta:
-            meta_channels = info.desc().append_child('channels')
-            for channel in device_spec.channel_specs:
-                channel_node = meta_channels.append_child('channel')
-                channel_node.append_child_value('label', channel.name)
-                if channel.units:
-                    channel_node.append_child_value('unit', channel.units)
-                if channel.type:
-                    channel_node.append_child_value('type', channel.type)
-
-        self.outlet = StreamOutlet(info)
-
-        self.add_markers = add_markers
-        if add_markers:
-            # Marker stream (C++ source below):
-            # lsl::stream_info marker_info("gUSBamp-"+deviceNumber+"Markers",
-            # "Markers",1,0,lsl::cf_string,
-            # "gUSBamp_" + boost::lexical_cast<std::string>(deviceNumber) +
-            # "_" + boost::lexical_cast<std::string>(serialNumber) +
-            # "_markers");
-            log.debug("Creating marker stream")
-            print(f"Marker channel name: {marker_stream_name}")
-            markers_info = StreamInfo(marker_stream_name,
-                                      "Markers", 1, 0, 'string',
-                                      "uid12345_markers")
-            self.markers_outlet = StreamOutlet(markers_info)
-        self.started = False
-
-    def stop(self):
-        """Stop the thread and cleanup resources."""
-
-        log.debug("[*] Stopping data server")
-        super(LslDataServer, self).stop()
-
-        # Allows pylsl to cleanup; The outlet will no longer be discoverable
-        # after destruction and all connected inlets will stop delivering data.
-        del self.outlet
-        self.outlet = None
-
-        if self.add_markers:
-            del self.markers_outlet
-            self.markers_outlet = None
-
-    def run(self):
-        """Main loop of the thread. Continuously streams data to the stream
-        outlet at a rate consistent with the sample frequency. May also
-        output markers at a different interval."""
-
-        sample_counter = 0
-        self.started = True
-
-        data_queue = Queue()
-        with Producer(data_queue, generator=self.generator,
-                      freq=1 / self.device_spec.sample_rate):
-            while self.running():
-                sample_counter += 1
-                try:
-                    sample = data_queue.get(True, 2)
-                    self.outlet.push_sample(sample)
-                    if self.add_markers and sample_counter % 1000 == 0:
-                        self.markers_outlet.push_sample(["1"])
-                except (Empty, AttributeError):
-                    # outlet.push_sample(sample) may cause an error after
-                    # the server has been stopped since the attribute is
-                    # deleted in another thread.
-                    break
-
-        log.debug("[*] No longer pushing data")
-
-
-def _settings(filename):
-    """Read the daq settings from the given data file"""
-
-    with open(filename, 'r', encoding=DEFAULT_ENCODING) as datafile:
-        daq_type = datafile.readline().strip().split(',')[1]
-        sample_hz = int(datafile.readline().strip().split(',')[1])
-        channels = datafile.readline().strip().split(',')
-        return (daq_type, sample_hz, channels)
-
-
-def await_start(dataserver: LslDataServer, max_wait: float = 2):
-    """Blocks until server is started. Raises if max_wait is exceeded before
-    server is started.
-
-    Parameters
-    ----------
-        dataserver - instantiated (unstarted) server on which to wait.
-        max_wait - the max number of seconds to wait. After this period if the
-            server has not succesfully started an exception is thrown.
-    """
-
-    dataserver.start()
-    wait = 0
-    wait_interval = 0.01
-    while not dataserver.started:
-        time.sleep(wait_interval)
-        wait += wait_interval
-        if wait >= max_wait:
-            dataserver.stop()
-            raise Exception("Server couldn't start up in time.")
-
-
-def main():
-    """Initialize and start the server."""
-    import time
-    import argparse
-
-    from bcipy.acquisition.datastream.generator import file_data_generator
-    from bcipy.acquisition.devices import preconfigured_device
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument('-f', '--filename', default=None,
-                        help="file containing data to be streamed; "
-                        "if missing, random data will be served.")
-    parser.add_argument('-m', '--markers', action="store_true", default=False)
-    parser.add_argument('-n', '--name', default='DSI-24', help='Name of the device spec to mock.')
-    args = parser.parse_args()
-
-    if args.filename:
-        daq_type, sample_rate, channels = _settings(args.filename)
-        device_spec = preconfigured_device(daq_type)
-        device_spec.sample_rate = sample_rate
-        device_spec.channels = channels
-        generator = file_data_generator(filename=args.filename)
-    else:
-        device_spec = preconfigured_device(args.name)
-        generator = None
-
-    markers = True if args.markers else False
-    try:
-        server = LslDataServer(device_spec=device_spec, generator=generator, add_markers=markers)
-
-        log.debug("New server created")
-        server.start()
-        log.debug("Server started")
-        while True:
-            time.sleep(1)
-    except KeyboardInterrupt:
-        print("Keyboard Interrupt")
-        server.stop()
-
-
-if __name__ == '__main__':
-    # Run this as: python -m bcipy.acquisition.datastream.lsl_server
-    main()
+"""Data server that streams EEG data over a LabStreamingLayer StreamOutlet
+using pylsl."""
+import logging
+from queue import Empty, Queue
+from typing import Generator
+import time
+import uuid
+
+from pylsl import StreamInfo, StreamOutlet
+
+from bcipy.config import DEFAULT_ENCODING
+from bcipy.acquisition.datastream.generator import random_data_generator
+from bcipy.acquisition.datastream.producer import Producer
+from bcipy.acquisition.devices import DeviceSpec
+from bcipy.acquisition.util import StoppableThread
+
+log = logging.getLogger(__name__)
+
+# pylint: disable=too-many-arguments
+
+MARKER_STREAM_NAME = 'TRG_device_stream'
+
+
+class LslDataServer(StoppableThread):
+    """Data server that streams EEG data over a LabStreamingLayer StreamOutlet
+    using pylsl. See https://github.com/sccn/labstreaminglayer/wiki.
+
+    In parameters.json, if the fake_data parameter is set to true and the
+    device is set to LSL, this server will be used to mock data. Alternatively,
+    fake_data can be set to false and this module can be run standalone in its
+    own python instance.
+
+    Parameters
+    ----------
+        device_spec : DeviceSpec
+            parameters used to configure the server. Should have at least
+            a list of channels and the sample frequency.
+        generator : optional Generator (see generator.py for options)
+            used to generate the data to be served. Uses random_data_generator
+            by default.
+        include_meta: bool, optional
+            if True, writes metadata to the outlet stream.
+        add_markers: bool, optional
+            if True, creates a the marker channel and streams data to this
+            channel at a fixed frequency.
+        marker_stream_name: str, optional
+            name of the sample marker stream
+    """
+
+    def __init__(self, device_spec: DeviceSpec, generator: Generator = None, include_meta: bool = True,
+                 add_markers: bool = False, marker_stream_name: str = MARKER_STREAM_NAME):
+        super(LslDataServer, self).__init__()
+
+        self.device_spec = device_spec
+        self.generator = generator or random_data_generator(channel_count=device_spec.channel_count)
+
+        log.debug("Starting LSL server for device: %s", device_spec.name)
+        print(f"Serving: {device_spec}")
+        info = StreamInfo(device_spec.name,
+                          device_spec.content_type, device_spec.channel_count,
+                          device_spec.sample_rate,
+                          device_spec.data_type,
+                          f'{device_spec.content_type.lower()}_{uuid.uuid1()}')
+
+        if include_meta:
+            # TODO: different types of metadata depending on the content type
+            unit = 'unknown'
+            channel_type = 'unknown'
+            if self.device_spec.content_type == 'EEG':
+                unit = 'microvolts'
+                channel_type = 'EEG'
+            meta_channels = info.desc().append_child('channels')
+            for channel in device_spec.channel_specs:
+                meta_channels.append_child('channel') \
+                    .append_child_value('label', channel.name) \
+                    .append_child_value('unit', channel.units or unit) \
+                    .append_child_value('type', channel.type or channel_type)
+
+        self.outlet = StreamOutlet(info)
+
+        self.add_markers = add_markers
+        if add_markers:
+            # Marker stream (C++ source below):
+            # lsl::stream_info marker_info("gUSBamp-"+deviceNumber+"Markers",
+            # "Markers",1,0,lsl::cf_string,
+            # "gUSBamp_" + boost::lexical_cast<std::string>(deviceNumber) +
+            # "_" + boost::lexical_cast<std::string>(serialNumber) +
+            # "_markers");
+            log.debug("Creating marker stream")
+            print(f"Marker channel name: {marker_stream_name}")
+            markers_info = StreamInfo(marker_stream_name,
+                                      "Markers", 1, 0, 'string',
+                                      "uid12345_markers")
+            self.markers_outlet = StreamOutlet(markers_info)
+        self.started = False
+
+    def stop(self):
+        """Stop the thread and cleanup resources."""
+
+        log.debug("[*] Stopping data server")
+        super(LslDataServer, self).stop()
+
+        # Allows pylsl to cleanup; The outlet will no longer be discoverable
+        # after destruction and all connected inlets will stop delivering data.
+        del self.outlet
+        self.outlet = None
+
+        if self.add_markers:
+            del self.markers_outlet
+            self.markers_outlet = None
+
+    def run(self):
+        """Main loop of the thread. Continuously streams data to the stream
+        outlet at a rate consistent with the sample frequency. May also
+        output markers at a different interval."""
+
+        sample_counter = 0
+        self.started = True
+
+        data_queue = Queue()
+        with Producer(data_queue, generator=self.generator,
+                      freq=1 / self.device_spec.sample_rate):
+            while self.running():
+                sample_counter += 1
+                try:
+                    sample = data_queue.get(True, 2)
+                    self.outlet.push_sample(sample)
+                    if self.add_markers and sample_counter % 1000 == 0:
+                        self.markers_outlet.push_sample(["1"])
+                except (Empty, AttributeError):
+                    # outlet.push_sample(sample) may cause an error after
+                    # the server has been stopped since the attribute is
+                    # deleted in another thread.
+                    break
+
+        log.debug("[*] No longer pushing data")
+
+
+def _settings(filename):
+    """Read the daq settings from the given data file"""
+
+    with open(filename, 'r', encoding=DEFAULT_ENCODING) as datafile:
+        daq_type = datafile.readline().strip().split(',')[1]
+        sample_hz = int(datafile.readline().strip().split(',')[1])
+        channels = datafile.readline().strip().split(',')
+        return (daq_type, sample_hz, channels)
+
+
+def await_start(dataserver: LslDataServer, max_wait: float = 2):
+    """Blocks until server is started. Raises if max_wait is exceeded before
+    server is started.
+
+    Parameters
+    ----------
+        dataserver - instantiated (unstarted) server on which to wait.
+        max_wait - the max number of seconds to wait. After this period if the
+            server has not succesfully started an exception is thrown.
+    """
+
+    dataserver.start()
+    wait = 0
+    wait_interval = 0.01
+    while not dataserver.started:
+        time.sleep(wait_interval)
+        wait += wait_interval
+        if wait >= max_wait:
+            dataserver.stop()
+            raise Exception("Server couldn't start up in time.")
+
+
+def main():
+    """Initialize and start the server."""
+    import time
+    import argparse
+
+    from bcipy.acquisition.datastream.generator import file_data_generator
+    from bcipy.acquisition.devices import preconfigured_device
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-f', '--filename', default=None,
+                        help="file containing data to be streamed; "
+                        "if missing, random data will be served.")
+    parser.add_argument('-m', '--markers', action="store_true", default=False)
+    parser.add_argument('-n', '--name', default='LSL', help='Name of the device spec to mock.')
+    args = parser.parse_args()
+
+    if args.filename:
+        daq_type, sample_rate, channels = _settings(args.filename)
+        device_spec = preconfigured_device(daq_type)
+        device_spec.sample_rate = sample_rate
+        device_spec.channels = channels
+        generator = file_data_generator(filename=args.filename)
+    else:
+        device_spec = preconfigured_device(args.name)
+        generator = None
+
+    markers = True if args.markers else False
+    try:
+        server = LslDataServer(device_spec=device_spec, generator=generator, add_markers=markers)
+
+        log.debug("New server created")
+        server.start()
+        log.debug("Server started")
+        while True:
+            time.sleep(1)
+    except KeyboardInterrupt:
+        print("Keyboard Interrupt")
+        server.stop()
+
+
+if __name__ == '__main__':
+    # Run this as: python -m bcipy.acquisition.datastream.lsl_server
+    main()
```

### Comparing `bcipy-2.0.0rc3/bcipy/acquisition/datastream/mock/eye_tracker_server.py` & `bcipy-2.0.1rc2/bcipy/acquisition/datastream/mock/eye_tracker_server.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/acquisition/datastream/mock/switch.py` & `bcipy-2.0.1rc2/bcipy/acquisition/datastream/mock/switch.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/acquisition/datastream/producer.py` & `bcipy-2.0.1rc2/bcipy/acquisition/datastream/producer.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/acquisition/devices.py` & `bcipy-2.0.1rc2/bcipy/acquisition/devices.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,225 +1,195 @@
-"""Functionality for loading and querying configuration for supported hardware
-devices."""
-import json
-import logging
-from pathlib import Path
-from typing import Dict, List, NamedTuple, Union
-
-from bcipy.config import DEFAULT_ENCODING, DEVICE_SPEC_PATH
-
-IRREGULAR_RATE = 0.0
-DEFAULT_CONFIG = DEVICE_SPEC_PATH
-_SUPPORTED_DEVICES = {}
-# see https://labstreaminglayer.readthedocs.io/projects/liblsl/ref/enums.html
-SUPPORTED_DATA_TYPES = [
-    'float32', 'double64', 'string', 'int32', 'int16', 'int8'
-]
-DEFAULT_DEVICE_TYPE = 'EEG'
-
-log = logging.getLogger(__name__)
-
-
-class ChannelSpec(NamedTuple):
-    """Represents metadata about a channel."""
-    name: str  # Label in the LSL metadata
-    label: str  # Label used within BciPy (raw_data, etc.)
-    type: str = None
-    units: str = None
-
-    def __repr__(self):
-        fields = ['name', 'label', 'type', 'units']
-        items = [(field, self.__getattribute__(field)) for field in fields]
-        props = [f"{key}='{val}'" for key, val in items if val]
-        return f"ChannelSpec({', '.join(props)})"
-
-
-def channel_spec(channel: Union[str, dict, ChannelSpec]) -> ChannelSpec:
-    """Creates a ChannelSpec from the given channel.
-
-    Parameters
-    ----------
-        channel - acquisition channel information specified as either just the
-          label or with additional data represented by a dict or ChannelSpec.
-    """
-    if isinstance(channel, str):
-        return ChannelSpec(name=channel, label=channel)
-    if isinstance(channel, ChannelSpec):
-        return channel
-    if isinstance(channel, dict):
-        return ChannelSpec(**channel)
-    raise Exception("Unexpected channel type")
-
-
-class DeviceSpec:
-    """Specification for a hardware device used in data acquisition.
-
-    Parameters
-    ----------
-        name - device short name; ex. DSI-24
-        channels - list of data collection channels; devices must have at least
-            one channel. Channels may be provided as a list of names or list of
-            ChannelSpecs.
-        sample_rate - sample frequency in Hz.
-        content_type - type of device; likely one of ['EEG', 'MoCap', 'Gaze',
-            'Audio', 'Markers']; see https://github.com/sccn/xdf/wiki/Meta-Data.
-        description - device description
-            ex. 'Wearable Sensing DSI-24 dry electrode EEG headset'
-        data_type - data format of a channel; all channels must have the same type;
-            see https://labstreaminglayer.readthedocs.io/projects/liblsl/ref/enums.html
-        excluded_from_analysis - list of channels (label) to exclude from analysis.
-    """
-
-    def __init__(self,
-                 name: str,
-                 channels: Union[List[str], List[ChannelSpec], List[dict]],
-                 sample_rate: float,
-                 content_type: str = DEFAULT_DEVICE_TYPE,
-                 description: str = None,
-                 excluded_from_analysis: List[str] = None,
-                 data_type='float32'):
-
-        assert sample_rate >= 0, "Sample rate can't be negative."
-        assert data_type in SUPPORTED_DATA_TYPES
-
-        self.name = name
-        self.channel_specs = [channel_spec(ch) for ch in channels]
-        self.sample_rate = sample_rate
-        self.content_type = content_type
-        self.description = description or name
-        self.data_type = data_type
-        self.excluded_from_analysis = excluded_from_analysis or []
-        self._validate_excluded_channels()
-
-    @property
-    def channel_count(self) -> int:
-        """Number of channels"""
-        return len(self.channel_specs)
-
-    @property
-    def channels(self) -> List[str]:
-        """List of channel labels. These may be customized for BciPy."""
-        return [ch.label for ch in self.channel_specs]
-
-    @property
-    def channel_names(self) -> List[str]:
-        """List of channel names from the device."""
-        return [ch.name for ch in self.channel_specs]
-
-    @property
-    def analysis_channels(self) -> List[str]:
-        """List of channels used for analysis by the signal module.
-        Parameters:
-        -----------
-            exclude_trg - indicates whether or not to exclude a TRG channel if present.
-        """
-
-        return list(
-            filter(lambda channel: channel not in self.excluded_from_analysis,
-                   self.channels))
-
-    def to_dict(self) -> dict:
-        """Converts the DeviceSpec to a dict."""
-        return {
-            'name': self.name,
-            'content_type': self.content_type,
-            'channels': [ch._asdict() for ch in self.channel_specs],
-            'sample_rate': self.sample_rate,
-            'description': self.description,
-            'excluded_from_analysis': self.excluded_from_analysis
-        }
-
-    def __str__(self):
-        """Custom str representation."""
-        names = [
-            'name', 'content_type', 'channels', 'sample_rate', 'description'
-        ]
-
-        def quoted_value(name):
-            value = self.__getattribute__(name)
-            return f"'{value}'" if isinstance(value, str) else value
-
-        props = [f"{name}={quoted_value(name)}" for name in names]
-        return f"DeviceSpec({', '.join(props)})"
-
-    def _validate_excluded_channels(self):
-        """Warn if excluded channels are not in the list of channels"""
-        for channel in self.excluded_from_analysis:
-            if channel not in self.channels:
-                log.warning(
-                    f"Excluded channel {channel} not found in spec for {self.name}"
-                )
-
-
-def make_device_spec(config: dict) -> DeviceSpec:
-    """Constructs a DeviceSpec from a dict. Throws a KeyError if any fields
-    are missing."""
-    return DeviceSpec(name=config['name'],
-                      content_type=config['content_type'],
-                      channels=config['channels'],
-                      sample_rate=config['sample_rate'],
-                      description=config['description'],
-                      excluded_from_analysis=config.get(
-                          'excluded_from_analysis', []))
-
-
-def load(config_path: Path = Path(DEFAULT_CONFIG), replace: bool = False) -> Dict[str, DeviceSpec]:
-    """Load the list of supported hardware for data acquisition from the given
-    configuration file.
-
-    Parameters
-    ----------
-        config_path - path to the devices json file
-        replace - optional; if true, existing devices are replaced; if false,
-            values will be overwritten or appended.
-    """
-    global _SUPPORTED_DEVICES
-
-    if config_path.is_file():
-        with open(config_path, 'r', encoding=DEFAULT_ENCODING) as json_file:
-            specs = [make_device_spec(entry) for entry in json.load(json_file)]
-            if specs and replace:
-                _SUPPORTED_DEVICES.clear()
-            for spec in specs:
-                _SUPPORTED_DEVICES[spec.name] = spec
-    return _SUPPORTED_DEVICES
-
-
-def preconfigured_devices() -> Dict[str, DeviceSpec]:
-    """Returns the preconfigured devices keyed by name. If no devices have yet
-    been configured, loads and returns the DEFAULT_CONFIG."""
-    global _SUPPORTED_DEVICES
-    if not _SUPPORTED_DEVICES:
-        load()
-    return _SUPPORTED_DEVICES
-
-
-def preconfigured_device(name: str, strict: bool = True) -> DeviceSpec:
-    """Retrieve the DeviceSpec with the given name. An exception is raised
-    if the device is not found."""
-    device = preconfigured_devices().get(name, None)
-    if strict and not device:
-        current = ', '.join(
-            [f"'{key}'" for key, _ in preconfigured_devices().items()])
-        msg = (
-            f"Device not found: {name}."
-            "\n\n"
-            f"The current list of devices includes the following: {current}."
-            "\n"
-            "You may register new devices using the device module `register` function or in bulk"
-            " using `load`.")
-        raise ValueError(msg)
-    return device
-
-
-def with_content_type(content_type: str) -> List[DeviceSpec]:
-    """Retrieve the list of DeviceSpecs with the given content_type."""
-    return [
-        spec for spec in preconfigured_devices().values()
-        if spec.content_type == content_type
-    ]
-
-
-def register(device_spec: DeviceSpec):
-    """Register the given DeviceSpec."""
-    config = preconfigured_devices()
-    config[device_spec.name] = device_spec
+"""Functionality for loading and querying configuration for supported hardware
+devices."""
+import json
+import logging
+from pathlib import Path
+from typing import Dict, List, NamedTuple, Union
+
+from bcipy.config import DEFAULT_ENCODING, DEVICE_SPEC_PATH
+
+IRREGULAR_RATE = 0.0
+DEFAULT_CONFIG = DEVICE_SPEC_PATH
+_SUPPORTED_DEVICES = {}
+# see https://labstreaminglayer.readthedocs.io/projects/liblsl/ref/enums.html
+SUPPORTED_DATA_TYPES = [
+    'float32', 'double64', 'string', 'int32', 'int16', 'int8'
+]
+DEFAULT_DEVICE_TYPE = 'EEG'
+
+log = logging.getLogger(__name__)
+
+
+class ChannelSpec(NamedTuple):
+    """Represents metadata about a channel."""
+    name: str  # Label in the LSL metadata
+    label: str  # Label used within BciPy (raw_data, etc.)
+    type: str = None
+    units: str = None
+
+    def __repr__(self):
+        fields = ['name', 'label', 'type', 'units']
+        items = [(field, self.__getattribute__(field)) for field in fields]
+        props = [f"{key}='{val}'" for key, val in items if val]
+        return f"ChannelSpec({', '.join(props)})"
+
+
+def channel_spec(channel: Union[str, dict, ChannelSpec]) -> ChannelSpec:
+    """Creates a ChannelSpec from the given channel.
+
+    Parameters
+    ----------
+        channel - acquisition channel information specified as either just the
+          label or with additional data represented by a dict or ChannelSpec.
+    """
+    if isinstance(channel, str):
+        return ChannelSpec(name=channel, label=channel)
+    if isinstance(channel, ChannelSpec):
+        return channel
+    if isinstance(channel, dict):
+        return ChannelSpec(**channel)
+    raise Exception("Unexpected channel type")
+
+
+class DeviceSpec:
+    """Specification for a hardware device used in data acquisition.
+
+    Parameters
+    ----------
+        name - device short name; ex. DSI-24
+        channels - list of data collection channels; devices must have at least
+            one channel. Channels may be provided as a list of names or list of
+            ChannelSpecs.
+        sample_rate - sample frequency in Hz.
+        content_type - type of device; likely one of ['EEG', 'MoCap', 'Gaze',
+            'Audio', 'Markers']; see https://github.com/sccn/xdf/wiki/Meta-Data.
+        description - device description
+            ex. 'Wearable Sensing DSI-24 dry electrode EEG headset'
+        data_type - data format of a channel; all channels must have the same type;
+            see https://labstreaminglayer.readthedocs.io/projects/liblsl/ref/enums.html
+        excluded_from_analysis - list of channels (label) to exclude from analysis.
+    """
+
+    def __init__(self,
+                 name: str,
+                 channels: Union[List[str], List[ChannelSpec], List[dict]],
+                 sample_rate: float,
+                 content_type: str = DEFAULT_DEVICE_TYPE,
+                 description: str = None,
+                 excluded_from_analysis: List[str] = None,
+                 data_type='float32'):
+
+        assert sample_rate >= 0, "Sample rate can't be negative."
+        assert data_type in SUPPORTED_DATA_TYPES
+
+        self.name = name
+        self.channel_specs = [channel_spec(ch) for ch in channels]
+        self.sample_rate = sample_rate
+        self.content_type = content_type
+        self.description = description or name
+        self.data_type = data_type
+        self.excluded_from_analysis = excluded_from_analysis or []
+        self._validate_excluded_channels()
+
+    @property
+    def channel_count(self) -> int:
+        """Number of channels"""
+        return len(self.channel_specs)
+
+    @property
+    def channels(self) -> List[str]:
+        """List of channel labels. These may be customized for BciPy."""
+        return [ch.label for ch in self.channel_specs]
+
+    @property
+    def channel_names(self) -> List[str]:
+        """List of channel names from the device."""
+        return [ch.name for ch in self.channel_specs]
+
+    @property
+    def analysis_channels(self) -> List[str]:
+        """List of channels used for analysis by the signal module.
+        Parameters:
+        -----------
+            exclude_trg - indicates whether or not to exclude a TRG channel if present.
+        """
+
+        return list(
+            filter(lambda channel: channel not in self.excluded_from_analysis,
+                   self.channels))
+
+    def to_dict(self) -> dict:
+        """Converts the DeviceSpec to a dict."""
+        return {
+            'name': self.name,
+            'content_type': self.content_type,
+            'channels': [ch._asdict() for ch in self.channel_specs],
+            'sample_rate': self.sample_rate,
+            'description': self.description,
+            'excluded_from_analysis': self.excluded_from_analysis
+        }
+
+    def __str__(self):
+        """Custom str representation."""
+        names = [
+            'name', 'content_type', 'channels', 'sample_rate', 'description'
+        ]
+
+        def quoted_value(name):
+            value = self.__getattribute__(name)
+            return f"'{value}'" if isinstance(value, str) else value
+
+        props = [f"{name}={quoted_value(name)}" for name in names]
+        return f"DeviceSpec({', '.join(props)})"
+
+    def _validate_excluded_channels(self):
+        """Warn if excluded channels are not in the list of channels"""
+        for channel in self.excluded_from_analysis:
+            if channel not in self.channels:
+                log.warning(
+                    f"Excluded channel {channel} not found in spec for {self.name}"
+                )
+
+
+def make_device_spec(config: dict) -> DeviceSpec:
+    """Constructs a DeviceSpec from a dict. Throws a KeyError if any fields
+    are missing."""
+    return DeviceSpec(name=config['name'],
+                      content_type=config['content_type'],
+                      channels=config['channels'],
+                      sample_rate=config['sample_rate'],
+                      description=config['description'],
+                      excluded_from_analysis=config.get(
+                          'excluded_from_analysis', []))
+
+
+def load(config_path: Path = Path(DEFAULT_CONFIG)) -> Dict[str, DeviceSpec]:
+    """Load the list of supported hardware for data acquisition from the given
+    configuration file."""
+    global _SUPPORTED_DEVICES
+    with open(config_path, 'r', encoding=DEFAULT_ENCODING) as json_file:
+        specs = [make_device_spec(entry) for entry in json.load(json_file)]
+        _SUPPORTED_DEVICES = {spec.name: spec for spec in specs}
+        return _SUPPORTED_DEVICES
+
+
+def preconfigured_devices() -> Dict[str, DeviceSpec]:
+    """Returns the preconfigured devices keyed by name."""
+    global _SUPPORTED_DEVICES
+    if not _SUPPORTED_DEVICES:
+        load()
+    return _SUPPORTED_DEVICES
+
+
+def preconfigured_device(name: str) -> DeviceSpec:
+    """Retrieve the DeviceSpec with the given name. An exception is raised
+    if the device is not found."""
+    device = preconfigured_devices().get(name, None)
+    if not device:
+        raise ValueError(f"Device not found: {name}")
+    return device
+
+
+def register(device_spec: DeviceSpec):
+    """Register the given DeviceSpec."""
+    config = preconfigured_devices()
+    config[device_spec.name] = device_spec
```

### Comparing `bcipy-2.0.0rc3/bcipy/acquisition/marker_writer.py` & `bcipy-2.0.1rc2/bcipy/acquisition/marker_writer.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/acquisition/protocols/lsl/lsl_client.py` & `bcipy-2.0.1rc2/bcipy/acquisition/protocols/lsl/lsl_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,319 +1,304 @@
-"""DataAcquisitionClient for LabStreamingLayer data sources."""
-import logging
-from typing import List
-
-from pylsl import StreamInfo, StreamInlet, local_clock, resolve_stream, resolve_byprop
-
-from bcipy.acquisition.devices import DEFAULT_DEVICE_TYPE, DeviceSpec, IRREGULAR_RATE
-from bcipy.acquisition.exceptions import InvalidClockError
-from bcipy.acquisition.protocols.lsl.lsl_connector import (channel_names,
-                                                           check_device)
-from bcipy.acquisition.protocols.lsl.lsl_recorder import LslRecordingThread
-from bcipy.acquisition.record import Record
-from bcipy.helpers.clock import Clock
-from bcipy.gui.viewer.ring_buffer import RingBuffer
-
-log = logging.getLogger(__name__)
-
-
-class LslAcquisitionClient:
-    """Data Acquisition Client for devices streaming data using Lab Streaming
-    Layer. Its primary use is dynamically querying streaming data in realtime,
-    however, if the save_directory and filename parameters are provided it uses
-    a LslRecordingThread to persist the data.
-
-    Parameters
-    ----------
-        max_buffer_len: the maximum length of data to be queried. For continuously
-            streaming data this is the number of seconds of data to retain. For
-            irregular data, specify the number of samples. When using the RSVP
-            paradigm, the max_buffer_len should be large enough to store data for
-            the entire inquiry.
-        device_spec: spec for the device from which to query data; if missing,
-            this class will attempt to find the first EEG stream.
-        save_directory: if present, persists the data to the given location.
-        raw_data_file_name: if present, uses this name for the data file.
-    """
-
-    def __init__(self,
-                 max_buffer_len: float = 1,
-                 device_spec: DeviceSpec = None,
-                 save_directory: str = None,
-                 raw_data_file_name: str = None):
-        super().__init__()
-        self.device_spec = device_spec
-        self.max_buffer_len = max_buffer_len
-
-        self.experiment_clock = None
-
-        self.inlet = None
-        self._first_sample_time = None
-
-        self.save_directory = save_directory
-        self.raw_data_file_name = raw_data_file_name
-
-        self.recorder = None
-        self.buffer = None
-
-    def start_acquisition(self) -> bool:
-        """Connect to the datasource and start acquiring data.
-
-        Returns
-        -------
-        bool : False if acquisition is already in progress, otherwise True.
-        """
-        if self.inlet:
-            return False
-
-        content_type = self.device_spec.content_type if self.device_spec else DEFAULT_DEVICE_TYPE
-        streams = resolve_stream('type', content_type)
-        if not streams:
-            raise Exception(
-                f'LSL Stream not found for content type {content_type}')
-        stream_info = streams[0]
-
-        self.inlet = StreamInlet(stream_info, max_buflen=self.max_buffer_len)
-
-        if self.device_spec:
-            check_device(self.device_spec, self.inlet.info())
-        else:
-            self.device_spec = device_from_metadata(self.inlet.info())
-
-        if self.save_directory:
-            self.recorder = LslRecordingThread(stream_info,
-                                               self.save_directory,
-                                               self.raw_data_file_name,
-                                               self.device_spec)
-            self.recorder.start()
-
-        if self.max_buffer_len and self.max_buffer_len > 0:
-            self.buffer = RingBuffer(size_max=self.max_samples)
-        _, self._first_sample_time = self.inlet.pull_sample()
-        return True
-
-    @property
-    def first_sample_time(self) -> float:
-        """Timestamp returned by the first sample. If the data is being
-        recorded this value reflects the timestamp of the first recorded sample"""
-        if self.recorder:
-            return self.recorder.first_sample_time
-        return self._first_sample_time
-
-    def stop_acquisition(self) -> None:
-        """Disconnect from the data source."""
-        log.debug("Stopping Acquisition...")
-        if self.inlet:
-            self.inlet.close_stream()
-            self.inlet = None
-        if self.recorder:
-            self.recorder.stop()
-            self.recorder.join()
-
-        self.buffer = None
-
-    def __enter__(self):
-        """Context manager enter method that starts data acquisition."""
-        self.start_acquisition()
-        return self
-
-    def __exit__(self, _exc_type, _exc_value, _traceback):
-        """Context manager exit method to clean up resources."""
-        self.stop_acquisition()
-
-    def get_data(self,
-                 start: float = None,
-                 end: float = None,
-                 limit: int = None) -> List[Record]:
-        """Get data in time range.
-
-        Parameters
-        ----------
-            start : starting timestamp (acquisition clock).
-            end : end timestamp (in acquisition clock).
-            limit: the max number of records that should be returned.
-
-        Returns
-        -------
-            List of Records
-        """
-        log.debug(f"Getting data from: {start} to: {end} limit: {limit}")
-
-        # Only data in the current buffer is available to query;
-        # requests for data outside of this will fail. Buffer size is
-        # set using the max_buffer_len parameter.
-        data = self.get_latest_data()
-
-        if not data:
-            log.debug('No records available')
-            return []
-
-        log.debug((f'{len(data)} records available '
-                   f'(From: {data[0].timestamp} To: {data[-1].timestamp})'))
-        start = start or data[0].timestamp
-        end = end or data[-1].timestamp
-        limit = limit or -1
-        assert start >= data[0].timestamp, (
-            f'Start time of {start} is out of range: '
-            f'({data[0].timestamp} to {data[-1].timestamp}).')
-
-        data_slice = [
-            record for record in data if start <= record.timestamp <= end
-        ][0:limit]
-        log.debug(f'{len(data_slice)} records returned')
-        return data_slice
-
-    @property
-    def max_samples(self) -> int:
-        """Maximum number of samples available at any given time."""
-        if self.device_spec.sample_rate == IRREGULAR_RATE:
-            return int(self.max_buffer_len)
-        return int(self.max_buffer_len * self.device_spec.sample_rate)
-
-    def get_latest_data(self) -> List[Record]:
-        """Add all available samples in the inlet to the buffer.
-
-        The number of items returned depends on the size of the configured
-        max_buffer_len and the amount of data available in the inlet."""
-        if not self.buffer:
-            return []
-        samples, timestamps = self.inlet.pull_chunk(
-            max_samples=self.max_samples)
-
-        for i, sample in enumerate(samples):
-            self.buffer.append(
-                Record(data=sample, timestamp=timestamps[i], rownum=None))
-
-        return self.buffer.get()
-
-    def convert_time(self, experiment_clock: Clock, timestamp: float) -> float:
-        """
-        Convert a timestamp from the experiment clock to the acquisition clock.
-        Used for querying the acquisition data for a time slice.
-
-        Parameters:
-        ----------
-        - experiment_clock : clock used to generate the timestamp
-        - timestamp : timestamp from the experiment clock
-
-        Returns:
-        --------
-            corresponding timestamp for the acquistion clock
-        """
-
-        # experiment_time = pylsl.local_clock() - offset
-        return timestamp + self.clock_offset(experiment_clock)
-
-    def get_data_seconds(self, seconds: int) -> List[Record]:
-        """Returns the last n second of data"""
-        assert seconds <= self.max_buffer_len, f"Seconds can't exceed {self.max_buffer_len}"
-
-        sample_count = seconds * self.device_spec.sample_rate
-        records = self.get_latest_data()
-
-        start_index = 0 if len(
-            records) > sample_count else len(records) - sample_count
-        return records[start_index:]
-
-    @property
-    def is_calibrated(self):
-        """Returns boolean indicating whether or not acquisition has been
-        calibrated (an offset calculated based on a trigger)."""
-        return True
-
-    @is_calibrated.setter
-    def is_calibrated(self, bool_val):
-        """Setter for the is_calibrated property that allows the user to
-        override the calculated value and use a 0 offset.
-
-        Parameters
-        ----------
-        - bool_val : boolean
-        if True, uses a 0 offset; if False forces the calculation.
-        """
-
-    def clock_offset(self, experiment_clock: Clock = None) -> float:
-        """
-        Offset in seconds from the experiment clock to the acquisition local clock.
-
-        The experiment clock should be monotonic from experiment start time.
-        The acquisition clock (pylsl.local_clock()) is monotonic from local
-        machine start time (or since 1970-01-01 00:00). Therefore the acquisition
-        clock should always be greater than experiment clock. An exception is
-        raised if this doesn't hold.
-
-        See https://labstreaminglayer.readthedocs.io/info/faqs.html#lsl-local-clock
-        """
-        clock = experiment_clock or self.experiment_clock
-        assert clock, "An experiment clock must be provided"
-
-        diff = local_clock() - clock.getTime()
-        if diff < 0:
-            raise InvalidClockError(
-                "The acquisition clock should always be greater than experiment clock"
-            )
-        return diff
-
-    def event_offset(self, event_clock: Clock, event_time: float) -> float:
-        """Compute number of seconds that recording started prior to the given
-        event.
-
-        Parameters
-        ----------
-        - event_clock : monotonic clock used to record the event time.
-        - event_time : timestamp of the event of interest.
-
-        Returns
-        -------
-        Seconds between acquisition start and the event.
-        """
-        if self.first_sample_time:
-            lsl_event_time = self.convert_time(event_clock, event_time)
-            return lsl_event_time - self.first_sample_time
-        return 0.0
-
-    def offset(self, first_stim_time: float) -> float:
-        """Offset in seconds from the start of acquisition to the given stim
-        time.
-
-        Parameters
-        ----------
-        - first_stim_time : LSL local clock timestamp of the first stimulus.
-
-        Returns
-        -------
-        The number of seconds between acquisition start and the calibration
-        event, or 0.0 .
-        """
-
-        if not first_stim_time:
-            return 0.0
-        assert self.first_sample_time, "Acquisition was not started."
-        offset_from_stim = first_stim_time - self.first_sample_time
-        log.debug(f"Acquisition offset: {offset_from_stim}")
-        return offset_from_stim
-
-    def cleanup(self):
-        """Perform any necessary cleanup."""
-
-
-def discover_device_spec(content_type: str) -> DeviceSpec:
-    """Finds the first LSL stream with the given content type and creates a
-    device spec from the stream's metadata."""
-    log.info(f"Waiting for {content_type} data to be streamed over LSL.")
-    streams = resolve_byprop('type', content_type, timeout=5.0)
-    if not streams:
-        raise Exception(
-            f'LSL Stream not found for content type {content_type}')
-    stream_info = streams[0]
-    inlet = StreamInlet(stream_info)
-    spec = device_from_metadata(inlet.info())
-    inlet.close_stream()
-    return spec
-
-
-def device_from_metadata(metadata: StreamInfo) -> DeviceSpec:
-    """Create a device_spec from the data stream metadata."""
-    return DeviceSpec(name=metadata.name(),
-                      channels=channel_names(metadata),
-                      sample_rate=metadata.nominal_srate(),
-                      content_type=metadata.type())
+"""DataAcquisitionClient for LabStreamingLayer data sources."""
+import logging
+from typing import List
+
+from pylsl import StreamInfo, StreamInlet, local_clock, resolve_stream
+
+from bcipy.acquisition.devices import DEFAULT_DEVICE_TYPE, DeviceSpec, IRREGULAR_RATE
+from bcipy.acquisition.exceptions import InvalidClockError
+from bcipy.acquisition.protocols.lsl.lsl_connector import (channel_names,
+                                                           check_device)
+from bcipy.acquisition.protocols.lsl.lsl_recorder import LslRecordingThread
+from bcipy.acquisition.record import Record
+from bcipy.helpers.clock import Clock
+from bcipy.gui.viewer.ring_buffer import RingBuffer
+
+log = logging.getLogger(__name__)
+
+
+class LslAcquisitionClient:
+    """Data Acquisition Client for devices streaming data using Lab Streaming
+    Layer. Its primary use is dynamically querying streaming data in realtime,
+    however, if the save_directory and filename parameters are provided it uses
+    a LslRecordingThread to persist the data.
+
+    Parameters
+    ----------
+        max_buffer_len: the maximum length of data to be queried. For continuously
+            streaming data this is the number of seconds of data to retain. For
+            irregular data, specify the number of samples. When using the RSVP
+            paradigm, the max_buffer_len should be large enough to store data for
+            the entire inquiry.
+        device_spec: spec for the device from which to query data; if missing,
+            this class will attempt to find the first EEG stream.
+        save_directory: if present, persists the data to the given location.
+        raw_data_file_name: if present, uses this name for the data file.
+    """
+
+    def __init__(self,
+                 max_buffer_len: float = 1,
+                 device_spec: DeviceSpec = None,
+                 save_directory: str = None,
+                 raw_data_file_name: str = None):
+        super().__init__()
+        self.device_spec = device_spec
+        self.max_buffer_len = max_buffer_len
+
+        self.experiment_clock = None
+
+        self.inlet = None
+        self._first_sample_time = None
+
+        self.save_directory = save_directory
+        self.raw_data_file_name = raw_data_file_name
+
+        self.recorder = None
+        self.buffer = None
+
+    def start_acquisition(self) -> bool:
+        """Connect to the datasource and start acquiring data.
+
+        Returns
+        -------
+        bool : False if acquisition is already in progress, otherwise True.
+        """
+        if self.inlet:
+            return False
+
+        content_type = self.device_spec.content_type if self.device_spec else DEFAULT_DEVICE_TYPE
+        streams = resolve_stream('type', content_type)
+        if not streams:
+            raise Exception(
+                f'LSL Stream not found for content type {content_type}')
+        stream_info = streams[0]
+
+        self.inlet = StreamInlet(stream_info, max_buflen=self.max_buffer_len)
+
+        if self.device_spec:
+            check_device(self.device_spec, self.inlet.info())
+        else:
+            self.device_spec = device_from_metadata(self.inlet.info())
+
+        if self.save_directory:
+            self.recorder = LslRecordingThread(stream_info,
+                                               self.save_directory,
+                                               self.raw_data_file_name,
+                                               self.device_spec)
+            self.recorder.start()
+
+        if self.max_buffer_len and self.max_buffer_len > 0:
+            self.buffer = RingBuffer(size_max=self.max_samples)
+        _, self._first_sample_time = self.inlet.pull_sample()
+        return True
+
+    @property
+    def first_sample_time(self) -> float:
+        """Timestamp returned by the first sample. If the data is being
+        recorded this value reflects the timestamp of the first recorded sample"""
+        if self.recorder:
+            return self.recorder.first_sample_time
+        return self._first_sample_time
+
+    def stop_acquisition(self) -> None:
+        """Disconnect from the data source."""
+        log.debug("Stopping Acquisition...")
+        if self.inlet:
+            self.inlet.close_stream()
+            self.inlet = None
+        if self.recorder:
+            self.recorder.stop()
+            self.recorder.join()
+
+        self.buffer = None
+
+    def __enter__(self):
+        """Context manager enter method that starts data acquisition."""
+        self.start_acquisition()
+        return self
+
+    def __exit__(self, _exc_type, _exc_value, _traceback):
+        """Context manager exit method to clean up resources."""
+        self.stop_acquisition()
+
+    def get_data(self,
+                 start: float = None,
+                 end: float = None,
+                 limit: int = None) -> List[Record]:
+        """Get data in time range.
+
+        Parameters
+        ----------
+            start : starting timestamp (acquisition clock).
+            end : end timestamp (in acquisition clock).
+            limit: the max number of records that should be returned.
+
+        Returns
+        -------
+            List of Records
+        """
+        log.debug(f"Getting data from: {start} to: {end} limit: {limit}")
+
+        # Only data in the current buffer is available to query;
+        # requests for data outside of this will fail. Buffer size is
+        # set using the max_buffer_len parameter.
+        data = self.get_latest_data()
+
+        if not data:
+            log.debug('No records available')
+            return []
+
+        log.debug((f'{len(data)} records available '
+                   f'(From: {data[0].timestamp} To: {data[-1].timestamp})'))
+        start = start or data[0].timestamp
+        end = end or data[-1].timestamp
+        limit = limit or -1
+        assert start >= data[0].timestamp, (
+            f'Start time of {start} is out of range: '
+            f'({data[0].timestamp} to {data[-1].timestamp}).')
+
+        data_slice = [
+            record for record in data if start <= record.timestamp <= end
+        ][0:limit]
+        log.debug(f'{len(data_slice)} records returned')
+        return data_slice
+
+    @property
+    def max_samples(self) -> int:
+        """Maximum number of samples available at any given time."""
+        if self.device_spec.sample_rate == IRREGULAR_RATE:
+            return int(self.max_buffer_len)
+        return int(self.max_buffer_len * self.device_spec.sample_rate)
+
+    def get_latest_data(self) -> List[Record]:
+        """Add all available samples in the inlet to the buffer.
+
+        The number of items returned depends on the size of the configured
+        max_buffer_len and the amount of data available in the inlet."""
+        if not self.buffer:
+            return []
+        samples, timestamps = self.inlet.pull_chunk(
+            max_samples=self.max_samples)
+
+        for i, sample in enumerate(samples):
+            self.buffer.append(
+                Record(data=sample, timestamp=timestamps[i], rownum=None))
+
+        return self.buffer.get()
+
+    def convert_time(self, experiment_clock: Clock, timestamp: float) -> float:
+        """
+        Convert a timestamp from the experiment clock to the acquisition clock.
+        Used for querying the acquisition data for a time slice.
+
+        Parameters:
+        ----------
+        - experiment_clock : clock used to generate the timestamp
+        - timestamp : timestamp from the experiment clock
+
+        Returns:
+        --------
+            corresponding timestamp for the acquistion clock
+        """
+
+        # experiment_time = pylsl.local_clock() - offset
+        return timestamp + self.clock_offset(experiment_clock)
+
+    def get_data_seconds(self, seconds: int) -> List[Record]:
+        """Returns the last n second of data"""
+        assert seconds <= self.max_buffer_len, f"Seconds can't exceed {self.max_buffer_len}"
+
+        sample_count = seconds * self.device_spec.sample_rate
+        records = self.get_latest_data()
+
+        start_index = 0 if len(
+            records) > sample_count else len(records) - sample_count
+        return records[start_index:]
+
+    @property
+    def is_calibrated(self):
+        """Returns boolean indicating whether or not acquisition has been
+        calibrated (an offset calculated based on a trigger)."""
+        return True
+
+    @is_calibrated.setter
+    def is_calibrated(self, bool_val):
+        """Setter for the is_calibrated property that allows the user to
+        override the calculated value and use a 0 offset.
+
+        Parameters
+        ----------
+        - bool_val : boolean
+        if True, uses a 0 offset; if False forces the calculation.
+        """
+
+    def clock_offset(self, experiment_clock: Clock = None) -> float:
+        """
+        Offset in seconds from the experiment clock to the acquisition local clock.
+
+        The experiment clock should be monotonic from experiment start time.
+        The acquisition clock (pylsl.local_clock()) is monotonic from local
+        machine start time (or since 1970-01-01 00:00). Therefore the acquisition
+        clock should always be greater than experiment clock. An exception is
+        raised if this doesn't hold.
+
+        See https://labstreaminglayer.readthedocs.io/info/faqs.html#lsl-local-clock
+        """
+        clock = experiment_clock or self.experiment_clock
+        assert clock, "An experiment clock must be provided"
+
+        diff = local_clock() - clock.getTime()
+        if diff < 0:
+            raise InvalidClockError(
+                "The acquisition clock should always be greater than experiment clock"
+            )
+        return diff
+
+    def event_offset(self, event_clock: Clock, event_time: float) -> float:
+        """Compute number of seconds that recording started prior to the given
+        event.
+
+        Parameters
+        ----------
+        - event_clock : monotonic clock used to record the event time.
+        - event_time : timestamp of the event of interest.
+
+        Returns
+        -------
+        Seconds between acquisition start and the event.
+        """
+        if self.first_sample_time:
+            lsl_event_time = self.convert_time(event_clock, event_time)
+            return lsl_event_time - self.first_sample_time
+        return 0.0
+
+    def offset(self, first_stim_time: float) -> float:
+        """Offset in seconds from the start of acquisition to the given stim
+        time.
+
+        Parameters
+        ----------
+        - first_stim_time : LSL local clock timestamp of the first stimulus.
+
+        Returns
+        -------
+        The number of seconds between acquisition start and the calibration
+        event, or 0.0 .
+        """
+
+        if not first_stim_time:
+            return 0.0
+        assert self.first_sample_time, "Acquisition was not started."
+        offset_from_stim = first_stim_time - self.first_sample_time
+        log.debug(f"Acquisition offset: {offset_from_stim}")
+        return offset_from_stim
+
+    def cleanup(self):
+        """Perform any necessary cleanup."""
+
+
+def device_from_metadata(metadata: StreamInfo) -> DeviceSpec:
+    """Create a device_spec from the data stream metadata."""
+    return DeviceSpec(name=metadata.name(),
+                      channels=channel_names(metadata),
+                      sample_rate=metadata.nominal_srate(),
+                      content_type=metadata.type())
```

### Comparing `bcipy-2.0.0rc3/bcipy/acquisition/protocols/lsl/lsl_connector.py` & `bcipy-2.0.1rc2/bcipy/acquisition/protocols/lsl/lsl_connector.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/acquisition/protocols/lsl/lsl_recorder.py` & `bcipy-2.0.1rc2/bcipy/acquisition/protocols/lsl/lsl_recorder.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/acquisition/util.py` & `bcipy-2.0.1rc2/bcipy/acquisition/util.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/config.py` & `bcipy-2.0.1rc2/bcipy/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,23 +17,19 @@
 DEFAULT_EXPERIMENT_PATH = f'{ROOT}/.bcipy/experiment'
 DEFAULT_FIELD_PATH = f'{ROOT}/.bcipy/field'
 
 DEFAULT_PARAMETER_FILENAME = 'parameters.json'
 DEFAULT_PARAMETERS_PATH = f'{BCIPY_ROOT}/parameters/{DEFAULT_PARAMETER_FILENAME}'
 DEFAULT_DEVICE_SPEC_FILENAME = 'devices.json'
 DEVICE_SPEC_PATH = f'{BCIPY_ROOT}/parameters/{DEFAULT_DEVICE_SPEC_FILENAME}'
-DEFAULT_LM_PARAMETERS_FILENAME = 'lm_params.json'
-DEFAULT_LM_PARAMETERS_PATH = f'{BCIPY_ROOT}/parameters/{DEFAULT_LM_PARAMETERS_FILENAME}'
 
 STATIC_PATH = f'{BCIPY_ROOT}/static'
 STATIC_IMAGES_PATH = f'{STATIC_PATH}/images'
 STATIC_AUDIO_PATH = f'{STATIC_PATH}/sounds'
 BCIPY_LOGO_PATH = f'{STATIC_IMAGES_PATH}/gui/cambi.png'
-PREFERENCES_PATH = f'{ROOT}/.bcipy/bcipy_cache'
-LM_PATH = f'{BCIPY_ROOT}/language/lms'
 
 # core data configuration
 RAW_DATA_FILENAME = 'raw_data'
 TRIGGER_FILENAME = 'triggers.txt'
 SESSION_DATA_FILENAME = 'session.json'
 SESSION_SUMMARY_FILENAME = 'session.xlsx'
 LOG_FILENAME = 'bcipy_system_log.txt'
```

### Comparing `bcipy-2.0.0rc3/bcipy/display/__init__.py` & `bcipy-2.0.1rc2/bcipy/display/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 from bcipy.config import BCIPY_LOGO_PATH
 from .main import (
     Display,
     InformationProperties,
     init_display_window,
     PreviewInquiryProperties,
     StimuliProperties,
-    VEPStimuliProperties
+    VEPStimuliProperties,
+    TaskDisplayProperties,
 )
 
 __all__ = [
     'Display',
     'init_display_window',
     'BCIPY_LOGO_PATH',
     'StimuliProperties',
     'VEPStimuliProperties',
     'InformationProperties',
+    'TaskDisplayProperties',
     'PreviewInquiryProperties'
 ]
```

### Comparing `bcipy-2.0.0rc3/bcipy/display/main.py` & `bcipy-2.0.1rc2/bcipy/display/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from logging import Logger
 from typing import List, Tuple, Union
 
 from psychopy import visual
 
 from bcipy.helpers.clock import Clock
-from bcipy.helpers.system_utils import get_screen_info
+from bcipy.helpers.system_utils import get_screen_resolution
 
 
 class Display(ABC):
     """Display.
 
     Base class for BciPy displays. This defines the logic necessary for task executions that require a display.
     """
@@ -36,18 +36,18 @@
         """Wait Screen.
 
         Define what happens on the screen when a user pauses a session.
         """
         ...
 
     @abstractmethod
-    def update_task_bar(self, *args, **kwargs) -> None:
+    def update_task(self) -> None:
         """Update Task.
 
-        Update any taskbar-related display items not related to the inquiry. Ex. stimuli count 1/200.
+        Update any task related display items not related to the inquiry. Ex. stimuli count 1/200.
         """
         ...
 
     def schedule_to(self, stimuli: list, timing: list, colors: list) -> None:
         """Schedule To.
 
         Schedule stimuli elements (works as a buffer) before calling do_inquiry.
@@ -84,17 +84,15 @@
         http://www.psychopy.org/api/visual/window.html
     """
 
     # Check is full_screen mode is set and get necessary values
     if parameters['full_screen']:
 
         # set window attributes based on resolution
-        screen_info = get_screen_info()
-        window_height = screen_info.height
-        window_width = screen_info.width
+        window_width, window_height = get_screen_resolution()
 
         # set full screen mode to true (removes os dock, explorer etc.)
         full_screen = True
 
     # otherwise, get user defined window attributes
     else:
 
@@ -129,36 +127,36 @@
     """
 
     def __init__(
             self,
             stim_font: str,
             stim_pos: Tuple[float, float],
             stim_height: float,
-            stim_inquiry: List[str] = None,
-            stim_colors: List[str] = None,
-            stim_timing: List[float] = None,
-            is_txt_stim: bool = True,
+            stim_inquiry: List[str],
+            stim_colors: List[str],
+            stim_timing: List[float],
+            is_txt_stim: bool,
             prompt_time: float = None):
         """Initialize Stimuli Parameters.
 
         stim_font(List[str]): Ordered list of colors to apply to information stimuli
         stim_pos(Tuple[float, float]): Position on window where the stimuli will be presented
         stim_height(float): Height of all stimuli
         stim_inquiry(List[str]): Ordered list of text to build stimuli with
         stim_colors(List[str]): Ordered list of colors to apply to stimuli
         stim_timing(List[float]): Ordered list of timing to apply to an inquiry using the stimuli
         is_txt_stim(bool): Whether or not this is a text based stimuli (False implies image based)
-        prompt_time(float): Time to display target prompt for at the beginning of inquiry
+        prompt_time(float): Time to display target prompt for at the beggining of inquiry
         """
         self.stim_font = stim_font
         self.stim_pos = stim_pos
         self.stim_height = stim_height
-        self.stim_inquiry = stim_inquiry or []
-        self.stim_colors = stim_colors or []
-        self.stim_timing = stim_timing or []
+        self.stim_inquiry = stim_inquiry
+        self.stim_colors = stim_colors
+        self.stim_timing = stim_timing
         self.is_txt_stim = is_txt_stim
         self.stim_length = len(self.stim_inquiry)
         self.sti = None
         self.prompt_time = prompt_time
 
     def build_init_stimuli(self, window: visual.Window) -> Union[visual.TextStim, visual.ImageStim]:
         """"Build Initial Stimuli.
@@ -230,28 +228,73 @@
                 font=self.info_font[idx],
                 pos=self.info_pos[idx],
                 wrapWidth=None, colorSpace='rgb',
                 opacity=1, depth=-6.0))
         return self.text_stim
 
 
+class TaskDisplayProperties:
+    """"Task Dispay Properties.
+
+    An encapsulation of properties relevant to task stimuli presentation in an RSVP paradigm.
+    """
+
+    def __init__(
+            self,
+            task_color: List[str],
+            task_font: str,
+            task_pos: Tuple[float, float],
+            task_height: float,
+            task_text: str):
+        """Initialize Task Display Parameters.
+
+        task_color(List[str]): Ordered list of colors to apply to task stimuli
+        task_font(str): Font to apply to all task stimuli
+        task_pos(Tuple[float, float]): Position on the screen where to present to task text
+        task_height(float): Height of all task text stimuli
+        task_text(str): Task text to apply to stimuli
+        """
+        self.task_color = task_color
+        self.task_font = task_font
+        self.task_pos = task_pos
+        self.task_height = task_height
+        self.task_text = task_text
+        self.task = None
+
+    def build_task(self, window: visual.Window) -> visual.TextStim:
+        """"Build Task.
+
+        This method constructs the task stimuli object which can be updated later. This is more
+            performant than creating a new stimuli for each update in task state.
+        """
+        self.task = visual.TextStim(
+            win=window,
+            color=self.task_color[0],
+            height=self.task_height,
+            text=self.task_text,
+            font=self.task_font,
+            pos=self.task_pos,
+            wrapWidth=None, colorSpace='rgb',
+            opacity=1, depth=-6.0)
+        return self.task
+
+
 class PreviewInquiryProperties:
     """"Preview Inquiry Properties.
     An encapsulation of properties relevant to preview_inquiry() operation.
     """
 
     def __init__(
             self,
             preview_only: bool,
             preview_inquiry_length: float,
             preview_inquiry_progress_method: int,
             preview_inquiry_key_input: str,
             preview_inquiry_isi: float):
         """Initialize Inquiry Preview Parameters.
-        preview_only(bool): If True, only preview the inquiry and do not probe for response
         preview_inquiry_length(float): Length of time in seconds to present the inquiry preview
         preview_inquiry_progress_method(int): Method of progression for inquiry preview.
             0 == preview only; 1 == press to accept inquiry; 2 == press to skip inquiry.
         preview_inquiry_key_input(str): Defines which key should be listened to for progressing
         preview_inquiry_isi(float): Length of time after displaying the inquiry preview to display a blank screen
         """
         self.preview_inquiry_length = preview_inquiry_length
```

### Comparing `bcipy-2.0.0rc3/bcipy/display/paradigm/matrix/display.py` & `bcipy-2.0.1rc2/bcipy/display/paradigm/matrix/display.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,351 +1,354 @@
-"""Display for presenting stimuli in a grid."""
-from typing import Dict, List, Optional, Tuple, NamedTuple
-import logging
-
-from psychopy import visual, core
-
-from bcipy.display import Display, StimuliProperties, InformationProperties, BCIPY_LOGO_PATH
-from bcipy.helpers.stimuli import resize_image
-from bcipy.helpers.triggers import _calibration_trigger
-from bcipy.helpers.symbols import alphabet
-from bcipy.display.components.task_bar import TaskBar
-
-
-class SymbolDuration(NamedTuple):
-    """Represents a symbol and its associated duration to display"""
-    symbol: str
-    duration: float
-    color: str = 'white'
-
-
-class MatrixDisplay(Display):
-    """Matrix Display Object for Inquiry Presentation.
-
-    Animates display objects in matrix grid common to any Matrix task.
-
-    NOTE: The following are recommended parameter values for matrix experiments:
-
-    time_fixation: 2
-    stim_pos_x: -0.6
-    stim_pos_y: 0.4
-    stim_height: 0.1
-    """
-
-    def __init__(
-            self,
-            window: visual.Window,
-            experiment_clock: core.Clock,
-            stimuli: StimuliProperties,
-            task_bar: TaskBar,
-            info: InformationProperties,
-            trigger_type: str = 'text',
-            symbol_set: Optional[List[str]] = None,
-            should_prompt_target: bool = True):
-        """Initialize Matrix display parameters and objects.
-
-        PARAMETERS:
-        ----------
-        # Experiment
-        window(visual.Window): PsychoPy Window
-        experiment_clock(core.Clock): Clock used to timestamp display onsets
-
-        # Stimuli
-        stimuli(StimuliProperties): attributes used for inquiries
-
-        # Task
-        task_bar(TaskBar): used for task tracking. Ex. 1/100
-
-        # Info
-        info(InformationProperties): attributes to display informational stimuli alongside task and inquiry stimuli.
-
-        trigger_type(str) default 'image': defines the calibration trigger type for the display at the beginning of any
-            task. This will be used to reconcile timing differences between acquisition and the display.
-        symbol_set default = none : subset of stimuli to be highlighted during an inquiry
-        should_prompt_target(bool): when True prompts for the target symbol. Assumes that this is
-            the first symbol of each inquiry. For example: [target, fixation, *stim].
-        """
-        self.window = window
-
-        self.logger = logging.getLogger(__name__)
-
-        self.stimuli_inquiry = []
-        self.stimuli_timing = []
-        self.stimuli_colors = []
-        self.stimuli_font = stimuli.stim_font
-
-        assert stimuli.is_txt_stim, "Matrix display is a text only display"
-
-        self.symbol_set = symbol_set or alphabet()
-
-        # Set position and parameters for grid of alphabet
-        self.position = stimuli.stim_pos
-        self.grid_stimuli_height = .17
-        self.position_increment = self.grid_stimuli_height + .05
-        self.max_grid_width = 0.7
-
-        self.grid_color = 'white'
-        self.start_opacity = 0.15
-        self.highlight_opacity = 0.95
-        self.full_grid_opacity = 0.95
-
-        # Trigger handling
-        self.first_run = True
-        self.first_stim_time = None
-        self.trigger_type = trigger_type
-        self._timing = []
-
-        self.experiment_clock = experiment_clock
-
-        self.task_bar = task_bar
-        self.info_text = info.build_info_text(window)
-
-        self.stim_registry = self.build_grid()
-        self.should_prompt_target = should_prompt_target
-
-    def schedule_to(self, stimuli: list, timing: list, colors: list) -> None:
-        """Schedule stimuli elements (works as a buffer).
-
-        Args:
-                stimuli(list[string]): list of stimuli text / name
-                timing(list[float]): list of timings of stimuli
-                colors(list[string]): list of colors
-        """
-        assert len(stimuli) == len(
-            timing), "each stimuli must have a timing value"
-        self.stimuli_inquiry = stimuli
-        self.stimuli_timing = timing
-        if colors:
-            assert len(stimuli) == len(colors), "each stimuli must have a color"
-            self.stimuli_colors = colors
-        else:
-            self.stimuli_colors = [self.grid_color] * len(stimuli)
-
-    def symbol_durations(self) -> List[SymbolDuration]:
-        """Symbols associated with their duration for the currently configured
-        stimuli_inquiry."""
-        return [
-            SymbolDuration(*sti)
-            for sti in zip(self.stimuli_inquiry, self.stimuli_timing, self.stimuli_colors)
-        ]
-
-    def add_timing(self, stimuli: str):
-        """Add a new timing entry using the stimuli as a label.
-
-        Useful as a callback function to register a marker at the time it is
-        first displayed."""
-        self._timing.append([stimuli, self.experiment_clock.getTime()])
-
-    def reset_timing(self):
-        """Reset the trigger timing."""
-        self._timing = []
-
-    def do_inquiry(self) -> List[float]:
-        """Animates an inquiry of stimuli and returns a list of stimuli trigger timing."""
-        self.reset_timing()
-        symbol_durations = self.symbol_durations()
-
-        if self.first_run:
-            self._trigger_pulse()
-
-        if self.should_prompt_target:
-            [target, fixation, *stim] = symbol_durations
-            self.prompt_target(target)
-        else:
-            [fixation, *stim] = symbol_durations
-
-        self.animate_scp(fixation, stim)
-
-        return self._timing
-
-    def build_grid(self) -> Dict[str, visual.TextStim]:
-        """Build grid.
-
-        Builds a 7x4 matrix of stimuli.
-        """
-        grid = {}
-        pos = self.position
-        for sym in self.symbol_set:
-            grid[sym] = visual.TextStim(win=self.window,
-                                        text=sym,
-                                        color=self.grid_color,
-                                        opacity=self.start_opacity,
-                                        pos=pos,
-                                        height=self.grid_stimuli_height)
-            pos = self.increment_position(pos)
-        return grid
-
-    def increment_position(self, pos: Tuple[float, float]) -> Tuple[float, float]:
-        """Computes the position of the next symbol in the matrix."""
-        x_coordinate, y_coordinate = pos
-        x_coordinate += self.position_increment
-        if x_coordinate >= self.max_grid_width:
-            y_coordinate -= self.position_increment
-            x_coordinate = self.position[0]
-        return (x_coordinate, y_coordinate)
-
-    def draw_grid(self,
-                  opacity: float = 1,
-                  color: Optional[str] = 'white',
-                  highlight: Optional[str] = None,
-                  highlight_color: Optional[str] = None):
-        """Draw the grid.
-
-        Parameters
-        ----------
-            opacity - opacity for each item in the matrix
-            color - optional color for each item in the matrix
-            highlight - optional stim label for the item to be highlighted
-                (rendered using the highlight_opacity).
-            highlight_color - optional color to use for rendering the
-              highlighted stim.
-        """
-        for symbol, stim in self.stim_registry.items():
-            stim.setOpacity(self.highlight_opacity if highlight ==
-                            symbol else opacity)
-            stim.setColor(highlight_color if highlight_color and
-                          highlight == symbol else color)
-            stim.draw()
-
-    def prompt_target(self, target: SymbolDuration) -> float:
-        """Present the target for the configured length of time. Records the
-        stimuli timing information.
-
-        Parameters
-        ----------
-            target - (symbol, duration) tuple
-        """
-        # register any timing and marker callbacks
-        self.window.callOnFlip(self.add_timing, target.symbol)
-        self.draw(grid_opacity=self.start_opacity,
-                  duration=target.duration,
-                  highlight=target.symbol,
-                  highlight_color=target.color)
-
-    def draw(self,
-             grid_opacity: float,
-             grid_color: Optional[str] = None,
-             duration: Optional[float] = None,
-             highlight: Optional[str] = None,
-             highlight_color: Optional[str] = None):
-        """Draw all screen elements and flip the window.
-
-        Parameters
-        ----------
-            grid_opacity - opacity value to use on all grid symbols
-            grid_color - optional color to use for all grid symbols
-            duration - optional seconds to wait after flipping the window.
-            highlight - optional symbol to highlight in the grid.
-            highlight_color - optional color to use for rendering the
-              highlighted stim.
-        """
-        self.draw_grid(opacity=grid_opacity,
-                       color=grid_color or self.grid_color,
-                       highlight=highlight,
-                       highlight_color=highlight_color)
-        self.draw_static()
-        self.window.flip()
-        if duration:
-            core.wait(duration)
-
-    def animate_scp(self, fixation: SymbolDuration,
-                    stimuli: List[SymbolDuration]):
-        """Animate the given stimuli using single character presentation.
-
-        Flashes each stimuli in stimuli_inquiry for their respective flash
-        times and records the timing information.
-        """
-
-        # Flashing the grid at full opacity is considered fixation.
-        self.window.callOnFlip(self.add_timing, fixation.symbol)
-        self.draw(grid_opacity=self.full_grid_opacity,
-                  grid_color=(fixation.color if self.should_prompt_target else
-                              self.grid_color),
-                  duration=fixation.duration / 2)
-        self.draw(grid_opacity=self.start_opacity,
-                  duration=fixation.duration / 2)
-
-        for stim in stimuli:
-            self.window.callOnFlip(self.add_timing, stim.symbol)
-            self.draw(grid_opacity=self.start_opacity,
-                      duration=stim.duration,
-                      highlight=stim.symbol,
-                      highlight_color=stim.color)
-        self.draw(self.start_opacity)
-
-    def wait_screen(self, message: str, message_color: str) -> None:
-        """Wait Screen.
-
-        Define what happens on the screen when a user pauses a session.
-        """
-
-        # Construct the wait message
-        wait_message = visual.TextStim(win=self.window,
-                                       font=self.stimuli_font,
-                                       text=message,
-                                       height=.1,
-                                       color=message_color,
-                                       pos=(0, -.5),
-                                       wrapWidth=2)
-
-        # try adding the BciPy logo to the wait screen
-        try:
-            wait_logo = visual.ImageStim(
-                self.window,
-                image=BCIPY_LOGO_PATH,
-                pos=(0, .25),
-                mask=None,
-                ori=0.0)
-            wait_logo.size = resize_image(
-                BCIPY_LOGO_PATH,
-                self.window.size,
-                1)
-            wait_logo.draw()
-
-        except Exception as e:
-            self.logger.exception(f'Cannot load logo image from path=[{BCIPY_LOGO_PATH}]')
-            raise e
-
-        # Draw and flip the screen.
-        wait_message.draw()
-        self.window.flip()
-
-    def draw_static(self) -> None:
-        """Draw static elements in a stimulus."""
-        if self.task_bar:
-            self.task_bar.draw()
-
-        for info in self.info_text:
-            info.draw()
-
-    def update_task_bar(self, text: str = ''):
-        """Update Task.
-
-        Update any task related display items not related to the inquiry. Ex. stimuli count 1/200.
-
-        PARAMETERS:
-
-        text: text for task
-        color_list: list of the colors for each stimuli
-        pos: position of task
-        """
-        if self.task_bar:
-            self.task_bar.update(text)
-
-    def _trigger_pulse(self) -> None:
-        """Trigger Pulse.
-
-        This method uses a calibration trigger to determine any functional
-            offsets needed for operation with this display. By setting the first_stim_time and searching for the
-            same stimuli output to the marker stream, the offsets between these proceses can be reconciled at the
-            beginning of an experiment. If drift is detected in your experiment, more frequent pulses and offset
-            correction may be required.
-        """
-        calibration_time = _calibration_trigger(
-            self.experiment_clock,
-            trigger_type=self.trigger_type,
-            display=self.window)
-
-        # set the first stim time if not present and first_run to False
-        if not self.first_stim_time:
-            self.first_stim_time = calibration_time[-1]
-            self.first_run = False
+from typing import List, Optional, Tuple
+import logging
+
+from psychopy import visual, core
+
+from bcipy.acquisition.marker_writer import NullMarkerWriter, MarkerWriter
+from bcipy.display import Display, StimuliProperties, TaskDisplayProperties, InformationProperties, BCIPY_LOGO_PATH
+from bcipy.helpers.task import SPACE_CHAR
+from bcipy.helpers.stimuli import resize_image
+from bcipy.helpers.triggers import TriggerCallback, _calibration_trigger
+from bcipy.helpers.task import alphabet
+from bcipy.helpers.exceptions import BciPyCoreException
+
+
+class MatrixDisplay(Display):
+    """Matrix Display Object for Inquiry Presentation.
+
+    Animates display objects in matrix grid common to any Matrix task.
+    """
+
+    def __init__(
+            self,
+            window: visual.Window,
+            static_clock,
+            experiment_clock: core.Clock,
+            stimuli: StimuliProperties,
+            task_display: TaskDisplayProperties,
+            info: InformationProperties,
+            marker_writer: Optional[MarkerWriter] = NullMarkerWriter(),
+            trigger_type: str = 'text',
+            space_char: str = SPACE_CHAR,
+            full_screen: bool = False,
+            symbol_set: Optional[List[str]] = None):
+        """Initialize Matrix display parameters and objects.
+
+        PARAMETERS:
+        ----------
+        # Experiment
+        window(visual.Window): PsychoPy Window
+        static_clock(core.Clock): Used to schedule static periods of display time
+        experiment_clock(core.Clock): Clock used to timestamp display onsets
+
+        # Stimuli
+        stimuli(StimuliProperties): attributes used for inquiries
+
+        # Task
+        task_display(TaskDisplayProperties): attributes used for task tracking. Ex. 1/100
+
+        # Info
+        info(InformationProperties): attributes to display informational stimuli alongside task and inquiry stimuli.
+
+        marker_writer(MarkerWriter) Optional: object used to write triggers to an acquisition stream.
+        trigger_type(str) default 'image': defines the calibration trigger type for the display at the beginning of any
+            task. This will be used to reconcile timing differences between acquisition and the display.
+        space_char(str) default SPACE_CHAR: defines the space character to use in the Matrix inquiry.
+        full_screen(bool) default False: Whether or not the window is set to a full screen dimension. Used for
+            scaling display items as needed.
+        symbol_set default = none : subset of stimuli to be highlighted during an inquiry
+        """
+        self.window = window
+        self.window_size = self.window.size  # [w, h]
+        self.refresh_rate = window.getActualFrameRate()
+
+        self.logger = logging.getLogger(__name__)
+
+        # Stimuli parameters, these are set on display in order to allow
+        # easy updating after definition
+        self.stimuli_inquiry = stimuli.stim_inquiry
+        self.stimuli_colors = stimuli.stim_colors
+        self.stimuli_timing = stimuli.stim_timing
+        self.stimuli_font = stimuli.stim_font
+        self.stimuli_height = stimuli.stim_height
+        self.stimuli_pos = stimuli.stim_pos
+        self.is_txt_stim = stimuli.is_txt_stim
+        assert self.is_txt_stim is True, "Matrix display is a text only display"
+        self.stim_length = stimuli.stim_length
+
+        self.prompt_time = stimuli.prompt_time
+
+        self.full_screen = full_screen
+
+        self.symbol_set = symbol_set or alphabet()
+
+        self.staticPeriod = static_clock
+
+        # Set position and parameters for grid of alphabet
+        self.position = stimuli.stim_pos
+        self.grid_stimuli_height = .17
+        self.position_increment = self.grid_stimuli_height + .05
+        self.max_grid_width = 0.7
+        self.stim_registry = {}
+
+        self.start_opacity = 0.15
+        self.highlight_opacity = 0.95
+        self.full_grid_opacity = 0.95
+
+        # Trigger handling
+        self.first_run = True
+        self.first_stim_time = None
+        self.trigger_type = trigger_type
+        self.trigger_callback = TriggerCallback()
+        self.marker_writer = marker_writer or NullMarkerWriter()
+        self.experiment_clock = experiment_clock
+
+        self.buffer_time = 2
+
+        # Callback used on presentation of first stimulus.
+        self.first_stim_callback = lambda _sti: None
+        self.size_list_sti = []
+        self.space_char = space_char
+        self.task_display = task_display
+        self.task = task_display.build_task(self.window)
+
+        self.scp = True  # for future row / col integration
+
+        self.info = info
+        self.info_text = info.build_info_text(window)
+
+        # Create initial stimuli object for updating
+        self.sti = stimuli.build_init_stimuli(window)
+
+    def schedule_to(self, stimuli: list, timing: list, colors: list) -> None:
+        """Schedule stimuli elements (works as a buffer).
+
+        Args:
+                stimuli(list[string]): list of stimuli text / name
+                timing(list[float]): list of timings of stimuli
+                colors(list[string]): list of colors
+        """
+        self.stimuli_inquiry = stimuli
+        self.stimuli_timing = timing
+        self.stimuli_colors = colors
+
+    def do_inquiry(self) -> List[float]:
+        """Do inquiry.
+
+        Animates an inquiry of stimuli and returns a list of stimuli trigger timing.
+        """
+        if self.first_run:
+            self._trigger_pulse()
+
+        if self.scp:
+            timing, target = self.prompt_target()
+            timing.extend(self.animate_scp())
+            return timing, target
+
+        raise BciPyCoreException('Only SCP Matrix is available.')
+
+    def build_grid(self, opacity: Optional[float] = None) -> None:
+        """Build grid.
+
+        Builds and displays a 7x4 matrix of stimuli.
+        """
+        pos = self.position
+        for sym in self.symbol_set:
+            text_stim = visual.TextStim(
+                win=self.window,
+                text=sym,
+                opacity=opacity if opacity is not None else self.start_opacity,
+                pos=pos,
+                height=self.grid_stimuli_height)
+            self.stim_registry[sym] = text_stim
+            self.stim_registry[sym].draw()
+
+            pos = self.increment_position(pos)
+
+    def increment_position(self, pos: Tuple[float]) -> Tuple[float]:
+        x_cordinate, y_cordinate = pos
+        x_cordinate += self.position_increment
+        if x_cordinate >= self.max_grid_width:
+            y_cordinate -= self.position_increment
+            x_cordinate = self.position[0]
+        return (x_cordinate, y_cordinate)
+
+    def prompt_target(self) -> List[float]:
+        timing = []
+
+        # select target which is first in list from the defined stimuli inquiry
+        target = self.stimuli_inquiry[0]
+
+        # cut off first two stimuli in inquiry, the target and fixation
+        self.stimuli_inquiry = self.stimuli_inquiry[2:]
+
+        # register any timing and marker callbacks
+        self.window.callOnFlip(
+            self.trigger_callback.callback,
+            self.experiment_clock,
+            target)
+        self.window.callOnFlip(self.marker_writer.push_marker, target)
+        target_prompt = visual.TextStim(win=self.window,
+                                        font=self.stimuli_font,
+                                        text=f'Target: {target}',
+                                        height=.25,
+                                        color='Green',
+                                        pos=(0, 0),
+                                        wrapWidth=2,
+                                        colorSpace='rgb',
+                                        opacity=1,
+                                        depth=-6.0)
+        target_prompt.draw()
+        self.draw_static()
+        self.window.flip()
+
+        core.wait(self.prompt_time)
+
+        # append timing information
+        timing.append(self.trigger_callback.timing)
+        self.trigger_callback.reset()
+
+        return timing, target
+
+    def animate_scp(self) -> List[float]:
+        """Animate SCP.
+
+        Flashes each stimuli in stimuli_inquiry for their respective flash
+        times.
+        """
+        timing = []
+        # build grid and static
+        self.build_grid(opacity=self.full_grid_opacity)
+        self.draw_static()
+        self.window.flip()
+        core.wait(self.buffer_time)
+
+        self.build_grid()
+        self.draw_static()
+        self.window.flip()
+        core.wait(self.buffer_time)
+
+        for i, sym in enumerate(self.stimuli_inquiry):
+
+            # register any timing and marker callbacks
+            self.window.callOnFlip(
+                self.trigger_callback.callback,
+                self.experiment_clock,
+                sym)
+            self.window.callOnFlip(self.marker_writer.push_marker, sym)
+
+            # build grid and static
+            self.build_grid()
+            self.draw_static()
+
+            # highlight a stimuli
+            self.stim_registry[sym].setOpacity(self.highlight_opacity)
+            self.stim_registry[sym].draw()
+            # present stimuli and wait for self.stimuli_timing
+
+            self.window.flip()
+            core.wait(self.stimuli_timing[i])
+
+            # reset the highlighted symbol and continue
+            self.stim_registry[sym].setOpacity(self.start_opacity)
+            self.stim_registry[sym].draw()
+
+            # append timing information
+            timing.append(self.trigger_callback.timing)
+            self.trigger_callback.reset()
+
+        self.build_grid()
+        self.draw_static()
+        self.window.flip()
+
+        return timing
+
+    def wait_screen(self, message: str, message_color: str) -> None:
+        """Wait Screen.
+
+        Define what happens on the screen when a user pauses a session.
+        """
+
+        # Construct the wait message
+        wait_message = visual.TextStim(win=self.window,
+                                       font=self.stimuli_font,
+                                       text=message,
+                                       height=.1,
+                                       color=message_color,
+                                       pos=(0, -.5),
+                                       wrapWidth=2,
+                                       colorSpace='rgb',
+                                       opacity=1,
+                                       depth=-6.0)
+
+        # try adding the BciPy logo to the wait screen
+        try:
+            wait_logo = visual.ImageStim(
+                self.window,
+                image=BCIPY_LOGO_PATH,
+                pos=(0, .25),
+                mask=None,
+                ori=0.0)
+            wait_logo.size = resize_image(
+                BCIPY_LOGO_PATH,
+                self.window.size,
+                1)
+            wait_logo.draw()
+
+        except Exception as e:
+            self.logger.exception(f'Cannot load logo image from path=[{BCIPY_LOGO_PATH}]')
+            raise e
+
+        # Draw and flip the screen.
+        wait_message.draw()
+        self.window.flip()
+
+    def draw_static(self) -> None:
+        """Draw static elements in a stimulus."""
+        self.task.draw()
+
+        for info in self.info_text:
+            info.draw()
+
+    def update_task(self, text: str, color_list: List[str], pos: Tuple[float, float]) -> None:
+        """Update Task.
+
+        Update any task related display items not related to the inquiry. Ex. stimuli count 1/200.
+
+        PARAMETERS:
+
+        text: text for task
+        color_list: list of the colors for each stimuli
+        pos: position of task
+        """
+        self.task.text = text
+        self.task.color = color_list[0]
+        self.task.pos = pos
+
+    def update_task_state(self, text: str, color_list: List[str]) -> None:
+        """Update task state.
+
+        Removes letters or appends to the right.
+        Args:
+                text(string): new text for task state
+                color_list(list[string]): list of colors for each stimuli
+        """
+        self.update_task(text=text, color_list=color_list, pos=self.task.pos)
+
+    def _trigger_pulse(self) -> None:
+        """Trigger Pulse.
+
+        This method uses a calibration trigger to determine any functional
+            offsets needed for operation with this display. By setting the first_stim_time and searching for the
+            same stimuli output to the marker stream, the offsets between these proceses can be reconciled at the
+            beginning of an experiment. If drift is detected in your experiment, more frequent pulses and offset
+            correction may be required.
+        """
+        calibration_time = _calibration_trigger(
+            self.experiment_clock,
+            trigger_type=self.trigger_type,
+            display=self.window)
+
+        # set the first stim time if not present and first_run to False
+        if not self.first_stim_time:
+            self.first_stim_time = calibration_time[-1]
+            self.first_run = False
```

### Comparing `bcipy-2.0.0rc3/bcipy/display/paradigm/rsvp/display.py` & `bcipy-2.0.1rc2/bcipy/display/paradigm/rsvp/display.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import logging
 import os.path as path
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 from psychopy import core, visual, event
 
 from bcipy.helpers.clock import Clock
-from bcipy.helpers.task import get_key_press
-from bcipy.helpers.symbols import SPACE_CHAR
+from bcipy.helpers.task import SPACE_CHAR, get_key_press
 from bcipy.display import (
     BCIPY_LOGO_PATH,
     Display,
     InformationProperties,
     PreviewInquiryProperties,
-    StimuliProperties
+    StimuliProperties,
+    TaskDisplayProperties,
 )
-from bcipy.display.components.task_bar import TaskBar
 from bcipy.helpers.stimuli import resize_image
-from bcipy.helpers.system_utils import get_screen_info
+from bcipy.helpers.system_utils import get_screen_resolution
 from bcipy.helpers.triggers import TriggerCallback, _calibration_trigger
 
 
 class RSVPDisplay(Display):
     """RSVP Display Object for inquiry Presentation.
 
     Animates display objects common to any RSVP task.
@@ -28,15 +27,15 @@
 
     def __init__(
             self,
             window: visual.Window,
             static_clock,
             experiment_clock: Clock,
             stimuli: StimuliProperties,
-            task_bar: TaskBar,
+            task_display: TaskDisplayProperties,
             info: InformationProperties,
             preview_inquiry: PreviewInquiryProperties = None,
             trigger_type: str = 'image',
             space_char: str = SPACE_CHAR,
             full_screen: bool = False):
         """Initialize RSVP display parameters and objects.
 
@@ -47,15 +46,15 @@
         static_clock(core.MonotonicClock): Used to schedule static periods of display time
         experiment_clock(Clock): Clock used to timestamp display onsets
 
         # Stimuli
         stimuli(StimuliProperties): attributes used for inquiries
 
         # Task
-        task_bar(TaskBar): used for task tracking. Ex. 1/100
+        task_display(TaskDisplayProperties): attributes used for task tracking. Ex. 1/100
 
         # Info
         info(InformationProperties): attributes to display informational stimuli alongside task and inquiry stimuli.
 
         # Preview Inquiry
         preview_inquiry(PreviewInquiryProperties) Optional: attributes to display a preview of upcoming stimuli defined
             via self.stimuli(StimuliProperties).
@@ -69,15 +68,15 @@
         self.window = window
         self.window_size = self.window.size  # [w, h]
         self.refresh_rate = window.getActualFrameRate()
 
         self.logger = logging.getLogger(__name__)
 
         # Stimuli parameters, these are set on display in order to allow
-        #  easy updating after definition
+        #  easy updating after defintion
         self.stimuli_inquiry = stimuli.stim_inquiry
         self.stimuli_colors = stimuli.stim_colors
         self.stimuli_timing = stimuli.stim_timing
         self.stimuli_font = stimuli.stim_font
         self.stimuli_height = stimuli.stim_height
         self.stimuli_pos = stimuli.stim_pos
         self.is_txt_stim = stimuli.is_txt_stim
@@ -95,99 +94,94 @@
         self.trigger_callback = TriggerCallback()
         self.experiment_clock = experiment_clock
 
         # Callback used on presentation of first stimulus.
         self.first_stim_callback = lambda _sti: None
         self.size_list_sti = []  # TODO force initial size definition
         self.space_char = space_char  # TODO remove and force task to define
-
-        self.task_bar = task_bar
+        self.task_display = task_display
+        self.task = task_display.build_task(self.window)
 
         # Create multiple text objects based on input
         self.info = info
         self.info_text = info.build_info_text(window)
 
         # Create initial stimuli object for updating
         self.sti = stimuli.build_init_stimuli(window)
 
     def draw_static(self):
         """Draw static elements in a stimulus."""
-        if self.task_bar:
-            self.task_bar.draw()
+        self.task.draw()
         for info in self.info_text:
             info.draw()
 
-    def schedule_to(self,
-                    stimuli: List[str] = None,
-                    timing: List[float] = None,
-                    colors: List[str] = None):
+    def schedule_to(self, stimuli=[], timing=[], colors=[]):
         """Schedule stimuli elements (works as a buffer).
 
         Args:
                 stimuli(list[string]): list of stimuli text / name
                 timing(list[float]): list of timings of stimuli
                 colors(list[string]): list of colors
         """
-        self.stimuli_inquiry = stimuli or []
-        self.stimuli_timing = timing or []
-        self.stimuli_colors = colors or []
-
-    def do_inquiry(self, preview_calibration: bool = False) -> List[float]:
-        """Do inquiry.
-
-        Animates an inquiry of flashing letters to achieve RSVP.
+        self.stimuli_inquiry = stimuli
+        self.stimuli_timing = timing
+        self.stimuli_colors = colors
 
+    def update_task(self, text: str, color_list: List[str], pos: Optional[Tuple] = None) -> None:
+        """Update Task Object.
 
         PARAMETERS:
         -----------
-        preview_calibration(bool) default False: Whether or not to preview the upcoming inquiry stimuli. This feature
-            is used to help the participant prepare for the upcoming inquiry after a prompt. It will present after
-            the first stimulus of the inquiry (assumed to be a prompt). Not recommended for use outside of a
-            calibration task.
-
-        RETURNS:
-        --------
-        timing(list[float]): list of timings of stimuli presented in the inquiry
+        text: text for task
+        color_list: list of the colors for each char
+        """
+        self.task.text = text
+        self.task.color = color_list[0]
+        if pos:
+            self.task.pos = pos
+
+    def do_inquiry(self) -> List[float]:
+        """Do inquiry.
+
+        Animates an inquiry of flashing letters to achieve RSVP.
         """
 
         # init an array for timing information
         timing = []
 
         if self.first_run:
             self._trigger_pulse()
 
         # generate a inquiry (list of stimuli with meta information)
         inquiry = self._generate_inquiry()
 
         # do the inquiry
         for idx in range(len(inquiry)):
 
-            # If this is the start of an inquiry and a callback registered for first_stim_callback evoke it
-            if idx == 0 and callable(self.first_stim_callback):
-                self.first_stim_callback(inquiry[idx]['sti'])
-
-            # If previewing the inquiry, do so after the first stimulus
-            if preview_calibration and idx == 1:
-                time, _ = self.preview_inquiry()
-                timing.extend(time)
-
             # Reset the timing clock to start presenting
             self.window.callOnFlip(
                 self.trigger_callback.callback,
                 self.experiment_clock,
                 inquiry[idx]['sti_label'])
 
+            # If this is the start of an inquiry and a callback registered for first_stim_callback evoke it
+            if idx == 0 and callable(self.first_stim_callback):
+                self.first_stim_callback(inquiry[idx]['sti'])
+
             # Draw stimulus for n frames
             inquiry[idx]['sti'].draw()
             self.draw_static()
             self.window.flip()
             core.wait(inquiry[idx]['time_to_present'])
 
             # append timing information
-            timing.append(self.trigger_callback.timing)
+            if self.is_txt_stim:
+                timing.append(self.trigger_callback.timing)
+            else:
+                timing.append(self.trigger_callback.timing)
 
             self.trigger_callback.reset()
 
         # draw in static and flip once more
         self.draw_static()
         self.window.flip()
 
@@ -283,24 +277,29 @@
 
     def _generate_inquiry_preview(self) -> visual.TextBox2:
         """Generate Inquiry Preview.
 
         Using the self.stimuli_inquiry list, construct a preview box to display to the user. This method
             assumes the presence of a fixation (+).
         """
+        if not self.full_screen:
+            reduce_factor = 4.85
+            wrap_width = 1.1
+        else:
+            reduce_factor = 4.75
+            wrap_width = .9
         text = ' '.join(self.stimuli_inquiry).split('+ ')[1]
 
         return self._create_stimulus(
-            0.12,
+            self.stimuli_height / reduce_factor,
             stimulus=text,
             units='height',
             stimuli_position=self.stimuli_pos,
             mode='textbox',
-            align_text='left',
-            wrap_width=0.025)
+            wrap_width=wrap_width)
 
     def _generate_inquiry(self) -> list:
         """Generate inquiry.
 
         Generate stimuli for next RSVP inquiry. [A + A, C, Q, D]
         """
         stim_info = []
@@ -334,17 +333,15 @@
                 current_stim['sti'].text = txt if txt != SPACE_CHAR else self.space_char
                 current_stim['sti'].color = self.stimuli_colors[idx]
                 current_stim['sti_label'] = txt
 
                 # test whether the word will be too big for the screen
                 text_width = current_stim['sti'].boundingBox[0]
                 if text_width > self.window.size[0]:
-                    screen_info = get_screen_info()
-                    monitor_width = screen_info.width
-                    monitor_height = screen_info.height
+                    monitor_width, monitor_height = get_screen_resolution()
                     text_height = current_stim['sti'].boundingBox[1]
                     # If we are in full-screen, text size in Psychopy norm units
                     # is monitor width/monitor height
                     if self.window.size[0] == monitor_width:
                         new_text_width = monitor_width / monitor_height
                     else:
                         # If not, text width is calculated relative to both
@@ -353,23 +350,24 @@
                             self.window.size[1] / monitor_height) * (
                                 monitor_width / monitor_height)
                     new_text_height = (text_height * new_text_width) / text_width
                     current_stim['sti'].height = new_text_height
             stim_info.append(current_stim)
         return stim_info
 
-    def update_task_bar(self, text: str = None) -> None:
+    def update_task_state(self, text: str, color_list: List[str], pos: Optional[Tuple] = None) -> None:
         """Update task state.
 
         Removes letters or appends to the right.
         Args:
                 text(string): new text for task state
+                color_list(list[string]): list of colors for each
+                pos(tuple): [optional] tuple of task position
         """
-        if self.task_bar:
-            self.task_bar.update(text)
+        self.update_task(text=text, color_list=color_list, pos=pos)
 
     def wait_screen(self, message: str, message_color: str) -> None:
         """Wait Screen.
 
         Args:
             message(string): message to be displayed while waiting
             message_color(string): color of the message to be displayed
@@ -418,15 +416,15 @@
             stimuli_position=None,
             align_text='center',
             units=None,
             wrap_width=None,
             border=False):
         """Create Stimulus.
 
-        Returns a TextStim, ImageStim or TextBox object.
+        Returns a TextStim or ImageStim object.
         """
         if not stimuli_position:
             stimuli_position = self.stimuli_pos
         if mode == 'text':
             return visual.TextStim(
                 win=self.window,
                 color=color,
@@ -458,9 +456,10 @@
                 borderWidth=2,
                 borderColor='white',
                 units=units,
                 font=self.stimuli_font,
                 letterHeight=height,
                 size=[.5, .5],
                 pos=stimuli_position,
+                anchor=align_text,
                 alignment=align_text,
             )
```

### Comparing `bcipy-2.0.0rc3/bcipy/display/paradigm/vep/display.py` & `bcipy-2.0.1rc2/bcipy/display/paradigm/vep/display.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,494 +1,494 @@
-import logging
-from typing import List, Tuple, Optional
-from bcipy.display import (
-    BCIPY_LOGO_PATH,
-    Display,
-    InformationProperties,
-    VEPStimuliProperties,
-    TaskDisplayProperties,
-)
-import numpy as np
-from psychopy import visual, core
-from bcipy.helpers.clock import Clock
-from bcipy.helpers.symbols import SPACE_CHAR
-from bcipy.helpers.triggers import TriggerCallback, _calibration_trigger
-from bcipy.helpers.stimuli import resize_image, get_fixation
-
-
-def create_vep_codes(length=32, count=4) -> List[List[int]]:
-    """Create a list of random VEP codes.
-
-    length - how many bits in each code. This should be greater than or equal to the refresh rate
-        if using these to flicker. For example, if the refresh rate is 60Hz, then the length should
-        be at least 60.
-    count - how many codes to generate, each will be unique.
-    """
-    np.random.seed(1)
-    return [np.random.randint(2, size=length) for _ in range(count)]
-
-
-class VEPBox:
-    """A class to represent a VEP box.
-
-    Attributes:
-        flicker: A list of two visual.GratingStim objects, one for on and one for off.
-        code: A list of integers representing the VEP code for this box.
-    """
-
-    def __init__(self, flicker: List[Tuple[visual.GratingStim, visual.GratingStim]], code: List[int]) -> None:
-        self.flicker = flicker
-        self.code = code
-
-    def frame_on(self) -> None:
-        """Frame On. Draw the frame for the first grating stim on the screen."""
-        self.flicker[0].draw()
-
-    def frame_off(self) -> None:
-        """Frame Off. Draw the frame for the second grating stim on the screen."""
-        self.flicker[1].draw()
-
-
-class VEPDisplay(Display):
-
-    def __init__(
-            self,
-            window: visual.Window,
-            experiment_clock: Clock,
-            stimuli: VEPStimuliProperties,
-            task_display: TaskDisplayProperties,
-            info: InformationProperties,
-            trigger_type: str = 'text',
-            space_char: str = SPACE_CHAR,
-            full_screen: bool = False,
-            codes: List[int] = None):
-        self.window = window
-        self.window_size = self.window.size  # [w, h]
-        self.refresh_rate = round(window.getActualFrameRate())
-
-        self.logger = logging.getLogger(__name__)
-
-        # Stimuli parameters, these are set on display in order to allow
-        #  easy updating after defintion
-        self.stimuli_inquiry = stimuli.stim_inquiry
-        self.stimuli_colors = stimuli.stim_colors
-        self.stimuli_timing = stimuli.stim_timing
-        self.stimuli_font = stimuli.stim_font
-        self.stimuli_height = stimuli.stim_height
-        self.stimuli_pos = stimuli.stim_pos
-        self.logger.info(self.stimuli_pos)
-        self.is_txt_stim = stimuli.is_txt_stim
-        self.stim_length = stimuli.stim_length
-        self.sti = []
-        self.fixation = visual.TextStim(
-            self.window,
-            text=get_fixation(True),
-            color='red',
-            height=self.stimuli_height,
-            units='height',
-            pos=[0, 0])
-
-        self.full_screen = full_screen
-
-        self.static_clock = core.Clock()
-
-        # Trigger handling
-        self.first_stim_time = None
-        self.trigger_type = trigger_type
-        self.trigger_callback = TriggerCallback()
-        self.experiment_clock = experiment_clock
-
-        # Callback used on presentation of first stimulus.
-        self.first_run = True
-        self.first_stim_callback = lambda _sti: None
-        self.size_list_sti = []
-
-        # Task parameters
-        self.space_char = space_char
-        self.task_display = task_display
-        self.task = task_display.build_task(self.window)
-
-        # Information parameters
-        self.info = info
-        self.info_text = info.build_info_text(window)
-
-        self.colors = [('white', 'black'), ('red', 'green'), ('blue', 'yellow'), ('orange', 'green')]
-        if not codes:
-            self.codes = create_vep_codes(length=self.refresh_rate, count=4)
-        else:
-            self.codes = codes
-
-        # build the VEP stimuli
-        self.vep = []
-        self.text_boxes = []
-        self.vep_type = 4
-        assert self.vep_type == 4, 'Only 4 stimuli are supported in VEP display at this time!'
-        self.vep_box_size = .1
-
-        self.animation_duration = 2
-
-    def do_fixation(self) -> None:
-        # draw fixation cross
-        self.fixation.draw()
-        self.draw_static()
-        self.window.flip()
-        core.wait(self.stimuli_timing[1])
-
-    def do_inquiry(self) -> List[float]:
-        """Do the inquiry."""
-
-        timing = []
-
-        # if this is the first run, calibrate using the trigger pulse and setup the VEP and text boxes
-        if self.first_run:
-            self._trigger_pulse()
-            self._build_vep_corner_stimuli(self.stimuli_pos, self.codes, self.colors, self.vep_box_size)
-            self._build_text_boxes()
-
-        # fixation --> animation / prompting --> VEP stimulate
-        self.do_fixation()
-        timing += self.animate_inquiry()
-        timing += self.stimulate()
-
-        # clear everyting expect static stimuli
-        self.draw_static()
-        self.window.flip()
-
-        return timing
-
-    def animate_inquiry(self) -> List[float]:
-        """Display the inquiry.
-
-        Inquiry is a list of lists of strings.
-        Each list contains what stimuli to display for each box defined in self.vep.
-        """
-        timing = []
-        self.trigger_callback.reset()
-        self.window.callOnFlip(
-            self.trigger_callback.callback,
-            self.experiment_clock,
-            'VEP_INQ_ANIMATION')
-
-        self._reset_text_boxes()
-        self._build_inquiry_stimuli()
-
-        self.static_clock.reset()
-        while self.static_clock.getTime() < self.animation_duration:
-            self.draw_boxes()
-            self.draw_animation()
-            self.draw_static()
-            self.window.flip()
-        timing += self.trigger_callback.timing
-
-        self._set_inquiry()
-        self.trigger_callback.reset()
-        self.window.callOnFlip(
-            self.trigger_callback.callback,
-            self.experiment_clock,
-            'VEP_INQUIRY')
-        # display the inquiry
-        self.static_clock.reset()
-        while self.static_clock.getTime() < self.stimuli_timing[0]:
-            self.draw_boxes()
-            self.draw_static()
-            self.window.flip()
-
-        timing += self.trigger_callback.timing
-
-        return timing
-
-    def draw_animation(self) -> None:
-        """Draw the stimuli animation."""
-        for sti in self.sti:
-            sti.draw()
-
-    def draw_boxes(self) -> None:
-        """Draw the text boxes under VEP stimuli."""
-        for box in self.text_boxes:
-            box.draw()
-
-    def stimulate(self) -> List[float]:
-        """Stimulate.
-
-        This is the main display function of the VEP paradigm. It is responsible for drawing the flickering stimuli.
-
-        It assumes that the VEP stimuli are already constructed using the _build_vep_corner_stimuli function.
-        These boxes are drawn in the order they are in the list as defined in self.vep."""
-        self.trigger_callback.reset()
-        self.window.callOnFlip(
-            self.trigger_callback.callback,
-            self.experiment_clock,
-            'VEP_STIMULATE')
-        self.static_clock.reset()
-        while self.static_clock.getTime() < self.stimuli_timing[-1]:
-            for frame in range(self.refresh_rate):
-                for box in self.vep:
-                    if box.code[frame] == 1:
-                        box.frame_on()
-                    else:
-                        box.frame_off()
-
-                # flicker!
-                self.draw_static()
-                self.window.flip()
-
-        return self.trigger_callback.timing
-
-    def draw_static(self) -> None:
-        """Draw static elements for the display."""
-        self.task.draw()
-        for info in self.info_text:
-            info.draw()
-
-    def update_task(self, text: str, color: str, pos: Optional[Tuple] = None) -> None:
-        """Update the task display which is displayed using the draw_static function."""
-        self.task.text = text
-        self.task.color = color
-        if pos:
-            self.task.pos = pos
-
-    def _build_inquiry_stimuli(self) -> None:
-        """Build the inquiry stimuli."""
-        all_letters = []
-        all_colors = []
-        self.sti = []
-        for letters, colors in zip(self.stimuli_inquiry, self.stimuli_colors):
-            for letter in letters:
-                all_letters.append(letter)
-                all_colors.append(colors[0])
-        pos = (0, 0)
-        for letter, color in zip(all_letters, all_colors):
-            pos = (pos[0] + self.stimuli_height, pos[1])
-            self.sti.append(
-                visual.TextStim(self.window, text=letter, color=color, pos=pos, height=self.stimuli_height))
-
-        return self.sti
-
-    def _build_vep_corner_stimuli(
-            self,
-            pos: Tuple[float, float],
-            codes: List[int],
-            colors: List[Tuple[str]],
-            box_size: float) -> List[visual.GratingStim]:
-        """Build the corner stimuli for the VEP.
-
-        Args:
-            window: psychopy window object
-        """
-        corner_stim = []
-        for pos, code, color in zip(pos, codes, colors):
-            corner_stim += self._build_2x2_vep_grid(pos, box_size, color, code)
-
-        return corner_stim
-
-    def _build_1x1_vep_grid(
-            self,
-            position: Tuple[float],
-            size: float,
-            color: str,
-            code: List[int]) -> List[visual.GratingStim]:
-        """Build a 1x1 VEP grid.
-
-        Args:
-            position: position of the flicking box
-            size: size of the flicking box
-            color: color of the flicking box
-            code: code to be used with the flicking box
-
-        Returns:
-            list of visual.GratingStim objects
-
-        """
-        assert len(code) >= self.refresh_rate, 'Code must be longer than refresh rate'
-        pattern1 = visual.GratingStim(win=self.window, name=f'1x1-1-{position}', units='height',
-                                      tex=None, mask=None,
-                                      ori=0, pos=position, size=size, sf=1, phase=0.0,
-                                      color=color[0], colorSpace='rgb', opacity=1,
-                                      texRes=256, interpolate=True, depth=-1.0)
-        pattern2 = visual.GratingStim(win=self.window, name=f'1x1-2-{position}', units='height',
-                                      tex=None, mask=None,
-                                      ori=0, pos=position, size=size, sf=1, phase=0,
-                                      color=color[1], colorSpace='rgb', opacity=1,
-                                      texRes=256, interpolate=True, depth=-2.0)
-        box = [VEPBox(flicker=[pattern1, pattern2], code=code)]
-        self.vep += box
-        return box
-
-    def _build_2x2_vep_grid(self,
-                            position: Tuple[float],
-                            size: float,
-                            color: str,
-                            code: List[int]) -> List[visual.GratingStim]:
-        """Build a 2x2 VEP grid.
-
-        Args:
-            position: position of the flicking box
-            size: size of the flicking box
-            color: color of the flicking box
-            code: code to be used with the flicking box
-
-        Returns:
-            list of visual.GratingStim objects
-        """
-
-        assert len(code) >= self.refresh_rate, 'Code must be longer than refresh rate'
-        starting_position = position
-        positions = [
-            starting_position,  # bottom left
-            [starting_position[0] + size, starting_position[1]],  # bottom right
-            [starting_position[0] + size, starting_position[1] + size],  # top right
-            [starting_position[0], starting_position[1] + size],  # top left
-        ]
-        box = []
-        for pos in positions:
-            pattern1 = visual.GratingStim(win=self.window, name=f'2x2-1-{pos}', units='height',
-                                          tex=None, mask=None,
-                                          ori=0, pos=pos, size=size, sf=1, phase=0.0,
-                                          color=color[0], colorSpace='rgb', opacity=1,
-                                          texRes=256, interpolate=True, depth=-1.0)
-            pattern2 = visual.GratingStim(win=self.window, name=f'2x2-2-{pos}', units='height',
-                                          tex=None, mask=None,
-                                          ori=0, pos=pos, size=size, sf=1, phase=0,
-                                          color=color[1], colorSpace='rgb', opacity=1,
-                                          texRes=256, interpolate=True, depth=-2.0)
-            color = (color[1], color[0])
-            box += [VEPBox(flicker=[pattern1, pattern2], code=code)]
-
-        self.vep += box
-        return box
-
-    def _trigger_pulse(self) -> None:
-        """Trigger Pulse.
-
-        This method uses a calibration trigger to determine any functional
-            offsets needed for operation with this display. By setting the first_stim_time and searching for the
-            same stimuli output to the marker stream, the offsets between these proceses can be reconciled at the
-            beginning of an experiment. If drift is detected in your experiment, more frequent pulses and offset
-            correction may be required.
-        """
-        calibration_time = _calibration_trigger(
-            self.experiment_clock,
-            trigger_type=self.trigger_type,
-            display=self.window)
-
-        # set the first stim time if not present and first_run to False
-        if not self.first_stim_time:
-            self.first_stim_time = calibration_time[-1]
-            self.first_run = False
-
-    def schedule_to(self, stimuli: List[List[str]], timing: List[List[float]], colors: List[List[str]]) -> None:
-        """Schedule stimuli elements (works as a buffer).
-        """
-        self.stimuli_inquiry = stimuli
-        self.stimuli_timing = timing
-        self.stimuli_colors = colors
-
-    def _build_text_boxes(self) -> List[visual.TextBox2]:
-        """Build the text boxes for the experiment.
-
-        This assumes that vep_type is 4 using a 2x2 grid. Additional configurations can be added in the future.
-        """
-        # generate the inquiry stimuli
-        assert len(
-            self.stimuli_colors) == self.vep_type, (
-                f"stmuli colors {len(self.stimuli_colors)} must be the same length as vep type {self.vep_type}")
-        assert len(
-            self.stimuli_pos) == self.vep_type, (
-                f"stmuli position {len(self.stimuli_pos)} must be the same length as vep type {self.vep_type}")
-
-        self.text_boxes = []
-        inc_q = int(self.vep_type / 2)
-        size = self.vep_box_size * inc_q
-        inc = 0  # get the last box in the grating stim per vep
-        for color in self.stimuli_colors:
-            text = ' '
-            first = self.vep[inc].flicker[0].pos
-            best_neighbor = self.vep[inc + inc_q].flicker[0].pos
-
-            # the textbox requires the pos to be centered on the middle of the box, so
-            # we need to calculate the center of the vep stimulus boxes
-            pos = (first[0] + best_neighbor[0]) / 2, (first[1] + best_neighbor[1]) / 2
-            self.text_boxes += [visual.TextBox2(
-                win=self.window,
-                text=text,
-                font=self.stimuli_font,
-                units='height',
-                pos=pos,
-                color=color[0],
-                colorSpace='rgb',
-                size=[size, size],
-                alignment='center',
-                anchor='center',
-                borderWidth=2,
-                borderColor='white',
-                letterHeight=self.stimuli_height / 2)]
-            inc += self.vep_type
-        return self.text_boxes
-
-    def _reset_text_boxes(self) -> None:
-        """Reset text boxes.
-
-        This method resets the text boxes to the blank state.
-        """
-        for text_box in self.text_boxes:
-            text_box.setText(' ')
-
-    def _set_inquiry(self) -> List[visual.TextBox2]:
-        """Generate Inquiry.
-
-        This method sets the correct inquiry text for each text boxes.
-        """
-        # generate the inquiry stimuli
-        assert len(
-            self.stimuli_inquiry) == self.vep_type, (
-                f"stmuli inquiry {len(self.stimuli_inquiry)} must be the same length as vep type {self.vep_type}")
-        assert len(
-            self.stimuli_colors) == self.vep_type, (
-                f"stmuli colors {len(self.stimuli_colors)} must be the same length as vep type {self.vep_type}")
-        for box_content, color, box in zip(self.stimuli_inquiry, self.stimuli_colors, self.text_boxes):
-            text = ' '.join(box_content)
-            box.text = text
-            box.color = color[0]
-        return self.text_boxes
-
-    def wait_screen(self, message: str, color: str) -> None:
-        """Wait Screen.
-
-        Args:
-            message(string): message to be displayed while waiting
-            color(string): color of the message to be displayed
-        """
-
-        # Construct the wait message
-        wait_message = visual.TextStim(win=self.window,
-                                       font=self.stimuli_font,
-                                       text=message,
-                                       height=.1,
-                                       color=color,
-                                       pos=(0, -.5),
-                                       wrapWidth=2,
-                                       colorSpace='rgb',
-                                       opacity=1,
-                                       depth=-6.0)
-
-        # try adding the BciPy logo to the wait screen
-        try:
-            wait_logo = visual.ImageStim(
-                self.window,
-                image=BCIPY_LOGO_PATH,
-                pos=(0, .25),
-                mask=None,
-                ori=0.0)
-            wait_logo.size = resize_image(
-                BCIPY_LOGO_PATH,
-                self.window.size,
-                1)
-            wait_logo.draw()
-
-        except Exception as e:
-            self.logger.exception(f'Cannot load logo image from path=[{BCIPY_LOGO_PATH}]')
-            raise e
-
-        # Draw and flip the screen.
-        wait_message.draw()
-        self.draw_static()
-        self.window.flip()
+import logging
+from typing import List, Tuple, Optional
+from bcipy.display import (
+    BCIPY_LOGO_PATH,
+    Display,
+    InformationProperties,
+    VEPStimuliProperties,
+    TaskDisplayProperties,
+)
+import numpy as np
+from psychopy import visual, core
+from bcipy.helpers.clock import Clock
+from bcipy.helpers.task import SPACE_CHAR
+from bcipy.helpers.triggers import TriggerCallback, _calibration_trigger
+from bcipy.helpers.stimuli import resize_image, get_fixation
+
+
+def create_vep_codes(length=32, count=4) -> List[List[int]]:
+    """Create a list of random VEP codes.
+
+    length - how many bits in each code. This should be greater than or equal to the refresh rate
+        if using these to flicker. For example, if the refresh rate is 60Hz, then the length should
+        be at least 60.
+    count - how many codes to generate, each will be unique.
+    """
+    np.random.seed(1)
+    return [np.random.randint(2, size=length) for _ in range(count)]
+
+
+class VEPBox:
+    """A class to represent a VEP box.
+
+    Attributes:
+        flicker: A list of two visual.GratingStim objects, one for on and one for off.
+        code: A list of integers representing the VEP code for this box.
+    """
+
+    def __init__(self, flicker: List[Tuple[visual.GratingStim, visual.GratingStim]], code: List[int]) -> None:
+        self.flicker = flicker
+        self.code = code
+
+    def frame_on(self) -> None:
+        """Frame On. Draw the frame for the first grating stim on the screen."""
+        self.flicker[0].draw()
+
+    def frame_off(self) -> None:
+        """Frame Off. Draw the frame for the second grating stim on the screen."""
+        self.flicker[1].draw()
+
+
+class VEPDisplay(Display):
+
+    def __init__(
+            self,
+            window: visual.Window,
+            experiment_clock: Clock,
+            stimuli: VEPStimuliProperties,
+            task_display: TaskDisplayProperties,
+            info: InformationProperties,
+            trigger_type: str = 'text',
+            space_char: str = SPACE_CHAR,
+            full_screen: bool = False,
+            codes: List[int] = None):
+        self.window = window
+        self.window_size = self.window.size  # [w, h]
+        self.refresh_rate = round(window.getActualFrameRate())
+
+        self.logger = logging.getLogger(__name__)
+
+        # Stimuli parameters, these are set on display in order to allow
+        #  easy updating after defintion
+        self.stimuli_inquiry = stimuli.stim_inquiry
+        self.stimuli_colors = stimuli.stim_colors
+        self.stimuli_timing = stimuli.stim_timing
+        self.stimuli_font = stimuli.stim_font
+        self.stimuli_height = stimuli.stim_height
+        self.stimuli_pos = stimuli.stim_pos
+        self.logger.info(self.stimuli_pos)
+        self.is_txt_stim = stimuli.is_txt_stim
+        self.stim_length = stimuli.stim_length
+        self.sti = []
+        self.fixation = visual.TextStim(
+            self.window,
+            text=get_fixation(True),
+            color='red',
+            height=self.stimuli_height,
+            units='height',
+            pos=[0, 0])
+
+        self.full_screen = full_screen
+
+        self.static_clock = core.Clock()
+
+        # Trigger handling
+        self.first_stim_time = None
+        self.trigger_type = trigger_type
+        self.trigger_callback = TriggerCallback()
+        self.experiment_clock = experiment_clock
+
+        # Callback used on presentation of first stimulus.
+        self.first_run = True
+        self.first_stim_callback = lambda _sti: None
+        self.size_list_sti = []
+
+        # Task parameters
+        self.space_char = space_char
+        self.task_display = task_display
+        self.task = task_display.build_task(self.window)
+
+        # Information parameters
+        self.info = info
+        self.info_text = info.build_info_text(window)
+
+        self.colors = [('white', 'black'), ('red', 'green'), ('blue', 'yellow'), ('orange', 'green')]
+        if not codes:
+            self.codes = create_vep_codes(length=self.refresh_rate, count=4)
+        else:
+            self.codes = codes
+
+        # build the VEP stimuli
+        self.vep = []
+        self.text_boxes = []
+        self.vep_type = 4
+        assert self.vep_type == 4, 'Only 4 stimuli are supported in VEP display at this time!'
+        self.vep_box_size = .1
+
+        self.animation_duration = 2
+
+    def do_fixation(self) -> None:
+        # draw fixation cross
+        self.fixation.draw()
+        self.draw_static()
+        self.window.flip()
+        core.wait(self.stimuli_timing[1])
+
+    def do_inquiry(self) -> List[float]:
+        """Do the inquiry."""
+
+        timing = []
+
+        # if this is the first run, calibrate using the trigger pulse and setup the VEP and text boxes
+        if self.first_run:
+            self._trigger_pulse()
+            self._build_vep_corner_stimuli(self.stimuli_pos, self.codes, self.colors, self.vep_box_size)
+            self._build_text_boxes()
+
+        # fixation --> animation / prompting --> VEP stimulate
+        self.do_fixation()
+        timing += self.animate_inquiry()
+        timing += self.stimulate()
+
+        # clear everyting expect static stimuli
+        self.draw_static()
+        self.window.flip()
+
+        return timing
+
+    def animate_inquiry(self) -> List[float]:
+        """Display the inquiry.
+
+        Inquiry is a list of lists of strings.
+        Each list contains what stimuli to display for each box defined in self.vep.
+        """
+        timing = []
+        self.trigger_callback.reset()
+        self.window.callOnFlip(
+            self.trigger_callback.callback,
+            self.experiment_clock,
+            'VEP_INQ_ANIMATION')
+
+        self._reset_text_boxes()
+        self._build_inquiry_stimuli()
+
+        self.static_clock.reset()
+        while self.static_clock.getTime() < self.animation_duration:
+            self.draw_boxes()
+            self.draw_animation()
+            self.draw_static()
+            self.window.flip()
+        timing += self.trigger_callback.timing
+
+        self._set_inquiry()
+        self.trigger_callback.reset()
+        self.window.callOnFlip(
+            self.trigger_callback.callback,
+            self.experiment_clock,
+            'VEP_INQUIRY')
+        # display the inquiry
+        self.static_clock.reset()
+        while self.static_clock.getTime() < self.stimuli_timing[0]:
+            self.draw_boxes()
+            self.draw_static()
+            self.window.flip()
+
+        timing += self.trigger_callback.timing
+
+        return timing
+
+    def draw_animation(self) -> None:
+        """Draw the stimuli animation."""
+        for sti in self.sti:
+            sti.draw()
+
+    def draw_boxes(self) -> None:
+        """Draw the text boxes under VEP stimuli."""
+        for box in self.text_boxes:
+            box.draw()
+
+    def stimulate(self) -> List[float]:
+        """Stimulate.
+
+        This is the main display function of the VEP paradigm. It is responsible for drawing the flickering stimuli.
+
+        It assumes that the VEP stimuli are already constructed using the _build_vep_corner_stimuli function.
+        These boxes are drawn in the order they are in the list as defined in self.vep."""
+        self.trigger_callback.reset()
+        self.window.callOnFlip(
+            self.trigger_callback.callback,
+            self.experiment_clock,
+            'VEP_STIMULATE')
+        self.static_clock.reset()
+        while self.static_clock.getTime() < self.stimuli_timing[-1]:
+            for frame in range(self.refresh_rate):
+                for box in self.vep:
+                    if box.code[frame] == 1:
+                        box.frame_on()
+                    else:
+                        box.frame_off()
+
+                # flicker!
+                self.draw_static()
+                self.window.flip()
+
+        return self.trigger_callback.timing
+
+    def draw_static(self) -> None:
+        """Draw static elements for the display."""
+        self.task.draw()
+        for info in self.info_text:
+            info.draw()
+
+    def update_task(self, text: str, color: str, pos: Optional[Tuple] = None) -> None:
+        """Update the task display which is displayed using the draw_static function."""
+        self.task.text = text
+        self.task.color = color
+        if pos:
+            self.task.pos = pos
+
+    def _build_inquiry_stimuli(self) -> None:
+        """Build the inquiry stimuli."""
+        all_letters = []
+        all_colors = []
+        self.sti = []
+        for letters, colors in zip(self.stimuli_inquiry, self.stimuli_colors):
+            for letter in letters:
+                all_letters.append(letter)
+                all_colors.append(colors[0])
+        pos = (0, 0)
+        for letter, color in zip(all_letters, all_colors):
+            pos = (pos[0] + self.stimuli_height, pos[1])
+            self.sti.append(
+                visual.TextStim(self.window, text=letter, color=color, pos=pos, height=self.stimuli_height))
+
+        return self.sti
+
+    def _build_vep_corner_stimuli(
+            self,
+            pos: Tuple[float, float],
+            codes: List[int],
+            colors: List[Tuple[str]],
+            box_size: float) -> List[visual.GratingStim]:
+        """Build the corner stimuli for the VEP.
+
+        Args:
+            window: psychopy window object
+        """
+        corner_stim = []
+        for pos, code, color in zip(pos, codes, colors):
+            corner_stim += self._build_2x2_vep_grid(pos, box_size, color, code)
+
+        return corner_stim
+
+    def _build_1x1_vep_grid(
+            self,
+            position: Tuple[float],
+            size: float,
+            color: str,
+            code: List[int]) -> List[visual.GratingStim]:
+        """Build a 1x1 VEP grid.
+
+        Args:
+            position: position of the flicking box
+            size: size of the flicking box
+            color: color of the flicking box
+            code: code to be used with the flicking box
+
+        Returns:
+            list of visual.GratingStim objects
+
+        """
+        assert len(code) >= self.refresh_rate, 'Code must be longer than refresh rate'
+        pattern1 = visual.GratingStim(win=self.window, name=f'1x1-1-{position}', units='height',
+                                      tex=None, mask=None,
+                                      ori=0, pos=position, size=size, sf=1, phase=0.0,
+                                      color=color[0], colorSpace='rgb', opacity=1,
+                                      texRes=256, interpolate=True, depth=-1.0)
+        pattern2 = visual.GratingStim(win=self.window, name=f'1x1-2-{position}', units='height',
+                                      tex=None, mask=None,
+                                      ori=0, pos=position, size=size, sf=1, phase=0,
+                                      color=color[1], colorSpace='rgb', opacity=1,
+                                      texRes=256, interpolate=True, depth=-2.0)
+        box = [VEPBox(flicker=[pattern1, pattern2], code=code)]
+        self.vep += box
+        return box
+
+    def _build_2x2_vep_grid(self,
+                            position: Tuple[float],
+                            size: float,
+                            color: str,
+                            code: List[int]) -> List[visual.GratingStim]:
+        """Build a 2x2 VEP grid.
+
+        Args:
+            position: position of the flicking box
+            size: size of the flicking box
+            color: color of the flicking box
+            code: code to be used with the flicking box
+
+        Returns:
+            list of visual.GratingStim objects
+        """
+
+        assert len(code) >= self.refresh_rate, 'Code must be longer than refresh rate'
+        starting_position = position
+        positions = [
+            starting_position,  # bottom left
+            [starting_position[0] + size, starting_position[1]],  # bottom right
+            [starting_position[0] + size, starting_position[1] + size],  # top right
+            [starting_position[0], starting_position[1] + size],  # top left
+        ]
+        box = []
+        for pos in positions:
+            pattern1 = visual.GratingStim(win=self.window, name=f'2x2-1-{pos}', units='height',
+                                          tex=None, mask=None,
+                                          ori=0, pos=pos, size=size, sf=1, phase=0.0,
+                                          color=color[0], colorSpace='rgb', opacity=1,
+                                          texRes=256, interpolate=True, depth=-1.0)
+            pattern2 = visual.GratingStim(win=self.window, name=f'2x2-2-{pos}', units='height',
+                                          tex=None, mask=None,
+                                          ori=0, pos=pos, size=size, sf=1, phase=0,
+                                          color=color[1], colorSpace='rgb', opacity=1,
+                                          texRes=256, interpolate=True, depth=-2.0)
+            color = (color[1], color[0])
+            box += [VEPBox(flicker=[pattern1, pattern2], code=code)]
+
+        self.vep += box
+        return box
+
+    def _trigger_pulse(self) -> None:
+        """Trigger Pulse.
+
+        This method uses a calibration trigger to determine any functional
+            offsets needed for operation with this display. By setting the first_stim_time and searching for the
+            same stimuli output to the marker stream, the offsets between these proceses can be reconciled at the
+            beginning of an experiment. If drift is detected in your experiment, more frequent pulses and offset
+            correction may be required.
+        """
+        calibration_time = _calibration_trigger(
+            self.experiment_clock,
+            trigger_type=self.trigger_type,
+            display=self.window)
+
+        # set the first stim time if not present and first_run to False
+        if not self.first_stim_time:
+            self.first_stim_time = calibration_time[-1]
+            self.first_run = False
+
+    def schedule_to(self, stimuli: List[List[str]], timing: List[List[float]], colors: List[List[str]]) -> None:
+        """Schedule stimuli elements (works as a buffer).
+        """
+        self.stimuli_inquiry = stimuli
+        self.stimuli_timing = timing
+        self.stimuli_colors = colors
+
+    def _build_text_boxes(self) -> List[visual.TextBox2]:
+        """Build the text boxes for the experiment.
+
+        This assumes that vep_type is 4 using a 2x2 grid. Additional configurations can be added in the future.
+        """
+        # generate the inquiry stimuli
+        assert len(
+            self.stimuli_colors) == self.vep_type, (
+                f"stmuli colors {len(self.stimuli_colors)} must be the same length as vep type {self.vep_type}")
+        assert len(
+            self.stimuli_pos) == self.vep_type, (
+                f"stmuli position {len(self.stimuli_pos)} must be the same length as vep type {self.vep_type}")
+
+        self.text_boxes = []
+        inc_q = int(self.vep_type / 2)
+        size = self.vep_box_size * inc_q
+        inc = 0  # get the last box in the grating stim per vep
+        for color in self.stimuli_colors:
+            text = ' '
+            first = self.vep[inc].flicker[0].pos
+            best_neighbor = self.vep[inc + inc_q].flicker[0].pos
+
+            # the textbox requires the pos to be centered on the middle of the box, so
+            # we need to calculate the center of the vep stimulus boxes
+            pos = (first[0] + best_neighbor[0]) / 2, (first[1] + best_neighbor[1]) / 2
+            self.text_boxes += [visual.TextBox2(
+                win=self.window,
+                text=text,
+                font=self.stimuli_font,
+                units='height',
+                pos=pos,
+                color=color[0],
+                colorSpace='rgb',
+                size=[size, size],
+                alignment='center',
+                anchor='center',
+                borderWidth=2,
+                borderColor='white',
+                letterHeight=self.stimuli_height / 2)]
+            inc += self.vep_type
+        return self.text_boxes
+
+    def _reset_text_boxes(self) -> None:
+        """Reset text boxes.
+
+        This method resets the text boxes to the blank state.
+        """
+        for text_box in self.text_boxes:
+            text_box.setText(' ')
+
+    def _set_inquiry(self) -> List[visual.TextBox2]:
+        """Generate Inquiry.
+
+        This method sets the correct inquiry text for each text boxes.
+        """
+        # generate the inquiry stimuli
+        assert len(
+            self.stimuli_inquiry) == self.vep_type, (
+                f"stmuli inquiry {len(self.stimuli_inquiry)} must be the same length as vep type {self.vep_type}")
+        assert len(
+            self.stimuli_colors) == self.vep_type, (
+                f"stmuli colors {len(self.stimuli_colors)} must be the same length as vep type {self.vep_type}")
+        for box_content, color, box in zip(self.stimuli_inquiry, self.stimuli_colors, self.text_boxes):
+            text = ' '.join(box_content)
+            box.text = text
+            box.color = color[0]
+        return self.text_boxes
+
+    def wait_screen(self, message: str, color: str) -> None:
+        """Wait Screen.
+
+        Args:
+            message(string): message to be displayed while waiting
+            color(string): color of the message to be displayed
+        """
+
+        # Construct the wait message
+        wait_message = visual.TextStim(win=self.window,
+                                       font=self.stimuli_font,
+                                       text=message,
+                                       height=.1,
+                                       color=color,
+                                       pos=(0, -.5),
+                                       wrapWidth=2,
+                                       colorSpace='rgb',
+                                       opacity=1,
+                                       depth=-6.0)
+
+        # try adding the BciPy logo to the wait screen
+        try:
+            wait_logo = visual.ImageStim(
+                self.window,
+                image=BCIPY_LOGO_PATH,
+                pos=(0, .25),
+                mask=None,
+                ori=0.0)
+            wait_logo.size = resize_image(
+                BCIPY_LOGO_PATH,
+                self.window.size,
+                1)
+            wait_logo.draw()
+
+        except Exception as e:
+            self.logger.exception(f'Cannot load logo image from path=[{BCIPY_LOGO_PATH}]')
+            raise e
+
+        # Draw and flip the screen.
+        wait_message.draw()
+        self.draw_static()
+        self.window.flip()
```

### Comparing `bcipy-2.0.0rc3/bcipy/feedback/feedback.py` & `bcipy-2.0.1rc2/bcipy/feedback/feedback.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/feedback/sound/auditory_feedback.py` & `bcipy-2.0.1rc2/bcipy/feedback/sound/auditory_feedback.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/feedback/visual/level_feedback.py` & `bcipy-2.0.1rc2/bcipy/feedback/visual/level_feedback.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/feedback/visual/visual_feedback.py` & `bcipy-2.0.1rc2/bcipy/feedback/visual/visual_feedback.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/gui/BCInterface.py` & `bcipy-2.0.1rc2/bcipy/gui/BCInterface.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/gui/alert.py` & `bcipy-2.0.1rc2/bcipy/gui/alert.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/gui/experiments/ExperimentField.py` & `bcipy-2.0.1rc2/bcipy/gui/experiments/ExperimentField.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/gui/experiments/ExperimentRegistry.py` & `bcipy-2.0.1rc2/bcipy/gui/experiments/ExperimentRegistry.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/gui/experiments/FieldRegistry.py` & `bcipy-2.0.1rc2/bcipy/gui/experiments/FieldRegistry.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/gui/file_dialog.py` & `bcipy-2.0.1rc2/bcipy/gui/file_dialog.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,91 @@
-# pylint: disable=no-name-in-module,missing-docstring,too-few-public-methods
-import sys
-from pathlib import Path
-from PyQt5.QtWidgets import QApplication, QWidget, QFileDialog, QDesktopWidget
-from bcipy.preferences import preferences
-
-DEFAULT_FILE_TYPES = "All Files (*)"
-
-
-class FileDialog(QWidget):
-    """GUI window that prompts the user to select a file."""
-
-    def __init__(self):
-        super().__init__()
-        self.title = 'PyQt5 file dialogs - pythonspot.com'
-        self.width = 640
-        self.height = 480
-
-        # Center on screen
-        self.resize(self.width, self.height)
-        frame_geom = self.frameGeometry()
-        frame_geom.moveCenter(QDesktopWidget().availableGeometry().center())
-        self.move(frame_geom.topLeft())
-
-        # The native dialog may prevent the selection from closing after a
-        # directory is selected.
-        self.options = QFileDialog.Options()
-        self.options |= QFileDialog.DontUseNativeDialog
-
-    def ask_file(self, file_types: str = DEFAULT_FILE_TYPES, directory: str = "") -> str:
-        """Opens a file dialog window.
-        Returns
-        -------
-        path or None
-        """
-        filename, _ = QFileDialog.getOpenFileName(self,
-                                                  "Select File",
-                                                  directory,
-                                                  file_types,
-                                                  options=self.options)
-        return filename
-
-    def ask_directory(self, directory: str = "") -> str:
-        """Opens a dialog window to select a directory.
-
-        Returns
-        -------
-        path or None
-        """
-        return QFileDialog.getExistingDirectory(self,
-                                                "Select Directory",
-                                                directory=directory,
-                                                options=self.options)
-
-
-def ask_filename(file_types: str = DEFAULT_FILE_TYPES, directory: str = "") -> str:
-    """Prompt for a file.
-
-    Parameters
-    ----------
-    - file_types : optional file type filters; Examples: 'Text files (*.txt)'
-    or 'Image files (*.jpg *.gif)' or '*.csv;;*.pkl'
-    - directory : optional directory
-
-    Returns
-    -------
-    path to file or None if the user cancelled the dialog.
-    """
-    app = QApplication(sys.argv)
-    dialog = FileDialog()
-    directory = directory or preferences.last_directory
-    filename = dialog.ask_file(file_types, directory)
-
-    # update last directory preference
-    path = Path(filename)
-    if filename and path.is_file():
-        preferences.last_directory = str(path.parent)
-
-    # Alternatively, we could use `app.closeAllWindows()`
-    app.quit()
-
-    return filename
-
-
-def ask_directory() -> str:
-    """Prompt for a directory.
-
-    Returns
-    -------
-    path to directory or None if the user cancelled the dialog.
-    """
-    app = QApplication(sys.argv)
-
-    dialog = FileDialog()
-    directory = ''
-    if preferences.last_directory:
-        directory = str(Path(preferences.last_directory).parent)
-    name = dialog.ask_directory(directory)
-    if name and Path(name).is_dir():
-        preferences.last_directory = name
-    # Alternatively, we could use `app.closeAllWindows()`
-    app.quit()
-
-    return name
+# pylint: disable=no-name-in-module,missing-docstring,too-few-public-methods
+import sys
+from PyQt5.QtWidgets import QApplication, QWidget, QFileDialog, QDesktopWidget
+
+DEFAULT_FILE_TYPES = "All Files (*)"
+
+
+class FileDialog(QWidget):
+    """GUI window that prompts the user to select a file."""
+
+    def __init__(self):
+        super().__init__()
+        self.title = 'PyQt5 file dialogs - pythonspot.com'
+        self.width = 640
+        self.height = 480
+
+        # Center on screen
+        self.resize(self.width, self.height)
+        frame_geom = self.frameGeometry()
+        frame_geom.moveCenter(QDesktopWidget().availableGeometry().center())
+        self.move(frame_geom.topLeft())
+
+        # The native dialog may prevent the selection from closing after a
+        # directory is selected.
+        self.options = QFileDialog.Options()
+        self.options |= QFileDialog.DontUseNativeDialog
+
+    def ask_file(self, file_types: str = DEFAULT_FILE_TYPES, directory: str = "") -> str:
+        """Opens a file dialog window.
+        Returns
+        -------
+        path or None
+        """
+        filename, _ = QFileDialog.getOpenFileName(self,
+                                                  "Select File",
+                                                  directory,
+                                                  file_types,
+                                                  options=self.options)
+        return filename
+
+    def ask_directory(self) -> str:
+        """Opens a dialog window to select a directory.
+
+        Returns
+        -------
+        path or None
+        """
+        return QFileDialog.getExistingDirectory(self,
+                                                "Select Directory",
+                                                options=self.options)
+
+
+def ask_filename(file_types: str = DEFAULT_FILE_TYPES, directory: str = "") -> str:
+    """Prompt for a file.
+
+    Parameters
+    ----------
+    - file_types : optional file type filters; Examples: 'Text files (*.txt)'
+    or 'Image files (*.jpg *.gif)' or '*.csv;;*.pkl'
+    - directory : optional directory
+
+    Returns
+    -------
+    path to file or None if the user cancelled the dialog.
+    """
+    app = QApplication(sys.argv)
+    dialog = FileDialog()
+    filename = dialog.ask_file(file_types, directory)
+
+    # Alternatively, we could use `app.closeAllWindows()`
+    app.quit()
+
+    return filename
+
+
+def ask_directory() -> str:
+    """Prompt for a directory.
+
+    Returns
+    -------
+    path to directory or None if the user cancelled the dialog.
+    """
+    app = QApplication(sys.argv)
+
+    dialog = FileDialog()
+    name = dialog.ask_directory()
+
+    # Alternatively, we could use `app.closeAllWindows()`
+    app.quit()
+
+    return name
```

### Comparing `bcipy-2.0.0rc3/bcipy/gui/viewer/data_source/data_source.py` & `bcipy-2.0.1rc2/bcipy/gui/viewer/data_source/data_source.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/gui/viewer/data_source/file_streamer.py` & `bcipy-2.0.1rc2/bcipy/gui/viewer/data_source/file_streamer.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/gui/viewer/data_source/lsl_data_source.py` & `bcipy-2.0.1rc2/bcipy/gui/viewer/data_source/lsl_data_source.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/gui/viewer/data_viewer.py` & `bcipy-2.0.1rc2/bcipy/gui/viewer/data_viewer.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/gui/viewer/ring_buffer.py` & `bcipy-2.0.1rc2/bcipy/gui/viewer/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/clock.py` & `bcipy-2.0.1rc2/bcipy/helpers/clock.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/convert.py` & `bcipy-2.0.1rc2/bcipy/helpers/convert.py`

 * *Files 11% similar despite different names*

```diff
@@ -482,104 +482,25 @@
     if tar_file_name.endswith('.tar.gz'):
         return tar_file_name
     return f'{tar_file_name}.tar.gz'
 
 
 def convert_to_mne(
         raw_data: RawData,
-        channel_map: List[int] = None,
-        channel_types: Optional[List[str]] = None,
+        channel_map: List[int],
         transform: Optional[Composition] = None,
-        montage: str = 'standard_1020',
-        volts: bool = True) -> RawArray:
+        montage: str = 'standard_1020') -> RawArray:
     """Convert to MNE.
 
-    Returns BciPy RawData as an MNE RawArray. This assumes all channel names
-    are reflective of provided montage locations.
-
-    Parameters
-    ----------
-        raw_data - BciPy RawData object
-        channel_map - optional list of channels to include in the MNE RawArray [1, 0, 1, 0, 1, 0, 1, 0].
-            1 indicates the channel should be included, 0 indicates it should be excluded.
-            Must be the same length as the number of channels in the raw_data.
-        channel_types - list of channel types to include in the MNE RawArray.
-            If None, all channels will be assumed to be eeg.
-            See: https://mne.tools/stable/overview/implementation.html#supported-channel-types
-        transform - optional transform to apply to the data
-        montage - name of the channel location montage to use.
-            See https://mne.tools/dev/generated/mne.channels.make_standard_montage.html
-        volts - if True, assume data is already in volts. If false, assume data is in microvolts and convert to volts.
-            MNE expects data to be in volts.
-            See: https://mne.tools/dev/overview/implementation.html#internal-representation-units
+    Returns BciPy RawData as an MNE RawArray. This assumes all data channels are eeg and channel names
+    are reflective of standard 1020 locations.
+    See https://mne.tools/dev/generated/mne.channels.make_standard_montage.html
     """
-    # if no channel map provided, assume all channels are included
-    if not channel_map:
-        channel_map = [1] * len(raw_data.channels)
-
     data, channels, fs = raw_data.by_channel_map(channel_map, transform)
-
-    # if no channel types provided, assume all channels are eeg
-    if not channel_types:
-        channel_types = ['eeg'] * len(channels)
-
-    # check that number of channel types matches number of channels in the case custom channel types are provided
-    assert len(channel_types) == len(channels), \
-        f'Number of channel types ({len(channel_types)}) must match number of channels ({len(channels)})'
+    channel_types = ['eeg' for _ in channels]
 
     info = mne.create_info(channels, fs, channel_types)
     mne_data = RawArray(data, info)
     ten_twenty_montage = mne.channels.make_standard_montage(montage)
     mne_data.set_montage(ten_twenty_montage)
 
-    # convert to volts if necessary (the default for many systems is microvolts)
-    if not volts:
-        mne_data = mne_data.apply_function(lambda x: x * 1e-6)
-
     return mne_data
-
-
-def tobii_to_norm(tobii_units: Tuple[float, float]) -> Tuple[float, float]:
-    """Tobii to PsychoPy's 'norm' units.
-
-    https://developer.tobiipro.com/commonconcepts/coordinatesystems.html
-    https://www.psychopy.org/general/units.html
-
-    Tobii uses an Active Display Coordinate System.
-        The point (0, 0) denotes the upper left corner and (1, 1) the lower right corner of it.
-
-    PsychoPy uses several coordinate systems, the normalized window unit is assumed here.
-        The point (0, 0) denotes the center of the screen and (-1, -1) the upper left corner
-        and (1, 1) the lower right corner.
-
-    """
-    # check that Tobii units are within the expected range
-    assert 0 <= tobii_units[0] <= 1, "Tobii x coordinate must be between 0 and 1"
-    assert 0 <= tobii_units[1] <= 1, "Tobii y coordinate must be between 0 and 1"
-
-    # convert Tobii units to Psychopy units
-    norm_x = (tobii_units[0] - 0.5) * 2
-    norm_y = (tobii_units[1] - 0.5) * 2 * -1
-    return (norm_x, norm_y)
-
-
-def norm_to_tobii(norm_units: Tuple[float, float]) -> Tuple[float, float]:
-    """PsychoPy's 'norm' units to Tobii.
-
-    https://developer.tobiipro.com/commonconcepts/coordinatesystems.html
-    https://www.psychopy.org/general/units.html
-
-    Tobii uses an Active Display Coordinate System.
-        The point (0, 0) denotes the upper left corner and (1, 1) the lower right corner of it.
-
-    PsychoPy uses several coordinate systems, the normalized window unit is assumed here.
-        The point (0, 0) denotes the center of the screen and (-1, -1) the upper left corner
-        and (1, 1) the lower right corner.
-    """
-    # check that the coordinates are within the bounds of the screen
-    assert norm_units[0] >= -1 and norm_units[0] <= 1, "X coordinate must be between -1 and 1"
-    assert norm_units[1] >= -1 and norm_units[1] <= 1, "Y coordinate must be between -1 and 1"
-
-    # convert PsychoPy norm units to Tobii units
-    tobii_x = (norm_units[0] / 2) + 0.5
-    tobii_y = ((norm_units[1] * -1) / 2) + 0.5
-    return (tobii_x, tobii_y)
```

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/copy_phrase_wrapper.py` & `bcipy-2.0.1rc2/bcipy/helpers/copy_phrase_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,327 +1,331 @@
-"""Defines the CopyPhraseWrapper."""
-from typing import List, Tuple
-
-import logging
-import numpy as np
-from bcipy.helpers.acquisition import analysis_channels, DeviceSpec
-from bcipy.helpers.exceptions import BciPyCoreException
-from bcipy.helpers.language_model import (
-    histogram,
-    with_min_prob,
-)
-from bcipy.helpers.stimuli import InquirySchedule, StimuliOrder, TrialReshaper
-from bcipy.helpers.symbols import BACKSPACE_CHAR
-from bcipy.signal.model import SignalModel
-from bcipy.signal.process import get_default_transform
-from bcipy.task.control.handler import DecisionMaker, EvidenceFusion
-from bcipy.task.control.query import NBestStimuliAgent
-from bcipy.task.control.criteria import (
-    CriteriaEvaluator,
-    MaxIterationsCriteria,
-    MinIterationsCriteria,
-    ProbThresholdCriteria,
-)
-from bcipy.task.data import EvidenceType
-from bcipy.language.main import LanguageModel
-
-
-log = logging.getLogger(__name__)
-
-
-class CopyPhraseWrapper:
-    """Basic copy phrase task duty cycle wrapper. Coordinates activities around
-    spelling tasks, including:
-
-    - Evidence management: adding and fusing evidence using the EvidenceFusion
-    module.
-    - Decision-making: uses evidence to make a decision or decide to continue
-    by providing another inquiry (DecisionMaker).
-    - Determining when to stop an inquiry and make a decision (StoppageCriteria).
-    - Generation of inquiries.
-    - Coordination with the Language Model.
-    - Preparing EEG data for the SignalModel for classification.
-
-    Parameters
-    ----------
-    - min_num_inq: The minimum number of inquiries to be displayed
-    - max_num_inq: The maximum number of inquiries to be displayed
-    - device_spec: Specification for the EEG device used for data collection.
-    - signal_model: model trained using a calibration session of the same user.
-    - k: down sampling rate
-    - alp: symbol set of the task
-    - evidence_names: list of evidence types used for decision-making
-    - task_list: list[(phrases, initial_states)] for the copy phrase task
-    - lmodel: language model used (when 'LM') evidence type is used.
-    - is_txt_stim: Whether or not the stimuli are text objects
-    - decision_threshold: Minimum likelihood value required for a decision
-    - backspace_prob: default language model probability for the
-    backspace character.
-    - backspace_always_shown: whether or not the backspace should
-    always be presented.
-    - filter_high: filter setting used when evaluating EEG data
-    - filter_low: filter setting used when evaluating EEG data
-    - filter_order: filter setting used when evaluating EEG data
-    - notch_filter_frequency: filter setting used when evaluating EEG data
-    - stim_length(int): the number of stimuli to present in each inquiry
-    - stim_timing: seconds each stimuli is displayed; used for inquiry
-    generation
-    - stim_jitter: seconds that inquiry stimuli should be jittered (-/+ stim_timing[-1])
-    """
-
-    def __init__(self,
-                 min_num_inq: int,
-                 max_num_inq: int,
-                 lmodel: LanguageModel,
-                 device_spec: DeviceSpec,
-                 signal_model: SignalModel = None,
-                 k: int = 2,
-                 alp: List[str] = None,
-                 evidence_names: List[EvidenceType] = [
-                     EvidenceType.LM, EvidenceType.ERP
-                 ],
-                 task_list: List[Tuple[str, str]] = [('I_LOVE_COOKIES',
-                                                      'I_LOVE_')],
-                 is_txt_stim: bool = True,
-                 decision_threshold: float = 0.8,
-                 backspace_prob: float = 0.05,
-                 backspace_always_shown: bool = False,
-                 filter_high: int = 45,
-                 filter_low: int = 2,
-                 filter_order: int = 2,
-                 notch_filter_frequency: int = 60,
-                 stim_timing: List[float] = [1, .2],
-                 stim_length: int = 10,
-                 stim_jitter: float = 0,
-                 stim_order: StimuliOrder = StimuliOrder.RANDOM):
-
-        self.lmodel = lmodel
-        self.conjugator = EvidenceFusion(evidence_names, len_dist=len(alp))
-
-        inq_constants = []
-        if backspace_always_shown and BACKSPACE_CHAR in alp:
-            inq_constants.append(BACKSPACE_CHAR)
-
-        # Stimuli Selection Module
-        stopping_criteria = CriteriaEvaluator(
-            continue_criteria=[MinIterationsCriteria(min_num_inq)],
-            commit_criteria=[MaxIterationsCriteria(max_num_inq),
-                             ProbThresholdCriteria(decision_threshold)])
-
-        self.stim_length = stim_length
-        self.stim_order = stim_order
-        stimuli_agent = NBestStimuliAgent(alphabet=alp,
-                                          len_query=self.stim_length)
-
-        self.decision_maker = DecisionMaker(
-            stimuli_agent=stimuli_agent,
-            stopping_evaluator=stopping_criteria,
-            state=task_list[0][1],
-            alphabet=alp,
-            is_txt_stim=is_txt_stim,
-            stimuli_jitter=stim_jitter,
-            stimuli_timing=stim_timing,
-            stimuli_order=self.stim_order,
-            inq_constants=inq_constants)
-
-        self.alp = alp
-        # non-letter target labels include the fixation cross and calibration.
-        self.nonletters = ['+', 'PLUS', 'calibration_trigger']
-        self.valid_targets = set(self.alp)
-
-        self.signal_model = signal_model
-        self.sampling_rate = device_spec.sample_rate
-        self.downsample_rate = k
-        self.filter_high = filter_high
-        self.filter_low = filter_low
-        self.filter_order = filter_order
-        self.notch_filter_frequency = notch_filter_frequency
-
-        self.mode = 'copy_phrase'
-        self.task_list = task_list
-        self.channel_map = analysis_channels(device_spec.channels, device_spec)
-        self.backspace_prob = backspace_prob
-
-    def evaluate_inquiry(
-            self, raw_data: np.array, triggers: List[Tuple[str, float]],
-            target_info: List[str], window_length: float
-    ) -> Tuple[bool, Tuple[List[str], List[float], List[str]]]:
-        """Once data is collected, infers meaning from the data and attempt to
-        make a decision.
-
-        Parameters
-        ----------
-        - raw_data: C x L eeg data where C is number of channels and L is the
-        signal length
-        - triggers: triggers e.g. `('A', 1)` as letter and flash time for the
-        letter
-        - target_info: target information about the stimuli
-        - window_length: The length of the time between stimuli presentation
-
-        Returns
-        -------
-        - (True, None) when commitment is made.
-        - (False, next set of stimuli) when not enough evidence has
-        been provided and stoppage criteria is not yet met.
-        """
-        lik_r = self.evaluate_eeg_evidence(raw_data, triggers, target_info,
-                                           window_length)
-        self.add_evidence(EvidenceType.ERP, lik_r)
-        return self.decide()
-
-    def evaluate_eeg_evidence(self, raw_data: np.array,
-                              triggers: List[Tuple[str, float]],
-                              target_info: List[str],
-                              window_length: float) -> np.array:
-        """Once data is collected, infers meaning from the data and return the results.
-
-        Parameters
-        ----------
-        - raw_data: C x L eeg data where C is number of channels and L is the
-        signal length
-        - triggers: triggers e.g. `('A', 1)` as letter and flash time for the
-        letter
-        - target_info: target information about the stimuli
-        - window_length: The length of the time between stimuli presentation
-
-        Returns
-        -------
-        np.array of likelihood evidence
-        """
-        letters, times, target_info = self.letter_info(triggers, target_info)
-
-        default_transform = get_default_transform(
-            sample_rate_hz=self.sampling_rate,
-            notch_freq_hz=self.notch_filter_frequency,
-            bandpass_low=self.filter_low,
-            bandpass_high=self.filter_high,
-            bandpass_order=self.filter_order,
-            downsample_factor=self.downsample_rate,
-        )
-
-        data, transformed_sample_rate = default_transform(raw_data, self.sampling_rate)
-
-        # The data from DAQ is assumed to have offsets applied
-        data, _ = TrialReshaper()(
-            trial_targetness_label=target_info,
-            timing_info=times,
-            eeg_data=data,
-            sample_rate=transformed_sample_rate,
-            channel_map=self.channel_map,
-            poststimulus_length=window_length)
-
-        return self.signal_model.predict(data, letters, self.alp)
-
-    def add_evidence(self, evidence_type: EvidenceType,
-                     evidence: List[float]) -> np.array:
-        """Add evidence to the conjugator.
-
-        Parameters
-        ----------
-        - evidence_type : type of evidence (ex. `'LM'`, `'ERP'`)
-        - evidence : ndarray[float], evidence for each stim
-
-        Returns
-        -------
-        updated likelihoods after fusing the new evidence
-        """
-        assert evidence_type in self.conjugator.evidence_history.keys(
-        ), f"Copy Phrase wrapper was not initialized with evidence type: {evidence_type}."
-        return self.conjugator.update_and_fuse(
-            {evidence_type: np.array(evidence)})
-
-    def decide(self) -> Tuple[bool, InquirySchedule]:
-        """Make a decision based on the current evidence.
-
-        Returns
-        -------
-        - (True, None) when commitment is made.
-        - (False, next set of stimuli) when not enough evidence has
-        been provided and stoppage criteria is not yet met.
-        """
-        decision, new_stim = self.decision_maker.decide(
-            self.conjugator.likelihood[:])
-        return decision, new_stim
-
-    def letter_info(self, triggers: List[Tuple[str, float]],
-                    target_info: List[str]
-                    ) -> Tuple[List[str], List[float], List[str]]:
-        """
-        Filters out non-letters and separates timings from letters.
-
-        Parameters
-        ----------
-        - triggers: triggers e.g. [['A', 0.5], ...]
-        as letter and flash time for the letter
-        - target_info: target information about the stimuli;
-        ex. ['nontarget', 'nontarget', ...]
-
-        Returns
-        -------
-        (letters, times, target_info)
-        """
-        letters = []
-        times = []
-        target_types = []
-
-        for i, (letter, stamp) in enumerate(triggers):
-            if letter not in self.nonletters:
-                letters.append(letter)
-                times.append(stamp)
-                target_types.append(target_info[i])
-
-        # Raise an error if the stimuli includes unexpected terms
-        if not set(letters).issubset(self.valid_targets):
-            invalid = set(letters).difference(self.valid_targets)
-            error_message = f'unexpected letters received in copy phrase: {invalid}'
-            log.error(error_message)
-            raise BciPyCoreException(error_message)
-
-        return letters, times, target_types
-
-    def initialize_series(self) -> Tuple[bool, InquirySchedule]:
-        """If a decision is made initializes the next series."""
-        assert self.lmodel, "Language model must be initialized."
-
-        try:
-            # First, reset the history for this new series
-            self.conjugator.reset_history()
-
-            # Get the displayed state
-            update = self.decision_maker.displayed_state
-            log.info(f"Querying language model: '{update}'")
-
-            # update the lmodel and get back the priors
-            lm_letter_prior = self.lmodel.predict(list(update))
-
-            if BACKSPACE_CHAR in self.alp:
-                # Apply configured backspace probability.
-                sym = (BACKSPACE_CHAR, self.backspace_prob)
-                lm_letter_prior = with_min_prob(lm_letter_prior, sym)
-
-            # convert to format needed for evidence fusion;
-            # probability value only in alphabet order.
-            prior = [
-                prior_prob for alp_letter in self.alp
-                for prior_sym, prior_prob in lm_letter_prior
-                if alp_letter == prior_sym
-            ]
-
-            # display histogram of LM probabilities
-            log.debug(histogram(lm_letter_prior))
-
-            # Try fusing the lmodel evidence
-            try:
-                prob_dist = self.conjugator.update_and_fuse(
-                    {EvidenceType.LM: np.array(prior)})
-            except Exception as fusion_error:
-                log.exception(f'Error fusing language model evidence!: {fusion_error}')
-                raise BciPyCoreException(fusion_error) from fusion_error
-
-            # Get decision maker to give us back some decisions and stimuli
-            is_accepted, sti = self.decision_maker.decide(prob_dist)
-
-        except Exception as init_series_error:
-            log.exception(f'Error in initialize_series: {init_series_error}')
-            raise BciPyCoreException(init_series_error) from init_series_error
-
-        return is_accepted, sti
+"""Defines the CopyPhraseWrapper."""
+from typing import List, Tuple
+
+import logging
+import numpy as np
+from bcipy.helpers.acquisition import analysis_channels
+from bcipy.helpers.exceptions import BciPyCoreException
+from bcipy.helpers.language_model import (
+    histogram,
+    with_min_prob,
+)
+from bcipy.helpers.stimuli import InquirySchedule, StimuliOrder, TrialReshaper
+from bcipy.helpers.task import BACKSPACE_CHAR
+from bcipy.signal.model import SignalModel
+from bcipy.signal.process import get_default_transform
+from bcipy.task.control.handler import DecisionMaker, EvidenceFusion
+from bcipy.task.control.query import NBestStimuliAgent
+from bcipy.task.control.criteria import (
+    CriteriaEvaluator,
+    MaxIterationsCriteria,
+    MinIterationsCriteria,
+    ProbThresholdCriteria,
+)
+from bcipy.task.data import EvidenceType
+from bcipy.language.main import LanguageModel
+
+
+log = logging.getLogger(__name__)
+
+
+class CopyPhraseWrapper:
+    """Basic copy phrase task duty cycle wrapper. Coordinates activities around
+    spelling tasks, including:
+
+    - Evidence management: adding and fusing evidence using the EvidenceFusion
+    module.
+    - Decision-making: uses evidence to make a decision or decide to continue
+    by providing another inquiry (DecisionMaker).
+    - Determining when to stop an inquiry and make a decision (StoppageCriteria).
+    - Generation of inquiries.
+    - Coordination with the Language Model.
+    - Preparing EEG data for the SignalModel for classification.
+
+    Parameters
+    ----------
+    - min_num_inq: The minimum number of inquiries to be displayed
+    - max_num_inq: The maximum number of inquiries to be displayed
+    - signal_model: model trained using a calibration session of the same user.
+    - fs: sampling frequency
+    - k: down sampling rate
+    - alp: symbol set of the task
+    - evidence_names: list of evidence types used for decision-making
+    - task_list: list[(phrases, initial_states)] for the copy phrase task
+    - lmodel: language model used (when 'LM') evidence type is used.
+    - is_txt_stim: Whether or not the stimuli are text objects
+    - device_name: name of the EEG device
+    - device_channels: list of device channel names
+    - decision_threshold: Minimum likelihood value required for a decision
+    - backspace_prob: default language model probability for the
+    backspace character.
+    - backspace_always_shown: whether or not the backspace should
+    always be presented.
+    - filter_high: filter setting used when evaluating EEG data
+    - filter_low: filter setting used when evaluating EEG data
+    - filter_order: filter setting used when evaluating EEG data
+    - notch_filter_frequency: filter setting used when evaluating EEG data
+    - stim_length(int): the number of stimuli to present in each inquiry
+    - stim_timing: seconds each stimuli is displayed; used for inquiry
+    generation
+    - stim_jitter: seconds that inquiry stimuli should be jittered (-/+ stim_timing[-1])
+    """
+
+    def __init__(self,
+                 min_num_inq: int,
+                 max_num_inq: int,
+                 lmodel: LanguageModel,
+                 signal_model: SignalModel = None,
+                 fs: int = 300,
+                 k: int = 2,
+                 alp: List[str] = None,
+                 evidence_names: List[EvidenceType] = [
+                     EvidenceType.LM, EvidenceType.ERP
+                 ],
+                 task_list: List[Tuple[str, str]] = [('I_LOVE_COOKIES',
+                                                      'I_LOVE_')],
+                 is_txt_stim: bool = True,
+                 device_name: str = 'LSL',
+                 device_channels: List[str] = None,
+                 decision_threshold: float = 0.8,
+                 backspace_prob: float = 0.05,
+                 backspace_always_shown: bool = False,
+                 filter_high: int = 45,
+                 filter_low: int = 2,
+                 filter_order: int = 2,
+                 notch_filter_frequency: int = 60,
+                 stim_timing: List[float] = [1, .2],
+                 stim_length: int = 10,
+                 stim_jitter: float = 0,
+                 stim_order: StimuliOrder = StimuliOrder.RANDOM):
+
+        self.lmodel = lmodel
+        self.conjugator = EvidenceFusion(evidence_names, len_dist=len(alp))
+
+        inq_constants = []
+        if backspace_always_shown and BACKSPACE_CHAR in alp:
+            inq_constants.append(BACKSPACE_CHAR)
+
+        # Stimuli Selection Module
+        stopping_criteria = CriteriaEvaluator(
+            continue_criteria=[MinIterationsCriteria(min_num_inq)],
+            commit_criteria=[MaxIterationsCriteria(max_num_inq),
+                             ProbThresholdCriteria(decision_threshold)])
+
+        self.stim_length = stim_length
+        self.stim_order = stim_order
+        stimuli_agent = NBestStimuliAgent(alphabet=alp,
+                                          len_query=self.stim_length)
+
+        self.decision_maker = DecisionMaker(
+            stimuli_agent=stimuli_agent,
+            stopping_evaluator=stopping_criteria,
+            state=task_list[0][1],
+            alphabet=alp,
+            is_txt_stim=is_txt_stim,
+            stimuli_jitter=stim_jitter,
+            stimuli_timing=stim_timing,
+            stimuli_order=self.stim_order,
+            inq_constants=inq_constants)
+
+        self.alp = alp
+        # non-letter target labels include the fixation cross and calibration.
+        self.nonletters = ['+', 'PLUS', 'calibration_trigger']
+        self.valid_targets = set(self.alp)
+
+        self.signal_model = signal_model
+        self.sampling_rate = fs
+        self.downsample_rate = k
+        self.filter_high = filter_high
+        self.filter_low = filter_low
+        self.filter_order = filter_order
+        self.notch_filter_frequency = notch_filter_frequency
+
+        self.mode = 'copy_phrase'
+        self.task_list = task_list
+        self.channel_map = analysis_channels(device_channels, device_name)
+        self.backspace_prob = backspace_prob
+
+    def evaluate_inquiry(
+            self, raw_data: np.array, triggers: List[Tuple[str, float]],
+            target_info: List[str], window_length: float
+    ) -> Tuple[bool, Tuple[List[str], List[float], List[str]]]:
+        """Once data is collected, infers meaning from the data and attempt to
+        make a decision.
+
+        Parameters
+        ----------
+        - raw_data: C x L eeg data where C is number of channels and L is the
+        signal length
+        - triggers: triggers e.g. `('A', 1)` as letter and flash time for the
+        letter
+        - target_info: target information about the stimuli
+        - window_length: The length of the time between stimuli presentation
+
+        Returns
+        -------
+        - (True, None) when commitment is made.
+        - (False, next set of stimuli) when not enough evidence has
+        been provided and stoppage criteria is not yet met.
+        """
+        lik_r = self.evaluate_eeg_evidence(raw_data, triggers, target_info,
+                                           window_length)
+        self.add_evidence(EvidenceType.ERP, lik_r)
+        return self.decide()
+
+    def evaluate_eeg_evidence(self, raw_data: np.array,
+                              triggers: List[Tuple[str, float]],
+                              target_info: List[str],
+                              window_length: float) -> np.array:
+        """Once data is collected, infers meaning from the data and return the results.
+
+        Parameters
+        ----------
+        - raw_data: C x L eeg data where C is number of channels and L is the
+        signal length
+        - triggers: triggers e.g. `('A', 1)` as letter and flash time for the
+        letter
+        - target_info: target information about the stimuli
+        - window_length: The length of the time between stimuli presentation
+
+        Returns
+        -------
+        np.array of likelihood evidence
+        """
+        letters, times, target_info = self.letter_info(triggers, target_info)
+
+        default_transform = get_default_transform(
+            sample_rate_hz=self.sampling_rate,
+            notch_freq_hz=self.notch_filter_frequency,
+            bandpass_low=self.filter_low,
+            bandpass_high=self.filter_high,
+            bandpass_order=self.filter_order,
+            downsample_factor=self.downsample_rate,
+        )
+
+        data, transformed_sample_rate = default_transform(raw_data, self.sampling_rate)
+
+        # The data from DAQ is assumed to have offsets applied
+        data, _ = TrialReshaper()(
+            trial_targetness_label=target_info,
+            timing_info=times,
+            eeg_data=data,
+            sample_rate=transformed_sample_rate,
+            channel_map=self.channel_map,
+            poststimulus_length=window_length)
+
+        return self.signal_model.predict(data, letters, self.alp)
+
+    def add_evidence(self, evidence_type: EvidenceType,
+                     evidence: List[float]) -> np.array:
+        """Add evidence to the conjugator.
+
+        Parameters
+        ----------
+        - evidence_type : type of evidence (ex. `'LM'`, `'ERP'`)
+        - evidence : ndarray[float], evidence for each stim
+
+        Returns
+        -------
+        updated likelihoods after fusing the new evidence
+        """
+        assert evidence_type in self.conjugator.evidence_history.keys(
+        ), f"Copy Phrase wrapper was not initialized with evidence type: {evidence_type}."
+        return self.conjugator.update_and_fuse(
+            {evidence_type: np.array(evidence)})
+
+    def decide(self) -> Tuple[bool, InquirySchedule]:
+        """Make a decision based on the current evidence.
+
+        Returns
+        -------
+        - (True, None) when commitment is made.
+        - (False, next set of stimuli) when not enough evidence has
+        been provided and stoppage criteria is not yet met.
+        """
+        decision, new_stim = self.decision_maker.decide(
+            self.conjugator.likelihood[:])
+        return decision, new_stim
+
+    def letter_info(self, triggers: List[Tuple[str, float]],
+                    target_info: List[str]
+                    ) -> Tuple[List[str], List[float], List[str]]:
+        """
+        Filters out non-letters and separates timings from letters.
+
+        Parameters
+        ----------
+        - triggers: triggers e.g. [['A', 0.5], ...]
+        as letter and flash time for the letter
+        - target_info: target information about the stimuli;
+        ex. ['nontarget', 'nontarget', ...]
+
+        Returns
+        -------
+        (letters, times, target_info)
+        """
+        letters = []
+        times = []
+        target_types = []
+
+        for i, (letter, stamp) in enumerate(triggers):
+            if letter not in self.nonletters:
+                letters.append(letter)
+                times.append(stamp)
+                target_types.append(target_info[i])
+
+        # Raise an error if the stimuli includes unexpected terms
+        if not set(letters).issubset(self.valid_targets):
+            invalid = set(letters).difference(self.valid_targets)
+            error_message = f'unexpected letters received in copy phrase: {invalid}'
+            log.error(error_message)
+            raise BciPyCoreException(error_message)
+
+        return letters, times, target_types
+
+    def initialize_series(self) -> Tuple[bool, InquirySchedule]:
+        """If a decision is made initializes the next series."""
+        assert self.lmodel, "Language model must be initialized."
+
+        try:
+            # First, reset the history for this new series
+            self.conjugator.reset_history()
+
+            # Get the displayed state
+            update = self.decision_maker.displayed_state
+            log.info(f"Querying language model: '{update}'")
+
+            # update the lmodel and get back the priors
+            lm_letter_prior = self.lmodel.predict(list(update))
+
+            if BACKSPACE_CHAR in self.alp:
+                # Apply configured backspace probability.
+                sym = (BACKSPACE_CHAR, self.backspace_prob)
+                lm_letter_prior = with_min_prob(lm_letter_prior, sym)
+
+            # convert to format needed for evidence fusion;
+            # probability value only in alphabet order.
+            prior = [
+                prior_prob for alp_letter in self.alp
+                for prior_sym, prior_prob in lm_letter_prior
+                if alp_letter == prior_sym
+            ]
+
+            # display histogram of LM probabilities
+            log.debug(histogram(lm_letter_prior))
+
+            # Try fusing the lmodel evidence
+            try:
+                prob_dist = self.conjugator.update_and_fuse(
+                    {EvidenceType.LM: np.array(prior)})
+            except Exception as fusion_error:
+                log.exception(f'Error fusing language model evidence!: {fusion_error}')
+                raise BciPyCoreException(fusion_error) from fusion_error
+
+            # Get decision maker to give us back some decisions and stimuli
+            is_accepted, sti = self.decision_maker.decide(prob_dist)
+
+        except Exception as init_series_error:
+            log.exception(f'Error in initialize_series: {init_series_error}')
+            raise BciPyCoreException(init_series_error) from init_series_error
+
+        return is_accepted, sti
```

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/exceptions.py` & `bcipy-2.0.1rc2/bcipy/helpers/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,26 +7,14 @@
 
     def __init__(self, message, errors=None):
         super().__init__(message)
         self.message = message
         self.errors = errors
 
 
-class SignalException(BciPyCoreException):
-    """
-    Signal Exception.
-
-    Thrown when signal module encounters an error.
-    """
-
-    def __init__(self, message, errors=None):
-        super().__init__(message)
-        self.errors = errors
-
-
 class FieldException(BciPyCoreException):
     """Field Exception.
 
     Thrown when there is an exception relating to experimental fields.
     """
     ...
 
@@ -84,21 +72,7 @@
 
 
 class TaskConfigurationException(BciPyCoreException):
     """Task Configuration Exception.
 
     Thrown when attempting to run a task with invalid configurations"""
     ...
-
-
-class InvalidLanguageModelException(BciPyCoreException):
-    """Invalid Language Model Exception.
-
-    Thrown when attempting to load a language model from an invalid path"""
-    ...
-
-
-class KenLMInstallationException(BciPyCoreException):
-    """KenLM Installation Exception.
-
-    Thrown when attempting to import kenlm without installing the module"""
-    ...
```

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/language_model.py` & `bcipy-2.0.1rc2/bcipy/helpers/language_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 """Helper functions for language model use."""
 import math
 import inspect
 from typing import Dict, List, Tuple
 import numpy as np
 from bcipy.language.main import LanguageModel, ResponseType
-from bcipy.helpers.symbols import alphabet
+from bcipy.helpers.task import alphabet
 # pylint: disable=unused-import
 # flake8: noqa
-
-"""Only imported models will be included in language_models_by_name"""
-from bcipy.language.model.uniform import UniformLanguageModel
-from bcipy.language.model.causal import CausalLanguageModel
-from bcipy.language.model.mixture import MixtureLanguageModel
-from bcipy.language.model.kenlm import KenLMLanguageModel
-from bcipy.language.model.unigram import UnigramLanguageModel
-
+from bcipy.language.uniform import UniformLanguageModel
 # flake8: noqa
-from bcipy.helpers.exceptions import InvalidLanguageModelException
+from bcipy.language.model.gpt2 import GPT2LanguageModel
 
 
 def language_models_by_name() -> Dict[str, LanguageModel]:
     """Returns available language models indexed by name."""
     return {lm.name(): lm for lm in LanguageModel.__subclasses__()}
 
 
@@ -33,15 +26,14 @@
         parameters : dict
             configuration details and path locations
 
     Returns
     -------
         instance of a LanguageModel
     """
-
     language_models = language_models_by_name()
     model = language_models[parameters.get("lang_model_type", "UNIFORM")]
 
     # introspect the model arguments to determine what parameters to pass.
     args = inspect.signature(model).parameters.keys()
 
     # select the relevant parameters into a dict.
```

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/list.py` & `bcipy-2.0.1rc2/bcipy/helpers/list.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/load.py` & `bcipy-2.0.1rc2/bcipy/helpers/load.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,290 +1,283 @@
-import json
-import logging
-import os
-from pathlib import Path
-from shutil import copyfile
-from time import localtime, strftime
-from typing import Any, Dict, List, Tuple
-
-from bcipy.config import (
-    ROOT,
-    DEFAULT_ENCODING,
-    DEFAULT_EXPERIMENT_PATH,
-    DEFAULT_PARAMETERS_PATH,
-    DEFAULT_FIELD_PATH,
-    EXPERIMENT_FILENAME,
-    FIELD_FILENAME)
-from bcipy.gui.file_dialog import ask_directory, ask_filename
-from bcipy.preferences import preferences
-from bcipy.helpers.exceptions import (BciPyCoreException,
-                                      InvalidExperimentException)
-from bcipy.helpers.parameters import Parameters
-from bcipy.helpers.raw_data import RawData
-from bcipy.signal.model import SignalModel
-
-log = logging.getLogger(__name__)
-
-
-def copy_parameters(path: str = DEFAULT_PARAMETERS_PATH,
-                    destination: str = None) -> str:
-    """Creates a copy of the given configuration (parameters.json) to the
-    given directory and returns the path.
-
-    Parameters:
-    -----------
-        path: str - optional path of parameters file to copy; used default if not provided.
-        destination: str - optional destination directory; default is the same
-          directory as the default parameters.
-    Returns:
-    --------
-        path to the new file.
-    """
-    default_dir = str(Path(DEFAULT_PARAMETERS_PATH).parent)
-
-    destination = default_dir if destination is None else destination
-    filename = strftime('parameters_%Y-%m-%d_%Hh%Mm%Ss.json', localtime())
-
-    path = str(Path(destination, filename))
-    copyfile(DEFAULT_PARAMETERS_PATH, path)
-    return path
-
-
-def load_experiments(path: str = f'{DEFAULT_EXPERIMENT_PATH}/{EXPERIMENT_FILENAME}') -> dict:
-    """Load Experiments.
-
-    PARAMETERS
-    ----------
-    :param: path: string path to the experiments file.
-
-    Returns
-    -------
-        A dictionary of experiments, with the following format:
-            { name: { fields : {name: '', required: bool, anonymize: bool}, summary: '' } }
-
-    """
-    with open(path, 'r', encoding=DEFAULT_ENCODING) as json_file:
-        return json.load(json_file)
-
-
-def extract_mode(bcipy_data_directory: str) -> str:
-    """Extract Mode.
-
-    This method extracts the task mode from a BciPy data save directory. This is important for
-        trigger conversions and extracting targeteness.
-
-    *note*: this is not compatible with older versions of BciPy (pre 1.5.0) where
-        the tasks and modes were considered together using integers (1, 2, 3).
-
-    PARAMETERS
-    ----------
-    :param: bcipy_data_directory: string path to the data directory
-    """
-    directory = bcipy_data_directory.lower()
-    if 'calibration' in directory:
-        return 'calibration'
-    elif 'copy' in directory:
-        return 'copy_phrase'
-    raise BciPyCoreException(f'No valid mode could be extracted from [{directory}]')
-
-
-def load_fields(path: str = f'{DEFAULT_FIELD_PATH}/{FIELD_FILENAME}') -> dict:
-    """Load Fields.
-
-    PARAMETERS
-    ----------
-    :param: path: string path to the fields file.
-
-    Returns
-    -------
-        A dictionary of fields, with the following format:
-            {
-                "field_name": {
-                    "help_text": "",
-                    "type": ""
-            }
-
-    """
-    with open(path, 'r', encoding=DEFAULT_ENCODING) as json_file:
-        return json.load(json_file)
-
-
-def load_experiment_fields(experiment: dict) -> list:
-    """Load Experiment Fields.
-
-    {
-        'fields': [{}, {}],
-        'summary': ''
-    }
-
-    Using the experiment dictionary, loop over the field keys and put them in a list.
-    """
-    if isinstance(experiment, dict):
-        try:
-            return [name for field in experiment['fields'] for name in field.keys()]
-        except KeyError:
-            raise InvalidExperimentException(
-                'Experiment is not formatted correctly. It should be passed as a dictionary with the fields and'
-                f' summary keys. Fields is a list of dictionaries. Summary is a string. \n experiment=[{experiment}]')
-    raise TypeError('Unsupported experiment type. It should be passed as a dictionary with the fields and summary keys')
-
-
-def load_json_parameters(path: str, value_cast: bool = False) -> Parameters:
-    """Load JSON Parameters.
-
-    Given a path to a json of parameters, convert to a dictionary and optionally
-        cast the type.
-
-    Expects the following format:
-    "fake_data": {
-        "value": "true",
-        "section": "bci_config",
-        "readableName": "Fake Data Sessions",
-        "helpTip": "If true, fake data server used",
-        "recommended_values": "",
-        "type": "bool"
-        }
-
-    PARAMETERS
-    ----------
-    :param: path: string path to the parameters file.
-    :param: value_case: True/False cast values to specified type.
-
-    Returns
-    -------
-        a Parameters object that behaves like a dict.
-    """
-    return Parameters(source=path, cast_values=value_cast)
-
-
-def load_experimental_data() -> str:
-    filename = ask_directory()  # show dialog box and return the path
-    log.debug("Loaded Experimental Data From: %s" % filename)
-    return filename
-
-
-def load_signal_model(model_class: SignalModel,
-                      model_kwargs: Dict[str, Any], filename: str = None) -> Tuple[SignalModel, str]:
-    """Construct the specified model and load pretrained parameters.
-
-    Args:
-        model_class (SignalModel, optional): Model class to construct.
-        model_kwargs (dict, optional): Keyword arguments for constructing model.
-        filename (str, optional): Location of pretrained model parameters.
-
-    Returns:
-        SignalModel: Model after loading pretrained parameters.
-    """
-    # use python's internal gui to call file explorers and get the filename
-    if not filename or Path(filename).is_dir():
-        directory = filename or preferences.signal_model_directory
-        filename = ask_filename('*.pkl', directory)
-
-        # update preferences
-        path = Path(filename)
-        if path.is_file():
-            preferences.signal_model_directory = str(path.parent)
-
-    # load the signal_model with pickle
-    signal_model = model_class(**model_kwargs)
-    signal_model.load(filename)
-
-    log.info(f'Loaded signal model from {filename}')
-
-    return signal_model, filename
-
-
-def choose_csv_file(filename: str = None) -> str:
-    """GUI prompt to select a csv file from the file system.
-
-    Parameters
-    ----------
-    - filename : optional filename to use; if provided the GUI is not shown.
-
-    Returns
-    -------
-    file name of selected file; throws an exception if the file is not a csv.
-    """
-    if not filename:
-        filename = ask_filename('*.csv')
-
-    # get the last part of the path to determine file type
-    file_name = filename.split('/')[-1]
-
-    if 'csv' not in file_name:
-        raise Exception(
-            'File type unrecognized. Please use a supported csv type')
-
-    return filename
-
-
-def load_raw_data(filename: str) -> RawData:
-    """Reads the data (.csv) file written by data acquisition.
-
-    Parameters
-    ----------
-    - filename : path to the serialized data (csv file)
-
-    Returns
-    -------
-    RawData object with data held in memory
-    """
-    return RawData.load(filename)
-
-
-def load_txt_data() -> str:
-    filename = ask_filename('*.txt')  # show dialog box and return the path
-    file_name = filename.split('/')[-1]
-
-    if 'txt' not in file_name:
-        raise Exception(
-            'File type unrecognized. Please use a supported text type')
-
-    return filename
-
-
-def load_users(data_save_loc) -> List[str]:
-    """Load Users.
-
-    Loads user directory names below experiments from the data path defined and returns them as a list.
-    If the save data directory is not found, this method returns an empty list assuming no experiments
-    have been run yet.
-    """
-    # build a saved users list, pull out the data save location from parameters
-    saved_users = []
-
-    # check the directory is valid, if it is, set path as data save location
-    if os.path.isdir(data_save_loc):
-        path = data_save_loc
-
-    # check the directory is valid after adding bcipy, if it is, set path as data save location
-    elif os.path.isdir(f'{ROOT}/{data_save_loc}'):
-        path = f'{ROOT}/{data_save_loc}'
-
-    else:
-        log.info(f'User save data location not found at [{data_save_loc}]! Returning empty user list.')
-        return saved_users
-
-    # grab all experiments in the directory and iterate over them to get the users
-    experiments = fast_scandir(path, return_path=True)
-
-    for experiment in experiments:
-        users = fast_scandir(experiment, return_path=False)
-        # If it is a new user, append it to the saved_user list
-        for user in users:
-            if user not in saved_users:
-                saved_users.append(user)
-
-    return saved_users
-
-
-def fast_scandir(directory_name: str, return_path: bool = True) -> List[str]:
-    """Fast Scan Directory.
-
-    directory_name: name of the directory to be scanned
-    return_path: whether or not to return the scanned directories as a relative path or name.
-        False will return the directory name only.
-    """
-    if return_path:
-        return [f.path for f in os.scandir(directory_name) if f.is_dir()]
-
-    return [f.name for f in os.scandir(directory_name) if f.is_dir()]
+import json
+import logging
+import os
+from pathlib import Path
+from shutil import copyfile
+from time import localtime, strftime
+from typing import Any, Dict, List, Tuple
+
+from bcipy.config import (
+    ROOT,
+    DEFAULT_ENCODING,
+    DEFAULT_EXPERIMENT_PATH,
+    DEFAULT_PARAMETERS_PATH,
+    DEFAULT_FIELD_PATH,
+    EXPERIMENT_FILENAME,
+    FIELD_FILENAME)
+from bcipy.gui.file_dialog import ask_directory, ask_filename
+from bcipy.helpers.exceptions import (BciPyCoreException,
+                                      InvalidExperimentException)
+from bcipy.helpers.parameters import Parameters
+from bcipy.helpers.raw_data import RawData
+from bcipy.signal.model import SignalModel
+
+log = logging.getLogger(__name__)
+
+
+def copy_parameters(path: str = DEFAULT_PARAMETERS_PATH,
+                    destination: str = None) -> str:
+    """Creates a copy of the given configuration (parameters.json) to the
+    given directory and returns the path.
+
+    Parameters:
+    -----------
+        path: str - optional path of parameters file to copy; used default if not provided.
+        destination: str - optional destination directory; default is the same
+          directory as the default parameters.
+    Returns:
+    --------
+        path to the new file.
+    """
+    default_dir = str(Path(DEFAULT_PARAMETERS_PATH).parent)
+
+    destination = default_dir if destination is None else destination
+    filename = strftime('parameters_%Y-%m-%d_%Hh%Mm%Ss.json', localtime())
+
+    path = str(Path(destination, filename))
+    copyfile(DEFAULT_PARAMETERS_PATH, path)
+    return path
+
+
+def load_experiments(path: str = f'{DEFAULT_EXPERIMENT_PATH}/{EXPERIMENT_FILENAME}') -> dict:
+    """Load Experiments.
+
+    PARAMETERS
+    ----------
+    :param: path: string path to the experiments file.
+
+    Returns
+    -------
+        A dictionary of experiments, with the following format:
+            { name: { fields : {name: '', required: bool, anonymize: bool}, summary: '' } }
+
+    """
+    with open(path, 'r', encoding=DEFAULT_ENCODING) as json_file:
+        return json.load(json_file)
+
+
+def extract_mode(bcipy_data_directory: str) -> str:
+    """Extract Mode.
+
+    This method extracts the task mode from a BciPy data save directory. This is important for
+        trigger conversions and extracting targeteness.
+
+    *note*: this is not compatible with older versions of BciPy (pre 1.5.0) where
+        the tasks and modes were considered together using integers (1, 2, 3).
+
+    PARAMETERS
+    ----------
+    :param: bcipy_data_directory: string path to the data directory
+    """
+    directory = bcipy_data_directory.lower()
+    if 'calibration' in directory:
+        return 'calibration'
+    elif 'copy' in directory:
+        return 'copy_phrase'
+    raise BciPyCoreException(f'No valid mode could be extracted from [{directory}]')
+
+
+def load_fields(path: str = f'{DEFAULT_FIELD_PATH}/{FIELD_FILENAME}') -> dict:
+    """Load Fields.
+
+    PARAMETERS
+    ----------
+    :param: path: string path to the fields file.
+
+    Returns
+    -------
+        A dictionary of fields, with the following format:
+            {
+                "field_name": {
+                    "help_text": "",
+                    "type": ""
+            }
+
+    """
+    with open(path, 'r', encoding=DEFAULT_ENCODING) as json_file:
+        return json.load(json_file)
+
+
+def load_experiment_fields(experiment: dict) -> list:
+    """Load Experiment Fields.
+
+    {
+        'fields': [{}, {}],
+        'summary': ''
+    }
+
+    Using the experiment dictionary, loop over the field keys and put them in a list.
+    """
+    if isinstance(experiment, dict):
+        try:
+            return [name for field in experiment['fields'] for name in field.keys()]
+        except KeyError:
+            raise InvalidExperimentException(
+                'Experiment is not formatted correctly. It should be passed as a dictionary with the fields and'
+                f' summary keys. Fields is a list of dictionaries. Summary is a string. \n experiment=[{experiment}]')
+    raise TypeError('Unsupported experiment type. It should be passed as a dictionary with the fields and summary keys')
+
+
+def load_json_parameters(path: str, value_cast: bool = False) -> Parameters:
+    """Load JSON Parameters.
+
+    Given a path to a json of parameters, convert to a dictionary and optionally
+        cast the type.
+
+    Expects the following format:
+    "fake_data": {
+        "value": "true",
+        "section": "bci_config",
+        "readableName": "Fake Data Sessions",
+        "helpTip": "If true, fake data server used",
+        "recommended_values": "",
+        "type": "bool"
+        }
+
+    PARAMETERS
+    ----------
+    :param: path: string path to the parameters file.
+    :param: value_case: True/False cast values to specified type.
+
+    Returns
+    -------
+        a Parameters object that behaves like a dict.
+    """
+    return Parameters(source=path, cast_values=value_cast)
+
+
+def load_experimental_data() -> str:
+    filename = ask_directory()  # show dialog box and return the path
+    log.debug("Loaded Experimental Data From: %s" % filename)
+    return filename
+
+
+def load_signal_model(model_class: SignalModel,
+                      model_kwargs: Dict[str, Any], filename: str = None) -> Tuple[SignalModel, str]:
+    """Construct the specified model and load pretrained parameters.
+
+    Args:
+        model_class (SignalModel, optional): Model class to construct.
+        model_kwargs (dict, optional): Keyword arguments for constructing model.
+        filename (str, optional): Location of pretrained model parameters.
+
+    Returns:
+        SignalModel: Model after loading pretrained parameters.
+    """
+    # use python's internal gui to call file explorers and get the filename
+    if not filename or Path(filename).is_dir():
+        filename = ask_filename('*.pkl', filename)
+
+    # load the signal_model with pickle
+    signal_model = model_class(**model_kwargs)
+    signal_model.load(filename)
+
+    log.info(f'Loaded signal model from {filename}')
+
+    return signal_model, filename
+
+
+def choose_csv_file(filename: str = None) -> str:
+    """GUI prompt to select a csv file from the file system.
+
+    Parameters
+    ----------
+    - filename : optional filename to use; if provided the GUI is not shown.
+
+    Returns
+    -------
+    file name of selected file; throws an exception if the file is not a csv.
+    """
+    if not filename:
+        filename = ask_filename('*.csv')
+
+    # get the last part of the path to determine file type
+    file_name = filename.split('/')[-1]
+
+    if 'csv' not in file_name:
+        raise Exception(
+            'File type unrecognized. Please use a supported csv type')
+
+    return filename
+
+
+def load_raw_data(filename: str) -> RawData:
+    """Reads the data (.csv) file written by data acquisition.
+
+    Parameters
+    ----------
+    - filename : path to the serialized data (csv file)
+
+    Returns
+    -------
+    RawData object with data held in memory
+    """
+    return RawData.load(filename)
+
+
+def load_txt_data() -> str:
+    filename = ask_filename('*.txt')  # show dialog box and return the path
+    file_name = filename.split('/')[-1]
+
+    if 'txt' not in file_name:
+        raise Exception(
+            'File type unrecognized. Please use a supported text type')
+
+    return filename
+
+
+def load_users(data_save_loc) -> List[str]:
+    """Load Users.
+
+    Loads user directory names below experiments from the data path defined and returns them as a list.
+    If the save data directory is not found, this method returns an empty list assuming no experiments
+    have been run yet.
+    """
+    # build a saved users list, pull out the data save location from parameters
+    saved_users = []
+
+    # check the directory is valid, if it is, set path as data save location
+    if os.path.isdir(data_save_loc):
+        path = data_save_loc
+
+    # check the directory is valid after adding bcipy, if it is, set path as data save location
+    elif os.path.isdir(f'{ROOT}/{data_save_loc}'):
+        path = f'{ROOT}/{data_save_loc}'
+
+    else:
+        log.info(f'User save data location not found at [{data_save_loc}]! Returning empty user list.')
+        return saved_users
+
+    # grab all experiments in the directory and iterate over them to get the users
+    experiments = fast_scandir(path, return_path=True)
+
+    for experiment in experiments:
+        users = fast_scandir(experiment, return_path=False)
+        # If it is a new user, append it to the saved_user list
+        for user in users:
+            if user not in saved_users:
+                saved_users.append(user)
+
+    return saved_users
+
+
+def fast_scandir(directory_name: str, return_path: bool = True) -> List[str]:
+    """Fast Scan Directory.
+
+    directory_name: name of the directory to be scanned
+    return_path: whether or not to return the scanned directories as a relative path or name.
+        False will return the directory name only.
+    """
+    if return_path:
+        return [f.path for f in os.scandir(directory_name) if f.is_dir()]
+
+    return [f.name for f in os.scandir(directory_name) if f.is_dir()]
```

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/parameters.py` & `bcipy-2.0.1rc2/bcipy/helpers/parameters.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/save.py` & `bcipy-2.0.1rc2/bcipy/helpers/save.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,24 @@
+from bcipy.acquisition.devices import DeviceSpec
+from bcipy.helpers.validate import validate_experiments
 import errno
-import json
 import os
-from pathlib import Path
-from shutil import copyfile
 from time import localtime, strftime
-from typing import Any, List
+from shutil import copyfile
+from pathlib import Path
+import json
 
-from bcipy.acquisition.devices import DeviceSpec
-from bcipy.config import (DEFAULT_ENCODING, DEFAULT_EXPERIMENT_ID,
-                          DEFAULT_LM_PARAMETERS_FILENAME,
-                          DEFAULT_LM_PARAMETERS_PATH,
-                          DEFAULT_PARAMETER_FILENAME)
-from bcipy.helpers.validate import validate_experiments
+from bcipy.config import DEFAULT_ENCODING, DEFAULT_EXPERIMENT_ID, DEFAULT_PARAMETER_FILENAME
 
 
-def save_json_data(data: Any, location: str, name: str) -> str:
+def save_json_data(data: dict, location: str, name: str) -> str:
     """
     Writes Parameters as a json file.
 
-        data: any data that can be dumped as json
+        parameters[dict]: dict of configuration
         location[str]: directory in which to save
         name[str]: optional name of file; default is parameters.json
 
     Returns path of saved file
     """
     path = Path(location, name)
     with open(Path(location, name), 'w', encoding=DEFAULT_ENCODING) as json_file:
@@ -79,34 +75,30 @@
 
         # since this is only called on init, we can make another folder run
         os.makedirs(save_directory)
         os.makedirs(os.path.join(save_directory, 'logs'), exist_ok=True)
 
     copyfile(parameters, Path(save_directory, DEFAULT_PARAMETER_FILENAME))
 
-    copyfile(DEFAULT_LM_PARAMETERS_PATH, Path(save_directory, DEFAULT_LM_PARAMETERS_FILENAME))
-
     return save_directory
 
 
-def save_device_specs(device_specs: List[DeviceSpec], location: str,
-                      name: str) -> str:
+def save_device_spec(device_spec: DeviceSpec, location: str, name: str) -> str:
     """
     Save device spec to a json file.
 
     Parameters:
         device_spec (DeviceSpec): device spec to save
         location (str): location to save the file
         name (str): name of the file to be saved
 
     Returns:
         str: path to the saved file
     """
-    return save_json_data([spec.to_dict() for spec in device_specs], location,
-                          name)
+    return save_json_data(device_spec.to_dict(), location, name)
 
 
 def _save_session_related_data(file, session_dictionary):
     """
     Save Session Related Data.
     Parameters
     ----------
```

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/session.py` & `bcipy-2.0.1rc2/bcipy/helpers/session.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/stimuli.py` & `bcipy-2.0.1rc2/bcipy/helpers/stimuli.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from mne import Annotations, Epochs
 from mne.io import RawArray
 import mne
 
 
 log = logging.getLogger(__name__)
 DEFAULT_FIXATION_PATH = 'bcipy/static/images/main/PLUS.png'
-DEFAULT_TEXT_FIXATION = '+'
 
 
 class StimuliOrder(Enum):
     """Stimuli Order.
 
     Enum to define the ordering of stimuli for inquiry.
     """
@@ -164,70 +163,41 @@
             first_trigger = trials_within_inquiry[0][1]
 
             trial_triggers = []
             for trial_idx, (trial_label, trigger) in enumerate(trials_within_inquiry):
                 if trial_label == target_label:
                     labels[inquiry_idx, trial_idx] = 1
 
-                # If prestimulus buffer is used, we add it here so that trigger timings will
+                # If presimulus buffer is used, we add it here so that trigger timings will
                 # still line up with trial onset
                 trial_triggers.append((trigger - first_trigger) + prestimulus_samples)
             reshaped_trigger_timing.append(trial_triggers)
             start = first_trigger - prestimulus_samples
             stop = first_trigger + num_samples_per_inq + buffer_samples
             reshaped_data.append(eeg_data[:, start:stop])
 
         return np.stack(reshaped_data, 1), labels, reshaped_trigger_timing
 
     @staticmethod
-    def extract_trials(
-            inquiries: np.ndarray,
-            samples_per_trial: int,
-            inquiry_timing: List[List[float]],
-            prestimulus_samples: int = 0) -> np.ndarray:
+    def extract_trials(inquiries, samples_per_trial, inquiry_timing, downsample_rate=1):
         """Extract Trials.
 
-        After using the InquiryReshaper, it may be necessary to further trial the data for processing.
+        After using the InquiryReshaper, it may be necessary to futher trial the data for processing.
         Using the number of samples and inquiry timing, the data is reshaped from Channels, Inquiry, Samples to
         Channels, Trials, Samples. These should match with the trials extracted from the TrialReshaper given the same
         slicing parameters.
-
-        Parameters
-        ----------
-        inquiries : np.ndarray
-            shape (Channels, Inquiries, Samples)
-        samples_per_trial : int
-            number of samples per trial
-        inquiry_timing : List[List[float]]
-            For each inquiry, a list of the sample index where each trial begins
-        prestimulus_samples : int, optional
-            Number of samples to move the start of each trial in each inquiry, by default 0.
-            This is useful if wanting to use baseline intervals before the trial onset, along with the trial data.
-
-        Returns
-        -------
-        np.ndarray
-            shape (Channels, Trials, Samples)
         """
         new_trials = []
         num_inquiries = inquiries.shape[1]
         for inquiry_idx, timing in zip(range(num_inquiries), inquiry_timing):  # C x I x S
 
-            # time == samples from the start of the inquiry
             for time in timing:
-                start = time - prestimulus_samples
-                end = time + samples_per_trial
-
-                try:
-                    new_trials.append(inquiries[:, inquiry_idx, start:end])
-                except IndexError:
-                    raise BciPyCoreException(
-                        f'InquiryReshaper.extract_trials: index out of bounds. \n'
-                        f'Inquiry: [{inquiry_idx}] from {start}:{end}. init_time: {time}, '
-                        f'prestimulus_samples: {prestimulus_samples}, samples_per_trial: {samples_per_trial} \n')
+                time = time // downsample_rate
+                y = time + samples_per_trial
+                new_trials.append(inquiries[:, inquiry_idx, time:y])
         return np.stack(new_trials, 1)  # C x T x S
 
 
 class TrialReshaper(Reshaper):
     def __call__(self,
                  trial_targetness_label: list,
                  timing_info: list,
@@ -236,30 +206,28 @@
                  offset: float = 0,
                  channel_map: List[int] = None,
                  poststimulus_length: float = 0.5,
                  prestimulus_length: float = 0.0,
                  target_label: str = "target") -> Tuple[np.ndarray, np.ndarray]:
         """Extract trial data and labels.
 
-        Parameters
-        ----------
+        Args:
             trial_targetness_label (list): labels each trial as "target", "non-target", "first_pres_target", etc
             timing_info (list): Timestamp of each event in seconds
             eeg_data (np.ndarray): shape (channels, samples) preprocessed EEG data
             sample_rate (int): sample rate of preprocessed EEG data
             trials_per_inquiry (int, optional): unused, kept here for consistent interface with `inquiry_reshaper`
             offset (float, optional): Any calculated or hypothesized offsets in timings.
                 Defaults to 0.
             channel_map (List, optional): Describes which channels to include or discard.
                 Defaults to None; all channels will be used.
             poststimulus_length (float, optional): [description]. Defaults to 0.5.
             target_label (str): label of target symbol. Defaults to "target"
 
-        Returns
-        -------
+        Returns:
             trial_data (np.ndarray): shape (channels, trials, samples) reshaped data
             labels (np.ndarray): integer label for each trial
         """
         # Remove the channels that we are not interested in
         if channel_map:
             channels_to_remove = [idx for idx, value in enumerate(channel_map) if value == 0]
             eeg_data = np.delete(eeg_data, channels_to_remove, axis=0)
@@ -280,24 +248,14 @@
 
             # For every channel append filtered channel data to trials
             reshaped_trials.append(eeg_data[:, trigger - prestim_samples: trigger + poststim_samples])
 
         return np.stack(reshaped_trials, 1), targetness_labels
 
 
-def update_inquiry_timing(timing: List[List[float]], downsample: int) -> List[List[float]]:
-    """Update inquiry timing to reflect downsampling."""
-
-    for i, inquiry in enumerate(timing):
-        for j, time in enumerate(inquiry):
-            timing[i][j] = time // downsample
-
-    return timing
-
-
 def mne_epochs(mne_data: RawArray, trigger_timing: List[float],
                trial_length: float, trigger_labels: List[int]) -> Epochs:
     """MNE Epochs.
 
     Using an MNE RawArray, reshape the data given trigger information. If two labels present [0, 1],
     each may be accessed by numbered order. Ex. first_class = epochs['1'], second_class = epochs['2']
     """
@@ -319,30 +277,27 @@
 def inq_generator(query: List[str],
                   timing: List[float] = [1, 0.2],
                   color: List[str] = ['red', 'white'],
                   inquiry_count: int = 1,
                   stim_jitter: float = 0,
                   stim_order: StimuliOrder = StimuliOrder.RANDOM,
                   is_txt: bool = True) -> InquirySchedule:
-    """Given the query set, prepares the stimuli, color and timing
-
-    Parameters
-    ----------
-        query(list[str]): list of queries to be shown
-        timing(list[float]): Task specific timing for generator
-        color(list[str]): Task specific color for generator
-            First element is the target, second element is the fixation
-            Observe that [-1] element represents the trial information
-    Return
-    ------
-        schedule_inq(tuple(
-            samples[list[list[str]]]: list of inquiries
-            timing(list[list[float]]): list of timings
-            color(list(list[str])): list of colors)): scheduled inquiries
-    """
+    """ Given the query set, prepares the stimuli, color and timing
+        Args:
+            query(list[str]): list of queries to be shown
+            timing(list[float]): Task specific timing for generator
+            color(list[str]): Task specific color for generator
+                First element is the target, second element is the fixation
+                Observe that [-1] element represents the trial information
+        Return:
+            schedule_inq(tuple(
+                samples[list[list[str]]]: list of inquiries
+                timing(list[list[float]]): list of timings
+                color(list(list[str])): list of colors)): scheduled inquiries
+            """
 
     if stim_order == StimuliOrder.ALPHABETICAL:
         query = alphabetize(query)
     else:
         random.shuffle(query)
 
     stim_length = len(query)
@@ -370,28 +325,25 @@
 
 def best_selection(selection_elements: list,
                    val: list,
                    len_query: int,
                    always_included: List[str] = None) -> list:
     """Best Selection.
 
-    Given set of elements and a value function over the set, picks the len_query
+     given set of elements and a value function over the set, picks the len_query
         number of elements with the best value.
 
-    Parameters
-    ----------
-        selection_elements(list[str]): the set of elements
-        val(list[float]): values for the corresponding elements
-        len_query(int): number of elements to be picked from the set
-        always_included(list[str]): subset of elements that should always be
-            included in the result. Defaults to None.
-    Return
-    ------
-        best_selection(list[str]): elements from selection_elements with the best values
-    """
+        Args:
+            selection_elements(list[str]): the set of elements
+            val(list[float]): values for the corresponding elements
+            len_query(int): number of elements to be picked from the set
+            always_included(list[str]): subset of elements that should always be
+                included in the result. Defaults to None.
+        Return:
+            best_selection(list[str]): elements from selection_elements with the best values """
 
     always_included = always_included or []
     # pick the top n items sorted by value in decreasing order
     elem_val = dict(zip(selection_elements, val))
     best = sorted(selection_elements, key=elem_val.get, reverse=True)[0:len_query]
 
     replacements = [
@@ -411,37 +363,34 @@
                            stim_number: int = 1,
                            stim_length: int = 10,
                            stim_order: StimuliOrder = StimuliOrder.RANDOM,
                            is_txt: bool = True,
                            inq_constants: List[str] = None) -> InquirySchedule:
     """Best Case RSVP Inquiry Generation.
 
-    Generates RSVPKeyboard inquiry by picking n-most likely letters.
-
-    Parameters
-    ----------
-        alp(list[str]): alphabet (can be arbitrary)
-        session_stimuli(ndarray[float]): quantifier metric for query selection
-            dim(session_stimuli) = card(alp)!
-        timing(list[float]): Task specific timing for generator
-        color(list[str]): Task specific color for generator
-            First element is the target, second element is the fixation
-            Observe that [-1] element represents the trial information
-        stim_number(int): number of random stimuli to be created
-        stim_length(int): number of trials in a inquiry
-        stim_order(StimuliOrder): ordering of stimuli in the inquiry
-        inq_constants(list[str]): list of letters that should always be
-            included in every inquiry. If provided, must be alp items.
-    Return
-    ------
-        schedule_inq(tuple(
-            samples[list[list[str]]]: list of inquiries
-            timing(list[list[float]]): list of timings
-            color(list(list[str])): list of colors)): scheduled inquiries
-    """
+    generates RSVPKeyboard inquiry by picking n-most likely letters.
+        Args:
+            alp(list[str]): alphabet (can be arbitrary)
+            session_stimuli(ndarray[float]): quantifier metric for query selection
+                dim(session_stimuli) = card(alp)!
+            timing(list[float]): Task specific timing for generator
+            color(list[str]): Task specific color for generator
+                First element is the target, second element is the fixation
+                Observe that [-1] element represents the trial information
+            stim_number(int): number of random stimuli to be created
+            stim_length(int): number of trials in a inquiry
+            stim_order(StimuliOrder): ordering of stimuli in the inquiry
+            inq_constants(list[str]): list of letters that should always be
+                included in every inquiry. If provided, must be alp items.
+        Return:
+            schedule_inq(tuple(
+                samples[list[list[str]]]: list of inquiries
+                timing(list[list[float]]): list of timings
+                color(list(list[str])): list of colors)): scheduled inquiries
+            """
 
     if len(alp) != len(session_stimuli):
         raise BciPyCoreException((
             f'Missing information about alphabet.'
             f'len(alp):{len(alp)} and len(session_stimuli):{len(session_stimuli)} should be same!'))
 
     if inq_constants and not set(inq_constants).issubset(alp):
@@ -490,38 +439,34 @@
         stim_order: StimuliOrder = StimuliOrder.RANDOM,
         target_positions: TargetPositions = TargetPositions.RANDOM,
         nontarget_inquiries: int = 10,
         is_txt: bool = True) -> InquirySchedule:
     """Calibration Inquiry Generator.
 
     Generates inquiries with target letters in all possible positions.
-
-    Parameters
-    ----------
-        alp(list[str]): stimuli
-        timing(list[float]): Task specific timing for generator.
-            [target, fixation, stimuli]
-        jitter(int): jitter for stimuli timing. If None, no jitter is applied.
-        color(list[str]): Task specific color for generator
-            [target, fixation, stimuli]
-        stim_number(int): number of trials in a inquiry
-        stim_length(int): number of random stimuli to be created
-        stim_order(StimuliOrder): ordering of stimuli in the inquiry
-        target_positions(TargetPositions): positioning of targets to select for the inquiries
-        nontarget_inquiries(int): percentage of inquiries for which target letter flashed is not in inquiry
-        is_txt(bool): whether or not the stimuli type is text. False would be an image stimuli.
-
-    Return
-    ------
-        schedule_inq(tuple(
-            samples[list[list[str]]]: list of inquiries
-            timing(list[list[float]]): list of timings
-            color(list(list[str])): list of colors)): scheduled inquiries
+        Args:
+            alp(list[str]): stimuli
+            timing(list[float]): Task specific timing for generator.
+                [target, fixation, stimuli]
+            jitter(int): jitter for stimuli timing. If None, no jitter is applied.
+            color(list[str]): Task specific color for generator
+                [target, fixation, stimuli]
+            stim_number(int): number of trials in a inquiry
+            stim_length(int): number of random stimuli to be created
+            stim_order(StimuliOrder): ordering of stimuli in the inquiry
+            target_positions(TargetPositions): positioning of targets to select for the inquiries
+            nontarget_inquiries(int): percentage of inquiries for which target letter flashed is not in inquiry
+            is_txt(bool): whether or not the stimuli type is text. False would be an image stimuli.
+        Return:
+            schedule_inq(tuple(
+                samples[list[list[str]]]: list of inquiries
+                timing(list[list[float]]): list of timings
+                color(list(list[str])): list of colors)): scheduled inquiries
     """
-    assert len(timing) == 3, "timing must include values for [target, fixation, stimuli]"
+
     target_indexes = []
     no_target = None
 
     if (target_positions == target_positions.DISTRIBUTED):
         target_indexes = distributed_target_positions(stim_number, stim_length, nontarget_inquiries)
     else:
         # make list of random targets with correct number of non-target inquiries
@@ -578,15 +523,15 @@
 def distributed_target_positions(stim_number: int, stim_length: int, nontarget_inquiries: int) -> list:
     """Distributed Target Positions.
 
     Generates evenly distributed target positions, including target letter not flashed at all, and shuffles them.
     Args:
         stim_number(int): Number of trials in calibration
         stim_length(int): Number of stimuli in each inquiry
-        nontarget_inquiries(int): percentage of inquiries for which target letter flashed is not in inquiry
+        nontarget_inquiries(int): percentage of iquiries for which target letter flashed is not in inquiry
 
     Return distributed_target_positions(list): targets: array of target indexes to be chosen
     """
 
     targets = []
     no_target = None
 
@@ -745,15 +690,15 @@
 
 def get_fixation(is_txt: bool) -> str:
     """Get Fixation.
 
     Return the correct stimulus fixation given the type (text or image).
     """
     if is_txt:
-        return DEFAULT_TEXT_FIXATION
+        return '+'
     else:
         return DEFAULT_FIXATION_PATH
 
 
 def ssvep_to_code(refresh_rate: int = 60, flicker_rate: int = 10) -> List[int]:
     """Convert SSVEP to Code.
```

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/system_utils.py` & `bcipy-2.0.1rc2/bcipy/helpers/system_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,305 +1,280 @@
-"""Utilities for system information and general functionality that may be
-shared across modules."""
-import importlib
-import logging
-import os
-import pkgutil
-import platform
-import socket
-import sys
-import time
-import torch
-from pathlib import Path
-from typing import Callable, List, Optional, NamedTuple
-
-import pkg_resources
-import psutil
-import pyglet
-from cpuinfo import get_cpu_info
-
-from bcipy.config import DEFAULT_ENCODING, LOG_FILENAME
-
-
-class ScreenInfo(NamedTuple):
-    width: int
-    height: int
-    rate: float
-
-
-def is_connected(hostname: str = "1.1.1.1", port=80) -> bool:
-    """Test for internet connectivity.
-
-    Parameters
-    ----------
-        hostname - name of host for attempted connection
-        port - port on host to which to connect
-    """
-    try:
-        conn = socket.create_connection(address=(hostname, port), timeout=2)
-        conn.close()
-        return True
-    except OSError:
-        pass
-    return False
-
-
-def is_battery_powered() -> bool:
-    """Check if this current computer is a laptop currently using its battery.
-
-    Returns
-    -------
-    True if the computer is currently running on battery power. This can impact
-    the performance of hardware (ex. GPU) needed for BciPy operation by entering
-    power saving operations."""
-    return psutil.sensors_battery(
-    ) and not psutil.sensors_battery().power_plugged
-
-
-def is_screen_refresh_rate_low(refresh: Optional[float] = None) -> bool:
-    """Check if the screen refresh rate is sufficient for BciPy operation.
-
-    Parameters
-    ----------
-        refresh(float) - optional screen refresh rate if already collected. If not provided,
-            the current screen refresh rate is gathered using get_screen_info().
-
-    Returns
-    -------
-    True if the refresh rate is less than 120 Hz; otherwise False.
-    """
-    if refresh is None:
-        refresh = get_screen_info().rate
-
-    return refresh < 120
-
-
-def git_dir() -> str:
-    """Git Directory.
-
-    Returns the root directory with the .git folder. If this source code
-    was not checked out from scm, answers None."""
-
-    # Relative to current file; may need to be modified if method is moved.
-    git_root = Path(os.path.abspath(__file__)).parent.parent.parent
-    git_meta = Path(os.path.join(git_root, '.git'))
-    return os.path.abspath(git_meta) if git_meta.is_dir() else None
-
-
-def git_hash() -> Optional[str]:
-    """Git Hash.
-
-    Returns an abbreviated git sha hash if this code is being run from a
-    git cloned version of bcipy; otherwise returns an empty string.
-
-    Could also consider making a system call to:
-    git describe --tags
-    """
-
-    git_path = git_dir()
-    if not git_path:
-        print('.git path not found')
-        return None
-
-    try:
-        head_path = Path(os.path.join(git_path, 'HEAD'))
-        with open(head_path, encoding=DEFAULT_ENCODING) as head_file:
-            # First line contains a reference to the current branch.
-            # ex. ref: refs/heads/branch_name
-            ref = head_file.readline()
-
-        ref_val = ref.split(':')[-1].strip()
-        ref_path = Path(os.path.join(git_path, ref_val))
-        with open(ref_path, encoding=DEFAULT_ENCODING) as ref_file:
-            sha = ref_file.readline()
-
-        # sha hash is 40 characters; use an abbreviated 7-char version which
-        # is displayed in github.
-        return sha[0:7]
-    except Exception as error:
-        print(f'Error reading git version: {error}')
-        return None
-
-
-def bcipy_version() -> str:
-    """BciPy Version.
-
-    Gets the current bcipy version. If the current instance of bcipy is a
-    git repository, appends the current abbreviated sha hash.
-    """
-    version = pkg_resources.get_distribution('bcipy').version
-    sha_hash = git_hash()
-
-    return f'{version} - {sha_hash}' if sha_hash else version
-
-
-def get_screen_info() -> ScreenInfo:
-    """Gets the screen information.
-
-    Note: Use this method if only the screen resolution is needed; it is much more efficient
-    than extracting that information from the dict returned by the get_system_info method.
-
-    Returns
-    -------
-        ScreenInfo(width, height, rate)
-     """
-    screen = pyglet.canvas.get_display().get_default_screen()
-    return ScreenInfo(screen.width, screen.height, screen.get_mode().rate)
-
-
-def get_gpu_info() -> List[dict]:
-    """Information about GPUs available for processing."""
-    properties = []
-    for idx in range(torch.cuda.device_count()):
-        prop = torch.get_device_properties(idx)
-        properties.append(dict(name=prop.name, total_memory=prop.total_memory))
-    return properties
-
-
-def get_system_info() -> dict:
-    """Get System Information.
-    See: https://stackoverflow.com/questions/3103178/how-to-get-the-system-info-with-python
-
-    Returns
-    -------
-        dict of system-related properties, including ['os', 'py_version', 'resolution',
-          'memory', 'bcipy_version', 'platform', 'platform-release', 'platform-version',
-          'architecture', 'processor', 'cpu_count', 'hz', 'ram']
-    """
-    screen_info = get_screen_info()
-    info = get_cpu_info()
-    gpu_info = get_gpu_info()
-    return {
-        'os': sys.platform,
-        'py_version': sys.version,
-        'screen_resolution': [screen_info.width, screen_info.height],
-        'memory': psutil.virtual_memory().available / 1024 / 1024,
-        'bcipy_version': bcipy_version(),
-        'platform': platform.system(),
-        'platform-release': platform.release(),
-        'platform-version': platform.version(),
-        'architecture': platform.machine(),
-        'processor': platform.processor(),
-        'cpu_count': os.cpu_count(),
-        'cpu_brand': info['brand_raw'],
-        'cpu_hz': info['hz_actual_friendly'],
-        'gpu_available': torch.cuda.is_available(),
-        'gpu_count': len(gpu_info),
-        'gpu_details': gpu_info,
-        'screen_refresh': f"{screen_info.rate}Hz",
-        'ram': str(round(psutil.virtual_memory().total / (1024.0**3))) + " GB"
-    }
-
-
-def configure_logger(
-        save_folder: str,
-        log_name=LOG_FILENAME,
-        log_level=logging.DEBUG,
-        version=None) -> None:
-    """Configure Logger.
-
-    Does what it says.
-    """
-    # create the log file
-    logfile = os.path.join(save_folder, 'logs', log_name)
-
-    # configure it
-    root_logger = logging.getLogger()
-    root_logger.setLevel(log_level)
-    handler = logging.FileHandler(logfile, 'w', encoding='utf-8')
-    handler.setFormatter(logging.Formatter(
-        '[%(threadName)-9s][%(asctime)s][%(name)s][%(levelname)s]: %(message)s'))
-    root_logger.addHandler(handler)
-
-    print(f'Printing all BciPy logs to: {logfile}')
-
-    if version:
-        logging.info(f'Start of Session for BciPy Version: ({version})')
-
-
-def import_submodules(package, recursive=True):
-    """Import Submodules.
-
-    Import all submodules of a module, recursively, including subpackages.
-    https://stackoverflow.com/questions/3365740/how-to-import-all-submodules
-
-    Parameters
-    ----------
-        package : str | package
-            name of package or package instance
-        recursive : bool, optional
-
-    Returns
-    -------
-        dict[str, types.ModuleType]
-    """
-    if isinstance(package, str):
-        package = importlib.import_module(package)
-    results = {}
-    for _loader, name, is_pkg in pkgutil.walk_packages(package.__path__):
-        full_name = package.__name__ + '.' + name
-        if name.startswith('test'):
-            continue
-        results[full_name] = importlib.import_module(full_name)
-        if recursive and is_pkg:
-            results.update(import_submodules(full_name))
-    return results
-
-
-def dot(relative_to: str, *argv) -> str:
-    """
-    Given a file location and one or more subdirectory/filename args, returns
-    a Path as a str for that file.
-
-    Ex. dot(__file__, 'fst', 'brown_closure.n5.kn.fst')
-    """
-    working_dir = Path(os.path.dirname(os.path.realpath(relative_to)))
-    for subdir in argv:
-        # uses the '/' operator in pathlib to construct a new Path.
-        working_dir = working_dir / subdir
-    return str(working_dir)
-
-
-def auto_str(cls):
-    """Autogenerate a str method to print all variable names and values.
-    https://stackoverflow.com/questions/32910096/is-there-a-way-to-auto-generate-a-str-implementation-in-python
-    """
-
-    def __str__(self):
-        return '%s(%s)' % (type(self).__name__, ', '.join(
-            '%s=%s' % item for item in vars(self).items()))
-
-    cls.__str__ = __str__
-    return cls
-
-
-def log_to_stdout():
-    """Set logging to stdout. Useful for demo scripts.
-    https://stackoverflow.com/questions/14058453/making-python-loggers-output-all-messages-to-stdout-in-addition-to-log-file
-    """
-
-    root = logging.getLogger()
-    root.setLevel(logging.DEBUG)
-
-    handler = logging.StreamHandler(sys.stdout)
-    handler.setLevel(logging.DEBUG)
-    formatter = logging.Formatter(
-        '[%(threadName)-9s][%(asctime)s][%(name)s][%(levelname)s]: %(message)s')
-    handler.setFormatter(formatter)
-    root.addHandler(handler)
-
-
-def report_execution_time(func: Callable) -> Callable:
-    """Report execution time.
-
-    A decorator to log execution time of methods in seconds. To use,
-        decorate your method with @report_execution_time.
-    """
-    log = logging.getLogger()
-
-    def wrap(*args, **kwargs):
-        time1 = time.perf_counter()
-        response = func(*args, **kwargs)
-        time2 = time.perf_counter()
-        log.info('{:s} method took {:0.4f}s to execute'.format(func.__name__, (time2 - time1)))
-        return response
-    return wrap
+"""Utilities for system information and general functionality that may be
+shared across modules."""
+import importlib
+import logging
+import os
+import pkgutil
+import platform
+import socket
+import sys
+import time
+import torch
+from pathlib import Path
+from typing import Callable, List, Optional, Tuple
+
+import pkg_resources
+import psutil
+import pyglet
+from cpuinfo import get_cpu_info
+
+from bcipy.config import DEFAULT_ENCODING, LOG_FILENAME
+
+
+def is_connected(hostname: str = "1.1.1.1", port=80) -> bool:
+    """Test for internet connectivity.
+
+    Parameters
+    ----------
+        hostname - name of host for attempted connection
+        port - port on host to which to connect
+    """
+    try:
+        conn = socket.create_connection(address=(hostname, port), timeout=2)
+        conn.close()
+        return True
+    except OSError:
+        pass
+    return False
+
+
+def is_battery_powered() -> bool:
+    """Check if this current computer is a laptop currently using its battery.
+
+    Returns
+    -------
+    True if the computer is currently running on battery power. This can impact
+    the performance of hardware (ex. GPU) needed for BciPy operation by entering
+    power saving operations."""
+    return psutil.sensors_battery(
+    ) and not psutil.sensors_battery().power_plugged
+
+
+def git_dir() -> str:
+    """Git Directory.
+
+    Returns the root directory with the .git folder. If this source code
+    was not checked out from scm, answers None."""
+
+    # Relative to current file; may need to be modified if method is moved.
+    git_root = Path(os.path.abspath(__file__)).parent.parent.parent
+    git_meta = Path(os.path.join(git_root, '.git'))
+    return os.path.abspath(git_meta) if git_meta.is_dir() else None
+
+
+def git_hash() -> Optional[str]:
+    """Git Hash.
+
+    Returns an abbreviated git sha hash if this code is being run from a
+    git cloned version of bcipy; otherwise returns an empty string.
+
+    Could also consider making a system call to:
+    git describe --tags
+    """
+
+    git_path = git_dir()
+    if not git_path:
+        print('.git path not found')
+        return None
+
+    try:
+        head_path = Path(os.path.join(git_path, 'HEAD'))
+        with open(head_path, encoding=DEFAULT_ENCODING) as head_file:
+            # First line contains a reference to the current branch.
+            # ex. ref: refs/heads/branch_name
+            ref = head_file.readline()
+
+        ref_val = ref.split(':')[-1].strip()
+        ref_path = Path(os.path.join(git_path, ref_val))
+        with open(ref_path, encoding=DEFAULT_ENCODING) as ref_file:
+            sha = ref_file.readline()
+
+        # sha hash is 40 characters; use an abbreviated 7-char version which
+        # is displayed in github.
+        return sha[0:7]
+    except Exception as error:
+        print(f'Error reading git version: {error}')
+        return None
+
+
+def bcipy_version() -> str:
+    """BciPy Version.
+
+    Gets the current bcipy version. If the current instance of bcipy is a
+    git repository, appends the current abbreviated sha hash.
+    """
+    version = pkg_resources.get_distribution('bcipy').version
+    sha_hash = git_hash()
+
+    return f'{version} - {sha_hash}' if sha_hash else version
+
+
+def get_screen_resolution() -> Tuple[int, int]:
+    """Gets the screen resolution.
+
+    Note: Use this method if only the screen resolution is needed; it is much more efficient
+    than extracting that information from the dict returned by the get_system_info method.
+
+    Returns
+    -------
+        (width, height)
+     """
+    screen = pyglet.canvas.get_display().get_default_screen()
+    return (screen.width, screen.height)
+
+
+def get_gpu_info() -> List[dict]:
+    """Information about GPUs available for processing."""
+    properties = []
+    for idx in range(torch.cuda.device_count()):
+        prop = torch.get_device_properties(idx)
+        properties.append(dict(name=prop.name, total_memory=prop.total_memory))
+    return properties
+
+
+def get_system_info() -> dict:
+    """Get System Information.
+    See: https://stackoverflow.com/questions/3103178/how-to-get-the-system-info-with-python
+
+    Returns
+    -------
+        dict of system-related properties, including ['os', 'py_version', 'resolution',
+          'memory', 'bcipy_version', 'platform', 'platform-release', 'platform-version',
+          'architecture', 'processor', 'cpu_count', 'hz', 'ram']
+    """
+    screen_width, screen_height = get_screen_resolution()
+    info = get_cpu_info()
+    gpu_info = get_gpu_info()
+    return {
+        'os': sys.platform,
+        'py_version': sys.version,
+        'resolution': [screen_width, screen_height],
+        'memory': psutil.virtual_memory().available / 1024 / 1024,
+        'bcipy_version': bcipy_version(),
+        'platform': platform.system(),
+        'platform-release': platform.release(),
+        'platform-version': platform.version(),
+        'architecture': platform.machine(),
+        'processor': platform.processor(),
+        'cpu_count': os.cpu_count(),
+        'cpu_brand': info['brand_raw'],
+        'gpu_available': torch.cuda.is_available(),
+        'gpu_count': len(gpu_info),
+        'gpu_details': gpu_info,
+        'hz': info['hz_actual_friendly'],
+        'ram': str(round(psutil.virtual_memory().total / (1024.0**3))) + " GB"
+    }
+
+
+def configure_logger(
+        save_folder: str,
+        log_name=LOG_FILENAME,
+        log_level=logging.DEBUG,
+        version=None) -> None:
+    """Configure Logger.
+
+    Does what it says.
+    """
+    # create the log file
+    logfile = os.path.join(save_folder, 'logs', log_name)
+
+    # configure it
+    root_logger = logging.getLogger()
+    root_logger.setLevel(log_level)
+    handler = logging.FileHandler(logfile, 'w', encoding='utf-8')
+    handler.setFormatter(logging.Formatter(
+        '[%(threadName)-9s][%(asctime)s][%(name)s][%(levelname)s]: %(message)s'))
+    root_logger.addHandler(handler)
+
+    print(f'Printing all BciPy logs to: {logfile}')
+
+    if version:
+        logging.info(f'Start of Session for BciPy Version: ({version})')
+
+
+def import_submodules(package, recursive=True):
+    """Import Submodules.
+
+    Import all submodules of a module, recursively, including subpackages.
+    https://stackoverflow.com/questions/3365740/how-to-import-all-submodules
+
+    Parameters
+    ----------
+        package : str | package
+            name of package or package instance
+        recursive : bool, optional
+
+    Returns
+    -------
+        dict[str, types.ModuleType]
+    """
+    if isinstance(package, str):
+        package = importlib.import_module(package)
+    results = {}
+    for _loader, name, is_pkg in pkgutil.walk_packages(package.__path__):
+        full_name = package.__name__ + '.' + name
+        if name.startswith('test'):
+            continue
+        results[full_name] = importlib.import_module(full_name)
+        if recursive and is_pkg:
+            results.update(import_submodules(full_name))
+    return results
+
+
+def dot(relative_to: str, *argv) -> str:
+    """
+    Given a file location and one or more subdirectory/filename args, returns
+    a Path as a str for that file.
+
+    Ex. dot(__file__, 'fst', 'brown_closure.n5.kn.fst')
+    """
+    working_dir = Path(os.path.dirname(os.path.realpath(relative_to)))
+    for subdir in argv:
+        # uses the '/' operator in pathlib to construct a new Path.
+        working_dir = working_dir / subdir
+    return str(working_dir)
+
+
+def auto_str(cls):
+    """Autogenerate a str method to print all variable names and values.
+    https://stackoverflow.com/questions/32910096/is-there-a-way-to-auto-generate-a-str-implementation-in-python
+    """
+
+    def __str__(self):
+        return '%s(%s)' % (type(self).__name__, ', '.join(
+            '%s=%s' % item for item in vars(self).items()))
+
+    cls.__str__ = __str__
+    return cls
+
+
+def log_to_stdout():
+    """Set logging to stdout. Useful for demo scripts.
+    https://stackoverflow.com/questions/14058453/making-python-loggers-output-all-messages-to-stdout-in-addition-to-log-file
+    """
+
+    root = logging.getLogger()
+    root.setLevel(logging.DEBUG)
+
+    handler = logging.StreamHandler(sys.stdout)
+    handler.setLevel(logging.DEBUG)
+    formatter = logging.Formatter(
+        '[%(threadName)-9s][%(asctime)s][%(name)s][%(levelname)s]: %(message)s')
+    handler.setFormatter(formatter)
+    root.addHandler(handler)
+
+
+def report_execution_time(func: Callable) -> Callable:
+    """Report execution time.
+
+    A decorator to log execution time of methods in seconds. To use,
+        decorate your method with @report_execution_time.
+    """
+    log = logging.getLogger()
+
+    def wrap(*args, **kwargs):
+        time1 = time.perf_counter()
+        response = func(*args, **kwargs)
+        time2 = time.perf_counter()
+        log.info('{:s} method took {:0.4f}s to execute'.format(func.__name__, (time2 - time1)))
+        return response
+    return wrap
```

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/task.py` & `bcipy-2.0.1rc2/bcipy/helpers/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import logging
+import os
 import random
+from string import ascii_uppercase
 from typing import Any, List, Tuple, Union
 
 import numpy as np
 from psychopy import core, event, visual
 
 from bcipy.config import SESSION_COMPLETE_MESSAGE
 from bcipy.helpers.clock import Clock
 from bcipy.helpers.stimuli import get_fixation
 from bcipy.task.exceptions import InsufficientDataException
 
 log = logging.getLogger(__name__)
 
+SPACE_CHAR = '_'
+BACKSPACE_CHAR = '<'
+
 
 def fake_copy_phrase_decision(copy_phrase, target_letter, text_task):
     """Fake Copy Phrase Decision.
 
     Parameters
     ----------
         copy_phrase(str): phrase to be copied
@@ -70,14 +75,41 @@
     :returns: frequency: stimulation frequency of the inquiry
     """
 
     # We want to know how many stimuli will present in a second
     return 1 / flash_time
 
 
+def alphabet(parameters=None, include_path=True):
+    """Alphabet.
+
+    Function used to standardize the symbols we use as alphabet.
+
+    Returns
+    -------
+        array of letters.
+    """
+    if parameters and not parameters['is_txt_stim']:
+        # construct an array of paths to images
+        path = parameters['path_to_presentation_images']
+        stimulus_array = []
+        for stimulus_filename in sorted(os.listdir(path)):
+            # PLUS.png is reserved for the fixation symbol
+            if stimulus_filename.endswith(
+                    '.png') and not stimulus_filename.endswith('PLUS.png'):
+                if include_path:
+                    img = os.path.join(path, stimulus_filename)
+                else:
+                    img = os.path.splitext(stimulus_filename)[0]
+                stimulus_array.append(img)
+        return stimulus_array
+
+    return list(ascii_uppercase) + [BACKSPACE_CHAR, SPACE_CHAR]
+
+
 def construct_triggers(inquiry_timing: List[List]) -> List[Tuple[str, float]]:
     """Construct triggers from inquiry_timing data.
 
     Parameters
     ----------
     - inquiry_timing: list of tuples containing stimulus timing and text
```

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/tests/test_clock.py` & `bcipy-2.0.1rc2/bcipy/helpers/tests/test_clock.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/tests/test_copy_phrase_wrapper.py` & `bcipy-2.0.1rc2/bcipy/helpers/tests/test_copy_phrase_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import numpy as np
 
 from bcipy.config import DEFAULT_PARAMETERS_PATH
 from bcipy.acquisition.devices import DeviceSpec, register
 from bcipy.helpers.copy_phrase_wrapper import CopyPhraseWrapper
 from bcipy.helpers.load import load_json_parameters
-from bcipy.helpers.symbols import alphabet
-from bcipy.language.model.uniform import UniformLanguageModel
+from bcipy.helpers.task import alphabet
+from bcipy.language.uniform import UniformLanguageModel
 from bcipy.signal.model import PcaRdaKdeModel
 from bcipy.task.data import EvidenceType
 
 
 class TestCopyPhraseWrapper(unittest.TestCase):
     """Test CopyPhraseWrapper"""
 
@@ -65,22 +65,23 @@
 
     def test_valid_letters(self):
         alp = alphabet()
         cp = CopyPhraseWrapper(
             min_num_inq=1,
             max_num_inq=50,
             lmodel=None,
-            device_spec=self.device_spec,
             signal_model=None,
-            # fs=25,
+            fs=25,
             k=2,
             alp=alp,
             task_list=[("HELLO_WORLD", "HE")],
             is_txt_stim=True,
+            device_name=self.device_spec.name,
             evidence_names=[EvidenceType.LM, EvidenceType.ERP],
+            device_channels=self.device_spec.channels,
             stim_timing=[0.5, 0.25],
         )
 
         triggers = [
             ("+", 0.0),
             ("H", 0.5670222830376588),
             ("D", 0.8171830819919705),
@@ -169,21 +170,23 @@
 
         # Note that frequencies for notch and bandpass filter below are chosen to be < 1/2 of sampling frequency
         # due to limitations of nyquist-shannon sampling theorem
         copy_phrase_task = CopyPhraseWrapper(
             min_num_inq=1,
             max_num_inq=50,
             lmodel=UniformLanguageModel(symbol_set=alp),
-            device_spec=self.device_spec,
             signal_model=self.model,
+            fs=self.device_spec.sample_rate,
             k=1,
             alp=alp,
             task_list=[("HELLO_WORLD", "HE")],
             is_txt_stim=True,
+            device_name=self.device_spec.name,
             evidence_names=[EvidenceType.LM, EvidenceType.ERP],
+            device_channels=self.device_spec.channels,
             stim_timing=[0.5, 0.25],
             notch_filter_frequency=4.0,
             filter_low=1.0,
             filter_high=4.0,
             stim_length=self.params["stim_length"],
         )
```

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/tests/test_language_model.py` & `bcipy-2.0.1rc2/bcipy/helpers/tests/test_language_model.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/tests/test_list.py` & `bcipy-2.0.1rc2/bcipy/helpers/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/tests/test_load.py` & `bcipy-2.0.1rc2/bcipy/helpers/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/tests/test_parameters.py` & `bcipy-2.0.1rc2/bcipy/helpers/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/tests/test_raw_data.py` & `bcipy-2.0.1rc2/bcipy/helpers/tests/test_raw_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,381 +1,374 @@
-"""Tests for BciPy raw data format."""
-import os
-import shutil
-import tempfile
-import unittest
-from pathlib import Path
-
-import numpy as np
-import pandas as pd
-
-from mockito import any, mock, when, verify, unstub
-
-from bcipy.helpers.exceptions import BciPyCoreException
-from bcipy.helpers.raw_data import (RawData, RawDataReader, RawDataWriter,
-                                    load, sample_data, settings, write)
-
-
-class TestRawData(unittest.TestCase):
-    """Tests for raw_data format"""
-
-    def setUp(self):
-        """Override; set up the needed path for load functions."""
-        self.data_dir = f"{os.path.dirname(__file__)}/resources/"
-        self.temp_dir = tempfile.mkdtemp()
-        self.path = Path(self.temp_dir, 'test_raw_data.csv')
-        self.daq_type = 'Test-Device'
-        self.sample_rate = 300.0
-        self.columns = ['timestamp', 'ch1', 'ch2', 'ch3']
-        self.row1 = [1, 1.0, 2.0, 3.0]
-        self.row2 = [2, 4.0, 5.0, 6.0]
-        self.row3 = [3, 7.0, 8.0, 9.0]
-
-    def tearDown(self):
-        """Override"""
-        shutil.rmtree(self.temp_dir)
-        unstub()
-
-    def _write_raw_data(self, include_rows=False) -> RawData:
-        """Helper function to write a sample raw data file to disk using the
-        settings from setUp.
-
-        Parameters
-        ----------
-        - include_rows : if True adds data, otherwise just writes the metadata
-        and columns.
-        """
-        data = RawData(daq_type=self.daq_type,
-                       sample_rate=self.sample_rate,
-                       columns=self.columns)
-        if include_rows:
-            data.append(self.row1)
-            data.append(self.row2)
-            data.append(self.row3)
-
-        write(data, self.path)
-
-    def test_init(self):
-        """Test that a RawData structure can be initialized"""
-        data = RawData(daq_type=self.daq_type,
-                       sample_rate=self.sample_rate,
-                       columns=self.columns)
-        self.assertEqual(data.daq_type, self.daq_type)
-        self.assertEqual(data.sample_rate, self.sample_rate)
-        self.assertEqual(data.columns, self.columns)
-
-    def test_write_with_no_data(self):
-        """Test that raw data can be persisted to disk."""
-        data = RawData(daq_type=self.daq_type,
-                       sample_rate=self.sample_rate,
-                       columns=self.columns)
-
-        self.assertFalse(self.path.exists())
-        write(data, self.path)
-        self.assertTrue(self.path.exists())
-
-    def test_load_with_no_data(self):
-        """Test that the raw data format can be read by the module."""
-        self._write_raw_data()
-        data = load(self.path)
-
-        self.assertEqual(data.daq_type, self.daq_type)
-        self.assertEqual(data.sample_rate, self.sample_rate)
-        self.assertEqual(data.columns, self.columns)
-        self.assertEqual(0, len(data.rows))
-
-    def test_load_with_data(self):
-        """Test that data can be loaded from a file."""
-        self._write_raw_data(include_rows=True)
-        loaded_data = load(self.path)
-
-        self.assertEqual(loaded_data.daq_type, self.daq_type)
-        self.assertEqual(loaded_data.sample_rate, self.sample_rate)
-        self.assertEqual(loaded_data.columns, self.columns)
-
-        self.assertEqual(len(loaded_data.rows), 3)
-        self.assertEqual(loaded_data.rows[0], self.row1)
-        self.assertEqual(loaded_data.rows[1], self.row2)
-        self.assertEqual(loaded_data.rows[2], self.row3)
-
-    def test_load_with_invalid_filepath(self):
-        """Test that an exception is raised when an invalid file is loaded."""
-        with self.assertRaises(BciPyCoreException):
-            path = "invalid/path/to/file.csv"
-            load(path)
-
-    def test_deserialization(self):
-        """Test that the load function can be accessed through a class
-        constructor."""
-        self._write_raw_data(include_rows=True)
-
-        loaded_data = RawData.load(self.path)
-
-        self.assertEqual(loaded_data.daq_type, self.daq_type)
-        self.assertEqual(loaded_data.sample_rate, self.sample_rate)
-        self.assertEqual(loaded_data.columns, self.columns)
-
-        self.assertEqual(len(loaded_data.rows), 3)
-        self.assertEqual(loaded_data.rows[0], self.row1)
-        self.assertEqual(loaded_data.rows[1], self.row2)
-        self.assertEqual(loaded_data.rows[2], self.row3)
-
-    def test_settings(self):
-        """Test that metadata settings can be extracted from a raw data
-        file."""
-        self._write_raw_data()
-
-        name, sample_rate, columns = settings(self.path)
-        self.assertEqual(name, self.daq_type)
-        self.assertEqual(sample_rate, self.sample_rate)
-        self.assertEqual(columns, self.columns)
-
-    def test_raw_data_reader(self):
-        """Test that data can be read from a file incrementally."""
-        self._write_raw_data(include_rows=True)
-
-        with RawDataReader(self.path) as reader:
-            self.assertEqual(reader.daq_type, self.daq_type)
-            self.assertEqual(reader.sample_rate, self.sample_rate)
-            self.assertEqual(reader.columns, self.columns)
-
-            # all columns are read as strings by default
-            self.assertEqual(list(map(str, self.row1)), next(reader))
-            self.assertEqual(list(map(str, self.row2)), next(reader))
-            self.assertEqual(list(map(str, self.row3)), next(reader))
-
-    def test_raw_data_reader_with_type_conversions(self):
-        """Test that data can be read incrementally and that data can be
-        converted to numeric types."""
-        columns = ['timestamp', 'ch1', 'ch2', 'ch3', 'TRG']
-        data = RawData(daq_type=self.daq_type,
-                       sample_rate=self.sample_rate,
-                       columns=columns)
-
-        row1 = [1, 1.0, 2.0, 3.0, 'A']
-        row2 = [2, 4.0, 5.0, 6.0, 'B']
-        row3 = [3, 7.0, 8.0, 9.0, 'C']
-
-        data.append(row1)
-        data.append(row2)
-        data.append(row3)
-        write(data, self.path)
-
-        with RawDataReader(self.path, convert_data=True) as reader:
-            self.assertEqual(reader.daq_type, self.daq_type)
-            self.assertEqual(reader.sample_rate, self.sample_rate)
-            self.assertEqual(reader.columns, data.columns)
-
-            self.assertEqual(row1, next(reader))
-            self.assertEqual(row2, next(reader))
-            self.assertEqual(row3, next(reader))
-
-    def test_raw_data_writer(self):
-        """Test that data can be written incrementally"""
-
-        rows = [self.row1, self.row2, self.row3]
-
-        self.assertFalse(self.path.exists())
-        with RawDataWriter(self.path,
-                           daq_type=self.daq_type,
-                           sample_rate=self.sample_rate,
-                           columns=self.columns) as writer:
-            for row in rows:
-                writer.writerow(row)
-        self.assertTrue(self.path.exists())
-
-    def test_raw_data_writer_writerows(self):
-        """Test that data can be written in chunks."""
-
-        rows = [self.row1, self.row2, self.row3]
-
-        self.assertFalse(self.path.exists())
-        with RawDataWriter(self.path,
-                           daq_type=self.daq_type,
-                           sample_rate=self.sample_rate,
-                           columns=self.columns) as writer:
-            writer.writerows(rows)
-        self.assertTrue(self.path.exists())
-
-        loaded_data = RawData.load(self.path)
-        self.assertEqual(loaded_data.daq_type, self.daq_type)
-        self.assertEqual(loaded_data.sample_rate, self.sample_rate)
-        self.assertEqual(loaded_data.columns, self.columns)
-        self.assertEqual(len(loaded_data.rows), 3)
-
-    def test_raw_data_writer_initialization(self):
-        """Test that writer can be manually opened and closed"""
-
-        rows = [self.row1, self.row2, self.row3]
-
-        self.assertFalse(self.path.exists())
-        writer = RawDataWriter(self.path,
-                               daq_type=self.daq_type,
-                               sample_rate=self.sample_rate,
-                               columns=self.columns)
-        writer.__enter__()
-        writer.writerows(rows)
-        writer.__exit__()
-
-        self.assertTrue(self.path.exists())
-        loaded_data = RawData.load(self.path)
-
-        self.assertEqual(loaded_data.daq_type, self.daq_type)
-        self.assertEqual(loaded_data.sample_rate, self.sample_rate)
-        self.assertEqual(loaded_data.columns, self.columns)
-
-        self.assertEqual(len(loaded_data.rows), 3)
-
-    def test_sample_data(self):
-        """Test that sample data can be generated for testing purposes."""
-        channels = ['ch1', 'ch2', 'ch3']
-        data = sample_data(rows=5, ch_names=channels)
-        self.assertEqual(5, len(data.rows))
-        self.assertEqual(['timestamp', 'ch1', 'ch2', 'ch3', 'TRG'],
-                         data.columns)
-        self.assertEqual(1, data.rows[0][0])
-        self.assertEqual(5, data.rows[4][0])
-
-        # Test data range of channel columns
-        for row in data.rows:
-            for col in row[1:-1]:
-                self.assertTrue(col >= -1000 and col <= 1000)
-
-    def test_sample_data_with_triggers(self):
-        """Test generating sample data with triggers at pre-defined timestamps.
-        This functionality is used primarily for other unit tests."""
-        channels = ['ch1', 'ch2', 'ch3']
-        data = sample_data(rows=10,
-                           ch_names=channels,
-                           triggers=[(1, 'A'), (5, 'B'), (10, 'C')])
-        self.assertEqual(10, len(data.rows))
-
-        trg_col = data.columns.index('TRG')
-        self.assertEqual('A', data.rows[0][trg_col])
-        self.assertEqual('B', data.rows[4][trg_col])
-        self.assertEqual('C', data.rows[9][trg_col])
-
-    def test_raw_data_numeric_channels(self):
-        """Tests that data channels can be extracted for analysis."""
-
-        columns = ['timestamp', 'ch1', 'ch2', 'ch3', 'TRG']
-        data = RawData(daq_type=self.daq_type,
-                       sample_rate=self.sample_rate,
-                       columns=columns)
-
-        row1 = [1, 1.0, 2.0, 3.0, '0.0']
-        row2 = [2, 4.0, 5.0, 6.0, 'A']
-        row3 = [3, 7.0, 8.0, 9.0, '0.0']
-
-        data.append(row1)
-        data.append(row2)
-        data.append(row3)
-
-        self.assertEqual(['ch1', 'ch2', 'ch3'], data.channels)
-
-        # Test numeric data frame
-        dataframe = pd.DataFrame(data=[[1, 1.0, 2.0, 3.0], [2, 4.0, 5.0, 6.0],
-                                       [3, 7.0, 8.0, 9.0]],
-                                 columns=['timestamp', 'ch1', 'ch2', 'ch3'])
-        self.assertTrue(np.all(dataframe == data.numeric_data))
-
-    def test_data_by_channel(self):
-        """Tests that data can be structured in column-order for analysis."""
-
-        columns = ['timestamp', 'ch1', 'ch2', 'TRG']
-        data = RawData(daq_type=self.daq_type,
-                       sample_rate=self.sample_rate,
-                       columns=columns)
-
-        data.append([1, 1.0, 2.0, '0.0'])
-        data.append([2, 4.0, 5.0, 'A'])
-        data.append([3, 7.0, 8.0, '0.0'])
-
-        arr, _ = data.by_channel()
-        self.assertEqual((2, 3), arr.shape)
-
-        self.assertTrue(len(data.channels), len(arr))
-        self.assertTrue(np.all(arr[0] == [1.0, 4.0, 7.0]),
-                        "Should have ch1 data")
-        self.assertTrue(np.all(arr[1] == [2.0, 5.0, 8.0]),
-                        "Should have ch2 data")
-
-    def test_data_by_channel_applies_transformation(self):
-        """Tests that data correctly structured, can have a transformation applied to it."""
-        columns = ['timestamp', 'ch1', 'ch2', 'TRG']
-        data = RawData(daq_type=self.daq_type,
-                       sample_rate=self.sample_rate,
-                       columns=columns)
-
-        data.append([1, 1.0, 2.0, '0.0'])
-        data.append([2, 4.0, 5.0, 'A'])
-        data.append([3, 7.0, 8.0, '0.0'])
-
-        transform = mock()
-        # note data here should be returned as a nd.array. for mocking we don't care as much
-        when(RawData).apply_transform(any(), transform).thenReturn((data, self.sample_rate))
-        resp, fs = data.by_channel(transform=transform)
-
-        self.assertEqual(self.sample_rate, fs)
-        self.assertEqual(resp, data)
-        verify(RawData, times=1).apply_transform(any(), transform)
-
-    def test_data_by_channel_map(self):
-        """Tests that when given a channel map, it will filter the numeric columns.
-
-        We assume most trigger columns will be removed (due to being read in as a string or object),
-        however some are numeric trigger channels and may require filtering with a channel map.
-        Other cases could be dropping bad channels.
-        """
-        columns = ['timestamp', 'ch1', 'ch2', 'TRG']
-        channel_map = [1, 1, 0]
-        expected_channels = ['ch1', 'ch2']
-        data = RawData(daq_type=self.daq_type,
-                       sample_rate=self.sample_rate,
-                       columns=columns)
-
-        data.append([1, 1.0, 2.0, 0.0])
-        data.append([2, 4.0, 5.0, 0.0])
-        data.append([3, 7.0, 8.0, 0.0])
-
-        arr, channels, _ = data.by_channel_map(channel_map=channel_map)
-
-        self.assertEqual((2, 3), arr.shape)
-
-        self.assertTrue(len(data.channels), len(arr))
-        self.assertTrue(np.all(arr[0] == [1.0, 4.0, 7.0]),
-                        "Should have ch1 data")
-        self.assertTrue(np.all(arr[1] == [2.0, 5.0, 8.0]),
-                        "Should have ch2 data")
-        self.assertEqual(channels, expected_channels)
-
-    def test_data_by_channel_map_applies_transformation(self):
-        """Tests that when given a channel map, it will filter the numeric columns.
-
-        We assume most trigger columns will be removed (due to being read in as a string or object),
-        however some are numeric trigger channels and may require filtering with a channel map.
-        Other cases could be dropping bad channels.
-        """
-        columns = ['timestamp', 'ch1', 'ch2', 'TRG']
-        channel_map = [1, 1, 1]
-        expected_channels = ['ch1', 'ch2', 'TRG']
-        data = RawData(daq_type=self.daq_type,
-                       sample_rate=self.sample_rate,
-                       columns=columns)
-
-        data.append([1, 1.0, 2.0, 0.0])
-        data.append([2, 4.0, 5.0, 0.0])
-        data.append([3, 7.0, 8.0, 0.0])
-
-        transform = mock()
-        expected_output, expected_fs = data.by_channel()
-        # note data here should be returned as a nd.array. for mocking we don't care as much
-        when(RawData).by_channel(transform).thenReturn((expected_output, expected_fs))
-        _, channels, fs = data.by_channel_map(channel_map=channel_map, transform=transform)
-
-        self.assertEqual(expected_fs, fs)
-        self.assertEqual(expected_channels, channels)
-        verify(RawData, times=1).by_channel(transform)
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""Tests for BciPy raw data format."""
+import os
+import shutil
+import tempfile
+import unittest
+from pathlib import Path
+
+import numpy as np
+import pandas as pd
+
+from mockito import any, mock, when, verify, unstub
+
+from bcipy.helpers.raw_data import (RawData, RawDataReader, RawDataWriter,
+                                    load, sample_data, settings, write)
+
+
+class TestRawData(unittest.TestCase):
+    """Tests for raw_data format"""
+
+    def setUp(self):
+        """Override; set up the needed path for load functions."""
+        self.data_dir = f"{os.path.dirname(__file__)}/resources/"
+        self.temp_dir = tempfile.mkdtemp()
+        self.path = Path(self.temp_dir, 'test_raw_data.csv')
+        self.daq_type = 'Test-Device'
+        self.sample_rate = 300.0
+        self.columns = ['timestamp', 'ch1', 'ch2', 'ch3']
+        self.row1 = [1, 1.0, 2.0, 3.0]
+        self.row2 = [2, 4.0, 5.0, 6.0]
+        self.row3 = [3, 7.0, 8.0, 9.0]
+
+    def tearDown(self):
+        """Override"""
+        shutil.rmtree(self.temp_dir)
+        unstub()
+
+    def _write_raw_data(self, include_rows=False) -> RawData:
+        """Helper function to write a sample raw data file to disk using the
+        settings from setUp.
+
+        Parameters
+        ----------
+        - include_rows : if True adds data, otherwise just writes the metadata
+        and columns.
+        """
+        data = RawData(daq_type=self.daq_type,
+                       sample_rate=self.sample_rate,
+                       columns=self.columns)
+        if include_rows:
+            data.append(self.row1)
+            data.append(self.row2)
+            data.append(self.row3)
+
+        write(data, self.path)
+
+    def test_init(self):
+        """Test that a RawData structure can be initialized"""
+        data = RawData(daq_type=self.daq_type,
+                       sample_rate=self.sample_rate,
+                       columns=self.columns)
+        self.assertEqual(data.daq_type, self.daq_type)
+        self.assertEqual(data.sample_rate, self.sample_rate)
+        self.assertEqual(data.columns, self.columns)
+
+    def test_write_with_no_data(self):
+        """Test that raw data can be persisted to disk."""
+        data = RawData(daq_type=self.daq_type,
+                       sample_rate=self.sample_rate,
+                       columns=self.columns)
+
+        self.assertFalse(self.path.exists())
+        write(data, self.path)
+        self.assertTrue(self.path.exists())
+
+    def test_load_with_no_data(self):
+        """Test that the raw data format can be read by the module."""
+        self._write_raw_data()
+        data = load(self.path)
+
+        self.assertEqual(data.daq_type, self.daq_type)
+        self.assertEqual(data.sample_rate, self.sample_rate)
+        self.assertEqual(data.columns, self.columns)
+        self.assertEqual(0, len(data.rows))
+
+    def test_load_with_data(self):
+        """Test that data can be loaded from a file."""
+        self._write_raw_data(include_rows=True)
+        loaded_data = load(self.path)
+
+        self.assertEqual(loaded_data.daq_type, self.daq_type)
+        self.assertEqual(loaded_data.sample_rate, self.sample_rate)
+        self.assertEqual(loaded_data.columns, self.columns)
+
+        self.assertEqual(len(loaded_data.rows), 3)
+        self.assertEqual(loaded_data.rows[0], self.row1)
+        self.assertEqual(loaded_data.rows[1], self.row2)
+        self.assertEqual(loaded_data.rows[2], self.row3)
+
+    def test_deserialization(self):
+        """Test that the load function can be accessed through a class
+        constructor."""
+        self._write_raw_data(include_rows=True)
+
+        loaded_data = RawData.load(self.path)
+
+        self.assertEqual(loaded_data.daq_type, self.daq_type)
+        self.assertEqual(loaded_data.sample_rate, self.sample_rate)
+        self.assertEqual(loaded_data.columns, self.columns)
+
+        self.assertEqual(len(loaded_data.rows), 3)
+        self.assertEqual(loaded_data.rows[0], self.row1)
+        self.assertEqual(loaded_data.rows[1], self.row2)
+        self.assertEqual(loaded_data.rows[2], self.row3)
+
+    def test_settings(self):
+        """Test that metadata settings can be extracted from a raw data
+        file."""
+        self._write_raw_data()
+
+        name, sample_rate, columns = settings(self.path)
+        self.assertEqual(name, self.daq_type)
+        self.assertEqual(sample_rate, self.sample_rate)
+        self.assertEqual(columns, self.columns)
+
+    def test_raw_data_reader(self):
+        """Test that data can be read from a file incrementally."""
+        self._write_raw_data(include_rows=True)
+
+        with RawDataReader(self.path) as reader:
+            self.assertEqual(reader.daq_type, self.daq_type)
+            self.assertEqual(reader.sample_rate, self.sample_rate)
+            self.assertEqual(reader.columns, self.columns)
+
+            # all columns are read as strings by default
+            self.assertEqual(list(map(str, self.row1)), next(reader))
+            self.assertEqual(list(map(str, self.row2)), next(reader))
+            self.assertEqual(list(map(str, self.row3)), next(reader))
+
+    def test_raw_data_reader_with_type_conversions(self):
+        """Test that data can be read incrementally and that data can be
+        converted to numeric types."""
+        columns = ['timestamp', 'ch1', 'ch2', 'ch3', 'TRG']
+        data = RawData(daq_type=self.daq_type,
+                       sample_rate=self.sample_rate,
+                       columns=columns)
+
+        row1 = [1, 1.0, 2.0, 3.0, 'A']
+        row2 = [2, 4.0, 5.0, 6.0, 'B']
+        row3 = [3, 7.0, 8.0, 9.0, 'C']
+
+        data.append(row1)
+        data.append(row2)
+        data.append(row3)
+        write(data, self.path)
+
+        with RawDataReader(self.path, convert_data=True) as reader:
+            self.assertEqual(reader.daq_type, self.daq_type)
+            self.assertEqual(reader.sample_rate, self.sample_rate)
+            self.assertEqual(reader.columns, data.columns)
+
+            self.assertEqual(row1, next(reader))
+            self.assertEqual(row2, next(reader))
+            self.assertEqual(row3, next(reader))
+
+    def test_raw_data_writer(self):
+        """Test that data can be written incrementally"""
+
+        rows = [self.row1, self.row2, self.row3]
+
+        self.assertFalse(self.path.exists())
+        with RawDataWriter(self.path,
+                           daq_type=self.daq_type,
+                           sample_rate=self.sample_rate,
+                           columns=self.columns) as writer:
+            for row in rows:
+                writer.writerow(row)
+        self.assertTrue(self.path.exists())
+
+    def test_raw_data_writer_writerows(self):
+        """Test that data can be written in chunks."""
+
+        rows = [self.row1, self.row2, self.row3]
+
+        self.assertFalse(self.path.exists())
+        with RawDataWriter(self.path,
+                           daq_type=self.daq_type,
+                           sample_rate=self.sample_rate,
+                           columns=self.columns) as writer:
+            writer.writerows(rows)
+        self.assertTrue(self.path.exists())
+
+        loaded_data = RawData.load(self.path)
+        self.assertEqual(loaded_data.daq_type, self.daq_type)
+        self.assertEqual(loaded_data.sample_rate, self.sample_rate)
+        self.assertEqual(loaded_data.columns, self.columns)
+        self.assertEqual(len(loaded_data.rows), 3)
+
+    def test_raw_data_writer_initialization(self):
+        """Test that writer can be manually opened and closed"""
+
+        rows = [self.row1, self.row2, self.row3]
+
+        self.assertFalse(self.path.exists())
+        writer = RawDataWriter(self.path,
+                               daq_type=self.daq_type,
+                               sample_rate=self.sample_rate,
+                               columns=self.columns)
+        writer.__enter__()
+        writer.writerows(rows)
+        writer.__exit__()
+
+        self.assertTrue(self.path.exists())
+        loaded_data = RawData.load(self.path)
+
+        self.assertEqual(loaded_data.daq_type, self.daq_type)
+        self.assertEqual(loaded_data.sample_rate, self.sample_rate)
+        self.assertEqual(loaded_data.columns, self.columns)
+
+        self.assertEqual(len(loaded_data.rows), 3)
+
+    def test_sample_data(self):
+        """Test that sample data can be generated for testing purposes."""
+        channels = ['ch1', 'ch2', 'ch3']
+        data = sample_data(rows=5, ch_names=channels)
+        self.assertEqual(5, len(data.rows))
+        self.assertEqual(['timestamp', 'ch1', 'ch2', 'ch3', 'TRG'],
+                         data.columns)
+        self.assertEqual(1, data.rows[0][0])
+        self.assertEqual(5, data.rows[4][0])
+
+        # Test data range of channel columns
+        for row in data.rows:
+            for col in row[1:-1]:
+                self.assertTrue(col >= -1000 and col <= 1000)
+
+    def test_sample_data_with_triggers(self):
+        """Test generating sample data with triggers at pre-defined timestamps.
+        This functionality is used primarily for other unit tests."""
+        channels = ['ch1', 'ch2', 'ch3']
+        data = sample_data(rows=10,
+                           ch_names=channels,
+                           triggers=[(1, 'A'), (5, 'B'), (10, 'C')])
+        self.assertEqual(10, len(data.rows))
+
+        trg_col = data.columns.index('TRG')
+        self.assertEqual('A', data.rows[0][trg_col])
+        self.assertEqual('B', data.rows[4][trg_col])
+        self.assertEqual('C', data.rows[9][trg_col])
+
+    def test_raw_data_numeric_channels(self):
+        """Tests that data channels can be extracted for analysis."""
+
+        columns = ['timestamp', 'ch1', 'ch2', 'ch3', 'TRG']
+        data = RawData(daq_type=self.daq_type,
+                       sample_rate=self.sample_rate,
+                       columns=columns)
+
+        row1 = [1, 1.0, 2.0, 3.0, '0.0']
+        row2 = [2, 4.0, 5.0, 6.0, 'A']
+        row3 = [3, 7.0, 8.0, 9.0, '0.0']
+
+        data.append(row1)
+        data.append(row2)
+        data.append(row3)
+
+        self.assertEqual(['ch1', 'ch2', 'ch3'], data.channels)
+
+        # Test numeric data frame
+        dataframe = pd.DataFrame(data=[[1, 1.0, 2.0, 3.0], [2, 4.0, 5.0, 6.0],
+                                       [3, 7.0, 8.0, 9.0]],
+                                 columns=['timestamp', 'ch1', 'ch2', 'ch3'])
+        self.assertTrue(np.all(dataframe == data.numeric_data))
+
+    def test_data_by_channel(self):
+        """Tests that data can be structured in column-order for analysis."""
+
+        columns = ['timestamp', 'ch1', 'ch2', 'TRG']
+        data = RawData(daq_type=self.daq_type,
+                       sample_rate=self.sample_rate,
+                       columns=columns)
+
+        data.append([1, 1.0, 2.0, '0.0'])
+        data.append([2, 4.0, 5.0, 'A'])
+        data.append([3, 7.0, 8.0, '0.0'])
+
+        arr, _ = data.by_channel()
+        self.assertEqual((2, 3), arr.shape)
+
+        self.assertTrue(len(data.channels), len(arr))
+        self.assertTrue(np.all(arr[0] == [1.0, 4.0, 7.0]),
+                        "Should have ch1 data")
+        self.assertTrue(np.all(arr[1] == [2.0, 5.0, 8.0]),
+                        "Should have ch2 data")
+
+    def test_data_by_channel_applies_transformation(self):
+        """Tests that data correctly structured, can have a transformation applied to it."""
+        columns = ['timestamp', 'ch1', 'ch2', 'TRG']
+        data = RawData(daq_type=self.daq_type,
+                       sample_rate=self.sample_rate,
+                       columns=columns)
+
+        data.append([1, 1.0, 2.0, '0.0'])
+        data.append([2, 4.0, 5.0, 'A'])
+        data.append([3, 7.0, 8.0, '0.0'])
+
+        transform = mock()
+        # note data here should be returned as a nd.array. for mocking we don't care as much
+        when(RawData).apply_transform(any(), transform).thenReturn((data, self.sample_rate))
+        resp, fs = data.by_channel(transform=transform)
+
+        self.assertEqual(self.sample_rate, fs)
+        self.assertEqual(resp, data)
+        verify(RawData, times=1).apply_transform(any(), transform)
+
+    def test_data_by_channel_map(self):
+        """Tests that when given a channel map, it will filter the numeric columns.
+
+        We assume most trigger columns will be removed (due to being read in as a string or object),
+        however some are numeric trigger channels and may require filtering with a channel map.
+        Other cases could be dropping bad channels.
+        """
+        columns = ['timestamp', 'ch1', 'ch2', 'TRG']
+        channel_map = [1, 1, 0]
+        expected_channels = ['ch1', 'ch2']
+        data = RawData(daq_type=self.daq_type,
+                       sample_rate=self.sample_rate,
+                       columns=columns)
+
+        data.append([1, 1.0, 2.0, 0.0])
+        data.append([2, 4.0, 5.0, 0.0])
+        data.append([3, 7.0, 8.0, 0.0])
+
+        arr, channels, _ = data.by_channel_map(channel_map=channel_map)
+
+        self.assertEqual((2, 3), arr.shape)
+
+        self.assertTrue(len(data.channels), len(arr))
+        self.assertTrue(np.all(arr[0] == [1.0, 4.0, 7.0]),
+                        "Should have ch1 data")
+        self.assertTrue(np.all(arr[1] == [2.0, 5.0, 8.0]),
+                        "Should have ch2 data")
+        self.assertEqual(channels, expected_channels)
+
+    def test_data_by_channel_map_applies_transformation(self):
+        """Tests that when given a channel map, it will filter the numeric columns.
+
+        We assume most trigger columns will be removed (due to being read in as a string or object),
+        however some are numeric trigger channels and may require filtering with a channel map.
+        Other cases could be dropping bad channels.
+        """
+        columns = ['timestamp', 'ch1', 'ch2', 'TRG']
+        channel_map = [1, 1, 1]
+        expected_channels = ['ch1', 'ch2', 'TRG']
+        data = RawData(daq_type=self.daq_type,
+                       sample_rate=self.sample_rate,
+                       columns=columns)
+
+        data.append([1, 1.0, 2.0, 0.0])
+        data.append([2, 4.0, 5.0, 0.0])
+        data.append([3, 7.0, 8.0, 0.0])
+
+        transform = mock()
+        expected_output, expected_fs = data.by_channel()
+        # note data here should be returned as a nd.array. for mocking we don't care as much
+        when(RawData).by_channel(transform).thenReturn((expected_output, expected_fs))
+        _, channels, fs = data.by_channel_map(channel_map=channel_map, transform=transform)
+
+        self.assertEqual(expected_fs, fs)
+        self.assertEqual(expected_channels, channels)
+        verify(RawData, times=1).by_channel(transform)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/tests/test_save.py` & `bcipy-2.0.1rc2/bcipy/helpers/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/tests/test_session.py` & `bcipy-2.0.1rc2/bcipy/helpers/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/tests/test_task.py` & `bcipy-2.0.1rc2/bcipy/helpers/tests/test_task.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,323 +1,351 @@
-import unittest
-
-from typing import List
-from collections import Counter
-from mockito import unstub, mock, when, verify, verifyStubbedInvocationsAreUsed
-
-import numpy as np
-import psychopy
-
-from bcipy.acquisition import LslAcquisitionClient
-from bcipy.acquisition.record import Record
-from bcipy.task.exceptions import InsufficientDataException
-
-from bcipy.helpers.task import (_float_val,
-                                calculate_stimulation_freq, construct_triggers,
-                                generate_targets, get_data_for_decision,
-                                get_key_press, target_info)
-
-
-class TestCalculateStimulationFreq(unittest.TestCase):
-    def test_calculate_stimulate_frequency_returns_number_less_one(self):
-        flash_time = 5
-        stimulation_frequency = calculate_stimulation_freq(flash_time)
-        expected = 1 / flash_time
-        self.assertEqual(stimulation_frequency, expected)
-
-    def test_calculate_stimulate_frequency_handles_zero(self):
-        flash_time = 0
-        with self.assertRaises(ZeroDivisionError):
-            calculate_stimulation_freq(flash_time)
-
-
-class TestFloatVal(unittest.TestCase):
-    def test_float_val_as_str(self):
-        col = 'Apple'
-        result = _float_val(col)
-        expected = 1.0
-        self.assertEqual(result, expected)
-
-    def test_float_val_as_int(self):
-        col = 3
-        result = _float_val(col)
-        expected = 3.0
-        self.assertEqual(result, expected)
-
-
-class TestTargetGeneration(unittest.TestCase):
-    """Tests for generation of target inquiries"""
-
-    def test_target_number_less_than_alp(self):
-        """Test when requested number of targets is less than the length of
-        the alphabet."""
-        alp = list(range(10))
-        targets = generate_targets(alp, 5)
-        self.assertEqual(len(targets), 5)
-        self.assertEqual(len(targets), len(set(targets)))
-
-    def test_target_greater_than_alp(self):
-        """Test behavior when number of targets is greater than the length
-        of the alphabet"""
-        alp = list(range(5))
-        targets = generate_targets(alp, 10)
-        self.assertEqual(len(targets), 10)
-
-        counts = Counter(targets)
-
-        for item in alp:
-            self.assertEqual(counts[item], 2)
-
-    def test_remainder(self):
-        """Test behavior when number of targets is greater than the length of
-        the alphabet by a value other than a multiple of the alphabet length.
-        """
-        alp = list(range(5))
-        targets = generate_targets(alp, 12)
-
-        counts = Counter(targets)
-        for item in alp:
-            self.assertGreaterEqual(counts[item], 2)
-            self.assertLessEqual(counts[item], 3)
-
-
-class TestGetKeyPress(unittest.TestCase):
-    """Tests for the get key press method"""
-
-    def tearDown(self):
-        verifyStubbedInvocationsAreUsed()
-        unstub()
-
-    def test_get_key_press_appends_stamp_label_defaults(self):
-        """Test for the stamp label defaults, ensures the calls occur with the correct inputs to psychopy"""
-        key_list = ['space']
-        clock = mock()
-        # get keys returns a list of lists with the key and timestamp per hit
-        key_response = [[key_list[0], 1000]]
-        when(psychopy.event).getKeys(keyList=key_list,
-                                     timeStamped=True).thenReturn(key_response)
-        when(clock).getTime().thenReturn(psychopy.core.getTime())
-        # use the default label
-        stamp_label = 'bcipy_key_press'
-        expected = [f'{stamp_label}_{key_response[0][0]}', key_response[0][1]]
-        response = get_key_press(key_list, clock)
-        self.assertEqual(expected[0], response[0])
-        self.assertAlmostEqual(expected[1], response[1], delta=0.01)
-
-    def test_get_key_press_clock_adjustment(self):
-        """Test for the stamp label defaults, ensures the calls occur with the correct inputs to psychopy"""
-        key_list = ['space']
-        clock = mock()
-        # get keys returns a list of lists with the key and timestamp per hit
-        key_response = [[key_list[0], 1000]]
-        when(psychopy.event).getKeys(keyList=key_list,
-                                     timeStamped=True).thenReturn(key_response)
-        when(clock).getTime().thenReturn(psychopy.core.getTime() + 100)
-        # use the default label
-        stamp_label = 'bcipy_key_press'
-        expected = [f'{stamp_label}_{key_response[0][0]}', key_response[0][1]]
-        response = get_key_press(key_list, clock)
-        self.assertEqual(expected[0], response[0])
-        self.assertAlmostEqual(1100, response[1], delta=0.01)
-
-    def test_get_key_press_returns_none_if_no_keys_pressed(self):
-        """Test for the case not keys are returned, ensures the calls occur with the correct inputs to psychopy"""
-
-        key_list = ['space']
-        key_response = None
-        clock = mock()
-        when(psychopy.event).getKeys(keyList=key_list,
-                                     timeStamped=True).thenReturn(key_response)
-
-        response = get_key_press(key_list, clock)
-        self.assertEqual(None, response)
-
-    def test_get_key_press_set_custom_stamp_message(self):
-        """Test for a custom stamp label, ensures the calls occur with the correct inputs to psychopy"""
-        clock = mock()
-        key_list = ['space']
-        # get keys returns a list of lists with the key and timestamp per hit
-        key_response = [[key_list[0], 1000]]
-        when(psychopy.event).getKeys(keyList=key_list,
-                                     timeStamped=True).thenReturn(key_response)
-        when(clock).getTime().thenReturn(psychopy.core.getTime())
-        # set a custom label
-        stamp_label = 'custom_label'
-        expected = [f'{stamp_label}_{key_response[0][0]}', key_response[0][1]]
-        response = get_key_press(key_list, clock, stamp_label=stamp_label)
-        self.assertEqual(expected[0], response[0])
-        self.assertAlmostEqual(expected[1], response[1], delta=0.01)
-
-
-class TestTriggers(unittest.TestCase):
-    """Tests related to triggers"""
-
-    def test_construct_triggers(self):
-        stim_times = [['+', 7.009946188016329], ['<', 7.477798109990545],
-                      ['_', 7.69470399999409], ['Z', 7.911495972017292],
-                      ['U', 8.128477902995655], ['S', 8.345279764995212],
-                      ['T', 8.562265532993479], ['V', 8.779025560012087],
-                      ['X', 8.995945784990909], ['Y', 9.213076218002243],
-                      ['W', 9.429835998016642]]
-        expected = [('+', 0.0), ('<', 0.46785192197421566),
-                    ('_', 0.6847578119777609), ('Z', 0.901549784000963),
-                    ('U', 1.1185317149793264), ('S', 1.3353335769788828),
-                    ('T', 1.5523193449771497), ('V', 1.7690793719957583),
-                    ('X', 1.9859995969745796), ('Y', 2.203130029985914),
-                    ('W', 2.4198898100003134)]
-        self.assertEqual(expected, construct_triggers(stim_times))
-        self.assertEqual([], construct_triggers([]))
-
-    def test_target_info(self):
-        triggers = [('+', 0.0), ('<', 0.46785192197421566),
-                    ('_', 0.6847578119777609), ('Z', 0.901549784000963),
-                    ('U', 1.1185317149793264), ('S', 1.3353335769788828),
-                    ('T', 1.5523193449771497), ('V', 1.7690793719957583),
-                    ('X', 1.9859995969745796), ('Y', 2.203130029985914),
-                    ('W', 2.4198898100003134)]
-        expected = [
-            'fixation', 'nontarget', 'nontarget', 'target', 'nontarget',
-            'nontarget', 'nontarget', 'nontarget', 'nontarget', 'nontarget',
-            'nontarget'
-        ]
-        self.assertEqual(expected, target_info(triggers, target_letter='Z'))
-
-        expected = [
-            'fixation', 'nontarget', 'nontarget', 'nontarget', 'nontarget',
-            'nontarget', 'nontarget', 'nontarget', 'nontarget', 'nontarget',
-            'nontarget'
-        ]
-        self.assertEqual(expected, target_info(triggers))
-        self.assertEqual([], target_info([]))
-
-
-def mock_get_data_response(samples: int, high: float, low: float,
-                           channels: int) -> List[Record]:
-    """Mock DataAcquisitionClient Response.
-
-    The data acquisition client returns a list of records that need to be looped through
-        to get the raw data without other items attached.
-    """
-    data = [np.random.uniform(low, high) for _ in range(channels)]
-    record_data = []
-    for i in range(samples):
-        record_data.append(Record(data, i, None))
-    return record_data
-
-
-class TestGetDataForDecision(unittest.TestCase):
-    def setUp(self) -> None:
-        self.inquiry_timing = [('A', 1), ('B', 2), ('C', 3)]
-        self.daq = mock(spec=LslAcquisitionClient)
-        self.daq.device_spec = mock()
-        self.daq.device_spec.sample_rate = 10
-        self.mock_eeg = mock_get_data_response(samples=1000,
-                                               high=1000,
-                                               low=-1000,
-                                               channels=4)
-
-    def tearDown(self) -> None:
-        unstub()
-
-    def test_get_data_for_decision_returns_tuple_of_eeg_data_and_triggers(
-            self):
-        when(self.daq).get_data(start=any, limit=any).thenReturn(self.mock_eeg)
-
-        response = get_data_for_decision(self.inquiry_timing, self.daq)
-
-        self.assertIsInstance(response, tuple)
-
-        _eeg_data, timing = response
-
-        # self.assertEqual(eeg_data[:1][0], self.mock_eeg[0].data[0])
-        self.assertIsInstance(timing, list)
-
-    def test_get_data_for_decision_prestim(self):
-        prestim = 1
-        first_stim_time = self.inquiry_timing[0][1]
-        last_stim_time = self.inquiry_timing[-1][1]
-
-        expected_start = first_stim_time - prestim
-        expected_stop = last_stim_time
-        expected_triggers = [(text, ((timing - first_stim_time) + prestim))
-                             for text, timing in self.inquiry_timing]
-        expected_data_limit = round((expected_stop - expected_start) *
-                                    self.daq.device_spec.sample_rate)
-
-        when(self.daq).get_data(start=expected_start,
-                                limit=expected_data_limit).thenReturn(
-                                    self.mock_eeg)
-        _, timing = get_data_for_decision(self.inquiry_timing,
-                                          self.daq,
-                                          prestim=prestim)
-
-        # self.assertEqual(eeg_data[:1][0], self.mock_eeg[0].data[0])
-        self.assertEqual(timing, expected_triggers)
-        verify(self.daq, times=1).get_data(start=expected_start,
-                                           limit=expected_data_limit)
-
-    def test_get_data_for_decision_poststim(self):
-        poststim = 1
-        first_stim_time = self.inquiry_timing[0][1]
-        last_stim_time = self.inquiry_timing[-1][1]
-
-        expected_triggers = [(text, ((timing) - first_stim_time))
-                             for text, timing in self.inquiry_timing]
-        expected_data_limit = round(
-            (last_stim_time - first_stim_time + poststim) *
-            self.daq.device_spec.sample_rate)
-
-        when(self.daq).get_data(start=first_stim_time,
-                                limit=expected_data_limit).thenReturn(
-                                    self.mock_eeg)
-        _, timing = get_data_for_decision(self.inquiry_timing,
-                                          self.daq,
-                                          poststim=poststim)
-
-        # self.assertEqual(eeg_data[:1][0], self.mock_eeg[0].data[0])
-        self.assertEqual(timing, expected_triggers)
-        verify(self.daq, times=1).get_data(start=first_stim_time,
-                                           limit=expected_data_limit)
-
-    def test_get_data_for_decision_offset(self):
-        offset = 1
-        first_stim_time = self.inquiry_timing[0][1]
-        last_stim_time = self.inquiry_timing[-1][1]
-
-        expected_start = first_stim_time + offset
-        expected_stop = last_stim_time + offset
-        expected_triggers = [(text, ((timing) - first_stim_time))
-                             for text, timing in self.inquiry_timing]
-        expected_data_limit = round((expected_stop - expected_start) *
-                                    self.daq.device_spec.sample_rate)
-
-        when(self.daq).get_data(start=expected_start,
-                                limit=expected_data_limit).thenReturn(
-                                    self.mock_eeg)
-        _, timing = get_data_for_decision(self.inquiry_timing,
-                                          self.daq,
-                                          offset=offset)
-
-        # self.assertEqual(eeg_data[:1][0], self.mock_eeg[0].data[0])
-        self.assertEqual(timing, expected_triggers)
-        verify(self.daq, times=1).get_data(start=expected_start,
-                                           limit=expected_data_limit)
-
-    def test_get_data_for_decision_throws_insufficient_data_error_if_less_than_data_limit(
-            self):
-
-        # return an empty list from the get data call
-        when(self.daq).get_data(start=any, limit=any).thenReturn([])
-
-        with self.assertRaises(InsufficientDataException):
-            get_data_for_decision(self.inquiry_timing, self.daq)
-
-    def test_get_data_for_decision_throws_insufficient_data_error_if_data_query_out_of_bounds(
-            self):
-        inquiry_timing = [('A', 10), ('D', 1)]
-
-        with self.assertRaises(InsufficientDataException):
-            get_data_for_decision(inquiry_timing, self.daq)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+
+from typing import List
+from collections import Counter
+from mockito import unstub, mock, when, verify, verifyStubbedInvocationsAreUsed
+
+import numpy as np
+import psychopy
+
+from bcipy.acquisition import LslAcquisitionClient
+from bcipy.acquisition.record import Record
+from bcipy.task.exceptions import InsufficientDataException
+
+from bcipy.helpers.task import (_float_val, alphabet,
+                                calculate_stimulation_freq, construct_triggers,
+                                generate_targets, get_data_for_decision,
+                                get_key_press, target_info)
+
+
+class TestAlphabet(unittest.TestCase):
+    def test_alphabet_text(self):
+        parameters = {}
+
+        parameters['is_txt_stim'] = True
+
+        alp = alphabet(parameters)
+
+        self.assertEqual(alp, [
+            'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M',
+            'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z',
+            '<', '_'
+        ])
+
+    def test_alphabet_images(self):
+        parameters = {}
+        parameters['is_txt_stim'] = False
+        parameters['path_to_presentation_images'] = ('bcipy/static/images/'
+                                                     'rsvp/')
+
+        alp = alphabet(parameters)
+
+        self.assertNotEqual(alp, [
+            'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M',
+            'N', 'O', 'P', 'R', 'S', 'T', 'U', 'V', 'Y', 'Z', '<', '_'
+        ])
+
+
+class TestCalculateStimulationFreq(unittest.TestCase):
+    def test_calculate_stimulate_frequency_returns_number_less_one(self):
+        flash_time = 5
+        stimulation_frequency = calculate_stimulation_freq(flash_time)
+        expected = 1 / flash_time
+        self.assertEqual(stimulation_frequency, expected)
+
+    def test_calculate_stimulate_frequency_handles_zero(self):
+        flash_time = 0
+        with self.assertRaises(ZeroDivisionError):
+            calculate_stimulation_freq(flash_time)
+
+
+class TestFloatVal(unittest.TestCase):
+    def test_float_val_as_str(self):
+        col = 'Apple'
+        result = _float_val(col)
+        expected = 1.0
+        self.assertEqual(result, expected)
+
+    def test_float_val_as_int(self):
+        col = 3
+        result = _float_val(col)
+        expected = 3.0
+        self.assertEqual(result, expected)
+
+
+class TestTargetGeneration(unittest.TestCase):
+    """Tests for generation of target inquiries"""
+
+    def test_target_number_less_than_alp(self):
+        """Test when requested number of targets is less than the length of
+        the alphabet."""
+        alp = list(range(10))
+        targets = generate_targets(alp, 5)
+        self.assertEqual(len(targets), 5)
+        self.assertEqual(len(targets), len(set(targets)))
+
+    def test_target_greater_than_alp(self):
+        """Test behavior when number of targets is greater than the length
+        of the alphabet"""
+        alp = list(range(5))
+        targets = generate_targets(alp, 10)
+        self.assertEqual(len(targets), 10)
+
+        counts = Counter(targets)
+
+        for item in alp:
+            self.assertEqual(counts[item], 2)
+
+    def test_remainder(self):
+        """Test behavior when number of targets is greater than the length of
+        the alphabet by a value other than a multiple of the alphabet length.
+        """
+        alp = list(range(5))
+        targets = generate_targets(alp, 12)
+
+        counts = Counter(targets)
+        for item in alp:
+            self.assertGreaterEqual(counts[item], 2)
+            self.assertLessEqual(counts[item], 3)
+
+
+class TestGetKeyPress(unittest.TestCase):
+    """Tests for the get key press method"""
+
+    def tearDown(self):
+        verifyStubbedInvocationsAreUsed()
+        unstub()
+
+    def test_get_key_press_appends_stamp_label_defaults(self):
+        """Test for the stamp label defaults, ensures the calls occur with the correct inputs to psychopy"""
+        key_list = ['space']
+        clock = mock()
+        # get keys returns a list of lists with the key and timestamp per hit
+        key_response = [[key_list[0], 1000]]
+        when(psychopy.event).getKeys(keyList=key_list,
+                                     timeStamped=True).thenReturn(key_response)
+        when(clock).getTime().thenReturn(psychopy.core.getTime())
+        # use the default label
+        stamp_label = 'bcipy_key_press'
+        expected = [f'{stamp_label}_{key_response[0][0]}', key_response[0][1]]
+        response = get_key_press(key_list, clock)
+        self.assertEqual(expected[0], response[0])
+        self.assertAlmostEqual(expected[1], response[1], delta=0.01)
+
+    def test_get_key_press_clock_adjustment(self):
+        """Test for the stamp label defaults, ensures the calls occur with the correct inputs to psychopy"""
+        key_list = ['space']
+        clock = mock()
+        # get keys returns a list of lists with the key and timestamp per hit
+        key_response = [[key_list[0], 1000]]
+        when(psychopy.event).getKeys(keyList=key_list,
+                                     timeStamped=True).thenReturn(key_response)
+        when(clock).getTime().thenReturn(psychopy.core.getTime() + 100)
+        # use the default label
+        stamp_label = 'bcipy_key_press'
+        expected = [f'{stamp_label}_{key_response[0][0]}', key_response[0][1]]
+        response = get_key_press(key_list, clock)
+        self.assertEqual(expected[0], response[0])
+        self.assertAlmostEqual(1100, response[1], delta=0.01)
+
+    def test_get_key_press_returns_none_if_no_keys_pressed(self):
+        """Test for the case not keys are returned, ensures the calls occur with the correct inputs to psychopy"""
+
+        key_list = ['space']
+        key_response = None
+        clock = mock()
+        when(psychopy.event).getKeys(keyList=key_list,
+                                     timeStamped=True).thenReturn(key_response)
+
+        response = get_key_press(key_list, clock)
+        self.assertEqual(None, response)
+
+    def test_get_key_press_set_custom_stamp_message(self):
+        """Test for a custom stamp label, ensures the calls occur with the correct inputs to psychopy"""
+        clock = mock()
+        key_list = ['space']
+        # get keys returns a list of lists with the key and timestamp per hit
+        key_response = [[key_list[0], 1000]]
+        when(psychopy.event).getKeys(keyList=key_list,
+                                     timeStamped=True).thenReturn(key_response)
+        when(clock).getTime().thenReturn(psychopy.core.getTime())
+        # set a custom label
+        stamp_label = 'custom_label'
+        expected = [f'{stamp_label}_{key_response[0][0]}', key_response[0][1]]
+        response = get_key_press(key_list, clock, stamp_label=stamp_label)
+        self.assertEqual(expected[0], response[0])
+        self.assertAlmostEqual(expected[1], response[1], delta=0.01)
+
+
+class TestTriggers(unittest.TestCase):
+    """Tests related to triggers"""
+
+    def test_construct_triggers(self):
+        stim_times = [['+', 7.009946188016329], ['<', 7.477798109990545],
+                      ['_', 7.69470399999409], ['Z', 7.911495972017292],
+                      ['U', 8.128477902995655], ['S', 8.345279764995212],
+                      ['T', 8.562265532993479], ['V', 8.779025560012087],
+                      ['X', 8.995945784990909], ['Y', 9.213076218002243],
+                      ['W', 9.429835998016642]]
+        expected = [('+', 0.0), ('<', 0.46785192197421566),
+                    ('_', 0.6847578119777609), ('Z', 0.901549784000963),
+                    ('U', 1.1185317149793264), ('S', 1.3353335769788828),
+                    ('T', 1.5523193449771497), ('V', 1.7690793719957583),
+                    ('X', 1.9859995969745796), ('Y', 2.203130029985914),
+                    ('W', 2.4198898100003134)]
+        self.assertEqual(expected, construct_triggers(stim_times))
+        self.assertEqual([], construct_triggers([]))
+
+    def test_target_info(self):
+        triggers = [('+', 0.0), ('<', 0.46785192197421566),
+                    ('_', 0.6847578119777609), ('Z', 0.901549784000963),
+                    ('U', 1.1185317149793264), ('S', 1.3353335769788828),
+                    ('T', 1.5523193449771497), ('V', 1.7690793719957583),
+                    ('X', 1.9859995969745796), ('Y', 2.203130029985914),
+                    ('W', 2.4198898100003134)]
+        expected = [
+            'fixation', 'nontarget', 'nontarget', 'target', 'nontarget',
+            'nontarget', 'nontarget', 'nontarget', 'nontarget', 'nontarget',
+            'nontarget'
+        ]
+        self.assertEqual(expected, target_info(triggers, target_letter='Z'))
+
+        expected = [
+            'fixation', 'nontarget', 'nontarget', 'nontarget', 'nontarget',
+            'nontarget', 'nontarget', 'nontarget', 'nontarget', 'nontarget',
+            'nontarget'
+        ]
+        self.assertEqual(expected, target_info(triggers))
+        self.assertEqual([], target_info([]))
+
+
+def mock_get_data_response(samples: int, high: float, low: float,
+                           channels: int) -> List[Record]:
+    """Mock DataAcquisitionClient Response.
+
+    The data acquisition client returns a list of records that need to be looped through
+        to get the raw data without other items attached.
+    """
+    data = [np.random.uniform(low, high) for _ in range(channels)]
+    record_data = []
+    for i in range(samples):
+        record_data.append(Record(data, i, None))
+    return record_data
+
+
+class TestGetDataForDecision(unittest.TestCase):
+    def setUp(self) -> None:
+        self.inquiry_timing = [('A', 1), ('B', 2), ('C', 3)]
+        self.daq = mock(spec=LslAcquisitionClient)
+        self.daq.device_spec = mock()
+        self.daq.device_spec.sample_rate = 10
+        self.mock_eeg = mock_get_data_response(samples=1000,
+                                               high=1000,
+                                               low=-1000,
+                                               channels=4)
+
+    def tearDown(self) -> None:
+        unstub()
+
+    def test_get_data_for_decision_returns_tuple_of_eeg_data_and_triggers(
+            self):
+        when(self.daq).get_data(start=any, limit=any).thenReturn(self.mock_eeg)
+
+        response = get_data_for_decision(self.inquiry_timing, self.daq)
+
+        self.assertIsInstance(response, tuple)
+
+        _eeg_data, timing = response
+
+        # self.assertEqual(eeg_data[:1][0], self.mock_eeg[0].data[0])
+        self.assertIsInstance(timing, list)
+
+    def test_get_data_for_decision_prestim(self):
+        prestim = 1
+        first_stim_time = self.inquiry_timing[0][1]
+        last_stim_time = self.inquiry_timing[-1][1]
+
+        expected_start = first_stim_time - prestim
+        expected_stop = last_stim_time
+        expected_triggers = [(text, ((timing - first_stim_time) + prestim))
+                             for text, timing in self.inquiry_timing]
+        expected_data_limit = round((expected_stop - expected_start) *
+                                    self.daq.device_spec.sample_rate)
+
+        when(self.daq).get_data(start=expected_start,
+                                limit=expected_data_limit).thenReturn(
+                                    self.mock_eeg)
+        _, timing = get_data_for_decision(self.inquiry_timing,
+                                          self.daq,
+                                          prestim=prestim)
+
+        # self.assertEqual(eeg_data[:1][0], self.mock_eeg[0].data[0])
+        self.assertEqual(timing, expected_triggers)
+        verify(self.daq, times=1).get_data(start=expected_start,
+                                           limit=expected_data_limit)
+
+    def test_get_data_for_decision_poststim(self):
+        poststim = 1
+        first_stim_time = self.inquiry_timing[0][1]
+        last_stim_time = self.inquiry_timing[-1][1]
+
+        expected_triggers = [(text, ((timing) - first_stim_time))
+                             for text, timing in self.inquiry_timing]
+        expected_data_limit = round(
+            (last_stim_time - first_stim_time + poststim) *
+            self.daq.device_spec.sample_rate)
+
+        when(self.daq).get_data(start=first_stim_time,
+                                limit=expected_data_limit).thenReturn(
+                                    self.mock_eeg)
+        _, timing = get_data_for_decision(self.inquiry_timing,
+                                          self.daq,
+                                          poststim=poststim)
+
+        # self.assertEqual(eeg_data[:1][0], self.mock_eeg[0].data[0])
+        self.assertEqual(timing, expected_triggers)
+        verify(self.daq, times=1).get_data(start=first_stim_time,
+                                           limit=expected_data_limit)
+
+    def test_get_data_for_decision_offset(self):
+        offset = 1
+        first_stim_time = self.inquiry_timing[0][1]
+        last_stim_time = self.inquiry_timing[-1][1]
+
+        expected_start = first_stim_time + offset
+        expected_stop = last_stim_time + offset
+        expected_triggers = [(text, ((timing) - first_stim_time))
+                             for text, timing in self.inquiry_timing]
+        expected_data_limit = round((expected_stop - expected_start) *
+                                    self.daq.device_spec.sample_rate)
+
+        when(self.daq).get_data(start=expected_start,
+                                limit=expected_data_limit).thenReturn(
+                                    self.mock_eeg)
+        _, timing = get_data_for_decision(self.inquiry_timing,
+                                          self.daq,
+                                          offset=offset)
+
+        # self.assertEqual(eeg_data[:1][0], self.mock_eeg[0].data[0])
+        self.assertEqual(timing, expected_triggers)
+        verify(self.daq, times=1).get_data(start=expected_start,
+                                           limit=expected_data_limit)
+
+    def test_get_data_for_decision_throws_insufficient_data_error_if_less_than_data_limit(
+            self):
+
+        # return an empty list from the get data call
+        when(self.daq).get_data(start=any, limit=any).thenReturn([])
+
+        with self.assertRaises(InsufficientDataException):
+            get_data_for_decision(self.inquiry_timing, self.daq)
+
+    def test_get_data_for_decision_throws_insufficient_data_error_if_data_query_out_of_bounds(
+            self):
+        inquiry_timing = [('A', 10), ('D', 1)]
+
+        with self.assertRaises(InsufficientDataException):
+            get_data_for_decision(inquiry_timing, self.daq)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/tests/test_triggers.py` & `bcipy-2.0.1rc2/bcipy/helpers/tests/test_triggers.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/tests/test_validate.py` & `bcipy-2.0.1rc2/bcipy/helpers/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/triggers.py` & `bcipy-2.0.1rc2/bcipy/helpers/triggers.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/helpers/validate.py` & `bcipy-2.0.1rc2/bcipy/helpers/validate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,125 @@
-import os
-
-from bcipy.config import (
-    DEFAULT_EXPERIMENT_PATH,
-    DEFAULT_FIELD_PATH,
-    EXPERIMENT_FILENAME,
-    FIELD_FILENAME)
-from bcipy.helpers.load import load_experiments, load_fields
-from bcipy.helpers.system_utils import is_battery_powered, is_connected, is_screen_refresh_rate_low
-from bcipy.helpers.exceptions import (InvalidFieldException,
-                                      InvalidExperimentException,
-                                      UnregisteredExperimentException,
-                                      UnregisteredFieldException)
-from bcipy.gui.alert import confirm
-
-
-def validate_bcipy_session(parameters: dict, fake_data: bool) -> bool:
-    """Check pre-conditions for a BciPy session. If any possible problems are
-    detected, alert the user and prompt to continue.
-
-    Parameters
-    ----------
-    parameters - configuration used to check for issues
-
-    Returns
-    -------
-    True if it's okay to continue, otherwise False
-    """
-    possible_alerts = [(fake_data, '* Fake data is on.'),
-                       (is_connected(), '* Internet is on.'),
-                       (is_battery_powered(), '* Operating on battery power'),
-                       (is_screen_refresh_rate_low(), '* Screen refresh rate is low (< 120 Hz)')]
-    alert_messages = [
-        message for (condition, message) in possible_alerts if condition
-    ]
-    if alert_messages:
-        lines = [
-            "The following conditions may affect system behavior:\n",
-            *alert_messages, "\nDo you want to continue?"
-        ]
-        return confirm("\n".join(lines))
-    return True
-
-
-def validate_experiment(
-        experiment_name: str,
-        experiment_path: str = f'{DEFAULT_EXPERIMENT_PATH}/{EXPERIMENT_FILENAME}',
-        field_path: str = f'{DEFAULT_FIELD_PATH}/{FIELD_FILENAME}'
-) -> bool:
-    """Validate Experiment.
-
-    Validate the experiment is in the correct format and the fields are properly registered.
-    """
-    experiments = load_experiments(experiment_path)
-    fields = load_fields(field_path)
-
-    # attempt to load the experiment by name
-    try:
-        experiment = experiments[experiment_name]
-    except KeyError:
-        raise UnregisteredExperimentException(
-            f'Experiment [{experiment_name}] is not registered at path [{experiment_path}]')
-
-    # attempt to load the experiment by name
-    _validate_experiment_format(experiment, experiment_name)
-    _validate_experiment_fields(experiment['fields'], fields)
-
-    return True
-
-
-def _validate_experiment_fields(experiment_fields, fields):
-    # loop over the experiment fields and attempt to load them by name
-    for field in experiment_fields:
-        # field is a dictionary with one key another dictionary as its' value
-        # {'field_name': {require: bool, anonymize: bool}}
-        field_name = list(field.keys())[0]
-        try:
-            fields[field_name]
-        except KeyError:
-            raise UnregisteredFieldException(f'Field [{field}] is not registered in [{fields}]')
-
-        try:
-            field[field_name]['required']
-            field[field_name]['anonymize']
-        except KeyError:
-            raise InvalidFieldException(
-                f'Experiment Field [{field}] incorrectly formatted. It should contain: required and anonymize')
-
-
-def validate_field_data_written(path: str, file_name: str) -> bool:
-    """Validate Field Data Written
-
-    Validate that a field data file was written after executing the experiment field collection.
-    """
-    experiment_data_path = f'{path}/{file_name}'
-    if os.path.isfile(experiment_data_path):
-        return True
-    raise InvalidFieldException(f'Experimental field data expected at path=[{experiment_data_path}] but not found.')
-
-
-def validate_experiments(experiments, fields) -> bool:
-    """Validate Experiments.
-
-    Validate all experiments are in the correct format and the fields are properly registered.
-    """
-    for experiment_name in experiments:
-        experiment = experiments[experiment_name]
-
-        _validate_experiment_format(experiment, experiment_name)
-        _validate_experiment_fields(experiment['fields'], fields)
-
-    return True
-
-
-def _validate_experiment_format(experiment, name):
-    try:
-        exp_summary = experiment['summary']
-        assert isinstance(exp_summary, str)
-        experiment_fields = experiment['fields']
-        assert isinstance(experiment_fields, list)
-    except KeyError:
-        raise InvalidExperimentException(
-            f'Experiment [{name}] is formatted incorrectly. It should contain the keys: summary and fields.')
-    except AssertionError:
-        raise InvalidExperimentException(
-            f'Experiment [{name}] is formatted incorrectly. Unexpected type on summary(string) or fields(List[dict]).')
+import os
+
+from bcipy.config import (
+    DEFAULT_EXPERIMENT_PATH,
+    DEFAULT_FIELD_PATH,
+    EXPERIMENT_FILENAME,
+    FIELD_FILENAME)
+from bcipy.helpers.load import load_experiments, load_fields
+from bcipy.helpers.system_utils import is_battery_powered, is_connected
+from bcipy.helpers.exceptions import (InvalidFieldException,
+                                      InvalidExperimentException,
+                                      UnregisteredExperimentException,
+                                      UnregisteredFieldException)
+from bcipy.gui.alert import confirm
+
+
+def validate_bcipy_session(parameters: dict) -> bool:
+    """Check pre-conditions for a BciPy session. If any possible problems are
+    detected, alert the user and prompt to continue.
+
+    Parameters
+    ----------
+    parameters - configuration used to check for issues
+
+    Returns
+    -------
+    True if it's okay to continue, otherwise False
+    """
+    possible_alerts = [(parameters['fake_data'], '* Fake data is on.'),
+                       (is_connected(), '* Internet is on.'),
+                       (is_battery_powered(), '* Operating on battery power')]
+    alert_messages = [
+        message for (condition, message) in possible_alerts if condition
+    ]
+    if alert_messages:
+        lines = [
+            "The following conditions may affect system behavior:\n",
+            *alert_messages, "\nDo you want to continue?"
+        ]
+        return confirm("\n".join(lines))
+    return True
+
+
+def validate_experiment(
+        experiment_name: str,
+        experiment_path: str = f'{DEFAULT_EXPERIMENT_PATH}/{EXPERIMENT_FILENAME}',
+        field_path: str = f'{DEFAULT_FIELD_PATH}/{FIELD_FILENAME}'
+) -> bool:
+    """Validate Experiment.
+
+    Validate the experiment is in the correct format and the fields are properly registered.
+    """
+    experiments = load_experiments(experiment_path)
+    fields = load_fields(field_path)
+
+    # attempt to load the experiment by name
+    try:
+        experiment = experiments[experiment_name]
+    except KeyError:
+        raise UnregisteredExperimentException(
+            f'Experiment [{experiment_name}] is not registered at path [{experiment_path}]')
+
+    # attempt to load the experiment by name
+    _validate_experiment_format(experiment, experiment_name)
+    _validate_experiment_fields(experiment['fields'], fields)
+
+    return True
+
+
+def _validate_experiment_fields(experiment_fields, fields):
+    # loop over the experiment fields and attempt to load them by name
+    for field in experiment_fields:
+        # field is a dictionary with one key another dictionary as its' value
+        # {'field_name': {require: bool, anonymize: bool}}
+        field_name = list(field.keys())[0]
+        try:
+            fields[field_name]
+        except KeyError:
+            raise UnregisteredFieldException(f'Field [{field}] is not registered in [{fields}]')
+
+        try:
+            field[field_name]['required']
+            field[field_name]['anonymize']
+        except KeyError:
+            raise InvalidFieldException(
+                f'Experiment Field [{field}] incorrectly formatted. It should contain: required and anonymize')
+
+
+def validate_field_data_written(path: str, file_name: str) -> bool:
+    """Validate Field Data Written
+
+    Validate that a field data file was written after executing the experiment field collection.
+    """
+    experiment_data_path = f'{path}/{file_name}'
+    if os.path.isfile(experiment_data_path):
+        return True
+    raise InvalidFieldException(f'Experimental field data expected at path=[{experiment_data_path}] but not found.')
+
+
+def validate_experiments(experiments, fields) -> bool:
+    """Validate Experiments.
+
+    Validate all experiments are in the correct format and the fields are properly registered.
+    """
+    for experiment_name in experiments:
+        experiment = experiments[experiment_name]
+
+        _validate_experiment_format(experiment, experiment_name)
+        _validate_experiment_fields(experiment['fields'], fields)
+
+    return True
+
+
+def _validate_experiment_format(experiment, name):
+    try:
+        exp_summary = experiment['summary']
+        assert isinstance(exp_summary, str)
+        experiment_fields = experiment['fields']
+        assert isinstance(experiment_fields, list)
+    except KeyError:
+        raise InvalidExperimentException(
+            f'Experiment [{name}] is formatted incorrectly. It should contain the keys: summary and fields.')
+    except AssertionError:
+        raise InvalidExperimentException(
+            f'Experiment [{name}] is formatted incorrectly. Unexpected type on summary(string) or fields(List[dict]).')
```

### Comparing `bcipy-2.0.0rc3/bcipy/main.py` & `bcipy-2.0.1rc2/bcipy/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,262 +1,228 @@
-import argparse
-import logging
-import multiprocessing
-
-from typing import List
-
-from psychopy import visual
-
-from bcipy.acquisition import LslDataServer, ClientManager
-from bcipy.display import init_display_window
-from bcipy.config import DEFAULT_PARAMETERS_PATH, DEFAULT_EXPERIMENT_ID, STATIC_AUDIO_PATH
-from bcipy.helpers.acquisition import init_eeg_acquisition
-from bcipy.helpers.language_model import init_language_model
-from bcipy.helpers.load import (load_experiments, load_json_parameters,
-                                load_signal_model)
-from bcipy.helpers.save import init_save_data_structure
-from bcipy.helpers.session import collect_experiment_field_data
-from bcipy.helpers.stimuli import play_sound
-from bcipy.helpers.system_utils import configure_logger, get_system_info
-from bcipy.helpers.task import print_message
-from bcipy.helpers.validate import validate_experiment, validate_bcipy_session
-from bcipy.helpers.visualization import visualize_session_data
-from bcipy.signal.model import PcaRdaKdeModel
-from bcipy.task import TaskType
-from bcipy.task.start_task import start_task
-
-log = logging.getLogger(__name__)
-
-
-def bci_main(
-        parameter_location: str,
-        user: str,
-        task: TaskType,
-        experiment: str = DEFAULT_EXPERIMENT_ID,
-        alert: bool = False,
-        visualize: bool = True,
-        fake: bool = False) -> bool:
-    """BCI Main.
-
-    The BCI main function will initialize a save folder, construct needed information
-    and execute the task. This is the main connection between any UI and
-    running the app.
-
-    It may also be invoked via tha command line.
-        Ex. `bcipy` this will default parameters, mode, user, and type.
-
-        You can pass it those attributes with flags, if desired.
-            Ex. `bcipy --user "bci_user" --task "RSVP Calibration" --experiment "default"
-
-    Input:
-        parameter_location (str): location of parameters file to use
-        user (str): name of the user
-        task (TaskType): registered bcipy TaskType
-        experiment_id (str): Name of the experiment. Default name is DEFAULT_EXPERIMENT_ID.
-        alert (bool): whether to alert the user when the task is complete
-        visualize (bool): whether to visualize data at the end of a task
-        fake (bool): whether to use fake acquisition data during the session. If None, the
-            fake data will be determined by the parameters file.
-    """
-    validate_experiment(experiment)
-    # Load parameters
-    parameters = load_json_parameters(parameter_location, value_cast=True)
-
-    # cli overrides parameters file for fake data if provided
-    fake = fake if fake is True else parameters['fake_data']
-
-    if not validate_bcipy_session(parameters, fake):
-        return False
-
-    # Update property to reflect the parameter source
-    parameters['parameter_location'] = parameter_location
-    if parameter_location != DEFAULT_PARAMETERS_PATH:
-        parameters.save()
-        default_params = load_json_parameters(DEFAULT_PARAMETERS_PATH, value_cast=True)
-        if parameters.add_missing_items(default_params):
-            msg = 'Parameters file out of date.'
-            log.exception(msg)
-            raise Exception(msg)
-
-    # update our parameters file with system related information
-    sys_info = get_system_info()
-
-    # Initialize Save Folder
-    save_folder = init_save_data_structure(
-        parameters['data_save_loc'],
-        user,
-        parameter_location,
-        task=task.label,
-        experiment_id=experiment)
-
-    # configure bcipy session logging
-    configure_logger(save_folder,
-                     version=sys_info['bcipy_version'])
-
-    log.info(sys_info)
-
-    # Collect experiment field data
-    collect_experiment_field_data(experiment, save_folder)
-
-    if execute_task(task, parameters, save_folder, alert, fake):
-        if visualize:
-            visualize_session_data(save_folder, parameters)
-        return True
-
-    return False
-
-
-def execute_task(
-        task: TaskType,
-        parameters: dict,
-        save_folder: str,
-        alert: bool,
-        fake: bool) -> bool:
-    """Execute Task.
-
-    Executes the desired task by setting up the display window and
-        data acquisition, then passing on to the start_task function
-        which will initialize experiment.
-
-    Input:
-        (str): registered bcipy TaskType
-        parameters (dict): parameter dictionary
-        save_folder (str): path to save folder
-        alert (bool): whether to alert the user when the task is complete
-        fake (bool): whether to use fake acquisition data during the session
-
-    Returns:
-        (bool): True if the task was successfully executed, False otherwise
-    """
-    signal_model = None
-    language_model = None
-
-    # Init EEG Model, if needed. Calibration Tasks Don't require probabilistic
-    # modules to be loaded.
-    if task not in TaskType.calibration_tasks():
-        # Try loading in our signal_model and starting a langmodel(if enabled)
-        if not fake:
-            try:
-                signal_model, _filename = load_signal_model(
-                    model_class=PcaRdaKdeModel,
-                    model_kwargs={'k_folds': parameters['k_folds']},
-                    filename=parameters['signal_model_path'])
-            except Exception as e:
-                log.exception(f'Cannot load signal model. Exiting. {e}')
-                raise e
-
-        language_model = init_language_model(parameters)
-
-    # Initialize DAQ and export the device configuration
-    daq, servers = init_eeg_acquisition(
-        parameters, save_folder, server=fake)
-
-    # Initialize Display Window
-    # We have to wait until after the prompt to load the signal model before
-    # displaying the window, otherwise in fullscreen mode this throws an error
-    display = init_display_window(parameters)
-    print_message(display, f'Initializing {task}...')
-
-    # Start Task
-    try:
-        start_task(display,
-                   daq.get_client('EEG'),
-                   task,
-                   parameters,
-                   save_folder,
-                   language_model=language_model,
-                   signal_model=signal_model,
-                   fake=fake)
-
-    # If exception, close all display and acquisition objects
-    except Exception as e:
-        log.exception(str(e))
-
-    if alert:
-        play_sound(f"{STATIC_AUDIO_PATH}/{parameters['alert_sound_file']}")
-
-    return _clean_up_session(display, daq, servers)
-
-
-def _clean_up_session(
-        display: visual.Window,
-        daq: ClientManager,
-        servers: List[LslDataServer] = None) -> bool:
-    """Clean up session.
-
-    Closes the display window and data acquisition objects. Returns True if the session was closed successfully.
-
-    Input:
-        display (visual.Window): display window
-        daq (LslAcquisitionClient): data acquisition client
-        server (LslDataServer): data server
-    """
-    try:
-        # Stop Acquisition
-        daq.stop_acquisition()
-        daq.cleanup()
-
-        for server in servers:
-            server.stop()
-
-        # Close the display window
-        # NOTE: There is currently a bug in psychopy when attempting to shutdown
-        # windows when using a USB-C monitor. Putting the display close last in
-        # the inquiry allows acquisition to properly shutdown.
-        display.close()
-        return True
-    except Exception as e:
-        log.exception(str(e))
-        return False
-
-
-def bcipy_main() -> None:
-    """BciPy Main.
-
-    Command line interface used for running a registered experiment task in BciPy. To see what
-        is available use the --help flag.
-    """
-    # Needed for windows machines
-    multiprocessing.freeze_support()
-
-    experiment_options = list(load_experiments().keys())
-    task_options = TaskType.list()
-    parser = argparse.ArgumentParser()
-
-    # Command line utility for adding arguments/ paths via command line
-    parser.add_argument('-p', '--parameters', default=DEFAULT_PARAMETERS_PATH,
-                        help='Parameter location. Pass as *.json')
-    parser.add_argument('-u', '--user', default='test_user')
-    parser.add_argument('-t', '--task', default='RSVP Calibration',
-                        help=f'Task type to execute. Registered options: {task_options}')
-    parser.add_argument(
-        '-e',
-        '--experiment',
-        default=DEFAULT_EXPERIMENT_ID,
-        help=f'Select a valid experiment to run the task for this user. Available options: {experiment_options}')
-    parser.add_argument(
-        '-a',
-        '--alert',
-        default=False,
-        action='store_true',
-        help='Alert the user when the session is complete.')
-    parser.add_argument(
-        '-nv',
-        '--noviz',
-        default=True,
-        action='store_false',
-        help='Suppress visuals of the data after the session is complete.')
-    parser.add_argument(
-        '-f',
-        '--fake',
-        default=False,
-        action='store_true',
-        help='Use fake acquisition data for testing.')
-    args = parser.parse_args()
-
-    # Start BCI Main
-    bci_main(args.parameters, str(args.user), TaskType.by_value(str(args.task)),
-             str(args.experiment), args.alert, args.noviz, args.fake)
-
-
-if __name__ == '__main__':
-    bcipy_main()
+import argparse
+import logging
+import multiprocessing
+
+from typing import Optional
+
+from psychopy import visual
+
+from bcipy.acquisition import LslAcquisitionClient, LslDataServer
+from bcipy.display import init_display_window
+from bcipy.config import DEFAULT_PARAMETERS_PATH, DEFAULT_EXPERIMENT_ID, STATIC_AUDIO_PATH
+from bcipy.helpers.acquisition import init_eeg_acquisition
+from bcipy.helpers.language_model import init_language_model
+from bcipy.helpers.load import (load_experiments, load_json_parameters,
+                                load_signal_model)
+from bcipy.helpers.save import init_save_data_structure
+from bcipy.helpers.session import collect_experiment_field_data
+from bcipy.helpers.stimuli import play_sound
+from bcipy.helpers.system_utils import configure_logger, get_system_info
+from bcipy.helpers.task import print_message
+from bcipy.helpers.validate import validate_experiment, validate_bcipy_session
+from bcipy.signal.model import PcaRdaKdeModel
+from bcipy.task import TaskType
+from bcipy.task.start_task import start_task
+
+log = logging.getLogger(__name__)
+
+
+def bci_main(
+        parameter_location: str,
+        user: str,
+        task: TaskType,
+        experiment: str = DEFAULT_EXPERIMENT_ID,
+        alert: bool = False) -> bool:
+    """BCI Main.
+
+    The BCI main function will initialize a save folder, construct needed information
+    and execute the task. This is the main connection between any UI and
+    running the app.
+
+    It may also be invoked via tha command line.
+        Ex. `bcipy` this will default parameters, mode, user, and type.
+
+        You can pass it those attributes with flags, if desired.
+            Ex. `bcipy --user "bci_user" --task "RSVP Calibration" --experiment "default"
+
+    Input:
+        parameter_location (str): location of parameters file to use
+        user (str): name of the user
+        task (TaskType): registered bcipy TaskType
+        experiment_id (str): Name of the experiment. Default name is DEFAULT_EXPERIMENT_ID.
+        alert (bool): whether to alert the user when the task is complete
+    """
+    validate_experiment(experiment)
+    # Load parameters
+    parameters = load_json_parameters(parameter_location, value_cast=True)
+
+    if not validate_bcipy_session(parameters):
+        return False
+
+    # Update property to reflect the parameter source
+    parameters['parameter_location'] = parameter_location
+    if parameter_location != DEFAULT_PARAMETERS_PATH:
+        parameters.save()
+        default_params = load_json_parameters(DEFAULT_PARAMETERS_PATH, value_cast=True)
+        if parameters.add_missing_items(default_params):
+            msg = 'Parameters file out of date.'
+            log.exception(msg)
+            raise Exception(msg)
+
+    # update our parameters file with system related information
+    sys_info = get_system_info()
+
+    # Initialize Save Folder
+    save_folder = init_save_data_structure(
+        parameters['data_save_loc'],
+        user,
+        parameter_location,
+        task=task.label,
+        experiment_id=experiment)
+
+    # configure bcipy session logging
+    configure_logger(save_folder,
+                     version=sys_info['bcipy_version'])
+
+    log.info(sys_info)
+
+    # Collect experiment field data
+    collect_experiment_field_data(experiment, save_folder)
+
+    return execute_task(task, parameters, save_folder, alert)
+
+
+def execute_task(
+        task: TaskType,
+        parameters: dict,
+        save_folder: str,
+        alert: bool) -> bool:
+    """Execute Task.
+
+    Executes the desired task by setting up the display window and
+        data acquisition, then passing on to the start_task function
+        which will initialize experiment.
+
+    Input:
+        (str): registered bcipy TaskType
+        parameters (dict): parameter dictionary
+        save_folder (str): path to save folder
+        alert (bool): whether to alert the user when the task is complete
+    """
+    signal_model = None
+    language_model = None
+
+    fake = parameters['fake_data']
+
+    # Init EEG Model, if needed. Calibration Tasks Don't require probabilistic
+    # modules to be loaded.
+    if task not in TaskType.calibration_tasks():
+        # Try loading in our signal_model and starting a langmodel(if enabled)
+        if not fake:
+            try:
+                signal_model, _filename = load_signal_model(
+                    model_class=PcaRdaKdeModel,
+                    model_kwargs={'k_folds': parameters['k_folds']},
+                    filename=parameters['signal_model_path'])
+            except Exception as e:
+                log.exception(f'Cannot load signal model. Exiting. {e}')
+                raise e
+
+        language_model = init_language_model(parameters)
+
+    # Initialize DAQ and export the device configuration
+    daq, server = init_eeg_acquisition(
+        parameters, save_folder, export_spec=True, server=fake)
+
+    # Initialize Display Window
+    # We have to wait until after the prompt to load the signal model before
+    # displaying the window, otherwise in fullscreen mode this throws an error
+    display = init_display_window(parameters)
+    print_message(display, f'Initializing {task}...')
+
+    # Start Task
+    try:
+        start_task(
+            display, daq, task, parameters, save_folder,
+            language_model=language_model,
+            signal_model=signal_model, fake=fake)
+
+    # If exception, close all display and acquisition objects
+    except Exception as e:
+        log.exception(str(e))
+
+    if alert:
+        play_sound(f"{STATIC_AUDIO_PATH}/{parameters['alert_sound_file']}")
+
+    return _clean_up_session(display, daq, server)
+
+
+def _clean_up_session(
+        display: visual.Window,
+        daq: LslAcquisitionClient,
+        server: Optional[LslDataServer] = None) -> bool:
+    """Clean up session.
+
+    Closes the display window and data acquisition objects. Returns True if the session was closed successfully.
+
+    Input:
+        display (visual.Window): display window
+        daq (LslAcquisitionClient): data acquisition client
+        server (LslDataServer): data server
+    """
+    try:
+        # Stop Acquisition
+        daq.stop_acquisition()
+        daq.cleanup()
+
+        if server:
+            server.stop()
+
+        # Close the display window
+        # NOTE: There is currently a bug in psychopy when attempting to shutdown
+        # windows when using a USB-C monitor. Putting the display close last in
+        # the inquiry allows acquisition to properly shutdown.
+        display.close()
+        return True
+    except Exception as e:
+        log.exception(str(e))
+        return False
+
+
+def bcipy_main() -> None:
+    """BciPy Main.
+
+    Command line interface used for running a registered experiment task in Bcipy. To see what
+        is available use the --help flag.
+    """
+    # Needed for windows machines
+    multiprocessing.freeze_support()
+
+    experiment_options = list(load_experiments().keys())
+    task_options = TaskType.list()
+    parser = argparse.ArgumentParser()
+
+    # Command line utility for adding arguments/ paths via command line
+    parser.add_argument('-p', '--parameters', default=DEFAULT_PARAMETERS_PATH,
+                        help='Parameter location. Pass as *.json')
+    parser.add_argument('-u', '--user', default='test_user')
+    parser.add_argument('-t', '--task', default='RSVP Calibration',
+                        help=f'Task type to execute. Registered options: {task_options}')
+    parser.add_argument(
+        '-e',
+        '--experiment',
+        default=DEFAULT_EXPERIMENT_ID,
+        help=f'Select a valid experiment to run the task for this user. Available options: {experiment_options}')
+    parser.add_argument(
+        '-a',
+        '--alert',
+        default=False,
+        action='store_true',
+        help='Alert the user when the task is complete.')
+    args = parser.parse_args()
+
+    # Start BCI Main
+    bci_main(args.parameters, str(args.user), TaskType.by_value(str(args.task)), str(args.experiment), args.alert)
+
+
+if __name__ == '__main__':
+    bcipy_main()
```

### Comparing `bcipy-2.0.0rc3/bcipy/signal/evaluate/evaluator.py` & `bcipy-2.0.1rc2/bcipy/signal/evaluate/evaluator.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/signal/evaluate/rules.py` & `bcipy-2.0.1rc2/bcipy/signal/evaluate/rules.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/signal/model/base_model.py` & `bcipy-2.0.1rc2/bcipy/signal/model/base_model.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/signal/model/classifier.py` & `bcipy-2.0.1rc2/bcipy/signal/model/pca_rda_kde/classifier.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/signal/model/cross_validation.py` & `bcipy-2.0.1rc2/bcipy/signal/model/pca_rda_kde/cross_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,22 +37,22 @@
 
     model.pipeline[opt_el].lam = param[0]
     model.pipeline[opt_el].gam = param[1]
 
     fold_x, fold_y = [], []
     sc_h, y_valid_h = [], []
     if split == 'uniform':
-        for idx_fold in range(k_folds):
-            fold_x.append(x[:, int(idx_fold * fold_len):int((idx_fold + 1) * fold_len), :])
-            fold_y.append(y[int(idx_fold * fold_len):int((idx_fold + 1) * fold_len)])
-
-            if len(np.unique(fold_y[idx_fold])) != 2:
-                raise Exception(
-                    f'Cannot use {split}-folding in cross_validation '
-                    'or # of folds is inconsistent')
+        for idx_fold in range(k_folds + 1):
+            fold_x.append(x[:, int(idx_fold * fold_len):int(
+                (idx_fold + 1) * fold_len), :])
+            fold_y.append(y[int(idx_fold * fold_len):int((idx_fold + 1) *
+                                                         fold_len)])
+            if len(np.unique(fold_y[idx_fold])) == 1:
+                raise Exception('Cannot use {}-folding in cross_validation '
+                                'or # of folds is inconsistent'.format(split))
 
         for idx_fold in range(k_folds):
             list_valid = idx_fold
             list_train = list(set(range(k_folds)) - set([idx_fold]))
 
             x_train = np.concatenate([fold_x[i] for i in list_train], axis=1)
             y_train = np.concatenate([fold_y[i] for i in list_train], axis=0)
@@ -93,16 +93,16 @@
         init = [model.pipeline[opt_el].lam, model.pipeline[opt_el].gam]
     if op_type:
         # TODO: maybe we should not have such an option and set it by ourselves
         if op_type == 'cost_auc':
             k_folds, split = arg_op_type
 
             def cost_fun_param(b):
-                return cost_cross_validation_auc(model, opt_el, x, y, [b[0], b[1]],
-                                                 k_folds=k_folds, split=split)[0]
+                return cost_cross_validation_auc(model, opt_el, x, y, [b[0],
+                                                                       b[1]], k_folds=k_folds, split=split)[0]
 
         # Intervals for lambda and gamma parameters
         # Observe that 0 < lam < 1, 0 < gam < 1
         def cst_1(v):
 
             return v[0] - np.power(0.1, 15)
```

### Comparing `bcipy-2.0.0rc3/bcipy/signal/model/density_estimation.py` & `bcipy-2.0.1rc2/bcipy/signal/model/pca_rda_kde/density_estimation.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/signal/model/inquiry_preview.py` & `bcipy-2.0.1rc2/bcipy/signal/model/inquiry_preview.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/signal/model/offline_analysis.py` & `bcipy-2.0.1rc2/bcipy/signal/model/offline_analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,242 +1,215 @@
-import logging
-from pathlib import Path
-from typing import Tuple
-
-from bcipy.config import (DEFAULT_PARAMETERS_PATH, TRIGGER_FILENAME,
-                          RAW_DATA_FILENAME, STATIC_AUDIO_PATH,
-                          DEFAULT_DEVICE_SPEC_FILENAME)
-from bcipy.preferences import preferences
-from bcipy.helpers.acquisition import analysis_channels
-from bcipy.helpers.load import (
-    load_experimental_data,
-    load_json_parameters,
-    load_raw_data,
-)
-from bcipy.helpers.stimuli import play_sound, update_inquiry_timing
-from bcipy.helpers.system_utils import report_execution_time
-from bcipy.helpers.triggers import TriggerType, trigger_decoder
-from bcipy.helpers.visualization import visualize_erp
-from bcipy.signal.model.base_model import SignalModel
-from bcipy.signal.model.pca_rda_kde import PcaRdaKdeModel
-from bcipy.signal.process import filter_inquiries, get_default_transform
-
-import numpy as np
-from matplotlib.figure import Figure
-from sklearn.metrics import balanced_accuracy_score
-from sklearn.model_selection import train_test_split
-import bcipy.acquisition.devices as devices
-
-log = logging.getLogger(__name__)
-logging.basicConfig(level=logging.INFO, format="[%(threadName)-9s][%(asctime)s][%(name)s][%(levelname)s]: %(message)s")
-
-
-def subset_data(data: np.ndarray, labels: np.ndarray, test_size: float, random_state=0):
-    """Performs a train/test split on the provided data and labels, accounting for
-    the current shape convention (channel dimension in front, instead of batch dimension in front).
-
-    Args:
-        data (np.ndarray): Shape (channels, items, time)
-        labels (np.ndarray): Shape (items,)
-        test_size (float): fraction of data to be used for testing
-        random_state (int, optional): fixed random seed
-
-    Returns:
-        train_data (np.ndarray): Shape (channels, train_items, time)
-        test_data (np.ndarray): Shape (channels, test_items, time)
-        train_labels (np.ndarray): Shape (train_items,)
-        test_labels (np.ndarray): Shape (test_items,)
-    """
-    data = data.swapaxes(0, 1)
-    train_data, test_data, train_labels, test_labels = train_test_split(
-        data, labels, test_size=test_size, random_state=random_state
-    )
-    train_data = train_data.swapaxes(0, 1)
-    test_data = test_data.swapaxes(0, 1)
-    return train_data, test_data, train_labels, test_labels
-
-
-@report_execution_time
-def offline_analysis(
-    data_folder: str = None,
-    parameters: dict = {},
-    alert_finished: bool = True,
-    estimate_balanced_acc: bool = False,
-    show_figures: bool = False,
-    save_figures: bool = False,
-) -> Tuple[SignalModel, Figure]:
-    """Gets calibration data and trains the model in an offline fashion.
-    pickle dumps the model into a .pkl folder
-    Args:
-        data_folder(str): folder of the data
-            save all information and load all from this folder
-        parameter(dict): parameters for running offline analysis
-        alert_finished(bool): whether or not to alert the user offline analysis complete
-        estimate_balanced_acc(bool): if true, uses another model copy on an 80/20 split to
-            estimate balanced accuracy
-        show_figures(bool): if true, shows ERP figures after training
-        save_figures(bool): if true, saves ERP figures after training to the data folder
-
-    How it Works:
-    - reads data and information from a .csv calibration file
-    - reads trigger information from a .txt trigger file
-    - filters data
-    - reshapes and labels the data for the training procedure
-    - fits the model to the data
-        - uses cross validation to select parameters
-        - based on the parameters, trains system using all the data
-    - pickle dumps model into .pkl file
-    - generates and [optional] saves/shows the ERP figure
-    - [optional] alert the user finished processing
-    """
-
-    if not data_folder:
-        data_folder = load_experimental_data()
-
-    # extract relevant session information from parameters file
-    poststim_length = parameters.get("trial_length")
-    prestim_length = parameters.get("prestim_length")
-    trials_per_inquiry = parameters.get("stim_length")
-    # The task buffer length defines the min time between two inquiries
-    # We use half of that time here to buffer during transforms
-    buffer = int(parameters.get("task_buffer_length") / 2)
-    raw_data_file = f"{RAW_DATA_FILENAME}.csv"
-
-    # get signal filtering information
-    downsample_rate = parameters.get("down_sampling_rate")
-    notch_filter = parameters.get("notch_filter_frequency")
-    filter_high = parameters.get("filter_high")
-    filter_low = parameters.get("filter_low")
-    filter_order = parameters.get("filter_order")
-    static_offset = parameters.get("static_trigger_offset")
-
-    log.info(
-        f"\nData processing settings: \n"
-        f"Filter: [{filter_low}-{filter_high}], Order: {filter_order},"
-        f" Notch: {notch_filter}, Downsample: {downsample_rate} \n"
-        f"Poststimulus: {poststim_length}s, Prestimulus: {prestim_length}s, Buffer: {buffer}s \n"
-        f"Static offset: {static_offset}"
-    )
-
-    # Load raw data
-    raw_data = load_raw_data(Path(data_folder, raw_data_file))
-    channels = raw_data.channels
-    type_amp = raw_data.daq_type
-    sample_rate = raw_data.sample_rate
-
-    devices.load(Path(data_folder, DEFAULT_DEVICE_SPEC_FILENAME))
-    device_spec = devices.preconfigured_device(raw_data.daq_type)
-
-    # setup filtering
-    default_transform = get_default_transform(
-        sample_rate_hz=sample_rate,
-        notch_freq_hz=notch_filter,
-        bandpass_low=filter_low,
-        bandpass_high=filter_high,
-        bandpass_order=filter_order,
-        downsample_factor=downsample_rate,
-    )
-
-    log.info(f"Channels read from csv: {channels}")
-    log.info(f"Device type: {type_amp}, fs={sample_rate}")
-
-    k_folds = parameters.get("k_folds")
-    model = PcaRdaKdeModel(k_folds=k_folds)
-
-    # Process triggers.txt files
-    trigger_targetness, trigger_timing, trigger_symbols = trigger_decoder(
-        offset=static_offset,
-        trigger_path=f"{data_folder}/{TRIGGER_FILENAME}",
-        exclusion=[TriggerType.PREVIEW, TriggerType.EVENT, TriggerType.FIXATION],
-    )
-    # Channel map can be checked from raw_data.csv file or the devices.json located in the acquisition module
-    # The timestamp column [0] is already excluded.
-    channel_map = analysis_channels(channels, device_spec)
-    channels_used = [channels[i] for i, keep in enumerate(channel_map) if keep == 1]
-    log.info(f'Channels used in analysis: {channels_used}')
-
-    data, fs = raw_data.by_channel()
-
-    inquiries, inquiry_labels, inquiry_timing = model.reshaper(
-        trial_targetness_label=trigger_targetness,
-        timing_info=trigger_timing,
-        eeg_data=data,
-        sample_rate=sample_rate,
-        trials_per_inquiry=trials_per_inquiry,
-        channel_map=channel_map,
-        poststimulus_length=poststim_length,
-        prestimulus_length=prestim_length,
-        transformation_buffer=buffer,
-    )
-
-    inquiries, fs = filter_inquiries(inquiries, default_transform, sample_rate)
-    inquiry_timing = update_inquiry_timing(inquiry_timing, downsample_rate)
-    trial_duration_samples = int(poststim_length * fs)
-    data = model.reshaper.extract_trials(inquiries, trial_duration_samples, inquiry_timing)
-
-    # define the training classes using integers, where 0=nontargets/1=targets
-    labels = inquiry_labels.flatten()
-
-    # train and save the model as a pkl file
-    log.info("Training model. This will take some time...")
-    model = PcaRdaKdeModel(k_folds=k_folds)
-    model.fit(data, labels)
-    log.info(f"Training complete [AUC={model.auc:0.4f}]. Saving data...")
-
-    model.save(data_folder + f"/model_{model.auc:0.4f}.pkl")
-    preferences.signal_model_directory = data_folder
-
-    # Using an 80/20 split, report on balanced accuracy
-    if estimate_balanced_acc:
-        train_data, test_data, train_labels, test_labels = subset_data(data, labels, test_size=0.2)
-        dummy_model = PcaRdaKdeModel(k_folds=k_folds)
-        dummy_model.fit(train_data, train_labels)
-        probs = dummy_model.predict_proba(test_data)
-        preds = probs.argmax(-1)
-        score = balanced_accuracy_score(test_labels, preds)
-        log.info(f"Balanced acc with 80/20 split: {score}")
-        del dummy_model, train_data, test_data, train_labels, test_labels, probs, preds
-
-    figure_handles = visualize_erp(
-        raw_data,
-        channel_map,
-        trigger_timing,
-        labels,
-        poststim_length,
-        transform=default_transform,
-        plot_average=True,
-        plot_topomaps=True,
-        save_path=data_folder if save_figures else None,
-        show=show_figures
-    )
-    if alert_finished:
-        play_sound(f"{STATIC_AUDIO_PATH}/{parameters['alert_sound_file']}")
-    return model, figure_handles
-
-
-if __name__ == "__main__":
-    import argparse
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-d", "--data_folder", default=None)
-    parser.add_argument("-p", "--parameters_file", default=DEFAULT_PARAMETERS_PATH)
-    parser.add_argument("-s", "--save_figures", action="store_true")
-    parser.add_argument("-v", "--show_figures", action="store_true")
-    parser.add_argument("--alert", dest="alert", action="store_true")
-    parser.add_argument("--balanced-acc", dest="balanced", action="store_true")
-    parser.set_defaults(alert=False)
-    parser.set_defaults(balanced=False)
-    parser.set_defaults(save_figures=False)
-    parser.set_defaults(show_figures=False)
-    args = parser.parse_args()
-
-    log.info(f"Loading params from {args.parameters_file}")
-    parameters = load_json_parameters(args.parameters_file, value_cast=True)
-
-    offline_analysis(
-        args.data_folder,
-        parameters,
-        alert_finished=args.alert,
-        estimate_balanced_acc=args.balanced,
-        save_figures=args.save_figures,
-        show_figures=args.show_figures)
-    log.info("Offline Analysis complete.")
+import logging
+from pathlib import Path
+from typing import Tuple
+
+import numpy as np
+from bcipy.config import DEFAULT_PARAMETERS_PATH, TRIGGER_FILENAME, RAW_DATA_FILENAME, STATIC_AUDIO_PATH
+from bcipy.helpers.acquisition import analysis_channels
+from bcipy.helpers.load import (
+    load_experimental_data,
+    load_json_parameters,
+    load_raw_data,
+)
+from bcipy.helpers.stimuli import play_sound
+from bcipy.helpers.system_utils import report_execution_time
+from bcipy.helpers.triggers import TriggerType, trigger_decoder
+from bcipy.helpers.visualization import visualize_erp
+from bcipy.signal.model.base_model import SignalModel
+from bcipy.signal.model.pca_rda_kde import PcaRdaKdeModel
+from bcipy.signal.process import filter_inquiries, get_default_transform
+from matplotlib.figure import Figure
+from sklearn.metrics import balanced_accuracy_score
+from sklearn.model_selection import train_test_split
+
+log = logging.getLogger(__name__)
+logging.basicConfig(level=logging.INFO, format="[%(threadName)-9s][%(asctime)s][%(name)s][%(levelname)s]: %(message)s")
+
+
+def subset_data(data: np.ndarray, labels: np.ndarray, test_size: float, random_state=0):
+    """Performs a train/test split on the provided data and labels, accounting for
+    the current shape convention (channel dimension in front, instead of batch dimension in front).
+
+    Args:
+        data (np.ndarray): Shape (channels, items, time)
+        labels (np.ndarray): Shape (items,)
+        test_size (float): fraction of data to be used for testing
+        random_state (int, optional): fixed random seed
+
+    Returns:
+        train_data (np.ndarray): Shape (channels, train_items, time)
+        test_data (np.ndarray): Shape (channels, test_items, time)
+        train_labels (np.ndarray): Shape (train_items,)
+        test_labels (np.ndarray): Shape (test_items,)
+    """
+    data = data.swapaxes(0, 1)
+    train_data, test_data, train_labels, test_labels = train_test_split(
+        data, labels, test_size=test_size, random_state=random_state
+    )
+    train_data = train_data.swapaxes(0, 1)
+    test_data = test_data.swapaxes(0, 1)
+    return train_data, test_data, train_labels, test_labels
+
+
+@report_execution_time
+def offline_analysis(
+    data_folder: str = None,
+    parameters: dict = {},
+    alert_finished: bool = True,
+    estimate_balanced_acc: bool = False,
+    show_figures: bool = False,
+) -> Tuple[SignalModel, Figure]:
+    """Gets calibration data and trains the model in an offline fashion.
+    pickle dumps the model into a .pkl folder
+    Args:
+        data_folder(str): folder of the data
+            save all information and load all from this folder
+        parameter(dict): parameters for running offline analysis
+        alert_finished(bool): whether or not to alert the user offline analysis complete
+        estimate_balanced_acc(bool): if true, uses another model copy on an 80/20 split to
+            estimate balanced accuracy
+
+    How it Works:
+    - reads data and information from a .csv calibration file
+    - reads trigger information from a .txt trigger file
+    - filters data
+    - reshapes and labels the data for the training procedure
+    - fits the model to the data
+        - uses cross validation to select parameters
+        - based on the parameters, trains system using all the data
+    - pickle dumps model into .pkl file
+    - generates and saves ERP figure
+    - [optional] alert the user finished processing
+    """
+
+    if not data_folder:
+        data_folder = load_experimental_data()
+
+    # extract relevant session information from parameters file
+    poststim_length = parameters.get("trial_length")
+    prestim_length = parameters.get("prestim_length")
+    trials_per_inquiry = parameters.get("stim_length")
+    # The task buffer length defines the min time between two inquiries
+    # We use half of that time here to buffer during transforms
+    buffer = int(parameters.get("task_buffer_length") / 2)
+    raw_data_file = f"{RAW_DATA_FILENAME}.csv"
+
+    # get signal filtering information
+    downsample_rate = parameters.get("down_sampling_rate")
+    notch_filter = parameters.get("notch_filter_frequency")
+    filter_high = parameters.get("filter_high")
+    filter_low = parameters.get("filter_low")
+    filter_order = parameters.get("filter_order")
+    static_offset = parameters.get("static_trigger_offset")
+
+    log.info(
+        f"\nData processing settings: \n"
+        f"Filter: [{filter_low}-{filter_high}], Order: {filter_order},"
+        f" Notch: {notch_filter}, Downsample: {downsample_rate} \n"
+        f"Poststimulus: {poststim_length}s, Prestimulus: {prestim_length}s, Buffer: {buffer}s \n"
+        f"Static offset: {static_offset}"
+    )
+
+    # Load raw data
+    raw_data = load_raw_data(Path(data_folder, raw_data_file))
+    channels = raw_data.channels
+    type_amp = raw_data.daq_type
+    sample_rate = raw_data.sample_rate
+
+    # setup filtering
+    default_transform = get_default_transform(
+        sample_rate_hz=sample_rate,
+        notch_freq_hz=notch_filter,
+        bandpass_low=filter_low,
+        bandpass_high=filter_high,
+        bandpass_order=filter_order,
+        downsample_factor=downsample_rate,
+    )
+
+    log.info(f"Channels read from csv: {channels}")
+    log.info(f"Device type: {type_amp}, fs={sample_rate}")
+
+    k_folds = parameters.get("k_folds")
+    model = PcaRdaKdeModel(k_folds=k_folds)
+
+    # Process triggers.txt files
+    trigger_targetness, trigger_timing, trigger_symbols = trigger_decoder(
+        offset=static_offset,
+        trigger_path=f"{data_folder}/{TRIGGER_FILENAME}",
+        exclusion=[TriggerType.PREVIEW, TriggerType.EVENT, TriggerType.FIXATION],
+    )
+    # Channel map can be checked from raw_data.csv file or the devices.json located in the acquisition module
+    # The timestamp column [0] is already excluded.
+    channel_map = analysis_channels(channels, type_amp)
+    data, fs = raw_data.by_channel()
+
+    inquiries, inquiry_labels, inquiry_timing = model.reshaper(
+        trial_targetness_label=trigger_targetness,
+        timing_info=trigger_timing,
+        eeg_data=data,
+        sample_rate=sample_rate,
+        trials_per_inquiry=trials_per_inquiry,
+        channel_map=channel_map,
+        poststimulus_length=poststim_length,
+        prestimulus_length=prestim_length,
+        transformation_buffer=buffer,
+    )
+
+    inquiries, fs = filter_inquiries(inquiries, default_transform, sample_rate)
+    trial_duration_samples = int(poststim_length * fs)
+    data = model.reshaper.extract_trials(inquiries, trial_duration_samples, inquiry_timing, downsample_rate)
+
+    # define the training classes using integers, where 0=nontargets/1=targets
+    labels = inquiry_labels.flatten()
+
+    # train and save the model as a pkl file
+    log.info("Training model. This will take some time...")
+    model = PcaRdaKdeModel(k_folds=k_folds)
+    model.fit(data, labels)
+    log.info(f"Training complete [AUC={model.auc:0.4f}]. Saving data...")
+
+    model.save(data_folder + f"/model_{model.auc:0.4f}.pkl")
+
+    # Using an 80/20 split, report on balanced accuracy
+    if estimate_balanced_acc:
+        train_data, test_data, train_labels, test_labels = subset_data(data, labels, test_size=0.8)
+        dummy_model = PcaRdaKdeModel(k_folds=k_folds)
+        dummy_model.fit(train_data, train_labels)
+        probs = dummy_model.predict_proba(test_data)
+        preds = probs.argmax(-1)
+        log.info(f"Balanced acc with 80/20 split: {balanced_accuracy_score(test_labels, preds)}")
+        del dummy_model, train_data, test_data, train_labels, test_labels, probs, preds
+
+    figure_handles = visualize_erp(
+        raw_data,
+        channel_map,
+        trigger_timing,
+        labels,
+        poststim_length,
+        transform=default_transform,
+        plot_average=True,
+        plot_topomaps=True,
+        save_path=data_folder,
+        show=show_figures
+    )
+    if alert_finished:
+        play_sound(f"{STATIC_AUDIO_PATH}/{parameters['alert_sound_file']}")
+    return model, figure_handles
+
+
+if __name__ == "__main__":
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-d", "--data_folder", default=None)
+    parser.add_argument("-p", "--parameters_file", default=DEFAULT_PARAMETERS_PATH)
+    parser.add_argument("--alert", dest="alert", action="store_true")
+    parser.add_argument("--balanced-acc", dest="balanced", action="store_true")
+    parser.set_defaults(alert=False)
+    parser.set_defaults(balanced=False)
+    args = parser.parse_args()
+
+    log.info(f"Loading params from {args.parameters_file}")
+    parameters = load_json_parameters(args.parameters_file, value_cast=True)
+
+    offline_analysis(args.data_folder, parameters, alert_finished=args.alert, estimate_balanced_acc=args.balanced)
+    log.info("Offline Analysis complete.")
```

### Comparing `bcipy-2.0.0rc3/bcipy/signal/model/pca_rda_kde/pca_rda_kde.py` & `bcipy-2.0.1rc2/bcipy/signal/model/pca_rda_kde/pca_rda_kde.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 import pickle
 from pathlib import Path
 from typing import List
 
 import numpy as np
 from bcipy.signal.model import ModelEvaluationReport, SignalModel
-from bcipy.signal.model.classifier import RegularizedDiscriminantAnalysis
-from bcipy.signal.model.cross_validation import cost_cross_validation_auc, cross_validation
-from bcipy.signal.model.density_estimation import KernelDensityEstimate
-from bcipy.signal.model.dimensionality_reduction import ChannelWisePrincipalComponentAnalysis
-from bcipy.signal.model.pipeline import Pipeline
-from bcipy.helpers.exceptions import SignalException
+from bcipy.signal.model.pca_rda_kde.classifier import RegularizedDiscriminantAnalysis
+from bcipy.signal.model.pca_rda_kde.cross_validation import cost_cross_validation_auc, cross_validation
+from bcipy.signal.model.pca_rda_kde.density_estimation import KernelDensityEstimate
+from bcipy.signal.model.pca_rda_kde.dimensionality_reduction import ChannelWisePrincipalComponentAnalysis
+from bcipy.signal.model.pca_rda_kde.pipeline import Pipeline
+from bcipy.signal.exceptions import SignalException
 from bcipy.helpers.stimuli import InquiryReshaper
 
 
 class PcaRdaKdeModel(SignalModel):
     reshaper = InquiryReshaper()
 
     def __init__(self, k_folds: int, prior_type="uniform", pca_n_components=0.9):
         self.k_folds = k_folds
-        self.prior_type = prior_type
-        self.pca_n_components = pca_n_components
-        self.optimization_elements = 1  # number of elements to optimized (RDA)
-        # min and max values for the likelihood ratio output
-        self.min = 1e-2
-        self.max = 1e2
         self.model = None
         self.auc = None
+        self.prior_type = prior_type
+        self.pca_n_components = pca_n_components
         self._ready_to_predict = False
 
     def fit(self, train_data: np.array, train_labels: np.array) -> SignalModel:
         """
         Train on provided data using K-fold cross validation and return self.
 
         Parameters:
@@ -97,16 +93,15 @@
         if not self._ready_to_predict:
             raise SignalException("must use model.fit() before model.evaluate()")
 
         tmp_model = Pipeline([self.model.pipeline[0], self.model.pipeline[1]])
 
         lam_gam = (self.model.pipeline[1].lam, self.model.pipeline[1].gam)
         tmp, _, _ = cost_cross_validation_auc(
-            tmp_model, self.optimization_elements, test_data, test_labels,
-            lam_gam, k_folds=self.k_folds, split="uniform"
+            tmp_model, 1, test_data, test_labels, lam_gam, k_folds=self.k_folds, split="uniform"
         )
         auc = -tmp
         return ModelEvaluationReport(auc)
 
     def predict(self, data: np.array, inquiry: List[str], symbol_set: List[str]) -> np.array:
         """
         For each trial in `data`, compute a likelihood ratio to update that symbol's probability.
@@ -129,15 +124,15 @@
         if not self._ready_to_predict:
             raise SignalException("must use model.fit() before model.predict()")
 
         # Evaluate likelihood probabilities for p(e|l=1) and p(e|l=0)
         log_likelihoods = self.model.transform(data)
         subset_likelihood_ratios = np.exp(log_likelihoods[:, 1] - log_likelihoods[:, 0])
         # Restrict multiplicative updates to a reasonable range
-        subset_likelihood_ratios = np.clip(subset_likelihood_ratios, self.min, self.max)
+        subset_likelihood_ratios = np.clip(subset_likelihood_ratios, 1e-2, 1e2)
 
         # Apply likelihood ratios to entire symbol set.
         likelihood_ratios = np.ones(len(symbol_set))
         for idx in range(len(subset_likelihood_ratios)):
             likelihood_ratios[symbol_set.index(inquiry[idx])] *= subset_likelihood_ratios[idx]
         return likelihood_ratios
```

### Comparing `bcipy-2.0.0rc3/bcipy/signal/model/pipeline.py` & `bcipy-2.0.1rc2/bcipy/signal/model/pca_rda_kde/pipeline.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/signal/process/decomposition/psd.py` & `bcipy-2.0.1rc2/bcipy/signal/process/decomposition/psd.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 from enum import Enum
 from scipy.signal import welch
 from scipy.integrate import simps
 from mne.time_frequency import psd_array_multitaper
 
 from typing import Tuple
 
-from bcipy.helpers.exceptions import SignalException
-
 
 class PSD_TYPE(Enum):
-    """Power Spectral Density Type.
+    """Power Spectal Density Type.
 
     Enum used to specify the type of power spectral approximation
         to use. They each have trade-offs in terms of computational
         cost and resolution.
     """
     WELCH = 'Welch'
     MULTITAPER = 'MutliTaper'
@@ -25,16 +23,15 @@
 def power_spectral_density(
         data: np.ndarray,
         band: Tuple[float, float],
         sampling_rate: float = 100.0,
         window_length: float = 4.0,
         plot: bool = False,
         method: PSD_TYPE = PSD_TYPE.WELCH,
-        window: str = 'hann',
-        relative=False) -> float:
+        relative=False):
     """Power spectral density:
 
     Many thanks to: https://raphaelvallat.github.io/bandpower.html
 
     Parameters
     ----------
         data: Numpy Array.
@@ -51,46 +48,39 @@
             Whether of not to plot the PSD estimated. Helpful for debugging and exploration.
         method: PSD_TYPE
             Type of PSD estimation method to use during calculation.
         relative: boolean
             Whether or not to express the power in a frequency band as a percentage of the
             total power of the signal.
 
-    Returns
-    -------
-        bp: float
-            Power spectral density in the specified band
     """
     band = np.asarray(band)
     low, high = band
 
     # Compute the modified periodogram (Welch)
     if method == PSD_TYPE.WELCH:
         nperseg = window_length * sampling_rate
-        freqs, psd = welch(data, sampling_rate, nperseg=nperseg, window=window)
+        freqs, psd = welch(data, sampling_rate, nperseg=nperseg)
 
     # Compute the modified periodogram (MultiTaper)
     elif method == PSD_TYPE.MULTITAPER:
         psd, freqs = psd_array_multitaper(
             data, sampling_rate, adaptive=True, normalization='full', verbose=False)
 
-    else:
-        raise SignalException(f'Unknown PSD method: {method}')
-
     # Find index of band in frequency vector
     idx_band = np.logical_and(freqs >= low, freqs <= high)
 
     # Frequency resolution
     freq_res = freqs[1] - freqs[0]
 
     # Integral approximation of the spectrum using parabola (Simpson's rule)
     bp = simps(psd[idx_band], dx=freq_res)
 
     # Plot the power spectrum
-    if plot:  # pragma: no cover
+    if plot:
         sns.set(font_scale=1.2, style='white')
         plt.figure(figsize=(8, 4))
         plt.plot(freqs, psd, color='k', lw=2)
         plt.xlabel('Frequency (Hz)')
         plt.ylabel('Power spectral density (V^2 / Hz)')
         plt.ylim([0, psd.max() * 1.1])
         plt.title(f'{method.value}')
@@ -99,7 +89,20 @@
         plt.show()
 
     # Whether or not to return PSD as a percentage of total power
     if relative:
         bp /= simps(psd, dx=freq_res)
 
     return bp
+
+
+if __name__ == '__main__':
+    data = np.loadtxt('bcipy/signal/process/decomposition/resources/data.txt')
+    sampling_rate = 100
+    band = (0, 100)
+    np.arange(data.size) / sampling_rate
+    power_spectral_density(
+        data,
+        band,
+        sampling_rate=sampling_rate,
+        method=PSD_TYPE.WELCH,
+        plot=True)
```

### Comparing `bcipy-2.0.0rc3/bcipy/signal/process/filter.py` & `bcipy-2.0.1rc2/bcipy/signal/process/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Tuple
 
 import numpy as np
-from scipy.signal import butter, filtfilt, iirnotch, sosfiltfilt
+from scipy.signal import butter, filtfilt, iirnotch, sosfilt
 
 
 class Notch:
     """Remove a single frequency"""
 
     def __init__(self, sample_rate_hz, remove_freq_hz=60.0, quality_factor=30):
         remove_freq_hz = remove_freq_hz / (sample_rate_hz / 2)
@@ -20,15 +20,15 @@
 
     def __init__(self, lo, hi, sample_rate_hz, order=5):
         nyq = 0.5 * sample_rate_hz
         lo, hi = lo / nyq, hi / nyq
         self.sos = butter(order, [lo, hi], analog=False, btype="band", output="sos")
 
     def __call__(self, data: np.ndarray, fs: Optional[int] = None) -> Tuple[np.ndarray, int]:
-        return sosfiltfilt(self.sos, data), fs
+        return sosfilt(self.sos, data), fs
 
 
 def filter_inquiries(inquiries, transform, sample_rate) -> Tuple[np.ndarray, float]:
     """Filter Inquiries.
 
     The shape of data after reshaping into inquiries requires a bit of pre-processing to apply the
         transforms and filters defined in BciPy without looping. Here we flatten the inquires, filter,
```

### Comparing `bcipy-2.0.0rc3/bcipy/signal/process/transform.py` & `bcipy-2.0.1rc2/bcipy/signal/process/transform.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/task/control/criteria.py` & `bcipy-2.0.1rc2/bcipy/task/control/criteria.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/task/control/handler.py` & `bcipy-2.0.1rc2/bcipy/task/control/handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,273 +1,273 @@
-import logging
-import string
-from typing import Dict, List, Tuple, Optional
-
-import numpy as np
-
-from bcipy.helpers.stimuli import InquirySchedule, inq_generator, StimuliOrder
-from bcipy.helpers.symbols import SPACE_CHAR, BACKSPACE_CHAR
-from bcipy.task.control.query import RandomStimuliAgent, StimuliAgent
-from bcipy.task.control.criteria import CriteriaEvaluator
-
-log = logging.getLogger(__name__)
-
-
-class EvidenceFusion():
-    """ Fuses likelihood evidences provided by the inference
-        Attr:
-            evidence_history(dict{list[ndarray]}): Dictionary of difference
-                evidence types in list. Lists are ordered using the arrival
-                time.
-            likelihood(ndarray[]): current probability distribution over the
-                set. Gets updated once new evidence arrives. """
-
-    def __init__(self, list_name_evidence, len_dist):
-        self.evidence_history = {name: [] for name in list_name_evidence}
-        self.likelihood = np.ones(len_dist) / len_dist
-
-    def update_and_fuse(self, dict_evidence):
-        """ Updates the probability distribution
-            Args:
-                dict_evidence(dict{name: ndarray[float]}): dictionary of
-                    evidences (EEG and other likelihoods)
-        """
-
-        for key in dict_evidence.keys():
-            tmp = dict_evidence[key][:][:]
-            self.evidence_history[key].append(tmp)
-
-        # Current rule is to multiply
-        for value in dict_evidence.values():
-            self.likelihood *= value[:]
-
-        if np.isinf(np.sum(self.likelihood)):
-            tmp = np.zeros(len(self.likelihood))
-            tmp[np.where(self.likelihood == np.inf)[0][0]] = 1
-            self.likelihood = tmp
-
-        if not np.isnan(np.sum(self.likelihood)):
-            self.likelihood = self.likelihood / np.sum(self.likelihood)
-
-        likelihood = self.likelihood[:]
-
-        return likelihood
-
-    def reset_history(self):
-        """ Clears evidence history """
-        for value in self.evidence_history.values():
-            del value[:]
-        self.likelihood = np.ones(len(self.likelihood)) / len(self.likelihood)
-
-    def save_history(self) -> None:
-        """ Saves the current likelihood history """
-        log.warning('save_history not implemented')
-        return
-
-    @property
-    def latest_evidence(self) -> Dict[str, List[float]]:
-        """Latest evidence of each type in the evidence history.
-
-        Returns
-        -------
-        a dictionary with an entry for all configured evidence types.
-        """
-        return {
-            name: list(evidence[-1]) if evidence else []
-            for name, evidence in self.evidence_history.items()
-        }
-
-
-class DecisionMaker:
-    """ Scheduler of the entire framework
-        Attr:
-            state(str): state of the framework, which increases in size
-                by 1 after each inquiry. Elements are alphabet, ".,_,<"
-                where ".": null_inquiry(no decision made)
-                      "_": space bar
-                      "<": back space
-            alphabet(list[str]): list of symbols used by the framework. Can
-                be switched with location of images or one hot encoded images.
-            is_txt_stim(bool): whether the stimuli are text or images
-            inq_constants(list[str]): optional list of letters which should appear in
-                every inquiry.
-            stopping_evaluator: CriteriaEvaluator - optional parameter to
-                provide alternative rules for committing to a decision.
-            stimuli_agent(StimuliAgent): the query selection mechanism of the
-                system
-            stimuli_timing(list[float]): list of timings for the stimuli ([fixation_time, stimuli_flash_time])
-            stimuli_order(StimuliOrder): ordering of the stimuli (random, distributed)
-            stimuli_jitter(float): jitter of the inquiry stimuli in seconds
-
-        Functions:
-            decide():
-                Checks the criteria for making and series, using all
-                evidences and decides to do an series or to collect more
-                evidence
-            do_series():
-                Once committed an series perform updates to condition the
-                distribution on the previous letter.
-            schedule_inquiry():
-                schedule the next inquiry using the current information
-            decide_state_update():
-                If committed to an series update the state using a decision
-                metric.
-                (e.g. pick the letter with highest likelihood)
-            prepare_stimuli():
-                prepares the query set for the next inquiry
-                (e.g pick n-highest likely letters and randomly shuffle)
-        """
-
-    def __init__(self,
-                 state: str = '',
-                 alphabet: List[str] = list(string.ascii_uppercase) + [BACKSPACE_CHAR] + [SPACE_CHAR],
-                 is_txt_stim: bool = True,
-                 stimuli_timing: List[float] = [1, .2],
-                 stimuli_jitter: float = 0,
-                 stimuli_order: StimuliOrder = StimuliOrder.RANDOM,
-                 inq_constants: Optional[List[str]] = None,
-                 stopping_evaluator: CriteriaEvaluator = CriteriaEvaluator.default(min_num_inq=2,
-                                                                                   max_num_inq=10,
-                                                                                   threshold=0.8),
-                 stimuli_agent: Optional[StimuliAgent] = None):
-        self.state = state
-        self.displayed_state = self.form_display_state(state)
-        self.stimuli_timing = stimuli_timing
-        self.stimuli_order = stimuli_order
-        self.stimuli_jitter = stimuli_jitter
-
-        self.alphabet = alphabet
-        self.is_txt_stim = is_txt_stim
-
-        self.list_series = [{'target': None, 'time_spent': 0,
-                             'list_sti': [], 'list_distribution': [],
-                             'decision': None}]
-        self.time = 0
-        self.inquiry_counter = 0
-
-        self.stopping_evaluator = stopping_evaluator
-        self.stimuli_agent = stimuli_agent or RandomStimuliAgent(alphabet=self.alphabet)
-        self.last_selection = ''
-
-        # Items shown in every inquiry
-        self.inq_constants = inq_constants
-
-    def reset(self, state=''):
-        """ Resets the decision maker with the initial state
-            Args:
-                state(str): current state of the system """
-        self.state = state
-        self.displayed_state = self.form_display_state(self.state)
-
-        self.list_series = [{'target': None, 'time_spent': 0,
-                             'list_sti': [], 'list_distribution': []}]
-        self.time = 0
-        self.inquiry_counter = 0
-
-        self.stimuli_agent.reset()
-
-    def form_display_state(self, state):
-        """ Forms the state information or the user that fits to the
-            display. Basically takes '.' and BACKSPACE_CHAR into consideration and rewrites
-            the state
-            Args:
-                state(str): state string
-            Return:
-                displayed_state(str): state without '<,.' and removes
-                    backspaced letters """
-        tmp = ''
-        for i in state:
-            if i == BACKSPACE_CHAR:
-                tmp = tmp[0:-1]
-            elif i != '.':
-                tmp += i
-
-        return tmp
-
-    def update(self, state=''):
-        self.state = state
-        self.displayed_state = self.form_display_state(state)
-
-    def decide(self, p) -> Tuple[bool, InquirySchedule]:
-        """ Once evidence is collected, decision_maker makes a decision to
-            stop or not by leveraging the information of the stopping
-            criteria. Can decide to do an series or schedule another inquiry.
-
-        Args
-        ----
-        p(ndarray[float]): |A| x 1 distribution array
-            |A|: cardinality of the alphabet
-
-        Return
-        ------
-        - commitment: True if a letter is a commitment is made
-        False if requires more evidence
-        - inquiry schedule: Extra arguments depending on the decision
-        """
-
-        self.list_series[-1]['list_distribution'].append(p[:])
-
-        # Check stopping criteria
-        if self.stopping_evaluator.should_commit(self.list_series[-1]):
-            self.do_series()
-            return True, None
-        else:
-            stimuli = self.schedule_inquiry()
-            return False, stimuli
-
-    def do_series(self):
-        """ series refers to a commitment to a decision.
-            If made, state is updated, displayed state is updated
-            a new series is appended. """
-        self.inquiry_counter = 0
-        decision = self.decide_state_update()
-        self.last_selection = decision
-        self.state += decision
-        self.displayed_state = self.form_display_state(self.state)
-
-        # Initialize next series
-        self.list_series.append({'target': None, 'time_spent': 0,
-                                 'list_sti': [], 'list_distribution': []})
-
-        self.stimuli_agent.do_series()
-        self.stopping_evaluator.do_series()
-
-    def schedule_inquiry(self) -> InquirySchedule:
-        """ Schedules next inquiry """
-        self.state += '.'
-        stimuli = self.prepare_stimuli()
-        self.list_series[-1]['list_sti'].append(stimuli[0])
-        self.inquiry_counter += 1
-
-        return stimuli
-
-    def decide_state_update(self):
-        """ Checks stopping criteria to commit to an series """
-        idx = np.where(
-            self.list_series[-1]['list_distribution'][-1] ==
-            np.max(self.list_series[-1]['list_distribution'][-1]))[0][0]
-        decision = self.alphabet[idx]
-        self.list_series[-1]['decision'] = decision
-        return decision
-
-    def prepare_stimuli(self) -> InquirySchedule:
-        """ Given the alphabet, under a rule, prepares a stimuli for
-            the next inquiry.
-
-        Return
-        ------
-        stimuli(tuple[list[char],list[float],list[str]]): tuple of
-        stimuli information. [0]: letter, [1]: timing, [2]: color
-        """
-
-        # querying agent decides on possible letters to be shown on the screen
-        query_els = self.stimuli_agent.return_stimuli(
-            self.list_series[-1]['list_distribution'],
-            constants=self.inq_constants)
-        # once querying is determined, append with timing and color info.
-        stimuli = inq_generator(query=query_els,
-                                inquiry_count=1,
-                                is_txt=self.is_txt_stim,
-                                timing=self.stimuli_timing,
-                                stim_order=self.stimuli_order,
-                                stim_jitter=self.stimuli_jitter)
-        return stimuli
+import logging
+import string
+from typing import Dict, List, Tuple, Optional
+
+import numpy as np
+
+from bcipy.helpers.stimuli import InquirySchedule, inq_generator, StimuliOrder
+from bcipy.helpers.task import SPACE_CHAR, BACKSPACE_CHAR
+from bcipy.task.control.query import RandomStimuliAgent, StimuliAgent
+from bcipy.task.control.criteria import CriteriaEvaluator
+
+log = logging.getLogger(__name__)
+
+
+class EvidenceFusion():
+    """ Fuses likelihood evidences provided by the inference
+        Attr:
+            evidence_history(dict{list[ndarray]}): Dictionary of difference
+                evidence types in list. Lists are ordered using the arrival
+                time.
+            likelihood(ndarray[]): current probability distribution over the
+                set. Gets updated once new evidence arrives. """
+
+    def __init__(self, list_name_evidence, len_dist):
+        self.evidence_history = {name: [] for name in list_name_evidence}
+        self.likelihood = np.ones(len_dist) / len_dist
+
+    def update_and_fuse(self, dict_evidence):
+        """ Updates the probability distribution
+            Args:
+                dict_evidence(dict{name: ndarray[float]}): dictionary of
+                    evidences (EEG and other likelihoods)
+        """
+
+        for key in dict_evidence.keys():
+            tmp = dict_evidence[key][:][:]
+            self.evidence_history[key].append(tmp)
+
+        # Current rule is to multiply
+        for value in dict_evidence.values():
+            self.likelihood *= value[:]
+
+        if np.isinf(np.sum(self.likelihood)):
+            tmp = np.zeros(len(self.likelihood))
+            tmp[np.where(self.likelihood == np.inf)[0][0]] = 1
+            self.likelihood = tmp
+
+        if not np.isnan(np.sum(self.likelihood)):
+            self.likelihood = self.likelihood / np.sum(self.likelihood)
+
+        likelihood = self.likelihood[:]
+
+        return likelihood
+
+    def reset_history(self):
+        """ Clears evidence history """
+        for value in self.evidence_history.values():
+            del value[:]
+        self.likelihood = np.ones(len(self.likelihood)) / len(self.likelihood)
+
+    def save_history(self) -> None:
+        """ Saves the current likelihood history """
+        log.warning('save_history not implemented')
+        return
+
+    @property
+    def latest_evidence(self) -> Dict[str, List[float]]:
+        """Latest evidence of each type in the evidence history.
+
+        Returns
+        -------
+        a dictionary with an entry for all configured evidence types.
+        """
+        return {
+            name: list(evidence[-1]) if evidence else []
+            for name, evidence in self.evidence_history.items()
+        }
+
+
+class DecisionMaker:
+    """ Scheduler of the entire framework
+        Attr:
+            state(str): state of the framework, which increases in size
+                by 1 after each inquiry. Elements are alphabet, ".,_,<"
+                where ".": null_inquiry(no decision made)
+                      "_": space bar
+                      "<": back space
+            alphabet(list[str]): list of symbols used by the framework. Can
+                be switched with location of images or one hot encoded images.
+            is_txt_stim(bool): whether the stimuli are text or images
+            inq_constants(list[str]): optional list of letters which should appear in
+                every inquiry.
+            stopping_evaluator: CriteriaEvaluator - optional parameter to
+                provide alternative rules for committing to a decision.
+            stimuli_agent(StimuliAgent): the query selection mechanism of the
+                system
+            stimuli_timing(list[float]): list of timings for the stimuli ([fixation_time, stimuli_flash_time])
+            stimuli_order(StimuliOrder): ordering of the stimuli (random, distributed)
+            stimuli_jitter(float): jitter of the inquiry stimuli in seconds
+
+        Functions:
+            decide():
+                Checks the criteria for making and series, using all
+                evidences and decides to do an series or to collect more
+                evidence
+            do_series():
+                Once committed an series perform updates to condition the
+                distribution on the previous letter.
+            schedule_inquiry():
+                schedule the next inquiry using the current information
+            decide_state_update():
+                If committed to an series update the state using a decision
+                metric.
+                (e.g. pick the letter with highest likelihood)
+            prepare_stimuli():
+                prepares the query set for the next inquiry
+                (e.g pick n-highest likely letters and randomly shuffle)
+        """
+
+    def __init__(self,
+                 state: str = '',
+                 alphabet: List[str] = list(string.ascii_uppercase) + [BACKSPACE_CHAR] + [SPACE_CHAR],
+                 is_txt_stim: bool = True,
+                 stimuli_timing: List[float] = [1, .2],
+                 stimuli_jitter: float = 0,
+                 stimuli_order: StimuliOrder = StimuliOrder.RANDOM,
+                 inq_constants: Optional[List[str]] = None,
+                 stopping_evaluator: CriteriaEvaluator = CriteriaEvaluator.default(min_num_inq=2,
+                                                                                   max_num_inq=10,
+                                                                                   threshold=0.8),
+                 stimuli_agent: Optional[StimuliAgent] = None):
+        self.state = state
+        self.displayed_state = self.form_display_state(state)
+        self.stimuli_timing = stimuli_timing
+        self.stimuli_order = stimuli_order
+        self.stimuli_jitter = stimuli_jitter
+
+        self.alphabet = alphabet
+        self.is_txt_stim = is_txt_stim
+
+        self.list_series = [{'target': None, 'time_spent': 0,
+                             'list_sti': [], 'list_distribution': [],
+                             'decision': None}]
+        self.time = 0
+        self.inquiry_counter = 0
+
+        self.stopping_evaluator = stopping_evaluator
+        self.stimuli_agent = stimuli_agent or RandomStimuliAgent(alphabet=self.alphabet)
+        self.last_selection = ''
+
+        # Items shown in every inquiry
+        self.inq_constants = inq_constants
+
+    def reset(self, state=''):
+        """ Resets the decision maker with the initial state
+            Args:
+                state(str): current state of the system """
+        self.state = state
+        self.displayed_state = self.form_display_state(self.state)
+
+        self.list_series = [{'target': None, 'time_spent': 0,
+                             'list_sti': [], 'list_distribution': []}]
+        self.time = 0
+        self.inquiry_counter = 0
+
+        self.stimuli_agent.reset()
+
+    def form_display_state(self, state):
+        """ Forms the state information or the user that fits to the
+            display. Basically takes '.' and BACKSPACE_CHAR into consideration and rewrites
+            the state
+            Args:
+                state(str): state string
+            Return:
+                displayed_state(str): state without '<,.' and removes
+                    backspaced letters """
+        tmp = ''
+        for i in state:
+            if i == BACKSPACE_CHAR:
+                tmp = tmp[0:-1]
+            elif i != '.':
+                tmp += i
+
+        return tmp
+
+    def update(self, state=''):
+        self.state = state
+        self.displayed_state = self.form_display_state(state)
+
+    def decide(self, p) -> Tuple[bool, InquirySchedule]:
+        """ Once evidence is collected, decision_maker makes a decision to
+            stop or not by leveraging the information of the stopping
+            criteria. Can decide to do an series or schedule another inquiry.
+
+        Args
+        ----
+        p(ndarray[float]): |A| x 1 distribution array
+            |A|: cardinality of the alphabet
+
+        Return
+        ------
+        - commitment: True if a letter is a commitment is made
+        False if requires more evidence
+        - inquiry schedule: Extra arguments depending on the decision
+        """
+
+        self.list_series[-1]['list_distribution'].append(p[:])
+
+        # Check stopping criteria
+        if self.stopping_evaluator.should_commit(self.list_series[-1]):
+            self.do_series()
+            return True, None
+        else:
+            stimuli = self.schedule_inquiry()
+            return False, stimuli
+
+    def do_series(self):
+        """ series refers to a commitment to a decision.
+            If made, state is updated, displayed state is updated
+            a new series is appended. """
+        self.inquiry_counter = 0
+        decision = self.decide_state_update()
+        self.last_selection = decision
+        self.state += decision
+        self.displayed_state = self.form_display_state(self.state)
+
+        # Initialize next series
+        self.list_series.append({'target': None, 'time_spent': 0,
+                                 'list_sti': [], 'list_distribution': []})
+
+        self.stimuli_agent.do_series()
+        self.stopping_evaluator.do_series()
+
+    def schedule_inquiry(self) -> InquirySchedule:
+        """ Schedules next inquiry """
+        self.state += '.'
+        stimuli = self.prepare_stimuli()
+        self.list_series[-1]['list_sti'].append(stimuli[0])
+        self.inquiry_counter += 1
+
+        return stimuli
+
+    def decide_state_update(self):
+        """ Checks stopping criteria to commit to an series """
+        idx = np.where(
+            self.list_series[-1]['list_distribution'][-1] ==
+            np.max(self.list_series[-1]['list_distribution'][-1]))[0][0]
+        decision = self.alphabet[idx]
+        self.list_series[-1]['decision'] = decision
+        return decision
+
+    def prepare_stimuli(self) -> InquirySchedule:
+        """ Given the alphabet, under a rule, prepares a stimuli for
+            the next inquiry.
+
+        Return
+        ------
+        stimuli(tuple[list[char],list[float],list[str]]): tuple of
+        stimuli information. [0]: letter, [1]: timing, [2]: color
+        """
+
+        # querying agent decides on possible letters to be shown on the screen
+        query_els = self.stimuli_agent.return_stimuli(
+            self.list_series[-1]['list_distribution'],
+            constants=self.inq_constants)
+        # once querying is determined, append with timing and color info.
+        stimuli = inq_generator(query=query_els,
+                                inquiry_count=1,
+                                is_txt=self.is_txt_stim,
+                                timing=self.stimuli_timing,
+                                stim_order=self.stimuli_order,
+                                stim_jitter=self.stimuli_jitter)
+        return stimuli
```

### Comparing `bcipy-2.0.0rc3/bcipy/task/control/query.py` & `bcipy-2.0.1rc2/bcipy/task/control/query.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/task/data.py` & `bcipy-2.0.1rc2/bcipy/task/data.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/task/exceptions.py` & `bcipy-2.0.1rc2/bcipy/task/exceptions.py`

 * *Files identical despite different names*

### Comparing `bcipy-2.0.0rc3/bcipy/task/paradigm/matrix/calibration.py` & `bcipy-2.0.1rc2/bcipy/task/paradigm/matrix/calibration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 from typing import List, Tuple
 
 from psychopy import core
 
 from bcipy.config import TRIGGER_FILENAME, WAIT_SCREEN_MESSAGE
-from bcipy.display import Display, InformationProperties, StimuliProperties
-from bcipy.display.components.task_bar import CalibrationTaskBar
-from bcipy.display.paradigm.matrix.display import MatrixDisplay
+from bcipy.display import InformationProperties, StimuliProperties, TaskDisplayProperties
+from bcipy.display.paradigm.matrix.mode.calibration import CalibrationDisplay
 from bcipy.helpers.clock import Clock
-from bcipy.helpers.stimuli import (DEFAULT_TEXT_FIXATION, StimuliOrder,
-                                   TargetPositions,
-                                   calibration_inquiry_generator,
-                                   InquirySchedule)
-from bcipy.helpers.task import (get_user_input, pause_calibration,
+from bcipy.helpers.stimuli import (StimuliOrder, TargetPositions, calibration_inquiry_generator,
+                                   get_task_info)
+from bcipy.helpers.task import (alphabet, get_user_input, pause_calibration,
                                 trial_complete_message)
 from bcipy.helpers.triggers import TriggerHandler, TriggerType, Trigger, FlushFrequency, convert_timing_triggers
 from bcipy.task import Task
-from bcipy.helpers.symbols import alphabet
 
 
 class MatrixCalibrationTask(Task):
     """Matrix Calibration Task.
 
     Calibration task performs an Matrix stimulus inquiry
         to elicit an ERP. Parameters change the number of stimuli
@@ -44,83 +40,70 @@
         self.window = win
         self.frame_rate = self.window.getActualFrameRate()
         self.parameters = parameters
         self.daq = daq
         self.static_clock = core.StaticPeriod(screenHz=self.frame_rate)
         self.experiment_clock = Clock()
         self.buffer_val = parameters['task_buffer_length']
-        self.symbol_set = alphabet(parameters)
+        self.alp = alphabet(parameters)
+
+        self.matrix = init_calibration_display_task(
+            self.parameters, self.window,
+            self.static_clock, self.experiment_clock)
 
         self.file_save = file_save
         self.trigger_handler = TriggerHandler(
             self.file_save,
             TRIGGER_FILENAME,
             FlushFrequency.EVERY)
 
         self.wait_screen_message = WAIT_SCREEN_MESSAGE
         self.wait_screen_message_color = parameters['stim_color']
 
         self.stim_number = parameters['stim_number']
         self.stim_length = parameters['stim_length']
-        self.jitter = parameters['stim_jitter']
         self.stim_order = StimuliOrder(parameters['stim_order'])
         self.target_positions = TargetPositions(parameters['target_positions'])
         self.nontarget_inquiries = parameters['nontarget_inquiries']
 
-        self.timing = [
-            parameters['time_prompt'], parameters['time_fixation'],
-            parameters['time_flash']
-        ]
-        self.color = [
-            parameters['target_color'], parameters['fixation_color'],
-            parameters['stim_color']
-        ]
+        self.timing = [parameters['time_flash']]
+        self.color = [parameters['stim_color']]
         self.task_info_color = parameters['task_color']
         self.stimuli_height = parameters['stim_height']
         self.is_txt_stim = parameters['is_txt_stim']
         self.enable_breaks = parameters['enable_breaks']
 
-        self.matrix = self.init_display()
-
-    def init_display(self) -> Display:
-        """Initialize the display"""
-        return init_calibration_display_task(self.parameters, self.window,
-                                             self.experiment_clock,
-                                             self.symbol_set)
-
-    def generate_stimuli(self) -> InquirySchedule:
+    def generate_stimuli(self):
         """Generates the inquiries to be presented.
         Returns:
         --------
             tuple(
                 samples[list[list[str]]]: list of inquiries
                 timing(list[list[float]]): list of timings
                 color(list(list[str])): list of colors)
         """
-        return calibration_inquiry_generator(
-            self.symbol_set,
-            stim_number=self.stim_number,
-            stim_length=self.stim_length,
-            stim_order=self.stim_order,
-            jitter=self.jitter,
-            target_positions=self.target_positions,
-            nontarget_inquiries=self.nontarget_inquiries,
-            timing=self.timing,
-            color=self.color)
+        samples, timing, color = calibration_inquiry_generator(self.alp,
+                                                               stim_number=self.stim_number,
+                                                               stim_length=self.stim_length,
+                                                               stim_order=self.stim_order,
+                                                               target_positions=self.target_positions,
+                                                               nontarget_inquiries=self.nontarget_inquiries,
+                                                               timing=self.timing,
+                                                               color=self.color)
+
+        return (samples, timing, color)
 
     def trigger_type(self, symbol: str, target: str, index: int) -> TriggerType:
         """Trigger Type.
 
         This method is passed to convert_timing_triggers to properly assign TriggerTypes
             to the timing of stimuli presented.
         """
         if index == 0:
             return TriggerType.PROMPT
-        if symbol == DEFAULT_TEXT_FIXATION:
-            return TriggerType.FIXATION
         if target == symbol:
             return TriggerType.TARGET
         return TriggerType.NONTARGET
 
     def execute(self):
 
         self.logger.info(f'Starting {self.name()}!')
@@ -139,28 +122,33 @@
         while run:
 
             # Get inquiry information given stimuli parameters
             (stimuli_labels, stimuli_timing, stimuli_colors) = self.generate_stimuli()
 
             assert len(stimuli_labels) == len(stimuli_timing)
 
-            for inquiry in range(self.stim_number):
+            (task_text, task_color) = get_task_info(self.stim_number,
+                                                    self.task_info_color)
+
+            for inquiry in range(len(task_text)):
 
                 # check user input to make sure we should be going
                 if not get_user_input(self.matrix, self.wait_screen_message,
                                       self.wait_screen_message_color):
                     break
 
                 # Take a break every number of trials defined
                 if self.enable_breaks:
                     pause_calibration(self.window, self.matrix, inquiry,
                                       self.parameters)
 
                 # update task state
-                self.matrix.update_task_bar(str(inquiry + 1))
+                self.matrix.update_task_state(
+                    text=task_text[inquiry],
+                    color_list=task_color[inquiry])
 
                 # Draw and flip screen
                 self.matrix.draw_static()
                 self.window.flip()
 
                 self.matrix.schedule_to(
                     stimuli_labels[inquiry],
@@ -168,15 +156,15 @@
                     stimuli_colors[inquiry])
                 # Schedule a inquiry
 
                 # Wait for a time
                 core.wait(self.buffer_val)
 
                 # Do the inquiry
-                timing = self.matrix.do_inquiry()
+                timing, target = self.matrix.do_inquiry()
 
                 # Write triggers for the inquiry
                 self.write_trigger_data(timing, (inquiry == 0))
 
                 # Wait for a time
                 core.wait(self.buffer_val)
 
@@ -236,15 +224,15 @@
         self.trigger_handler.close()
 
     def name(self):
         return 'Matrix Calibration Task'
 
 
 def init_calibration_display_task(
-        parameters, window, experiment_clock, symbol_set):
+        parameters, window, static_clock, experiment_clock):
     info = InformationProperties(
         info_color=[parameters['info_color']],
         info_pos=[(parameters['info_pos_x'],
                    parameters['info_pos_y'])],
         info_height=[parameters['info_height']],
         info_font=[parameters['font']],
         info_text=[parameters['info_text']],
@@ -254,22 +242,24 @@
                                 stim_height=0.1,
                                 stim_inquiry=[''] * parameters['stim_length'],
                                 stim_colors=[parameters['stim_color']] * parameters['stim_length'],
                                 stim_timing=[10] * parameters['stim_length'],
                                 is_txt_stim=parameters['is_txt_stim'],
                                 prompt_time=parameters["time_prompt"])
 
-    task_bar = CalibrationTaskBar(window,
-                                  inquiry_count=parameters['stim_number'],
-                                  current_index=0,
-                                  colors=[parameters['task_color']],
-                                  font=parameters['font'],
-                                  height=parameters['task_height'])
-
-    return MatrixDisplay(
+    task_display = TaskDisplayProperties(
+        task_color=[parameters['task_color']],
+        task_pos=(-.8, .85),
+        task_font=parameters['font'],
+        task_height=parameters['task_height'],
+        task_text=''
+    )
+    return CalibrationDisplay(
         window,
+        static_clock,
         experiment_clock,
         stimuli,
-        task_bar,
+        task_display,
         info,
         trigger_type=parameters['trigger_type'],
-        symbol_set=symbol_set)
+        space_char=parameters['stim_space_char'],
+        full_screen=parameters['full_screen'])
```

### Comparing `bcipy-2.0.0rc3/bcipy/task/paradigm/matrix/timing_verification.py` & `bcipy-2.0.1rc2/bcipy/task/paradigm/rsvp/calibration/timing_verification.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from itertools import cycle
-from typing import List
-from bcipy.task.paradigm.matrix.calibration import (
-    MatrixCalibrationTask, InquirySchedule, DEFAULT_TEXT_FIXATION, Display,
-    init_calibration_display_task)
-from bcipy.helpers.stimuli import PhotoDiodeStimuli, jittered_timing
-
-
-class MatrixTimingVerificationCalibration(MatrixCalibrationTask):
-    """Matrix Timing Verification Task.
-
-    This task is used for verifying display timing by alternating solid and empty boxes. These
-        stimuli can be used with a photodiode to ensure accurate presentations.
-
-    Input:
-        win (PsychoPy Display Object)
-        daq (Data Acquisition Object)
-        parameters (Dictionary)
-        file_save (String)
-
-    Output:
-        file_save (String)
-    """
-    TASK_NAME = 'Matrix Timing Verification Task'
-
-    def init_display(self) -> Display:
-        """Initialize the display"""
-        display = init_calibration_display_task(
-            self.parameters, self.window, self.experiment_clock,
-            symbols_with_photodiode_stim(self.symbol_set))
-        display.start_opacity = 0.0
-        return display
-
-    def generate_stimuli(self) -> InquirySchedule:
-        """Generates the inquiries to be presented.
-        """
-        samples, times, colors = [], [], []
-        [time_target, time_fixation, time_stim] = self.timing
-        stimuli = cycle(PhotoDiodeStimuli.list())
-        stim_timing = jittered_timing(time_stim, self.jitter, self.stim_length)
-
-        # advance iterator to start on the solid stim.
-        next(stimuli)
-
-        # alternate between solid and empty boxes
-        inq_stim = [PhotoDiodeStimuli.SOLID.value, DEFAULT_TEXT_FIXATION
-                    ] + [next(stimuli) for _ in range(self.stim_length)]
-        inq_times = [time_target, time_fixation
-                     ] + stim_timing
-        inq_colors = [self.color[0]] * (self.stim_length + 2)
-
-        for _ in range(self.stim_number):
-            samples.append(inq_stim)
-            times.append(inq_times)
-            colors.append(inq_colors)
-
-        return InquirySchedule(samples, times, colors)
-
-
-def symbols_with_photodiode_stim(symbols: List[str]) -> List[str]:
-    """Stim symbols with the central letters swapped out for Photodiode stim.
-    """
-    mid = int(len(symbols) / 2)
-
-    def sym_at_index(sym, index) -> str:
-        if index == mid:
-            return PhotoDiodeStimuli.SOLID.value
-        if index == mid + 1:
-            return PhotoDiodeStimuli.EMPTY.value
-        return sym
-
-    return [sym_at_index(sym, i) for i, sym in enumerate(symbols)]
+from itertools import cycle
+from bcipy.task import Task
+from bcipy.task.paradigm.rsvp.calibration.calibration import RSVPCalibrationTask
+from bcipy.helpers.stimuli import PhotoDiodeStimuli, get_fixation
+
+
+class RSVPTimingVerificationCalibration(Task):
+    """RSVP Calibration Task.
+
+    This task is used for verifying display timing by alternating solid and empty boxes. These
+        stimuli can be used with a photodiode to ensure accurate presentations.
+
+    Input:
+        win (PsychoPy Display Object)
+        daq (Data Acquisition Object)
+        parameters (Dictionary)
+        file_save (String)
+
+    Output:
+        file_save (String)
+    """
+    TASK_NAME = 'RSVP Timing Verification Task'
+
+    def __init__(self, win, daq, parameters, file_save):
+        super(RSVPTimingVerificationCalibration, self).__init__()
+        parameters['stim_height'] = 0.8
+        parameters['stim_pos_y'] = 0.0
+        self.stimuli = PhotoDiodeStimuli.list()
+        self._task = RSVPCalibrationTask(win, daq, parameters, file_save)
+        self._task.generate_stimuli = self.generate_stimuli
+
+    def generate_stimuli(self):
+        """Generates the inquiries to be presented.
+        Returns:
+        --------
+            tuple(
+                samples[list[list[str]]]: list of inquiries
+                timing(list[list[float]]): list of timings
+                color(list(list[str])): list of colors)
+        """
+        samples, times, colors = [], [], []
+
+        # alternate between solid and empty boxes
+        letters = cycle(self.stimuli)
+        time_prompt, time_fixation, time_stim = self._task.timing
+        color_target, color_fixation, color_stim = self._task.color
+
+        target = next(letters)
+        fixation = get_fixation(is_txt=True)
+
+        inq_len = self._task.stim_length
+        inq_stim = [target, fixation, *[next(letters) for _ in range(inq_len)]]
+        inq_times = [time_prompt, time_fixation, *[time_stim for _ in range(inq_len)]]
+        inq_colors = [color_target, color_fixation, *[color_stim for _ in range(inq_len)]]
+
+        for _ in range(self._task.stim_number):
+            samples.append(inq_stim)
+            times.append(inq_times)
+            colors.append(inq_colors)
+
+        return (samples, times, colors)
+
+    def execute(self):
+        self.logger.debug(f'Starting {self.name()}!')
+        self._task.execute()
+
+    @classmethod
+    def label(cls):
+        return RSVPTimingVerificationCalibration.TASK_NAME
+
+    def name(self):
+        return RSVPTimingVerificationCalibration.TASK_NAME
```

### Comparing `bcipy-2.0.0rc3/bcipy/task/paradigm/rsvp/calibration/calibration.py` & `bcipy-2.0.1rc2/bcipy/task/paradigm/rsvp/calibration/calibration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,276 +1,265 @@
-from psychopy import core
-from typing import List, Tuple
-
-from bcipy.config import TRIGGER_FILENAME, WAIT_SCREEN_MESSAGE
-from bcipy.display import (
-    InformationProperties,
-    PreviewInquiryProperties,
-    StimuliProperties)
-from bcipy.display.paradigm.rsvp.mode.calibration import CalibrationDisplay
-from bcipy.display.components.task_bar import CalibrationTaskBar
-from bcipy.helpers.clock import Clock
-
-from bcipy.helpers.stimuli import (StimuliOrder, TargetPositions, calibration_inquiry_generator)
-from bcipy.helpers.task import (get_user_input, pause_calibration,
-                                trial_complete_message)
-from bcipy.helpers.symbols import alphabet
-from bcipy.helpers.triggers import FlushFrequency, TriggerHandler, Trigger, TriggerType, convert_timing_triggers
-from bcipy.task import Task
-
-
-class RSVPCalibrationTask(Task):
-    """RSVP Calibration Task.
-
-    Calibration task performs an RSVP stimulus inquiry
-        to elicit an ERP. Parameters will change how many stimuli
-        and for how long they present. Parameters also change
-        color and text / image inputs.
-
-    This task progresses as follows:
-
-    setting up variables --> initializing eeg --> awaiting user input to start --> setting up stimuli -->
-    presenting inquiries --> saving data
-
-    PARAMETERS:
-    ----------
-    win (PsychoPy Display)
-    daq (Data Acquisition Client)
-    parameters (dict)
-    file_save (str)
-    """
-
-    def __init__(self, win, daq, parameters, file_save):
-        super(RSVPCalibrationTask, self).__init__()
-
-        self.window = win
-        self.frame_rate = self.window.getActualFrameRate()
-        self.parameters = parameters
-        self.daq = daq
-        self.static_clock = core.StaticPeriod(screenHz=self.frame_rate)
-        self.experiment_clock = Clock()
-        self.buffer_val = parameters['task_buffer_length']
-        self.alp = alphabet(parameters)
-        self.rsvp = init_calibration_display_task(
-            self.parameters, self.window,
-            self.static_clock, self.experiment_clock)
-        self.file_save = file_save
-        self.trigger_handler = TriggerHandler(
-            self.file_save,
-            TRIGGER_FILENAME,
-            FlushFrequency.EVERY)
-
-        self.stim_number = parameters['stim_number']
-        self.stim_length = parameters['stim_length']
-        self.stim_order = StimuliOrder(parameters['stim_order'])
-        self.target_positions = TargetPositions(parameters['target_positions'])
-        self.nontarget_inquiries = parameters['nontarget_inquiries']
-
-        self.show_preview_inquiry = parameters['show_preview_inquiry']
-
-        self.timing = [parameters['time_prompt'],
-                       parameters['time_fixation'],
-                       parameters['time_flash']]
-        self.jitter = parameters['stim_jitter']
-
-        self.color = [parameters['target_color'],
-                      parameters['fixation_color'],
-                      parameters['stim_color']]
-        self.wait_screen_message_color = self.color[-1]
-        self.task_info_color = parameters['task_color']
-
-        self.stimuli_height = parameters['stim_height']
-        self.is_txt_stim = parameters['is_txt_stim']
-        self.enable_breaks = parameters['enable_breaks']
-
-    def generate_stimuli(self):
-        """Generates the inquiries to be presented.
-        Returns:
-        --------
-            tuple(
-                samples[list[list[str]]]: list of inquiries
-                timing(list[list[float]]): list of timings
-                color(list(list[str])): list of colors)
-        """
-        return calibration_inquiry_generator(self.alp,
-                                             stim_number=self.stim_number,
-                                             stim_length=self.stim_length,
-                                             stim_order=self.stim_order,
-                                             target_positions=self.target_positions,
-                                             nontarget_inquiries=self.nontarget_inquiries,
-                                             timing=self.timing,
-                                             jitter=self.jitter,
-                                             is_txt=self.rsvp.is_txt_stim,
-                                             color=self.color)
-
-    def trigger_type(self, symbol: str, target: str, index: int) -> TriggerType:
-        """Trigger Type.
-
-        This method is passed to convert_timing_triggers to properly assign TriggerTypes
-            to the timing of stimuli presented.
-        """
-        if index == 0:
-            return TriggerType.PROMPT
-        if symbol == 'inquiry_preview' and index == 1:
-            return TriggerType.PREVIEW
-        if symbol == '+':
-            return TriggerType.FIXATION
-        if target == symbol:
-            return TriggerType.TARGET
-        return TriggerType.NONTARGET
-
-    def execute(self):
-
-        self.logger.debug(f'Starting {self.name()}!')
-        run = True
-
-        # Check user input to make sure we should be going
-        if not get_user_input(self.rsvp, WAIT_SCREEN_MESSAGE,
-                              self.wait_screen_message_color,
-                              first_run=True):
-            run = False
-
-        # Begin the Experiment
-        while run:
-
-            # Get inquiry information given stimuli parameters
-            (stimuli, stimuli_timing, stimuli_color) = self.generate_stimuli()
-
-            # Execute the RSVP inquiries
-            for inquiry in range(self.stim_number):
-
-                # check user input to make sure we should be going
-                if not get_user_input(self.rsvp, WAIT_SCREEN_MESSAGE,
-                                      self.wait_screen_message_color):
-                    break
-
-                # Take a break every number of trials defined
-                if self.enable_breaks:
-                    pause_calibration(self.window, self.rsvp, inquiry,
-                                      self.parameters)
-
-                # update task state
-                self.rsvp.update_task_bar()
-
-                # Draw and flip screen
-                self.rsvp.draw_static()
-                self.window.flip()
-
-                # Schedule a inquiry
-                self.rsvp.stimuli_inquiry = stimuli[inquiry]
-
-                # check if text stimuli or not for color information
-                if self.is_txt_stim:
-                    self.rsvp.stimuli_colors = stimuli_color[inquiry]
-
-                self.rsvp.stimuli_timing = stimuli_timing[inquiry]
-
-                core.wait(self.buffer_val)
-
-                # do inquiry and get timing information back from the display
-                timing = self.rsvp.do_inquiry(preview_calibration=self.show_preview_inquiry)
-
-                self.write_trigger_data(timing, (inquiry == 0))
-                core.wait(self.buffer_val)
-
-            # Set run to False to stop looping
-            run = False
-
-        # Say Goodbye!
-        self.rsvp.info_text = trial_complete_message(self.window, self.parameters)
-        self.rsvp.draw_static()
-        self.window.flip()
-
-        self.write_offset_trigger()
-
-        # Wait some time before exiting so there is trailing eeg data saved
-        core.wait(self.buffer_val)
-
-        return self.file_save
-
-    def write_trigger_data(self, timing: List[Tuple[str, float]], first_run) -> None:
-        """Write Trigger Data.
-
-        Using the timing provided from the display and calibration information from the data acquisition
-        client, write trigger data in the correct format.
-
-        *Note on offsets*: we write the full offset value which can be used to transform all stimuli to the time since
-            session start (t = 0) for all values (as opposed to most system clocks which start much higher).
-            We do not write the calibration trigger used to generate this offset from the display.
-            See RSVPDisplay._trigger_pulse() for more information.
-        """
-        # write offsets. currently, we only check for offsets at the beginning.
-        if self.daq.is_calibrated and first_run:
-            self.trigger_handler.add_triggers(
-                [Trigger(
-                    'starting_offset',
-                    TriggerType.OFFSET,
-                    # offset will factor in true offset and time relative from beginning
-                    (self.daq.offset(self.rsvp.first_stim_time) - self.rsvp.first_stim_time)
-                )]
-            )
-
-        # make sure triggers are written for the inquiry
-        self.trigger_handler.add_triggers(convert_timing_triggers(timing, timing[0][0], self.trigger_type))
-
-    def write_offset_trigger(self) -> None:
-        """Append an offset value to the end of the trigger file.
-        """
-        if self.daq.is_calibrated:
-            self.trigger_handler.add_triggers(
-                [Trigger(
-                    'daq_sample_offset',
-                    TriggerType.SYSTEM,
-                    # to help support future refactoring or use of lsl timestamps only
-                    # we write only the sample offset here
-                    self.daq.offset(self.rsvp.first_stim_time)
-                )])
-        self.trigger_handler.close()
-
-    def name(self):
-        return 'RSVP Calibration Task'
-
-
-def init_calibration_display_task(
-        parameters, window, static_clock, experiment_clock):
-    info = InformationProperties(
-        info_color=[parameters['info_color']],
-        info_pos=[(parameters['info_pos_x'],
-                   parameters['info_pos_y'])],
-        info_height=[parameters['info_height']],
-        info_font=[parameters['font']],
-        info_text=[parameters['info_text']],
-    )
-    stimuli = StimuliProperties(stim_font=parameters['font'],
-                                stim_pos=(parameters['stim_pos_x'],
-                                          parameters['stim_pos_y']),
-                                stim_height=parameters['stim_height'],
-                                stim_inquiry=[''] * parameters['stim_length'],
-                                stim_colors=[parameters['stim_color']] * parameters['stim_length'],
-                                stim_timing=[10] * parameters['stim_length'],
-                                is_txt_stim=parameters['is_txt_stim'])
-
-    task_bar = CalibrationTaskBar(window,
-                                  inquiry_count=parameters['stim_number'],
-                                  current_index=0,
-                                  colors=[parameters['task_color']],
-                                  font=parameters['font'],
-                                  height=parameters['task_height'])
-
-    preview_inquiry = PreviewInquiryProperties(
-        preview_only=True,
-        preview_inquiry_length=parameters['preview_inquiry_length'],
-        preview_inquiry_progress_method=parameters['preview_inquiry_progress_method'],
-        preview_inquiry_key_input=parameters['preview_inquiry_key_input'],
-        preview_inquiry_isi=parameters['preview_inquiry_isi'])
-
-    return CalibrationDisplay(
-        window,
-        static_clock,
-        experiment_clock,
-        stimuli,
-        task_bar,
-        info,
-        preview_inquiry=preview_inquiry,
-        trigger_type=parameters['trigger_type'],
-        space_char=parameters['stim_space_char'],
-        full_screen=parameters['full_screen'])
+from psychopy import core
+from typing import List, Tuple
+
+from bcipy.config import TRIGGER_FILENAME, WAIT_SCREEN_MESSAGE
+from bcipy.display import InformationProperties, StimuliProperties, TaskDisplayProperties
+from bcipy.display.paradigm.rsvp.mode.calibration import CalibrationDisplay
+from bcipy.helpers.clock import Clock
+from bcipy.helpers.stimuli import (StimuliOrder, TargetPositions, calibration_inquiry_generator,
+                                   get_task_info)
+from bcipy.helpers.task import (alphabet, get_user_input, pause_calibration,
+                                trial_complete_message)
+from bcipy.helpers.triggers import FlushFrequency, TriggerHandler, Trigger, TriggerType, convert_timing_triggers
+from bcipy.task import Task
+
+
+class RSVPCalibrationTask(Task):
+    """RSVP Calibration Task.
+
+    Calibration task performs an RSVP stimulus inquiry
+        to elicit an ERP. Parameters will change how many stimuli
+        and for how long they present. Parameters also change
+        color and text / image inputs.
+
+    This task progresses as follows:
+
+    setting up variables --> initializing eeg --> awaiting user input to start --> setting up stimuli -->
+    presenting inquiries --> saving data
+
+    PARAMETERS:
+    ----------
+    win (PsychoPy Display)
+    daq (Data Acquisition Client)
+    parameters (dict)
+    file_save (str)
+    """
+
+    def __init__(self, win, daq, parameters, file_save):
+        super(RSVPCalibrationTask, self).__init__()
+
+        self.window = win
+        self.frame_rate = self.window.getActualFrameRate()
+        self.parameters = parameters
+        self.daq = daq
+        self.static_clock = core.StaticPeriod(screenHz=self.frame_rate)
+        self.experiment_clock = Clock()
+        self.buffer_val = parameters['task_buffer_length']
+        self.alp = alphabet(parameters)
+        self.rsvp = init_calibration_display_task(
+            self.parameters, self.window,
+            self.static_clock, self.experiment_clock)
+        self.file_save = file_save
+        self.trigger_handler = TriggerHandler(
+            self.file_save,
+            TRIGGER_FILENAME,
+            FlushFrequency.EVERY)
+
+        self.stim_number = parameters['stim_number']
+        self.stim_length = parameters['stim_length']
+        self.stim_order = StimuliOrder(parameters['stim_order'])
+        self.target_positions = TargetPositions(parameters['target_positions'])
+        self.nontarget_inquiries = parameters['nontarget_inquiries']
+
+        self.timing = [parameters['time_prompt'],
+                       parameters['time_fixation'],
+                       parameters['time_flash']]
+        self.jitter = parameters['stim_jitter']
+
+        self.color = [parameters['target_color'],
+                      parameters['fixation_color'],
+                      parameters['stim_color']]
+        self.wait_screen_message_color = self.color[-1]
+
+        self.task_info_color = parameters['task_color']
+
+        self.stimuli_height = parameters['stim_height']
+
+        self.is_txt_stim = parameters['is_txt_stim']
+
+        self.enable_breaks = parameters['enable_breaks']
+
+    def generate_stimuli(self):
+        """Generates the inquiries to be presented.
+        Returns:
+        --------
+            tuple(
+                samples[list[list[str]]]: list of inquiries
+                timing(list[list[float]]): list of timings
+                color(list(list[str])): list of colors)
+        """
+        return calibration_inquiry_generator(self.alp,
+                                             stim_number=self.stim_number,
+                                             stim_length=self.stim_length,
+                                             stim_order=self.stim_order,
+                                             target_positions=self.target_positions,
+                                             nontarget_inquiries=self.nontarget_inquiries,
+                                             timing=self.timing,
+                                             jitter=self.jitter,
+                                             is_txt=self.rsvp.is_txt_stim,
+                                             color=self.color)
+
+    def trigger_type(self, symbol: str, target: str, index: int) -> TriggerType:
+        """Trigger Type.
+
+        This method is passed to convert_timing_triggers to properly assign TriggerTypes
+            to the timing of stimuli presented.
+        """
+        if index == 0:
+            return TriggerType.PROMPT
+        if symbol == '+':
+            return TriggerType.FIXATION
+        if target == symbol:
+            return TriggerType.TARGET
+        return TriggerType.NONTARGET
+
+    def execute(self):
+
+        self.logger.debug(f'Starting {self.name()}!')
+        run = True
+
+        # Check user input to make sure we should be going
+        if not get_user_input(self.rsvp, WAIT_SCREEN_MESSAGE,
+                              self.wait_screen_message_color,
+                              first_run=True):
+            run = False
+
+        # Begin the Experiment
+        while run:
+
+            # Get inquiry information given stimuli parameters
+            (stimuli, stimuli_timing, stimuli_color) = self.generate_stimuli()
+
+            (task_text, task_color) = get_task_info(self.stim_number,
+                                                    self.task_info_color)
+
+            # Execute the RSVP inquiries
+            for inquiry in range(len(task_text)):
+
+                # check user input to make sure we should be going
+                if not get_user_input(self.rsvp, WAIT_SCREEN_MESSAGE,
+                                      self.wait_screen_message_color):
+                    break
+
+                # Take a break every number of trials defined
+                if self.enable_breaks:
+                    pause_calibration(self.window, self.rsvp, inquiry,
+                                      self.parameters)
+
+                # update task state
+                self.rsvp.update_task_state(
+                    text=task_text[inquiry],
+                    color_list=task_color[inquiry])
+
+                # Draw and flip screen
+                self.rsvp.draw_static()
+                self.window.flip()
+
+                # Schedule a inquiry
+                self.rsvp.stimuli_inquiry = stimuli[inquiry]
+
+                # check if text stimuli or not for color information
+                if self.is_txt_stim:
+                    self.rsvp.stimuli_colors = stimuli_color[inquiry]
+
+                self.rsvp.stimuli_timing = stimuli_timing[inquiry]
+
+                core.wait(self.buffer_val)
+
+                # Do the inquiry and write necessary data
+                timing = self.rsvp.do_inquiry()
+                self.write_trigger_data(timing, (inquiry == 0))
+                core.wait(self.buffer_val)
+
+            # Set run to False to stop looping
+            run = False
+
+        # Say Goodbye!
+        self.rsvp.info_text = trial_complete_message(self.window, self.parameters)
+        self.rsvp.draw_static()
+        self.window.flip()
+
+        self.write_offset_trigger()
+
+        # Wait some time before exiting so there is trailing eeg data saved
+        core.wait(self.buffer_val)
+
+        return self.file_save
+
+    def write_trigger_data(self, timing: List[Tuple[str, float]], first_run) -> None:
+        """Write Trigger Data.
+
+        Using the timing provided from the display and calibration information from the data acquisition
+        client, write trigger data in the correct format.
+
+        *Note on offsets*: we write the full offset value which can be used to transform all stimuli to the time since
+            session start (t = 0) for all values (as opposed to most system clocks which start much higher).
+            We do not write the calibration trigger used to generate this offset from the display.
+            See RSVPDisplay._trigger_pulse() for more information.
+        """
+        # write offsets. currently, we only check for offsets at the beginning.
+        if self.daq.is_calibrated and first_run:
+            self.trigger_handler.add_triggers(
+                [Trigger(
+                    'starting_offset',
+                    TriggerType.OFFSET,
+                    # offset will factor in true offset and time relative from beginning
+                    (self.daq.offset(self.rsvp.first_stim_time) - self.rsvp.first_stim_time)
+                )]
+            )
+
+        # make sure triggers are written for the inquiry
+        self.trigger_handler.add_triggers(convert_timing_triggers(timing, timing[0][0], self.trigger_type))
+
+    def write_offset_trigger(self) -> None:
+        """Append an offset value to the end of the trigger file.
+        """
+        if self.daq.is_calibrated:
+            self.trigger_handler.add_triggers(
+                [Trigger(
+                    'daq_sample_offset',
+                    TriggerType.SYSTEM,
+                    # to help support future refactoring or use of lsl timestamps only
+                    # we write only the sample offset here
+                    self.daq.offset(self.rsvp.first_stim_time)
+                )])
+        self.trigger_handler.close()
+
+    def name(self):
+        return 'RSVP Calibration Task'
+
+
+def init_calibration_display_task(
+        parameters, window, static_clock, experiment_clock):
+    info = InformationProperties(
+        info_color=[parameters['info_color']],
+        info_pos=[(parameters['info_pos_x'],
+                   parameters['info_pos_y'])],
+        info_height=[parameters['info_height']],
+        info_font=[parameters['font']],
+        info_text=[parameters['info_text']],
+    )
+    stimuli = StimuliProperties(stim_font=parameters['font'],
+                                stim_pos=(parameters['stim_pos_x'],
+                                          parameters['stim_pos_y']),
+                                stim_height=parameters['stim_height'],
+                                stim_inquiry=[''] * parameters['stim_length'],
+                                stim_colors=[parameters['stim_color']] * parameters['stim_length'],
+                                stim_timing=[10] * parameters['stim_length'],
+                                is_txt_stim=parameters['is_txt_stim'])
+    task_display = TaskDisplayProperties(
+        task_color=[parameters['task_color']],
+        task_pos=(-.8, .85),
+        task_font=parameters['font'],
+        task_height=parameters['task_height'],
+        task_text=''
+    )
+    return CalibrationDisplay(
+        window,
+        static_clock,
+        experiment_clock,
+        stimuli,
+        task_display,
+        info,
+        trigger_type=parameters['trigger_type'],
+        space_char=parameters['stim_space_char'],
+        full_screen=parameters['full_screen'])
```

### Comparing `bcipy-2.0.0rc3/bcipy/task/paradigm/rsvp/calibration/timing_verification.py` & `bcipy-2.0.1rc2/bcipy/task/paradigm/matrix/timing_verification.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,82 @@
-from itertools import cycle
-from bcipy.task import Task
-from bcipy.task.paradigm.rsvp.calibration.calibration import RSVPCalibrationTask
-from bcipy.helpers.stimuli import PhotoDiodeStimuli, get_fixation, jittered_timing
-
-
-class RSVPTimingVerificationCalibration(Task):
-    """RSVP Calibration Task.
-
-    This task is used for verifying display timing by alternating solid and empty boxes. These
-        stimuli can be used with a photodiode to ensure accurate presentations.
-
-    Input:
-        win (PsychoPy Display Object)
-        daq (Data Acquisition Object)
-        parameters (Dictionary)
-        file_save (String)
-
-    Output:
-        file_save (String)
-    """
-    TASK_NAME = 'RSVP Timing Verification Task'
-
-    def __init__(self, win, daq, parameters, file_save):
-        super(RSVPTimingVerificationCalibration, self).__init__()
-        parameters['stim_height'] = 0.8
-        parameters['stim_pos_y'] = 0.0
-        self.stimuli = PhotoDiodeStimuli.list()
-        self._task = RSVPCalibrationTask(win, daq, parameters, file_save)
-        self._task.generate_stimuli = self.generate_stimuli
-
-    def generate_stimuli(self):
-        """Generates the inquiries to be presented.
-        Returns:
-        --------
-            tuple(
-                samples[list[list[str]]]: list of inquiries
-                timing(list[list[float]]): list of timings
-                color(list(list[str])): list of colors)
-        """
-        samples, times, colors = [], [], []
-
-        # alternate between solid and empty boxes
-        letters = cycle(self.stimuli)
-        time_prompt, time_fixation, time_stim = self._task.timing
-        color_target, color_fixation, color_stim = self._task.color
-        inq_len = self._task.stim_length
-
-        stim_timing = jittered_timing(time_stim, self._task.jitter, inq_len)
-        target = next(letters)
-        fixation = get_fixation(is_txt=True)
-
-        inq_stim = [target, fixation, *[next(letters) for _ in range(inq_len)]]
-        inq_times = [time_prompt, time_fixation] + stim_timing
-        inq_colors = [color_target, color_fixation, *[color_stim for _ in range(inq_len)]]
-
-        for _ in range(self._task.stim_number):
-            samples.append(inq_stim)
-            times.append(inq_times)
-            colors.append(inq_colors)
-
-        return (samples, times, colors)
-
-    def execute(self):
-        self.logger.debug(f'Starting {self.name()}!')
-        self._task.execute()
-
-    @classmethod
-    def label(cls):
-        return RSVPTimingVerificationCalibration.TASK_NAME
-
-    def name(self):
-        return RSVPTimingVerificationCalibration.TASK_NAME
+from itertools import cycle
+from bcipy.task import Task
+from bcipy.task.paradigm.matrix.calibration import MatrixCalibrationTask
+from bcipy.helpers.stimuli import PhotoDiodeStimuli
+
+
+class MatrixTimingVerificationCalibration(Task):
+    """Matrix Calibration Task.
+
+    This task is used for verifying display timing by alternating solid and empty boxes. These
+        stimuli can be used with a photodiode to ensure accurate presentations.
+
+    Input:
+        win (PsychoPy Display Object)
+        daq (Data Acquisition Object)
+        parameters (Dictionary)
+        file_save (String)
+
+    Output:
+        file_save (String)
+    """
+    TASK_NAME = 'Matrix Timing Verification Task'
+
+    def __init__(self, win, daq, parameters, file_save):
+        super(MatrixTimingVerificationCalibration, self).__init__()
+        self._task = MatrixCalibrationTask(win, daq, parameters, file_save)
+        self.stimuli = PhotoDiodeStimuli.list()
+        self.create_testing_grid()
+        self._task.matrix.start_opacity = 0
+        self._task.matrix.full_grid_opacity = 0
+        self._task.matrix.grid_stimuli_height = 0.8
+        self._task.generate_stimuli = self.generate_stimuli
+
+    def create_testing_grid(self):
+        """Create Testing Grid.
+
+        To test timing, we require the photodiode stimuli to flicker at the rate used in the execute method. The middle
+            of the existing grid is replaced with the necessary stimuli.
+        """
+        mid = int(len(self._task.matrix.symbol_set) / 2)
+
+        for i, stim in enumerate(self.stimuli):
+            self._task.matrix.symbol_set[mid + i] = stim
+
+    def generate_stimuli(self):
+        """Generates the inquiries to be presented.
+        Returns:
+        --------
+            tuple(
+                samples[list[list[str]]]: list of inquiries
+                timing(list[list[float]]): list of timings
+                color(list(list[str])): list of colors)
+        """
+        samples, times, colors = [], [], []
+        stimuli = cycle(self.stimuli)
+
+        # alternate between solid and empty boxes
+        time_stim = self._task.timing
+        color_stim = self._task.color
+
+        inq_len = self._task.stim_length
+        inq_stim = [next(stimuli) for _ in range(inq_len)]
+        inq_times = [time_stim[0] for _ in range(inq_len)]
+        inq_colors = [color_stim[0] for _ in range(inq_len)]
+
+        for _ in range(self._task.stim_number):
+            samples.append(inq_stim)
+            times.append(inq_times)
+            colors.append(inq_colors)
+
+        return (samples, times, colors)
+
+    def execute(self):
+        self.logger.debug(f'Starting {self.name()}!')
+        self._task.execute()
+
+    @classmethod
+    def label(cls):
+        return MatrixTimingVerificationCalibration.TASK_NAME
+
+    def name(self):
+        return MatrixTimingVerificationCalibration.TASK_NAME
```

### Comparing `bcipy-2.0.0rc3/bcipy/task/paradigm/rsvp/copy_phrase.py` & `bcipy-2.0.1rc2/bcipy/task/paradigm/rsvp/copy_phrase.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,876 +1,904 @@
-import logging
-from typing import List, NamedTuple, Optional, Tuple
-
-from psychopy import core
-
-from bcipy.config import (
-    SESSION_DATA_FILENAME, TRIGGER_FILENAME, WAIT_SCREEN_MESSAGE, SESSION_SUMMARY_FILENAME)
-from bcipy.display import (InformationProperties, PreviewInquiryProperties,
-                           StimuliProperties)
-from bcipy.display import Display
-from bcipy.display.paradigm.rsvp.mode.copy_phrase import CopyPhraseDisplay
-from bcipy.display.components.task_bar import CopyPhraseTaskBar
-from bcipy.feedback.visual.visual_feedback import VisualFeedback
-from bcipy.helpers.clock import Clock
-from bcipy.helpers.copy_phrase_wrapper import CopyPhraseWrapper
-from bcipy.helpers.exceptions import TaskConfigurationException
-from bcipy.helpers.list import destutter
-from bcipy.helpers.save import _save_session_related_data
-from bcipy.helpers.session import session_excel
-from bcipy.helpers.stimuli import InquirySchedule, StimuliOrder
-from bcipy.helpers.task import (construct_triggers,
-                                fake_copy_phrase_decision,
-                                get_data_for_decision, get_user_input,
-                                target_info, trial_complete_message)
-from bcipy.helpers.symbols import BACKSPACE_CHAR, alphabet
-from bcipy.helpers.triggers import (FlushFrequency, Trigger, TriggerHandler,
-                                    TriggerType, convert_timing_triggers)
-from bcipy.signal.model.inquiry_preview import compute_probs_after_preview
-from bcipy.task import Task
-from bcipy.task.data import EvidenceType, Inquiry, Session
-
-
-class Decision(NamedTuple):
-    """Represents the result of evaluating evidence.
-
-    Attrs
-    -----
-    - decision_made : whether or a not there was a commitment to a letter.
-    - selection : selected letter; will be an empty string if there was no
-    commitment.
-    - spelled_text : spelled text resulting from the decision.
-    - new_inq_schedule : the next inquiry to present if there was not a
-    decision.
-    """
-    decision_made: bool
-    selection: str
-    spelled_text: str
-    new_inq_schedule: Optional[InquirySchedule]
-
-
-class RSVPCopyPhraseTask(Task):
-    """RSVP Copy Phrase Task.
-
-    Initializes and runs all needed code for executing a copy phrase task. A
-        phrase is set in parameters and necessary objects (daq, display) are
-        passed to this function. Certain Wrappers and Task Specific objects are
-        executed here.
-
-    Parameters
-    ----------
-        win : object,
-            display window to present visual stimuli.
-        daq : object,
-            data acquisition object initialized for the desired protocol
-        parameters : dict,
-            configuration details regarding the experiment. See parameters.json
-        file_save : str,
-            path location of where to save data from the session
-        signal_model : loaded pickle file,
-            trained signal model.
-        language_model: object,
-            trained language model.
-        fake : boolean, optional
-            boolean to indicate whether this is a fake session or not.
-    Returns
-    -------
-        file_save : str,
-            path location of where to save data from the session
-    """
-
-    TASK_NAME = 'RSVP Copy Phrase Task'
-    MODE = 'RSVP'
-
-    PARAMETERS_USED = [
-        'time_fixation', 'time_flash', 'time_prompt', 'trial_length',
-        'font', 'fixation_color', 'trigger_type',
-        'filter_high', 'filter_low', 'filter_order', 'notch_filter_frequency', 'down_sampling_rate', 'prestim_length',
-        'is_txt_stim', 'lm_backspace_prob', 'backspace_always_shown',
-        'decision_threshold', 'max_inq_len', 'max_inq_per_series', 'max_minutes', 'max_selections', 'min_inq_len',
-        'show_feedback', 'feedback_duration',
-        'show_preview_inquiry', 'preview_inquiry_isi',
-        'preview_inquiry_key_input', 'preview_inquiry_length', 'preview_inquiry_progress_method',
-        'spelled_letters_count', 'static_trigger_offset',
-        'stim_color', 'stim_height', 'stim_jitter', 'stim_length', 'stim_number',
-        'stim_order', 'stim_pos_x', 'stim_pos_y', 'stim_space_char', 'target_color',
-        'task_buffer_length', 'task_color', 'task_height', 'task_text',
-        'info_pos_x', 'info_pos_y', 'info_color', 'info_height', 'info_text', 'info_color', 'info_height', 'info_text',
-    ]
-
-    def __init__(self, win, daq, parameters, file_save, signal_model,
-                 language_model, fake):
-        super(RSVPCopyPhraseTask, self).__init__()
-
-        self.window = win
-        self.daq = daq
-        self.parameters = parameters
-
-        self.validate_parameters()
-
-        self.static_clock = core.StaticPeriod(
-            screenHz=self.window.getActualFrameRate())
-        self.experiment_clock = Clock()
-        self.start_time = self.experiment_clock.getTime()
-
-        self.alp = alphabet(self.parameters)
-
-        self.button_press_error_prob = 0.05
-        self.evidence_types = [EvidenceType.LM, EvidenceType.ERP]
-        if self.parameters['show_preview_inquiry']:
-            self.evidence_types.append(EvidenceType.BTN)
-
-        self.file_save = file_save
-
-        self.trigger_handler = TriggerHandler(self.file_save, TRIGGER_FILENAME, FlushFrequency.EVERY)
-        self.session_save_location = f"{self.file_save}/{SESSION_DATA_FILENAME}"
-        self.copy_phrase = parameters['task_text']
-
-        self.fake = fake
-        self.language_model = language_model
-        self.signal_model = signal_model
-        self.evidence_precision = 5
-
-        self.feedback = VisualFeedback(
-            self.window,
-            {'feedback_font': self.parameters['font'],
-             'feedback_color': self.parameters['info_color'],
-             'feedback_pos_x': self.parameters['info_pos_x'],
-             'feedback_pos_y': self.parameters['info_pos_y'],
-             'feedback_stim_height': self.parameters['info_height'],
-             'feedback_duration': self.parameters['feedback_duration']},
-            self.experiment_clock)
-
-        self.setup()
-
-        # set a preview_only parameter
-        self.parameters.add_entry(
-            'preview_only',
-            {
-                'value': 'true' if self.parameters['preview_inquiry_progress_method'] == 0 else 'false',
-                'section': '',
-                'readableName': '',
-                'helpTip': '',
-                'recommended_values': '',
-                'type': 'bool'
-            }
-        )
-
-        self.rsvp = self.init_display()
-
-    def setup(self) -> None:
-        """Initialize/reset parameters used in the execute run loop."""
-
-        self.spelled_text = str(
-            self.copy_phrase[0:self.starting_spelled_letters()])
-        self.last_selection = ''
-        self.inq_counter = 0
-        self.session = Session(
-            save_location=self.file_save,
-            task='Copy Phrase',
-            mode=self.MODE,
-            symbol_set=self.alp,
-            decision_threshold=self.parameters['decision_threshold'])
-        self.write_session_data()
-
-        self.init_copy_phrase_task()
-        self.current_inquiry = self.next_inquiry()
-
-    def init_display(self) -> Display:
-        """Initialize the display"""
-        return _init_copy_phrase_display(self.parameters, self.window,
-                                         self.static_clock,
-                                         self.experiment_clock,
-                                         self.spelled_text)
-
-    def validate_parameters(self) -> None:
-        """Validate.
-
-        Confirm Task is configured with correct parameters and within operating limits.
-        """
-
-        # ensure all required parameters are provided
-        for param in RSVPCopyPhraseTask.PARAMETERS_USED:
-            if param not in self.parameters:
-                raise TaskConfigurationException(f"parameter '{param}' is required")
-
-        # ensure data / query parameters are set correctly
-        buffer_len = self.parameters['task_buffer_length']
-        prestim = self.parameters['prestim_length']
-        poststim = self.parameters['trial_length']
-        if buffer_len < prestim:
-            raise TaskConfigurationException(
-                f'task_buffer_length=[{buffer_len}] must be greater than prestim_length=[{prestim}]')
-
-        if buffer_len < poststim:
-            raise TaskConfigurationException(
-                f'task_buffer_length=[{buffer_len}] must be greater than trial_length=[{poststim}]')
-
-    def starting_spelled_letters(self) -> int:
-        """Number of letters already spelled at the start of the task."""
-        spelled_letters_count = self.parameters['spelled_letters_count']
-        if spelled_letters_count > len(self.copy_phrase):
-            self.logger.debug('Already spelled letters exceeds phrase length.')
-            spelled_letters_count = 0
-        return spelled_letters_count
-
-    def next_inquiry(self) -> Optional[InquirySchedule]:
-        """Generate an InquirySchedule for spelling the next letter."""
-        if self.copy_phrase_task:
-            _, inquiry_schedule = self.copy_phrase_task.initialize_series()
-            return inquiry_schedule
-        return None
-
-    def init_copy_phrase_task(self) -> None:
-        """Initialize the CopyPhraseWrapper.
-
-        Returns:
-        --------
-        initialized CopyPhraseWrapper
-        """
-
-        self.copy_phrase_task = CopyPhraseWrapper(
-            self.parameters['min_inq_len'],
-            self.parameters['max_inq_per_series'],
-            lmodel=self.language_model,
-            device_spec=self.daq.device_spec,
-            signal_model=self.signal_model,
-            k=self.parameters['down_sampling_rate'],
-            alp=self.alp,
-            evidence_names=self.evidence_types,
-            task_list=[(str(self.copy_phrase), self.spelled_text)],
-            is_txt_stim=self.parameters['is_txt_stim'],
-            stim_timing=[
-                self.parameters['time_fixation'], self.parameters['time_flash']
-            ],
-            decision_threshold=self.parameters['decision_threshold'],
-            backspace_prob=self.parameters['lm_backspace_prob'],
-            backspace_always_shown=self.parameters['backspace_always_shown'],
-            filter_high=self.parameters['filter_high'],
-            filter_low=self.parameters['filter_low'],
-            filter_order=self.parameters['filter_order'],
-            notch_filter_frequency=self.parameters['notch_filter_frequency'],
-            stim_length=self.parameters['stim_length'],
-            stim_jitter=self.parameters['stim_jitter'],
-            stim_order=StimuliOrder(self.parameters['stim_order']))
-
-    def user_wants_to_continue(self) -> bool:
-        """Check if user wants to continue or terminate.
-
-        Returns
-        -------
-        - `True` to continue
-        - `False` to finish the task.
-        """
-        should_continue = get_user_input(
-            self.rsvp,
-            WAIT_SCREEN_MESSAGE,
-            self.parameters['stim_color'],
-            first_run=self.first_run)
-        if not should_continue:
-            self.logger.debug('User wants to exit.')
-        return should_continue
-
-    def wait(self, seconds: float = None):
-        """Pause for a time.
-
-        Parameters
-        ----------
-        - seconds : duration of time to wait; if missing, defaults to the
-        value of the parameter `'task_buffer_length'`
-        """
-        seconds = seconds or self.parameters['task_buffer_length']
-        core.wait(seconds)
-
-    def present_inquiry(self, inquiry_schedule: InquirySchedule
-                        ) -> Tuple[List[Tuple[str, float]], bool]:
-        """Present the given inquiry and return the trigger timing info.
-
-        Parameters
-        ----------
-        - inquiry_schedule : schedule for next sequences of stimuli to present.
-        Currently, only the first list of stims in the schedule is used.
-
-        Returns
-        -------
-        Tuple of `(stim_times, proceed)`
-
-        - stim_times : list of tuples representing the stimulus and time that
-        it was presented relative to the experiment clock. Non-stim triggers
-        may be also be included in the list ('calibration', etc).
-        - proceed : indicates whether to proceed with evaluating eeg evidence.
-        a value of False indicates that the inquiry was previewed but not
-        presented in sequence.
-        """
-        # Update task state and reset the static
-        self.rsvp.update_task_bar(self.spelled_text)
-        self.rsvp.draw_static()
-        self.window.flip()
-
-        self.wait()
-
-        # Setup the new stimuli
-        self.rsvp.schedule_to(stimuli=inquiry_schedule.stimuli[0],
-                              timing=inquiry_schedule.durations[0],
-                              colors=inquiry_schedule.colors[0]
-                              if self.parameters['is_txt_stim'] else None)
-
-        if self.parameters['show_preview_inquiry']:
-            stim_times, proceed = self.rsvp.preview_inquiry()
-            if proceed:
-                stim_times.extend(self.rsvp.do_inquiry())
-        else:
-            stim_times = self.rsvp.do_inquiry()
-            proceed = True
-
-        return stim_times, proceed
-
-    def show_feedback(self, selection: str, correct: bool = True):
-        """Display the selection as feedback if the 'show_feedback'
-        parameter is configured.
-
-        Parameters
-        ----------
-        - selection : selected stimulus to display
-        - correct : whether or not the correct stim was chosen
-        """
-        if self.parameters['show_feedback']:
-            self.feedback.administer(f'Selected: {selection}')
-
-    def check_stop_criteria(self) -> bool:
-        """Returns True if experiment is currently within params and the task
-        should continue.
-        """
-        if self.copy_phrase == self.spelled_text:
-            self.logger.debug('Spelling complete')
-            return False
-
-        if (self.inq_counter + 1) >= self.parameters['max_inq_len']:
-            self.logger.debug('Max tries exceeded: to allow for more tries'
-                              ' adjust the Maximum inquiry Length '
-                              '(max_inq_len) parameter.')
-            return False
-
-        if self.session.total_time_spent >= (self.parameters['max_minutes'] *
-                                             60):
-            self.logger.debug('Max time exceeded. To allow for more time '
-                              'adjust the max_minutes parameter.')
-            return False
-
-        if self.session.total_number_decisions >= self.parameters['max_selections']:
-            self.logger.debug('Max number of selections reached '
-                              '(configured with the max_selections parameter)')
-            return False
-
-        return True
-
-    def next_target(self) -> str:
-        """Computes the next target letter based on the currently spelled_text.
-        """
-        if self.copy_phrase[0:len(self.spelled_text)] == self.spelled_text:
-            # if correctly spelled so far, get the next letter.
-            return self.copy_phrase[len(self.spelled_text)]
-        return BACKSPACE_CHAR
-
-    def execute(self) -> str:
-        """Executes the task.
-
-        Returns
-        -------
-        data save location (triggers.txt, session.json)
-        """
-        self.logger.debug('Starting Copy Phrase Task!')
-        run = True
-        self.wait()  # buffer for data processing
-
-        while run and self.user_wants_to_continue() and self.current_inquiry:
-            target_stimuli = self.next_target()
-            stim_times, proceed = self.present_inquiry(
-                self.current_inquiry)
-
-            self.write_trigger_data(stim_times, target_stimuli)
-            self.wait()
-
-            evidence_types = self.add_evidence(stim_times, proceed)
-            decision = self.evaluate_evidence()
-
-            data = self.new_data_record(stim_times,
-                                        target_stimuli,
-                                        current_text=self.spelled_text,
-                                        decision=decision,
-                                        evidence_types=evidence_types)
-            self.update_session_data(data,
-                                     save=True,
-                                     decision_made=decision.decision_made)
-
-            if decision.decision_made:
-                self.show_feedback(decision.selection,
-                                   (decision.selection == target_stimuli))
-                self.spelled_text = decision.spelled_text
-                self.current_inquiry = self.next_inquiry()
-
-            else:
-                self.current_inquiry = decision.new_inq_schedule
-
-            run = self.check_stop_criteria()
-            self.inq_counter += 1
-
-        self.exit_display()
-        self.write_offset_trigger()
-
-        self.session.task_summary = TaskSummary(
-            self.session, self.parameters['show_preview_inquiry'],
-            self.parameters['preview_inquiry_progress_method'],
-            self.trigger_handler.file_path).as_dict()
-        self.write_session_data()
-
-        # Evidence is not recorded in the session when using fake decisions.
-        if self.parameters['summarize_session'] and self.session.has_evidence():
-            session_excel(session=self.session,
-                          excel_file=f"{self.file_save}/{SESSION_SUMMARY_FILENAME}")
-
-        # Wait some time before exiting so there is trailing eeg data saved
-        self.wait()
-
-        return self.file_save
-
-    def evaluate_evidence(self) -> Decision:
-        """Uses the `copy_phrase_task` parameter to evaluate the provided
-        evidence and attempt a decision.
-
-        Modifies
-        --------
-        - self.copy_phrase_task
-        """
-        if self.fake:
-            _, spelled, _ = fake_copy_phrase_decision(self.copy_phrase,
-                                                      self.next_target(),
-                                                      self.spelled_text)
-            # Reset the stoppage criteria by forcing the commit to a decision.
-            self.copy_phrase_task.decision_maker.do_series()
-            # In fake mode, only the LM is providing evidence, so the decision
-            # made is the highest symbol predicted. Override this state
-            self.copy_phrase_task.decision_maker.update(spelled)
-
-            # In fake mode, all inquiries result in a selection.
-            return Decision(decision_made=True,
-                            selection=spelled[-1],
-                            spelled_text=spelled,
-                            new_inq_schedule=None)
-
-        decision_made, new_sti = self.copy_phrase_task.decide()
-        spelled_text = self.copy_phrase_task.decision_maker.displayed_state
-        selection = ''
-        if decision_made:
-            selection = self.copy_phrase_task.decision_maker.last_selection
-
-        return Decision(decision_made, selection, spelled_text, new_sti)
-
-    def add_evidence(self, stim_times: List[List],
-                     proceed: bool = True) -> List[EvidenceType]:
-        """Add all evidence used to make a decision.
-
-        Parameters
-        ----------
-        - stim_times : list of stimuli returned from the display
-        - proceed : whether or not to proceed with the inquiry
-
-        Returns
-        -------
-        list of evidence types added
-
-        Modifies
-        --------
-        - self.copy_phrase_task
-        """
-        evidences = [
-            self.compute_button_press_evidence(proceed),
-            self.compute_eeg_evidence(stim_times, proceed)
-        ]
-        evidence_types = []
-        for evidence in evidences:
-            if evidence:
-                evidence_type, probs = evidence
-                evidence_types.append(evidence_type)
-                self.copy_phrase_task.add_evidence(evidence_type, probs)
-        if self.session.latest_series_is_empty():
-            evidence_types.append(EvidenceType.LM)
-        return evidence_types
-
-    def compute_button_press_evidence(
-            self, proceed: bool) -> Optional[Tuple[EvidenceType, List[float]]]:
-        """If 'show_preview_inquiry' feature is enabled, compute the button
-        press evidence and add it to the copy phrase task.
-
-        Parameters
-        ----------
-            proceed : whether to proceed with the inquiry after the preview
-
-        Returns
-        -------
-            tuple of (evidence type, evidence) or None if inquiry preview is
-            not enabled.
-        """
-        if not self.parameters['show_preview_inquiry'] \
-                or not self.current_inquiry \
-                or self.parameters['preview_only']:
-            return None
-        probs = compute_probs_after_preview(self.current_inquiry.stimuli[0],
-                                            self.alp,
-                                            self.button_press_error_prob,
-                                            proceed)
-        return (EvidenceType.BTN, probs)
-
-    def compute_eeg_evidence(self,
-                             stim_times: List[List],
-                             proceed: bool = True
-                             ) -> Optional[Tuple[EvidenceType, List[float]]]:
-        """Evaluate the EEG evidence and add it to the copy_phrase_task, but
-        don't yet attempt a decision.
-
-        Parameters
-        ----------
-        - stim_times : list of stimuli returned from the display
-        - proceed : whether or not to evaluate the evidence, if `False` returns
-        empty values.
-
-        Returns
-        -------
-        tuple of (evidence type, evidence)
-        """
-        if not proceed or self.fake:
-            return None
-
-        # currently prestim_length is used as a buffer for filter application, use the same at the end of the inquiry
-        post_stim_buffer = self.parameters['prestim_length']
-        raw_data, triggers = get_data_for_decision(
-            inquiry_timing=self.stims_for_decision(stim_times),
-            daq=self.daq,
-            offset=self.parameters['static_trigger_offset'],
-            prestim=self.parameters['prestim_length'],
-            poststim=post_stim_buffer + self.parameters['trial_length'])
-
-        # we assume all are nontargets at this point
-        labels = ['nontarget'] * len(triggers)
-
-        probs = self.copy_phrase_task.evaluate_eeg_evidence(
-            raw_data, triggers, labels, self.parameters['trial_length'])
-        return (EvidenceType.ERP, probs)
-
-    def stims_for_decision(self, stim_times: List[List]) -> List[List]:
-        """The stim_timings from the display may include non-letter stimuli
-        such as calibration and inquiry_preview timings. This method extracts
-        only the letter data used to process the data for a decision.
-
-        Parameters
-        ----------
-        - stim_times : list of [stim, clock_time] pairs returned from display.
-
-        Returns
-        -------
-        stim times where the stim is in the current alphabet; filters out
-        'calibration', 'inquiry_preview', etc.
-        """
-        return [
-            timing for timing in stim_times if timing[0] in (self.alp + ['+'])
-        ]
-
-    def new_data_record(self,
-                        stim_times: List[List],
-                        target_stimuli: str,
-                        current_text: str,
-                        decision: Decision,
-                        evidence_types: List[EvidenceType] = None) -> Inquiry:
-        """Construct a new inquiry data record.
-
-        Parameters
-        ----------
-        - stim_times : list of [stim, clock_time] pairs returned from display.
-        - target_stimuli : stim the user is currently attempting to spell.
-        - current_text : spelled text before the inquiry
-        - decision : decision made by the decision maker
-        - evidence_types : evidence provided to the decision-maker during the
-        current inquiry.
-
-        Returns
-        -------
-        Inquiry data for the current schedule; returned value only contains
-        evidence for the provided evidence_types, leaving the other types empty
-        """
-        assert self.current_inquiry, "Current inquiry is required"
-        evidence_types = evidence_types or []
-        triggers = construct_triggers(self.stims_for_decision(stim_times))
-        data = Inquiry(stimuli=self.current_inquiry.stimuli,
-                       timing=self.current_inquiry.durations,
-                       triggers=triggers,
-                       target_info=target_info(triggers, target_stimuli,
-                                               self.parameters['is_txt_stim']),
-                       target_letter=target_stimuli,
-                       current_text=current_text,
-                       target_text=self.copy_phrase,
-                       selection=decision.selection,
-                       next_display_state=decision.spelled_text)
-        data.precision = self.evidence_precision
-
-        if not self.fake:
-            latest_evidence = self.copy_phrase_task.conjugator.latest_evidence
-            data.evidences = {
-                ev_type: evidence if ev_type in evidence_types else []
-                for ev_type, evidence in latest_evidence.items()
-            }
-            data.likelihood = list(self.copy_phrase_task.conjugator.likelihood)
-        return data
-
-    def exit_display(self):
-        """Close the UI and cleanup."""
-        # Update task state and reset the static
-        self.rsvp.update_task_bar(text=self.spelled_text)
-
-        # Say Goodbye!
-        self.rsvp.info_text = trial_complete_message(self.window, self.parameters)
-        self.rsvp.draw_static()
-        self.window.flip()
-
-        # Give the system time to process
-        self.wait()
-
-    def update_session_data(self,
-                            data: Inquiry,
-                            save: bool = True,
-                            decision_made: bool = False) -> None:
-        """Update the current session with the latest inquiry data
-
-        Parameters
-        ----------
-        - data : inquiry to append to the session
-        - save : if True, persists the session to disk.
-
-        Modifies
-        --------
-        - self.session
-        """
-        self.session.add_sequence(data)
-        self.session.total_time_spent = self.experiment_clock.getTime() - self.start_time
-        if save:
-            self.write_session_data()
-        if decision_made:
-            self.session.add_series()
-
-    def write_session_data(self) -> None:
-        """Save session data to disk."""
-        if self.session:
-            session_file = _save_session_related_data(
-                self.session_save_location,
-                self.session.as_dict())
-            session_file.close()
-
-    def write_offset_trigger(self) -> None:
-        """Append the offset to the end of the triggers file.
-        """
-        if self.daq.is_calibrated:
-            self.trigger_handler.add_triggers(
-                [Trigger(
-                    'daq_sample_offset',
-                    TriggerType.SYSTEM,
-                    # to help support future refactoring or use of lsl timestamps only
-                    # we write only the sample offset here
-                    self.daq.offset(self.rsvp.first_stim_time)
-                )])
-        self.trigger_handler.close()
-
-    def write_trigger_data(self, stim_times: List[Tuple[str, float]], target_stimuli: str) -> None:
-        """Save trigger data to disk.
-
-        Parameters
-        ----------
-        - stim_times : list of (stim, clock_time) tuples
-        - target_stimuli : current target stimuli
-        """
-        if self.first_run and self.daq.is_calibrated:
-            # write offset first
-            self.trigger_handler.add_triggers(
-                [Trigger(
-                    'starting_offset',
-                    TriggerType.OFFSET,
-                    # offset will factor in true offset and time relative from beginning
-                    (self.daq.offset(self.rsvp.first_stim_time) - self.rsvp.first_stim_time)
-                )]
-            )
-
-        triggers = convert_timing_triggers(stim_times, target_stimuli, self.trigger_type)
-        self.trigger_handler.add_triggers(triggers)
-
-    def trigger_type(self, symbol: str, target: str, index: int) -> TriggerType:
-        """Trigger Type.
-
-        Cast a given symbol to a TriggerType.
-        """
-        if symbol == 'inquiry_preview':
-            return TriggerType.PREVIEW
-        if 'bcipy_key_press' in symbol:
-            return TriggerType.EVENT
-        if symbol == '+':
-            return TriggerType.FIXATION
-        if target == symbol:
-            return TriggerType.TARGET
-        return TriggerType.NONTARGET
-
-    def name(self) -> str:
-        return self.TASK_NAME
-
-    @property
-    def first_run(self) -> bool:
-        """First run.
-
-        Determines whether it is the first inquiry presentation / run.
-        """
-        return self.inq_counter == 0
-
-
-class TaskSummary:
-    """Summary data for tracking performance metrics.
-
-    Parameters
-    ----------
-        session - current session information
-        show_preview - whether or not inquiry preview was displayed
-        preview_mode - the switch mode for inquiry preview:
-            0 = preview only;
-            1 = press to confirm;
-            2 = press to skip to another inquiry
-    """
-
-    def __init__(self,
-                 session: Session,
-                 show_preview: bool = False,
-                 preview_mode: int = 0,
-                 trigger_path: str = None):
-        assert preview_mode in range(3), 'Preview mode out of range'
-        self.session = session
-        self.show_preview = show_preview
-        self.preview_mode = preview_mode
-        self.trigger_path = trigger_path
-        self.logger = logging.getLogger(__name__)
-
-    def as_dict(self) -> dict:
-        """Computes the task summary data to append to the session."""
-
-        selections = [
-            inq for inq in self.session.all_inquiries if inq.selection
-        ]
-        correct = [inq for inq in selections if inq.is_correct_decision]
-        incorrect = [inq for inq in selections if not inq.is_correct_decision]
-
-        # Note that SPACE is considered a symbol
-        correct_symbols = [
-            inq for inq in correct if inq.selection != BACKSPACE_CHAR
-        ]
-
-        btn_presses = self.btn_press_count()
-        sel_count = len(selections)
-        switch_per_selection = (btn_presses /
-                                sel_count) if sel_count > 0 else 0
-        accuracy = (len(correct) / sel_count) if sel_count > 0 else 0
-
-        # Note that minutes includes startup time and any breaks.
-        minutes = self.session.total_time_spent / 60
-        return {
-            'selections_correct': len(correct),
-            'selections_incorrect': len(incorrect),
-            'selections_correct_symbols': len(correct_symbols),
-            'switch_total': btn_presses,
-            'switch_per_selection': switch_per_selection,
-            'switch_response_time': self.switch_response_time(),
-            'typing_accuracy': accuracy,
-            'correct_rate': len(correct) / minutes if minutes else 0,
-            'copy_rate': len(correct_symbols) / minutes if minutes else 0
-        }
-
-    def btn_press_count(self) -> int:
-        """Compute the number of times the switch was activated. Returns 0 if
-        inquiry preview mode was off or mode was preview-only."""
-
-        if not self.show_preview or self.preview_mode == 0:
-            return 0
-
-        inquiries = self.session.all_inquiries
-        if self.preview_mode == 1:
-            # press to confirm
-            activations = [inq for inq in inquiries if inq.eeg_evidence]
-        elif self.preview_mode == 2:
-            # press to skip
-            activations = [inq for inq in inquiries if not inq.eeg_evidence]
-        return len(activations)
-
-    def switch_response_time(self) -> Optional[float]:
-        """Computes the average switch response in seconds."""
-
-        # Remove consecutive items with the same type; we are only interested
-        # in PREVIEW followed by a EVENT.
-        triggers = destutter(self.switch_triggers(), key=lambda trg: trg.type)
-        pairs = list(zip(triggers[::2], triggers[1::2]))
-
-        # Confirm that the data is structured as expected.
-        for preview, keypress in pairs:
-            if (preview.type != TriggerType.PREVIEW) or (
-                    keypress.type != TriggerType.EVENT):
-                self.logger.info('Could not compute switch_response_time')
-                return None
-
-        response_times = [
-            keypress.time - preview.time for preview, keypress in pairs
-        ]
-        count = len(response_times)
-        return sum(response_times) / count if count > 0 else None
-
-    def switch_triggers(self) -> List[Trigger]:
-        """Returns a list of switch-related triggers"""
-        if not self.trigger_path:
-            return []
-        triggers, _offset = TriggerHandler.read_text_file(self.trigger_path)
-        return [
-            trg for trg in triggers
-            if trg.type in [TriggerType.PREVIEW, TriggerType.EVENT]
-        ]
-
-
-def _init_copy_phrase_display(parameters, win, static_clock, experiment_clock, starting_spelled_text):
-    preview_inquiry = PreviewInquiryProperties(
-        preview_only=parameters['preview_only'],
-        preview_inquiry_length=parameters['preview_inquiry_length'],
-        preview_inquiry_key_input=parameters['preview_inquiry_key_input'],
-        preview_inquiry_progress_method=parameters[
-            'preview_inquiry_progress_method'],
-        preview_inquiry_isi=parameters['preview_inquiry_isi'])
-    info = InformationProperties(
-        info_color=[parameters['info_color']],
-        info_pos=[(parameters['info_pos_x'], parameters['info_pos_y'])],
-        info_height=[parameters['info_height']],
-        info_font=[parameters['font']],
-        info_text=[parameters['info_text']],
-    )
-    stimuli = StimuliProperties(stim_font=parameters['font'],
-                                stim_pos=(parameters['stim_pos_x'],
-                                          parameters['stim_pos_y']),
-                                stim_height=parameters['stim_height'],
-                                stim_inquiry=['A'] * parameters['stim_length'],
-                                stim_colors=[parameters['stim_color']] * parameters['stim_length'],
-                                stim_timing=[10] * parameters['stim_length'],
-                                is_txt_stim=parameters['is_txt_stim'])
-
-    task_bar = CopyPhraseTaskBar(win,
-                                 task_text=parameters['task_text'],
-                                 spelled_text=starting_spelled_text,
-                                 colors=[parameters['task_color']],
-                                 font=parameters['font'],
-                                 height=parameters['task_height'])
-
-    return CopyPhraseDisplay(win,
-                             static_clock,
-                             experiment_clock,
-                             stimuli,
-                             task_bar,
-                             info,
-                             starting_spelled_text,
-                             trigger_type=parameters['trigger_type'],
-                             space_char=parameters['stim_space_char'],
-                             preview_inquiry=preview_inquiry)
+import logging
+from typing import List, NamedTuple, Optional, Tuple
+
+from psychopy import core
+
+from bcipy.config import (
+    SESSION_DATA_FILENAME, TRIGGER_FILENAME, WAIT_SCREEN_MESSAGE, SESSION_SUMMARY_FILENAME)
+from bcipy.display import (InformationProperties, PreviewInquiryProperties,
+                           StimuliProperties, TaskDisplayProperties)
+from bcipy.display.paradigm.rsvp.mode.copy_phrase import CopyPhraseDisplay
+from bcipy.feedback.visual.visual_feedback import VisualFeedback
+from bcipy.helpers.clock import Clock
+from bcipy.helpers.copy_phrase_wrapper import CopyPhraseWrapper
+from bcipy.helpers.exceptions import TaskConfigurationException
+from bcipy.helpers.list import destutter
+from bcipy.helpers.save import _save_session_related_data
+from bcipy.helpers.session import session_excel
+from bcipy.helpers.stimuli import InquirySchedule, StimuliOrder
+from bcipy.helpers.task import (BACKSPACE_CHAR, alphabet, construct_triggers,
+                                fake_copy_phrase_decision,
+                                get_data_for_decision, get_user_input,
+                                target_info, trial_complete_message)
+from bcipy.helpers.triggers import (FlushFrequency, Trigger, TriggerHandler,
+                                    TriggerType, convert_timing_triggers)
+from bcipy.signal.model.inquiry_preview import compute_probs_after_preview
+from bcipy.task import Task
+from bcipy.task.data import EvidenceType, Inquiry, Session
+
+
+class Decision(NamedTuple):
+    """Represents the result of evaluating evidence.
+
+    Attrs
+    -----
+    - decision_made : whether or a not there was a commitment to a letter.
+    - selection : selected letter; will be an empty string if there was no
+    commitment.
+    - spelled_text : spelled text resulting from the decision.
+    - new_inq_schedule : the next inquiry to present if there was not a
+    decision.
+    """
+    decision_made: bool
+    selection: str
+    spelled_text: str
+    new_inq_schedule: Optional[InquirySchedule]
+
+
+class RSVPCopyPhraseTask(Task):
+    """RSVP Copy Phrase Task.
+
+    Initializes and runs all needed code for executing a copy phrase task. A
+        phrase is set in parameters and necessary objects (daq, display) are
+        passed to this function. Certain Wrappers and Task Specific objects are
+        executed here.
+
+    Parameters
+    ----------
+        win : object,
+            display window to present visual stimuli.
+        daq : object,
+            data acquisition object initialized for the desired protocol
+        parameters : dict,
+            configuration details regarding the experiment. See parameters.json
+        file_save : str,
+            path location of where to save data from the session
+        signal_model : loaded pickle file,
+            trained signal model.
+        language_model: object,
+            trained language model.
+        fake : boolean, optional
+            boolean to indicate whether this is a fake session or not.
+    Returns
+    -------
+        file_save : str,
+            path location of where to save data from the session
+    """
+
+    TASK_NAME = 'RSVP Copy Phrase Task'
+    PARAMETERS_USED = [
+        'time_fixation', 'time_flash', 'time_prompt', 'trial_length',
+        'font', 'fixation_color', 'trigger_type',
+        'filter_high', 'filter_low', 'filter_order', 'notch_filter_frequency', 'down_sampling_rate', 'prestim_length',
+        'is_txt_stim', 'lm_backspace_prob', 'backspace_always_shown',
+        'decision_threshold', 'max_inq_len', 'max_inq_per_series', 'max_minutes', 'max_selections', 'min_inq_len',
+        'show_feedback', 'feedback_duration',
+        'show_preview_inquiry', 'preview_inquiry_isi',
+        'preview_inquiry_key_input', 'preview_inquiry_length', 'preview_inquiry_progress_method',
+        'spelled_letters_count', 'static_trigger_offset',
+        'stim_color', 'stim_height', 'stim_jitter', 'stim_length', 'stim_number',
+        'stim_order', 'stim_pos_x', 'stim_pos_y', 'stim_space_char', 'target_color',
+        'task_buffer_length', 'task_color', 'task_height', 'task_text',
+        'info_pos_x', 'info_pos_y', 'info_color', 'info_height', 'info_text', 'info_color', 'info_height', 'info_text',
+    ]
+
+    def __init__(self, win, daq, parameters, file_save, signal_model,
+                 language_model, fake):
+        super(RSVPCopyPhraseTask, self).__init__()
+
+        self.window = win
+        self.daq = daq
+        self.parameters = parameters
+
+        self.validate_parameters()
+
+        self.static_clock = core.StaticPeriod(
+            screenHz=self.window.getActualFrameRate())
+        self.experiment_clock = Clock()
+        self.start_time = self.experiment_clock.getTime()
+
+        self.alp = alphabet(self.parameters)
+
+        self.button_press_error_prob = 0.05
+        self.evidence_types = [EvidenceType.LM, EvidenceType.ERP]
+        if self.parameters['show_preview_inquiry']:
+            self.evidence_types.append(EvidenceType.BTN)
+
+        self.file_save = file_save
+
+        self.trigger_handler = TriggerHandler(self.file_save, TRIGGER_FILENAME, FlushFrequency.EVERY)
+        self.session_save_location = f"{self.file_save}/{SESSION_DATA_FILENAME}"
+        self.copy_phrase = parameters['task_text']
+
+        self.fake = fake
+        self.language_model = language_model
+        self.signal_model = signal_model
+        self.evidence_precision = 5
+
+        self.feedback = VisualFeedback(
+            self.window,
+            {'feedback_font': self.parameters['font'],
+             'feedback_color': self.parameters['info_color'],
+             'feedback_pos_x': self.parameters['info_pos_x'],
+             'feedback_pos_y': self.parameters['info_pos_y'],
+             'feedback_stim_height': self.parameters['info_height'],
+             'feedback_duration': self.parameters['feedback_duration']},
+            self.experiment_clock)
+
+        self.setup()
+
+        # set a preview_only parameter
+        self.parameters.add_entry(
+            'preview_only',
+            {
+                'value': 'true' if self.parameters['preview_inquiry_progress_method'] == 0 else 'false',
+                'section': '',
+                'readableName': '',
+                'helpTip': '',
+                'recommended_values': '',
+                'type': 'bool'
+            }
+        )
+
+        self.rsvp = _init_copy_phrase_display(
+            self.parameters,
+            self.window,
+            self.static_clock,
+            self.experiment_clock,
+            self.spelled_text)
+
+    def setup(self) -> None:
+        """Initialize/reset parameters used in the execute run loop."""
+
+        self.spelled_text = str(
+            self.copy_phrase[0:self.starting_spelled_letters()])
+        self.last_selection = ''
+        self.inq_counter = 0
+        self.session = Session(
+            save_location=self.file_save,
+            task='Copy Phrase',
+            mode='RSVP',
+            symbol_set=self.alp,
+            decision_threshold=self.parameters['decision_threshold'])
+        self.write_session_data()
+
+        self.init_copy_phrase_task()
+        self.current_inquiry = self.next_inquiry()
+
+    def validate_parameters(self) -> None:
+        """Validate.
+
+        Confirm Task is configured with correct parameters and within operating limits.
+        """
+
+        # ensure all required parameters are provided
+        for param in RSVPCopyPhraseTask.PARAMETERS_USED:
+            if param not in self.parameters:
+                raise TaskConfigurationException(f"parameter '{param}' is required")
+
+        # ensure data / query parameters are set correctly
+        buffer_len = self.parameters['task_buffer_length']
+        prestim = self.parameters['prestim_length']
+        poststim = self.parameters['trial_length']
+        if buffer_len < prestim:
+            raise TaskConfigurationException(
+                f'task_buffer_length=[{buffer_len}] must be greater than prestim_length=[{prestim}]')
+
+        if buffer_len < poststim:
+            raise TaskConfigurationException(
+                f'task_buffer_length=[{buffer_len}] must be greater than trial_length=[{poststim}]')
+
+    def starting_spelled_letters(self) -> int:
+        """Number of letters already spelled at the start of the task."""
+        spelled_letters_count = self.parameters['spelled_letters_count']
+        if spelled_letters_count > len(self.copy_phrase):
+            self.logger.debug('Already spelled letters exceeds phrase length.')
+            spelled_letters_count = 0
+        return spelled_letters_count
+
+    def next_inquiry(self) -> Optional[InquirySchedule]:
+        """Generate an InquirySchedule for spelling the next letter."""
+        if self.copy_phrase_task:
+            _, inquiry_schedule = self.copy_phrase_task.initialize_series()
+            return inquiry_schedule
+        return None
+
+    def init_copy_phrase_task(self) -> None:
+        """Initialize the CopyPhraseWrapper.
+
+        Returns:
+        --------
+        initialized CopyPhraseWrapper
+        """
+
+        self.copy_phrase_task = _init_copy_phrase_wrapper(
+            self.parameters['min_inq_len'],
+            self.parameters['max_inq_per_series'],
+            signal_model=self.signal_model,
+            fs=self.daq.device_spec.sample_rate,
+            k=self.parameters['down_sampling_rate'],
+            alp=self.alp,
+            evidence_names=self.evidence_types,
+            task_list=[(str(self.copy_phrase), self.spelled_text)],
+            lmodel=self.language_model,
+            is_txt_stim=self.parameters['is_txt_stim'],
+            device_name=self.daq.device_spec.name,
+            device_channels=self.daq.device_spec.channels,
+            stim_timing=[
+                self.parameters['time_fixation'], self.parameters['time_flash']
+            ],
+            decision_threshold=self.parameters['decision_threshold'],
+            backspace_prob=self.parameters['lm_backspace_prob'],
+            backspace_always_shown=self.parameters['backspace_always_shown'],
+            filter_high=self.parameters['filter_high'],
+            filter_low=self.parameters['filter_low'],
+            filter_order=self.parameters['filter_order'],
+            notch_filter_frequency=self.parameters['notch_filter_frequency'],
+            stim_length=self.parameters['stim_length'],
+            stim_jitter=self.parameters['stim_jitter'],
+            stim_order=StimuliOrder(self.parameters['stim_order']))
+
+    def user_wants_to_continue(self) -> bool:
+        """Check if user wants to continue or terminate.
+
+        Returns
+        -------
+        - `True` to continue
+        - `False` to finish the task.
+        """
+        should_continue = get_user_input(
+            self.rsvp,
+            WAIT_SCREEN_MESSAGE,
+            self.parameters['stim_color'],
+            first_run=self.first_run)
+        if not should_continue:
+            self.logger.debug('User wants to exit.')
+        return should_continue
+
+    def wait(self, seconds: float = None):
+        """Pause for a time.
+
+        Parameters
+        ----------
+        - seconds : duration of time to wait; if missing, defaults to the
+        value of the parameter `'task_buffer_length'`
+        """
+        seconds = seconds or self.parameters['task_buffer_length']
+        core.wait(seconds)
+
+    def present_inquiry(self, inquiry_schedule: InquirySchedule
+                        ) -> Tuple[List[Tuple[str, float]], bool]:
+        """Present the given inquiry and return the trigger timing info.
+
+        Parameters
+        ----------
+        - inquiry_schedule : schedule for next sequences of stimuli to present.
+        Currently, only the first list of stims in the schedule is used.
+
+        Returns
+        -------
+        Tuple of `(stim_times, proceed)`
+
+        - stim_times : list of tuples representing the stimulus and time that
+        it was presented relative to the experiment clock. Non-stim triggers
+        may be also be included in the list ('calibration', etc).
+        - proceed : indicates whether to proceed with evaluating eeg evidence.
+        a value of False indicates that the inquiry was previewed but not
+        presented in sequence.
+        """
+        # Update task state and reset the static
+        self.rsvp.update_task_state(text=self.spelled_text,
+                                    color_list=['white'])
+        self.rsvp.draw_static()
+        self.window.flip()
+
+        self.wait()
+
+        # Setup the new stimuli
+        self.rsvp.stimuli_inquiry = inquiry_schedule.stimuli[0]
+        if self.parameters['is_txt_stim']:
+            self.rsvp.stimuli_colors = inquiry_schedule.colors[0]
+        self.rsvp.stimuli_timing = inquiry_schedule.durations[0]
+
+        if self.parameters['show_preview_inquiry']:
+            stim_times, proceed = self.rsvp.preview_inquiry()
+            if proceed:
+                stim_times.extend(self.rsvp.do_inquiry())
+        else:
+            stim_times = self.rsvp.do_inquiry()
+            proceed = True
+
+        return stim_times, proceed
+
+    def show_feedback(self, selection: str, correct: bool = True):
+        """Display the selection as feedback if the 'show_feedback'
+        parameter is configured.
+
+        Parameters
+        ----------
+        - selection : selected stimulus to display
+        - correct : whether or not the correct stim was chosen
+        """
+        if self.parameters['show_feedback']:
+            self.feedback.administer(f'Selected: {selection}')
+
+    def check_stop_criteria(self) -> bool:
+        """Returns True if experiment is currently within params and the task
+        should continue.
+        """
+        if self.copy_phrase == self.spelled_text:
+            self.logger.debug('Spelling complete')
+            return False
+
+        if (self.inq_counter + 1) >= self.parameters['max_inq_len']:
+            self.logger.debug('Max tries exceeded: to allow for more tries'
+                              ' adjust the Maximum inquiry Length '
+                              '(max_inq_len) parameter.')
+            return False
+
+        if self.session.total_time_spent >= (self.parameters['max_minutes'] *
+                                             60):
+            self.logger.debug('Max time exceeded. To allow for more time '
+                              'adjust the max_minutes parameter.')
+            return False
+
+        if self.session.total_number_decisions >= self.parameters['max_selections']:
+            self.logger.debug('Max number of selections reached '
+                              '(configured with the max_selections parameter)')
+            return False
+
+        return True
+
+    def next_target(self) -> str:
+        """Computes the next target letter based on the currently spelled_text.
+        """
+        if self.copy_phrase[0:len(self.spelled_text)] == self.spelled_text:
+            # if correctly spelled so far, get the next letter.
+            return self.copy_phrase[len(self.spelled_text)]
+        return BACKSPACE_CHAR
+
+    def execute(self) -> str:
+        """Executes the task.
+
+        Returns
+        -------
+        data save location (triggers.txt, session.json)
+        """
+        self.logger.debug('Starting Copy Phrase Task!')
+        run = True
+        self.wait()  # buffer for data processing
+
+        while run and self.user_wants_to_continue() and self.current_inquiry:
+            target_stimuli = self.next_target()
+            stim_times, proceed = self.present_inquiry(
+                self.current_inquiry)
+
+            self.write_trigger_data(stim_times, target_stimuli)
+            self.wait()
+
+            evidence_types = self.add_evidence(stim_times, proceed)
+            decision = self.evaluate_evidence()
+
+            data = self.new_data_record(stim_times,
+                                        target_stimuli,
+                                        current_text=self.spelled_text,
+                                        decision=decision,
+                                        evidence_types=evidence_types)
+            self.update_session_data(data,
+                                     save=True,
+                                     decision_made=decision.decision_made)
+
+            if decision.decision_made:
+                self.show_feedback(decision.selection,
+                                   (decision.selection == target_stimuli))
+                self.spelled_text = decision.spelled_text
+                self.current_inquiry = self.next_inquiry()
+
+            else:
+                self.current_inquiry = decision.new_inq_schedule
+
+            run = self.check_stop_criteria()
+            self.inq_counter += 1
+
+        self.exit_display()
+        self.write_offset_trigger()
+
+        self.session.task_summary = TaskSummary(
+            self.session, self.parameters['show_preview_inquiry'],
+            self.parameters['preview_inquiry_progress_method'],
+            self.trigger_handler.file_path).as_dict()
+        self.write_session_data()
+
+        # Evidence is not recorded in the session when using fake decisions.
+        if self.parameters['summarize_session'] and self.session.has_evidence():
+            session_excel(session=self.session,
+                          excel_file=f"{self.file_save}/{SESSION_SUMMARY_FILENAME}")
+
+        # Wait some time before exiting so there is trailing eeg data saved
+        self.wait()
+
+        return self.file_save
+
+    def evaluate_evidence(self) -> Decision:
+        """Uses the `copy_phrase_task` parameter to evaluate the provided
+        evidence and attempt a decision.
+
+        Modifies
+        --------
+        - self.copy_phrase_task
+        """
+        if self.fake:
+            _, spelled, _ = fake_copy_phrase_decision(self.copy_phrase,
+                                                      self.next_target(),
+                                                      self.spelled_text)
+            # Reset the stoppage criteria by forcing the commit to a decision.
+            self.copy_phrase_task.decision_maker.do_series()
+            # In fake mode, only the LM is providing evidence, so the decision
+            # made is the highest symbol predicted. Override this state
+            self.copy_phrase_task.decision_maker.update(spelled)
+
+            # In fake mode, all inquiries result in a selection.
+            return Decision(decision_made=True,
+                            selection=spelled[-1],
+                            spelled_text=spelled,
+                            new_inq_schedule=None)
+
+        decision_made, new_sti = self.copy_phrase_task.decide()
+        spelled_text = self.copy_phrase_task.decision_maker.displayed_state
+        selection = ''
+        if decision_made:
+            selection = self.copy_phrase_task.decision_maker.last_selection
+
+        return Decision(decision_made, selection, spelled_text, new_sti)
+
+    def add_evidence(self, stim_times: List[List],
+                     proceed: bool = True) -> List[EvidenceType]:
+        """Add all evidence used to make a decision.
+
+        Parameters
+        ----------
+        - stim_times : list of stimuli returned from the display
+        - proceed : whether or not to proceed with the inquiry
+
+        Returns
+        -------
+        list of evidence types added
+
+        Modifies
+        --------
+        - self.copy_phrase_task
+        """
+        evidences = [
+            self.compute_button_press_evidence(proceed),
+            self.compute_eeg_evidence(stim_times, proceed)
+        ]
+        evidence_types = []
+        for evidence in evidences:
+            if evidence:
+                evidence_type, probs = evidence
+                evidence_types.append(evidence_type)
+                self.copy_phrase_task.add_evidence(evidence_type, probs)
+        if self.session.latest_series_is_empty():
+            evidence_types.append(EvidenceType.LM)
+        return evidence_types
+
+    def compute_button_press_evidence(
+            self, proceed: bool) -> Optional[Tuple[EvidenceType, List[float]]]:
+        """If 'show_preview_inquiry' feature is enabled, compute the button
+        press evidence and add it to the copy phrase task.
+
+        Parameters
+        ----------
+            proceed : whether to proceed with the inquiry after the preview
+
+        Returns
+        -------
+            tuple of (evidence type, evidence) or None if inquiry preview is
+            not enabled.
+        """
+        if not self.parameters['show_preview_inquiry'] \
+                or not self.current_inquiry \
+                or self.parameters['preview_only']:
+            return None
+        probs = compute_probs_after_preview(self.current_inquiry.stimuli[0],
+                                            self.alp,
+                                            self.button_press_error_prob,
+                                            proceed)
+        return (EvidenceType.BTN, probs)
+
+    def compute_eeg_evidence(self,
+                             stim_times: List[List],
+                             proceed: bool = True
+                             ) -> Optional[Tuple[EvidenceType, List[float]]]:
+        """Evaluate the EEG evidence and add it to the copy_phrase_task, but
+        don't yet attempt a decision.
+
+        Parameters
+        ----------
+        - stim_times : list of stimuli returned from the display
+        - proceed : whether or not to evaluate the evidence, if `False` returns
+        empty values.
+
+        Returns
+        -------
+        tuple of (evidence type, evidence)
+        """
+        if not proceed or self.fake:
+            return None
+
+        # currently prestim_length is used as a buffer for filter application, use the same at the end of the inquiry
+        post_stim_buffer = self.parameters['prestim_length']
+        raw_data, triggers = get_data_for_decision(
+            inquiry_timing=self.stims_for_decision(stim_times),
+            daq=self.daq,
+            offset=self.parameters['static_trigger_offset'],
+            prestim=self.parameters['prestim_length'],
+            poststim=post_stim_buffer + self.parameters['trial_length'])
+
+        # we assume all are nontargets at this point
+        labels = ['nontarget'] * len(triggers)
+
+        probs = self.copy_phrase_task.evaluate_eeg_evidence(
+            raw_data, triggers, labels, self.parameters['trial_length'])
+        return (EvidenceType.ERP, probs)
+
+    def stims_for_decision(self, stim_times: List[List]) -> List[List]:
+        """The stim_timings from the display may include non-letter stimuli
+        such as calibration and inquiry_preview timings. This method extracts
+        only the letter data used to process the data for a decision.
+
+        Parameters
+        ----------
+        - stim_times : list of [stim, clock_time] pairs returned from display.
+
+        Returns
+        -------
+        stim times where the stim is in the current alphabet; filters out
+        'calibration', 'inquiry_preview', etc.
+        """
+        return [
+            timing for timing in stim_times if timing[0] in (self.alp + ['+'])
+        ]
+
+    def new_data_record(self,
+                        stim_times: List[List],
+                        target_stimuli: str,
+                        current_text: str,
+                        decision: Decision,
+                        evidence_types: List[EvidenceType] = None) -> Inquiry:
+        """Construct a new inquiry data record.
+
+        Parameters
+        ----------
+        - stim_times : list of [stim, clock_time] pairs returned from display.
+        - target_stimuli : stim the user is currently attempting to spell.
+        - current_text : spelled text before the inquiry
+        - decision : decision made by the decision maker
+        - evidence_types : evidence provided to the decision-maker during the
+        current inquiry.
+
+        Returns
+        -------
+        Inquiry data for the current schedule; returned value only contains
+        evidence for the provided evidence_types, leaving the other types empty
+        """
+        assert self.current_inquiry, "Current inquiry is required"
+        evidence_types = evidence_types or []
+        triggers = construct_triggers(self.stims_for_decision(stim_times))
+        data = Inquiry(stimuli=self.current_inquiry.stimuli,
+                       timing=self.current_inquiry.durations,
+                       triggers=triggers,
+                       target_info=target_info(triggers, target_stimuli,
+                                               self.parameters['is_txt_stim']),
+                       target_letter=target_stimuli,
+                       current_text=current_text,
+                       target_text=self.copy_phrase,
+                       selection=decision.selection,
+                       next_display_state=decision.spelled_text)
+        data.precision = self.evidence_precision
+
+        if not self.fake:
+            latest_evidence = self.copy_phrase_task.conjugator.latest_evidence
+            data.evidences = {
+                ev_type: evidence if ev_type in evidence_types else []
+                for ev_type, evidence in latest_evidence.items()
+            }
+            data.likelihood = list(self.copy_phrase_task.conjugator.likelihood)
+        return data
+
+    def exit_display(self):
+        """Close the UI and cleanup."""
+        # Update task state and reset the static
+        self.rsvp.update_task_state(text=self.spelled_text,
+                                    color_list=['white'])
+        # Say Goodbye!
+        self.rsvp.info_text = trial_complete_message(self.window, self.parameters)
+        self.rsvp.draw_static()
+        self.window.flip()
+
+        # Give the system time to process
+        self.wait()
+
+    def update_session_data(self,
+                            data: Inquiry,
+                            save: bool = True,
+                            decision_made: bool = False) -> None:
+        """Update the current session with the latest inquiry data
+
+        Parameters
+        ----------
+        - data : inquiry to append to the session
+        - save : if True, persists the session to disk.
+
+        Modifies
+        --------
+        - self.session
+        """
+        self.session.add_sequence(data)
+        self.session.total_time_spent = self.experiment_clock.getTime() - self.start_time
+        if save:
+            self.write_session_data()
+        if decision_made:
+            self.session.add_series()
+
+    def write_session_data(self) -> None:
+        """Save session data to disk."""
+        if self.session:
+            session_file = _save_session_related_data(
+                self.session_save_location,
+                self.session.as_dict())
+            session_file.close()
+
+    def write_offset_trigger(self) -> None:
+        """Append the offset to the end of the triggers file.
+        """
+        if self.daq.is_calibrated:
+            self.trigger_handler.add_triggers(
+                [Trigger(
+                    'daq_sample_offset',
+                    TriggerType.SYSTEM,
+                    # to help support future refactoring or use of lsl timestamps only
+                    # we write only the sample offset here
+                    self.daq.offset(self.rsvp.first_stim_time)
+                )])
+        self.trigger_handler.close()
+
+    def write_trigger_data(self, stim_times: List[Tuple[str, float]], target_stimuli: str) -> None:
+        """Save trigger data to disk.
+
+        Parameters
+        ----------
+        - stim_times : list of (stim, clock_time) tuples
+        - target_stimuli : current target stimuli
+        """
+        if self.first_run and self.daq.is_calibrated:
+            # write offset first
+            self.trigger_handler.add_triggers(
+                [Trigger(
+                    'starting_offset',
+                    TriggerType.OFFSET,
+                    # offset will factor in true offset and time relative from beginning
+                    (self.daq.offset(self.rsvp.first_stim_time) - self.rsvp.first_stim_time)
+                )]
+            )
+
+        triggers = convert_timing_triggers(stim_times, target_stimuli, self.trigger_type)
+        self.trigger_handler.add_triggers(triggers)
+
+    def trigger_type(self, symbol: str, target: str, index: int) -> TriggerType:
+        """Trigger Type.
+
+        Cast a given symbol to a TriggerType.
+        """
+        if symbol == 'inquiry_preview':
+            return TriggerType.PREVIEW
+        if 'bcipy_key_press' in symbol:
+            return TriggerType.EVENT
+        if symbol == '+':
+            return TriggerType.FIXATION
+        if target == symbol:
+            return TriggerType.TARGET
+        return TriggerType.NONTARGET
+
+    def name(self) -> str:
+        return self.TASK_NAME
+
+    @property
+    def first_run(self) -> bool:
+        """First run.
+
+        Determines whether it is the first inquiry presentation / run.
+        """
+        return self.inq_counter == 0
+
+
+class TaskSummary:
+    """Summary data for tracking performance metrics.
+
+    Parameters
+    ----------
+        session - current session information
+        show_preview - whether or not inquiry preview was displayed
+        preview_mode - the switch mode for inquiry preview:
+            0 = preview only;
+            1 = press to confirm;
+            2 = press to skip to another inquiry
+    """
+
+    def __init__(self,
+                 session: Session,
+                 show_preview: bool = False,
+                 preview_mode: int = 0,
+                 trigger_path: str = None):
+        assert preview_mode in range(3), 'Preview mode out of range'
+        self.session = session
+        self.show_preview = show_preview
+        self.preview_mode = preview_mode
+        self.trigger_path = trigger_path
+        self.logger = logging.getLogger(__name__)
+
+    def as_dict(self) -> dict:
+        """Computes the task summary data to append to the session."""
+
+        selections = [
+            inq for inq in self.session.all_inquiries if inq.selection
+        ]
+        correct = [inq for inq in selections if inq.is_correct_decision]
+        incorrect = [inq for inq in selections if not inq.is_correct_decision]
+
+        # Note that SPACE is considered a symbol
+        correct_symbols = [
+            inq for inq in correct if inq.selection != BACKSPACE_CHAR
+        ]
+
+        btn_presses = self.btn_press_count()
+        sel_count = len(selections)
+        switch_per_selection = (btn_presses /
+                                sel_count) if sel_count > 0 else 0
+        accuracy = (len(correct) / sel_count) if sel_count > 0 else 0
+
+        # Note that minutes includes startup time and any breaks.
+        minutes = self.session.total_time_spent / 60
+        return {
+            'selections_correct': len(correct),
+            'selections_incorrect': len(incorrect),
+            'selections_correct_symbols': len(correct_symbols),
+            'switch_total': btn_presses,
+            'switch_per_selection': switch_per_selection,
+            'switch_response_time': self.switch_response_time(),
+            'typing_accuracy': accuracy,
+            'correct_rate': len(correct) / minutes if minutes else 0,
+            'copy_rate': len(correct_symbols) / minutes if minutes else 0
+        }
+
+    def btn_press_count(self) -> int:
+        """Compute the number of times the switch was activated. Returns 0 if
+        inquiry preview mode was off or mode was preview-only."""
+
+        if not self.show_preview or self.preview_mode == 0:
+            return 0
+
+        inquiries = self.session.all_inquiries
+        if self.preview_mode == 1:
+            # press to confirm
+            activations = [inq for inq in inquiries if inq.eeg_evidence]
+        elif self.preview_mode == 2:
+            # press to skip
+            activations = [inq for inq in inquiries if not inq.eeg_evidence]
+        return len(activations)
+
+    def switch_response_time(self) -> Optional[float]:
+        """Computes the average switch response in seconds."""
+
+        # Remove consecutive items with the same type; we are only interested
+        # in PREVIEW followed by a EVENT.
+        triggers = destutter(self.switch_triggers(), key=lambda trg: trg.type)
+        pairs = list(zip(triggers[::2], triggers[1::2]))
+
+        # Confirm that the data is structured as expected.
+        for preview, keypress in pairs:
+            if (preview.type != TriggerType.PREVIEW) or (
+                    keypress.type != TriggerType.EVENT):
+                self.logger.info('Could not compute switch_response_time')
+                return None
+
+        response_times = [
+            keypress.time - preview.time for preview, keypress in pairs
+        ]
+        count = len(response_times)
+        return sum(response_times) / count if count > 0 else None
+
+    def switch_triggers(self) -> List[Trigger]:
+        """Returns a list of switch-related triggers"""
+        if not self.trigger_path:
+            return []
+        triggers, _offset = TriggerHandler.read_text_file(self.trigger_path)
+        return [
+            trg for trg in triggers
+            if trg.type in [TriggerType.PREVIEW, TriggerType.EVENT]
+        ]
+
+
+def _init_copy_phrase_display(parameters, win, static_clock, experiment_clock, starting_spelled_text):
+    preview_inquiry = PreviewInquiryProperties(
+        preview_only=parameters['preview_only'],
+        preview_inquiry_length=parameters['preview_inquiry_length'],
+        preview_inquiry_key_input=parameters['preview_inquiry_key_input'],
+        preview_inquiry_progress_method=parameters[
+            'preview_inquiry_progress_method'],
+        preview_inquiry_isi=parameters['preview_inquiry_isi'])
+    info = InformationProperties(
+        info_color=[parameters['info_color']],
+        info_pos=[(parameters['info_pos_x'], parameters['info_pos_y'])],
+        info_height=[parameters['info_height']],
+        info_font=[parameters['font']],
+        info_text=[parameters['info_text']],
+    )
+    stimuli = StimuliProperties(stim_font=parameters['font'],
+                                stim_pos=(parameters['stim_pos_x'],
+                                          parameters['stim_pos_y']),
+                                stim_height=parameters['stim_height'],
+                                stim_inquiry=['A'] * parameters['stim_length'],
+                                stim_colors=[parameters['stim_color']] * parameters['stim_length'],
+                                stim_timing=[10] * parameters['stim_length'],
+                                is_txt_stim=parameters['is_txt_stim'])
+    padding = abs(len(parameters['task_text']) - len(starting_spelled_text))
+    starting_spelled_text += ' ' * padding
+    task_display = TaskDisplayProperties(task_color=[parameters['task_color']],
+                                         task_pos=(0, 1 - (2 * parameters['task_height'])),
+                                         task_font=parameters['font'],
+                                         task_height=parameters['task_height'],
+                                         task_text=starting_spelled_text)
+    return CopyPhraseDisplay(win,
+                             static_clock,
+                             experiment_clock,
+                             stimuli,
+                             task_display,
+                             info,
+                             static_task_text=parameters['task_text'],
+                             static_task_color=parameters['task_color'],
+                             trigger_type=parameters['trigger_type'],
+                             space_char=parameters['stim_space_char'],
+                             preview_inquiry=preview_inquiry)
+
+
+def _init_copy_phrase_wrapper(min_num_inq, max_num_inq, signal_model, fs, k,
+                              alp, evidence_names, task_list, lmodel,
+                              is_txt_stim, device_name, device_channels,
+                              stim_timing, decision_threshold,
+                              backspace_prob, backspace_always_shown,
+                              filter_high, filter_low, filter_order,
+                              notch_filter_frequency, stim_length, stim_jitter, stim_order):
+    return CopyPhraseWrapper(min_num_inq,
+                             max_num_inq,
+                             signal_model=signal_model,
+                             fs=fs,
+                             k=k,
+                             alp=alp,
+                             evidence_names=evidence_names,
+                             task_list=task_list,
+                             lmodel=lmodel,
+                             is_txt_stim=is_txt_stim,
+                             device_name=device_name,
+                             device_channels=device_channels,
+                             stim_timing=stim_timing,
+                             decision_threshold=decision_threshold,
+                             backspace_prob=backspace_prob,
+                             backspace_always_shown=backspace_always_shown,
+                             filter_high=filter_high,
+                             filter_low=filter_low,
+                             filter_order=filter_order,
+                             notch_filter_frequency=notch_filter_frequency,
+                             stim_length=stim_length,
+                             stim_jitter=stim_jitter,
+                             stim_order=stim_order)
```

### Comparing `bcipy-2.0.0rc3/bcipy/task/start_task.py` & `bcipy-2.0.1rc2/bcipy/task/start_task.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,62 @@
-"""Code for constructing and executing registered tasks"""
-from bcipy.task.paradigm.rsvp.calibration.calibration import RSVPCalibrationTask
-from bcipy.task.paradigm.rsvp.copy_phrase import RSVPCopyPhraseTask
-from bcipy.task.paradigm.rsvp.calibration.timing_verification import RSVPTimingVerificationCalibration
-
-from bcipy.task.paradigm.matrix.calibration import MatrixCalibrationTask
-from bcipy.task.paradigm.matrix.timing_verification import MatrixTimingVerificationCalibration
-from bcipy.task.paradigm.matrix.copy_phrase import MatrixCopyPhraseTask
-
-from bcipy.task import Task
-from bcipy.task.exceptions import TaskRegistryException
-from bcipy.task.task_registry import TaskType
-
-
-def make_task(display_window, daq, task, parameters, file_save,
-              signal_model=None, language_model=None, fake=True) -> Task:
-    """Creates a Task based on the provided parameters.
-
-    Parameters:
-    -----------
-        display_window: psychopy Window
-        daq: DataAcquisitionClient
-        task: TaskType
-        parameters: dict
-        file_save: str - path to file in which to save data
-        signal_model
-        language_model - language model
-        fake: boolean - true if eeg stream is randomly generated
-    Returns:
-    --------
-        Task instance
-    """
-
-    # NORMAL RSVP MODES
-    if task is TaskType.RSVP_CALIBRATION:
-        return RSVPCalibrationTask(
-            display_window, daq, parameters, file_save)
-
-    if task is TaskType.RSVP_COPY_PHRASE:
-        return RSVPCopyPhraseTask(
-            display_window, daq, parameters, file_save, signal_model,
-            language_model, fake=fake)
-
-    if task is TaskType.RSVP_TIMING_VERIFICATION_CALIBRATION:
-        return RSVPTimingVerificationCalibration(display_window, daq, parameters, file_save)
-
-    if task is TaskType.MATRIX_CALIBRATION:
-        return MatrixCalibrationTask(
-            display_window, daq, parameters, file_save
-        )
-
-    if task is TaskType.MATRIX_TIMING_VERIFICATION_CALIBRATION:
-        return MatrixTimingVerificationCalibration(display_window, daq, parameters, file_save)
-
-    if task is TaskType.MATRIX_COPY_PHRASE:
-        return MatrixCopyPhraseTask(
-            display_window, daq, parameters, file_save, signal_model,
-            language_model, fake=fake)
-    raise TaskRegistryException(
-        'The provided experiment type is not registered.')
-
-
-def start_task(display_window, daq, task, parameters, file_save,
-               signal_model=None, language_model=None, fake=True):
-    """Creates a Task and starts execution."""
-    task = make_task(display_window, daq, task, parameters, file_save,
-                     signal_model, language_model, fake)
-    task.execute()
+"""Code for constructing and executing registered tasks"""
+from bcipy.task.paradigm.rsvp.calibration.calibration import RSVPCalibrationTask
+from bcipy.task.paradigm.rsvp.copy_phrase import RSVPCopyPhraseTask
+from bcipy.task.paradigm.rsvp.calibration.timing_verification import RSVPTimingVerificationCalibration
+
+from bcipy.task.paradigm.matrix.calibration import MatrixCalibrationTask
+from bcipy.task.paradigm.matrix.timing_verification import MatrixTimingVerificationCalibration
+
+from bcipy.task import Task
+from bcipy.task.exceptions import TaskRegistryException
+from bcipy.task.task_registry import TaskType
+
+
+def make_task(display_window, daq, task, parameters, file_save,
+              signal_model=None, language_model=None, fake=True) -> Task:
+    """Creates a Task based on the provided parameters.
+
+    Parameters:
+    -----------
+        display_window: psychopy Window
+        daq: DataAcquisitionClient
+        task: TaskType
+        parameters: dict
+        file_save: str - path to file in which to save data
+        signal_model
+        language_model - language model
+        fake: boolean - true if eeg stream is randomly generated
+    Returns:
+    --------
+        Task instance
+    """
+
+    # NORMAL RSVP MODES
+    if task is TaskType.RSVP_CALIBRATION:
+        return RSVPCalibrationTask(
+            display_window, daq, parameters, file_save)
+
+    if task is TaskType.RSVP_COPY_PHRASE:
+        return RSVPCopyPhraseTask(
+            display_window, daq, parameters, file_save, signal_model,
+            language_model, fake=fake)
+
+    if task is TaskType.RSVP_TIMING_VERIFICATION_CALIBRATION:
+        return RSVPTimingVerificationCalibration(display_window, daq, parameters, file_save)
+
+    if task is TaskType.MATRIX_CALIBRATION:
+        return MatrixCalibrationTask(
+            display_window, daq, parameters, file_save
+        )
+
+    if task is TaskType.MATRIX_TIMING_VERIFICATION_CALIBRATION:
+        return MatrixTimingVerificationCalibration(display_window, daq, parameters, file_save)
+    raise TaskRegistryException(
+        'The provided experiment type is not registered.')
+
+
+def start_task(display_window, daq, task, parameters, file_save,
+               signal_model=None, language_model=None, fake=True):
+    """Creates a Task and starts execution."""
+    task = make_task(display_window, daq, task, parameters, file_save,
+                     signal_model, language_model, fake)
+    task.execute()
```

### Comparing `bcipy-2.0.0rc3/bcipy/task/task_registry.py` & `bcipy-2.0.1rc2/bcipy/task/task_registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,68 @@
-"""Task Registry ; used to provide task options to the GUI and command line
-tools. User defined tasks can be added to the Registry."""
-
-
-# NOTE:
-# In the future we may want to consider dynamically retrieving all subclasses
-# of Task and use these to populate a registry. We could also provide
-# functionality for bcipy users to define their own tasks and register them so
-# they would appear as options in the GUI.
-#
-# However, this approach is currently problematic for the GUI interface. Due
-# to the tight coupling of the display code with the Tasks, importing any of
-# the Task subclasses causes pygame (a psychopy dependency) to create a GUI,
-# which seems to prevent our other GUI code from working.
-
-from enum import Enum
-from typing import List
-
-from bcipy.helpers.exceptions import BciPyCoreException
-
-
-class TaskType(Enum):
-    """Enum of the registered experiment types (Tasks), along with the label
-    used for display in the GUI and command line tools. Values are looked up
-    by their (1-based) index.
-
-    Examples:
-    >>> TaskType(1)
-    <TaskType.RSVP_CALIBRATION: 1>
-
-    >>> TaskType(1).label
-    'RSVP Calibration'
-    """
-
-    RSVP_CALIBRATION = 'RSVP Calibration'
-    RSVP_COPY_PHRASE = 'RSVP Copy Phrase'
-    RSVP_TIMING_VERIFICATION_CALIBRATION = 'RSVP Time Test Calibration'
-    MATRIX_CALIBRATION = 'Matrix Calibration'
-    MATRIX_TIMING_VERIFICATION_CALIBRATION = 'Matrix Time Test Calibration'
-    MATRIX_COPY_PHRASE = 'Matrix Copy Phrase'
-
-    def __new__(cls, *args, **kwds):
-        """Autoincrements the value of each item added to the enum."""
-        value = len(cls.__members__) + 1
-        obj = object.__new__(cls)
-        obj._value_ = value
-        return obj
-
-    def __init__(self, label):
-        self.label = label
-
-    @classmethod
-    def by_value(cls, item):
-        tasks = cls.list()
-        # The cls.list method returns a sorted list of enum tasks
-        # check if item present and return the index + 1 (which is the ENUM value for the task)
-        if item in tasks:
-            return cls(tasks.index(item) + 1)
-        raise BciPyCoreException(f'{item} not a registered TaskType={tasks}')
-
-    @classmethod
-    def calibration_tasks(cls) -> List['TaskType']:
-        return [task for task in cls
-                if task.name.endswith('CALIBRATION') and 'COPY_PHRASE'
-                not in task.name]
-
-    @classmethod
-    def list(cls) -> List[str]:
-        return list(map(lambda c: c.label, cls))
+"""Task Registry ; used to provide task options to the GUI and command line
+tools. User defined tasks can be added to the Registry."""
+
+
+# NOTE:
+# In the future we may want to consider dynamically retrieving all subclasses
+# of Task and use these to populate a registry. We could also provide
+# functionality for bcipy users to define their own tasks and register them so
+# they would appear as options in the GUI.
+#
+# However, this approach is currently problematic for the GUI interface. Due
+# to the tight coupling of the display code with the Tasks, importing any of
+# the Task subclasses causes pygame (a psychopy dependency) to create a GUI,
+# which seems to prevent our other GUI code from working.
+
+from enum import Enum
+from typing import List
+
+from bcipy.helpers.exceptions import BciPyCoreException
+
+
+class TaskType(Enum):
+    """Enum of the registered experiment types (Tasks), along with the label
+    used for display in the GUI and command line tools. Values are looked up
+    by their (1-based) index.
+
+    Examples:
+    >>> TaskType(1)
+    <TaskType.RSVP_CALIBRATION: 1>
+
+    >>> TaskType(1).label
+    'RSVP Calibration'
+    """
+
+    RSVP_CALIBRATION = 'RSVP Calibration'
+    RSVP_COPY_PHRASE = 'RSVP Copy Phrase'
+    RSVP_TIMING_VERIFICATION_CALIBRATION = 'RSVP Time Test Calibration'
+    MATRIX_CALIBRATION = 'Matrix Calibration'
+    MATRIX_TIMING_VERIFICATION_CALIBRATION = 'Matrix Time Test Calibration'
+
+    def __new__(cls, *args, **kwds):
+        """Autoincrements the value of each item added to the enum."""
+        value = len(cls.__members__) + 1
+        obj = object.__new__(cls)
+        obj._value_ = value
+        return obj
+
+    def __init__(self, label):
+        self.label = label
+
+    @classmethod
+    def by_value(cls, item):
+        tasks = cls.list()
+        # The cls.list method returns a sorted list of enum tasks
+        # check if item present and return the index + 1 (which is the ENUM value for the task)
+        if item in tasks:
+            return cls(tasks.index(item) + 1)
+        raise BciPyCoreException(f'{item} not a registered TaskType={tasks}')
+
+    @classmethod
+    def calibration_tasks(cls) -> List['TaskType']:
+        return [task for task in cls
+                if task.name.endswith('CALIBRATION') and 'COPY_PHRASE'
+                not in task.name]
+
+    @classmethod
+    def list(cls) -> List[str]:
+        return list(map(lambda c: c.label, cls))
```

### Comparing `bcipy-2.0.0rc3/bcipy.egg-info/PKG-INFO` & `bcipy-2.0.1rc2/bcipy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bcipy
-Version: 2.0.0rc3
+Version: 2.0.1rc2
 Summary: Python Software for Brain-Computer Interface.
 Home-page: https://github.com/CAMBI-tech/BciPy
 Author: CAMBI
 Author-email: cambi_support@googlegroups.com
 License: Hippocratic License 2.1
 Description: Python Brain-Computer Interface Software
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >3.7,<3.10
+Requires-Python: >3.6,<3.9
 Description-Content-Type: text/markdown
```

### Comparing `bcipy-2.0.0rc3/bcipy.egg-info/SOURCES.txt` & `bcipy-2.0.1rc2/bcipy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 LICENSE.md
 README.md
 setup.cfg
 setup.py
 bcipy/__init__.py
 bcipy/config.py
 bcipy/main.py
-bcipy/preferences.py
 bcipy.egg-info/PKG-INFO
 bcipy.egg-info/SOURCES.txt
 bcipy.egg-info/dependency_links.txt
 bcipy.egg-info/entry_points.txt
 bcipy.egg-info/requires.txt
 bcipy.egg-info/top_level.txt
 bcipy/acquisition/__init__.py
 bcipy/acquisition/devices.py
 bcipy/acquisition/exceptions.py
 bcipy/acquisition/marker_writer.py
-bcipy/acquisition/multimodal.py
 bcipy/acquisition/record.py
 bcipy/acquisition/util.py
 bcipy/acquisition/datastream/__init__.py
 bcipy/acquisition/datastream/generator.py
 bcipy/acquisition/datastream/lsl_server.py
 bcipy/acquisition/datastream/producer.py
 bcipy/acquisition/datastream/mock/__init__.py
@@ -32,14 +30,16 @@
 bcipy/acquisition/protocols/lsl/lsl_connector.py
 bcipy/acquisition/protocols/lsl/lsl_recorder.py
 bcipy/display/__init__.py
 bcipy/display/main.py
 bcipy/display/paradigm/__init__.py
 bcipy/display/paradigm/matrix/__init__.py
 bcipy/display/paradigm/matrix/display.py
+bcipy/display/paradigm/matrix/mode/__init__.py
+bcipy/display/paradigm/matrix/mode/calibration.py
 bcipy/display/paradigm/rsvp/__init__.py
 bcipy/display/paradigm/rsvp/display.py
 bcipy/display/paradigm/rsvp/mode/__init__.py
 bcipy/display/paradigm/rsvp/mode/calibration.py
 bcipy/display/paradigm/rsvp/mode/copy_phrase.py
 bcipy/display/paradigm/vep/__init__.py
 bcipy/display/paradigm/vep/display.py
@@ -76,15 +76,14 @@
 bcipy/helpers/list.py
 bcipy/helpers/load.py
 bcipy/helpers/parameters.py
 bcipy/helpers/raw_data.py
 bcipy/helpers/save.py
 bcipy/helpers/session.py
 bcipy/helpers/stimuli.py
-bcipy/helpers/symbols.py
 bcipy/helpers/system_utils.py
 bcipy/helpers/task.py
 bcipy/helpers/triggers.py
 bcipy/helpers/validate.py
 bcipy/helpers/visualization.py
 bcipy/helpers/tests/__init__.py
 bcipy/helpers/tests/test_acquisition.py
@@ -95,61 +94,52 @@
 bcipy/helpers/tests/test_list.py
 bcipy/helpers/tests/test_load.py
 bcipy/helpers/tests/test_parameters.py
 bcipy/helpers/tests/test_raw_data.py
 bcipy/helpers/tests/test_save.py
 bcipy/helpers/tests/test_session.py
 bcipy/helpers/tests/test_stimuli.py
-bcipy/helpers/tests/test_symbols.py
-bcipy/helpers/tests/test_system_utils.py
 bcipy/helpers/tests/test_task.py
 bcipy/helpers/tests/test_triggers.py
 bcipy/helpers/tests/test_validate.py
-bcipy/helpers/tests/test_visualization.py
-bcipy/language/__init__.py
-bcipy/language/main.py
-bcipy/parameters/__init__.py
 bcipy/signal/__init__.py
+bcipy/signal/exceptions.py
 bcipy/signal/evaluate/__init__.py
 bcipy/signal/evaluate/evaluator.py
 bcipy/signal/evaluate/rules.py
 bcipy/signal/generator/__init__.py
 bcipy/signal/generator/generator.py
 bcipy/signal/model/__init__.py
 bcipy/signal/model/base_model.py
-bcipy/signal/model/classifier.py
-bcipy/signal/model/cross_validation.py
-bcipy/signal/model/density_estimation.py
-bcipy/signal/model/dimensionality_reduction.py
 bcipy/signal/model/inquiry_preview.py
 bcipy/signal/model/offline_analysis.py
-bcipy/signal/model/pipeline.py
 bcipy/signal/model/pca_rda_kde/__init__.py
+bcipy/signal/model/pca_rda_kde/classifier.py
+bcipy/signal/model/pca_rda_kde/cross_validation.py
+bcipy/signal/model/pca_rda_kde/density_estimation.py
+bcipy/signal/model/pca_rda_kde/dimensionality_reduction.py
 bcipy/signal/model/pca_rda_kde/pca_rda_kde.py
-bcipy/signal/model/rda_kde/__init__.py
-bcipy/signal/model/rda_kde/rda_kde.py
+bcipy/signal/model/pca_rda_kde/pipeline.py
 bcipy/signal/process/__init__.py
 bcipy/signal/process/filter.py
 bcipy/signal/process/transform.py
 bcipy/signal/process/decomposition/__init__.py
-bcipy/signal/process/decomposition/cwt.py
 bcipy/signal/process/decomposition/psd.py
 bcipy/task/__init__.py
 bcipy/task/data.py
 bcipy/task/exceptions.py
 bcipy/task/main.py
 bcipy/task/start_task.py
 bcipy/task/task_registry.py
 bcipy/task/control/__init__.py
 bcipy/task/control/criteria.py
 bcipy/task/control/handler.py
 bcipy/task/control/query.py
 bcipy/task/paradigm/__init__.py
 bcipy/task/paradigm/matrix/__init__.py
 bcipy/task/paradigm/matrix/calibration.py
-bcipy/task/paradigm/matrix/copy_phrase.py
 bcipy/task/paradigm/matrix/timing_verification.py
 bcipy/task/paradigm/rsvp/__init__.py
 bcipy/task/paradigm/rsvp/copy_phrase.py
 bcipy/task/paradigm/rsvp/calibration/__init__.py
 bcipy/task/paradigm/rsvp/calibration/calibration.py
 bcipy/task/paradigm/rsvp/calibration/timing_verification.py
```

### Comparing `bcipy-2.0.0rc3/setup.py` & `bcipy-2.0.1rc2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,43 @@
+# Modified from https://github.com/kennethreitz/setup.py
 import os
 import sys
-import platform
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = 'bcipy'
 DESCRIPTION = 'Python Software for Brain-Computer Interface.'
 URL = 'https://github.com/CAMBI-tech/BciPy'
 EMAIL = 'cambi_support@googlegroups.com'
 AUTHOR = 'CAMBI'
-REQUIRES_PYTHON = '>3.7,<3.10'
+REQUIRES_PYTHON = '>3.6,<3.9'
 
-VERSION = '2.0.0rc3'
+VERSION = '2.0.1rc2'
 
-REQUIRED = []
 
 # What packages are required for this module to be executed?
-if platform.system() == 'Windows' or platform.system() == 'Darwin':
-    with open('requirements-winmac.txt', 'r', encoding='utf-8') as f:
-        REQUIRED += f.read().splitlines()
 with open('requirements.txt', 'r', encoding='utf-8') as f:
-    REQUIRED += f.read().splitlines()
+    REQUIRED = f.read().splitlines()
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 long_description = 'Python Brain-Computer Interface Software'
 
 about = {'__version__': VERSION}
 
 
 class UploadCommand(Command):
-    """Support setup.py upload.
-    
-    Modified from https://github.com/kennethreitz/setup.py
-    """
+    """Support setup.py upload."""
 
     description = 'Build and publish the package.'
     user_options = []
 
     @staticmethod
     def status(s):
         """Prints things in bold."""
@@ -99,15 +92,15 @@
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: Other/Proprietary License',
         'Topic :: Scientific/Engineering :: Human Machine Interfaces',
         'Intended Audience :: Science/Research',
         'Intended Audience :: End Users/Desktop',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
+        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
 )
```

