# Comparing `tmp/ooo_dev_tools-0.9.6.tar.gz` & `tmp/ooo_dev_tools-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooo_dev_tools-0.9.6.tar", max compression
+gzip compressed data, was "ooo_dev_tools-0.9.7.tar", max compression
```

## Comparing `ooo_dev_tools-0.9.6.tar` & `ooo_dev_tools-0.9.7.tar`

### file list

```diff
@@ -1,985 +1,985 @@
--rw-r--r--   0        0        0    10174 2022-06-09 05:52:04.135315 ooo_dev_tools-0.9.6/LICENSE
--rw-r--r--   0        0        0      272 2023-04-25 00:03:57.141368 ooo_dev_tools-0.9.6/ooodev/__init__.py
--rw-r--r--   0        0        0        0 2022-11-29 00:27:48.235332 ooo_dev_tools-0.9.6/ooodev/adapter/__init__.py
--rw-r--r--   0        0        0     1806 2022-11-29 00:27:48.236329 ooo_dev_tools-0.9.6/ooodev/adapter/adapter_base.py
--rw-r--r--   0        0        0        0 2022-11-29 00:27:48.236329 ooo_dev_tools-0.9.6/ooodev/adapter/awt/__init__.py
--rw-r--r--   0        0        0     3451 2022-12-03 04:37:37.329802 ooo_dev_tools-0.9.6/ooodev/adapter/awt/top_window_listener.py
--rw-r--r--   0        0        0        0 2022-11-29 00:27:48.238329 ooo_dev_tools-0.9.6/ooodev/adapter/frame/__init__.py
--rw-r--r--   0        0        0     2711 2022-12-03 04:37:37.330805 ooo_dev_tools-0.9.6/ooodev/adapter/frame/terminate_listener.py
--rw-r--r--   0        0        0        0 2022-11-29 00:27:48.239328 ooo_dev_tools-0.9.6/ooodev/adapter/lang/__init__.py
--rw-r--r--   0        0        0     1543 2022-12-03 04:37:37.330805 ooo_dev_tools-0.9.6/ooodev/adapter/lang/event_listener.py
--rw-r--r--   0        0        0        0 2022-11-29 00:27:48.240329 ooo_dev_tools-0.9.6/ooodev/adapter/util/__init__.py
--rw-r--r--   0        0        0     2336 2022-12-03 04:37:37.331804 ooo_dev_tools-0.9.6/ooodev/adapter/util/modify_listener.py
--rw-r--r--   0        0        0        0 2022-11-29 00:27:48.241329 ooo_dev_tools-0.9.6/ooodev/adapter/view/__init__.py
--rw-r--r--   0        0        0     2628 2023-04-06 02:13:08.626094 ooo_dev_tools-0.9.6/ooodev/adapter/view/selection_change_listener.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.785323 ooo_dev_tools-0.9.6/ooodev/cfg/__init__.py
--rw-r--r--   0        0        0       89 2022-10-27 15:27:12.042995 ooo_dev_tools-0.9.6/ooodev/cfg/config.json
--rw-r--r--   0        0        0     2012 2022-10-27 15:27:12.042995 ooo_dev_tools-0.9.6/ooodev/cfg/config.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.786382 ooo_dev_tools-0.9.6/ooodev/conn/__init__.py
--rw-r--r--   0        0        0     5699 2022-07-14 20:40:23.787320 ooo_dev_tools-0.9.6/ooodev/conn/cache.py
--rw-r--r--   0        0        0    18466 2023-04-06 02:13:08.627093 ooo_dev_tools-0.9.6/ooodev/conn/connect.py
--rw-r--r--   0        0        0     6968 2022-12-20 23:59:58.431481 ooo_dev_tools-0.9.6/ooodev/conn/connectors.py
--rw-r--r--   0        0        0        0 2022-10-27 15:27:12.043993 ooo_dev_tools-0.9.6/ooodev/dialog/__init__.py
--rw-r--r--   0        0        0     3161 2022-11-05 19:29:24.377395 ooo_dev_tools-0.9.6/ooodev/dialog/input.py
--rw-r--r--   0        0        0     2297 2022-11-13 02:25:58.183785 ooo_dev_tools-0.9.6/ooodev/dialog/msgbox.py
--rw-r--r--   0        0        0     2019 2022-10-27 15:27:12.045993 ooo_dev_tools-0.9.6/ooodev/dialog/tk_input.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.789060 ooo_dev_tools-0.9.6/ooodev/events/__init__.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.789342 ooo_dev_tools-0.9.6/ooodev/events/args/__init__.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.789342 ooo_dev_tools-0.9.6/ooodev/events/args/calc/__init__.py
--rw-r--r--   0        0        0     1371 2023-04-02 18:09:12.324621 ooo_dev_tools-0.9.6/ooodev/events/args/calc/cell_args.py
--rw-r--r--   0        0        0     1461 2023-04-02 18:09:12.325621 ooo_dev_tools-0.9.6/ooodev/events/args/calc/cell_cancel_args.py
--rw-r--r--   0        0        0     1590 2023-04-02 18:09:12.326621 ooo_dev_tools-0.9.6/ooodev/events/args/calc/sheet_args.py
--rw-r--r--   0        0        0     1575 2023-04-02 18:09:12.327740 ooo_dev_tools-0.9.6/ooodev/events/args/calc/sheet_cancel_args.py
--rw-r--r--   0        0        0     1451 2023-04-02 18:09:12.328623 ooo_dev_tools-0.9.6/ooodev/events/args/cancel_event_args.py
--rw-r--r--   0        0        0     1163 2023-04-02 18:09:12.328745 ooo_dev_tools-0.9.6/ooodev/events/args/dispatch_args.py
--rw-r--r--   0        0        0     1450 2023-04-02 18:09:12.329620 ooo_dev_tools-0.9.6/ooodev/events/args/dispatch_cancel_args.py
--rw-r--r--   0        0        0     4051 2023-04-06 02:13:08.628097 ooo_dev_tools-0.9.6/ooodev/events/args/event_args.py
--rw-r--r--   0        0        0      640 2022-11-29 00:27:48.243330 ooo_dev_tools-0.9.6/ooodev/events/args/generic_args.py
--rw-r--r--   0        0        0     1366 2023-04-02 18:09:12.330620 ooo_dev_tools-0.9.6/ooodev/events/args/key_val_args.py
--rw-r--r--   0        0        0     1608 2023-04-02 18:09:12.331622 ooo_dev_tools-0.9.6/ooodev/events/args/key_val_cancel_args.py
--rw-r--r--   0        0        0     5995 2023-04-02 18:09:12.332622 ooo_dev_tools-0.9.6/ooodev/events/calc_named_event.py
--rw-r--r--   0        0        0      863 2023-04-23 13:05:05.528317 ooo_dev_tools-0.9.6/ooodev/events/chart2_named_event.py
--rw-r--r--   0        0        0      391 2022-11-29 00:27:48.244327 ooo_dev_tools-0.9.6/ooodev/events/command.py
--rw-r--r--   0        0        0      312 2023-04-02 18:09:12.332622 ooo_dev_tools-0.9.6/ooodev/events/draw_named_event.py
--rw-r--r--   0        0        0     4247 2023-04-02 18:09:12.333621 ooo_dev_tools-0.9.6/ooodev/events/event_singleton.py
--rw-r--r--   0        0        0     3816 2023-04-23 13:05:05.537315 ooo_dev_tools-0.9.6/ooodev/events/format_named_event.py
--rw-r--r--   0        0        0      210 2023-04-02 18:09:12.334621 ooo_dev_tools-0.9.6/ooodev/events/gbl_named_event.py
--rw-r--r--   0        0        0     9544 2023-04-02 18:09:12.335620 ooo_dev_tools-0.9.6/ooodev/events/lo_events.py
--rw-r--r--   0        0        0     3082 2023-04-02 18:09:12.336620 ooo_dev_tools-0.9.6/ooodev/events/lo_named_event.py
--rw-r--r--   0        0        0     1022 2023-04-23 13:05:05.538318 ooo_dev_tools-0.9.6/ooodev/events/props_named_event.py
--rw-r--r--   0        0        0     5175 2023-04-02 18:09:12.337911 ooo_dev_tools-0.9.6/ooodev/events/write_named_event.py
--rw-r--r--   0        0        0        0 2022-06-09 05:52:04.175567 ooo_dev_tools-0.9.6/ooodev/exceptions/__init__.py
--rw-r--r--   0        0        0     9928 2023-04-06 02:13:08.630095 ooo_dev_tools-0.9.6/ooodev/exceptions/ex.py
--rw-r--r--   0        0        0      160 2023-04-06 02:13:08.630095 ooo_dev_tools-0.9.6/ooodev/format/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.339621 ooo_dev_tools-0.9.6/ooodev/format/calc/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.339621 ooo_dev_tools-0.9.6/ooodev/format/calc/direct/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.631093 ooo_dev_tools-0.9.6/ooodev/format/calc/direct/cell/__init__.py
--rw-r--r--   0        0        0      812 2023-04-06 02:13:48.174066 ooo_dev_tools-0.9.6/ooodev/format/calc/direct/cell/alignment/__init__.py
--rw-r--r--   0        0        0      108 2023-04-06 02:13:08.632095 ooo_dev_tools-0.9.6/ooodev/format/calc/direct/cell/background/__init__.py
--rw-r--r--   0        0        0      782 2023-04-07 18:06:32.190987 ooo_dev_tools-0.9.6/ooodev/format/calc/direct/cell/borders/__init__.py
--rw-r--r--   0        0        0      139 2023-04-06 02:13:08.633094 ooo_dev_tools-0.9.6/ooodev/format/calc/direct/cell/cell_protection/__init__.py
--rw-r--r--   0        0        0     1376 2023-04-23 13:05:05.539317 ooo_dev_tools-0.9.6/ooodev/format/calc/direct/cell/font/__init__.py
--rw-r--r--   0        0        0      281 2023-04-23 13:05:05.540318 ooo_dev_tools-0.9.6/ooodev/format/calc/direct/cell/numbers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.634096 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.634096 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/cell/__init__.py
--rw-r--r--   0        0        0     1376 2023-04-06 02:13:08.635093 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/cell/alignment/__init__.py
--rw-r--r--   0        0        0      291 2023-04-06 02:13:08.635093 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/cell/background/__init__.py
--rw-r--r--   0        0        0      852 2023-04-07 18:06:32.191986 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/cell/borders/__init__.py
--rw-r--r--   0        0        0      375 2023-04-06 02:13:08.636101 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/cell/cell_protection/__init__.py
--rw-r--r--   0        0        0     1245 2023-04-06 02:13:08.637094 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/cell/font/__init__.py
--rw-r--r--   0        0        0      530 2023-04-23 13:05:05.542331 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/cell/numbers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.637094 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/__init__.py
--rw-r--r--   0        0        0     1123 2023-04-06 02:13:08.638093 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/area/__init__.py
--rw-r--r--   0        0        0     1019 2023-04-06 02:13:08.638093 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/borders/__init__.py
--rw-r--r--   0        0        0      276 2023-04-06 02:13:08.639095 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/footer/__init__.py
--rw-r--r--   0        0        0     1100 2023-04-06 02:13:08.639095 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/footer/area/__init__.py
--rw-r--r--   0        0        0     1005 2023-04-06 02:13:08.640095 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/footer/borders/__init__.py
--rw-r--r--   0        0        0      290 2023-04-06 02:13:08.640095 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/header/__init__.py
--rw-r--r--   0        0        0     1235 2023-04-06 02:13:08.641104 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/header/area/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-06 02:13:08.641104 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/header/borders/__init__.py
--rw-r--r--   0        0        0     1162 2023-04-06 02:13:08.642093 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/page/__init__.py
--rw-r--r--   0        0        0      708 2023-04-06 02:13:08.642093 ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/sheet/__init__.py
--rw-r--r--   0        0        0      254 2023-04-06 02:13:48.198066 ooo_dev_tools-0.9.6/ooodev/format/calc/style/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.643095 ooo_dev_tools-0.9.6/ooodev/format/calc/style/cell/__init__.py
--rw-r--r--   0        0        0     4313 2023-04-06 02:13:48.198066 ooo_dev_tools-0.9.6/ooodev/format/calc/style/cell/cell.py
--rw-r--r--   0        0        0       60 2023-04-06 02:13:08.644094 ooo_dev_tools-0.9.6/ooodev/format/calc/style/cell/kind/__init__.py
--rw-r--r--   0        0        0      588 2023-04-06 02:13:08.645093 ooo_dev_tools-0.9.6/ooodev/format/calc/style/cell/kind/style_cell_kind.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.645093 ooo_dev_tools-0.9.6/ooodev/format/calc/style/page/__init__.py
--rw-r--r--   0        0        0       73 2023-04-06 02:13:08.645093 ooo_dev_tools-0.9.6/ooodev/format/calc/style/page/kind/__init__.py
--rw-r--r--   0        0        0      207 2023-04-06 02:13:08.646094 ooo_dev_tools-0.9.6/ooodev/format/calc/style/page/kind/calc_style_page_kind.py
--rw-r--r--   0        0        0     4101 2023-04-06 02:13:48.199068 ooo_dev_tools-0.9.6/ooodev/format/calc/style/page/page.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.542331 ooo_dev_tools-0.9.6/ooodev/format/chart2/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.543317 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.543317 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/axis/__init__.py
--rw-r--r--   0        0        0     1096 2023-04-23 13:05:05.544315 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/axis/font/__init__.py
--rw-r--r--   0        0        0      683 2023-04-23 13:05:05.545317 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/axis/label/__init__.py
--rw-r--r--   0        0        0      305 2023-04-23 13:05:05.546314 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/axis/line/__init__.py
--rw-r--r--   0        0        0      338 2023-04-23 13:05:05.547315 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/axis/numbers/__init__.py
--rw-r--r--   0        0        0      887 2023-04-23 13:05:05.548318 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/axis/positioning/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.548318 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/general/__init__.py
--rw-r--r--   0        0        0     1809 2023-04-23 13:05:05.549318 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/general/area/__init__.py
--rw-r--r--   0        0        0      309 2023-04-23 13:05:05.550320 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/general/borders/__init__.py
--rw-r--r--   0        0        0      339 2023-04-23 13:05:05.550320 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/general/numbers/__init__.py
--rw-r--r--   0        0        0      212 2023-04-23 13:05:05.551317 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/general/position_size/__init__.py
--rw-r--r--   0        0        0      519 2023-04-23 13:05:05.552317 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/general/transparency/__init__.py
--rw-r--r--   0        0        0      309 2023-04-23 13:05:05.553316 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/grid/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.553316 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/legend/__init__.py
--rw-r--r--   0        0        0     1812 2023-04-23 13:05:05.554315 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/legend/area/__init__.py
--rw-r--r--   0        0        0      310 2023-04-23 13:05:05.555318 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/legend/borders/__init__.py
--rw-r--r--   0        0        0     1280 2023-04-23 13:05:05.556318 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/legend/font/__init__.py
--rw-r--r--   0        0        0      314 2023-04-23 13:05:05.557317 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/legend/position_size/__init__.py
--rw-r--r--   0        0        0      521 2023-04-23 13:05:05.558318 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/legend/transparency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.558318 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.559327 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_labels/__init__.py
--rw-r--r--   0        0        0      331 2023-04-23 13:05:05.560319 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_labels/borders/__init__.py
--rw-r--r--   0        0        0     1314 2023-04-23 13:05:05.561318 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_labels/data_labels/__init__.py
--rw-r--r--   0        0        0     1124 2023-04-23 13:05:05.562318 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_labels/font/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.563317 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_series/__init__.py
--rw-r--r--   0        0        0     1874 2023-04-23 13:05:05.564315 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_series/area/__init__.py
--rw-r--r--   0        0        0      331 2023-04-23 13:05:05.564315 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_series/borders/__init__.py
--rw-r--r--   0        0        0     1085 2023-04-23 13:05:05.566315 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_series/options/__init__.py
--rw-r--r--   0        0        0      545 2023-04-23 13:05:05.568318 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_series/transparency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.569317 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/title/__init__.py
--rw-r--r--   0        0        0      357 2023-04-23 13:05:05.608317 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/title/alignment/__init__.py
--rw-r--r--   0        0        0     1807 2023-04-23 13:05:05.651316 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/title/area/__init__.py
--rw-r--r--   0        0        0      309 2023-04-23 13:05:05.652314 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/title/borders/__init__.py
--rw-r--r--   0        0        0     1277 2023-04-23 13:05:05.653316 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/title/font/__init__.py
--rw-r--r--   0        0        0      132 2023-04-23 13:05:05.654316 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/title/position_size/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.654316 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/wall/__init__.py
--rw-r--r--   0        0        0     1804 2023-04-23 13:05:05.655315 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/wall/area/__init__.py
--rw-r--r--   0        0        0      308 2023-04-23 13:05:05.656316 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/wall/borders/__init__.py
--rw-r--r--   0        0        0      517 2023-04-23 13:05:05.657316 ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/wall/transparency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.403612 ooo_dev_tools-0.9.6/ooodev/format/draw/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.404613 ooo_dev_tools-0.9.6/ooodev/format/draw/direct/__init__.py
--rw-r--r--   0        0        0     1401 2023-04-23 13:05:05.659315 ooo_dev_tools-0.9.6/ooodev/format/draw/direct/area/__init__.py
--rw-r--r--   0        0        0      641 2023-04-06 02:13:08.648096 ooo_dev_tools-0.9.6/ooodev/format/draw/direct/transparency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.405614 ooo_dev_tools-0.9.6/ooodev/format/draw/modify/__init__.py
--rw-r--r--   0        0        0      945 2023-04-06 02:13:08.675095 ooo_dev_tools-0.9.6/ooodev/format/draw/modify/area/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.406613 ooo_dev_tools-0.9.6/ooodev/format/draw/style/__init__.py
--rw-r--r--   0        0        0      277 2023-04-02 18:09:12.406613 ooo_dev_tools-0.9.6/ooodev/format/draw/style/kind/__init__.py
--rw-r--r--   0        0        0     2652 2023-04-02 18:09:12.407617 ooo_dev_tools-0.9.6/ooodev/format/draw/style/lookup/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.408612 ooo_dev_tools-0.9.6/ooodev/format/impress/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.408612 ooo_dev_tools-0.9.6/ooodev/format/impress/modify/__init__.py
--rw-r--r--   0        0        0      945 2023-04-06 02:13:08.676094 ooo_dev_tools-0.9.6/ooodev/format/impress/modify/area/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.677093 ooo_dev_tools-0.9.6/ooodev/format/inner/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.677093 ooo_dev_tools-0.9.6/ooodev/format/inner/common/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.677093 ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/__init__.py
--rw-r--r--   0        0        0     3954 2023-04-06 02:13:08.678094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_document.py
--rw-r--r--   0        0        0     4577 2023-04-06 02:13:48.214066 ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_fill_color.py
--rw-r--r--   0        0        0    16076 2023-04-06 02:13:48.251066 ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_hf.py
--rw-r--r--   0        0        0     7849 2023-04-06 02:13:08.680093 ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_line_number.py
--rw-r--r--   0        0        0    11818 2023-04-06 02:13:08.681095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_padding.py
--rw-r--r--   0        0        0    10284 2023-04-06 02:13:08.682094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_sides.py
--rw-r--r--   0        0        0     5204 2023-04-23 13:05:05.660316 ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_writing_mode.py
--rw-r--r--   0        0        0     4323 2023-04-06 02:13:08.683094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/border_width_impl.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.683094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/format_types/__init__.py
--rw-r--r--   0        0        0      262 2023-04-06 02:13:08.684096 ooo_dev_tools-0.9.6/ooodev/format/inner/common/format_types/offset_column.py
--rw-r--r--   0        0        0      256 2023-04-06 02:13:08.684096 ooo_dev_tools-0.9.6/ooodev/format/inner/common/format_types/offset_row.py
--rw-r--r--   0        0        0      252 2023-04-06 02:13:08.685095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/format_types/size_percent.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.685095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/__init__.py
--rw-r--r--   0        0        0      318 2023-04-06 02:13:08.685095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/area_gradient_props.py
--rw-r--r--   0        0        0      324 2023-04-06 02:13:08.686095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/area_hatch_props.py
--rw-r--r--   0        0        0      531 2023-04-06 02:13:08.686095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/area_img_props.py
--rw-r--r--   0        0        0      294 2023-04-06 02:13:08.687092 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/area_pattern_props.py
--rw-r--r--   0        0        0      187 2023-04-06 02:13:08.687092 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/border_props.py
--rw-r--r--   0        0        0      181 2023-04-06 02:13:08.688095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/cell_background_color_props.py
--rw-r--r--   0        0        0      650 2023-04-06 02:13:08.688095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/cell_borders_props.py
--rw-r--r--   0        0        0      499 2023-04-06 02:13:08.689094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/cell_style_borders_props.py
--rw-r--r--   0        0        0      238 2023-04-06 02:13:08.689094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/cell_text_align_props.py
--rw-r--r--   0        0        0      197 2023-04-06 02:13:08.690093 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/cell_text_orientation_props.py
--rw-r--r--   0        0        0      203 2023-04-06 02:13:08.690093 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/cell_text_properties_props.py
--rw-r--r--   0        0        0      288 2023-04-06 02:13:08.691092 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/fill_color_props.py
--rw-r--r--   0        0        0      179 2023-04-06 02:13:08.691092 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/font_only_props.py
--rw-r--r--   0        0        0      176 2023-04-06 02:13:08.692095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/frame_options_align_props.py
--rw-r--r--   0        0        0      196 2023-04-06 02:13:08.692095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/frame_options_names_props.py
--rw-r--r--   0        0        0      239 2023-04-06 02:13:08.693095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/frame_options_properties.py
--rw-r--r--   0        0        0      244 2023-04-06 02:13:08.693095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/frame_options_protect_props.py
--rw-r--r--   0        0        0      166 2023-04-06 02:13:08.694094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/frame_type_anchor_props.py
--rw-r--r--   0        0        0      445 2023-04-06 02:13:08.695094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/frame_type_positon_props.py
--rw-r--r--   0        0        0      449 2023-04-06 02:13:08.695094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/frame_type_size_props.py
--rw-r--r--   0        0        0      231 2023-04-06 02:13:08.696094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/frame_wrap_options_props.py
--rw-r--r--   0        0        0      165 2023-04-06 02:13:08.696094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/frame_wrap_settings_props.py
--rw-r--r--   0        0        0      628 2023-04-06 02:13:08.697094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/hf_props.py
--rw-r--r--   0        0        0      313 2023-04-06 02:13:08.697094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/hyperlink_props.py
--rw-r--r--   0        0        0      263 2023-04-06 02:13:08.698096 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/image_crop_props.py
--rw-r--r--   0        0        0      253 2023-04-06 02:13:08.698096 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/image_flip_props.py
--rw-r--r--   0        0        0      209 2023-04-06 02:13:08.699094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/image_options_names_props.py
--rw-r--r--   0        0        0      168 2023-04-06 02:13:08.699094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/image_options_properties.py
--rw-r--r--   0        0        0      154 2023-04-06 02:13:08.700095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/image_rotation_props.py
--rw-r--r--   0        0        0      218 2023-04-06 02:13:08.700095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/img_para_area_props.py
--rw-r--r--   0        0        0      178 2023-04-06 02:13:08.701096 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/list_style_props.py
--rw-r--r--   0        0        0      207 2023-04-06 02:13:08.701096 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/page_margin_props.py
--rw-r--r--   0        0        0      157 2023-04-06 02:13:08.702098 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/prop_pair.py
--rw-r--r--   0        0        0      329 2023-04-06 02:13:08.702098 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/shape_shadow_props.py
--rw-r--r--   0        0        0      319 2023-04-06 02:13:08.703097 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/struct_border_table_props.py
--rw-r--r--   0        0        0      266 2023-04-06 02:13:08.703097 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/struct_cell_protection_props.py
--rw-r--r--   0        0        0      235 2023-04-06 02:13:08.704097 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/struct_crop_props.py
--rw-r--r--   0        0        0      349 2023-04-23 13:05:05.661314 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/struct_data_point_label_props.py
--rw-r--r--   0        0        0      208 2023-04-06 02:13:08.704097 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/struct_size_props.py
--rw-r--r--   0        0        0      333 2023-04-06 02:13:08.705094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/struct_table_border_distances_props.py
--rw-r--r--   0        0        0      443 2023-04-06 02:13:08.705094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/table_borders_props.py
--rw-r--r--   0        0        0      281 2023-04-06 02:13:08.706095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/table_properties_props.py
--rw-r--r--   0        0        0      181 2023-04-23 13:05:05.662316 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/title_alignment_orientation_props.py
--rw-r--r--   0        0        0      279 2023-04-06 02:13:08.706095 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/transparent_gradient_props.py
--rw-r--r--   0        0        0      188 2023-04-06 02:13:08.707094 ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/transparent_transparency_props.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.707094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.747094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.783096 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/alignment/__init__.py
--rw-r--r--   0        0        0     6882 2023-04-06 02:13:08.785095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/alignment/properties.py
--rw-r--r--   0        0        0     8619 2023-04-06 02:13:08.786095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/alignment/text_align.py
--rw-r--r--   0        0        0     6213 2023-04-06 02:13:08.786095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/alignment/text_orientation.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.787101 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/background/__init__.py
--rw-r--r--   0        0        0     5291 2023-04-06 02:13:48.252066 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/background/color.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.788097 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/border/__init__.py
--rw-r--r--   0        0        0    21721 2023-04-23 13:05:05.663315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/border/borders.py
--rw-r--r--   0        0        0     4491 2023-04-25 00:03:57.142368 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/border/padding.py
--rw-r--r--   0        0        0     2467 2023-04-25 00:03:57.143369 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/border/shadow.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.790094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/cell_protection/__init__.py
--rw-r--r--   0        0        0      340 2023-04-06 02:13:08.790094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/cell_protection/cell_protection.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.665318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/char/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.665318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/char/font/__init__.py
--rw-r--r--   0        0        0     5474 2023-04-23 13:05:05.666314 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/char/font/font.py
--rw-r--r--   0        0        0      483 2023-04-23 13:05:05.667318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/char/font/font_effects.py
--rw-r--r--   0        0        0      414 2023-04-23 13:05:05.667318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/char/font/font_only.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.668318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/numbers/__init__.py
--rw-r--r--   0        0        0    13621 2023-04-23 13:05:05.669315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/numbers/numbers.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.791094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/page/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.791094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/page/page/__init__.py
--rw-r--r--   0        0        0     6479 2023-04-06 02:13:08.792095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/page/page/layout_settings.py
--rw-r--r--   0        0        0     7798 2023-04-06 02:13:08.792095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/page/page/margins.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.669315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.669315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.669315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/font/__init__.py
--rw-r--r--   0        0        0      829 2023-04-23 13:05:05.670316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/font/font_effects.py
--rw-r--r--   0        0        0     2473 2023-04-23 13:05:05.671317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/font/font_only.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.671317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/label/__init__.py
--rw-r--r--   0        0        0     1727 2023-04-23 13:05:05.672315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/label/order.py
--rw-r--r--   0        0        0     3433 2023-04-23 13:05:05.690317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/label/orientation.py
--rw-r--r--   0        0        0     1539 2023-04-23 13:05:05.692315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/label/show.py
--rw-r--r--   0        0        0     2158 2023-04-23 13:05:05.693316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/label/text_flow.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.693316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/line/__init__.py
--rw-r--r--   0        0        0      269 2023-04-23 13:05:05.694316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/line/line_properties.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.695316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/numbers/__init__.py
--rw-r--r--   0        0        0      590 2023-04-23 13:05:05.697316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/numbers/numbers.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.697316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/positioning/__init__.py
--rw-r--r--   0        0        0     3064 2023-04-23 13:05:05.698315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/positioning/axis_line.py
--rw-r--r--   0        0        0     3481 2023-04-23 13:05:05.699318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/positioning/interval_marks.py
--rw-r--r--   0        0        0     1757 2023-04-23 13:05:05.721313 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/positioning/label_position.py
--rw-r--r--   0        0        0     3043 2023-04-23 13:05:05.722317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/positioning/position_axis.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.723316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.723316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/area/__init__.py
--rw-r--r--   0        0        0      895 2023-04-23 13:05:05.725319 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/area/color.py
--rw-r--r--   0        0        0     7146 2023-04-23 13:05:05.727315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/area/gradient.py
--rw-r--r--   0        0        0     9958 2023-04-23 13:05:05.728316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/area/hatch.py
--rw-r--r--   0        0        0     7581 2023-04-23 13:05:05.729316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/area/img.py
--rw-r--r--   0        0        0     5901 2023-04-23 13:05:05.729316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.730316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/borders/__init__.py
--rw-r--r--   0        0        0     4771 2023-04-23 13:05:05.731317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/borders/line_properties.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.731317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/numbers/__init__.py
--rw-r--r--   0        0        0     6352 2023-04-23 13:05:05.732316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/numbers/numbers.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.732316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/transparent/__init__.py
--rw-r--r--   0        0        0     5650 2023-04-23 13:05:05.733316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/transparent/gradient.py
--rw-r--r--   0        0        0     1173 2023-04-23 13:05:05.734315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/transparent/transparency.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.734315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/grid/__init__.py
--rw-r--r--   0        0        0     1542 2023-04-23 13:05:05.735316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/grid/line_properties.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.736317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.736317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/area/__init__.py
--rw-r--r--   0        0        0      213 2023-04-23 13:05:05.737315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/area/color.py
--rw-r--r--   0        0        0      285 2023-04-23 13:05:05.738316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/area/gradient.py
--rw-r--r--   0        0        0      224 2023-04-23 13:05:05.738316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/area/hatch.py
--rw-r--r--   0        0        0      253 2023-04-23 13:05:05.739316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/area/img.py
--rw-r--r--   0        0        0      236 2023-04-23 13:05:05.740315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.740315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/borders/__init__.py
--rw-r--r--   0        0        0      279 2023-04-23 13:05:05.741315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/borders/line_properties.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.742317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/font/__init__.py
--rw-r--r--   0        0        0      535 2023-04-23 13:05:05.744318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/font/font.py
--rw-r--r--   0        0        0      561 2023-04-23 13:05:05.745325 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/font/font_effects.py
--rw-r--r--   0        0        0      465 2023-04-23 13:05:05.745325 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/font/font_only.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.746317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/position/__init__.py
--rw-r--r--   0        0        0     5243 2023-04-23 13:05:05.808315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/position/position.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.808315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/transparent/__init__.py
--rw-r--r--   0        0        0      372 2023-04-23 13:05:05.856315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/transparent/gradient.py
--rw-r--r--   0        0        0      288 2023-04-23 13:05:05.856315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/transparent/transparency.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.857317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/position_size/__init__.py
--rw-r--r--   0        0        0     4171 2023-04-23 13:05:05.858317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/position_size/position.py
--rw-r--r--   0        0        0     4066 2023-04-23 13:05:05.859318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/position_size/size.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.859318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/__index__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.860316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.860316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/borders/__init__.py
--rw-r--r--   0        0        0     3112 2023-04-23 13:05:05.861316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/borders/line_properties.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.862317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/__init__.py
--rw-r--r--   0        0        0     3326 2023-04-23 13:05:05.863316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/attrib_options.py
--rw-r--r--   0        0        0     6717 2023-04-23 13:05:05.864316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/number_format.py
--rw-r--r--   0        0        0     4193 2023-04-23 13:05:05.864316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/orientation.py
--rw-r--r--   0        0        0     7580 2023-04-23 13:05:05.865316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/percent_format.py
--rw-r--r--   0        0        0      250 2023-04-23 13:05:05.866317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/text_attribs.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.866317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/font/__init__.py
--rw-r--r--   0        0        0      867 2023-04-23 13:05:05.867314 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/font/font_effects.py
--rw-r--r--   0        0        0     2511 2023-04-23 13:05:05.868317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/font/font_only.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.868317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.869315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/area/__init__.py
--rw-r--r--   0        0        0      220 2023-04-23 13:05:05.870317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/area/color.py
--rw-r--r--   0        0        0      292 2023-04-23 13:05:05.870317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/area/gradient.py
--rw-r--r--   0        0        0      231 2023-04-23 13:05:05.871315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/area/hatch.py
--rw-r--r--   0        0        0      260 2023-04-23 13:05:05.872317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/area/img.py
--rw-r--r--   0        0        0      243 2023-04-23 13:05:05.873317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.873317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/borders/__init__.py
--rw-r--r--   0        0        0     5492 2023-04-23 13:05:05.874316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/borders/line_properties.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.874316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/options/__init__.py
--rw-r--r--   0        0        0     4504 2023-04-23 13:05:05.876317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/options/align_series.py
--rw-r--r--   0        0        0     2841 2023-04-23 13:05:05.877319 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/options/legend_entry.py
--rw-r--r--   0        0        0     5033 2023-04-23 13:05:05.878316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/options/orientation.py
--rw-r--r--   0        0        0     2126 2023-04-23 13:05:05.879315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/options/plot.py
--rw-r--r--   0        0        0     3329 2023-04-23 13:05:05.880316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/options/plot_simple.py
--rw-r--r--   0        0        0     6823 2023-04-23 13:05:05.881314 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/options/settings.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.881314 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/transparent/__init__.py
--rw-r--r--   0        0        0      304 2023-04-23 13:05:05.882316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/transparent/gradient.py
--rw-r--r--   0        0        0      286 2023-04-23 13:05:05.882316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/transparent/transparency.py
--rw-r--r--   0        0        0     4171 2023-04-23 13:05:05.883315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/alignment/direction.py
--rw-r--r--   0        0        0     4313 2023-04-23 13:05:05.884316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/alignment/orientation.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.884316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/area/__init__.py
--rw-r--r--   0        0        0      213 2023-04-23 13:05:05.886315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/area/color.py
--rw-r--r--   0        0        0      285 2023-04-23 13:05:05.887313 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/area/gradient.py
--rw-r--r--   0        0        0      224 2023-04-23 13:05:05.930313 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/area/hatch.py
--rw-r--r--   0        0        0      253 2023-04-23 13:05:05.931335 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/area/img.py
--rw-r--r--   0        0        0      236 2023-04-23 13:05:05.932316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.932316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/borders/__init__.py
--rw-r--r--   0        0        0      278 2023-04-23 13:05:05.933316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/borders/line_properties.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.934319 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/font/__init__.py
--rw-r--r--   0        0        0     6359 2023-04-23 13:05:05.935317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/font/font.py
--rw-r--r--   0        0        0      918 2023-04-23 13:05:05.936322 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/font/font_effects.py
--rw-r--r--   0        0        0     2312 2023-04-23 13:05:05.936322 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/font/font_only.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.937320 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/position_size/__init__.py
--rw-r--r--   0        0        0      880 2023-04-23 13:05:05.938317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/position_size/position.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.938317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.938317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/area/__init__.py
--rw-r--r--   0        0        0      657 2023-04-23 13:05:05.939316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/area/color.py
--rw-r--r--   0        0        0      712 2023-04-23 13:05:05.940318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/area/gradient.py
--rw-r--r--   0        0        0      658 2023-04-23 13:05:05.941317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/area/hatch.py
--rw-r--r--   0        0        0      686 2023-04-23 13:05:05.942316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/area/img.py
--rw-r--r--   0        0        0      670 2023-04-23 13:05:05.943317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.943317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/borders/__init__.py
--rw-r--r--   0        0        0      719 2023-04-23 13:05:05.944316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/borders/line_properties.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.944316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/transparent/__init__.py
--rw-r--r--   0        0        0      725 2023-04-23 13:05:05.945315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/transparent/gradient.py
--rw-r--r--   0        0        0     1040 2023-04-23 13:05:05.946318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/transparent/transparency.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.947318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/draw/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.947318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/draw/fill/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:05.947318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/draw/fill/area/__init__.py
--rw-r--r--   0        0        0      229 2023-04-23 13:05:05.948315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/draw/fill/area/color.py
--rw-r--r--   0        0        0      288 2023-04-23 13:05:06.011316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/draw/fill/area/gradient.py
--rw-r--r--   0        0        0      249 2023-04-23 13:05:06.014318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/draw/fill/area/hatch.py
--rw-r--r--   0        0        0      266 2023-04-23 13:05:06.016320 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/draw/fill/area/img.py
--rw-r--r--   0        0        0      250 2023-04-23 13:05:06.061315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/draw/fill/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:06.062319 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/draw/shape/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:06.062319 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/draw/shape/position_size/__init__.py
--rw-r--r--   0        0        0     3378 2023-04-23 13:05:06.063318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/draw/shape/position_size/position.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.793096 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/__init__.py
--rw-r--r--   0        0        0     9315 2023-04-06 02:13:48.258068 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/cell_protection_struct.py
--rw-r--r--   0        0        0    11233 2023-04-06 02:13:48.260066 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/crop_struct.py
--rw-r--r--   0        0        0    11148 2023-04-23 13:05:06.064318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/data_point_label_struct.py
--rw-r--r--   0        0        0    10183 2023-04-06 02:13:48.262067 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/drop_cap_struct.py
--rw-r--r--   0        0        0    14924 2023-04-23 13:05:06.065314 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/gradient_struct.py
--rw-r--r--   0        0        0     8274 2023-04-06 02:13:48.266068 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/hatch_struct.py
--rw-r--r--   0        0        0    10085 2023-04-06 02:13:48.267067 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/line_spacing_struct.py
--rw-r--r--   0        0        0    31720 2023-04-06 02:13:48.269067 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/locale_struct.py
--rw-r--r--   0        0        0     7412 2023-04-23 13:05:06.066317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/point_struct.py
--rw-r--r--   0        0        0    11808 2023-04-25 00:03:57.144366 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/shadow_struct.py
--rw-r--r--   0        0        0    25317 2023-04-06 02:13:48.277068 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/side.py
--rw-r--r--   0        0        0     8482 2023-04-23 13:05:06.068316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/size_struct.py
--rw-r--r--   0        0        0      640 2023-04-06 02:13:08.801095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/struct_base.py
--rw-r--r--   0        0        0    13991 2023-04-06 02:13:48.280068 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/tab_stop_struct.py
--rw-r--r--   0        0        0    13469 2023-04-06 02:13:48.281067 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/table_border_distances_struct.py
--rw-r--r--   0        0        0    20841 2023-04-06 02:13:48.282066 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/table_border_struct.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.803095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.803095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.804095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/border/__init__.py
--rw-r--r--   0        0        0    10699 2023-04-25 00:03:57.146365 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/border/borders.py
--rw-r--r--   0        0        0     3673 2023-04-25 00:03:57.148365 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/border/padding.py
--rw-r--r--   0        0        0     2842 2023-04-25 00:03:57.149366 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/border/shadow.py
--rw-r--r--   0        0        0     1766 2023-04-06 02:13:08.806095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/border/sides.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.807104 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/font/__init__.py
--rw-r--r--   0        0        0    34878 2023-04-23 13:05:06.069317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/font/font.py
--rw-r--r--   0        0        0    26959 2023-04-23 13:05:06.070317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/font/font_effects.py
--rw-r--r--   0        0        0    21564 2023-04-23 13:05:06.070317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/font/font_only.py
--rw-r--r--   0        0        0    21425 2023-04-23 13:05:06.120316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/font/font_position.py
--rw-r--r--   0        0        0        1 2023-04-06 02:13:08.810097 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/highlight/__init__.py
--rw-r--r--   0        0        0     5299 2023-04-23 13:05:06.121316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/highlight/highlight.py
--rw-r--r--   0        0        0        1 2023-04-06 02:13:08.811097 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/hyperlink/__init__.py
--rw-r--r--   0        0        0     5191 2023-04-23 13:05:06.122323 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/hyperlink/hyperlink.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.812096 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.812096 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/area/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-06 02:13:08.813095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/area/fill_color.py
--rw-r--r--   0        0        0    14379 2023-04-25 00:03:57.150372 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/area/gradient.py
--rw-r--r--   0        0        0    13254 2023-04-23 13:05:06.124315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/area/hatch.py
--rw-r--r--   0        0        0    18444 2023-04-23 13:05:06.126315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/area/img.py
--rw-r--r--   0        0        0    10537 2023-04-23 13:05:06.127315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.837095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/transparent/__init__.py
--rw-r--r--   0        0        0    12939 2023-04-23 13:05:06.129317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/transparent/gradient.py
--rw-r--r--   0        0        0     5167 2023-04-25 00:03:57.152366 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/transparent/transparency.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.852094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.852094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/frame_type/__init__.py
--rw-r--r--   0        0        0     4866 2023-04-06 02:13:08.853094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/frame_type/anchor.py
--rw-r--r--   0        0        0    18717 2023-04-06 02:13:08.866093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/frame_type/position.py
--rw-r--r--   0        0        0     6874 2023-04-06 02:13:08.867093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/frame_type/size.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.867093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/hyperlink/__init__.py
--rw-r--r--   0        0        0     4026 2023-04-06 02:13:08.868093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/hyperlink/image_map_options.py
--rw-r--r--   0        0        0     5997 2023-04-06 02:13:08.869093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/hyperlink/link_to.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.869093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/options/__init__.py
--rw-r--r--   0        0        0     4913 2023-04-06 02:13:08.870096 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/options/align.py
--rw-r--r--   0        0        0     8725 2023-04-06 02:13:08.871096 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/options/names.py
--rw-r--r--   0        0        0     9653 2023-04-06 02:13:08.871096 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/options/properties.py
--rw-r--r--   0        0        0     4781 2023-04-06 02:13:08.872094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/options/protect.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.872094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/wrap/__init__.py
--rw-r--r--   0        0        0     7691 2023-04-06 02:13:08.873093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/wrap/options.py
--rw-r--r--   0        0        0     3655 2023-04-06 02:13:08.873093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/wrap/settings.py
--rw-r--r--   0        0        0     1796 2023-04-06 02:13:08.874109 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/wrap/spacing.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.874109 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.874109 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/crop/__init__.py
--rw-r--r--   0        0        0    18759 2023-04-06 02:13:48.323067 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/crop/crop.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.875093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/image/__init__.py
--rw-r--r--   0        0        0     5201 2023-04-06 02:13:08.876094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/image/flip.py
--rw-r--r--   0        0        0     3716 2023-04-06 02:13:08.876094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/image/rotation.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.877095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/image_type/__init__.py
--rw-r--r--   0        0        0    11093 2023-04-06 02:13:08.877095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/image_type/size.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.878097 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/options/__init__.py
--rw-r--r--   0        0        0     2718 2023-04-06 02:13:08.878097 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/options/names.py
--rw-r--r--   0        0        0     3786 2023-04-06 02:13:08.879093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/options/properties.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.879093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:48.323067 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:48.324069 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/area/__init__.py
--rw-r--r--   0        0        0      961 2023-04-06 02:13:48.325067 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/area/color.py
--rw-r--r--   0        0        0     1247 2023-04-06 02:13:48.325067 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/area/gradient.py
--rw-r--r--   0        0        0     1302 2023-04-06 02:13:48.326069 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/area/hatch.py
--rw-r--r--   0        0        0     1505 2023-04-06 02:13:48.326069 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/area/img.py
--rw-r--r--   0        0        0     1226 2023-04-06 02:13:48.327067 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/area/pattern.py
--rw-r--r--   0        0        0     1432 2023-04-06 02:13:48.328065 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/footer.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:48.328065 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:48.329080 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/area/__init__.py
--rw-r--r--   0        0        0     1376 2023-04-06 02:13:48.329080 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/area/color.py
--rw-r--r--   0        0        0     1679 2023-04-06 02:13:48.359068 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/area/gradient.py
--rw-r--r--   0        0        0     1815 2023-04-06 02:13:48.360070 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/area/hatch.py
--rw-r--r--   0        0        0     1962 2023-04-06 02:13:48.361065 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/area/img.py
--rw-r--r--   0        0        0     1683 2023-04-06 02:13:48.362067 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/area/pattern.py
--rw-r--r--   0        0        0     1432 2023-04-06 02:13:48.413067 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/header.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.879093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/page/__init__.py
--rw-r--r--   0        0        0     6554 2023-04-06 02:13:08.880098 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/page/layout_settings.py
--rw-r--r--   0        0        0     3103 2023-04-06 02:13:08.881093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/page/margins.py
--rw-r--r--   0        0        0     5382 2023-04-06 02:13:08.882094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/page/paper_format.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.882094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/__init__.py
--rw-r--r--   0        0        0      389 2023-04-06 02:13:08.883094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/align/__init__.py
--rw-r--r--   0        0        0    15153 2023-04-23 13:05:06.130316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/align/alignment.py
--rw-r--r--   0        0        0     3563 2023-04-23 13:05:06.131316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/align/writing_mode.py
--rw-r--r--   0        0        0        1 2023-04-06 02:13:08.886093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/area/__init__.py
--rw-r--r--   0        0        0     2329 2023-04-23 13:05:06.132317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/area/color.py
--rw-r--r--   0        0        0    16148 2023-04-25 00:03:57.157367 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/area/hatch.py
--rw-r--r--   0        0        0    12316 2023-04-25 00:03:57.158377 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/area/img.py
--rw-r--r--   0        0        0     7090 2023-04-25 00:03:57.162369 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/area/pattern.py
--rw-r--r--   0        0        0      471 2023-04-06 02:13:08.889093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/border/__init__.py
--rw-r--r--   0        0        0    11995 2023-04-23 13:05:06.133316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/border/borders.py
--rw-r--r--   0        0        0     2524 2023-04-06 02:13:08.890095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/border/padding.py
--rw-r--r--   0        0        0      834 2023-04-06 02:13:08.891093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/border/shadow.py
--rw-r--r--   0        0        0     2025 2023-04-06 02:13:08.892093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/border/sides.py
--rw-r--r--   0        0        0        1 2023-04-06 02:13:08.892093 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/drop_cap/__init__.py
--rw-r--r--   0        0        0     9215 2023-04-23 13:05:06.134314 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/drop_cap/drop_caps.py
--rw-r--r--   0        0        0      303 2023-04-06 02:13:08.894096 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/indent_space/__init__.py
--rw-r--r--   0        0        0     9784 2023-04-23 13:05:06.135316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/indent_space/indent.py
--rw-r--r--   0        0        0     8011 2023-04-06 02:13:08.895096 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/indent_space/indent_spacing.py
--rw-r--r--   0        0        0     7733 2023-04-23 13:05:06.136315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/indent_space/line_spacing.py
--rw-r--r--   0        0        0     8546 2023-04-23 13:05:06.137317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/indent_space/spacing.py
--rw-r--r--   0        0        0      368 2023-04-06 02:13:08.917097 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/outline_list/__init__.py
--rw-r--r--   0        0        0     1937 2023-04-23 13:05:06.138318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/outline_list/line_num.py
--rw-r--r--   0        0        0    10154 2023-04-23 13:05:06.138318 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/outline_list/list_style.py
--rw-r--r--   0        0        0     7701 2023-04-23 13:05:06.139319 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/outline_list/outline.py
--rw-r--r--   0        0        0     7271 2023-04-23 13:05:06.140316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/outline_list/outline_list.py
--rw-r--r--   0        0        0     2936 2023-04-06 02:13:08.920094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/padding.py
--rw-r--r--   0        0        0      191 2023-04-06 02:13:08.920094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/tabs/__init__.py
--rw-r--r--   0        0        0    10188 2023-04-23 13:05:06.141315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/tabs/tabs.py
--rw-r--r--   0        0        0      261 2023-04-06 02:13:08.921095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/text_flow/__init__.py
--rw-r--r--   0        0        0     6561 2023-04-23 13:05:06.142317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/text_flow/breaks.py
--rw-r--r--   0        0        0    10397 2023-04-23 13:05:06.143317 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/text_flow/flow_options.py
--rw-r--r--   0        0        0    10282 2023-04-23 13:05:06.144316 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/text_flow/hyphenation.py
--rw-r--r--   0        0        0     7546 2023-04-23 13:05:06.145315 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/text_flow/text_flow.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.924094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/transparent/__init__.py
--rw-r--r--   0        0        0     3859 2023-04-06 02:13:08.925095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/transparent/gradient.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.925095 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/shape/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.926092 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/shape/area/__init__.py
--rw-r--r--   0        0        0    16356 2023-04-06 02:13:48.420065 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/shape/area/shadow.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.927094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/table/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.927094 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/table/background/__init__.py
--rw-r--r--   0        0        0     1628 2023-04-25 00:03:57.164367 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/table/background/color.py
--rw-r--r--   0        0        0     4880 2023-04-25 00:03:57.165366 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/table/background/img.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.929096 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/table/borders/__init__.py
--rw-r--r--   0        0        0    18876 2023-04-25 00:03:57.173370 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/table/borders/borders.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.929096 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/table/props/__init__.py
--rw-r--r--   0        0        0    74742 2023-04-25 00:03:57.175369 ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/table/props/table_properties.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.931093 ooo_dev_tools-0.9.6/ooodev/format/inner/kind/__init__.py
--rw-r--r--   0        0        0      231 2023-04-06 02:13:08.932094 ooo_dev_tools-0.9.6/ooodev/format/inner/kind/border_kind.py
--rw-r--r--   0        0        0      509 2023-04-06 02:13:48.421066 ooo_dev_tools-0.9.6/ooodev/format/inner/kind/format_kind.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.932094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.933097 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.933097 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/alignment/__init__.py
--rw-r--r--   0        0        0     3747 2023-04-06 02:13:08.934097 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/alignment/properties.py
--rw-r--r--   0        0        0     3809 2023-04-06 02:13:08.935098 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/alignment/text_align.py
--rw-r--r--   0        0        0     3655 2023-04-06 02:13:08.935098 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/alignment/text_orientation.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.935098 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/background/__init__.py
--rw-r--r--   0        0        0     3261 2023-04-06 02:13:48.422065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/background/color.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.936097 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/border/__init__.py
--rw-r--r--   0        0        0    23992 2023-04-07 18:06:32.203989 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/border/borders.py
--rw-r--r--   0        0        0      172 2023-04-07 18:06:32.209987 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/border/padding.py
--rw-r--r--   0        0        0      166 2023-04-07 18:06:32.210989 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/border/shadow.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.937094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/cell_protection/__init__.py
--rw-r--r--   0        0        0     4681 2023-04-06 02:13:08.938093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/cell_protection/cell_protection.py
--rw-r--r--   0        0        0     3739 2023-04-06 02:13:08.938093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/cell_style_base.py
--rw-r--r--   0        0        0      820 2023-04-06 02:13:08.939094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/cell_style_base_multi.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.939094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/font/__init__.py
--rw-r--r--   0        0        0     6013 2023-04-06 02:13:48.425066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/font/font_effects.py
--rw-r--r--   0        0        0     4325 2023-04-06 02:13:08.941096 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/font/font_only.py
--rw-r--r--   0        0        0        0 2023-04-23 13:05:06.145315 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/numbers/__index__.py
--rw-r--r--   0        0        0     4733 2023-04-23 13:05:06.146314 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/numbers/numbers.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.941096 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.941096 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/area/__init__.py
--rw-r--r--   0        0        0     4943 2023-04-06 02:13:48.426066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/area/color.py
--rw-r--r--   0        0        0     5808 2023-04-06 02:13:08.942093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/area/img.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.943095 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/border/__init__.py
--rw-r--r--   0        0        0     5359 2023-04-06 02:13:08.943095 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/border/padding.py
--rw-r--r--   0        0        0     4973 2023-04-06 02:13:48.426066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/border/shadow.py
--rw-r--r--   0        0        0     5300 2023-04-06 02:13:08.945095 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/border/sides.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.945095 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.945095 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/area/__init__.py
--rw-r--r--   0        0        0     1028 2023-04-06 02:13:48.427066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/area/color.py
--rw-r--r--   0        0        0     1943 2023-04-06 02:13:48.428066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/area/img.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.947095 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/border/__init__.py
--rw-r--r--   0        0        0     1095 2023-04-06 02:13:48.429066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/border/padding.py
--rw-r--r--   0        0        0      917 2023-04-06 02:13:48.429066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/border/shadow.py
--rw-r--r--   0        0        0     1092 2023-04-06 02:13:48.430065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/border/sides.py
--rw-r--r--   0        0        0     1116 2023-04-06 02:13:48.431066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/footer.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.982094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.982094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/area/__init__.py
--rw-r--r--   0        0        0     5283 2023-04-06 02:13:48.431066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/area/color.py
--rw-r--r--   0        0        0     7094 2023-04-06 02:13:48.432068 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/area/img.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.984094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/border/__init__.py
--rw-r--r--   0        0        0     6626 2023-04-06 02:13:48.433067 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/border/padding.py
--rw-r--r--   0        0        0     6045 2023-04-06 02:13:48.434070 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/border/shadow.py
--rw-r--r--   0        0        0     6289 2023-04-06 02:13:48.434070 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/border/sides.py
--rw-r--r--   0        0        0     7271 2023-04-06 02:13:48.435066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/header.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.986093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/page/__init__.py
--rw-r--r--   0        0        0     3819 2023-04-06 02:13:08.987094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/page/layout_settings.py
--rw-r--r--   0        0        0     3565 2023-04-06 02:13:08.987094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/page/margins.py
--rw-r--r--   0        0        0     4332 2023-04-06 02:13:08.988093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/page/paper_format.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.988093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/sheet/__init__.py
--rw-r--r--   0        0        0     4051 2023-04-06 02:13:08.989095 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/sheet/order.py
--rw-r--r--   0        0        0     7444 2023-04-06 02:13:08.989095 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/sheet/printing.py
--rw-r--r--   0        0        0     3418 2023-04-06 02:13:08.990094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/sheet/scale_num_of_pages.py
--rw-r--r--   0        0        0     4164 2023-04-06 02:13:08.991094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/sheet/scale_pages_width_height.py
--rw-r--r--   0        0        0     3543 2023-04-06 02:13:08.991094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/sheet/scale_reduce_enlarge.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.991094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.992093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.992093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/border/__init__.py
--rw-r--r--   0        0        0     3830 2023-04-06 02:13:08.993104 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/border/padding.py
--rw-r--r--   0        0        0     3881 2023-04-06 02:13:48.436066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/border/shadow.py
--rw-r--r--   0        0        0     3905 2023-04-06 02:13:08.994096 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/border/sides.py
--rw-r--r--   0        0        0      701 2023-04-06 02:13:08.994096 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/char_style_base_multi.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.995093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/font/__init__.py
--rw-r--r--   0        0        0     5324 2023-04-06 02:13:48.437065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/font/font_effects.py
--rw-r--r--   0        0        0     3778 2023-04-06 02:13:08.996095 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/font/font_only.py
--rw-r--r--   0        0        0     4855 2023-04-06 02:13:08.997094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/font/font_position.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.997094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/highlight/__init__.py
--rw-r--r--   0        0        0     3099 2023-04-06 02:13:48.438068 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/highlight/highlight.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.998094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/fill/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:08.999094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/fill/area/__init__.py
--rw-r--r--   0        0        0     5010 2023-04-06 02:13:48.439067 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/fill/area/img.py
--rw-r--r--   0        0        0      686 2023-04-06 02:13:09.000093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/fill/fill_style_base_multi.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.001095 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.001095 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/area/__init__.py
--rw-r--r--   0        0        0     3731 2023-04-06 02:13:48.440068 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/area/color.py
--rw-r--r--   0        0        0     6551 2023-04-06 02:13:48.441068 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/area/gradient.py
--rw-r--r--   0        0        0     5763 2023-04-06 02:13:48.442065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/area/hatch.py
--rw-r--r--   0        0        0     6033 2023-04-06 02:13:09.004092 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/area/img.py
--rw-r--r--   0        0        0     5246 2023-04-06 02:13:48.442065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.005095 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/border/__init__.py
--rw-r--r--   0        0        0     4498 2023-04-06 02:13:09.006094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/border/padding.py
--rw-r--r--   0        0        0     4409 2023-04-06 02:13:48.443065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/border/shadow.py
--rw-r--r--   0        0        0     4309 2023-04-06 02:13:09.007094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/border/sides.py
--rw-r--r--   0        0        0      742 2023-04-06 02:13:09.008093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/frame_style_base_multi.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.009094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/frame_type/__init__.py
--rw-r--r--   0        0        0     3280 2023-04-06 02:13:09.009094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/frame_type/anchor.py
--rw-r--r--   0        0        0     3895 2023-04-06 02:13:09.010094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/frame_type/position.py
--rw-r--r--   0        0        0     3568 2023-04-06 02:13:09.011093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/frame_type/size.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.011093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/options/__init__.py
--rw-r--r--   0        0        0     3294 2023-04-06 02:13:09.012094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/options/align.py
--rw-r--r--   0        0        0     3551 2023-04-06 02:13:09.012094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/options/properties.py
--rw-r--r--   0        0        0     3335 2023-04-06 02:13:09.013101 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/options/protect.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.013101 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/transparent/__init__.py
--rw-r--r--   0        0        0     4635 2023-04-06 02:13:09.040094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/transparent/gradient.py
--rw-r--r--   0        0        0     3782 2023-04-06 02:13:09.041093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/transparent/transparency.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.041093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/wrap/__init__.py
--rw-r--r--   0        0        0     3838 2023-04-06 02:13:09.042094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/wrap/options.py
--rw-r--r--   0        0        0     3185 2023-04-06 02:13:09.043094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/wrap/settings.py
--rw-r--r--   0        0        0     3864 2023-04-06 02:13:09.043094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/wrap/spacing.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.044094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.044094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/area/__init__.py
--rw-r--r--   0        0        0     4253 2023-04-06 02:13:48.444065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/area/color.py
--rw-r--r--   0        0        0     6171 2023-04-06 02:13:48.444065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/area/gradient.py
--rw-r--r--   0        0        0     5020 2023-04-06 02:13:48.445065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/area/hatch.py
--rw-r--r--   0        0        0     5914 2023-04-06 02:13:09.046093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/area/img.py
--rw-r--r--   0        0        0     4802 2023-04-06 02:13:48.446066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.047093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/border/__init__.py
--rw-r--r--   0        0        0     3905 2023-04-06 02:13:09.048094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/border/padding.py
--rw-r--r--   0        0        0     5049 2023-04-06 02:13:48.447065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/border/shadow.py
--rw-r--r--   0        0        0     3829 2023-04-06 02:13:09.049093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/border/sides.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.049093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.049093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/area/__init__.py
--rw-r--r--   0        0        0      892 2023-04-06 02:13:48.447065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/area/color.py
--rw-r--r--   0        0        0     1072 2023-04-06 02:13:48.448067 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/area/gradient.py
--rw-r--r--   0        0        0     1007 2023-04-06 02:13:48.449065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/area/hatch.py
--rw-r--r--   0        0        0     1346 2023-04-06 02:13:48.449065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/area/img.py
--rw-r--r--   0        0        0     1077 2023-04-06 02:13:48.450068 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.052094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/border/__init__.py
--rw-r--r--   0        0        0     1052 2023-04-06 02:13:48.510066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/border/padding.py
--rw-r--r--   0        0        0      976 2023-04-06 02:13:48.511066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/border/shadow.py
--rw-r--r--   0        0        0      971 2023-04-06 02:13:48.511066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/border/sides.py
--rw-r--r--   0        0        0     1176 2023-04-06 02:13:48.512066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/footer.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.055093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/transparency/__init__.py
--rw-r--r--   0        0        0     1095 2023-04-06 02:13:48.513065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/transparency/gradient.py
--rw-r--r--   0        0        0      994 2023-04-06 02:13:48.513065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/transparency/transparency.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.056092 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.057094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/area/__init__.py
--rw-r--r--   0        0        0     5331 2023-04-06 02:13:48.514066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/area/color.py
--rw-r--r--   0        0        0     7596 2023-04-06 02:13:48.515074 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/area/gradient.py
--rw-r--r--   0        0        0     6455 2023-04-06 02:13:48.515074 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/area/hatch.py
--rw-r--r--   0        0        0     7602 2023-04-06 02:13:48.516066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/area/img.py
--rw-r--r--   0        0        0     6295 2023-04-06 02:13:48.517067 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.060095 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/border/__init__.py
--rw-r--r--   0        0        0     6729 2023-04-06 02:13:48.517067 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/border/padding.py
--rw-r--r--   0        0        0     6148 2023-04-06 02:13:48.518065 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/border/shadow.py
--rw-r--r--   0        0        0     6403 2023-04-06 02:13:48.519066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/border/sides.py
--rw-r--r--   0        0        0     7279 2023-04-06 02:13:48.519066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/header.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.063098 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/transparency/__init__.py
--rw-r--r--   0        0        0     5959 2023-04-06 02:13:48.520064 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/transparency/gradient.py
--rw-r--r--   0        0        0     4560 2023-04-06 02:13:48.521067 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/transparency/transparency.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.064093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/page/__init__.py
--rw-r--r--   0        0        0     4052 2023-04-06 02:13:09.065093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/page/layout_settings.py
--rw-r--r--   0        0        0     3750 2023-04-06 02:13:09.066093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/page/margins.py
--rw-r--r--   0        0        0     4359 2023-04-06 02:13:09.066093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/page/paper_format.py
--rw-r--r--   0        0        0      778 2023-04-06 02:13:09.066093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/page_style_base_multi.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.067093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/transparency/__init__.py
--rw-r--r--   0        0        0     3751 2023-04-06 02:13:09.068093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/transparency/gradient.py
--rw-r--r--   0        0        0     3261 2023-04-06 02:13:09.069094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/transparency/transparency.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.069094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.069094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/align/__init__.py
--rw-r--r--   0        0        0     4517 2023-04-06 02:13:09.070093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/align/alignment.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.070093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/area/__init__.py
--rw-r--r--   0        0        0     2740 2023-04-06 02:13:48.522066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/area/color.py
--rw-r--r--   0        0        0     5562 2023-04-06 02:13:48.523066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/area/gradient.py
--rw-r--r--   0        0        0     5340 2023-04-06 02:13:48.523066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/area/hatch.py
--rw-r--r--   0        0        0     5005 2023-04-06 02:13:48.524066 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/area/img.py
--rw-r--r--   0        0        0     4841 2023-04-06 02:13:09.073094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/area/pattern.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.073094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/border/__init__.py
--rw-r--r--   0        0        0     4484 2023-04-06 02:13:09.085094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/border/borders.py
--rw-r--r--   0        0        0     3853 2023-04-06 02:13:09.086093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/border/padding.py
--rw-r--r--   0        0        0     3916 2023-04-06 02:13:48.525067 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/border/shadow.py
--rw-r--r--   0        0        0     3752 2023-04-06 02:13:09.087092 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/border/sides.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.087092 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/drop_cap/__init__.py
--rw-r--r--   0        0        0     3892 2023-04-06 02:13:09.088093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/drop_cap/drop_caps.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.088093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/font/__init__.py
--rw-r--r--   0        0        0     5359 2023-04-06 02:13:48.565068 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/font/font_effects.py
--rw-r--r--   0        0        0     3722 2023-04-06 02:13:09.089094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/font/font_only.py
--rw-r--r--   0        0        0     4933 2023-04-06 02:13:09.090093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/font/font_position.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.090093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/highlight/__init__.py
--rw-r--r--   0        0        0     3162 2023-04-06 02:13:48.570063 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/highlight/highlight.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.091092 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/indent_space/__init__.py
--rw-r--r--   0        0        0     3715 2023-04-06 02:13:09.092093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/indent_space/indent.py
--rw-r--r--   0        0        0     4124 2023-04-06 02:13:48.592064 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/indent_space/line_spacing.py
--rw-r--r--   0        0        0     3555 2023-04-06 02:13:09.093094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/indent_space/spacing.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.093094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/outline_list/__init__.py
--rw-r--r--   0        0        0     4065 2023-04-06 02:13:09.094093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/outline_list/line_num.py
--rw-r--r--   0        0        0     8129 2023-04-06 02:13:09.095094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/outline_list/list_style.py
--rw-r--r--   0        0        0     3214 2023-04-06 02:13:09.095094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/outline_list/outline.py
--rw-r--r--   0        0        0      837 2023-04-06 02:13:09.096093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/para_style_base_multi.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.096093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/tabs/__init__.py
--rw-r--r--   0        0        0     5372 2023-04-06 02:13:09.097093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/tabs/tabs.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.097093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/text_flow/__init__.py
--rw-r--r--   0        0        0     3288 2023-04-06 02:13:09.099100 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/text_flow/breaks.py
--rw-r--r--   0        0        0     3449 2023-04-06 02:13:09.110092 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/text_flow/flow_options.py
--rw-r--r--   0        0        0     3577 2023-04-06 02:13:09.110092 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/text_flow/hyphenation.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.111094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/transparent/__init__.py
--rw-r--r--   0        0        0     3765 2023-04-06 02:13:09.111094 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/transparent/gradient.py
--rw-r--r--   0        0        0     3230 2023-04-06 02:13:09.112093 ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/transparent/transparency.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:09.112093 ooo_dev_tools-0.9.6/ooodev/format/inner/preset/__init__.py
--rw-r--r--   0        0        0    28652 2023-04-23 13:05:06.147315 ooo_dev_tools-0.9.6/ooodev/format/inner/preset/preset_border_line.py
--rw-r--r--   0        0        0     8819 2023-04-06 02:13:48.593066 ooo_dev_tools-0.9.6/ooodev/format/inner/preset/preset_gradient.py
--rw-r--r--   0        0        0     7403 2023-04-06 02:13:48.594065 ooo_dev_tools-0.9.6/ooodev/format/inner/preset/preset_hatch.py
--rw-r--r--   0        0        0  1674033 2023-04-06 02:13:09.129092 ooo_dev_tools-0.9.6/ooodev/format/inner/preset/preset_image.py
--rw-r--r--   0        0        0     1257 2023-04-06 02:13:09.135093 ooo_dev_tools-0.9.6/ooodev/format/inner/preset/preset_paper_format.py
--rw-r--r--   0        0        0     5884 2023-04-06 02:13:09.137094 ooo_dev_tools-0.9.6/ooodev/format/inner/preset/preset_pattern.py
--rw-r--r--   0        0        0    53215 2023-04-23 13:05:06.149315 ooo_dev_tools-0.9.6/ooodev/format/inner/style_base.py
--rw-r--r--   0        0        0    17583 2023-04-23 13:05:06.150314 ooo_dev_tools-0.9.6/ooodev/format/readme.md
--rw-r--r--   0        0        0      738 2023-04-06 02:13:09.175094 ooo_dev_tools-0.9.6/ooodev/format/styler.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.738588 ooo_dev_tools-0.9.6/ooodev/format/writer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.738588 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.739586 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/char/__init__.py
--rw-r--r--   0        0        0      957 2023-04-06 02:13:09.175094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/char/borders/__init__.py
--rw-r--r--   0        0        0     1687 2023-04-23 13:05:06.151315 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/char/font/__init__.py
--rw-r--r--   0        0        0      129 2023-04-06 02:13:09.177094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/char/highlight/__init__.py
--rw-r--r--   0        0        0      238 2023-04-06 02:13:09.178103 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/char/hyperlink/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.741673 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/frame/__init__.py
--rw-r--r--   0        0        0     2001 2023-04-06 02:13:09.178103 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/frame/area/__init__.py
--rw-r--r--   0        0        0      636 2023-04-06 02:13:09.180093 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/frame/borders/__init__.py
--rw-r--r--   0        0        0      349 2023-04-06 02:13:09.181096 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/frame/hyperlink/__init__.py
--rw-r--r--   0        0        0      653 2023-04-06 02:13:09.183092 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/frame/options/__init__.py
--rw-r--r--   0        0        0      584 2023-04-06 02:13:09.184095 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/frame/transparency/__init__.py
--rw-r--r--   0        0        0     1471 2023-04-06 02:13:09.184095 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/frame/type/__init__.py
--rw-r--r--   0        0        0      378 2023-04-06 02:13:09.185094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/frame/wrap/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.753585 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/image/__init__.py
--rw-r--r--   0        0        0     2001 2023-04-06 02:13:09.186092 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/image/area/__init__.py
--rw-r--r--   0        0        0      636 2023-04-06 02:13:09.187095 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/image/borders/__init__.py
--rw-r--r--   0        0        0      313 2023-04-06 02:13:09.188095 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/image/crop/__init__.py
--rw-r--r--   0        0        0      351 2023-04-06 02:13:09.188095 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/image/hyperlink/__init__.py
--rw-r--r--   0        0        0      289 2023-04-06 02:13:09.189094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/image/image/__init__.py
--rw-r--r--   0        0        0      318 2023-04-06 02:13:09.190093 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/image/options/__init__.py
--rw-r--r--   0        0        0      584 2023-04-06 02:13:09.191094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/image/transparency/__init__.py
--rw-r--r--   0        0        0     1471 2023-04-06 02:13:09.191094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/image/type/__init__.py
--rw-r--r--   0        0        0      378 2023-04-06 02:13:09.192094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/image/wrap/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.758699 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/obj/__init__.py
--rw-r--r--   0        0        0     2001 2023-04-06 02:13:09.193093 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/obj/area/__init__.py
--rw-r--r--   0        0        0      636 2023-04-06 02:13:09.194093 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/obj/borders/__init__.py
--rw-r--r--   0        0        0      349 2023-04-06 02:13:09.194093 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/obj/hyperlink/__init__.py
--rw-r--r--   0        0        0      318 2023-04-06 02:13:09.196094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/obj/options/__init__.py
--rw-r--r--   0        0        0      584 2023-04-06 02:13:09.197093 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/obj/transparency/__init__.py
--rw-r--r--   0        0        0     1471 2023-04-06 02:13:09.198094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/obj/type/__init__.py
--rw-r--r--   0        0        0      378 2023-04-06 02:13:09.198094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/obj/wrap/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 02:13:48.596069 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/page/__init__.py
--rw-r--r--   0        0        0      114 2023-04-06 02:13:48.597066 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/page/footer/__init__.py
--rw-r--r--   0        0        0     1743 2023-04-06 02:13:48.598067 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/page/footer/area/__init__.py
--rw-r--r--   0        0        0      114 2023-04-06 02:13:48.598067 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/page/header/__init__.py
--rw-r--r--   0        0        0     1743 2023-04-06 02:13:48.599067 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/page/header/area/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.766787 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/para/__init__.py
--rw-r--r--   0        0        0      596 2023-04-06 02:13:09.199097 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/para/alignment/__init__.py
--rw-r--r--   0        0        0     1894 2023-04-25 00:03:57.176369 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/para/area/__init__.py
--rw-r--r--   0        0        0      838 2023-04-06 02:13:09.203094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/para/borders/__init__.py
--rw-r--r--   0        0        0      205 2023-04-06 02:13:09.204094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/para/drop_caps/__init__.py
--rw-r--r--   0        0        0      439 2023-04-06 02:13:09.205092 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/para/indent_space/__init__.py
--rw-r--r--   0        0        0      517 2023-04-06 02:13:09.205092 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/para/outline_list/__init__.py
--rw-r--r--   0        0        0      269 2023-04-06 02:13:09.206092 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/para/tabs/__init__.py
--rw-r--r--   0        0        0      406 2023-04-06 02:13:09.207091 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/para/text_flow/__init__.py
--rw-r--r--   0        0        0      536 2023-04-06 02:13:09.207091 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/para/transparency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.773090 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/shape/__init__.py
--rw-r--r--   0        0        0     1828 2023-04-23 13:05:06.193317 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/shape/area/__init__.py
--rw-r--r--   0        0        0      396 2023-04-06 02:13:09.223094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/shape/shadow/__init__.py
--rw-r--r--   0        0        0      584 2023-04-06 02:13:09.223094 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/shape/transparency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.775216 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/table/__init__.py
--rw-r--r--   0        0        0     1099 2023-04-25 00:03:57.178376 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/table/background/__init__.py
--rw-r--r--   0        0        0      769 2023-04-25 00:03:57.179369 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/table/borders/__init__.py
--rw-r--r--   0        0        0      265 2023-04-06 02:13:09.226093 ooo_dev_tools-0.9.6/ooodev/format/writer/direct/table/properties/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.776595 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.777629 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/char/__init__.py
--rw-r--r--   0        0        0     1134 2023-04-06 02:13:09.228094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/char/borders/__init__.py
--rw-r--r--   0        0        0     1683 2023-04-06 02:13:09.229095 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/char/font/__init__.py
--rw-r--r--   0        0        0      346 2023-04-06 02:13:09.230094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/char/highlight/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.779585 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/frame/__init__.py
--rw-r--r--   0        0        0     2421 2023-04-06 02:13:09.231100 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/frame/area/__init__.py
--rw-r--r--   0        0        0     1091 2023-04-06 02:13:09.232094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/frame/borders/__init__.py
--rw-r--r--   0        0        0     1034 2023-04-06 02:13:09.233093 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/frame/options/__init__.py
--rw-r--r--   0        0        0      818 2023-04-06 02:13:09.233093 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/frame/transparency/__init__.py
--rw-r--r--   0        0        0     1911 2023-04-06 02:13:09.234094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/frame/type/__init__.py
--rw-r--r--   0        0        0      805 2023-04-06 02:13:09.235094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/frame/wrap/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.783676 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/__init__.py
--rw-r--r--   0        0        0     2427 2023-04-06 02:13:48.600068 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/area/__init__.py
--rw-r--r--   0        0        0     1105 2023-04-06 02:13:09.236092 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/borders/__init__.py
--rw-r--r--   0        0        0      321 2023-04-06 02:13:09.237093 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/footer/__init__.py
--rw-r--r--   0        0        0     2535 2023-04-06 02:13:09.237093 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/footer/area/__init__.py
--rw-r--r--   0        0        0     1147 2023-04-06 02:13:09.238094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/footer/borders/__init__.py
--rw-r--r--   0        0        0      995 2023-04-06 02:13:09.239092 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/footer/transparency/__init__.py
--rw-r--r--   0        0        0      321 2023-04-06 02:13:09.239092 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/header/__init__.py
--rw-r--r--   0        0        0     2535 2023-04-06 02:13:09.240096 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/header/area/__init__.py
--rw-r--r--   0        0        0     1148 2023-04-06 02:13:09.241093 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/header/borders/__init__.py
--rw-r--r--   0        0        0      995 2023-04-06 02:13:09.241093 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/header/transparency/__init__.py
--rw-r--r--   0        0        0     1293 2023-04-06 02:13:09.242093 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/page/__init__.py
--rw-r--r--   0        0        0     3526 2023-04-06 02:13:09.243093 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/page_style_base.py
--rw-r--r--   0        0        0     3939 2023-04-06 02:13:09.246092 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/page_style_base_multi.py
--rw-r--r--   0        0        0      958 2023-04-06 02:13:09.247094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/transparency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 18:09:12.792731 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/__init__.py
--rw-r--r--   0        0        0      794 2023-04-06 02:13:09.249093 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/alignment/__init__.py
--rw-r--r--   0        0        0     2297 2023-04-06 02:13:09.250094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/area/__init__.py
--rw-r--r--   0        0        0     1347 2023-04-06 02:13:09.250094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/borders/__init__.py
--rw-r--r--   0        0        0      402 2023-04-06 02:13:09.251094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/drop_caps/__init__.py
--rw-r--r--   0        0        0     1685 2023-04-06 02:13:09.252093 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/font/__init__.py
--rw-r--r--   0        0        0      319 2023-04-06 02:13:09.252093 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/highlight/__init__.py
--rw-r--r--   0        0        0      880 2023-04-06 02:13:09.253094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/indent_space/__init__.py
--rw-r--r--   0        0        0      955 2023-04-06 02:13:09.255094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/outline_list/__init__.py
--rw-r--r--   0        0        0      446 2023-04-06 02:13:09.257094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/tabs/__init__.py
--rw-r--r--   0        0        0      855 2023-04-06 02:13:09.257094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/text_flow/__init__.py
--rw-r--r--   0        0        0      839 2023-04-06 02:13:09.258094 ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/transparency/__init__.py
--rw-r--r--   0        0        0      750 2023-04-06 02:13:09.300094 ooo_dev_tools-0.9.6/ooodev/format/writer/style/__init__.py
--rw-r--r--   0        0        0      110 2023-04-02 18:09:12.799670 ooo_dev_tools-0.9.6/ooodev/format/writer/style/bullet_list/__init__.py
--rw-r--r--   0        0        0     4599 2023-04-23 13:05:06.194315 ooo_dev_tools-0.9.6/ooodev/format/writer/style/bullet_list/bullet_list.py
--rw-r--r--   0        0        0      107 2023-04-02 18:09:12.800581 ooo_dev_tools-0.9.6/ooodev/format/writer/style/char/__init__.py
--rw-r--r--   0        0        0     7058 2023-04-23 13:05:06.195315 ooo_dev_tools-0.9.6/ooodev/format/writer/style/char/char.py
--rw-r--r--   0        0        0       60 2023-04-02 18:09:12.802395 ooo_dev_tools-0.9.6/ooodev/format/writer/style/char/kind/__init__.py
--rw-r--r--   0        0        0     1135 2023-04-06 02:13:09.303093 ooo_dev_tools-0.9.6/ooodev/format/writer/style/char/kind/style_char_kind.py
--rw-r--r--   0        0        0       97 2023-04-06 02:13:09.304092 ooo_dev_tools-0.9.6/ooodev/format/writer/style/frame/__init__.py
--rw-r--r--   0        0        0     3704 2023-04-06 02:13:48.603067 ooo_dev_tools-0.9.6/ooodev/format/writer/style/frame/frame.py
--rw-r--r--   0        0        0      353 2023-04-06 02:13:09.305109 ooo_dev_tools-0.9.6/ooodev/format/writer/style/frame/style_frame_kind.py
--rw-r--r--   0        0        0       60 2023-04-02 18:09:12.804657 ooo_dev_tools-0.9.6/ooodev/format/writer/style/lst/__init__.py
--rw-r--r--   0        0        0      791 2023-04-06 02:13:09.306094 ooo_dev_tools-0.9.6/ooodev/format/writer/style/lst/style_list_kind.py
--rw-r--r--   0        0        0      115 2023-04-06 02:13:09.307094 ooo_dev_tools-0.9.6/ooodev/format/writer/style/page/__init__.py
--rw-r--r--   0        0        0       79 2023-04-06 02:13:09.308096 ooo_dev_tools-0.9.6/ooodev/format/writer/style/page/kind/__init__.py
--rw-r--r--   0        0        0      412 2023-04-06 02:13:09.309094 ooo_dev_tools-0.9.6/ooodev/format/writer/style/page/kind/writer_style_page_kind.py
--rw-r--r--   0        0        0     4711 2023-04-06 02:13:48.605068 ooo_dev_tools-0.9.6/ooodev/format/writer/style/page/page.py
--rw-r--r--   0        0        0       91 2023-04-03 22:12:05.347628 ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/__init__.py
--rw-r--r--   0        0        0      579 2023-04-02 18:09:12.808625 ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/__init__.py
--rw-r--r--   0        0        0      335 2023-04-06 02:13:09.310097 ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_chapter_kind.py
--rw-r--r--   0        0        0      260 2023-04-06 02:13:09.311093 ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_para_cond_kind.py
--rw-r--r--   0        0        0     1225 2023-04-06 02:13:09.312094 ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_para_html_kind.py
--rw-r--r--   0        0        0     2105 2023-04-06 02:13:09.312094 ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_para_index_kind.py
--rw-r--r--   0        0        0     4274 2023-04-06 02:13:09.313095 ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_para_kind.py
--rw-r--r--   0        0        0     2492 2023-04-06 02:13:09.314095 ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_para_list_kind.py
--rw-r--r--   0        0        0     1139 2023-04-06 02:13:09.316093 ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_para_special_kind.py
--rw-r--r--   0        0        0     1278 2023-04-06 02:13:09.317099 ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_para_text_kind.py
--rw-r--r--   0        0        0    11566 2023-04-23 13:05:06.196317 ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/para.py
--rw-r--r--   0        0        0      218 2022-11-22 00:28:23.283709 ooo_dev_tools-0.9.6/ooodev/formatters/__init__.py
--rw-r--r--   0        0        0     1185 2022-11-22 00:28:23.284709 ooo_dev_tools-0.9.6/ooodev/formatters/format_list_item.py
--rw-r--r--   0        0        0     1101 2022-11-22 00:28:23.284709 ooo_dev_tools-0.9.6/ooodev/formatters/format_string.py
--rw-r--r--   0        0        0     2540 2022-11-22 00:28:23.285710 ooo_dev_tools-0.9.6/ooodev/formatters/format_table_item.py
--rw-r--r--   0        0        0     3182 2022-11-22 00:28:23.285710 ooo_dev_tools-0.9.6/ooodev/formatters/formatter_list.py
--rw-r--r--   0        0        0    10394 2023-04-06 02:13:09.319094 ooo_dev_tools-0.9.6/ooodev/formatters/formatter_table.py
--rw-r--r--   0        0        0      130 2022-11-22 00:28:23.287709 ooo_dev_tools-0.9.6/ooodev/formatters/only_ignore_kind.py
--rw-r--r--   0        0        0      196 2022-11-22 00:28:23.287709 ooo_dev_tools-0.9.6/ooodev/formatters/string_kind.py
--rw-r--r--   0        0        0      720 2022-11-22 00:28:23.288717 ooo_dev_tools-0.9.6/ooodev/formatters/table_item_kind.py
--rw-r--r--   0        0        0     4482 2022-11-22 00:28:23.289713 ooo_dev_tools-0.9.6/ooodev/formatters/table_item_processer.py
--rw-r--r--   0        0        0      336 2022-11-22 00:28:23.290711 ooo_dev_tools-0.9.6/ooodev/formatters/table_rule_kind.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.797175 ooo_dev_tools-0.9.6/ooodev/lazy/__init__.py
--rw-r--r--   0        0        0     1551 2022-07-24 03:34:34.541590 ooo_dev_tools-0.9.6/ooodev/lazy/lazy_import.py
--rw-r--r--   0        0        0        0 2022-06-09 05:52:04.176192 ooo_dev_tools-0.9.6/ooodev/listeners/__init__.py
--rw-r--r--   0        0        0     1130 2022-07-20 01:40:32.577461 ooo_dev_tools-0.9.6/ooodev/listeners/x_event_adapter.py
--rw-r--r--   0        0        0     1402 2022-07-20 01:40:32.578458 ooo_dev_tools-0.9.6/ooodev/listeners/x_modify_adapter.py
--rw-r--r--   0        0        0     1355 2022-08-23 05:01:45.222321 ooo_dev_tools-0.9.6/ooodev/listeners/x_selection_change_adapter.py
--rw-r--r--   0        0        0     1827 2022-07-20 01:40:32.580453 ooo_dev_tools-0.9.6/ooodev/listeners/x_terminate_adapter.py
--rw-r--r--   0        0        0     2034 2022-07-20 01:40:32.581450 ooo_dev_tools-0.9.6/ooodev/listeners/x_top_window_adapter.py
--rw-r--r--   0        0        0        0 2022-06-09 05:52:04.177777 ooo_dev_tools-0.9.6/ooodev/meta/__init__.py
--rw-r--r--   0        0        0      518 2023-04-02 18:09:12.815585 ooo_dev_tools-0.9.6/ooodev/meta/class_property_readonly.py
--rw-r--r--   0        0        0      545 2023-04-02 18:09:12.820755 ooo_dev_tools-0.9.6/ooodev/meta/deleted_attrib.py
--rw-r--r--   0        0        0     1617 2023-04-02 18:09:12.821833 ooo_dev_tools-0.9.6/ooodev/meta/deleted_enum_meta.py
--rw-r--r--   0        0        0      915 2023-04-02 18:09:12.822581 ooo_dev_tools-0.9.6/ooodev/meta/disabled_method.py
--rw-r--r--   0        0        0      241 2022-07-14 20:40:23.800284 ooo_dev_tools-0.9.6/ooodev/meta/singleton.py
--rw-r--r--   0        0        0     2135 2023-01-10 14:23:45.008570 ooo_dev_tools-0.9.6/ooodev/meta/static_meta.py
--rw-r--r--   0        0        0      518 2023-04-02 18:09:12.822581 ooo_dev_tools-0.9.6/ooodev/meta/static_prop.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.801281 ooo_dev_tools-0.9.6/ooodev/mock/__init__.py
--rw-r--r--   0        0        0      559 2022-07-14 20:40:23.801281 ooo_dev_tools-0.9.6/ooodev/mock/mock_g.py
--rw-r--r--   0        0        0      579 2022-10-04 00:14:04.239070 ooo_dev_tools-0.9.6/ooodev/mock/unohelper.py
--rw-r--r--   0        0        0        0 2022-06-09 05:51:34.370860 ooo_dev_tools-0.9.6/ooodev/office/__init__.py
--rw-r--r--   0        0        0   265485 2023-04-23 13:05:06.199317 ooo_dev_tools-0.9.6/ooodev/office/calc.py
--rw-r--r--   0        0        0    45621 2023-04-06 02:13:09.324093 ooo_dev_tools-0.9.6/ooodev/office/chart.py
--rw-r--r--   0        0        0   114364 2023-04-23 13:05:06.202317 ooo_dev_tools-0.9.6/ooodev/office/chart2.py
--rw-r--r--   0        0        0   135614 2023-04-06 02:13:48.632065 ooo_dev_tools-0.9.6/ooodev/office/draw.py
--rw-r--r--   0        0        0   150899 2023-04-25 00:03:57.182369 ooo_dev_tools-0.9.6/ooodev/office/write.py
--rw-r--r--   0        0        0        0 2022-07-14 20:40:23.805270 ooo_dev_tools-0.9.6/ooodev/proto/__init__.py
--rw-r--r--   0        0        0      626 2023-04-06 02:13:09.329093 ooo_dev_tools-0.9.6/ooodev/proto/dispatch_shape.py
--rw-r--r--   0        0        0     1453 2023-04-06 02:13:09.329093 ooo_dev_tools-0.9.6/ooodev/proto/event_observer.py
--rw-r--r--   0        0        0      450 2023-04-06 02:13:09.330101 ooo_dev_tools-0.9.6/ooodev/proto/size_obj.py
--rw-r--r--   0        0        0     2394 2023-04-06 02:13:09.331094 ooo_dev_tools-0.9.6/ooodev/proto/style_obj.py
--rw-r--r--   0        0        0      636 2023-04-06 02:13:48.635066 ooo_dev_tools-0.9.6/ooodev/theme/__init__.py
--rw-r--r--   0        0        0     1604 2023-04-07 18:06:32.211989 ooo_dev_tools-0.9.6/ooodev/theme/theme.py
--rw-r--r--   0        0        0     2212 2023-04-06 02:13:48.638067 ooo_dev_tools-0.9.6/ooodev/theme/theme_basic.py
--rw-r--r--   0        0        0     4152 2023-04-06 02:13:48.639065 ooo_dev_tools-0.9.6/ooodev/theme/theme_calc.py
--rw-r--r--   0        0        0      865 2023-04-06 02:13:48.640067 ooo_dev_tools-0.9.6/ooodev/theme/theme_draw.py
--rw-r--r--   0        0        0     4342 2023-04-06 02:13:48.640067 ooo_dev_tools-0.9.6/ooodev/theme/theme_general.py
--rw-r--r--   0        0        0     1416 2023-04-06 02:13:48.641076 ooo_dev_tools-0.9.6/ooodev/theme/theme_html.py
--rw-r--r--   0        0        0     3982 2023-04-06 02:13:48.641076 ooo_dev_tools-0.9.6/ooodev/theme/theme_rpt_builder.py
--rw-r--r--   0        0        0     2215 2023-04-06 02:13:48.642067 ooo_dev_tools-0.9.6/ooodev/theme/theme_sql.py
--rw-r--r--   0        0        0     4975 2023-04-06 02:13:48.642067 ooo_dev_tools-0.9.6/ooodev/theme/theme_text_doc.py
--rw-r--r--   0        0        0      820 2023-04-23 13:05:06.206317 ooo_dev_tools-0.9.6/ooodev/units/__init__.py
--rw-r--r--   0        0        0     5979 2023-04-23 13:05:06.206317 ooo_dev_tools-0.9.6/ooodev/units/unit_cm.py
--rw-r--r--   0        0        0     8844 2023-04-06 02:13:09.334092 ooo_dev_tools-0.9.6/ooodev/units/unit_convert.py
--rw-r--r--   0        0        0     5352 2023-04-23 13:05:06.208316 ooo_dev_tools-0.9.6/ooodev/units/unit_inch.py
--rw-r--r--   0        0        0     5394 2023-04-23 13:05:06.209317 ooo_dev_tools-0.9.6/ooodev/units/unit_inch10.py
--rw-r--r--   0        0        0     5447 2023-04-23 13:05:06.210316 ooo_dev_tools-0.9.6/ooodev/units/unit_inch100.py
--rw-r--r--   0        0        0     6082 2023-04-23 13:05:06.211316 ooo_dev_tools-0.9.6/ooodev/units/unit_inch1000.py
--rw-r--r--   0        0        0     5897 2023-04-23 13:05:06.212316 ooo_dev_tools-0.9.6/ooodev/units/unit_mm.py
--rw-r--r--   0        0        0     6131 2023-04-23 13:05:06.213315 ooo_dev_tools-0.9.6/ooodev/units/unit_mm10.py
--rw-r--r--   0        0        0     6677 2023-04-23 13:05:06.214316 ooo_dev_tools-0.9.6/ooodev/units/unit_mm100.py
--rw-r--r--   0        0        0     1329 2023-04-06 02:13:48.644066 ooo_dev_tools-0.9.6/ooodev/units/unit_obj.py
--rw-r--r--   0        0        0     5700 2023-04-23 13:05:06.215315 ooo_dev_tools-0.9.6/ooodev/units/unit_pt.py
--rw-r--r--   0        0        0     5960 2023-04-23 13:05:06.216316 ooo_dev_tools-0.9.6/ooodev/units/unit_px.py
--rw-r--r--   0        0        0     1907 2022-07-14 20:40:23.806682 ooo_dev_tools-0.9.6/ooodev/utils/__init__.py
--rw-r--r--   0        0        0    26819 2023-04-06 02:13:48.645065 ooo_dev_tools-0.9.6/ooodev/utils/color.py
--rw-r--r--   0        0        0        0 2022-10-27 15:27:12.052996 ooo_dev_tools-0.9.6/ooodev/utils/data_type/__init__.py
--rw-r--r--   0        0        0     2758 2023-04-02 18:09:12.852582 ooo_dev_tools-0.9.6/ooodev/utils/data_type/angle.py
--rw-r--r--   0        0        0     3820 2022-12-17 01:13:14.728078 ooo_dev_tools-0.9.6/ooodev/utils/data_type/base_float_value.py
--rw-r--r--   0        0        0     3785 2023-04-02 18:09:12.853581 ooo_dev_tools-0.9.6/ooodev/utils/data_type/base_int_value.py
--rw-r--r--   0        0        0     1280 2023-04-02 18:09:12.874577 ooo_dev_tools-0.9.6/ooodev/utils/data_type/byte.py
--rw-r--r--   0        0        0     1298 2023-04-02 18:09:12.875872 ooo_dev_tools-0.9.6/ooodev/utils/data_type/byte_signed.py
--rw-r--r--   0        0        0    14993 2023-04-02 18:09:12.876578 ooo_dev_tools-0.9.6/ooodev/utils/data_type/cell_obj.py
--rw-r--r--   0        0        0     3298 2023-04-02 18:09:12.877797 ooo_dev_tools-0.9.6/ooodev/utils/data_type/cell_values.py
--rw-r--r--   0        0        0    10497 2023-04-06 02:13:09.375094 ooo_dev_tools-0.9.6/ooodev/utils/data_type/col_obj.py
--rw-r--r--   0        0        0      522 2023-04-02 18:09:12.879580 ooo_dev_tools-0.9.6/ooodev/utils/data_type/color_range.py
--rw-r--r--   0        0        0      195 2022-11-13 02:25:58.188785 ooo_dev_tools-0.9.6/ooodev/utils/data_type/dialog_title.py
--rw-r--r--   0        0        0     1020 2023-04-02 18:09:12.880576 ooo_dev_tools-0.9.6/ooodev/utils/data_type/image_offset.py
--rw-r--r--   0        0        0     1290 2023-04-02 18:09:12.882575 ooo_dev_tools-0.9.6/ooodev/utils/data_type/intensity.py
--rw-r--r--   0        0        0      880 2023-04-06 02:13:09.376093 ooo_dev_tools-0.9.6/ooodev/utils/data_type/intensity_range.py
--rw-r--r--   0        0        0      209 2023-04-02 18:09:12.884666 ooo_dev_tools-0.9.6/ooodev/utils/data_type/offset.py
--rw-r--r--   0        0        0      431 2023-04-02 18:09:12.884666 ooo_dev_tools-0.9.6/ooodev/utils/data_type/point.py
--rw-r--r--   0        0        0      482 2023-04-02 18:09:12.885575 ooo_dev_tools-0.9.6/ooodev/utils/data_type/point_positive.py
--rw-r--r--   0        0        0     1282 2023-04-02 18:09:12.886577 ooo_dev_tools-0.9.6/ooodev/utils/data_type/poly_sides.py
--rw-r--r--   0        0        0    22190 2023-04-06 02:13:09.377092 ooo_dev_tools-0.9.6/ooodev/utils/data_type/range_obj.py
--rw-r--r--   0        0        0    15997 2023-04-06 02:13:09.402093 ooo_dev_tools-0.9.6/ooodev/utils/data_type/range_values.py
--rw-r--r--   0        0        0     7314 2023-04-02 18:09:12.888579 ooo_dev_tools-0.9.6/ooodev/utils/data_type/row_obj.py
--rw-r--r--   0        0        0     1993 2023-04-06 02:13:09.403093 ooo_dev_tools-0.9.6/ooodev/utils/data_type/size.py
--rw-r--r--   0        0        0     3154 2023-04-06 02:13:09.404094 ooo_dev_tools-0.9.6/ooodev/utils/data_type/size_mm.py
--rw-r--r--   0        0        0     1126 2023-04-02 18:09:12.890576 ooo_dev_tools-0.9.6/ooodev/utils/data_type/width_height_fraction.py
--rw-r--r--   0        0        0      935 2023-04-02 18:09:12.891577 ooo_dev_tools-0.9.6/ooodev/utils/data_type/width_height_percent.py
--rw-r--r--   0        0        0      270 2022-11-13 02:25:58.189784 ooo_dev_tools-0.9.6/ooodev/utils/data_type/window_title.py
--rw-r--r--   0        0        0     5657 2022-12-10 17:01:36.559035 ooo_dev_tools-0.9.6/ooodev/utils/date_time_util.py
--rw-r--r--   0        0        0        0 2022-10-27 15:27:12.055992 ooo_dev_tools-0.9.6/ooodev/utils/decorator/__init__.py
--rw-r--r--   0        0        0     2737 2023-04-23 13:05:06.217315 ooo_dev_tools-0.9.6/ooodev/utils/decorator/enforce.py
--rw-r--r--   0        0        0    24793 2023-04-06 02:13:09.404094 ooo_dev_tools-0.9.6/ooodev/utils/dialogs.py
--rw-r--r--   0        0        0        0 2022-10-27 15:27:12.056992 ooo_dev_tools-0.9.6/ooodev/utils/dispatch/__init__.py
--rw-r--r--   0        0        0     3178 2022-10-27 15:27:12.057993 ooo_dev_tools-0.9.6/ooodev/utils/dispatch/draw_drawing_dispatch.py
--rw-r--r--   0        0        0     2806 2022-10-27 15:27:12.058992 ooo_dev_tools-0.9.6/ooodev/utils/dispatch/draw_view_dispatch.py
--rw-r--r--   0        0        0     3180 2022-10-27 15:27:12.059993 ooo_dev_tools-0.9.6/ooodev/utils/dispatch/global_edit_dispatch.py
--rw-r--r--   0        0        0     9772 2022-10-27 15:27:12.059993 ooo_dev_tools-0.9.6/ooodev/utils/dispatch/global_format_dispatch.py
--rw-r--r--   0        0        0     2911 2022-10-27 15:27:12.060992 ooo_dev_tools-0.9.6/ooodev/utils/dispatch/global_view_dispatch.py
--rw-r--r--   0        0        0    11843 2022-11-08 11:09:51.358105 ooo_dev_tools-0.9.6/ooodev/utils/dispatch/shape_dispatch_kind.py
--rw-r--r--   0        0        0     1562 2022-07-24 03:34:47.720953 ooo_dev_tools-0.9.6/ooodev/utils/enum_helper.py
--rw-r--r--   0        0        0    21457 2022-11-30 23:26:32.117139 ooo_dev_tools-0.9.6/ooodev/utils/file_io.py
--rw-r--r--   0        0        0    44086 2023-04-06 02:13:48.646066 ooo_dev_tools-0.9.6/ooodev/utils/forms.py
--rw-r--r--   0        0        0    21957 2023-04-02 18:09:12.895589 ooo_dev_tools-0.9.6/ooodev/utils/gallery.py
--rw-r--r--   0        0        0     7499 2023-04-23 13:05:06.218316 ooo_dev_tools-0.9.6/ooodev/utils/gen_util.py
--rw-r--r--   0        0        0    58911 2023-04-06 02:13:09.406094 ooo_dev_tools-0.9.6/ooodev/utils/gui.py
--rw-r--r--   0        0        0     2062 2022-07-14 20:40:23.810268 ooo_dev_tools-0.9.6/ooodev/utils/image_transferable.py
--rw-r--r--   0        0        0     3745 2022-07-24 03:34:34.555553 ooo_dev_tools-0.9.6/ooodev/utils/images.py
--rw-r--r--   0        0        0    15354 2023-04-06 02:13:48.647065 ooo_dev_tools-0.9.6/ooodev/utils/images_lo.py
--rw-r--r--   0        0        0    79006 2023-04-23 13:05:06.220317 ooo_dev_tools-0.9.6/ooodev/utils/info.py
--rw-r--r--   0        0        0        0 2022-10-27 15:27:12.066994 ooo_dev_tools-0.9.6/ooodev/utils/kind/__init__.py
--rw-r--r--   0        0        0      658 2022-11-05 19:28:56.359598 ooo_dev_tools-0.9.6/ooodev/utils/kind/axis_kind.py
--rw-r--r--   0        0        0     2943 2022-11-05 19:28:56.360598 ooo_dev_tools-0.9.6/ooodev/utils/kind/chart2_data_role_kind.py
--rw-r--r--   0        0        0     7423 2022-12-17 01:13:14.740079 ooo_dev_tools-0.9.6/ooodev/utils/kind/chart2_types.py
--rw-r--r--   0        0        0     1061 2022-11-05 19:28:56.361599 ooo_dev_tools-0.9.6/ooodev/utils/kind/chart_diagram_kind.py
--rw-r--r--   0        0        0     1979 2022-11-05 19:28:56.361599 ooo_dev_tools-0.9.6/ooodev/utils/kind/curve_kind.py
--rw-r--r--   0        0        0      893 2022-11-05 19:28:56.362600 ooo_dev_tools-0.9.6/ooodev/utils/kind/data_point_label_type_kind.py
--rw-r--r--   0        0        0      922 2022-11-05 19:28:56.363598 ooo_dev_tools-0.9.6/ooodev/utils/kind/data_point_lable_placement_kind.py
--rw-r--r--   0        0        0     1921 2022-11-05 19:28:56.364600 ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_bitmap_kind.py
--rw-r--r--   0        0        0     1510 2022-11-05 19:28:56.364600 ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_gradient_kind.py
--rw-r--r--   0        0        0     1781 2022-11-05 19:28:56.365599 ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_hatching_kind.py
--rw-r--r--   0        0        0     1053 2022-11-05 19:28:56.366599 ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_layer_kind.py
--rw-r--r--   0        0        0     1343 2022-11-05 19:28:56.367602 ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_name_space_kind.py
--rw-r--r--   0        0        0     2298 2022-11-05 19:28:56.368600 ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_shape_kind.py
--rw-r--r--   0        0        0     1123 2022-11-05 19:28:56.369599 ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_slide_show_kind.py
--rw-r--r--   0        0        0     2482 2022-11-05 19:28:56.370602 ooo_dev_tools-0.9.6/ooodev/utils/kind/form_component_kind.py
--rw-r--r--   0        0        0     1778 2022-11-05 19:28:56.371600 ooo_dev_tools-0.9.6/ooodev/utils/kind/form_control_kind.py
--rw-r--r--   0        0        0     1309 2022-11-05 19:28:56.371600 ooo_dev_tools-0.9.6/ooodev/utils/kind/gallery_kind.py
--rw-r--r--   0        0        0      945 2022-11-05 19:28:56.372599 ooo_dev_tools-0.9.6/ooodev/utils/kind/gallery_search_by_kind.py
--rw-r--r--   0        0        0      812 2022-11-05 19:28:56.373599 ooo_dev_tools-0.9.6/ooodev/utils/kind/glue_points_kind.py
--rw-r--r--   0        0        0     2878 2022-11-08 11:08:31.782891 ooo_dev_tools-0.9.6/ooodev/utils/kind/graphic_arrow_style_kind.py
--rw-r--r--   0        0        0     2131 2022-11-05 19:28:56.374601 ooo_dev_tools-0.9.6/ooodev/utils/kind/graphic_style_kind.py
--rw-r--r--   0        0        0     1526 2022-11-30 23:26:32.119139 ooo_dev_tools-0.9.6/ooodev/utils/kind/info_paths_kind.py
--rw-r--r--   0        0        0      209 2022-10-27 15:27:12.079996 ooo_dev_tools-0.9.6/ooodev/utils/kind/kind_base.py
--rw-r--r--   0        0        0     2389 2022-11-13 02:25:58.191785 ooo_dev_tools-0.9.6/ooodev/utils/kind/kind_helper.py
--rw-r--r--   0        0        0     1260 2022-11-05 19:28:56.376599 ooo_dev_tools-0.9.6/ooodev/utils/kind/line_style_name_kind.py
--rw-r--r--   0        0        0     2202 2022-11-05 19:28:56.377600 ooo_dev_tools-0.9.6/ooodev/utils/kind/presentation_kind.py
--rw-r--r--   0        0        0     1898 2022-11-13 02:25:58.191785 ooo_dev_tools-0.9.6/ooodev/utils/kind/presentation_layout_kind.py
--rw-r--r--   0        0        0     1146 2022-11-05 19:28:56.377600 ooo_dev_tools-0.9.6/ooodev/utils/kind/search_match_kind.py
--rw-r--r--   0        0        0     1183 2023-04-23 13:05:06.221317 ooo_dev_tools-0.9.6/ooodev/utils/kind/shape_base_point_kind.py
--rw-r--r--   0        0        0      820 2022-11-05 19:28:56.378600 ooo_dev_tools-0.9.6/ooodev/utils/kind/shape_comb_kind.py
--rw-r--r--   0        0        0    99082 2023-04-23 13:05:06.222317 ooo_dev_tools-0.9.6/ooodev/utils/lo.py
--rw-r--r--   0        0        0     2783 2022-07-24 03:34:34.561536 ooo_dev_tools-0.9.6/ooodev/utils/lo_util.py
--rw-r--r--   0        0        0     8437 2022-11-25 03:43:11.801371 ooo_dev_tools-0.9.6/ooodev/utils/paths.py
--rw-r--r--   0        0        0    57557 2023-04-23 13:05:06.224316 ooo_dev_tools-0.9.6/ooodev/utils/props.py
--rw-r--r--   0        0        0     1896 2022-07-20 01:40:32.607380 ooo_dev_tools-0.9.6/ooodev/utils/script_context.py
--rw-r--r--   0        0        0    25545 2023-04-23 13:05:06.227316 ooo_dev_tools-0.9.6/ooodev/utils/selection.py
--rw-r--r--   0        0        0     6400 2022-10-31 22:59:24.504932 ooo_dev_tools-0.9.6/ooodev/utils/session.py
--rw-r--r--   0        0        0      727 2022-10-29 21:44:16.952005 ooo_dev_tools-0.9.6/ooodev/utils/sys_info.py
--rw-r--r--   0        0        0    26396 2023-04-02 18:09:12.907574 ooo_dev_tools-0.9.6/ooodev/utils/table_helper.py
--rw-r--r--   0        0        0     2023 2022-07-14 20:40:23.817443 ooo_dev_tools-0.9.6/ooodev/utils/text_transferable.py
--rw-r--r--   0        0        0     1453 2022-07-24 03:34:34.568523 ooo_dev_tools-0.9.6/ooodev/utils/type_var.py
--rw-r--r--   0        0        0     3478 2022-07-14 20:40:23.818235 ooo_dev_tools-0.9.6/ooodev/utils/uno_const.py
--rw-r--r--   0        0        0     6513 2022-10-04 00:14:04.247070 ooo_dev_tools-0.9.6/ooodev/utils/uno_enum.py
--rw-r--r--   0        0        0      562 2022-10-27 15:27:12.084993 ooo_dev_tools-0.9.6/ooodev/utils/validation.py
--rw-r--r--   0        0        0    11180 2022-11-25 03:43:11.802373 ooo_dev_tools-0.9.6/ooodev/utils/view_state.py
--rw-r--r--   0        0        0    18910 2022-07-24 03:34:47.735913 ooo_dev_tools-0.9.6/ooodev/utils/xml_util.py
--rw-r--r--   0        0        0        0 2022-07-16 02:19:46.806983 ooo_dev_tools-0.9.6/ooodev/wrapper/__init__.py
--rw-r--r--   0        0        0      929 2022-08-23 05:01:45.230317 ooo_dev_tools-0.9.6/ooodev/wrapper/break_context.py
--rw-r--r--   0        0        0     2366 2023-04-25 00:03:57.183366 ooo_dev_tools-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     5220 2023-04-23 13:05:05.060319 ooo_dev_tools-0.9.6/README.rst
--rw-r--r--   0        0        0     6770 1970-01-01 00:00:00.000000 ooo_dev_tools-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0    10174 2022-06-09 05:52:04.135315 ooo_dev_tools-0.9.7/LICENSE
+-rw-r--r--   0        0        0      272 2023-04-27 15:20:03.725631 ooo_dev_tools-0.9.7/ooodev/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-29 00:27:48.235332 ooo_dev_tools-0.9.7/ooodev/adapter/__init__.py
+-rw-r--r--   0        0        0     1806 2022-11-29 00:27:48.236329 ooo_dev_tools-0.9.7/ooodev/adapter/adapter_base.py
+-rw-r--r--   0        0        0        0 2022-11-29 00:27:48.236329 ooo_dev_tools-0.9.7/ooodev/adapter/awt/__init__.py
+-rw-r--r--   0        0        0     3451 2022-12-03 04:37:37.329802 ooo_dev_tools-0.9.7/ooodev/adapter/awt/top_window_listener.py
+-rw-r--r--   0        0        0        0 2022-11-29 00:27:48.238329 ooo_dev_tools-0.9.7/ooodev/adapter/frame/__init__.py
+-rw-r--r--   0        0        0     2711 2022-12-03 04:37:37.330805 ooo_dev_tools-0.9.7/ooodev/adapter/frame/terminate_listener.py
+-rw-r--r--   0        0        0        0 2022-11-29 00:27:48.239328 ooo_dev_tools-0.9.7/ooodev/adapter/lang/__init__.py
+-rw-r--r--   0        0        0     1543 2022-12-03 04:37:37.330805 ooo_dev_tools-0.9.7/ooodev/adapter/lang/event_listener.py
+-rw-r--r--   0        0        0        0 2022-11-29 00:27:48.240329 ooo_dev_tools-0.9.7/ooodev/adapter/util/__init__.py
+-rw-r--r--   0        0        0     2336 2022-12-03 04:37:37.331804 ooo_dev_tools-0.9.7/ooodev/adapter/util/modify_listener.py
+-rw-r--r--   0        0        0        0 2022-11-29 00:27:48.241329 ooo_dev_tools-0.9.7/ooodev/adapter/view/__init__.py
+-rw-r--r--   0        0        0     2628 2023-04-06 02:13:08.626094 ooo_dev_tools-0.9.7/ooodev/adapter/view/selection_change_listener.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.785323 ooo_dev_tools-0.9.7/ooodev/cfg/__init__.py
+-rw-r--r--   0        0        0       89 2022-10-27 15:27:12.042995 ooo_dev_tools-0.9.7/ooodev/cfg/config.json
+-rw-r--r--   0        0        0     2012 2022-10-27 15:27:12.042995 ooo_dev_tools-0.9.7/ooodev/cfg/config.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.786382 ooo_dev_tools-0.9.7/ooodev/conn/__init__.py
+-rw-r--r--   0        0        0     5699 2022-07-14 20:40:23.787320 ooo_dev_tools-0.9.7/ooodev/conn/cache.py
+-rw-r--r--   0        0        0    18466 2023-04-06 02:13:08.627093 ooo_dev_tools-0.9.7/ooodev/conn/connect.py
+-rw-r--r--   0        0        0     6968 2022-12-20 23:59:58.431481 ooo_dev_tools-0.9.7/ooodev/conn/connectors.py
+-rw-r--r--   0        0        0        0 2022-10-27 15:27:12.043993 ooo_dev_tools-0.9.7/ooodev/dialog/__init__.py
+-rw-r--r--   0        0        0     3161 2022-11-05 19:29:24.377395 ooo_dev_tools-0.9.7/ooodev/dialog/input.py
+-rw-r--r--   0        0        0     2297 2022-11-13 02:25:58.183785 ooo_dev_tools-0.9.7/ooodev/dialog/msgbox.py
+-rw-r--r--   0        0        0     2019 2022-10-27 15:27:12.045993 ooo_dev_tools-0.9.7/ooodev/dialog/tk_input.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.789060 ooo_dev_tools-0.9.7/ooodev/events/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.789342 ooo_dev_tools-0.9.7/ooodev/events/args/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.789342 ooo_dev_tools-0.9.7/ooodev/events/args/calc/__init__.py
+-rw-r--r--   0        0        0     1371 2023-04-02 18:09:12.324621 ooo_dev_tools-0.9.7/ooodev/events/args/calc/cell_args.py
+-rw-r--r--   0        0        0     1461 2023-04-02 18:09:12.325621 ooo_dev_tools-0.9.7/ooodev/events/args/calc/cell_cancel_args.py
+-rw-r--r--   0        0        0     1590 2023-04-02 18:09:12.326621 ooo_dev_tools-0.9.7/ooodev/events/args/calc/sheet_args.py
+-rw-r--r--   0        0        0     1575 2023-04-02 18:09:12.327740 ooo_dev_tools-0.9.7/ooodev/events/args/calc/sheet_cancel_args.py
+-rw-r--r--   0        0        0     1451 2023-04-02 18:09:12.328623 ooo_dev_tools-0.9.7/ooodev/events/args/cancel_event_args.py
+-rw-r--r--   0        0        0     1163 2023-04-02 18:09:12.328745 ooo_dev_tools-0.9.7/ooodev/events/args/dispatch_args.py
+-rw-r--r--   0        0        0     1450 2023-04-02 18:09:12.329620 ooo_dev_tools-0.9.7/ooodev/events/args/dispatch_cancel_args.py
+-rw-r--r--   0        0        0     4051 2023-04-06 02:13:08.628097 ooo_dev_tools-0.9.7/ooodev/events/args/event_args.py
+-rw-r--r--   0        0        0      640 2022-11-29 00:27:48.243330 ooo_dev_tools-0.9.7/ooodev/events/args/generic_args.py
+-rw-r--r--   0        0        0     1366 2023-04-02 18:09:12.330620 ooo_dev_tools-0.9.7/ooodev/events/args/key_val_args.py
+-rw-r--r--   0        0        0     1608 2023-04-02 18:09:12.331622 ooo_dev_tools-0.9.7/ooodev/events/args/key_val_cancel_args.py
+-rw-r--r--   0        0        0     5995 2023-04-02 18:09:12.332622 ooo_dev_tools-0.9.7/ooodev/events/calc_named_event.py
+-rw-r--r--   0        0        0      863 2023-04-23 13:05:05.528317 ooo_dev_tools-0.9.7/ooodev/events/chart2_named_event.py
+-rw-r--r--   0        0        0      391 2022-11-29 00:27:48.244327 ooo_dev_tools-0.9.7/ooodev/events/command.py
+-rw-r--r--   0        0        0      312 2023-04-02 18:09:12.332622 ooo_dev_tools-0.9.7/ooodev/events/draw_named_event.py
+-rw-r--r--   0        0        0     4247 2023-04-02 18:09:12.333621 ooo_dev_tools-0.9.7/ooodev/events/event_singleton.py
+-rw-r--r--   0        0        0     3816 2023-04-23 13:05:05.537315 ooo_dev_tools-0.9.7/ooodev/events/format_named_event.py
+-rw-r--r--   0        0        0      210 2023-04-02 18:09:12.334621 ooo_dev_tools-0.9.7/ooodev/events/gbl_named_event.py
+-rw-r--r--   0        0        0     9544 2023-04-02 18:09:12.335620 ooo_dev_tools-0.9.7/ooodev/events/lo_events.py
+-rw-r--r--   0        0        0     3082 2023-04-02 18:09:12.336620 ooo_dev_tools-0.9.7/ooodev/events/lo_named_event.py
+-rw-r--r--   0        0        0     1022 2023-04-23 13:05:05.538318 ooo_dev_tools-0.9.7/ooodev/events/props_named_event.py
+-rw-r--r--   0        0        0     5175 2023-04-02 18:09:12.337911 ooo_dev_tools-0.9.7/ooodev/events/write_named_event.py
+-rw-r--r--   0        0        0        0 2022-06-09 05:52:04.175567 ooo_dev_tools-0.9.7/ooodev/exceptions/__init__.py
+-rw-r--r--   0        0        0     9928 2023-04-06 02:13:08.630095 ooo_dev_tools-0.9.7/ooodev/exceptions/ex.py
+-rw-r--r--   0        0        0      160 2023-04-06 02:13:08.630095 ooo_dev_tools-0.9.7/ooodev/format/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.339621 ooo_dev_tools-0.9.7/ooodev/format/calc/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.339621 ooo_dev_tools-0.9.7/ooodev/format/calc/direct/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.631093 ooo_dev_tools-0.9.7/ooodev/format/calc/direct/cell/__init__.py
+-rw-r--r--   0        0        0      812 2023-04-06 02:13:48.174066 ooo_dev_tools-0.9.7/ooodev/format/calc/direct/cell/alignment/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-06 02:13:08.632095 ooo_dev_tools-0.9.7/ooodev/format/calc/direct/cell/background/__init__.py
+-rw-r--r--   0        0        0      782 2023-04-07 18:06:32.190987 ooo_dev_tools-0.9.7/ooodev/format/calc/direct/cell/borders/__init__.py
+-rw-r--r--   0        0        0      139 2023-04-06 02:13:08.633094 ooo_dev_tools-0.9.7/ooodev/format/calc/direct/cell/cell_protection/__init__.py
+-rw-r--r--   0        0        0     1376 2023-04-23 13:05:05.539317 ooo_dev_tools-0.9.7/ooodev/format/calc/direct/cell/font/__init__.py
+-rw-r--r--   0        0        0      281 2023-04-23 13:05:05.540318 ooo_dev_tools-0.9.7/ooodev/format/calc/direct/cell/numbers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.634096 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.634096 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/cell/__init__.py
+-rw-r--r--   0        0        0     1376 2023-04-06 02:13:08.635093 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/cell/alignment/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-06 02:13:08.635093 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/cell/background/__init__.py
+-rw-r--r--   0        0        0      852 2023-04-07 18:06:32.191986 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/cell/borders/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-06 02:13:08.636101 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/cell/cell_protection/__init__.py
+-rw-r--r--   0        0        0     1245 2023-04-06 02:13:08.637094 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/cell/font/__init__.py
+-rw-r--r--   0        0        0      530 2023-04-23 13:05:05.542331 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/cell/numbers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.637094 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/__init__.py
+-rw-r--r--   0        0        0     1123 2023-04-06 02:13:08.638093 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/area/__init__.py
+-rw-r--r--   0        0        0     1019 2023-04-06 02:13:08.638093 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/borders/__init__.py
+-rw-r--r--   0        0        0      276 2023-04-06 02:13:08.639095 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/footer/__init__.py
+-rw-r--r--   0        0        0     1100 2023-04-06 02:13:08.639095 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/footer/area/__init__.py
+-rw-r--r--   0        0        0     1005 2023-04-06 02:13:08.640095 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/footer/borders/__init__.py
+-rw-r--r--   0        0        0      290 2023-04-06 02:13:08.640095 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/header/__init__.py
+-rw-r--r--   0        0        0     1235 2023-04-06 02:13:08.641104 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/header/area/__init__.py
+-rw-r--r--   0        0        0     1112 2023-04-06 02:13:08.641104 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/header/borders/__init__.py
+-rw-r--r--   0        0        0     1162 2023-04-06 02:13:08.642093 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/page/__init__.py
+-rw-r--r--   0        0        0      708 2023-04-06 02:13:08.642093 ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/sheet/__init__.py
+-rw-r--r--   0        0        0      254 2023-04-06 02:13:48.198066 ooo_dev_tools-0.9.7/ooodev/format/calc/style/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.643095 ooo_dev_tools-0.9.7/ooodev/format/calc/style/cell/__init__.py
+-rw-r--r--   0        0        0     4313 2023-04-06 02:13:48.198066 ooo_dev_tools-0.9.7/ooodev/format/calc/style/cell/cell.py
+-rw-r--r--   0        0        0       60 2023-04-06 02:13:08.644094 ooo_dev_tools-0.9.7/ooodev/format/calc/style/cell/kind/__init__.py
+-rw-r--r--   0        0        0      588 2023-04-06 02:13:08.645093 ooo_dev_tools-0.9.7/ooodev/format/calc/style/cell/kind/style_cell_kind.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.645093 ooo_dev_tools-0.9.7/ooodev/format/calc/style/page/__init__.py
+-rw-r--r--   0        0        0       73 2023-04-06 02:13:08.645093 ooo_dev_tools-0.9.7/ooodev/format/calc/style/page/kind/__init__.py
+-rw-r--r--   0        0        0      207 2023-04-06 02:13:08.646094 ooo_dev_tools-0.9.7/ooodev/format/calc/style/page/kind/calc_style_page_kind.py
+-rw-r--r--   0        0        0     4101 2023-04-06 02:13:48.199068 ooo_dev_tools-0.9.7/ooodev/format/calc/style/page/page.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.542331 ooo_dev_tools-0.9.7/ooodev/format/chart2/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.543317 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.543317 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/axis/__init__.py
+-rw-r--r--   0        0        0     1096 2023-04-23 13:05:05.544315 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/axis/font/__init__.py
+-rw-r--r--   0        0        0      683 2023-04-23 13:05:05.545317 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/axis/label/__init__.py
+-rw-r--r--   0        0        0      305 2023-04-23 13:05:05.546314 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/axis/line/__init__.py
+-rw-r--r--   0        0        0      338 2023-04-23 13:05:05.547315 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/axis/numbers/__init__.py
+-rw-r--r--   0        0        0      887 2023-04-23 13:05:05.548318 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/axis/positioning/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.548318 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/general/__init__.py
+-rw-r--r--   0        0        0     1809 2023-04-23 13:05:05.549318 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/general/area/__init__.py
+-rw-r--r--   0        0        0      309 2023-04-23 13:05:05.550320 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/general/borders/__init__.py
+-rw-r--r--   0        0        0      339 2023-04-23 13:05:05.550320 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/general/numbers/__init__.py
+-rw-r--r--   0        0        0      212 2023-04-23 13:05:05.551317 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/general/position_size/__init__.py
+-rw-r--r--   0        0        0      519 2023-04-23 13:05:05.552317 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/general/transparency/__init__.py
+-rw-r--r--   0        0        0      309 2023-04-23 13:05:05.553316 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/grid/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.553316 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/legend/__init__.py
+-rw-r--r--   0        0        0     1812 2023-04-23 13:05:05.554315 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/legend/area/__init__.py
+-rw-r--r--   0        0        0      310 2023-04-23 13:05:05.555318 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/legend/borders/__init__.py
+-rw-r--r--   0        0        0     1280 2023-04-23 13:05:05.556318 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/legend/font/__init__.py
+-rw-r--r--   0        0        0      314 2023-04-23 13:05:05.557317 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/legend/position_size/__init__.py
+-rw-r--r--   0        0        0      521 2023-04-23 13:05:05.558318 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/legend/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.558318 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.559327 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_labels/__init__.py
+-rw-r--r--   0        0        0      331 2023-04-23 13:05:05.560319 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_labels/borders/__init__.py
+-rw-r--r--   0        0        0     1314 2023-04-23 13:05:05.561318 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_labels/data_labels/__init__.py
+-rw-r--r--   0        0        0     1124 2023-04-23 13:05:05.562318 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_labels/font/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.563317 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_series/__init__.py
+-rw-r--r--   0        0        0     1874 2023-04-23 13:05:05.564315 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_series/area/__init__.py
+-rw-r--r--   0        0        0      331 2023-04-23 13:05:05.564315 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_series/borders/__init__.py
+-rw-r--r--   0        0        0     1085 2023-04-23 13:05:05.566315 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_series/options/__init__.py
+-rw-r--r--   0        0        0      545 2023-04-23 13:05:05.568318 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_series/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.569317 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/title/__init__.py
+-rw-r--r--   0        0        0      357 2023-04-23 13:05:05.608317 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/title/alignment/__init__.py
+-rw-r--r--   0        0        0     1807 2023-04-23 13:05:05.651316 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/title/area/__init__.py
+-rw-r--r--   0        0        0      309 2023-04-23 13:05:05.652314 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/title/borders/__init__.py
+-rw-r--r--   0        0        0     1277 2023-04-23 13:05:05.653316 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/title/font/__init__.py
+-rw-r--r--   0        0        0      132 2023-04-23 13:05:05.654316 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/title/position_size/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.654316 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/wall/__init__.py
+-rw-r--r--   0        0        0     1804 2023-04-23 13:05:05.655315 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/wall/area/__init__.py
+-rw-r--r--   0        0        0      308 2023-04-23 13:05:05.656316 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/wall/borders/__init__.py
+-rw-r--r--   0        0        0      517 2023-04-23 13:05:05.657316 ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/wall/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.403612 ooo_dev_tools-0.9.7/ooodev/format/draw/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.404613 ooo_dev_tools-0.9.7/ooodev/format/draw/direct/__init__.py
+-rw-r--r--   0        0        0     1401 2023-04-23 13:05:05.659315 ooo_dev_tools-0.9.7/ooodev/format/draw/direct/area/__init__.py
+-rw-r--r--   0        0        0      641 2023-04-06 02:13:08.648096 ooo_dev_tools-0.9.7/ooodev/format/draw/direct/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.405614 ooo_dev_tools-0.9.7/ooodev/format/draw/modify/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-06 02:13:08.675095 ooo_dev_tools-0.9.7/ooodev/format/draw/modify/area/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.406613 ooo_dev_tools-0.9.7/ooodev/format/draw/style/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-02 18:09:12.406613 ooo_dev_tools-0.9.7/ooodev/format/draw/style/kind/__init__.py
+-rw-r--r--   0        0        0     2652 2023-04-02 18:09:12.407617 ooo_dev_tools-0.9.7/ooodev/format/draw/style/lookup/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.408612 ooo_dev_tools-0.9.7/ooodev/format/impress/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.408612 ooo_dev_tools-0.9.7/ooodev/format/impress/modify/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-06 02:13:08.676094 ooo_dev_tools-0.9.7/ooodev/format/impress/modify/area/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.677093 ooo_dev_tools-0.9.7/ooodev/format/inner/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.677093 ooo_dev_tools-0.9.7/ooodev/format/inner/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.677093 ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/__init__.py
+-rw-r--r--   0        0        0     4252 2023-04-28 12:39:00.162728 ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_document.py
+-rw-r--r--   0        0        0     4577 2023-04-06 02:13:48.214066 ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_fill_color.py
+-rw-r--r--   0        0        0    16076 2023-04-06 02:13:48.251066 ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_hf.py
+-rw-r--r--   0        0        0     7849 2023-04-06 02:13:08.680093 ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_line_number.py
+-rw-r--r--   0        0        0    11818 2023-04-06 02:13:08.681095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_padding.py
+-rw-r--r--   0        0        0    10284 2023-04-06 02:13:08.682094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_sides.py
+-rw-r--r--   0        0        0     5204 2023-04-23 13:05:05.660316 ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_writing_mode.py
+-rw-r--r--   0        0        0     4323 2023-04-06 02:13:08.683094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/border_width_impl.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.683094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/format_types/__init__.py
+-rw-r--r--   0        0        0      262 2023-04-06 02:13:08.684096 ooo_dev_tools-0.9.7/ooodev/format/inner/common/format_types/offset_column.py
+-rw-r--r--   0        0        0      256 2023-04-06 02:13:08.684096 ooo_dev_tools-0.9.7/ooodev/format/inner/common/format_types/offset_row.py
+-rw-r--r--   0        0        0      252 2023-04-06 02:13:08.685095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/format_types/size_percent.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.685095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-06 02:13:08.685095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/area_gradient_props.py
+-rw-r--r--   0        0        0      324 2023-04-06 02:13:08.686095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/area_hatch_props.py
+-rw-r--r--   0        0        0      531 2023-04-06 02:13:08.686095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/area_img_props.py
+-rw-r--r--   0        0        0      294 2023-04-06 02:13:08.687092 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/area_pattern_props.py
+-rw-r--r--   0        0        0      187 2023-04-06 02:13:08.687092 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/border_props.py
+-rw-r--r--   0        0        0      181 2023-04-06 02:13:08.688095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/cell_background_color_props.py
+-rw-r--r--   0        0        0      650 2023-04-06 02:13:08.688095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/cell_borders_props.py
+-rw-r--r--   0        0        0      499 2023-04-06 02:13:08.689094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/cell_style_borders_props.py
+-rw-r--r--   0        0        0      238 2023-04-06 02:13:08.689094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/cell_text_align_props.py
+-rw-r--r--   0        0        0      197 2023-04-06 02:13:08.690093 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/cell_text_orientation_props.py
+-rw-r--r--   0        0        0      203 2023-04-06 02:13:08.690093 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/cell_text_properties_props.py
+-rw-r--r--   0        0        0      288 2023-04-06 02:13:08.691092 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/fill_color_props.py
+-rw-r--r--   0        0        0      179 2023-04-06 02:13:08.691092 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/font_only_props.py
+-rw-r--r--   0        0        0      176 2023-04-06 02:13:08.692095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/frame_options_align_props.py
+-rw-r--r--   0        0        0      196 2023-04-06 02:13:08.692095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/frame_options_names_props.py
+-rw-r--r--   0        0        0      239 2023-04-06 02:13:08.693095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/frame_options_properties.py
+-rw-r--r--   0        0        0      244 2023-04-06 02:13:08.693095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/frame_options_protect_props.py
+-rw-r--r--   0        0        0      166 2023-04-06 02:13:08.694094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/frame_type_anchor_props.py
+-rw-r--r--   0        0        0      445 2023-04-06 02:13:08.695094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/frame_type_positon_props.py
+-rw-r--r--   0        0        0      449 2023-04-06 02:13:08.695094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/frame_type_size_props.py
+-rw-r--r--   0        0        0      231 2023-04-06 02:13:08.696094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/frame_wrap_options_props.py
+-rw-r--r--   0        0        0      165 2023-04-06 02:13:08.696094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/frame_wrap_settings_props.py
+-rw-r--r--   0        0        0      628 2023-04-06 02:13:08.697094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/hf_props.py
+-rw-r--r--   0        0        0      313 2023-04-06 02:13:08.697094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/hyperlink_props.py
+-rw-r--r--   0        0        0      263 2023-04-06 02:13:08.698096 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/image_crop_props.py
+-rw-r--r--   0        0        0      253 2023-04-06 02:13:08.698096 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/image_flip_props.py
+-rw-r--r--   0        0        0      209 2023-04-06 02:13:08.699094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/image_options_names_props.py
+-rw-r--r--   0        0        0      168 2023-04-06 02:13:08.699094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/image_options_properties.py
+-rw-r--r--   0        0        0      154 2023-04-06 02:13:08.700095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/image_rotation_props.py
+-rw-r--r--   0        0        0      218 2023-04-06 02:13:08.700095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/img_para_area_props.py
+-rw-r--r--   0        0        0      178 2023-04-06 02:13:08.701096 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/list_style_props.py
+-rw-r--r--   0        0        0      207 2023-04-06 02:13:08.701096 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/page_margin_props.py
+-rw-r--r--   0        0        0      157 2023-04-06 02:13:08.702098 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/prop_pair.py
+-rw-r--r--   0        0        0      329 2023-04-06 02:13:08.702098 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/shape_shadow_props.py
+-rw-r--r--   0        0        0      319 2023-04-06 02:13:08.703097 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/struct_border_table_props.py
+-rw-r--r--   0        0        0      266 2023-04-06 02:13:08.703097 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/struct_cell_protection_props.py
+-rw-r--r--   0        0        0      235 2023-04-06 02:13:08.704097 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/struct_crop_props.py
+-rw-r--r--   0        0        0      349 2023-04-23 13:05:05.661314 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/struct_data_point_label_props.py
+-rw-r--r--   0        0        0      208 2023-04-06 02:13:08.704097 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/struct_size_props.py
+-rw-r--r--   0        0        0      333 2023-04-06 02:13:08.705094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/struct_table_border_distances_props.py
+-rw-r--r--   0        0        0      443 2023-04-06 02:13:08.705094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/table_borders_props.py
+-rw-r--r--   0        0        0      281 2023-04-06 02:13:08.706095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/table_properties_props.py
+-rw-r--r--   0        0        0      181 2023-04-23 13:05:05.662316 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/title_alignment_orientation_props.py
+-rw-r--r--   0        0        0      279 2023-04-06 02:13:08.706095 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/transparent_gradient_props.py
+-rw-r--r--   0        0        0      188 2023-04-06 02:13:08.707094 ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/transparent_transparency_props.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.707094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.747094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.783096 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/alignment/__init__.py
+-rw-r--r--   0        0        0     6882 2023-04-06 02:13:08.785095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/alignment/properties.py
+-rw-r--r--   0        0        0     8619 2023-04-06 02:13:08.786095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/alignment/text_align.py
+-rw-r--r--   0        0        0     6213 2023-04-06 02:13:08.786095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/alignment/text_orientation.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.787101 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/background/__init__.py
+-rw-r--r--   0        0        0     5291 2023-04-06 02:13:48.252066 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/background/color.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.788097 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/border/__init__.py
+-rw-r--r--   0        0        0    21721 2023-04-23 13:05:05.663315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/border/borders.py
+-rw-r--r--   0        0        0     4491 2023-04-25 00:03:57.142368 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/border/padding.py
+-rw-r--r--   0        0        0     2467 2023-04-25 00:03:57.143369 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/border/shadow.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.790094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/cell_protection/__init__.py
+-rw-r--r--   0        0        0      340 2023-04-06 02:13:08.790094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/cell_protection/cell_protection.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.665318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/char/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.665318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/char/font/__init__.py
+-rw-r--r--   0        0        0     5474 2023-04-23 13:05:05.666314 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/char/font/font.py
+-rw-r--r--   0        0        0      483 2023-04-23 13:05:05.667318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/char/font/font_effects.py
+-rw-r--r--   0        0        0      414 2023-04-23 13:05:05.667318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/char/font/font_only.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.668318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/numbers/__init__.py
+-rw-r--r--   0        0        0    13621 2023-04-23 13:05:05.669315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/numbers/numbers.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.791094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/page/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.791094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/page/page/__init__.py
+-rw-r--r--   0        0        0     6479 2023-04-06 02:13:08.792095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/page/page/layout_settings.py
+-rw-r--r--   0        0        0     7920 2023-04-28 12:39:00.163730 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/page/page/margins.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.669315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.669315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.669315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/font/__init__.py
+-rw-r--r--   0        0        0      829 2023-04-23 13:05:05.670316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/font/font_effects.py
+-rw-r--r--   0        0        0     2473 2023-04-23 13:05:05.671317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/font/font_only.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.671317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/label/__init__.py
+-rw-r--r--   0        0        0     1727 2023-04-23 13:05:05.672315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/label/order.py
+-rw-r--r--   0        0        0     3433 2023-04-23 13:05:05.690317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/label/orientation.py
+-rw-r--r--   0        0        0     1539 2023-04-23 13:05:05.692315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/label/show.py
+-rw-r--r--   0        0        0     2158 2023-04-23 13:05:05.693316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/label/text_flow.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.693316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/line/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-23 13:05:05.694316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/line/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.695316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/numbers/__init__.py
+-rw-r--r--   0        0        0      590 2023-04-23 13:05:05.697316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/numbers/numbers.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.697316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/positioning/__init__.py
+-rw-r--r--   0        0        0     3064 2023-04-23 13:05:05.698315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/positioning/axis_line.py
+-rw-r--r--   0        0        0     3481 2023-04-23 13:05:05.699318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/positioning/interval_marks.py
+-rw-r--r--   0        0        0     1757 2023-04-23 13:05:05.721313 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/positioning/label_position.py
+-rw-r--r--   0        0        0     3043 2023-04-23 13:05:05.722317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/positioning/position_axis.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.723316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.723316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/area/__init__.py
+-rw-r--r--   0        0        0      895 2023-04-23 13:05:05.725319 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/area/color.py
+-rw-r--r--   0        0        0     7146 2023-04-23 13:05:05.727315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/area/gradient.py
+-rw-r--r--   0        0        0     9958 2023-04-23 13:05:05.728316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/area/hatch.py
+-rw-r--r--   0        0        0     7581 2023-04-23 13:05:05.729316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/area/img.py
+-rw-r--r--   0        0        0     5901 2023-04-23 13:05:05.729316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.730316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/borders/__init__.py
+-rw-r--r--   0        0        0     4771 2023-04-23 13:05:05.731317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/borders/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.731317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/numbers/__init__.py
+-rw-r--r--   0        0        0     6352 2023-04-23 13:05:05.732316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/numbers/numbers.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.732316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/transparent/__init__.py
+-rw-r--r--   0        0        0     5650 2023-04-23 13:05:05.733316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/transparent/gradient.py
+-rw-r--r--   0        0        0     1173 2023-04-23 13:05:05.734315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/transparent/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.734315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/grid/__init__.py
+-rw-r--r--   0        0        0     1542 2023-04-23 13:05:05.735316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/grid/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.736317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.736317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/area/__init__.py
+-rw-r--r--   0        0        0      213 2023-04-23 13:05:05.737315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/area/color.py
+-rw-r--r--   0        0        0      285 2023-04-23 13:05:05.738316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/area/gradient.py
+-rw-r--r--   0        0        0      224 2023-04-23 13:05:05.738316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/area/hatch.py
+-rw-r--r--   0        0        0      253 2023-04-23 13:05:05.739316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/area/img.py
+-rw-r--r--   0        0        0      236 2023-04-23 13:05:05.740315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.740315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/borders/__init__.py
+-rw-r--r--   0        0        0      279 2023-04-23 13:05:05.741315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/borders/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.742317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/font/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-23 13:05:05.744318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/font/font.py
+-rw-r--r--   0        0        0      561 2023-04-23 13:05:05.745325 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/font/font_effects.py
+-rw-r--r--   0        0        0      465 2023-04-23 13:05:05.745325 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/font/font_only.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.746317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/position/__init__.py
+-rw-r--r--   0        0        0     5243 2023-04-23 13:05:05.808315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/position/position.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.808315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/transparent/__init__.py
+-rw-r--r--   0        0        0      372 2023-04-23 13:05:05.856315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/transparent/gradient.py
+-rw-r--r--   0        0        0      288 2023-04-23 13:05:05.856315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/transparent/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.857317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/position_size/__init__.py
+-rw-r--r--   0        0        0     4171 2023-04-23 13:05:05.858317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/position_size/position.py
+-rw-r--r--   0        0        0     4066 2023-04-23 13:05:05.859318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/position_size/size.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.859318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/__index__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.860316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.860316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/borders/__init__.py
+-rw-r--r--   0        0        0     3112 2023-04-23 13:05:05.861316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/borders/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.862317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/__init__.py
+-rw-r--r--   0        0        0     3326 2023-04-23 13:05:05.863316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/attrib_options.py
+-rw-r--r--   0        0        0     6717 2023-04-23 13:05:05.864316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/number_format.py
+-rw-r--r--   0        0        0     4193 2023-04-23 13:05:05.864316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/orientation.py
+-rw-r--r--   0        0        0     7580 2023-04-23 13:05:05.865316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/percent_format.py
+-rw-r--r--   0        0        0      250 2023-04-23 13:05:05.866317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/text_attribs.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.866317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/font/__init__.py
+-rw-r--r--   0        0        0      867 2023-04-23 13:05:05.867314 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/font/font_effects.py
+-rw-r--r--   0        0        0     2511 2023-04-23 13:05:05.868317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/font/font_only.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.868317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.869315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/area/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-23 13:05:05.870317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/area/color.py
+-rw-r--r--   0        0        0      292 2023-04-23 13:05:05.870317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/area/gradient.py
+-rw-r--r--   0        0        0      231 2023-04-23 13:05:05.871315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/area/hatch.py
+-rw-r--r--   0        0        0      260 2023-04-23 13:05:05.872317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/area/img.py
+-rw-r--r--   0        0        0      243 2023-04-23 13:05:05.873317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.873317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/borders/__init__.py
+-rw-r--r--   0        0        0     5492 2023-04-23 13:05:05.874316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/borders/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.874316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/options/__init__.py
+-rw-r--r--   0        0        0     4504 2023-04-23 13:05:05.876317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/options/align_series.py
+-rw-r--r--   0        0        0     2841 2023-04-23 13:05:05.877319 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/options/legend_entry.py
+-rw-r--r--   0        0        0     5033 2023-04-23 13:05:05.878316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/options/orientation.py
+-rw-r--r--   0        0        0     2126 2023-04-23 13:05:05.879315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/options/plot.py
+-rw-r--r--   0        0        0     3329 2023-04-23 13:05:05.880316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/options/plot_simple.py
+-rw-r--r--   0        0        0     6823 2023-04-23 13:05:05.881314 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/options/settings.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.881314 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/transparent/__init__.py
+-rw-r--r--   0        0        0      304 2023-04-23 13:05:05.882316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/transparent/gradient.py
+-rw-r--r--   0        0        0      286 2023-04-23 13:05:05.882316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/transparent/transparency.py
+-rw-r--r--   0        0        0     4171 2023-04-23 13:05:05.883315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/alignment/direction.py
+-rw-r--r--   0        0        0     4313 2023-04-23 13:05:05.884316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/alignment/orientation.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.884316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/area/__init__.py
+-rw-r--r--   0        0        0      213 2023-04-23 13:05:05.886315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/area/color.py
+-rw-r--r--   0        0        0      285 2023-04-23 13:05:05.887313 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/area/gradient.py
+-rw-r--r--   0        0        0      224 2023-04-23 13:05:05.930313 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/area/hatch.py
+-rw-r--r--   0        0        0      253 2023-04-23 13:05:05.931335 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/area/img.py
+-rw-r--r--   0        0        0      236 2023-04-23 13:05:05.932316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.932316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/borders/__init__.py
+-rw-r--r--   0        0        0      278 2023-04-23 13:05:05.933316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/borders/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.934319 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/font/__init__.py
+-rw-r--r--   0        0        0     6359 2023-04-23 13:05:05.935317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/font/font.py
+-rw-r--r--   0        0        0      918 2023-04-23 13:05:05.936322 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/font/font_effects.py
+-rw-r--r--   0        0        0     2312 2023-04-23 13:05:05.936322 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/font/font_only.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.937320 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/position_size/__init__.py
+-rw-r--r--   0        0        0      880 2023-04-23 13:05:05.938317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/position_size/position.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.938317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.938317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/area/__init__.py
+-rw-r--r--   0        0        0      657 2023-04-23 13:05:05.939316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/area/color.py
+-rw-r--r--   0        0        0      712 2023-04-23 13:05:05.940318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/area/gradient.py
+-rw-r--r--   0        0        0      658 2023-04-23 13:05:05.941317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/area/hatch.py
+-rw-r--r--   0        0        0      686 2023-04-23 13:05:05.942316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/area/img.py
+-rw-r--r--   0        0        0      670 2023-04-23 13:05:05.943317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.943317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/borders/__init__.py
+-rw-r--r--   0        0        0      719 2023-04-23 13:05:05.944316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/borders/line_properties.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.944316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/transparent/__init__.py
+-rw-r--r--   0        0        0      725 2023-04-23 13:05:05.945315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/transparent/gradient.py
+-rw-r--r--   0        0        0     1040 2023-04-23 13:05:05.946318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/transparent/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.947318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/draw/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.947318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/draw/fill/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:05.947318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/draw/fill/area/__init__.py
+-rw-r--r--   0        0        0      229 2023-04-23 13:05:05.948315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/draw/fill/area/color.py
+-rw-r--r--   0        0        0      288 2023-04-23 13:05:06.011316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/draw/fill/area/gradient.py
+-rw-r--r--   0        0        0      249 2023-04-23 13:05:06.014318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/draw/fill/area/hatch.py
+-rw-r--r--   0        0        0      266 2023-04-23 13:05:06.016320 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/draw/fill/area/img.py
+-rw-r--r--   0        0        0      250 2023-04-23 13:05:06.061315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/draw/fill/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:06.062319 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/draw/shape/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:06.062319 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/draw/shape/position_size/__init__.py
+-rw-r--r--   0        0        0     3378 2023-04-23 13:05:06.063318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/draw/shape/position_size/position.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.793096 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/__init__.py
+-rw-r--r--   0        0        0     9315 2023-04-06 02:13:48.258068 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/cell_protection_struct.py
+-rw-r--r--   0        0        0    11233 2023-04-06 02:13:48.260066 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/crop_struct.py
+-rw-r--r--   0        0        0    11148 2023-04-23 13:05:06.064318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/data_point_label_struct.py
+-rw-r--r--   0        0        0    10183 2023-04-06 02:13:48.262067 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/drop_cap_struct.py
+-rw-r--r--   0        0        0    14924 2023-04-23 13:05:06.065314 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/gradient_struct.py
+-rw-r--r--   0        0        0     8274 2023-04-06 02:13:48.266068 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/hatch_struct.py
+-rw-r--r--   0        0        0    10085 2023-04-06 02:13:48.267067 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/line_spacing_struct.py
+-rw-r--r--   0        0        0    31720 2023-04-06 02:13:48.269067 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/locale_struct.py
+-rw-r--r--   0        0        0     7412 2023-04-23 13:05:06.066317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/point_struct.py
+-rw-r--r--   0        0        0    11808 2023-04-25 00:03:57.144366 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/shadow_struct.py
+-rw-r--r--   0        0        0    25317 2023-04-06 02:13:48.277068 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/side.py
+-rw-r--r--   0        0        0     8482 2023-04-23 13:05:06.068316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/size_struct.py
+-rw-r--r--   0        0        0      640 2023-04-06 02:13:08.801095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/struct_base.py
+-rw-r--r--   0        0        0    13991 2023-04-06 02:13:48.280068 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/tab_stop_struct.py
+-rw-r--r--   0        0        0    13469 2023-04-06 02:13:48.281067 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/table_border_distances_struct.py
+-rw-r--r--   0        0        0    20841 2023-04-06 02:13:48.282066 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/table_border_struct.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.803095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.803095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.804095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/border/__init__.py
+-rw-r--r--   0        0        0    10699 2023-04-25 00:03:57.146365 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/border/borders.py
+-rw-r--r--   0        0        0     3673 2023-04-25 00:03:57.148365 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/border/padding.py
+-rw-r--r--   0        0        0     2842 2023-04-25 00:03:57.149366 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/border/shadow.py
+-rw-r--r--   0        0        0     1766 2023-04-06 02:13:08.806095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/border/sides.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.807104 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/font/__init__.py
+-rw-r--r--   0        0        0    34878 2023-04-23 13:05:06.069317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/font/font.py
+-rw-r--r--   0        0        0    26959 2023-04-23 13:05:06.070317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/font/font_effects.py
+-rw-r--r--   0        0        0    21564 2023-04-23 13:05:06.070317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/font/font_only.py
+-rw-r--r--   0        0        0    21425 2023-04-23 13:05:06.120316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/font/font_position.py
+-rw-r--r--   0        0        0        1 2023-04-06 02:13:08.810097 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/highlight/__init__.py
+-rw-r--r--   0        0        0     5299 2023-04-23 13:05:06.121316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/highlight/highlight.py
+-rw-r--r--   0        0        0        1 2023-04-06 02:13:08.811097 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/hyperlink/__init__.py
+-rw-r--r--   0        0        0     5191 2023-04-23 13:05:06.122323 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/hyperlink/hyperlink.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.812096 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.812096 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/area/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-06 02:13:08.813095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/area/fill_color.py
+-rw-r--r--   0        0        0    14379 2023-04-25 00:03:57.150372 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/area/gradient.py
+-rw-r--r--   0        0        0    13254 2023-04-23 13:05:06.124315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/area/hatch.py
+-rw-r--r--   0        0        0    18444 2023-04-23 13:05:06.126315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/area/img.py
+-rw-r--r--   0        0        0    10537 2023-04-23 13:05:06.127315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.837095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/transparent/__init__.py
+-rw-r--r--   0        0        0    12939 2023-04-23 13:05:06.129317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/transparent/gradient.py
+-rw-r--r--   0        0        0     5167 2023-04-25 00:03:57.152366 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/transparent/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.852094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.852094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/frame_type/__init__.py
+-rw-r--r--   0        0        0     4866 2023-04-06 02:13:08.853094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/frame_type/anchor.py
+-rw-r--r--   0        0        0    18717 2023-04-06 02:13:08.866093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/frame_type/position.py
+-rw-r--r--   0        0        0     6874 2023-04-06 02:13:08.867093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/frame_type/size.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.867093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/hyperlink/__init__.py
+-rw-r--r--   0        0        0     4026 2023-04-06 02:13:08.868093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/hyperlink/image_map_options.py
+-rw-r--r--   0        0        0     5997 2023-04-06 02:13:08.869093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/hyperlink/link_to.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.869093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/options/__init__.py
+-rw-r--r--   0        0        0     4913 2023-04-06 02:13:08.870096 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/options/align.py
+-rw-r--r--   0        0        0     8725 2023-04-06 02:13:08.871096 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/options/names.py
+-rw-r--r--   0        0        0     9653 2023-04-06 02:13:08.871096 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/options/properties.py
+-rw-r--r--   0        0        0     4781 2023-04-06 02:13:08.872094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/options/protect.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.872094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/wrap/__init__.py
+-rw-r--r--   0        0        0     7691 2023-04-06 02:13:08.873093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/wrap/options.py
+-rw-r--r--   0        0        0     3655 2023-04-06 02:13:08.873093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/wrap/settings.py
+-rw-r--r--   0        0        0     1796 2023-04-06 02:13:08.874109 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/wrap/spacing.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.874109 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.874109 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/crop/__init__.py
+-rw-r--r--   0        0        0    18759 2023-04-06 02:13:48.323067 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/crop/crop.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.875093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/image/__init__.py
+-rw-r--r--   0        0        0     5201 2023-04-06 02:13:08.876094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/image/flip.py
+-rw-r--r--   0        0        0     3716 2023-04-06 02:13:08.876094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/image/rotation.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.877095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/image_type/__init__.py
+-rw-r--r--   0        0        0    11093 2023-04-06 02:13:08.877095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/image_type/size.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.878097 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/options/__init__.py
+-rw-r--r--   0        0        0     2718 2023-04-06 02:13:08.878097 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/options/names.py
+-rw-r--r--   0        0        0     3786 2023-04-06 02:13:08.879093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/options/properties.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.879093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:48.323067 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:48.324069 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/area/__init__.py
+-rw-r--r--   0        0        0      961 2023-04-06 02:13:48.325067 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/area/color.py
+-rw-r--r--   0        0        0     1247 2023-04-06 02:13:48.325067 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/area/gradient.py
+-rw-r--r--   0        0        0     1302 2023-04-06 02:13:48.326069 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/area/hatch.py
+-rw-r--r--   0        0        0     1505 2023-04-06 02:13:48.326069 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/area/img.py
+-rw-r--r--   0        0        0     1226 2023-04-06 02:13:48.327067 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/area/pattern.py
+-rw-r--r--   0        0        0     1432 2023-04-06 02:13:48.328065 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/footer.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:48.328065 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:48.329080 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/area/__init__.py
+-rw-r--r--   0        0        0     1376 2023-04-06 02:13:48.329080 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/area/color.py
+-rw-r--r--   0        0        0     1679 2023-04-06 02:13:48.359068 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/area/gradient.py
+-rw-r--r--   0        0        0     1815 2023-04-06 02:13:48.360070 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/area/hatch.py
+-rw-r--r--   0        0        0     1962 2023-04-06 02:13:48.361065 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/area/img.py
+-rw-r--r--   0        0        0     1683 2023-04-06 02:13:48.362067 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/area/pattern.py
+-rw-r--r--   0        0        0     1432 2023-04-06 02:13:48.413067 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/header.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.879093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/page/__init__.py
+-rw-r--r--   0        0        0     6554 2023-04-06 02:13:08.880098 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/page/layout_settings.py
+-rw-r--r--   0        0        0     3103 2023-04-06 02:13:08.881093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/page/margins.py
+-rw-r--r--   0        0        0     5382 2023-04-06 02:13:08.882094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/page/paper_format.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.882094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/__init__.py
+-rw-r--r--   0        0        0      389 2023-04-06 02:13:08.883094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/align/__init__.py
+-rw-r--r--   0        0        0    15153 2023-04-23 13:05:06.130316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/align/alignment.py
+-rw-r--r--   0        0        0     3563 2023-04-23 13:05:06.131316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/align/writing_mode.py
+-rw-r--r--   0        0        0        1 2023-04-06 02:13:08.886093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/area/__init__.py
+-rw-r--r--   0        0        0     2329 2023-04-23 13:05:06.132317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/area/color.py
+-rw-r--r--   0        0        0    16148 2023-04-25 00:03:57.157367 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/area/hatch.py
+-rw-r--r--   0        0        0    12316 2023-04-25 00:03:57.158377 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/area/img.py
+-rw-r--r--   0        0        0     7090 2023-04-25 00:03:57.162369 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/area/pattern.py
+-rw-r--r--   0        0        0      471 2023-04-06 02:13:08.889093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/border/__init__.py
+-rw-r--r--   0        0        0    11995 2023-04-23 13:05:06.133316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/border/borders.py
+-rw-r--r--   0        0        0     2524 2023-04-06 02:13:08.890095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/border/padding.py
+-rw-r--r--   0        0        0      834 2023-04-06 02:13:08.891093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/border/shadow.py
+-rw-r--r--   0        0        0     2025 2023-04-06 02:13:08.892093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/border/sides.py
+-rw-r--r--   0        0        0        1 2023-04-06 02:13:08.892093 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/drop_cap/__init__.py
+-rw-r--r--   0        0        0     9215 2023-04-23 13:05:06.134314 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/drop_cap/drop_caps.py
+-rw-r--r--   0        0        0      303 2023-04-06 02:13:08.894096 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/indent_space/__init__.py
+-rw-r--r--   0        0        0     9784 2023-04-23 13:05:06.135316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/indent_space/indent.py
+-rw-r--r--   0        0        0     8011 2023-04-06 02:13:08.895096 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/indent_space/indent_spacing.py
+-rw-r--r--   0        0        0     7733 2023-04-23 13:05:06.136315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/indent_space/line_spacing.py
+-rw-r--r--   0        0        0     8546 2023-04-23 13:05:06.137317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/indent_space/spacing.py
+-rw-r--r--   0        0        0      368 2023-04-06 02:13:08.917097 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/outline_list/__init__.py
+-rw-r--r--   0        0        0     1937 2023-04-23 13:05:06.138318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/outline_list/line_num.py
+-rw-r--r--   0        0        0    10154 2023-04-23 13:05:06.138318 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/outline_list/list_style.py
+-rw-r--r--   0        0        0     7701 2023-04-23 13:05:06.139319 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/outline_list/outline.py
+-rw-r--r--   0        0        0     7271 2023-04-23 13:05:06.140316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/outline_list/outline_list.py
+-rw-r--r--   0        0        0     2936 2023-04-06 02:13:08.920094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/padding.py
+-rw-r--r--   0        0        0      191 2023-04-06 02:13:08.920094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/tabs/__init__.py
+-rw-r--r--   0        0        0    10188 2023-04-23 13:05:06.141315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/tabs/tabs.py
+-rw-r--r--   0        0        0      261 2023-04-06 02:13:08.921095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/text_flow/__init__.py
+-rw-r--r--   0        0        0     6561 2023-04-23 13:05:06.142317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/text_flow/breaks.py
+-rw-r--r--   0        0        0    10397 2023-04-23 13:05:06.143317 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/text_flow/flow_options.py
+-rw-r--r--   0        0        0    10282 2023-04-23 13:05:06.144316 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/text_flow/hyphenation.py
+-rw-r--r--   0        0        0     7546 2023-04-23 13:05:06.145315 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/text_flow/text_flow.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.924094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/transparent/__init__.py
+-rw-r--r--   0        0        0     3859 2023-04-06 02:13:08.925095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/transparent/gradient.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.925095 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/shape/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.926092 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/shape/area/__init__.py
+-rw-r--r--   0        0        0    16356 2023-04-06 02:13:48.420065 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/shape/area/shadow.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.927094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/table/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.927094 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/table/background/__init__.py
+-rw-r--r--   0        0        0     1628 2023-04-25 00:03:57.164367 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/table/background/color.py
+-rw-r--r--   0        0        0     4880 2023-04-25 00:03:57.165366 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/table/background/img.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.929096 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/table/borders/__init__.py
+-rw-r--r--   0        0        0    18876 2023-04-25 00:03:57.173370 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/table/borders/borders.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.929096 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/table/props/__init__.py
+-rw-r--r--   0        0        0    74742 2023-04-25 00:03:57.175369 ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/table/props/table_properties.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.931093 ooo_dev_tools-0.9.7/ooodev/format/inner/kind/__init__.py
+-rw-r--r--   0        0        0      231 2023-04-06 02:13:08.932094 ooo_dev_tools-0.9.7/ooodev/format/inner/kind/border_kind.py
+-rw-r--r--   0        0        0      509 2023-04-06 02:13:48.421066 ooo_dev_tools-0.9.7/ooodev/format/inner/kind/format_kind.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.932094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.933097 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.933097 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/alignment/__init__.py
+-rw-r--r--   0        0        0     3747 2023-04-06 02:13:08.934097 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/alignment/properties.py
+-rw-r--r--   0        0        0     3809 2023-04-06 02:13:08.935098 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/alignment/text_align.py
+-rw-r--r--   0        0        0     3655 2023-04-06 02:13:08.935098 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/alignment/text_orientation.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.935098 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/background/__init__.py
+-rw-r--r--   0        0        0     3261 2023-04-06 02:13:48.422065 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/background/color.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.936097 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/border/__init__.py
+-rw-r--r--   0        0        0    23992 2023-04-07 18:06:32.203989 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/border/borders.py
+-rw-r--r--   0        0        0      172 2023-04-07 18:06:32.209987 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/border/padding.py
+-rw-r--r--   0        0        0      166 2023-04-07 18:06:32.210989 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/border/shadow.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.937094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/cell_protection/__init__.py
+-rw-r--r--   0        0        0     4681 2023-04-06 02:13:08.938093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/cell_protection/cell_protection.py
+-rw-r--r--   0        0        0     3739 2023-04-06 02:13:08.938093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/cell_style_base.py
+-rw-r--r--   0        0        0      820 2023-04-06 02:13:08.939094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/cell_style_base_multi.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.939094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/font/__init__.py
+-rw-r--r--   0        0        0     6013 2023-04-06 02:13:48.425066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/font/font_effects.py
+-rw-r--r--   0        0        0     4325 2023-04-06 02:13:08.941096 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/font/font_only.py
+-rw-r--r--   0        0        0        0 2023-04-23 13:05:06.145315 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/numbers/__index__.py
+-rw-r--r--   0        0        0     4733 2023-04-23 13:05:06.146314 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/numbers/numbers.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.941096 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.941096 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/area/__init__.py
+-rw-r--r--   0        0        0     4943 2023-04-06 02:13:48.426066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/area/color.py
+-rw-r--r--   0        0        0     5808 2023-04-06 02:13:08.942093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/area/img.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.943095 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/border/__init__.py
+-rw-r--r--   0        0        0     5359 2023-04-06 02:13:08.943095 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/border/padding.py
+-rw-r--r--   0        0        0     4973 2023-04-06 02:13:48.426066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/border/shadow.py
+-rw-r--r--   0        0        0     5300 2023-04-06 02:13:08.945095 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/border/sides.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.945095 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.945095 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/area/__init__.py
+-rw-r--r--   0        0        0     1028 2023-04-06 02:13:48.427066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/area/color.py
+-rw-r--r--   0        0        0     1943 2023-04-06 02:13:48.428066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/area/img.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.947095 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/border/__init__.py
+-rw-r--r--   0        0        0     1095 2023-04-06 02:13:48.429066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/border/padding.py
+-rw-r--r--   0        0        0      917 2023-04-06 02:13:48.429066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/border/shadow.py
+-rw-r--r--   0        0        0     1092 2023-04-06 02:13:48.430065 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/border/sides.py
+-rw-r--r--   0        0        0     1116 2023-04-06 02:13:48.431066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/footer.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.982094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.982094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/area/__init__.py
+-rw-r--r--   0        0        0     5283 2023-04-06 02:13:48.431066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/area/color.py
+-rw-r--r--   0        0        0     7094 2023-04-06 02:13:48.432068 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/area/img.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.984094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/border/__init__.py
+-rw-r--r--   0        0        0     6626 2023-04-06 02:13:48.433067 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/border/padding.py
+-rw-r--r--   0        0        0     6045 2023-04-06 02:13:48.434070 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/border/shadow.py
+-rw-r--r--   0        0        0     6289 2023-04-06 02:13:48.434070 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/border/sides.py
+-rw-r--r--   0        0        0     7271 2023-04-06 02:13:48.435066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/header.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.986093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/page/__init__.py
+-rw-r--r--   0        0        0     3819 2023-04-06 02:13:08.987094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/page/layout_settings.py
+-rw-r--r--   0        0        0     3565 2023-04-06 02:13:08.987094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/page/margins.py
+-rw-r--r--   0        0        0     4332 2023-04-06 02:13:08.988093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/page/paper_format.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.988093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/sheet/__init__.py
+-rw-r--r--   0        0        0     4051 2023-04-06 02:13:08.989095 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/sheet/order.py
+-rw-r--r--   0        0        0     7444 2023-04-06 02:13:08.989095 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/sheet/printing.py
+-rw-r--r--   0        0        0     3418 2023-04-06 02:13:08.990094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/sheet/scale_num_of_pages.py
+-rw-r--r--   0        0        0     4164 2023-04-06 02:13:08.991094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/sheet/scale_pages_width_height.py
+-rw-r--r--   0        0        0     3543 2023-04-06 02:13:08.991094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/sheet/scale_reduce_enlarge.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.991094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.992093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.992093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/border/__init__.py
+-rw-r--r--   0        0        0     3984 2023-04-25 13:12:44.849692 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/border/padding.py
+-rw-r--r--   0        0        0     4035 2023-04-25 13:12:44.854694 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/border/shadow.py
+-rw-r--r--   0        0        0     4059 2023-04-25 13:12:44.855694 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/border/sides.py
+-rw-r--r--   0        0        0      701 2023-04-06 02:13:08.994096 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/char_style_base_multi.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.995093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/font/__init__.py
+-rw-r--r--   0        0        0     5488 2023-04-25 13:12:44.857691 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/font/font_effects.py
+-rw-r--r--   0        0        0     3936 2023-04-25 13:12:44.858691 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/font/font_only.py
+-rw-r--r--   0        0        0     5021 2023-04-25 13:12:44.859691 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/font/font_position.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.997094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/highlight/__init__.py
+-rw-r--r--   0        0        0     3257 2023-04-25 13:12:44.861692 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/highlight/highlight.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.998094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/fill/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:08.999094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/fill/area/__init__.py
+-rw-r--r--   0        0        0     5010 2023-04-06 02:13:48.439067 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/fill/area/img.py
+-rw-r--r--   0        0        0      686 2023-04-06 02:13:09.000093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/fill/fill_style_base_multi.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.001095 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.001095 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/area/__init__.py
+-rw-r--r--   0        0        0     3731 2023-04-06 02:13:48.440068 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/area/color.py
+-rw-r--r--   0        0        0     6551 2023-04-06 02:13:48.441068 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/area/gradient.py
+-rw-r--r--   0        0        0     5763 2023-04-06 02:13:48.442065 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/area/hatch.py
+-rw-r--r--   0        0        0     6033 2023-04-06 02:13:09.004092 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/area/img.py
+-rw-r--r--   0        0        0     5246 2023-04-06 02:13:48.442065 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.005095 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/border/__init__.py
+-rw-r--r--   0        0        0     4498 2023-04-06 02:13:09.006094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/border/padding.py
+-rw-r--r--   0        0        0     4409 2023-04-06 02:13:48.443065 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/border/shadow.py
+-rw-r--r--   0        0        0     4309 2023-04-06 02:13:09.007094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/border/sides.py
+-rw-r--r--   0        0        0      742 2023-04-06 02:13:09.008093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/frame_style_base_multi.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.009094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/frame_type/__init__.py
+-rw-r--r--   0        0        0     3280 2023-04-06 02:13:09.009094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/frame_type/anchor.py
+-rw-r--r--   0        0        0     3895 2023-04-06 02:13:09.010094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/frame_type/position.py
+-rw-r--r--   0        0        0     3568 2023-04-06 02:13:09.011093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/frame_type/size.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.011093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/options/__init__.py
+-rw-r--r--   0        0        0     3294 2023-04-06 02:13:09.012094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/options/align.py
+-rw-r--r--   0        0        0     3551 2023-04-06 02:13:09.012094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/options/properties.py
+-rw-r--r--   0        0        0     3335 2023-04-06 02:13:09.013101 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/options/protect.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.013101 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/transparent/__init__.py
+-rw-r--r--   0        0        0     4635 2023-04-06 02:13:09.040094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/transparent/gradient.py
+-rw-r--r--   0        0        0     3782 2023-04-06 02:13:09.041093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/transparent/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.041093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/wrap/__init__.py
+-rw-r--r--   0        0        0     3838 2023-04-06 02:13:09.042094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/wrap/options.py
+-rw-r--r--   0        0        0     3185 2023-04-06 02:13:09.043094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/wrap/settings.py
+-rw-r--r--   0        0        0     3864 2023-04-06 02:13:09.043094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/wrap/spacing.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.044094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.044094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/area/__init__.py
+-rw-r--r--   0        0        0     4473 2023-04-28 14:55:36.888820 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/area/color.py
+-rw-r--r--   0        0        0     6319 2023-04-28 14:56:04.056825 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/area/gradient.py
+-rw-r--r--   0        0        0     5168 2023-04-28 14:56:24.884697 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/area/hatch.py
+-rw-r--r--   0        0        0     6062 2023-04-28 14:56:44.877265 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/area/img.py
+-rw-r--r--   0        0        0     4950 2023-04-28 14:57:03.244244 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.047093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/border/__init__.py
+-rw-r--r--   0        0        0     3905 2023-04-06 02:13:09.048094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/border/padding.py
+-rw-r--r--   0        0        0     5049 2023-04-06 02:13:48.447065 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/border/shadow.py
+-rw-r--r--   0        0        0     3829 2023-04-06 02:13:09.049093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/border/sides.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.049093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.049093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/area/__init__.py
+-rw-r--r--   0        0        0      892 2023-04-06 02:13:48.447065 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/area/color.py
+-rw-r--r--   0        0        0     1072 2023-04-06 02:13:48.448067 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/area/gradient.py
+-rw-r--r--   0        0        0     1007 2023-04-06 02:13:48.449065 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/area/hatch.py
+-rw-r--r--   0        0        0     1346 2023-04-06 02:13:48.449065 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/area/img.py
+-rw-r--r--   0        0        0     1077 2023-04-06 02:13:48.450068 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.052094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/border/__init__.py
+-rw-r--r--   0        0        0     1052 2023-04-06 02:13:48.510066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/border/padding.py
+-rw-r--r--   0        0        0      976 2023-04-06 02:13:48.511066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/border/shadow.py
+-rw-r--r--   0        0        0      971 2023-04-06 02:13:48.511066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/border/sides.py
+-rw-r--r--   0        0        0     1176 2023-04-06 02:13:48.512066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/footer.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.055093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/transparency/__init__.py
+-rw-r--r--   0        0        0     1095 2023-04-06 02:13:48.513065 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/transparency/gradient.py
+-rw-r--r--   0        0        0      994 2023-04-06 02:13:48.513065 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/transparency/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.056092 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.057094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/area/__init__.py
+-rw-r--r--   0        0        0     5331 2023-04-06 02:13:48.514066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/area/color.py
+-rw-r--r--   0        0        0     7596 2023-04-06 02:13:48.515074 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/area/gradient.py
+-rw-r--r--   0        0        0     6455 2023-04-06 02:13:48.515074 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/area/hatch.py
+-rw-r--r--   0        0        0     7602 2023-04-06 02:13:48.516066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/area/img.py
+-rw-r--r--   0        0        0     6295 2023-04-06 02:13:48.517067 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.060095 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/border/__init__.py
+-rw-r--r--   0        0        0     6729 2023-04-06 02:13:48.517067 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/border/padding.py
+-rw-r--r--   0        0        0     6148 2023-04-06 02:13:48.518065 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/border/shadow.py
+-rw-r--r--   0        0        0     6403 2023-04-06 02:13:48.519066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/border/sides.py
+-rw-r--r--   0        0        0     7279 2023-04-06 02:13:48.519066 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/header.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.063098 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/transparency/__init__.py
+-rw-r--r--   0        0        0     5959 2023-04-06 02:13:48.520064 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/transparency/gradient.py
+-rw-r--r--   0        0        0     4560 2023-04-06 02:13:48.521067 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/transparency/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.064093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/page/__init__.py
+-rw-r--r--   0        0        0     9183 2023-04-28 13:03:13.282972 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/page/layout_settings.py
+-rw-r--r--   0        0        0     3898 2023-04-28 13:03:46.509070 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/page/margins.py
+-rw-r--r--   0        0        0     4507 2023-04-28 13:04:13.000087 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/page/paper_format.py
+-rw-r--r--   0        0        0      778 2023-04-06 02:13:09.066093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/page_style_base_multi.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.067093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/transparency/__init__.py
+-rw-r--r--   0        0        0     3915 2023-04-28 15:53:25.241244 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/transparency/gradient.py
+-rw-r--r--   0        0        0     3425 2023-04-28 15:53:04.854247 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/transparency/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.069094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.069094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/align/__init__.py
+-rw-r--r--   0        0        0     4675 2023-04-26 02:29:49.580425 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/align/alignment.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.070093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/area/__init__.py
+-rw-r--r--   0        0        0     2890 2023-04-26 02:29:49.581423 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/area/color.py
+-rw-r--r--   0        0        0     5718 2023-04-26 02:29:49.582426 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/area/gradient.py
+-rw-r--r--   0        0        0     5490 2023-04-26 02:29:49.583426 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/area/hatch.py
+-rw-r--r--   0        0        0     5155 2023-04-26 02:29:49.584425 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/area/img.py
+-rw-r--r--   0        0        0     4995 2023-04-26 02:29:49.585427 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/area/pattern.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.073094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/border/__init__.py
+-rw-r--r--   0        0        0     4597 2023-04-26 02:29:49.586424 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/border/borders.py
+-rw-r--r--   0        0        0     4007 2023-04-26 02:29:49.589427 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/border/padding.py
+-rw-r--r--   0        0        0     4070 2023-04-26 02:29:49.590432 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/border/shadow.py
+-rw-r--r--   0        0        0     3906 2023-04-26 02:29:49.591426 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/border/sides.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.087092 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/drop_cap/__init__.py
+-rw-r--r--   0        0        0     4050 2023-04-27 02:41:12.824613 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/drop_cap/drop_caps.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.088093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/font/__init__.py
+-rw-r--r--   0        0        0     5523 2023-04-27 02:41:12.825609 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/font/font_effects.py
+-rw-r--r--   0        0        0     3879 2023-04-27 02:41:12.826609 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/font/font_only.py
+-rw-r--r--   0        0        0     5099 2023-04-27 02:41:12.827609 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/font/font_position.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.090093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/highlight/__init__.py
+-rw-r--r--   0        0        0     3320 2023-04-27 02:41:12.829610 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/highlight/highlight.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.091092 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/indent_space/__init__.py
+-rw-r--r--   0        0        0     3883 2023-04-27 02:41:12.830611 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/indent_space/indent.py
+-rw-r--r--   0        0        0     4292 2023-04-27 02:41:12.832620 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/indent_space/line_spacing.py
+-rw-r--r--   0        0        0     3723 2023-04-27 02:41:12.833610 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/indent_space/spacing.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.093094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/outline_list/__init__.py
+-rw-r--r--   0        0        0     4237 2023-04-26 02:29:49.592425 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/outline_list/line_num.py
+-rw-r--r--   0        0        0     8473 2023-04-27 02:41:12.834608 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/outline_list/list_style.py
+-rw-r--r--   0        0        0     3386 2023-04-26 02:29:49.595427 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/outline_list/outline.py
+-rw-r--r--   0        0        0      837 2023-04-06 02:13:09.096093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/para_style_base_multi.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.096093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/tabs/__init__.py
+-rw-r--r--   0        0        0     5520 2023-04-27 02:41:12.835610 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/tabs/tabs.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.097093 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/text_flow/__init__.py
+-rw-r--r--   0        0        0     3446 2023-04-27 02:41:12.837618 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/text_flow/breaks.py
+-rw-r--r--   0        0        0     3607 2023-04-27 02:41:12.838610 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/text_flow/flow_options.py
+-rw-r--r--   0        0        0     3735 2023-04-27 02:41:12.839609 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/text_flow/hyphenation.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.111094 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/transparent/__init__.py
+-rw-r--r--   0        0        0     3929 2023-04-27 02:41:12.840625 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/transparent/gradient.py
+-rw-r--r--   0        0        0     3394 2023-04-27 02:41:12.841609 ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/transparent/transparency.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:09.112093 ooo_dev_tools-0.9.7/ooodev/format/inner/preset/__init__.py
+-rw-r--r--   0        0        0    28652 2023-04-23 13:05:06.147315 ooo_dev_tools-0.9.7/ooodev/format/inner/preset/preset_border_line.py
+-rw-r--r--   0        0        0     8819 2023-04-06 02:13:48.593066 ooo_dev_tools-0.9.7/ooodev/format/inner/preset/preset_gradient.py
+-rw-r--r--   0        0        0     7403 2023-04-06 02:13:48.594065 ooo_dev_tools-0.9.7/ooodev/format/inner/preset/preset_hatch.py
+-rw-r--r--   0        0        0  1674033 2023-04-06 02:13:09.129092 ooo_dev_tools-0.9.7/ooodev/format/inner/preset/preset_image.py
+-rw-r--r--   0        0        0     1257 2023-04-06 02:13:09.135093 ooo_dev_tools-0.9.7/ooodev/format/inner/preset/preset_paper_format.py
+-rw-r--r--   0        0        0     5884 2023-04-06 02:13:09.137094 ooo_dev_tools-0.9.7/ooodev/format/inner/preset/preset_pattern.py
+-rw-r--r--   0        0        0    53215 2023-04-23 13:05:06.149315 ooo_dev_tools-0.9.7/ooodev/format/inner/style_base.py
+-rw-r--r--   0        0        0    17583 2023-04-23 13:05:06.150314 ooo_dev_tools-0.9.7/ooodev/format/readme.md
+-rw-r--r--   0        0        0      738 2023-04-06 02:13:09.175094 ooo_dev_tools-0.9.7/ooodev/format/styler.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.738588 ooo_dev_tools-0.9.7/ooodev/format/writer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.738588 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.739586 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/char/__init__.py
+-rw-r--r--   0        0        0      888 2023-04-28 19:00:41.401047 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/char/borders/__init__.py
+-rw-r--r--   0        0        0     1591 2023-04-28 19:01:23.556876 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/char/font/__init__.py
+-rw-r--r--   0        0        0      129 2023-04-06 02:13:09.177094 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/char/highlight/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-28 19:02:01.196489 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/char/hyperlink/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.741673 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/frame/__init__.py
+-rw-r--r--   0        0        0     1805 2023-04-28 19:02:35.199488 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/frame/area/__init__.py
+-rw-r--r--   0        0        0      598 2023-04-28 19:02:57.792062 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/frame/borders/__init__.py
+-rw-r--r--   0        0        0      335 2023-04-28 19:04:02.648799 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/frame/hyperlink/__init__.py
+-rw-r--r--   0        0        0      614 2023-04-28 19:04:54.093354 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/frame/options/__init__.py
+-rw-r--r--   0        0        0      584 2023-04-06 02:13:09.184095 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/frame/transparency/__init__.py
+-rw-r--r--   0        0        0     1266 2023-04-28 19:07:14.533084 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/frame/type/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-06 02:13:09.185094 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/frame/wrap/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.753585 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/image/__init__.py
+-rw-r--r--   0        0        0     1805 2023-04-28 19:08:05.841183 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/image/area/__init__.py
+-rw-r--r--   0        0        0      598 2023-04-28 19:08:25.147181 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/image/borders/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-06 02:13:09.188095 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/image/crop/__init__.py
+-rw-r--r--   0        0        0      337 2023-04-28 19:09:40.621396 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/image/hyperlink/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-28 19:09:53.230170 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/image/image/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-06 02:13:09.190093 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/image/options/__init__.py
+-rw-r--r--   0        0        0      584 2023-04-06 02:13:09.191094 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/image/transparency/__init__.py
+-rw-r--r--   0        0        0     1266 2023-04-28 19:11:19.877175 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/image/type/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-06 02:13:09.192094 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/image/wrap/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.758699 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/obj/__init__.py
+-rw-r--r--   0        0        0     1805 2023-04-28 19:11:54.800233 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/obj/area/__init__.py
+-rw-r--r--   0        0        0      598 2023-04-28 19:12:13.627216 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/obj/borders/__init__.py
+-rw-r--r--   0        0        0      335 2023-04-28 19:12:27.551214 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/obj/hyperlink/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-06 02:13:09.196094 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/obj/options/__init__.py
+-rw-r--r--   0        0        0      584 2023-04-06 02:13:09.197093 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/obj/transparency/__init__.py
+-rw-r--r--   0        0        0     1266 2023-04-28 19:13:03.782866 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/obj/type/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-06 02:13:09.198094 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/obj/wrap/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 02:13:48.596069 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/page/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-06 02:13:48.597066 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/page/footer/__init__.py
+-rw-r--r--   0        0        0     1743 2023-04-06 02:13:48.598067 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/page/footer/area/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-06 02:13:48.598067 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/page/header/__init__.py
+-rw-r--r--   0        0        0     1743 2023-04-06 02:13:48.599067 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/page/header/area/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.766787 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/para/__init__.py
+-rw-r--r--   0        0        0      580 2023-04-28 19:14:14.586205 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/para/alignment/__init__.py
+-rw-r--r--   0        0        0     1871 2023-04-28 19:14:24.029203 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/para/area/__init__.py
+-rw-r--r--   0        0        0      800 2023-04-28 19:14:37.486204 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/para/borders/__init__.py
+-rw-r--r--   0        0        0      205 2023-04-06 02:13:09.204094 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/para/drop_caps/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-28 19:15:27.977931 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/para/indent_space/__init__.py
+-rw-r--r--   0        0        0      504 2023-04-28 19:15:44.675037 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/para/outline_list/__init__.py
+-rw-r--r--   0        0        0      253 2023-04-28 19:15:52.559040 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/para/tabs/__init__.py
+-rw-r--r--   0        0        0      406 2023-04-06 02:13:09.207091 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/para/text_flow/__init__.py
+-rw-r--r--   0        0        0      276 2023-04-28 19:16:25.389906 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/para/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.773090 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/shape/__init__.py
+-rw-r--r--   0        0        0     1805 2023-04-28 19:16:42.331628 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/shape/area/__init__.py
+-rw-r--r--   0        0        0      374 2023-04-28 19:17:06.425625 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/shape/shadow/__init__.py
+-rw-r--r--   0        0        0      584 2023-04-06 02:13:09.223094 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/shape/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.775216 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/table/__init__.py
+-rw-r--r--   0        0        0     1099 2023-04-25 00:03:57.178376 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/table/background/__init__.py
+-rw-r--r--   0        0        0      769 2023-04-25 00:03:57.179369 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/table/borders/__init__.py
+-rw-r--r--   0        0        0      247 2023-04-28 19:17:36.117625 ooo_dev_tools-0.9.7/ooodev/format/writer/direct/table/properties/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.776595 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.777629 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/char/__init__.py
+-rw-r--r--   0        0        0     1012 2023-04-25 13:12:44.869693 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/char/borders/__init__.py
+-rw-r--r--   0        0        0     1521 2023-04-25 13:12:44.870691 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/char/font/__init__.py
+-rw-r--r--   0        0        0      328 2023-04-28 18:59:31.183716 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/char/highlight/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.779585 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/frame/__init__.py
+-rw-r--r--   0        0        0     2167 2023-04-28 19:18:31.553469 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/frame/area/__init__.py
+-rw-r--r--   0        0        0      969 2023-04-28 19:19:12.144867 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/frame/borders/__init__.py
+-rw-r--r--   0        0        0      911 2023-04-28 19:22:22.028085 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/frame/options/__init__.py
+-rw-r--r--   0        0        0      797 2023-04-28 19:22:39.752087 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/frame/transparency/__init__.py
+-rw-r--r--   0        0        0     1649 2023-04-28 19:23:59.085998 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/frame/type/__init__.py
+-rw-r--r--   0        0        0      756 2023-04-28 19:24:57.534700 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/frame/wrap/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.783676 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/__init__.py
+-rw-r--r--   0        0        0     2350 2023-04-28 15:23:32.352383 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/area/__init__.py
+-rw-r--r--   0        0        0      983 2023-04-28 18:58:57.606332 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/borders/__init__.py
+-rw-r--r--   0        0        0      321 2023-04-06 02:13:09.237093 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/footer/__init__.py
+-rw-r--r--   0        0        0     2246 2023-04-28 19:25:33.253830 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/footer/area/__init__.py
+-rw-r--r--   0        0        0     1025 2023-04-28 19:25:56.063254 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/footer/borders/__init__.py
+-rw-r--r--   0        0        0      957 2023-04-28 19:26:07.353251 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/footer/transparency/__init__.py
+-rw-r--r--   0        0        0      321 2023-04-06 02:13:09.239092 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/header/__init__.py
+-rw-r--r--   0        0        0     2246 2023-04-28 19:26:30.760255 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/header/area/__init__.py
+-rw-r--r--   0        0        0     1026 2023-04-28 19:26:46.019168 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/header/borders/__init__.py
+-rw-r--r--   0        0        0      957 2023-04-28 19:26:56.558153 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/header/transparency/__init__.py
+-rw-r--r--   0        0        0     1088 2023-04-28 15:20:50.307775 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/page/__init__.py
+-rw-r--r--   0        0        0     3526 2023-04-06 02:13:09.243093 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/page_style_base.py
+-rw-r--r--   0        0        0     3939 2023-04-06 02:13:09.246092 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/page_style_base_multi.py
+-rw-r--r--   0        0        0      920 2023-04-28 15:19:40.611540 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/transparency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 18:09:12.792731 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/__init__.py
+-rw-r--r--   0        0        0      745 2023-04-26 02:29:49.596427 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/alignment/__init__.py
+-rw-r--r--   0        0        0     2047 2023-04-28 19:27:39.767154 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/area/__init__.py
+-rw-r--r--   0        0        0     1190 2023-04-26 02:29:49.597426 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/borders/__init__.py
+-rw-r--r--   0        0        0      385 2023-04-27 02:41:12.843610 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/drop_caps/__init__.py
+-rw-r--r--   0        0        0     1523 2023-04-27 02:41:12.844610 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/font/__init__.py
+-rw-r--r--   0        0        0      301 2023-04-27 02:41:12.845609 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/highlight/__init__.py
+-rw-r--r--   0        0        0      817 2023-04-27 02:41:12.847613 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/indent_space/__init__.py
+-rw-r--r--   0        0        0      892 2023-04-27 02:41:12.863609 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/outline_list/__init__.py
+-rw-r--r--   0        0        0      417 2023-04-27 02:41:12.879608 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/tabs/__init__.py
+-rw-r--r--   0        0        0      800 2023-04-27 02:41:12.880609 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/text_flow/__init__.py
+-rw-r--r--   0        0        0      881 2023-04-27 02:41:12.881608 ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/transparency/__init__.py
+-rw-r--r--   0        0        0      750 2023-04-06 02:13:09.300094 ooo_dev_tools-0.9.7/ooodev/format/writer/style/__init__.py
+-rw-r--r--   0        0        0      136 2023-04-28 19:29:36.036733 ooo_dev_tools-0.9.7/ooodev/format/writer/style/bullet_list/__init__.py
+-rw-r--r--   0        0        0     4599 2023-04-23 13:05:06.194315 ooo_dev_tools-0.9.7/ooodev/format/writer/style/bullet_list/bullet_list.py
+-rw-r--r--   0        0        0      127 2023-04-28 19:29:58.067335 ooo_dev_tools-0.9.7/ooodev/format/writer/style/char/__init__.py
+-rw-r--r--   0        0        0     7058 2023-04-23 13:05:06.195315 ooo_dev_tools-0.9.7/ooodev/format/writer/style/char/char.py
+-rw-r--r--   0        0        0       60 2023-04-02 18:09:12.802395 ooo_dev_tools-0.9.7/ooodev/format/writer/style/char/kind/__init__.py
+-rw-r--r--   0        0        0     1135 2023-04-06 02:13:09.303093 ooo_dev_tools-0.9.7/ooodev/format/writer/style/char/kind/style_char_kind.py
+-rw-r--r--   0        0        0      118 2023-04-28 19:30:11.346332 ooo_dev_tools-0.9.7/ooodev/format/writer/style/frame/__init__.py
+-rw-r--r--   0        0        0     3704 2023-04-06 02:13:48.603067 ooo_dev_tools-0.9.7/ooodev/format/writer/style/frame/frame.py
+-rw-r--r--   0        0        0      353 2023-04-06 02:13:09.305109 ooo_dev_tools-0.9.7/ooodev/format/writer/style/frame/style_frame_kind.py
+-rw-r--r--   0        0        0       60 2023-04-02 18:09:12.804657 ooo_dev_tools-0.9.7/ooodev/format/writer/style/lst/__init__.py
+-rw-r--r--   0        0        0      791 2023-04-06 02:13:09.306094 ooo_dev_tools-0.9.7/ooodev/format/writer/style/lst/style_list_kind.py
+-rw-r--r--   0        0        0      136 2023-04-28 19:30:30.975334 ooo_dev_tools-0.9.7/ooodev/format/writer/style/page/__init__.py
+-rw-r--r--   0        0        0       79 2023-04-06 02:13:09.308096 ooo_dev_tools-0.9.7/ooodev/format/writer/style/page/kind/__init__.py
+-rw-r--r--   0        0        0      412 2023-04-06 02:13:09.309094 ooo_dev_tools-0.9.7/ooodev/format/writer/style/page/kind/writer_style_page_kind.py
+-rw-r--r--   0        0        0     4711 2023-04-06 02:13:48.605068 ooo_dev_tools-0.9.7/ooodev/format/writer/style/page/page.py
+-rw-r--r--   0        0        0      111 2023-04-28 19:30:43.544020 ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/__init__.py
+-rw-r--r--   0        0        0      579 2023-04-02 18:09:12.808625 ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/__init__.py
+-rw-r--r--   0        0        0      335 2023-04-06 02:13:09.310097 ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_chapter_kind.py
+-rw-r--r--   0        0        0      260 2023-04-06 02:13:09.311093 ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_para_cond_kind.py
+-rw-r--r--   0        0        0     1225 2023-04-06 02:13:09.312094 ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_para_html_kind.py
+-rw-r--r--   0        0        0     2105 2023-04-06 02:13:09.312094 ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_para_index_kind.py
+-rw-r--r--   0        0        0     4274 2023-04-25 18:58:24.159468 ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_para_kind.py
+-rw-r--r--   0        0        0     2492 2023-04-06 02:13:09.314095 ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_para_list_kind.py
+-rw-r--r--   0        0        0     1139 2023-04-06 02:13:09.316093 ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_para_special_kind.py
+-rw-r--r--   0        0        0     1278 2023-04-06 02:13:09.317099 ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_para_text_kind.py
+-rw-r--r--   0        0        0    11566 2023-04-23 13:05:06.196317 ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/para.py
+-rw-r--r--   0        0        0      218 2022-11-22 00:28:23.283709 ooo_dev_tools-0.9.7/ooodev/formatters/__init__.py
+-rw-r--r--   0        0        0     1185 2022-11-22 00:28:23.284709 ooo_dev_tools-0.9.7/ooodev/formatters/format_list_item.py
+-rw-r--r--   0        0        0     1101 2022-11-22 00:28:23.284709 ooo_dev_tools-0.9.7/ooodev/formatters/format_string.py
+-rw-r--r--   0        0        0     2540 2022-11-22 00:28:23.285710 ooo_dev_tools-0.9.7/ooodev/formatters/format_table_item.py
+-rw-r--r--   0        0        0     3182 2022-11-22 00:28:23.285710 ooo_dev_tools-0.9.7/ooodev/formatters/formatter_list.py
+-rw-r--r--   0        0        0    10394 2023-04-06 02:13:09.319094 ooo_dev_tools-0.9.7/ooodev/formatters/formatter_table.py
+-rw-r--r--   0        0        0      130 2022-11-22 00:28:23.287709 ooo_dev_tools-0.9.7/ooodev/formatters/only_ignore_kind.py
+-rw-r--r--   0        0        0      196 2022-11-22 00:28:23.287709 ooo_dev_tools-0.9.7/ooodev/formatters/string_kind.py
+-rw-r--r--   0        0        0      720 2022-11-22 00:28:23.288717 ooo_dev_tools-0.9.7/ooodev/formatters/table_item_kind.py
+-rw-r--r--   0        0        0     4482 2022-11-22 00:28:23.289713 ooo_dev_tools-0.9.7/ooodev/formatters/table_item_processer.py
+-rw-r--r--   0        0        0      336 2022-11-22 00:28:23.290711 ooo_dev_tools-0.9.7/ooodev/formatters/table_rule_kind.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.797175 ooo_dev_tools-0.9.7/ooodev/lazy/__init__.py
+-rw-r--r--   0        0        0     1551 2022-07-24 03:34:34.541590 ooo_dev_tools-0.9.7/ooodev/lazy/lazy_import.py
+-rw-r--r--   0        0        0        0 2022-06-09 05:52:04.176192 ooo_dev_tools-0.9.7/ooodev/listeners/__init__.py
+-rw-r--r--   0        0        0     1130 2022-07-20 01:40:32.577461 ooo_dev_tools-0.9.7/ooodev/listeners/x_event_adapter.py
+-rw-r--r--   0        0        0     1402 2022-07-20 01:40:32.578458 ooo_dev_tools-0.9.7/ooodev/listeners/x_modify_adapter.py
+-rw-r--r--   0        0        0     1355 2022-08-23 05:01:45.222321 ooo_dev_tools-0.9.7/ooodev/listeners/x_selection_change_adapter.py
+-rw-r--r--   0        0        0     1827 2022-07-20 01:40:32.580453 ooo_dev_tools-0.9.7/ooodev/listeners/x_terminate_adapter.py
+-rw-r--r--   0        0        0     2034 2022-07-20 01:40:32.581450 ooo_dev_tools-0.9.7/ooodev/listeners/x_top_window_adapter.py
+-rw-r--r--   0        0        0        0 2022-06-09 05:52:04.177777 ooo_dev_tools-0.9.7/ooodev/meta/__init__.py
+-rw-r--r--   0        0        0      518 2023-04-02 18:09:12.815585 ooo_dev_tools-0.9.7/ooodev/meta/class_property_readonly.py
+-rw-r--r--   0        0        0      545 2023-04-02 18:09:12.820755 ooo_dev_tools-0.9.7/ooodev/meta/deleted_attrib.py
+-rw-r--r--   0        0        0     1617 2023-04-02 18:09:12.821833 ooo_dev_tools-0.9.7/ooodev/meta/deleted_enum_meta.py
+-rw-r--r--   0        0        0      915 2023-04-02 18:09:12.822581 ooo_dev_tools-0.9.7/ooodev/meta/disabled_method.py
+-rw-r--r--   0        0        0      241 2022-07-14 20:40:23.800284 ooo_dev_tools-0.9.7/ooodev/meta/singleton.py
+-rw-r--r--   0        0        0     2135 2023-01-10 14:23:45.008570 ooo_dev_tools-0.9.7/ooodev/meta/static_meta.py
+-rw-r--r--   0        0        0      518 2023-04-02 18:09:12.822581 ooo_dev_tools-0.9.7/ooodev/meta/static_prop.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.801281 ooo_dev_tools-0.9.7/ooodev/mock/__init__.py
+-rw-r--r--   0        0        0      559 2022-07-14 20:40:23.801281 ooo_dev_tools-0.9.7/ooodev/mock/mock_g.py
+-rw-r--r--   0        0        0      579 2022-10-04 00:14:04.239070 ooo_dev_tools-0.9.7/ooodev/mock/unohelper.py
+-rw-r--r--   0        0        0        0 2022-06-09 05:51:34.370860 ooo_dev_tools-0.9.7/ooodev/office/__init__.py
+-rw-r--r--   0        0        0   265485 2023-04-23 13:05:06.199317 ooo_dev_tools-0.9.7/ooodev/office/calc.py
+-rw-r--r--   0        0        0    45621 2023-04-06 02:13:09.324093 ooo_dev_tools-0.9.7/ooodev/office/chart.py
+-rw-r--r--   0        0        0   114364 2023-04-23 13:05:06.202317 ooo_dev_tools-0.9.7/ooodev/office/chart2.py
+-rw-r--r--   0        0        0   135614 2023-04-06 02:13:48.632065 ooo_dev_tools-0.9.7/ooodev/office/draw.py
+-rw-r--r--   0        0        0   151392 2023-04-28 12:39:00.168729 ooo_dev_tools-0.9.7/ooodev/office/write.py
+-rw-r--r--   0        0        0        0 2022-07-14 20:40:23.805270 ooo_dev_tools-0.9.7/ooodev/proto/__init__.py
+-rw-r--r--   0        0        0      626 2023-04-06 02:13:09.329093 ooo_dev_tools-0.9.7/ooodev/proto/dispatch_shape.py
+-rw-r--r--   0        0        0     1453 2023-04-06 02:13:09.329093 ooo_dev_tools-0.9.7/ooodev/proto/event_observer.py
+-rw-r--r--   0        0        0      450 2023-04-06 02:13:09.330101 ooo_dev_tools-0.9.7/ooodev/proto/size_obj.py
+-rw-r--r--   0        0        0     2394 2023-04-06 02:13:09.331094 ooo_dev_tools-0.9.7/ooodev/proto/style_obj.py
+-rw-r--r--   0        0        0      636 2023-04-06 02:13:48.635066 ooo_dev_tools-0.9.7/ooodev/theme/__init__.py
+-rw-r--r--   0        0        0     1604 2023-04-07 18:06:32.211989 ooo_dev_tools-0.9.7/ooodev/theme/theme.py
+-rw-r--r--   0        0        0     2212 2023-04-06 02:13:48.638067 ooo_dev_tools-0.9.7/ooodev/theme/theme_basic.py
+-rw-r--r--   0        0        0     4152 2023-04-06 02:13:48.639065 ooo_dev_tools-0.9.7/ooodev/theme/theme_calc.py
+-rw-r--r--   0        0        0      865 2023-04-06 02:13:48.640067 ooo_dev_tools-0.9.7/ooodev/theme/theme_draw.py
+-rw-r--r--   0        0        0     4342 2023-04-06 02:13:48.640067 ooo_dev_tools-0.9.7/ooodev/theme/theme_general.py
+-rw-r--r--   0        0        0     1416 2023-04-06 02:13:48.641076 ooo_dev_tools-0.9.7/ooodev/theme/theme_html.py
+-rw-r--r--   0        0        0     3982 2023-04-06 02:13:48.641076 ooo_dev_tools-0.9.7/ooodev/theme/theme_rpt_builder.py
+-rw-r--r--   0        0        0     2215 2023-04-06 02:13:48.642067 ooo_dev_tools-0.9.7/ooodev/theme/theme_sql.py
+-rw-r--r--   0        0        0     4975 2023-04-06 02:13:48.642067 ooo_dev_tools-0.9.7/ooodev/theme/theme_text_doc.py
+-rw-r--r--   0        0        0      820 2023-04-23 13:05:06.206317 ooo_dev_tools-0.9.7/ooodev/units/__init__.py
+-rw-r--r--   0        0        0     5979 2023-04-23 13:05:06.206317 ooo_dev_tools-0.9.7/ooodev/units/unit_cm.py
+-rw-r--r--   0        0        0     8844 2023-04-06 02:13:09.334092 ooo_dev_tools-0.9.7/ooodev/units/unit_convert.py
+-rw-r--r--   0        0        0     5352 2023-04-23 13:05:06.208316 ooo_dev_tools-0.9.7/ooodev/units/unit_inch.py
+-rw-r--r--   0        0        0     5394 2023-04-23 13:05:06.209317 ooo_dev_tools-0.9.7/ooodev/units/unit_inch10.py
+-rw-r--r--   0        0        0     5447 2023-04-23 13:05:06.210316 ooo_dev_tools-0.9.7/ooodev/units/unit_inch100.py
+-rw-r--r--   0        0        0     6082 2023-04-23 13:05:06.211316 ooo_dev_tools-0.9.7/ooodev/units/unit_inch1000.py
+-rw-r--r--   0        0        0     5897 2023-04-23 13:05:06.212316 ooo_dev_tools-0.9.7/ooodev/units/unit_mm.py
+-rw-r--r--   0        0        0     6131 2023-04-23 13:05:06.213315 ooo_dev_tools-0.9.7/ooodev/units/unit_mm10.py
+-rw-r--r--   0        0        0     6677 2023-04-23 13:05:06.214316 ooo_dev_tools-0.9.7/ooodev/units/unit_mm100.py
+-rw-r--r--   0        0        0     1329 2023-04-06 02:13:48.644066 ooo_dev_tools-0.9.7/ooodev/units/unit_obj.py
+-rw-r--r--   0        0        0     5700 2023-04-23 13:05:06.215315 ooo_dev_tools-0.9.7/ooodev/units/unit_pt.py
+-rw-r--r--   0        0        0     5960 2023-04-23 13:05:06.216316 ooo_dev_tools-0.9.7/ooodev/units/unit_px.py
+-rw-r--r--   0        0        0     1907 2022-07-14 20:40:23.806682 ooo_dev_tools-0.9.7/ooodev/utils/__init__.py
+-rw-r--r--   0        0        0    26819 2023-04-06 02:13:48.645065 ooo_dev_tools-0.9.7/ooodev/utils/color.py
+-rw-r--r--   0        0        0        0 2022-10-27 15:27:12.052996 ooo_dev_tools-0.9.7/ooodev/utils/data_type/__init__.py
+-rw-r--r--   0        0        0     2758 2023-04-02 18:09:12.852582 ooo_dev_tools-0.9.7/ooodev/utils/data_type/angle.py
+-rw-r--r--   0        0        0     3820 2022-12-17 01:13:14.728078 ooo_dev_tools-0.9.7/ooodev/utils/data_type/base_float_value.py
+-rw-r--r--   0        0        0     3785 2023-04-02 18:09:12.853581 ooo_dev_tools-0.9.7/ooodev/utils/data_type/base_int_value.py
+-rw-r--r--   0        0        0     1280 2023-04-02 18:09:12.874577 ooo_dev_tools-0.9.7/ooodev/utils/data_type/byte.py
+-rw-r--r--   0        0        0     1298 2023-04-02 18:09:12.875872 ooo_dev_tools-0.9.7/ooodev/utils/data_type/byte_signed.py
+-rw-r--r--   0        0        0    14993 2023-04-02 18:09:12.876578 ooo_dev_tools-0.9.7/ooodev/utils/data_type/cell_obj.py
+-rw-r--r--   0        0        0     3298 2023-04-02 18:09:12.877797 ooo_dev_tools-0.9.7/ooodev/utils/data_type/cell_values.py
+-rw-r--r--   0        0        0    10497 2023-04-06 02:13:09.375094 ooo_dev_tools-0.9.7/ooodev/utils/data_type/col_obj.py
+-rw-r--r--   0        0        0      522 2023-04-02 18:09:12.879580 ooo_dev_tools-0.9.7/ooodev/utils/data_type/color_range.py
+-rw-r--r--   0        0        0      195 2022-11-13 02:25:58.188785 ooo_dev_tools-0.9.7/ooodev/utils/data_type/dialog_title.py
+-rw-r--r--   0        0        0     1020 2023-04-02 18:09:12.880576 ooo_dev_tools-0.9.7/ooodev/utils/data_type/image_offset.py
+-rw-r--r--   0        0        0     1290 2023-04-02 18:09:12.882575 ooo_dev_tools-0.9.7/ooodev/utils/data_type/intensity.py
+-rw-r--r--   0        0        0      880 2023-04-06 02:13:09.376093 ooo_dev_tools-0.9.7/ooodev/utils/data_type/intensity_range.py
+-rw-r--r--   0        0        0      209 2023-04-02 18:09:12.884666 ooo_dev_tools-0.9.7/ooodev/utils/data_type/offset.py
+-rw-r--r--   0        0        0      431 2023-04-02 18:09:12.884666 ooo_dev_tools-0.9.7/ooodev/utils/data_type/point.py
+-rw-r--r--   0        0        0      482 2023-04-02 18:09:12.885575 ooo_dev_tools-0.9.7/ooodev/utils/data_type/point_positive.py
+-rw-r--r--   0        0        0     1282 2023-04-02 18:09:12.886577 ooo_dev_tools-0.9.7/ooodev/utils/data_type/poly_sides.py
+-rw-r--r--   0        0        0    22190 2023-04-06 02:13:09.377092 ooo_dev_tools-0.9.7/ooodev/utils/data_type/range_obj.py
+-rw-r--r--   0        0        0    15997 2023-04-06 02:13:09.402093 ooo_dev_tools-0.9.7/ooodev/utils/data_type/range_values.py
+-rw-r--r--   0        0        0     7314 2023-04-02 18:09:12.888579 ooo_dev_tools-0.9.7/ooodev/utils/data_type/row_obj.py
+-rw-r--r--   0        0        0     1993 2023-04-06 02:13:09.403093 ooo_dev_tools-0.9.7/ooodev/utils/data_type/size.py
+-rw-r--r--   0        0        0     3150 2023-04-27 15:20:03.727631 ooo_dev_tools-0.9.7/ooodev/utils/data_type/size_mm.py
+-rw-r--r--   0        0        0     1126 2023-04-02 18:09:12.890576 ooo_dev_tools-0.9.7/ooodev/utils/data_type/width_height_fraction.py
+-rw-r--r--   0        0        0      935 2023-04-02 18:09:12.891577 ooo_dev_tools-0.9.7/ooodev/utils/data_type/width_height_percent.py
+-rw-r--r--   0        0        0      270 2022-11-13 02:25:58.189784 ooo_dev_tools-0.9.7/ooodev/utils/data_type/window_title.py
+-rw-r--r--   0        0        0     5657 2022-12-10 17:01:36.559035 ooo_dev_tools-0.9.7/ooodev/utils/date_time_util.py
+-rw-r--r--   0        0        0        0 2022-10-27 15:27:12.055992 ooo_dev_tools-0.9.7/ooodev/utils/decorator/__init__.py
+-rw-r--r--   0        0        0     2737 2023-04-23 13:05:06.217315 ooo_dev_tools-0.9.7/ooodev/utils/decorator/enforce.py
+-rw-r--r--   0        0        0    24793 2023-04-06 02:13:09.404094 ooo_dev_tools-0.9.7/ooodev/utils/dialogs.py
+-rw-r--r--   0        0        0        0 2022-10-27 15:27:12.056992 ooo_dev_tools-0.9.7/ooodev/utils/dispatch/__init__.py
+-rw-r--r--   0        0        0     3178 2022-10-27 15:27:12.057993 ooo_dev_tools-0.9.7/ooodev/utils/dispatch/draw_drawing_dispatch.py
+-rw-r--r--   0        0        0     2806 2022-10-27 15:27:12.058992 ooo_dev_tools-0.9.7/ooodev/utils/dispatch/draw_view_dispatch.py
+-rw-r--r--   0        0        0     3180 2022-10-27 15:27:12.059993 ooo_dev_tools-0.9.7/ooodev/utils/dispatch/global_edit_dispatch.py
+-rw-r--r--   0        0        0     9772 2022-10-27 15:27:12.059993 ooo_dev_tools-0.9.7/ooodev/utils/dispatch/global_format_dispatch.py
+-rw-r--r--   0        0        0     2911 2022-10-27 15:27:12.060992 ooo_dev_tools-0.9.7/ooodev/utils/dispatch/global_view_dispatch.py
+-rw-r--r--   0        0        0    11843 2022-11-08 11:09:51.358105 ooo_dev_tools-0.9.7/ooodev/utils/dispatch/shape_dispatch_kind.py
+-rw-r--r--   0        0        0     1562 2022-07-24 03:34:47.720953 ooo_dev_tools-0.9.7/ooodev/utils/enum_helper.py
+-rw-r--r--   0        0        0    21457 2022-11-30 23:26:32.117139 ooo_dev_tools-0.9.7/ooodev/utils/file_io.py
+-rw-r--r--   0        0        0    44086 2023-04-06 02:13:48.646066 ooo_dev_tools-0.9.7/ooodev/utils/forms.py
+-rw-r--r--   0        0        0    21957 2023-04-02 18:09:12.895589 ooo_dev_tools-0.9.7/ooodev/utils/gallery.py
+-rw-r--r--   0        0        0     7499 2023-04-23 13:05:06.218316 ooo_dev_tools-0.9.7/ooodev/utils/gen_util.py
+-rw-r--r--   0        0        0    58887 2023-04-28 12:39:00.169729 ooo_dev_tools-0.9.7/ooodev/utils/gui.py
+-rw-r--r--   0        0        0     2062 2022-07-14 20:40:23.810268 ooo_dev_tools-0.9.7/ooodev/utils/image_transferable.py
+-rw-r--r--   0        0        0     3745 2022-07-24 03:34:34.555553 ooo_dev_tools-0.9.7/ooodev/utils/images.py
+-rw-r--r--   0        0        0    15354 2023-04-06 02:13:48.647065 ooo_dev_tools-0.9.7/ooodev/utils/images_lo.py
+-rw-r--r--   0        0        0    79006 2023-04-23 13:05:06.220317 ooo_dev_tools-0.9.7/ooodev/utils/info.py
+-rw-r--r--   0        0        0        0 2022-10-27 15:27:12.066994 ooo_dev_tools-0.9.7/ooodev/utils/kind/__init__.py
+-rw-r--r--   0        0        0      658 2022-11-05 19:28:56.359598 ooo_dev_tools-0.9.7/ooodev/utils/kind/axis_kind.py
+-rw-r--r--   0        0        0     2943 2022-11-05 19:28:56.360598 ooo_dev_tools-0.9.7/ooodev/utils/kind/chart2_data_role_kind.py
+-rw-r--r--   0        0        0     7423 2022-12-17 01:13:14.740079 ooo_dev_tools-0.9.7/ooodev/utils/kind/chart2_types.py
+-rw-r--r--   0        0        0     1061 2022-11-05 19:28:56.361599 ooo_dev_tools-0.9.7/ooodev/utils/kind/chart_diagram_kind.py
+-rw-r--r--   0        0        0     1979 2022-11-05 19:28:56.361599 ooo_dev_tools-0.9.7/ooodev/utils/kind/curve_kind.py
+-rw-r--r--   0        0        0      893 2022-11-05 19:28:56.362600 ooo_dev_tools-0.9.7/ooodev/utils/kind/data_point_label_type_kind.py
+-rw-r--r--   0        0        0      922 2022-11-05 19:28:56.363598 ooo_dev_tools-0.9.7/ooodev/utils/kind/data_point_lable_placement_kind.py
+-rw-r--r--   0        0        0     1921 2022-11-05 19:28:56.364600 ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_bitmap_kind.py
+-rw-r--r--   0        0        0     1510 2022-11-05 19:28:56.364600 ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_gradient_kind.py
+-rw-r--r--   0        0        0     1781 2022-11-05 19:28:56.365599 ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_hatching_kind.py
+-rw-r--r--   0        0        0     1053 2022-11-05 19:28:56.366599 ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_layer_kind.py
+-rw-r--r--   0        0        0     1343 2022-11-05 19:28:56.367602 ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_name_space_kind.py
+-rw-r--r--   0        0        0     2298 2022-11-05 19:28:56.368600 ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_shape_kind.py
+-rw-r--r--   0        0        0     1123 2022-11-05 19:28:56.369599 ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_slide_show_kind.py
+-rw-r--r--   0        0        0     2482 2022-11-05 19:28:56.370602 ooo_dev_tools-0.9.7/ooodev/utils/kind/form_component_kind.py
+-rw-r--r--   0        0        0     1778 2022-11-05 19:28:56.371600 ooo_dev_tools-0.9.7/ooodev/utils/kind/form_control_kind.py
+-rw-r--r--   0        0        0     1309 2022-11-05 19:28:56.371600 ooo_dev_tools-0.9.7/ooodev/utils/kind/gallery_kind.py
+-rw-r--r--   0        0        0      945 2022-11-05 19:28:56.372599 ooo_dev_tools-0.9.7/ooodev/utils/kind/gallery_search_by_kind.py
+-rw-r--r--   0        0        0      812 2022-11-05 19:28:56.373599 ooo_dev_tools-0.9.7/ooodev/utils/kind/glue_points_kind.py
+-rw-r--r--   0        0        0     2878 2022-11-08 11:08:31.782891 ooo_dev_tools-0.9.7/ooodev/utils/kind/graphic_arrow_style_kind.py
+-rw-r--r--   0        0        0     2131 2022-11-05 19:28:56.374601 ooo_dev_tools-0.9.7/ooodev/utils/kind/graphic_style_kind.py
+-rw-r--r--   0        0        0     1526 2022-11-30 23:26:32.119139 ooo_dev_tools-0.9.7/ooodev/utils/kind/info_paths_kind.py
+-rw-r--r--   0        0        0      209 2022-10-27 15:27:12.079996 ooo_dev_tools-0.9.7/ooodev/utils/kind/kind_base.py
+-rw-r--r--   0        0        0     2389 2022-11-13 02:25:58.191785 ooo_dev_tools-0.9.7/ooodev/utils/kind/kind_helper.py
+-rw-r--r--   0        0        0     1260 2022-11-05 19:28:56.376599 ooo_dev_tools-0.9.7/ooodev/utils/kind/line_style_name_kind.py
+-rw-r--r--   0        0        0     2202 2022-11-05 19:28:56.377600 ooo_dev_tools-0.9.7/ooodev/utils/kind/presentation_kind.py
+-rw-r--r--   0        0        0     1898 2022-11-13 02:25:58.191785 ooo_dev_tools-0.9.7/ooodev/utils/kind/presentation_layout_kind.py
+-rw-r--r--   0        0        0     1146 2022-11-05 19:28:56.377600 ooo_dev_tools-0.9.7/ooodev/utils/kind/search_match_kind.py
+-rw-r--r--   0        0        0     1183 2023-04-23 13:05:06.221317 ooo_dev_tools-0.9.7/ooodev/utils/kind/shape_base_point_kind.py
+-rw-r--r--   0        0        0      820 2022-11-05 19:28:56.378600 ooo_dev_tools-0.9.7/ooodev/utils/kind/shape_comb_kind.py
+-rw-r--r--   0        0        0    99082 2023-04-23 13:05:06.222317 ooo_dev_tools-0.9.7/ooodev/utils/lo.py
+-rw-r--r--   0        0        0     2783 2022-07-24 03:34:34.561536 ooo_dev_tools-0.9.7/ooodev/utils/lo_util.py
+-rw-r--r--   0        0        0     8437 2022-11-25 03:43:11.801371 ooo_dev_tools-0.9.7/ooodev/utils/paths.py
+-rw-r--r--   0        0        0    57557 2023-04-23 13:05:06.224316 ooo_dev_tools-0.9.7/ooodev/utils/props.py
+-rw-r--r--   0        0        0     1896 2022-07-20 01:40:32.607380 ooo_dev_tools-0.9.7/ooodev/utils/script_context.py
+-rw-r--r--   0        0        0    25545 2023-04-23 13:05:06.227316 ooo_dev_tools-0.9.7/ooodev/utils/selection.py
+-rw-r--r--   0        0        0     6400 2022-10-31 22:59:24.504932 ooo_dev_tools-0.9.7/ooodev/utils/session.py
+-rw-r--r--   0        0        0      727 2022-10-29 21:44:16.952005 ooo_dev_tools-0.9.7/ooodev/utils/sys_info.py
+-rw-r--r--   0        0        0    26396 2023-04-02 18:09:12.907574 ooo_dev_tools-0.9.7/ooodev/utils/table_helper.py
+-rw-r--r--   0        0        0     2023 2022-07-14 20:40:23.817443 ooo_dev_tools-0.9.7/ooodev/utils/text_transferable.py
+-rw-r--r--   0        0        0     1453 2022-07-24 03:34:34.568523 ooo_dev_tools-0.9.7/ooodev/utils/type_var.py
+-rw-r--r--   0        0        0     3478 2022-07-14 20:40:23.818235 ooo_dev_tools-0.9.7/ooodev/utils/uno_const.py
+-rw-r--r--   0        0        0     6513 2022-10-04 00:14:04.247070 ooo_dev_tools-0.9.7/ooodev/utils/uno_enum.py
+-rw-r--r--   0        0        0      562 2022-10-27 15:27:12.084993 ooo_dev_tools-0.9.7/ooodev/utils/validation.py
+-rw-r--r--   0        0        0    11180 2022-11-25 03:43:11.802373 ooo_dev_tools-0.9.7/ooodev/utils/view_state.py
+-rw-r--r--   0        0        0    18910 2022-07-24 03:34:47.735913 ooo_dev_tools-0.9.7/ooodev/utils/xml_util.py
+-rw-r--r--   0        0        0        0 2022-07-16 02:19:46.806983 ooo_dev_tools-0.9.7/ooodev/wrapper/__init__.py
+-rw-r--r--   0        0        0      929 2022-08-23 05:01:45.230317 ooo_dev_tools-0.9.7/ooodev/wrapper/break_context.py
+-rw-r--r--   0        0        0     2366 2023-04-27 15:20:03.729631 ooo_dev_tools-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     5220 2023-04-23 13:05:05.060319 ooo_dev_tools-0.9.7/README.rst
+-rw-r--r--   0        0        0     6770 1970-01-01 00:00:00.000000 ooo_dev_tools-0.9.7/PKG-INFO
```

### Comparing `ooo_dev_tools-0.9.6/LICENSE` & `ooo_dev_tools-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/adapter/adapter_base.py` & `ooo_dev_tools-0.9.7/ooodev/adapter/adapter_base.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/adapter/awt/top_window_listener.py` & `ooo_dev_tools-0.9.7/ooodev/adapter/awt/top_window_listener.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/adapter/frame/terminate_listener.py` & `ooo_dev_tools-0.9.7/ooodev/adapter/frame/terminate_listener.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/adapter/lang/event_listener.py` & `ooo_dev_tools-0.9.7/ooodev/adapter/lang/event_listener.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/adapter/util/modify_listener.py` & `ooo_dev_tools-0.9.7/ooodev/adapter/util/modify_listener.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/adapter/view/selection_change_listener.py` & `ooo_dev_tools-0.9.7/ooodev/adapter/view/selection_change_listener.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/cfg/config.py` & `ooo_dev_tools-0.9.7/ooodev/cfg/config.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/conn/cache.py` & `ooo_dev_tools-0.9.7/ooodev/conn/cache.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/conn/connect.py` & `ooo_dev_tools-0.9.7/ooodev/conn/connect.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/conn/connectors.py` & `ooo_dev_tools-0.9.7/ooodev/conn/connectors.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/dialog/input.py` & `ooo_dev_tools-0.9.7/ooodev/dialog/input.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/dialog/msgbox.py` & `ooo_dev_tools-0.9.7/ooodev/dialog/msgbox.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/dialog/tk_input.py` & `ooo_dev_tools-0.9.7/ooodev/dialog/tk_input.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/args/calc/cell_args.py` & `ooo_dev_tools-0.9.7/ooodev/events/args/calc/cell_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/args/calc/cell_cancel_args.py` & `ooo_dev_tools-0.9.7/ooodev/events/args/calc/cell_cancel_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/args/calc/sheet_args.py` & `ooo_dev_tools-0.9.7/ooodev/events/args/calc/sheet_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/args/calc/sheet_cancel_args.py` & `ooo_dev_tools-0.9.7/ooodev/events/args/calc/sheet_cancel_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/args/cancel_event_args.py` & `ooo_dev_tools-0.9.7/ooodev/events/args/cancel_event_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/args/dispatch_args.py` & `ooo_dev_tools-0.9.7/ooodev/events/args/dispatch_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/args/dispatch_cancel_args.py` & `ooo_dev_tools-0.9.7/ooodev/events/args/dispatch_cancel_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/args/event_args.py` & `ooo_dev_tools-0.9.7/ooodev/events/args/event_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/args/generic_args.py` & `ooo_dev_tools-0.9.7/ooodev/events/args/generic_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/args/key_val_args.py` & `ooo_dev_tools-0.9.7/ooodev/events/args/key_val_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/args/key_val_cancel_args.py` & `ooo_dev_tools-0.9.7/ooodev/events/args/key_val_cancel_args.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/calc_named_event.py` & `ooo_dev_tools-0.9.7/ooodev/events/calc_named_event.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/chart2_named_event.py` & `ooo_dev_tools-0.9.7/ooodev/events/chart2_named_event.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/event_singleton.py` & `ooo_dev_tools-0.9.7/ooodev/events/event_singleton.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/format_named_event.py` & `ooo_dev_tools-0.9.7/ooodev/events/format_named_event.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/lo_events.py` & `ooo_dev_tools-0.9.7/ooodev/events/lo_events.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/lo_named_event.py` & `ooo_dev_tools-0.9.7/ooodev/events/lo_named_event.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/props_named_event.py` & `ooo_dev_tools-0.9.7/ooodev/events/props_named_event.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/events/write_named_event.py` & `ooo_dev_tools-0.9.7/ooodev/events/write_named_event.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/exceptions/ex.py` & `ooo_dev_tools-0.9.7/ooodev/exceptions/ex.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/direct/cell/alignment/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/direct/cell/alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/direct/cell/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/direct/cell/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/direct/cell/font/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/direct/cell/font/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/modify/cell/alignment/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/modify/cell/alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/modify/cell/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/modify/cell/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/modify/cell/font/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/modify/cell/font/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/modify/cell/numbers/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/modify/cell/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/footer/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/footer/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/footer/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/footer/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/header/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/header/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/header/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/header/borders/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/page/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/page/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/modify/page/sheet/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/modify/page/sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/style/cell/cell.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/style/cell/cell.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/style/cell/kind/style_cell_kind.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/style/cell/kind/style_cell_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/calc/style/page/page.py` & `ooo_dev_tools-0.9.7/ooodev/format/calc/style/page/page.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/axis/font/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/axis/font/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/axis/label/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/axis/label/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/axis/positioning/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/axis/positioning/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/general/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/general/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/general/transparency/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/general/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/legend/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/legend/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/legend/font/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/legend/font/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/legend/transparency/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/legend/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_labels/data_labels/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_labels/data_labels/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_labels/font/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_labels/font/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_series/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_series/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_series/options/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_series/options/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/series/data_series/transparency/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/series/data_series/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/title/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/title/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/title/font/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/title/font/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/wall/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/wall/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/chart2/direct/wall/transparency/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/chart2/direct/wall/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/draw/direct/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/draw/direct/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/draw/direct/transparency/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/draw/direct/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/draw/modify/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/draw/modify/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/draw/style/lookup/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/draw/style/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/impress/modify/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/impress/modify/area/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_document.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_document.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # region Import
 from __future__ import annotations
 
+import uno
 from com.sun.star.text import XTextDocument
 from com.sun.star.container import XNameAccess
+from com.sun.star.beans import XPropertySet
 
 from ooodev.exceptions import ex as mEx
 from ooodev.utils import info as mInfo
 from ooodev.utils.data_type.size import Size
 from ooodev.office import write as mWrite
 from ooodev.format.inner.style_base import StyleBase
 
@@ -111,8 +113,19 @@
 
         Returns:
             XNameAccess | None: Text Frames on success, Otherwise, None
         """
         # return mLo.Lo.this_component.TextFrames
         return mWrite.Write.get_text_frames(mWrite.Write.active_doc)
 
+    def get_doc_settings(self) -> XPropertySet:
+        """
+        Gets the document settings
+
+        Returns:
+            XPropertySet: Properties
+
+        .. versionadded:: 0.9.7
+        """
+        return mWrite.Write.get_doc_settings()
+
     # endregion methods
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_fill_color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_fill_color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_hf.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_hf.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_line_number.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_line_number.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_sides.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/common/abstract/abstract_writing_mode.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/common/abstract/abstract_writing_mode.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/common/border_width_impl.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/common/border_width_impl.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/area_img_props.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/area_img_props.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/cell_borders_props.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/cell_borders_props.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/common/props/hf_props.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/common/props/hf_props.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/alignment/properties.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/alignment/properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/alignment/text_align.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/alignment/text_align.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/alignment/text_orientation.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/alignment/text_orientation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/background/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/background/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/border/borders.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/border/borders.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/border/padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/border/shadow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/char/font/font.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/char/font/font.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/numbers/numbers.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/numbers/numbers.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/page/page/layout_settings.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/page/page/layout_settings.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/calc/page/page/margins.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/calc/page/page/margins.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,22 @@
         super().__init__()
         self.prop_left = left
         self.prop_right = right
         self.prop_top = top
         self.prop_bottom = bottom
 
     # region Internal Methods
-    def _check(self, value: float | None, name: str) -> None:
+    def _check(self, value: float | UnitObj | None, name: str) -> None:
         if value is None:
             return
-        if value < 0.0:
+        try:
+            val = value.get_value_mm()
+        except AttributeError:
+            val = float(value)
+        if val < 0.0:
             raise ValueError(f'"{name}" parameter must be a positive value')
 
     # endregion Internal Methods
 
     # region dunder methods
     def __eq__(self, oth: object) -> bool:
         if isinstance(oth, Margins):
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/font/font_effects.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/font/font_effects.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/font/font_only.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/font/font_only.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/label/order.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/label/order.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/label/orientation.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/label/orientation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/label/show.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/label/show.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/label/text_flow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/label/text_flow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/numbers/numbers.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/numbers/numbers.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/positioning/axis_line.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/positioning/axis_line.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/positioning/interval_marks.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/positioning/interval_marks.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/positioning/label_position.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/positioning/label_position.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/axis/positioning/position_axis.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/axis/positioning/position_axis.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/area/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/area/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/area/hatch.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/area/pattern.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/borders/line_properties.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/borders/line_properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/numbers/numbers.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/numbers/numbers.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/transparent/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/transparent/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/chart/transparent/transparency.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/chart/transparent/transparency.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/grid/line_properties.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/grid/line_properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/font/font.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/font/font.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/font/font_effects.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/font/font_effects.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/legend/position/position.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/legend/position/position.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/position_size/position.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/position_size/position.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/position_size/size.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/position_size/size.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/borders/line_properties.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/borders/line_properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/attrib_options.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/attrib_options.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/number_format.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/number_format.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/orientation.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/orientation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/percent_format.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/data_labels/percent_format.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/font/font_effects.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/font/font_effects.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_labels/font/font_only.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_labels/font/font_only.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/borders/line_properties.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/borders/line_properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/options/align_series.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/options/align_series.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/options/legend_entry.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/options/legend_entry.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/options/orientation.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/options/orientation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/options/plot.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/options/plot.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/options/plot_simple.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/options/plot_simple.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/series/data_series/options/settings.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/series/data_series/options/settings.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/alignment/direction.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/alignment/direction.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/alignment/orientation.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/alignment/orientation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/font/font.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/font/font.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/font/font_effects.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/font/font_effects.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/font/font_only.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/font/font_only.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/title/position_size/position.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/title/position_size/position.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/area/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/area/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/area/hatch.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/area/pattern.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/borders/line_properties.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/borders/line_properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/transparent/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/transparent/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/chart2/wall/transparent/transparency.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/chart2/wall/transparent/transparency.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/draw/shape/position_size/position.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/draw/shape/position_size/position.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/cell_protection_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/cell_protection_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/crop_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/crop_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/data_point_label_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/data_point_label_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/drop_cap_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/drop_cap_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/gradient_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/gradient_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/hatch_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/hatch_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/line_spacing_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/line_spacing_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/locale_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/locale_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/point_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/point_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/shadow_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/shadow_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/side.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/side.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/size_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/size_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/struct_base.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/struct_base.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/tab_stop_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/tab_stop_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/table_border_distances_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/table_border_distances_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/structs/table_border_struct.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/structs/table_border_struct.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/border/borders.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/border/borders.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/border/padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/border/shadow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/border/sides.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/font/font.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/font/font.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/font/font_effects.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/font/font_effects.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/font/font_only.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/font/font_only.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/font/font_position.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/font/font_position.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/highlight/highlight.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/highlight/highlight.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/char/hyperlink/hyperlink.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/char/hyperlink/hyperlink.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/area/fill_color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/area/fill_color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/area/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/area/hatch.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/area/pattern.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/transparent/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/transparent/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/fill/transparent/transparency.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/fill/transparent/transparency.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/frame_type/anchor.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/frame_type/anchor.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/frame_type/position.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/frame_type/position.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/frame_type/size.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/frame_type/size.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/hyperlink/image_map_options.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/hyperlink/image_map_options.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/hyperlink/link_to.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/hyperlink/link_to.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/options/align.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/options/align.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/options/names.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/options/names.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/options/properties.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/options/properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/options/protect.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/options/protect.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/wrap/options.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/wrap/options.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/wrap/settings.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/wrap/settings.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/frame/wrap/spacing.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/frame/wrap/spacing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/crop/crop.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/crop/crop.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/image/flip.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/image/flip.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/image/rotation.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/image/rotation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/image_type/size.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/image_type/size.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/options/names.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/options/names.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/image/options/properties.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/image/options/properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/area/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/area/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/area/hatch.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/area/pattern.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/footer/footer.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/footer/footer.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/area/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/area/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/area/hatch.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/area/pattern.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/header/header.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/header/header.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/page/layout_settings.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/page/layout_settings.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/page/margins.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/page/margins.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/page/page/paper_format.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/page/page/paper_format.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/align/alignment.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/align/alignment.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/align/writing_mode.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/align/writing_mode.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/area/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/area/hatch.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/area/pattern.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/border/borders.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/border/borders.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/border/padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/border/shadow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/border/sides.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/drop_cap/drop_caps.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/drop_cap/drop_caps.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/indent_space/indent.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/indent_space/indent.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/indent_space/indent_spacing.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/indent_space/indent_spacing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/indent_space/line_spacing.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/indent_space/line_spacing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/indent_space/spacing.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/indent_space/spacing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/outline_list/line_num.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/outline_list/line_num.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/outline_list/list_style.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/outline_list/list_style.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/outline_list/outline.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/outline_list/outline.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/outline_list/outline_list.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/outline_list/outline_list.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/tabs/tabs.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/tabs/tabs.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/text_flow/breaks.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/text_flow/breaks.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/text_flow/flow_options.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/text_flow/flow_options.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/text_flow/hyphenation.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/text_flow/hyphenation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/text_flow/text_flow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/text_flow/text_flow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/para/transparent/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/para/transparent/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/shape/area/shadow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/shape/area/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/table/background/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/table/background/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/table/background/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/table/background/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/table/borders/borders.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/table/borders/borders.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/direct/write/table/props/table_properties.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/direct/write/table/props/table_properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/alignment/properties.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/alignment/properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/alignment/text_align.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/alignment/text_align.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/alignment/text_orientation.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/alignment/text_orientation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/background/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/background/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/border/borders.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/border/borders.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/cell_protection/cell_protection.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/cell_protection/cell_protection.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/cell_style_base.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/cell_style_base.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/cell_style_base_multi.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/cell_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/font/font_effects.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/font/font_effects.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/font/font_only.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/font/font_only.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/numbers/numbers.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/numbers/numbers.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/area/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/border/padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/border/shadow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/border/sides.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/area/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/border/padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/border/shadow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/border/sides.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/footer/footer.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/footer/footer.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/area/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/border/padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/border/shadow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/border/sides.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/header/header.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/header/header.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/page/layout_settings.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/page/layout_settings.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/page/margins.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/page/margins.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/page/paper_format.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/page/paper_format.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/sheet/order.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/sheet/order.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/sheet/printing.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/sheet/printing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/sheet/scale_num_of_pages.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/sheet/scale_num_of_pages.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/sheet/scale_pages_width_height.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/sheet/scale_pages_width_height.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/calc/page/sheet/scale_reduce_enlarge.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/calc/page/sheet/scale_reduce_enlarge.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/border/padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/border/padding.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 # endregion Imports
 
 
 class Padding(CharStyleBaseMulti):
     """
     Character Style Border padding.
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_char_borders`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         left: float | UnitObj | None = None,
@@ -38,14 +42,17 @@
             bottom (float, UnitObj,  optional): Bottom (in ``mm`` units)  or :ref:`proto_unit_obj`.
             all (float, UnitObj, optional): Left, right, top, bottom (in ``mm`` units)  or :ref:`proto_unit_obj`. If argument is present then ``left``, ``right``, ``top``, and ``bottom`` arguments are ignored.
             style_name (StyleParaKind, str, optional): Specifies the Character Style that instance applies to. Default is Default Character Style.
             style_family (str, optional): Style family. Default ``CharacterStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_char_borders`
         """
 
         direct = InnerPadding(left=left, right=right, top=top, bottom=bottom, all=all)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/border/shadow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/border/shadow.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 # endregion Imports
 
 
 class Shadow(CharStyleBaseMulti):
     """
     Character Style Border padding.
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_char_borders`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         location: ShadowLocation = ShadowLocation.BOTTOM_RIGHT,
@@ -40,14 +44,17 @@
             transparent (bool, optional): Shadow transparency. Defaults to False.
             width (float, Unit100MM, optional): contains the size of the shadow (in ``mm`` units) or :ref:`proto_unit_obj`. Defaults to ``1.76``.
             style_name (StyleCharKind, str, optional): Specifies the Character Style that instance applies to. Default is Default Character Style.
             style_family (str, optional): Style family. Default ``CharacterStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_char_borders`
         """
 
         direct = InnerShadow(location=location, color=color, transparent=transparent, width=width)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/border/sides.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/border/sides.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 # endregion Imports
 
 
 class Sides(CharStyleBaseMulti):
     """
     Character Style Border Sides (lines).
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_char_borders`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         left: Side | None = None,
@@ -41,14 +45,17 @@
             border_side (Side | None, optional): Determines the line style at the top, bottom, left, right edges. If this argument has a value then arguments ``top``, ``bottom``, ``left``, ``right`` are ignored
             shadowed (bool, optional): Specifies if the characters are formatted and displayed with a shadow effect.
             style_name (StyleParaKind, str, optional): Specifies the Character Style that instance applies to. Default is Default Character Style.
             style_family (str, optional): Style family. Default ``CharacterStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_char_borders`
         """
 
         direct = InnerSides(left=left, right=right, top=top, bottom=bottom, all=border_side)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/char_style_base_multi.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/char_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/font/font_effects.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/font/font_effects.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 # endregion Imports
 
 
 class FontEffects(CharStyleBaseMulti):
     """
     Character Style Font Effects
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_char_font_effects`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         color: Color | None = None,
@@ -59,14 +63,17 @@
             hidden (bool, optional): Specifies if the font is hidden.
             shadowed (bool, optional): Specifies if the characters are formatted and displayed with a shadow effect.
             style_name (StyleParaKind, str, optional): Specifies the Character Style that instance applies to. Default is Default Character Style.
             style_family (str, optional): Style family. Default ``CharacterStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_char_font_effects`
         """
 
         direct = InnerFontEffects(
             color=color,
             transparency=transparency,
             overline=overline,
             underline=underline,
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/font/font_only.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/font/font_only.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 # endregion Imports
 
 
 class FontOnly(CharStyleBaseMulti):
     """
     Character Style Font
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_char_font_only`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         name: str | None = None,
@@ -39,14 +43,17 @@
             lang (Lang, optional): Font Language
             shadowed (bool, optional): Specifies if the characters are formatted and displayed with a shadow effect.
             style_name (StyleParaKind, str, optional): Specifies the Character Style that instance applies to. Default is Default Character Style.
             style_family (str, optional): Style family. Default ``CharacterStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_char_font_only`
         """
 
         direct = InnerFontOnly(name=name, size=size, font_style=font_style_name, lang=lang)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/font/font_position.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/font/font_position.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 # endregion Imports
 
 
 class FontPosition(CharStyleBaseMulti):
     """
     Character Style Font Effects
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_char_font_position`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         script_kind: FontScriptKind | None = None,
@@ -49,14 +53,17 @@
             spacing (CharSpacingKind, float, UnitObj, optional): Specifies character spacing in ``pt`` (point) units or :ref:`proto_unit_obj`.
             pair (bool, optional): Specifies pair kerning.
             style_name (StyleCharKind, str, optional): Specifies the Character Style that instance applies to. Default is Default Character Style.
             style_family (str, optional): Style family. Default ``CharacterStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_char_font_position`
         """
 
         direct = InnerFontPosition(
             script_kind=script_kind,
             raise_lower=raise_lower,
             rel_size=rel_size,
             rotation=rotation,
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/char/highlight/highlight.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/char/highlight/highlight.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 # endregion Imports
 
 
 class Highlight(CharStyleBaseMulti):
     """
     Character Style Highlight.
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_char_highlight`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         color: Color = -1,
@@ -56,14 +60,17 @@
         Args:
             doc (object): UNO Document Object.
             style_name (StyleCharKind, str, optional): Specifies the Character Style that instance applies to. Default is Default Character Style.
             style_family (str, optional): Style family. Default ``CharacterStyles``.
 
         Returns:
             Highlight: ``Highlight`` instance from document properties.
+
+        See Also:
+            - :ref:`help_writer_format_modify_char_highlight`
         """
         inst = cls(style_name=style_name, style_family=style_family)
         direct = InnerHighlight.from_obj(inst.get_style_props(doc))
         inst._set_style("direct", direct, *direct.get_attrs())
         return inst
 
     @property
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/fill/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/fill/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/fill/fill_style_base_multi.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/fill/fill_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/area/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/area/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/area/hatch.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/area/pattern.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/border/padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/border/shadow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/border/sides.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/frame_style_base_multi.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/frame_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/frame_type/anchor.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/frame_type/anchor.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/frame_type/position.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/frame_type/position.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/frame_type/size.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/frame_type/size.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/options/align.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/options/align.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/options/properties.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/options/properties.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/options/protect.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/options/protect.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/transparent/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/transparent/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/transparent/transparency.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/transparent/transparency.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/wrap/options.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/wrap/options.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/wrap/settings.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/wrap/settings.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/frame/wrap/spacing.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/frame/wrap/spacing.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/area/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/area/color.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 # endregion Imports
 
 
 class InnerColor(AbstractColor):
     """
     Page Style Color.
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_page_area`
+
     .. versionadded:: 0.9.0
     """
 
     def _supported_services(self) -> Tuple[str, ...]:
         try:
             return self._supported_services_values
         except AttributeError:
@@ -44,14 +48,18 @@
         return self._props_internal_attributes
 
 
 class Color(PageStyleBaseMulti):
     """
     Page Style Color.
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_page_area`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         color: mColor.Color = -1,
@@ -65,14 +73,17 @@
             color (:py:data:`~.utils.color.Color`, optional): FillColor Color
             style_name (WriterStylePageKind, str, optional): Specifies the Page Style that instance applies to.
                 Default is Default Page Style.
             style_family (str, optional): Style family. Default ``PageStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_page_area`
         """
 
         direct = InnerColor(color=color)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/area/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/area/gradient.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 # endregion Imports
 
 
 class Gradient(PageStyleBaseMulti):
     """
     Page Style Gradient
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_page_area`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         style: GradientStyle = GradientStyle.LINEAR,
@@ -58,14 +62,17 @@
             name (str, optional): Specifies the Fill Gradient Name.
             style_name (StyleParaKind, str, optional): Specifies the Page Style that instance applies to.
                 Default is Default Page Style.
             style_family (str, optional): Style family. Default ``PageStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_page_area`
         """
 
         direct = InnerGradient(
             style=style,
             step_count=step_count,
             offset=offset,
             angle=angle,
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/area/hatch.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/area/hatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 # endregion Imports
 
 
 class Hatch(PageStyleBaseMulti):
     """
     Page Style Pattern
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_page_area`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         style: HatchStyle = HatchStyle.SINGLE,
@@ -47,14 +51,17 @@
                 for no background color.
             style_name (StyleParaKind, str, optional): Specifies the Page Style that instance applies to.
             Default is Default Page Style.
             style_family (str, optional): Style family. Default ``PageStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_page_area`
         """
 
         direct = InnerHatch(style=style, color=color, space=space, angle=angle, bg_color=bg_color)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/area/img.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 # endregion Imports
 
 
 class Img(PageStyleBaseMulti):
     """
     Page Style Image
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_page_area`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         bitmap: XBitmap | None = None,
@@ -57,14 +61,17 @@
             auto_name (bool, optional): Specifies if ``name`` is ensured to be unique. Defaults to ``False``.
             style_name (WriterStylePageKind, str, optional): Specifies the Page Style that instance applies to.
                 Default is Default Page Style.
             style_family (str, optional): Style family. Default ``PageStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_page_area`
         """
 
         direct = InnerImg(
             bitmap=bitmap,
             name=name,
             mode=mode,
             size=size,
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/area/pattern.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/area/pattern.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 # endregion Imports
 
 
 class Pattern(PageStyleBaseMulti):
     """
     Page Style Pattern
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_page_area`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         bitmap: XBitmap | None = None,
@@ -43,14 +47,17 @@
             auto_name (bool, optional): Specifies if ``name`` is ensured to be unique. Defaults to ``False``.
             style_name (StyleParaKind, str, optional): Specifies the Page Style that instance applies to.
                 Default is Default Page Style.
             style_family (str, optional): Style family. Default ``PageStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_page_area`
         """
 
         direct = InnerPattern(bitmap=bitmap, name=name, tile=tile, stretch=stretch, auto_name=auto_name)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/border/padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/border/shadow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/border/sides.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/area/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/area/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/area/hatch.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/area/pattern.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/border/padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/border/shadow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/border/sides.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/footer.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/footer.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/transparency/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/transparency/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/footer/transparency/transparency.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/footer/transparency/transparency.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/area/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/area/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/area/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/area/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/area/hatch.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/area/hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/area/img.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/area/pattern.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/area/pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/border/padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/border/padding.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/border/shadow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/border/shadow.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/border/sides.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/border/sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/header.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/header.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/transparency/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/transparency/gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/header/transparency/transparency.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/header/transparency/transparency.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/page/layout_settings.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/transparency/gradient.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,103 +1,109 @@
 # region Import
 from __future__ import annotations
-from typing import cast
+from typing import Tuple, cast, Any
 import uno
-from ooo.dyn.style.page_style_layout import PageStyleLayout as PageStyleLayout
-from ooo.dyn.style.numbering_type import NumberingTypeEnum as NumberingTypeEnum
+from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
 
-from ooodev.format.writer.style.page.kind import WriterStylePageKind as WriterStylePageKind
-from ooodev.format.writer.style.para.kind.style_para_kind import StyleParaKind as StyleParaKind
-from ooodev.format.inner.direct.write.page.page.layout_settings import LayoutSettings as InnerLayoutSettings
+from ooodev.utils.data_type.angle import Angle as Angle
+from ooodev.utils.data_type.offset import Offset as Offset
+from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
+from ooodev.format.writer.style.page.kind.writer_style_page_kind import WriterStylePageKind as WriterStylePageKind
+from ooodev.utils.data_type.intensity import Intensity as Intensity
+from ooodev.format.inner.direct.write.fill.transparent.gradient import Gradient as InnerGradient
 from ..page_style_base_multi import PageStyleBaseMulti
 
 # endregion Import
 
 
-class LayoutSettings(PageStyleBaseMulti):
+class Gradient(PageStyleBaseMulti):
     """
-    Page Layout Setting style
+    Page Style Transparency.
+
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_page_transparency`
 
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
-        layout: PageStyleLayout | None = None,
-        numbers: NumberingTypeEnum | None = None,
-        ref_style: str | StyleParaKind | None = None,
-        right_gutter: bool | None = None,
+        style: GradientStyle = GradientStyle.LINEAR,
+        offset: Offset = Offset(50, 50),
+        angle: Angle | int = 0,
+        border: Intensity | int = 0,
+        grad_intensity: IntensityRange = IntensityRange(0, 0),
         style_name: WriterStylePageKind | str = WriterStylePageKind.STANDARD,
         style_family: str = "PageStyles",
     ) -> None:
         """
         Constructor
 
         Args:
-            layout (PageStyleLayout, optional): Specifies the layout of the page.
-            numbers (NumberingTypeEnum, optional): Specifies the default numbering type for this page.
-            ref_style (str, StyleParaKind, optional): Specifies the name of the paragraph style that is used as
-                reference of the register mode.
-            right_gutter (bool, optional): Specifies that the page gutter shall be placed on the right side of the page.
-            style_name (WriterStylePageKind, str, optional): Specifies the Page Style that instance applies to.
+            value (Intensity, int, optional): Specifies the transparency value from ``0`` to ``100``.
+            style_name (StyleParaKind, str, optional): Specifies the Page Style that instance applies to.
                 Default is Default Page Style.
             style_family (str, optional): Style family. Default ``PageStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_page_transparency`
         """
 
-        direct = InnerLayoutSettings(layout=layout, numbers=numbers, ref_style=ref_style, right_gutter=right_gutter)
+        direct = InnerGradient(style=style, offset=offset, angle=angle, border=border, grad_intensity=grad_intensity)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
 
     @classmethod
     def from_style(
         cls,
         doc: object,
         style_name: WriterStylePageKind | str = WriterStylePageKind.STANDARD,
         style_family: str = "PageStyles",
-    ) -> LayoutSettings:
+    ) -> Gradient:
         """
         Gets instance from Document.
 
         Args:
             doc (object): UNO Document Object.
-            style_name (WriterStylePageKind, str, optional): Specifies the Paragraph Style that instance applies to.
+            style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``PageStyles``.
 
         Returns:
-            LayoutSettings: ``LayoutSettings`` instance from document properties.
+            Gradient: ``Gradient`` instance from document properties.
         """
         inst = cls(style_name=style_name, style_family=style_family)
-        direct = InnerLayoutSettings.from_obj(inst.get_style_props(doc))
+        direct = InnerGradient.from_obj(inst.get_style_props(doc))
         inst._set_style("direct", direct, *direct.get_attrs())
         return inst
 
     @property
     def prop_style_name(self) -> str:
         """Gets/Sets property Style Name"""
         return self._style_name
 
     @prop_style_name.setter
     def prop_style_name(self, value: str | WriterStylePageKind):
         self._style_name = str(value)
 
     @property
-    def prop_inner(self) -> InnerLayoutSettings:
-        """Gets/Sets Inner Layout Settings instance"""
+    def prop_inner(self) -> InnerGradient:
+        """Gets/Sets Inner Transparency instance"""
         try:
             return self._direct_inner
         except AttributeError:
-            self._direct_inner = cast(InnerLayoutSettings, self._get_style_inst("direct"))
+            self._direct_inner = cast(InnerGradient, self._get_style_inst("direct"))
         return self._direct_inner
 
     @prop_inner.setter
-    def prop_inner(self, value: InnerLayoutSettings) -> None:
-        if not isinstance(value, InnerLayoutSettings):
-            raise TypeError(f'Expected type of InnerLayoutSettings, got "{type(value).__name__}"')
+    def prop_inner(self, value: InnerGradient) -> None:
+        if not isinstance(value, InnerGradient):
+            raise TypeError(f'Expected type of InnerGradient, got "{type(value).__name__}"')
         self._del_attribs("_direct_inner")
         self._set_style("direct", value, *value.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/page/margins.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/page/margins.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 # endregion Import
 
 
 class Margins(PageStyleBaseMulti):
     """
     Page Style Margins
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_page_page`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         left: float | UnitObj | None = None,
@@ -38,14 +42,17 @@
             gutter (float, optional): Gutter Margin Value in ``mm`` units  or :ref:`proto_unit_obj`.
             style_name (WriterStylePageKind, str, optional): Specifies the Page Style that instance applies to.
                 Default is Default Page Style.
             style_family (str, optional): Style family. Default ``PageStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_page_page`
         """
 
         direct = InnerMargins(left=left, right=right, top=top, bottom=bottom, gutter=gutter)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/page/paper_format.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/page/paper_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 # endregion Import
 
 
 class PaperFormat(PageStyleBaseMulti):
     """
     Page Style Paper Format
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_page_page`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         size: SizeMM = SizeMM(215.9, 279.4),
@@ -31,14 +35,17 @@
             size (SizeMM, optional): Width and height in ``mm`` units. Defaults to Letter size in Portrait mode.
             style_name (WriterStylePageKind, str, optional): Specifies the Page Style that instance applies to.
                 Default is Default Page Style.
             style_family (str, optional): Style family. Default ``PageStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_page_page`
         """
 
         direct = InnerPaperFormat(size=size)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/page_style_base_multi.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/page_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/transparency/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/transparent/gradient.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,86 @@
 # region Import
 from __future__ import annotations
-from typing import Tuple, cast, Any
+from typing import cast, Any
 import uno
 from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
 
 from ooodev.utils.data_type.angle import Angle as Angle
-from ooodev.utils.data_type.offset import Offset as Offset
-from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
-from ooodev.format.writer.style.page.kind.writer_style_page_kind import WriterStylePageKind as WriterStylePageKind
 from ooodev.utils.data_type.intensity import Intensity as Intensity
+from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
+from ooodev.utils.data_type.offset import Offset as Offset
+from ooodev.format.writer.style.para.kind import StyleParaKind as StyleParaKind
 from ooodev.format.inner.direct.write.fill.transparent.gradient import Gradient as InnerGradient
-from ..page_style_base_multi import PageStyleBaseMulti
+from ..para_style_base_multi import ParaStyleBaseMulti
 
 # endregion Import
 
 
-class Gradient(PageStyleBaseMulti):
+class Gradient(ParaStyleBaseMulti):
     """
-    Page Style Transparency.
+    Paragraph Style Gradient
+
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_transparency`
 
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         style: GradientStyle = GradientStyle.LINEAR,
         offset: Offset = Offset(50, 50),
         angle: Angle | int = 0,
         border: Intensity | int = 0,
         grad_intensity: IntensityRange = IntensityRange(0, 0),
-        style_name: WriterStylePageKind | str = WriterStylePageKind.STANDARD,
-        style_family: str = "PageStyles",
+        style_name: StyleParaKind | str = StyleParaKind.STANDARD,
+        style_family: str = "ParagraphStyles",
+        **kwargs: Any,
     ) -> None:
         """
         Constructor
 
         Args:
             value (Intensity, int, optional): Specifies the transparency value from ``0`` to ``100``.
-            style_name (StyleParaKind, str, optional): Specifies the Page Style that instance applies to.
-                Default is Default Page Style.
-            style_family (str, optional): Style family. Default ``PageStyles``.
+            style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
+                Default is Default Paragraph Style.
+            style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_transparency`
         """
 
-        direct = InnerGradient(style=style, offset=offset, angle=angle, border=border, grad_intensity=grad_intensity)
+        direct = InnerGradient(
+            style=style, offset=offset, angle=angle, border=border, grad_intensity=grad_intensity, kwargs=kwargs
+        )
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
 
     @classmethod
     def from_style(
         cls,
         doc: object,
-        style_name: WriterStylePageKind | str = WriterStylePageKind.STANDARD,
-        style_family: str = "PageStyles",
+        style_name: StyleParaKind | str = StyleParaKind.STANDARD,
+        style_family: str = "ParagraphStyles",
     ) -> Gradient:
         """
         Gets instance from Document.
 
         Args:
             doc (object): UNO Document Object.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
-            style_family (str, optional): Style family. Default ``PageStyles``.
+            style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             Gradient: ``Gradient`` instance from document properties.
         """
         inst = cls(style_name=style_name, style_family=style_family)
         direct = InnerGradient.from_obj(inst.get_style_props(doc))
         inst._set_style("direct", direct, *direct.get_attrs())
@@ -78,20 +88,20 @@
 
     @property
     def prop_style_name(self) -> str:
         """Gets/Sets property Style Name"""
         return self._style_name
 
     @prop_style_name.setter
-    def prop_style_name(self, value: str | WriterStylePageKind):
+    def prop_style_name(self, value: str | StyleParaKind):
         self._style_name = str(value)
 
     @property
     def prop_inner(self) -> InnerGradient:
-        """Gets/Sets Inner Transparency instance"""
+        """Gets/Sets Inner Gradient instance"""
         try:
             return self._direct_inner
         except AttributeError:
             self._direct_inner = cast(InnerGradient, self._get_style_inst("direct"))
         return self._direct_inner
 
     @prop_inner.setter
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/page/transparency/transparency.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/page/transparency/transparency.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 # endregion Import
 
 
 class Transparency(PageStyleBaseMulti):
     """
     Page Style Transparency.
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_page_transparency`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         value: Intensity | int = 0,
@@ -31,14 +35,17 @@
             value (Intensity, int, optional): Specifies the transparency value from ``0`` to ``100``.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``PageStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_page_transparency`
         """
 
         direct = InnerTransparency(value=value)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/align/alignment.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/align/alignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 
 class Alignment(ParaStyleBaseMulti):
     """
     Paragraph Alignment
 
     Any properties starting with ``prop_`` set or get current instance values.
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_alignment`
+
     .. versionadded:: 0.9.0
     """
 
     # region init
 
     def __init__(
         self,
@@ -49,14 +53,17 @@
             snap_to_grid (bool, optional): Determines snap to text grid (if active).
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Family Style. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_alignment`
         """
 
         direct = InnerAlignment(
             align=align,
             align_vert=align_vert,
             txt_direction=txt_direction,
             align_last=align_last,
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/area/color.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/area/color.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 # endregion Import
 
 
 class Color(ParaStyleBaseMulti):
     """
     Paragraph Style Fill Coloring
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_color`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         color: mColor.Color = -1,
@@ -31,14 +35,17 @@
             color (:py:data:`~.utils.color.Color`, optional): Fill Color.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_color`
         """
 
         direct = InnerColor(color=color)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/area/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/area/gradient.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 # endregion Import
 
 
 class Gradient(ParaStyleBaseMulti):
     """
     Paragraph Style Gradient Color
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_gradient`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         style: GradientStyle = GradientStyle.LINEAR,
@@ -59,14 +63,17 @@
             name (str, optional): Specifies the Fill Gradient Name.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_gradient`
         """
 
         direct = InnerGradient(
             style=style,
             step_count=step_count,
             offset=offset,
             angle=angle,
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/area/hatch.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/area/hatch.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 # endregion Import
 
 
 class Hatch(ParaStyleBaseMulti):
     """
     Paragraph Style Gradient Color
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_hatch`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         style: HatchStyle = HatchStyle.SINGLE,
@@ -56,14 +60,17 @@
             auto_name (bool, optional): Specifies if Hatch is give an auto name such as ``Hatch ``. Default ``False``.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_hatch`
         """
 
         direct = InnerHatch(
             style=style, color=color, space=space, angle=angle, bg_color=bg_color, name=name, auto_name=auto_name
         )
         super().__init__()
         self._style_name = str(style_name)
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/area/img.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/area/img.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 # works whereas setting paragraph properties on style messes up the graphic in this case.
 
 
 class Img(ParaStyleBaseMulti):
     """
     Paragraph Style Fill Coloring
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_image`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         bitmap: XBitmap | None = None,
@@ -50,14 +54,17 @@
             color (:py:data:`~.utils.color.Color`, optional): FillColor Color
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_image`
         """
 
         direct = InnerImg(
             bitmap=bitmap,
             name=name,
             mode=mode,
             size=size,
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/area/pattern.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/area/pattern.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 # endregion Import
 
 
 class Pattern(ParaStyleBaseMulti):
     """
     Paragraph Style Gradient Color
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_pattern`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         bitmap: XBitmap | None = None,
@@ -48,14 +52,17 @@
             auto_name (bool, optional): Specifies if ``name`` is ensured to be unique. Defaults to ``False``.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_pattern`
         """
 
         direct = InnerPattern(bitmap=bitmap, name=name, tile=tile, stretch=stretch, auto_name=auto_name)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/border/borders.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/border/borders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # region Import
 from __future__ import annotations
 from typing import cast
 import uno
 from ooodev.format.writer.style.para.kind import StyleParaKind as StyleParaKind
 from ooodev.format.inner.direct.structs.side import Side as Side, LineSize as LineSize
-from ooodev.format.inner.direct.write.para.border.shadow import Shadow as InnerShadow
-from ooodev.format.inner.direct.write.para.border.padding import Padding as InnerPadding
+from ooodev.format.inner.direct.write.para.border.shadow import Shadow
+from ooodev.format.inner.direct.write.para.border.padding import Padding
 from ooodev.format.inner.direct.write.para.border.borders import Borders as InnerBorders
 from ..para_style_base_multi import ParaStyleBaseMulti
 
 # endregion Import
 
 
 class Borders(ParaStyleBaseMulti):
     """
     Paragraph Style Borders
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_borders`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         right: Side | None = None,
         left: Side | None = None,
         top: Side | None = None,
         bottom: Side | None = None,
         border_side: Side | None = None,
-        shadow: InnerShadow | None = None,
-        padding: InnerPadding | None = None,
+        shadow: Shadow | None = None,
+        padding: Padding | None = None,
         merge: bool | None = None,
         style_name: StyleParaKind | str = StyleParaKind.STANDARD,
         style_family: str = "ParagraphStyles",
     ) -> None:
         """
         Constructor
 
@@ -48,14 +52,17 @@
             merge (bool, None, optional): Merge with next paragraph
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_borders`
         """
 
         direct = InnerBorders(
             right=right,
             left=left,
             top=top,
             bottom=bottom,
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/border/padding.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/border/padding.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 # endregion Import
 
 
 class Padding(ParaStyleBaseMulti):
     """
     Paragraph Style Padding
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_borders`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         left: float | UnitObj | None = None,
@@ -41,14 +45,17 @@
                 If argument is present then ``left``, ``right``, ``top``, and ``bottom`` arguments are ignored.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_borders`
         """
 
         direct = InnerPadding(left=left, right=right, top=top, bottom=bottom, all=all)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/border/shadow.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/border/shadow.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 # endregion Import
 
 
 class Shadow(ParaStyleBaseMulti):
     """
     Paragraph Style Shadow
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_borders`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         location: ShadowLocation = ShadowLocation.BOTTOM_RIGHT,
@@ -43,14 +47,17 @@
                 or :ref:`proto_unit_obj`. Defaults to ``1.76``.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_borders`
         """
 
         direct = InnerShadow(location=location, color=color, transparent=transparent, width=width)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/border/sides.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/border/sides.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 # endregion Import
 
 
 class Sides(ParaStyleBaseMulti):
     """
     Paragraph Style Sides (lines)
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_borders`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         left: Side | None = None,
@@ -41,14 +45,17 @@
                 If this argument has a value then arguments ``top``, ``bottom``, ``left``, ``right`` are ignored
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_borders`
         """
 
         direct = InnerSides(left=left, right=right, top=top, bottom=bottom, all=all)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/drop_cap/drop_caps.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/drop_cap/drop_caps.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 # endregion Import
 
 
 class DropCaps(ParaStyleBaseMulti):
     """
     Paragraph Style Drop Caps
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_drop_caps`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         count: int = 0,
@@ -42,14 +46,17 @@
             whole_word (bool, optional): specifies if Drop Cap is applied to the whole first word.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_drop_caps`
         """
 
         direct = InnerDropCaps(count=count, spaces=spaces, lines=lines, style=style, whole_word=whole_word)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/font/font_effects.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/font/font_effects.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 # endregion Import
 
 
 class FontEffects(ParaStyleBaseMulti):
     """
     Style Font Effects
 
+    .. seealos::
+
+        - :ref:`help_writer_format_modify_para_font_effects`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         color: Color | None = None,
@@ -60,14 +64,17 @@
             shadowed (bool, optional): Specifies if the characters are formatted and displayed with a shadow effect.
             style_name (StyleParaKind, str, optional): Specifies the Character Style that instance applies to.
                 Default is Default Character Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_font_effects`
         """
 
         direct = InnerFontEffects(
             color=color,
             transparency=transparency,
             overline=overline,
             underline=underline,
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/font/font_only.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/font/font_only.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 # endregion Import
 
 
 class FontOnly(ParaStyleBaseMulti):
     """
     Style Font
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_font_only
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         name: str | None = None,
@@ -41,14 +45,17 @@
             lang (Lang, optional): Font Language
             style_name (StyleParaKind, str, optional): Specifies the Character Style that instance applies to.
                 Default is Default Character Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_font_only`
         """
 
         direct = InnerFontOnly(name=name, size=size, font_style=font_style_name, lang=lang)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/font/font_position.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/font/font_position.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 # endregion Import
 
 
 class FontPosition(ParaStyleBaseMulti):
     """
     Character Style Font Effects
 
+    .. seealos::
+
+        - :ref:`help_writer_format_modify_para_font_position`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         script_kind: FontScriptKind | None = None,
@@ -53,14 +57,17 @@
             pair (bool, optional): Specifies pair kerning.
             style_name (StyleParaKind, str, optional): Specifies the Character Style that instance applies to.
                 Default is Default Character Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_font_position`
         """
 
         direct = InnerFontPosition(
             script_kind=script_kind,
             raise_lower=raise_lower,
             rel_size=rel_size,
             rotation=rotation,
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/highlight/highlight.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/highlight/highlight.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 # endregion Import
 
 
 class Highlight(ParaStyleBaseMulti):
     """
     Paragraph Style Highlight
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_highlight`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         color: Color = -1,
@@ -32,14 +36,17 @@
             color (:py:data:`~.utils.color.Color`, optional): Highlight Color. A value of ``-1`` Set color to Transparent.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_highlight`
         """
 
         direct = InnerHighlight(color=color)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/indent_space/indent.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/indent_space/indent.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 # endregion Import
 
 
 class Indent(ParaStyleBaseMulti):
     """
     Paragraph Style Indent
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_indent_spacing`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         before: float | UnitObj | None = None,
@@ -40,14 +44,17 @@
             auto (bool, optional): Determines if the first line should be indented automatically.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_indent_spacing`
         """
 
         direct = InnerIndent(before=before, after=after, first=first, auto=auto)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/indent_space/line_spacing.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/indent_space/line_spacing.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 # endregion Import
 
 
 class LineSpacing(ParaStyleBaseMulti):
     """
     Paragraph Style Line Spacing
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_indent_spacing`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         mode: ModeKind | None = None,
@@ -47,14 +51,17 @@
             If ``ModeKind`` is ``SINGLE``, ``LINE_1_15``, ``LINE_1_5``, or ``DOUBLE`` then ``value`` is ignored.
 
             If ``ModeKind`` is ``AT_LEAST``, ``LEADING``, or ``FIXED`` then ``value`` is a float (``in mm units``)
             or :ref:`proto_unit_obj`
 
             If ``ModeKind`` is ``PROPORTIONAL`` then value is an int representing percentage.
             For example ``95`` equals ``95%``, ``130`` equals ``130%``
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_indent_spacing`
         """
 
         direct = InnerLineSpacing(mode=mode, value=value, active_ln_spacing=active_ln_spacing)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/indent_space/spacing.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/indent_space/spacing.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 # endregion Import
 
 
 class Spacing(ParaStyleBaseMulti):
     """
     Paragraph Style Spacing
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_indent_spacing`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         above: float | UnitObj | None = None,
@@ -38,14 +42,17 @@
             style_no_space (bool, optional): Do not add space between paragraphs of the same style.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_indent_spacing`
         """
 
         direct = InnerSpacing(above=above, below=below, style_no_space=style_no_space)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/outline_list/line_num.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/outline_list/line_num.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,18 @@
         return self._format_kind_prop
 
 
 class LineNum(ParaStyleBaseMulti):
     """
     Paragraph Style Line Number
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_outline_and_list`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         num_start: int = 0,
@@ -54,14 +58,17 @@
                 If greater than zero this paragraph is included in line numbering and the numbering is restarted with
                 value of ``num_start``.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to. Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_outline_and_list`
         """
 
         direct = InnerLineNum(num_start=num_start)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/outline_list/list_style.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/outline_list/list_style.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,28 +21,35 @@
     """
     Style Paragraph ListStyle
 
     Any properties starting with ``prop_`` set or get current instance values.
 
     All methods starting with ``fmt_`` can be used to chain together properties.
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_outline_and_list`
+
     .. versionadded:: 0.9.0
     """
 
     # region init
 
     def __init__(self, list_style: str | StyleListKind | None = None) -> None:
         """
         Constructor
 
         Args:
             list_style (str, StyleListKind, optional): List Style.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_outline_and_list`
         """
         # https://api.libreoffice.org/docs/idl/ref/servicecom_1_1sun_1_1star_1_1style_1_1ParagraphProperties-members.html
 
         init_vals = {}
         if not list_style is None:
             # if list_style is StyleListKind, and it is StyleListKind.NONE then str will be empty string
             str_style = str(list_style)
@@ -175,14 +182,18 @@
     # endregion properties
 
 
 class ListStyle(ParaStyleBaseMulti):
     """
     Paragraph List Style
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_outline_and_list`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         list_style: str | StyleListKind | None = None,
@@ -196,14 +207,17 @@
             list_style (str, StyleListKind, optional): List Style.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_outline_and_list`
         """
 
         direct = InnerListStyle(list_style=list_style)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/outline_list/outline.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/outline_list/outline.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 # endregion Import
 
 
 class Outline(ParaStyleBaseMulti):
     """
     Paragraph Style Outline
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_outline_and_list`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         level: LevelKind = LevelKind.TEXT_BODY,
@@ -33,14 +37,17 @@
             level (LevelKind): Outline level.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_outline_and_list`
         """
 
         direct = InnerOutline(level=level)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/para_style_base_multi.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/para_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/tabs/tabs.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/tabs/tabs.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 # endregion Import
 
 
 class Tabs(ParaStyleBaseMulti):
     """
     Paragraph Style Breaks
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_tabs`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         position: float | UnitObj = 0.0,
@@ -47,14 +51,17 @@
                 Defaults to ``FillCharKind.NONE``.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_tabs`
         """
 
         direct = InnerTabs(position=position, align=align, decimal_char=decimal_char, fill_char=fill_char)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/text_flow/breaks.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/text_flow/breaks.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 # endregion Import
 
 
 class Breaks(ParaStyleBaseMulti):
     """
     Paragraph Style Breaks
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_text_flow`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         type: BreakType | None = None,
@@ -36,14 +40,17 @@
             num (int, optional): Page number to apply to break.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_text_flow`
         """
 
         direct = InnerBreaks(type=type, style=style, num=num)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/text_flow/flow_options.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/text_flow/flow_options.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 # endregion Import
 
 
 class FlowOptions(ParaStyleBaseMulti):
     """
     Paragraph Style Flow Options
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_text_flow`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         orphans: int | None = None,
@@ -37,14 +41,17 @@
             no_split (bool, optional): Do not split paragraph.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_text_flow`
         """
 
         direct = InnerFlowOptions(orphans=orphans, widows=widows, keep=keep, no_split=no_split)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/text_flow/hyphenation.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/text_flow/hyphenation.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 # endregion Import
 
 
 class Hyphenation(ParaStyleBaseMulti):
     """
     Paragraph Style Hyphenation
 
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_text_flow`
+
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
         auto: bool | None = None,
@@ -39,14 +43,17 @@
             max (int, optional): Maximum consecutive hyphenated lines.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_text_flow`
         """
 
         direct = InnerHyphenation(auto=auto, no_caps=no_caps, start_chars=start_chars, end_chars=end_chars, max=max)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/modify/write/para/transparent/gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/modify/write/para/transparent/transparency.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,105 +1,100 @@
 # region Import
 from __future__ import annotations
-from typing import cast, Any
+from typing import cast
 import uno
-from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
-
-from ooodev.utils.data_type.angle import Angle as Angle
 from ooodev.utils.data_type.intensity import Intensity as Intensity
-from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
-from ooodev.utils.data_type.offset import Offset as Offset
 from ooodev.format.writer.style.para.kind import StyleParaKind as StyleParaKind
-from ooodev.format.inner.direct.write.fill.transparent.gradient import Gradient as InnerGradient
+from ooodev.format.inner.direct.write.fill.transparent.transparency import Transparency as InnerTransparency
 from ..para_style_base_multi import ParaStyleBaseMulti
 
 # endregion Import
 
 
-class Gradient(ParaStyleBaseMulti):
+class Transparency(ParaStyleBaseMulti):
     """
-    Paragraph Style Gradient
+    Paragraph Style Transparency
+
+    .. seealso::
+
+        - :ref:`help_writer_format_modify_para_transparency`
 
     .. versionadded:: 0.9.0
     """
 
     def __init__(
         self,
         *,
-        style: GradientStyle = GradientStyle.LINEAR,
-        offset: Offset = Offset(50, 50),
-        angle: Angle | int = 0,
-        border: Intensity | int = 0,
-        grad_intensity: IntensityRange = IntensityRange(0, 0),
+        value: Intensity | int = 0,
         style_name: StyleParaKind | str = StyleParaKind.STANDARD,
         style_family: str = "ParagraphStyles",
-        **kwargs: Any,
     ) -> None:
         """
         Constructor
 
         Args:
             value (Intensity, int, optional): Specifies the transparency value from ``0`` to ``100``.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
             None:
+
+        See Also:
+            - :ref:`help_writer_format_modify_para_transparency`
         """
 
-        direct = InnerGradient(
-            style=style, offset=offset, angle=angle, border=border, grad_intensity=grad_intensity, kwargs=kwargs
-        )
+        direct = InnerTransparency(value=value)
         super().__init__()
         self._style_name = str(style_name)
         self._style_family_name = style_family
         self._set_style("direct", direct, *direct.get_attrs())
 
     @classmethod
     def from_style(
         cls,
         doc: object,
         style_name: StyleParaKind | str = StyleParaKind.STANDARD,
         style_family: str = "ParagraphStyles",
-    ) -> Gradient:
+    ) -> Transparency:
         """
         Gets instance from Document.
 
         Args:
             doc (object): UNO Document Object.
             style_name (StyleParaKind, str, optional): Specifies the Paragraph Style that instance applies to.
                 Default is Default Paragraph Style.
             style_family (str, optional): Style family. Default ``ParagraphStyles``.
 
         Returns:
-            Gradient: ``Gradient`` instance from document properties.
+            Transparency: ``Transparency`` instance from document properties.
         """
         inst = cls(style_name=style_name, style_family=style_family)
-        direct = InnerGradient.from_obj(inst.get_style_props(doc))
+        direct = InnerTransparency.from_obj(inst.get_style_props(doc))
         inst._set_style("direct", direct, *direct.get_attrs())
         return inst
 
     @property
     def prop_style_name(self) -> str:
         """Gets/Sets property Style Name"""
         return self._style_name
 
     @prop_style_name.setter
     def prop_style_name(self, value: str | StyleParaKind):
         self._style_name = str(value)
 
     @property
-    def prop_inner(self) -> InnerGradient:
-        """Gets/Sets Inner Gradient instance"""
+    def prop_inner(self) -> InnerTransparency:
+        """Gets/Sets Inner Transparency instance"""
         try:
             return self._direct_inner
         except AttributeError:
-            self._direct_inner = cast(InnerGradient, self._get_style_inst("direct"))
+            self._direct_inner = cast(InnerTransparency, self._get_style_inst("direct"))
         return self._direct_inner
 
     @prop_inner.setter
-    def prop_inner(self, value: InnerGradient) -> None:
-        if not isinstance(value, InnerGradient):
-            raise TypeError(f'Expected type of InnerGradient, got "{type(value).__name__}"')
+    def prop_inner(self, value: InnerTransparency) -> None:
+        if not isinstance(value, InnerTransparency):
+            raise TypeError(f'Expected type of InnerTransparency, got "{type(value).__name__}"')
         self._del_attribs("_direct_inner")
         self._set_style("direct", value, *value.get_attrs())
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/preset/preset_border_line.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/preset/preset_border_line.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/preset/preset_gradient.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/preset/preset_gradient.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/preset/preset_hatch.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/preset/preset_hatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/preset/preset_image.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/preset/preset_image.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/preset/preset_paper_format.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/preset/preset_paper_format.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/preset/preset_pattern.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/preset/preset_pattern.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/inner/style_base.py` & `ooo_dev_tools-0.9.7/ooodev/format/inner/style_base.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/readme.md` & `ooo_dev_tools-0.9.7/ooodev/format/readme.md`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/styler.py` & `ooo_dev_tools-0.9.7/ooodev/format/styler.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/char/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/header/borders/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 import uno
-from ooo.dyn.table.border_line import BorderLine as BorderLine
-from ooo.dyn.table.border_line2 import BorderLine2 as BorderLine2
-from ooo.dyn.table.shadow_format import ShadowFormat as ShadowFormat
 from ooo.dyn.table.shadow_location import ShadowLocation as ShadowLocation
 
 from ooodev.format.inner.direct.structs.side import BorderLineKind as BorderLineKind
 from ooodev.format.inner.direct.structs.side import LineSize as LineSize
 from ooodev.format.inner.direct.structs.side import Side as Side
-from ooodev.format.inner.direct.write.char.border.borders import Borders as Borders
-from ooodev.format.inner.direct.write.char.border.padding import Padding as Padding
-from ooodev.format.inner.direct.write.char.border.shadow import Shadow as Shadow
-from ooodev.format.inner.direct.write.char.border.sides import Sides as Sides
+from ooodev.format.inner.modify.write.page.header.border.padding import InnerPadding as InnerPadding
+from ooodev.format.inner.modify.write.page.header.border.padding import Padding as Padding
+from ooodev.format.inner.modify.write.page.header.border.shadow import InnerShadow as InnerShadow
+from ooodev.format.inner.modify.write.page.header.border.shadow import Shadow as Shadow
+from ooodev.format.inner.modify.write.page.header.border.sides import InnerSides as InnerSides
+from ooodev.format.inner.modify.write.page.header.border.sides import Sides as Sides
+from ooodev.format.writer.style.page.kind.writer_style_page_kind import WriterStylePageKind as WriterStylePageKind
 
-__all__ = [
-    "BorderLineKind",
-    "LineSize",
-    "Side",
-    "Borders",
-    "Padding",
-    "Shadow",
-    "Sides",
-]
+
+__all__ = ["Padding", "Shadow", "Sides"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/char/font/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/char/font/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,17 +16,8 @@
 from ooodev.format.inner.direct.write.char.font.font_only import FontLang as FontLang
 from ooodev.format.inner.direct.write.char.font.font_only import FontOnly as FontOnly
 from ooodev.format.inner.direct.write.char.font.font_position import CharSpacingKind as CharSpacingKind
 from ooodev.format.inner.direct.write.char.font.font_position import FontPosition as FontPosition
 from ooodev.format.inner.direct.write.char.font.font_position import FontScriptKind as FontScriptKind
 from ooodev.format.writer.style.char.kind.style_char_kind import StyleCharKind as StyleCharKind
 
-__all__ = [
-    "FontPosition",
-    "FontScriptKind",
-    "CharSpacingKind",
-    "Font",
-    "FontEffects",
-    "FontLine",
-    "FontOnly",
-    "FontLang",
-]
+__all__ = ["Font", "FontEffects", "FontOnly", "FontPosition"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/frame/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/page/header/area/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,25 @@
 import uno
 from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
-from ooo.dyn.drawing.hatch_style import HatchStyle as HatchStyle
 from ooo.dyn.drawing.rectangle_point import RectanglePoint as RectanglePoint
+from ooo.dyn.drawing.hatch_style import HatchStyle as HatchStyle
 
-from ooodev.utils.data_type.angle import Angle as Angle
-from ooodev.utils.data_type.color_range import ColorRange as ColorRange
-from ooodev.utils.data_type.intensity import Intensity as Intensity
-from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
-from ooodev.utils.data_type.offset import Offset as Offset
 from ooodev.format.inner.common.format_types.offset_column import OffsetColumn as OffsetColumn
 from ooodev.format.inner.common.format_types.offset_row import OffsetRow as OffsetRow
-from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 from ooodev.format.inner.common.format_types.size_percent import SizePercent as SizePercent
-from ooodev.format.inner.direct.write.fill.area.img import ImgStyleKind as ImgStyleKind
+from ooodev.format.inner.direct.write.page.header.area.color import Color as Color
+from ooodev.format.inner.direct.write.page.header.area.gradient import Gradient as Gradient
+from ooodev.format.inner.direct.write.page.header.area.hatch import Hatch as Hatch
+from ooodev.format.inner.direct.write.page.header.area.img import Img as Img
+from ooodev.format.inner.direct.write.page.header.area.pattern import Pattern as Pattern
 from ooodev.format.inner.preset.preset_gradient import PresetGradientKind as PresetGradientKind
 from ooodev.format.inner.preset.preset_hatch import PresetHatchKind as PresetHatchKind
 from ooodev.format.inner.preset.preset_image import PresetImageKind as PresetImageKind
 from ooodev.format.inner.preset.preset_pattern import PresetPatternKind as PresetPatternKind
-from ooodev.format.inner.direct.write.fill.area.fill_color import FillColor as Color
-from ooodev.format.inner.direct.write.fill.area.gradient import Gradient as Gradient
-from ooodev.format.inner.direct.write.fill.area.hatch import Hatch as Hatch
-from ooodev.format.inner.direct.write.fill.area.img import Img as Img
-from ooodev.format.inner.direct.write.fill.area.pattern import Pattern as Pattern
+from ooodev.utils.data_type.angle import Angle as Angle
+from ooodev.utils.data_type.color_range import ColorRange as ColorRange
+from ooodev.utils.data_type.intensity import Intensity as Intensity
+from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
+from ooodev.utils.data_type.offset import Offset as Offset
+from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 
-__all__ = [
-    "OffsetColumn",
-    "OffsetRow",
-    "SizePercent",
-    "ImgStyleKind",
-    "PresetGradientKind",
-    "PresetHatchKind",
-    "PresetImageKind",
-    "PresetPatternKind",
-    "Color",
-    "Gradient",
-    "Hatch",
-    "Img",
-    "Pattern",
-]
+__all__ = ["Color", "Gradient", "Hatch", "Img", "Pattern"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/frame/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/para/borders/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import uno
+from ooo.dyn.table.border_line import BorderLine as BorderLine
+from ooo.dyn.table.border_line2 import BorderLine2 as BorderLine2
+from ooo.dyn.table.shadow_format import ShadowFormat as ShadowFormat
 from ooo.dyn.table.shadow_location import ShadowLocation as ShadowLocation
-
-from ooodev.format.inner.direct.structs.side import Side as Side
-from ooodev.format.inner.direct.structs.side import LineSize as LineSize
 from ooodev.format.inner.direct.structs.side import BorderLineKind as BorderLineKind
+from ooodev.format.inner.direct.structs.side import LineSize as LineSize
+from ooodev.format.inner.direct.structs.side import Side as Side
 from ooodev.format.inner.direct.write.para.border.padding import Padding as Padding
-from ooodev.format.inner.direct.structs.shadow_struct import ShadowStruct as Shadow
-from ooodev.format.inner.direct.write.para.border.sides import Sides as Sides
+from ooodev.format.inner.direct.write.para.border.shadow import Shadow as Shadow
+from ooodev.format.inner.direct.write.para.border.borders import Borders as Borders
 
-__all__ = ["Side", "LineSize", "BorderLineKind", "Padding", "Shadow", "Sides"]
+__all__ = ["Padding", "Shadow", "Borders"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/frame/options/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/frame/options/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 from ooodev.format.inner.direct.write.frame.options.align import VertAdjustKind as VertAdjustKind
 from ooodev.format.inner.direct.write.frame.options.properties import TextDirectionKind as TextDirectionKind
 from ooodev.format.inner.direct.write.frame.options.protect import Protect as Protect
 from ooodev.format.inner.direct.write.frame.options.align import Align as Align
 from ooodev.format.inner.direct.write.frame.options.properties import Properties as Properties
 from ooodev.format.inner.direct.write.frame.options.names import Names as Names
 
-__all__ = ["VertAdjustKind", "TextDirectionKind", "Protect", "Align", "Properties", "Names"]
+__all__ = ["Protect", "Align", "Properties", "Names"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/frame/transparency/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/frame/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/frame/type/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/frame/type/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,22 +8,8 @@
 from ooodev.format.inner.direct.write.frame.frame_type.position import Horizontal as Horizontal
 from ooodev.format.inner.direct.write.frame.frame_type.position import Vertical as Vertical
 from ooodev.format.inner.direct.write.frame.frame_type.position import Position as Position
 from ooodev.format.inner.direct.write.frame.frame_type.size import Size as Size
 from ooodev.format.inner.direct.write.frame.frame_type.anchor import AnchorKind as AnchorKind
 from ooodev.format.inner.direct.write.frame.frame_type.anchor import Anchor as Anchor
 
-__all__ = [
-    "RelativeKind",
-    "RelativeSize",
-    "AbsoluteSize",
-    "HoriOrient",
-    "VertOrient",
-    "RelHoriOrient",
-    "RelVertOrient",
-    "Horizontal",
-    "Vertical",
-    "Position",
-    "Size",
-    "AnchorKind",
-    "Anchor",
-]
+__all__ = ["Position", "Size", "Anchor"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/image/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/page/footer/area/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,25 @@
 import uno
 from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
-from ooo.dyn.drawing.hatch_style import HatchStyle as HatchStyle
 from ooo.dyn.drawing.rectangle_point import RectanglePoint as RectanglePoint
+from ooo.dyn.drawing.hatch_style import HatchStyle as HatchStyle
 
-from ooodev.utils.data_type.angle import Angle as Angle
-from ooodev.utils.data_type.color_range import ColorRange as ColorRange
-from ooodev.utils.data_type.intensity import Intensity as Intensity
-from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
-from ooodev.utils.data_type.offset import Offset as Offset
 from ooodev.format.inner.common.format_types.offset_column import OffsetColumn as OffsetColumn
 from ooodev.format.inner.common.format_types.offset_row import OffsetRow as OffsetRow
-from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 from ooodev.format.inner.common.format_types.size_percent import SizePercent as SizePercent
-from ooodev.format.inner.direct.write.fill.area.img import ImgStyleKind as ImgStyleKind
+from ooodev.format.inner.direct.write.page.footer.area.color import Color as Color
+from ooodev.format.inner.direct.write.page.footer.area.gradient import Gradient as Gradient
+from ooodev.format.inner.direct.write.page.footer.area.hatch import Hatch as Hatch
+from ooodev.format.inner.direct.write.page.footer.area.img import Img as Img
+from ooodev.format.inner.direct.write.page.footer.area.pattern import Pattern as Pattern
 from ooodev.format.inner.preset.preset_gradient import PresetGradientKind as PresetGradientKind
 from ooodev.format.inner.preset.preset_hatch import PresetHatchKind as PresetHatchKind
 from ooodev.format.inner.preset.preset_image import PresetImageKind as PresetImageKind
 from ooodev.format.inner.preset.preset_pattern import PresetPatternKind as PresetPatternKind
-from ooodev.format.inner.direct.write.fill.area.fill_color import FillColor as Color
-from ooodev.format.inner.direct.write.fill.area.gradient import Gradient as Gradient
-from ooodev.format.inner.direct.write.fill.area.hatch import Hatch as Hatch
-from ooodev.format.inner.direct.write.fill.area.img import Img as Img
-from ooodev.format.inner.direct.write.fill.area.pattern import Pattern as Pattern
+from ooodev.utils.data_type.angle import Angle as Angle
+from ooodev.utils.data_type.color_range import ColorRange as ColorRange
+from ooodev.utils.data_type.intensity import Intensity as Intensity
+from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
+from ooodev.utils.data_type.offset import Offset as Offset
+from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 
-__all__ = [
-    "OffsetColumn",
-    "OffsetRow",
-    "SizePercent",
-    "ImgStyleKind",
-    "PresetGradientKind",
-    "PresetHatchKind",
-    "PresetImageKind",
-    "PresetPatternKind",
-    "Color",
-    "Gradient",
-    "Hatch",
-    "Img",
-    "Pattern",
-]
+__all__ = ["Color", "Gradient", "Hatch", "Img", "Pattern"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/image/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/table/borders/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import uno
+from ooo.dyn.table.border_line import BorderLine as BorderLine
+from ooo.dyn.table.border_line2 import BorderLine2 as BorderLine2
+from ooo.dyn.table.shadow_format import ShadowFormat as ShadowFormat
 from ooo.dyn.table.shadow_location import ShadowLocation as ShadowLocation
-
-from ooodev.format.inner.direct.structs.side import Side as Side
-from ooodev.format.inner.direct.structs.side import LineSize as LineSize
 from ooodev.format.inner.direct.structs.side import BorderLineKind as BorderLineKind
-from ooodev.format.inner.direct.write.para.border.padding import Padding as Padding
-from ooodev.format.inner.direct.structs.shadow_struct import ShadowStruct as Shadow
-from ooodev.format.inner.direct.write.para.border.sides import Sides as Sides
+from ooodev.format.inner.direct.structs.side import LineSize as LineSize
+from ooodev.format.inner.direct.structs.side import Side as Side
+from ooodev.format.inner.direct.calc.border.padding import Padding as Padding
+from ooodev.format.inner.direct.calc.border.shadow import Shadow as Shadow
+from ooodev.format.inner.direct.write.table.borders.borders import Borders as Borders
 
-__all__ = ["Side", "LineSize", "BorderLineKind", "Padding", "Shadow", "Sides"]
+__all__ = ["Borders"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/image/transparency/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/image/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/obj/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/frame/area/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,30 @@
 import uno
 from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
 from ooo.dyn.drawing.hatch_style import HatchStyle as HatchStyle
 from ooo.dyn.drawing.rectangle_point import RectanglePoint as RectanglePoint
 
-from ooodev.utils.data_type.angle import Angle as Angle
-from ooodev.utils.data_type.color_range import ColorRange as ColorRange
-from ooodev.utils.data_type.intensity import Intensity as Intensity
-from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
-from ooodev.utils.data_type.offset import Offset as Offset
-from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 from ooodev.format.inner.common.format_types.offset_column import OffsetColumn as OffsetColumn
-from ooodev.format.inner.common.format_types.offset_row import OffsetRow as OffsetRow
+from ooodev.format.inner.common.format_types.offset_row import OffsetRow as OffsetwRow
 from ooodev.format.inner.common.format_types.size_percent import SizePercent as SizePercent
 from ooodev.format.inner.direct.write.fill.area.img import ImgStyleKind as ImgStyleKind
+from ooodev.format.inner.modify.write.frame.area.color import Color as Color
+from ooodev.format.inner.modify.write.frame.area.color import InnerColor as InnerColor
+from ooodev.format.inner.modify.write.frame.area.gradient import Gradient as Gradient
+from ooodev.format.inner.modify.write.frame.area.gradient import InnerGradient as InnerGradient
+from ooodev.format.inner.modify.write.frame.area.hatch import Hatch as Hatch
+from ooodev.format.inner.modify.write.frame.area.hatch import InnerHatch as InnerHatch
+from ooodev.format.inner.modify.write.frame.area.img import Img as Img
+from ooodev.format.inner.modify.write.frame.area.pattern import Pattern as Pattern
 from ooodev.format.inner.preset.preset_gradient import PresetGradientKind as PresetGradientKind
 from ooodev.format.inner.preset.preset_hatch import PresetHatchKind as PresetHatchKind
 from ooodev.format.inner.preset.preset_image import PresetImageKind as PresetImageKind
 from ooodev.format.inner.preset.preset_pattern import PresetPatternKind as PresetPatternKind
-from ooodev.format.inner.direct.write.fill.area.fill_color import FillColor as Color
-from ooodev.format.inner.direct.write.fill.area.gradient import Gradient as Gradient
-from ooodev.format.inner.direct.write.fill.area.hatch import Hatch as Hatch
-from ooodev.format.inner.direct.write.fill.area.img import Img as Img
-from ooodev.format.inner.direct.write.fill.area.pattern import Pattern as Pattern
+from ooodev.format.writer.style.frame.style_frame_kind import StyleFrameKind as StyleFrameKind
+from ooodev.utils.data_type.angle import Angle as Angle
+from ooodev.utils.data_type.color_range import ColorRange as ColorRange
+from ooodev.utils.data_type.intensity import Intensity as Intensity
+from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
+from ooodev.utils.data_type.offset import Offset as Offset
+from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 
-__all__ = [
-    "OffsetColumn",
-    "OffsetRow",
-    "SizePercent",
-    "ImgStyleKind",
-    "PresetGradientKind",
-    "PresetHatchKind",
-    "PresetImageKind",
-    "PresetPatternKind",
-    "Color",
-    "Gradient",
-    "Hatch",
-    "Img",
-    "Pattern",
-]
+__all__ = ["Color", "Gradient", "Hatch", "Img", "Pattern"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/obj/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/frame/borders/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uno
 from ooo.dyn.table.shadow_location import ShadowLocation as ShadowLocation
 
-from ooodev.format.inner.direct.structs.side import BorderLineKind as BorderLineKind
-from ooodev.format.inner.direct.structs.side import LineSize as LineSize
 from ooodev.format.inner.direct.structs.side import Side as Side
+from ooodev.format.inner.direct.structs.side import LineSize as LineSize
+from ooodev.format.inner.direct.structs.side import BorderLineKind as BorderLineKind
 from ooodev.format.inner.direct.write.para.border.padding import Padding as Padding
 from ooodev.format.inner.direct.structs.shadow_struct import ShadowStruct as Shadow
 from ooodev.format.inner.direct.write.para.border.sides import Sides as Sides
 
-__all__ = ["BorderLineKind", "LineSize", "Side", "Padding", "Shadow", "Sides"]
+__all__ = ["Padding", "Shadow", "Sides"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/obj/transparency/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/obj/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/page/footer/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/shape/area/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import uno
 from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
-from ooo.dyn.drawing.rectangle_point import RectanglePoint as RectanglePoint
 from ooo.dyn.drawing.hatch_style import HatchStyle as HatchStyle
+from ooo.dyn.drawing.rectangle_point import RectanglePoint as RectanglePoint
 
 from ooodev.format.inner.common.format_types.offset_column import OffsetColumn as OffsetColumn
 from ooodev.format.inner.common.format_types.offset_row import OffsetRow as OffsetRow
 from ooodev.format.inner.common.format_types.size_percent import SizePercent as SizePercent
-from ooodev.format.inner.direct.write.page.footer.area.color import Color as Color
-from ooodev.format.inner.direct.write.page.footer.area.gradient import Gradient as Gradient
-from ooodev.format.inner.direct.write.page.footer.area.hatch import Hatch as Hatch
-from ooodev.format.inner.direct.write.page.footer.area.img import Img as Img
-from ooodev.format.inner.direct.write.page.footer.area.pattern import Pattern as Pattern
+from ooodev.format.inner.direct.write.fill.area.fill_color import FillColor as Color
+from ooodev.format.inner.direct.write.fill.area.gradient import Gradient as Gradient
+from ooodev.format.inner.direct.write.fill.area.hatch import Hatch as Hatch
+from ooodev.format.inner.direct.write.fill.area.img import Img as Img
+from ooodev.format.inner.direct.write.fill.area.img import ImgStyleKind as ImgStyleKind
+from ooodev.format.inner.direct.write.fill.area.pattern import Pattern as Pattern
 from ooodev.format.inner.preset.preset_gradient import PresetGradientKind as PresetGradientKind
 from ooodev.format.inner.preset.preset_hatch import PresetHatchKind as PresetHatchKind
 from ooodev.format.inner.preset.preset_image import PresetImageKind as PresetImageKind
 from ooodev.format.inner.preset.preset_pattern import PresetPatternKind as PresetPatternKind
 from ooodev.utils.data_type.angle import Angle as Angle
 from ooodev.utils.data_type.color_range import ColorRange as ColorRange
 from ooodev.utils.data_type.intensity import Intensity as Intensity
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/page/header/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/frame/area/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import uno
 from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
-from ooo.dyn.drawing.rectangle_point import RectanglePoint as RectanglePoint
 from ooo.dyn.drawing.hatch_style import HatchStyle as HatchStyle
+from ooo.dyn.drawing.rectangle_point import RectanglePoint as RectanglePoint
 
+from ooodev.utils.data_type.angle import Angle as Angle
+from ooodev.utils.data_type.color_range import ColorRange as ColorRange
+from ooodev.utils.data_type.intensity import Intensity as Intensity
+from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
+from ooodev.utils.data_type.offset import Offset as Offset
 from ooodev.format.inner.common.format_types.offset_column import OffsetColumn as OffsetColumn
 from ooodev.format.inner.common.format_types.offset_row import OffsetRow as OffsetRow
+from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 from ooodev.format.inner.common.format_types.size_percent import SizePercent as SizePercent
-from ooodev.format.inner.direct.write.page.header.area.color import Color as Color
-from ooodev.format.inner.direct.write.page.header.area.gradient import Gradient as Gradient
-from ooodev.format.inner.direct.write.page.header.area.hatch import Hatch as Hatch
-from ooodev.format.inner.direct.write.page.header.area.img import Img as Img
-from ooodev.format.inner.direct.write.page.header.area.pattern import Pattern as Pattern
+from ooodev.format.inner.direct.write.fill.area.img import ImgStyleKind as ImgStyleKind
 from ooodev.format.inner.preset.preset_gradient import PresetGradientKind as PresetGradientKind
 from ooodev.format.inner.preset.preset_hatch import PresetHatchKind as PresetHatchKind
 from ooodev.format.inner.preset.preset_image import PresetImageKind as PresetImageKind
 from ooodev.format.inner.preset.preset_pattern import PresetPatternKind as PresetPatternKind
-from ooodev.utils.data_type.angle import Angle as Angle
-from ooodev.utils.data_type.color_range import ColorRange as ColorRange
-from ooodev.utils.data_type.intensity import Intensity as Intensity
-from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
-from ooodev.utils.data_type.offset import Offset as Offset
-from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
+from ooodev.format.inner.direct.write.fill.area.fill_color import FillColor as Color
+from ooodev.format.inner.direct.write.fill.area.gradient import Gradient as Gradient
+from ooodev.format.inner.direct.write.fill.area.hatch import Hatch as Hatch
+from ooodev.format.inner.direct.write.fill.area.img import Img as Img
+from ooodev.format.inner.direct.write.fill.area.pattern import Pattern as Pattern
 
 __all__ = ["Color", "Gradient", "Hatch", "Img", "Pattern"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/para/alignment/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/para/alignment/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 from ooo.dyn.style.paragraph_adjust import ParagraphAdjust as ParagraphAdjust
 from ooo.dyn.text.paragraph_vert_align import ParagraphVertAlignEnum as ParagraphVertAlignEnum
 from ooo.dyn.text.writing_mode2 import WritingMode2Enum as WritingMode2Enum
 from ooodev.format.inner.direct.write.para.align.alignment import LastLineKind as LastLineKind
 from ooodev.format.inner.direct.write.para.align.alignment import Alignment as Alignment
 from ooodev.format.inner.direct.write.para.align.writing_mode import WritingMode as WritingMode
 
-__all__ = ["LastLineKind", "Alignment", "WritingMode"]
+__all__ = ["Alignment", "WritingMode"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/para/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/para/area/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,8 @@
 from ooodev.format.inner.direct.write.fill.area.img import SizePercent as SizePercent
 from ooodev.format.inner.direct.write.fill.area.img import Offset as Offset
 from ooodev.format.inner.direct.write.fill.area.img import OffsetColumn as OffsetColumn
 from ooodev.format.inner.direct.write.fill.area.img import OffsetRow as OffsetRow
 from ooodev.format.inner.direct.write.para.area.img import Img as Img
 from ooodev.format.inner.direct.write.para.area.hatch import Hatch as Hatch
 
-__all__ = [
-    "Color",
-    "Gradient",
-    "Pattern",
-    "Img",
-    "Hatch",
-]
+__all__ = ["Color", "Gradient", "Pattern", "Img", "Hatch"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/para/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/char/borders/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import uno
 from ooo.dyn.table.border_line import BorderLine as BorderLine
 from ooo.dyn.table.border_line2 import BorderLine2 as BorderLine2
 from ooo.dyn.table.shadow_format import ShadowFormat as ShadowFormat
 from ooo.dyn.table.shadow_location import ShadowLocation as ShadowLocation
+
 from ooodev.format.inner.direct.structs.side import BorderLineKind as BorderLineKind
 from ooodev.format.inner.direct.structs.side import LineSize as LineSize
 from ooodev.format.inner.direct.structs.side import Side as Side
-from ooodev.format.inner.direct.write.para.border.padding import Padding as Padding
-from ooodev.format.inner.direct.write.para.border.shadow import Shadow as Shadow
-from ooodev.format.inner.direct.write.para.border.borders import Borders as Borders
+from ooodev.format.inner.direct.write.char.border.borders import Borders as Borders
+from ooodev.format.inner.direct.write.char.border.padding import Padding as Padding
+from ooodev.format.inner.direct.write.char.border.shadow import Shadow as Shadow
+from ooodev.format.inner.direct.write.char.border.sides import Sides as Sides
 
-__all__ = ["BorderLineKind", "LineSize", "Side", "Padding", "Shadow", "Borders"]
+__all__ = ["Borders", "Padding", "Shadow", "Sides"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/shape/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/image/area/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 import uno
 from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
 from ooo.dyn.drawing.hatch_style import HatchStyle as HatchStyle
 from ooo.dyn.drawing.rectangle_point import RectanglePoint as RectanglePoint
 
+from ooodev.utils.data_type.angle import Angle as Angle
+from ooodev.utils.data_type.color_range import ColorRange as ColorRange
+from ooodev.utils.data_type.intensity import Intensity as Intensity
+from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
+from ooodev.utils.data_type.offset import Offset as Offset
 from ooodev.format.inner.common.format_types.offset_column import OffsetColumn as OffsetColumn
 from ooodev.format.inner.common.format_types.offset_row import OffsetRow as OffsetRow
+from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 from ooodev.format.inner.common.format_types.size_percent import SizePercent as SizePercent
-from ooodev.format.inner.direct.write.fill.area.fill_color import FillColor as Color
-from ooodev.format.inner.direct.write.fill.area.gradient import Gradient as Gradient
-from ooodev.format.inner.direct.write.fill.area.hatch import Hatch as Hatch
-from ooodev.format.inner.direct.write.fill.area.img import Img as Img
 from ooodev.format.inner.direct.write.fill.area.img import ImgStyleKind as ImgStyleKind
-from ooodev.format.inner.direct.write.fill.area.pattern import Pattern as Pattern
 from ooodev.format.inner.preset.preset_gradient import PresetGradientKind as PresetGradientKind
 from ooodev.format.inner.preset.preset_hatch import PresetHatchKind as PresetHatchKind
 from ooodev.format.inner.preset.preset_image import PresetImageKind as PresetImageKind
 from ooodev.format.inner.preset.preset_pattern import PresetPatternKind as PresetPatternKind
-from ooodev.utils.data_type.angle import Angle as Angle
-from ooodev.utils.data_type.color_range import ColorRange as ColorRange
-from ooodev.utils.data_type.intensity import Intensity as Intensity
-from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
-from ooodev.utils.data_type.offset import Offset as Offset
-from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
+from ooodev.format.inner.direct.write.fill.area.fill_color import FillColor as Color
+from ooodev.format.inner.direct.write.fill.area.gradient import Gradient as Gradient
+from ooodev.format.inner.direct.write.fill.area.hatch import Hatch as Hatch
+from ooodev.format.inner.direct.write.fill.area.img import Img as Img
+from ooodev.format.inner.direct.write.fill.area.pattern import Pattern as Pattern
 
-__all__ = [
-    "Color",
-    "Gradient",
-    "Hatch",
-    "Img",
-    "Pattern",
-]
+__all__ = ["Color", "Gradient", "Hatch", "Img", "Pattern"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/shape/transparency/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/shape/transparency/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/table/background/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/direct/table/background/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/direct/table/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/borders/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import uno
-from ooo.dyn.table.border_line import BorderLine as BorderLine
-from ooo.dyn.table.border_line2 import BorderLine2 as BorderLine2
-from ooo.dyn.table.shadow_format import ShadowFormat as ShadowFormat
 from ooo.dyn.table.shadow_location import ShadowLocation as ShadowLocation
+
 from ooodev.format.inner.direct.structs.side import BorderLineKind as BorderLineKind
 from ooodev.format.inner.direct.structs.side import LineSize as LineSize
 from ooodev.format.inner.direct.structs.side import Side as Side
-from ooodev.format.inner.direct.calc.border.padding import Padding as Padding
-from ooodev.format.inner.direct.calc.border.shadow import Shadow as Shadow
-from ooodev.format.inner.direct.write.table.borders.borders import Borders as Borders
+from ooodev.format.inner.modify.write.page.border.padding import InnerPadding as InnerPadding
+from ooodev.format.inner.modify.write.page.border.padding import Padding as Padding
+from ooodev.format.inner.modify.write.page.border.shadow import InnerShadow as InnerShadow
+from ooodev.format.inner.modify.write.page.border.shadow import Shadow as Shadow
+from ooodev.format.inner.modify.write.page.border.sides import InnerSides as InnerSides
+from ooodev.format.inner.modify.write.page.border.sides import Sides as Sides
+from ooodev.format.writer.style.page.kind.writer_style_page_kind import WriterStylePageKind as WriterStylePageKind
 
-__all__ = ["Borders"]
+__all__ = ["Padding", "Shadow", "Sides"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/char/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/char/borders/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,18 +9,8 @@
 from ooodev.format.inner.modify.write.char.border.sides import InnerSides as InnerSides
 from ooodev.format.inner.modify.write.char.border.sides import Sides as Sides
 from ooodev.format.inner.modify.write.char.border.padding import InnerPadding as InnerPadding
 from ooodev.format.inner.modify.write.char.border.padding import Padding as Padding
 from ooodev.format.inner.modify.write.char.border.shadow import InnerShadow as InnerShadow
 from ooodev.format.inner.modify.write.char.border.shadow import Shadow as Shadow
 
-__all__ = [
-    "BorderLineKind",
-    "LineSize",
-    "Side",
-    "InnerSides",
-    "Sides",
-    "InnerPadding",
-    "Padding",
-    "InnerShadow",
-    "Shadow",
-]
+__all__ = ["Sides", "Padding", "Shadow"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/char/font/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/font/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 import uno
 from ooo.dyn.awt.font_strikeout import FontStrikeoutEnum as FontStrikeoutEnum
 from ooo.dyn.awt.font_underline import FontUnderlineEnum as FontUnderlineEnum
 from ooo.dyn.style.case_map import CaseMapEnum as CaseMapEnum
 from ooo.dyn.awt.font_relief import FontReliefEnum as FontReliefEnum
-from ooodev.utils.data_type.intensity import Intensity as Intensity
-from ooodev.utils.data_type.angle import Angle as Angle
-from ooodev.format.writer.style.char import StyleCharKind as StyleCharKind
-from ooodev.format.inner.direct.write.char.font.font_only import FontLang as FontLang
+
 from ooodev.format.inner.direct.write.char.font.font_effects import FontLine as FontLine
+from ooodev.format.inner.direct.write.char.font.font_only import FontLang as FontLang
 from ooodev.format.inner.direct.write.char.font.font_position import CharSpacingKind as CharSpacingKind
 from ooodev.format.inner.direct.write.char.font.font_position import FontScriptKind as FontScriptKind
-from ooodev.format.inner.modify.write.char.font.font_effects import FontEffects as FontEffects
-from ooodev.format.inner.modify.write.char.font.font_effects import InnerFontEffects as InnerFontEffects
-from ooodev.format.inner.modify.write.char.font.font_only import InnerFontOnly as InnerFontOnly
-from ooodev.format.inner.modify.write.char.font.font_only import FontOnly as FontOnly
-from ooodev.format.inner.modify.write.char.font.font_position import InnerFontPosition as InnerFontPosition
-from ooodev.format.inner.modify.write.char.font.font_position import FontPosition as FontPosition
+from ooodev.format.inner.modify.write.para.font.font_effects import FontEffects as FontEffects
+from ooodev.format.inner.modify.write.para.font.font_effects import InnerFontEffects as InnerFontEffects
+from ooodev.format.inner.modify.write.para.font.font_only import FontOnly as FontOnly
+from ooodev.format.inner.modify.write.para.font.font_only import InnerFontOnly as InnerFontOnly
+from ooodev.format.inner.modify.write.para.font.font_position import FontPosition as FontPosition
+from ooodev.format.inner.modify.write.para.font.font_position import InnerFontPosition as InnerFontPosition
+from ooodev.format.writer.style.para import StyleParaKind as StyleParaKind
+from ooodev.utils.data_type.angle import Angle as Angle
+from ooodev.utils.data_type.intensity import Intensity as Intensity
+
 
-__all__ = [
-    "FontLang",
-    "FontLine",
-    "CharSpacingKind",
-    "FontScriptKind",
-    "FontEffects",
-    "InnerFontEffects",
-    "InnerFontOnly",
-    "FontOnly",
-    "InnerFontPosition",
-    "FontPosition",
-]
+__all__ = ["FontEffects", "FontOnly", "FontPosition"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/frame/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/header/area/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,30 @@
 import uno
 from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
 from ooo.dyn.drawing.hatch_style import HatchStyle as HatchStyle
 from ooo.dyn.drawing.rectangle_point import RectanglePoint as RectanglePoint
 
 from ooodev.format.inner.common.format_types.offset_column import OffsetColumn as OffsetColumn
-from ooodev.format.inner.common.format_types.offset_row import OffsetRow as OffsetwRow
+from ooodev.format.inner.common.format_types.offset_row import OffsetRow as OffsetRow
 from ooodev.format.inner.common.format_types.size_percent import SizePercent as SizePercent
 from ooodev.format.inner.direct.write.fill.area.img import ImgStyleKind as ImgStyleKind
-from ooodev.format.inner.modify.write.frame.area.color import Color as Color
-from ooodev.format.inner.modify.write.frame.area.color import InnerColor as InnerColor
-from ooodev.format.inner.modify.write.frame.area.gradient import Gradient as Gradient
-from ooodev.format.inner.modify.write.frame.area.gradient import InnerGradient as InnerGradient
-from ooodev.format.inner.modify.write.frame.area.hatch import Hatch as Hatch
-from ooodev.format.inner.modify.write.frame.area.hatch import InnerHatch as InnerHatch
-from ooodev.format.inner.modify.write.frame.area.img import Img as Img
-from ooodev.format.inner.modify.write.frame.area.pattern import Pattern as Pattern
+from ooodev.format.inner.modify.write.page.header.area.color import Color as Color
+from ooodev.format.inner.modify.write.page.header.area.color import InnerColor as InnerColor
+from ooodev.format.inner.modify.write.page.header.area.gradient import Gradient as Gradient
+from ooodev.format.inner.modify.write.page.header.area.gradient import InnerGradient as InnerGradient
+from ooodev.format.inner.modify.write.page.header.area.hatch import Hatch as Hatch
+from ooodev.format.inner.modify.write.page.header.area.hatch import InnerHatch as InnerHatch
+from ooodev.format.inner.modify.write.page.header.area.img import Img as Img
+from ooodev.format.inner.modify.write.page.header.area.img import InnerImg as InnerImg
+from ooodev.format.inner.modify.write.page.header.area.pattern import InnerPattern as InnerPattern
+from ooodev.format.inner.modify.write.page.header.area.pattern import Pattern as Pattern
 from ooodev.format.inner.preset.preset_gradient import PresetGradientKind as PresetGradientKind
 from ooodev.format.inner.preset.preset_hatch import PresetHatchKind as PresetHatchKind
 from ooodev.format.inner.preset.preset_image import PresetImageKind as PresetImageKind
 from ooodev.format.inner.preset.preset_pattern import PresetPatternKind as PresetPatternKind
-from ooodev.format.writer.style.frame.style_frame_kind import StyleFrameKind as StyleFrameKind
 from ooodev.utils.data_type.angle import Angle as Angle
 from ooodev.utils.data_type.color_range import ColorRange as ColorRange
 from ooodev.utils.data_type.intensity import Intensity as Intensity
 from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
-from ooodev.utils.data_type.offset import Offset as Offset
 from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 
-__all__ = [
-    "OffsetColumn",
-    "OffsetwRow",
-    "SizePercent",
-    "ImgStyleKind",
-    "Color",
-    "InnerColor",
-    "Gradient",
-    "InnerGradient",
-    "Hatch",
-    "InnerHatch",
-    "Img",
-    "Pattern",
-    "PresetGradientKind",
-    "PresetHatchKind",
-    "PresetImageKind",
-    "PresetPatternKind",
-]
+__all__ = ["Color", "Gradient", "Hatch", "Img", "Pattern"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/frame/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/frame/borders/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,18 +8,8 @@
 from ooodev.format.inner.modify.write.frame.border.padding import Padding as Padding
 from ooodev.format.inner.modify.write.frame.border.shadow import InnerShadow as InnerShadow
 from ooodev.format.inner.modify.write.frame.border.shadow import Shadow as Shadow
 from ooodev.format.inner.modify.write.frame.border.sides import InnerSides as InnerSides
 from ooodev.format.inner.modify.write.frame.border.sides import Sides as Sides
 from ooodev.format.writer.style.frame.style_frame_kind import StyleFrameKind as StyleFrameKind
 
-__all__ = [
-    "BorderLineKind",
-    "LineSize",
-    "Side",
-    "InnerPadding",
-    "Padding",
-    "InnerShadow",
-    "Shadow",
-    "InnerSides",
-    "Sides",
-]
+__all__ = ["Padding", "Shadow", "Sides"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/frame/transparency/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/transparency/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import uno
 from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
 
-from ooodev.format.inner.modify.write.frame.transparent.gradient import Gradient as Gradient
-from ooodev.format.inner.modify.write.frame.transparent.transparency import InnerTransparency as InnerTransparency
-from ooodev.format.inner.modify.write.frame.transparent.transparency import Transparency as Transparency
-from ooodev.format.writer.style.frame.style_frame_kind import StyleFrameKind as StyleFrameKind
+from ooodev.format.inner.modify.write.para.transparent.gradient import Gradient as Gradient
+from ooodev.format.inner.modify.write.para.transparent.gradient import InnerGradient as InnerGradient
+from ooodev.format.inner.modify.write.para.transparent.transparency import InnerTransparency as InnerTransparency
+from ooodev.format.inner.modify.write.para.transparent.transparency import Transparency as Transparency
+from ooodev.format.writer.style.para.kind import StyleParaKind as StyleParaKind
 from ooodev.utils.data_type.angle import Angle as Angle
 from ooodev.utils.data_type.intensity import Intensity as Intensity
 from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
 from ooodev.utils.data_type.offset import Offset as Offset
 
-__all__ = ["Gradient", "InnerTransparency", "Transparency"]
+__all__ = ["Gradient", "Transparency"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/frame/type/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/frame/type/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,25 +12,8 @@
 from ooodev.format.inner.modify.write.frame.frame_type.anchor import InnerAnchor as InnerAnchor
 from ooodev.format.inner.modify.write.frame.frame_type.position import InnerPosition as InnerPosition
 from ooodev.format.inner.modify.write.frame.frame_type.position import Position as Position
 from ooodev.format.inner.modify.write.frame.frame_type.size import InnerSize as InnerSize
 from ooodev.format.inner.modify.write.frame.frame_type.size import Size as Size
 from ooodev.format.writer.style.frame.style_frame_kind import StyleFrameKind as StyleFrameKind
 
-__all__ = [
-    "AnchorKind",
-    "HoriOrient",
-    "Horizontal",
-    "RelHoriOrient",
-    "RelVertOrient",
-    "Vertical",
-    "VertOrient",
-    "AbsoluteSize",
-    "RelativeKind",
-    "RelativeSize",
-    "Anchor",
-    "InnerAnchor",
-    "InnerPosition",
-    "Position",
-    "InnerSize",
-    "Size",
-]
+__all__ = ["Anchor", "Position", "Size"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/frame/wrap/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/frame/wrap/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 from ooodev.format.inner.modify.write.frame.wrap.options import Options as Options
 from ooodev.format.inner.modify.write.frame.wrap.settings import InnerSettings as InnerSettings
 from ooodev.format.inner.modify.write.frame.wrap.settings import Settings as Settings
 from ooodev.format.inner.modify.write.frame.wrap.spacing import InnerSpacing as InnerSpacing
 from ooodev.format.inner.modify.write.frame.wrap.spacing import Spacing as Spacing
 from ooodev.format.writer.style.frame.style_frame_kind import StyleFrameKind as StyleFrameKind
 
-__all__ = ["InnerOptions", "Options", "InnerSettings", "Settings", "InnerSpacing", "Spacing"]
+__all__ = ["Options", "Settings", "Spacing"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/area/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,8 @@
 from ooodev.utils.data_type.angle import Angle as Angle
 from ooodev.utils.data_type.color_range import ColorRange as ColorRange
 from ooodev.utils.data_type.intensity import Intensity as Intensity
 from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
 from ooodev.utils.data_type.offset import Offset as Offset
 from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 
-__all__ = [
-    "Color",
-    "InnerColor",
-    "Gradient",
-    "Hatch",
-    "Img",
-    "InnerImg",
-    "InnerPattern",
-    "Pattern",
-]
+__all__ = ["Color", "Gradient", "Hatch", "Img", "Pattern"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/borders/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 import uno
+from ooo.dyn.table.shadow_format import ShadowFormat as ShadowFormat
 from ooo.dyn.table.shadow_location import ShadowLocation as ShadowLocation
 
 from ooodev.format.inner.direct.structs.side import BorderLineKind as BorderLineKind
 from ooodev.format.inner.direct.structs.side import LineSize as LineSize
 from ooodev.format.inner.direct.structs.side import Side as Side
-from ooodev.format.inner.modify.write.page.border.padding import InnerPadding as InnerPadding
-from ooodev.format.inner.modify.write.page.border.padding import Padding as Padding
-from ooodev.format.inner.modify.write.page.border.shadow import InnerShadow as InnerShadow
-from ooodev.format.inner.modify.write.page.border.shadow import Shadow as Shadow
-from ooodev.format.inner.modify.write.page.border.sides import InnerSides as InnerSides
-from ooodev.format.inner.modify.write.page.border.sides import Sides as Sides
-from ooodev.format.writer.style.page.kind.writer_style_page_kind import WriterStylePageKind as WriterStylePageKind
+from ooodev.format.inner.modify.write.para.border.borders import Borders as Borders
+from ooodev.format.inner.modify.write.para.border.borders import InnerBorders as InnerBorders
+from ooodev.format.inner.modify.write.para.border.padding import InnerPadding as InnerPadding
+from ooodev.format.inner.modify.write.para.border.padding import Padding as Padding
+from ooodev.format.inner.modify.write.para.border.shadow import InnerShadow as InnerShadow
+from ooodev.format.inner.modify.write.para.border.shadow import Shadow as Shadow
+from ooodev.format.inner.modify.write.para.border.sides import InnerSides as InnerSides
+from ooodev.format.inner.modify.write.para.border.sides import Sides as Sides
+from ooodev.format.writer.style.para import StyleParaKind as StyleParaKind
 
-__all__ = [
-    "BorderLineKind",
-    "LineSize",
-    "Side",
-    "InnerPadding",
-    "Padding",
-    "InnerShadow",
-    "Shadow",
-    "InnerSides",
-    "Sides",
-]
+__all__ = ["Padding", "Shadow", "Sides"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/footer/area/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/area/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,29 @@
 import uno
-from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
-from ooo.dyn.drawing.hatch_style import HatchStyle as HatchStyle
 from ooo.dyn.drawing.rectangle_point import RectanglePoint as RectanglePoint
+from ooo.dyn.drawing.hatch_style import HatchStyle as HatchStyle
 
-from ooodev.format.inner.common.format_types.offset_column import OffsetColumn as OffsetColumn
-from ooodev.format.inner.common.format_types.offset_row import OffsetRow as OffsetRow
-from ooodev.format.inner.common.format_types.size_percent import SizePercent as SizePercent
 from ooodev.format.inner.direct.write.fill.area.img import ImgStyleKind as ImgStyleKind
-from ooodev.format.inner.modify.write.page.footer.area.color import Color as Color
-from ooodev.format.inner.modify.write.page.footer.area.gradient import Gradient as Gradient
-from ooodev.format.inner.modify.write.page.footer.area.hatch import Hatch as Hatch
-from ooodev.format.inner.modify.write.page.footer.area.img import Img as Img
-from ooodev.format.inner.modify.write.page.footer.area.pattern import Pattern as Pattern
-from ooodev.format.inner.modify.write.page.header.area.color import InnerColor as InnerColor
-from ooodev.format.inner.modify.write.page.header.area.gradient import InnerGradient as InnerGradient
-from ooodev.format.inner.modify.write.page.header.area.hatch import InnerHatch as InnerHatch
-from ooodev.format.inner.modify.write.page.header.area.img import InnerImg as InnerImg
-from ooodev.format.inner.modify.write.page.header.area.pattern import InnerPattern as InnerPattern
+from ooodev.format.inner.direct.write.fill.area.img import OffsetColumn as OffsetColumn
+from ooodev.format.inner.direct.write.fill.area.img import OffsetRow as OffsetRow
+from ooodev.format.inner.direct.write.fill.area.img import SizePercent as SizePercent
+from ooodev.format.inner.modify.write.para.area.color import Color as Color
+from ooodev.format.inner.modify.write.para.area.gradient import Gradient as Gradient
+from ooodev.format.inner.modify.write.para.area.hatch import Hatch as Hatch
+from ooodev.format.inner.modify.write.para.area.hatch import InnerHatch as InnerHatch
+from ooodev.format.inner.modify.write.para.area.img import Img as Img
+from ooodev.format.inner.modify.write.para.area.img import InnerImg as InnerImg
+from ooodev.format.inner.modify.write.para.area.pattern import InnerPattern as InnerPattern
+from ooodev.format.inner.modify.write.para.area.pattern import Pattern as Pattern
 from ooodev.format.inner.preset.preset_gradient import PresetGradientKind as PresetGradientKind
 from ooodev.format.inner.preset.preset_hatch import PresetHatchKind as PresetHatchKind
 from ooodev.format.inner.preset.preset_image import PresetImageKind as PresetImageKind
 from ooodev.format.inner.preset.preset_pattern import PresetPatternKind as PresetPatternKind
+from ooodev.format.writer.style.para.kind import StyleParaKind as StyleParaKind
 from ooodev.utils.data_type.angle import Angle as Angle
 from ooodev.utils.data_type.color_range import ColorRange as ColorRange
 from ooodev.utils.data_type.intensity import Intensity as Intensity
 from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
+from ooodev.utils.data_type.offset import Offset as Offset
 from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 
-__all__ = [
-    "OffsetColumn",
-    "OffsetRow",
-    "SizePercent",
-    "ImgStyleKind",
-    "Color",
-    "Gradient",
-    "Hatch",
-    "Img",
-    "Pattern",
-    "InnerColor",
-    "InnerGradient",
-    "InnerHatch",
-    "InnerImg",
-    "InnerPattern",
-    "PresetGradientKind",
-    "PresetHatchKind",
-    "PresetImageKind",
-    "PresetPatternKind",
-]
+__all__ = ["Color", "Gradient", "Hatch", "Img", "Pattern"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/footer/borders/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/outline_list/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,12 @@
 import uno
-from ooo.dyn.table.shadow_location import ShadowLocation as ShadowLocation
+from ooodev.format.inner.direct.write.para.outline_list.outline import LevelKind as LevelKind
+from ooodev.format.inner.modify.write.para.outline_list.line_num import InnerLineNum as InnerLineNum
+from ooodev.format.inner.modify.write.para.outline_list.line_num import LineNum as LineNum
+from ooodev.format.inner.modify.write.para.outline_list.list_style import InnerListStyle as InnerListStyle
+from ooodev.format.inner.modify.write.para.outline_list.list_style import ListStyle as ListStyle
+from ooodev.format.inner.modify.write.para.outline_list.outline import InnerOutline as InnerOutline
+from ooodev.format.inner.modify.write.para.outline_list.outline import Outline as Outline
+from ooodev.format.writer.style.lst import StyleListKind as StyleListKind
+from ooodev.format.writer.style.para.kind import StyleParaKind as StyleParaKind
 
-from ooodev.format.inner.direct.structs.side import BorderLineKind as BorderLineKind
-from ooodev.format.inner.direct.structs.side import LineSize as LineSize
-from ooodev.format.inner.direct.structs.side import Side as Side
-from ooodev.format.inner.modify.write.page.footer.border.padding import Padding as Padding
-from ooodev.format.inner.modify.write.page.footer.border.shadow import Shadow as Shadow
-from ooodev.format.inner.modify.write.page.footer.border.sides import Sides as Sides
-from ooodev.format.inner.modify.write.page.header.border.padding import InnerPadding as InnerPadding
-from ooodev.format.inner.modify.write.page.header.border.shadow import InnerShadow as InnerShadow
-from ooodev.format.inner.modify.write.page.header.border.sides import InnerSides as InnerSides
-from ooodev.format.writer.style.page.kind.writer_style_page_kind import WriterStylePageKind as WriterStylePageKind
-
-__all__ = [
-    "BorderLineKind",
-    "LineSize",
-    "Side",
-    "Padding",
-    "Shadow",
-    "Sides",
-    "InnerPadding",
-    "InnerShadow",
-    "InnerSides",
-]
+__all__ = ["LineNum", "ListStyle", "Outline"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/footer/transparency/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/footer/transparency/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 )
 from ooodev.format.writer.style.page.kind.writer_style_page_kind import WriterStylePageKind as WriterStylePageKind
 from ooodev.utils.data_type.angle import Angle as Angle
 from ooodev.utils.data_type.intensity import Intensity as Intensity
 from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
 from ooodev.utils.data_type.offset import Offset as Offset
 
-__all__ = ["Gradient", "Transparency", "InnerGradient", "InnerTransparency"]
+__all__ = ["Gradient", "Transparency"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/header/transparency/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/transparency/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import uno
 from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
 
-from ooodev.format.inner.modify.write.page.header.transparency.gradient import Gradient as Gradient
-from ooodev.format.inner.modify.write.page.header.transparency.gradient import InnerGradient as InnerGradient
-from ooodev.format.inner.modify.write.page.header.transparency.transparency import (
-    InnerTransparency as InnerTransparency,
-)
-from ooodev.format.inner.modify.write.page.header.transparency.transparency import Transparency as Transparency
+from ooodev.format.inner.modify.write.page.transparency.gradient import Gradient as Gradient
+from ooodev.format.inner.modify.write.page.transparency.gradient import InnerGradient as InnerGradient
+from ooodev.format.inner.modify.write.page.transparency.transparency import InnerTransparency as InnerTransparency
+from ooodev.format.inner.modify.write.page.transparency.transparency import Transparency as Transparency
 from ooodev.format.writer.style.page.kind.writer_style_page_kind import WriterStylePageKind as WriterStylePageKind
 from ooodev.utils.data_type.angle import Angle as Angle
 from ooodev.utils.data_type.intensity import Intensity as Intensity
 from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
 from ooodev.utils.data_type.offset import Offset as Offset
 
-__all__ = ["Gradient", "InnerGradient", "InnerTransparency", "Transparency"]
+__all__ = ["Gradient", "Transparency"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/page/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/page/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,10 @@
 from ooodev.format.inner.modify.write.page.page.layout_settings import LayoutSettings as LayoutSettings
 from ooodev.format.inner.modify.write.page.page.margins import InnerMargins as InnerMargins
 from ooodev.format.inner.modify.write.page.page.margins import Margins as Margins
 from ooodev.format.inner.modify.write.page.page.paper_format import InnerPaperFormat as InnerPaperFormat
 from ooodev.format.inner.modify.write.page.page.paper_format import PaperFormat as PaperFormat
 from ooodev.format.inner.preset.preset_paper_format import PaperFormatKind as PaperFormatKind
 from ooodev.format.writer.style.page.kind.writer_style_page_kind import WriterStylePageKind as WriterStylePageKind
-from ooodev.format.writer.style.para.kind.style_para_kind import StyleParaKind as StyleParaKind
 from ooodev.utils.data_type.size_mm import SizeMM as SizeMM
 
-__all__ = [
-    "InnerLayoutSettings",
-    "LayoutSettings",
-    "InnerMargins",
-    "Margins",
-    "InnerPaperFormat",
-    "PaperFormat",
-    "PaperFormatKind",
-]
+__all__ = ["LayoutSettings", "Margins", "PaperFormat"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/page_style_base.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/page_style_base.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/page_style_base_multi.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/page_style_base_multi.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/page/transparency/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/page/header/transparency/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import uno
 from ooo.dyn.awt.gradient_style import GradientStyle as GradientStyle
 
-from ooodev.format.inner.modify.write.page.transparency.gradient import Gradient as Gradient
-from ooodev.format.inner.modify.write.page.transparency.gradient import InnerGradient as InnerGradient
-from ooodev.format.inner.modify.write.page.transparency.transparency import InnerTransparency as InnerTransparency
-from ooodev.format.inner.modify.write.page.transparency.transparency import Transparency as Transparency
+from ooodev.format.inner.modify.write.page.header.transparency.gradient import Gradient as Gradient
+from ooodev.format.inner.modify.write.page.header.transparency.gradient import InnerGradient as InnerGradient
+from ooodev.format.inner.modify.write.page.header.transparency.transparency import (
+    InnerTransparency as InnerTransparency,
+)
+from ooodev.format.inner.modify.write.page.header.transparency.transparency import Transparency as Transparency
 from ooodev.format.writer.style.page.kind.writer_style_page_kind import WriterStylePageKind as WriterStylePageKind
 from ooodev.utils.data_type.angle import Angle as Angle
 from ooodev.utils.data_type.intensity import Intensity as Intensity
 from ooodev.utils.data_type.intensity_range import IntensityRange as IntensityRange
 from ooodev.utils.data_type.offset import Offset as Offset
 
-__all__ = ["Gradient", "InnerGradient", "InnerTransparency", "Transparency"]
+__all__ = ["Gradient", "Transparency"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/alignment/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/alignment/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 
 from ooodev.format.inner.direct.write.para.align.alignment import LastLineKind as LastLineKind
 from ooodev.format.inner.direct.write.para.align.writing_mode import WritingMode as WritingMode
 from ooodev.format.inner.modify.write.para.align.alignment import Alignment as Alignment
 from ooodev.format.inner.modify.write.para.align.alignment import InnerAlignment as InnerAlignment
 from ooodev.format.writer.style.para.kind import StyleParaKind as StyleParaKind
 
-__all__ = ["LastLineKind", "WritingMode", "Alignment", "InnerAlignment"]
+__all__ = ["Alignment"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/indent_space/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/indent_space/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,8 +4,8 @@
 from ooodev.format.inner.modify.write.para.indent_space.indent import InnerIndent as InnerIndent
 from ooodev.format.inner.modify.write.para.indent_space.line_spacing import InnerLineSpacing as InnerLineSpacing
 from ooodev.format.inner.modify.write.para.indent_space.line_spacing import LineSpacing as LineSpacing
 from ooodev.format.inner.modify.write.para.indent_space.spacing import InnerSpacing as InnerSpacing
 from ooodev.format.inner.modify.write.para.indent_space.spacing import Spacing as Spacing
 from ooodev.format.writer.style.para.kind import StyleParaKind as StyleParaKind
 
-__all__ = ["ModeKind", "Indent", "InnerIndent", "InnerLineSpacing", "LineSpacing", "InnerSpacing", "Spacing"]
+__all__ = ["Indent", "LineSpacing", "Spacing"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/modify/para/text_flow/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/modify/para/text_flow/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 from ooodev.format.inner.modify.write.para.text_flow.breaks import InnerBreaks as InnerBreaks
 from ooodev.format.inner.modify.write.para.text_flow.flow_options import FlowOptions as FlowOptions
 from ooodev.format.inner.modify.write.para.text_flow.flow_options import InnerFlowOptions as InnerFlowOptions
 from ooodev.format.inner.modify.write.para.text_flow.hyphenation import Hyphenation as Hyphenation
 from ooodev.format.inner.modify.write.para.text_flow.hyphenation import InnerHyphenation as InnerHyphenation
 from ooodev.format.writer.style.para.kind import StyleParaKind as StyleParaKind
 
-__all__ = ["Breaks", "InnerBreaks", "FlowOptions", "InnerFlowOptions", "Hyphenation", "InnerHyphenation"]
+__all__ = ["Breaks", "FlowOptions", "Hyphenation"]
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/bullet_list/bullet_list.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/bullet_list/bullet_list.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/char/char.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/char/char.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/char/kind/style_char_kind.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/char/kind/style_char_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/frame/frame.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/frame/frame.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/lst/style_list_kind.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/lst/style_list_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/page/page.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/page/page.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_para_html_kind.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_para_html_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_para_index_kind.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_para_index_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_para_kind.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_para_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_para_list_kind.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_para_list_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_para_special_kind.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_para_special_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/kind/style_para_text_kind.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/kind/style_para_text_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/format/writer/style/para/para.py` & `ooo_dev_tools-0.9.7/ooodev/format/writer/style/para/para.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/formatters/format_list_item.py` & `ooo_dev_tools-0.9.7/ooodev/formatters/format_list_item.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/formatters/format_string.py` & `ooo_dev_tools-0.9.7/ooodev/formatters/format_string.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/formatters/format_table_item.py` & `ooo_dev_tools-0.9.7/ooodev/formatters/format_table_item.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/formatters/formatter_list.py` & `ooo_dev_tools-0.9.7/ooodev/formatters/formatter_list.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/formatters/formatter_table.py` & `ooo_dev_tools-0.9.7/ooodev/formatters/formatter_table.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/formatters/table_item_kind.py` & `ooo_dev_tools-0.9.7/ooodev/formatters/table_item_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/formatters/table_item_processer.py` & `ooo_dev_tools-0.9.7/ooodev/formatters/table_item_processer.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/lazy/lazy_import.py` & `ooo_dev_tools-0.9.7/ooodev/lazy/lazy_import.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/listeners/x_event_adapter.py` & `ooo_dev_tools-0.9.7/ooodev/listeners/x_event_adapter.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/listeners/x_modify_adapter.py` & `ooo_dev_tools-0.9.7/ooodev/listeners/x_modify_adapter.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/listeners/x_selection_change_adapter.py` & `ooo_dev_tools-0.9.7/ooodev/listeners/x_selection_change_adapter.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/listeners/x_terminate_adapter.py` & `ooo_dev_tools-0.9.7/ooodev/listeners/x_terminate_adapter.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/listeners/x_top_window_adapter.py` & `ooo_dev_tools-0.9.7/ooodev/listeners/x_top_window_adapter.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/meta/class_property_readonly.py` & `ooo_dev_tools-0.9.7/ooodev/meta/class_property_readonly.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/meta/deleted_attrib.py` & `ooo_dev_tools-0.9.7/ooodev/meta/deleted_attrib.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/meta/deleted_enum_meta.py` & `ooo_dev_tools-0.9.7/ooodev/meta/deleted_enum_meta.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/meta/disabled_method.py` & `ooo_dev_tools-0.9.7/ooodev/meta/disabled_method.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/meta/static_meta.py` & `ooo_dev_tools-0.9.7/ooodev/meta/static_meta.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/meta/static_prop.py` & `ooo_dev_tools-0.9.7/ooodev/meta/static_prop.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/mock/mock_g.py` & `ooo_dev_tools-0.9.7/ooodev/mock/mock_g.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/mock/unohelper.py` & `ooo_dev_tools-0.9.7/ooodev/mock/unohelper.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/office/calc.py` & `ooo_dev_tools-0.9.7/ooodev/office/calc.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/office/chart.py` & `ooo_dev_tools-0.9.7/ooodev/office/chart.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/office/chart2.py` & `ooo_dev_tools-0.9.7/ooodev/office/chart2.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/office/draw.py` & `ooo_dev_tools-0.9.7/ooodev/office/draw.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/office/write.py` & `ooo_dev_tools-0.9.7/ooodev/office/write.py`

 * *Files 0% similar despite different names*

```diff
@@ -644,14 +644,29 @@
         except Exception as e:
             raise Exception("Could not insert document") from e
         _Events().trigger(WriteNamedEvent.DOC_OPENED, EventArgs.from_args(cargs))
         return text_doc
 
     # endregion open_flat_doc_using_text_template()
 
+    @staticmethod
+    def get_doc_settings() -> XPropertySet:
+        """
+        Gets Text Document Settings
+
+        Returns:
+            XPropertySet: Settings
+
+        See Also:
+            `API DocumentSettings Service <https://api.libreoffice.org/docs/idl/ref/servicecom_1_1sun_1_1star_1_1text_1_1DocumentSettings.html>`__
+        
+        .. versionadded:: 0.9.7
+        """
+        return mLo.Lo.create_instance_msf(XPropertySet, "com.sun.star.text.DocumentSettings", raise_err=True)
+
     # endregion ---------- doc / open / close /create/ etc -------------
 
     # region ------------- page methods --------------------------------
     @classmethod
     def get_page_cursor(cls, view_cursor_obj: XTextDocument | XTextViewCursor) -> XPageCursor:
         """
         Get Page cursor
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/proto/dispatch_shape.py` & `ooo_dev_tools-0.9.7/ooodev/proto/dispatch_shape.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/proto/event_observer.py` & `ooo_dev_tools-0.9.7/ooodev/proto/event_observer.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/proto/style_obj.py` & `ooo_dev_tools-0.9.7/ooodev/proto/style_obj.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/theme/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/theme/theme.py` & `ooo_dev_tools-0.9.7/ooodev/theme/theme.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/theme/theme_basic.py` & `ooo_dev_tools-0.9.7/ooodev/theme/theme_basic.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/theme/theme_calc.py` & `ooo_dev_tools-0.9.7/ooodev/theme/theme_calc.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/theme/theme_draw.py` & `ooo_dev_tools-0.9.7/ooodev/theme/theme_draw.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/theme/theme_general.py` & `ooo_dev_tools-0.9.7/ooodev/theme/theme_general.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/theme/theme_html.py` & `ooo_dev_tools-0.9.7/ooodev/theme/theme_html.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/theme/theme_rpt_builder.py` & `ooo_dev_tools-0.9.7/ooodev/theme/theme_rpt_builder.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/theme/theme_sql.py` & `ooo_dev_tools-0.9.7/ooodev/theme/theme_sql.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/theme/theme_text_doc.py` & `ooo_dev_tools-0.9.7/ooodev/theme/theme_text_doc.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/units/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/units/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/units/unit_cm.py` & `ooo_dev_tools-0.9.7/ooodev/units/unit_cm.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/units/unit_convert.py` & `ooo_dev_tools-0.9.7/ooodev/units/unit_convert.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/units/unit_inch.py` & `ooo_dev_tools-0.9.7/ooodev/units/unit_inch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/units/unit_inch10.py` & `ooo_dev_tools-0.9.7/ooodev/units/unit_inch10.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/units/unit_inch100.py` & `ooo_dev_tools-0.9.7/ooodev/units/unit_inch100.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/units/unit_inch1000.py` & `ooo_dev_tools-0.9.7/ooodev/units/unit_inch1000.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/units/unit_mm.py` & `ooo_dev_tools-0.9.7/ooodev/units/unit_mm.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/units/unit_mm10.py` & `ooo_dev_tools-0.9.7/ooodev/units/unit_mm10.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/units/unit_mm100.py` & `ooo_dev_tools-0.9.7/ooodev/units/unit_mm100.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/units/unit_obj.py` & `ooo_dev_tools-0.9.7/ooodev/units/unit_obj.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/units/unit_pt.py` & `ooo_dev_tools-0.9.7/ooodev/units/unit_pt.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/units/unit_px.py` & `ooo_dev_tools-0.9.7/ooodev/units/unit_px.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/__init__.py` & `ooo_dev_tools-0.9.7/ooodev/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/color.py` & `ooo_dev_tools-0.9.7/ooodev/utils/color.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/angle.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/angle.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/base_float_value.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/base_float_value.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/base_int_value.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/base_int_value.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/byte.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/byte.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/byte_signed.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/byte_signed.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/cell_obj.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/cell_obj.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/cell_values.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/cell_values.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/col_obj.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/col_obj.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/color_range.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/color_range.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/image_offset.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/image_offset.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/intensity.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/intensity.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/intensity_range.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/intensity_range.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/poly_sides.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/poly_sides.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/range_obj.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/range_obj.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/range_values.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/range_values.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/row_obj.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/row_obj.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/size.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/size.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/size_mm.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/size_mm.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,22 @@
     """Size Width and Height in ``mm`` units."""
 
     def __init__(self, width: float | UnitObj, height: float | UnitObj) -> None:
         """
         Constructor
 
         Args:
-            width (float, UnitObj, optional): Specifies width in ``mm`` units or :ref:`proto_unit_obj`.
-            height (float, UnitObj, optional): Specifies height in ``mm`` units or :ref:`proto_unit_obj`.
+            width (float, UnitObj): Specifies width in ``mm`` units or :ref:`proto_unit_obj`.
+            height (float, UnitObj): Specifies height in ``mm`` units or :ref:`proto_unit_obj`.
+
+        Returns:
+            None:
         """
-        self.width = round(width, 2)
-        self.height = round(height, 2)
+        self.width = width
+        self.height = height
 
     def get_size_mm100(self) -> Size:
         """
         Gets instance converted to Size in ``1/100th mm`` units.
 
         Returns:
             Size: Size in ``mm`` units.
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/width_height_fraction.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/width_height_fraction.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/data_type/width_height_percent.py` & `ooo_dev_tools-0.9.7/ooodev/utils/data_type/width_height_percent.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/date_time_util.py` & `ooo_dev_tools-0.9.7/ooodev/utils/date_time_util.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/decorator/enforce.py` & `ooo_dev_tools-0.9.7/ooodev/utils/decorator/enforce.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/dialogs.py` & `ooo_dev_tools-0.9.7/ooodev/utils/dialogs.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/dispatch/draw_drawing_dispatch.py` & `ooo_dev_tools-0.9.7/ooodev/utils/dispatch/draw_drawing_dispatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/dispatch/draw_view_dispatch.py` & `ooo_dev_tools-0.9.7/ooodev/utils/dispatch/draw_view_dispatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/dispatch/global_edit_dispatch.py` & `ooo_dev_tools-0.9.7/ooodev/utils/dispatch/global_edit_dispatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/dispatch/global_format_dispatch.py` & `ooo_dev_tools-0.9.7/ooodev/utils/dispatch/global_format_dispatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/dispatch/global_view_dispatch.py` & `ooo_dev_tools-0.9.7/ooodev/utils/dispatch/global_view_dispatch.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/dispatch/shape_dispatch_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/dispatch/shape_dispatch_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/enum_helper.py` & `ooo_dev_tools-0.9.7/ooodev/utils/enum_helper.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/file_io.py` & `ooo_dev_tools-0.9.7/ooodev/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/forms.py` & `ooo_dev_tools-0.9.7/ooodev/utils/forms.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/gallery.py` & `ooo_dev_tools-0.9.7/ooodev/utils/gallery.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/gen_util.py` & `ooo_dev_tools-0.9.7/ooodev/utils/gen_util.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/gui.py` & `ooo_dev_tools-0.9.7/ooodev/utils/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,43 +5,45 @@
 from typing import TYPE_CHECKING, Iterable, overload, Any
 from enum import Enum, IntEnum
 import uno
 
 from com.sun.star.accessibility import XAccessible
 from com.sun.star.accessibility import XAccessibleContext
 from com.sun.star.awt import PosSize  # const
-from com.sun.star.awt import WindowAttribute  # const
 from com.sun.star.awt import VclWindowPeerAttribute  # const
+from com.sun.star.awt import WindowAttribute  # const
 from com.sun.star.awt import XExtendedToolkit
 from com.sun.star.awt import XMenuBar
 from com.sun.star.awt import XMessageBox
 from com.sun.star.awt import XSystemDependentWindowPeer
 from com.sun.star.awt import XToolkit
 from com.sun.star.awt import XTopWindow
 from com.sun.star.awt import XTopWindow2
 from com.sun.star.awt import XUserInputInterception
 from com.sun.star.awt import XWindow
 from com.sun.star.awt import XWindow2
 from com.sun.star.awt import XWindowPeer
 from com.sun.star.beans import XPropertySet
 from com.sun.star.container import XIndexContainer
 from com.sun.star.frame import XDispatchProviderInterception
-from com.sun.star.frame import XLayoutManager
 from com.sun.star.frame import XFrame
 from com.sun.star.frame import XFrame2
 from com.sun.star.frame import XFramesSupplier
+from com.sun.star.frame import XLayoutManager
 from com.sun.star.frame import XModel
 from com.sun.star.lang import SystemDependent  # const
 from com.sun.star.lang import XComponent
-from com.sun.star.view import XControlAccess
-from com.sun.star.view import XSelectionSupplier
 from com.sun.star.ui import UIElementType  # const
 from com.sun.star.ui import XImageManager
-from com.sun.star.ui import XUIConfigurationManagerSupplier
+from com.sun.star.ui import XModuleUIConfigurationManagerSupplier
 from com.sun.star.ui import XUIConfigurationManager
+from com.sun.star.ui import XUIConfigurationManagerSupplier
+from com.sun.star.view import XControlAccess
+from com.sun.star.view import XSelectionSupplier
+
 
 if TYPE_CHECKING:
     from com.sun.star.frame import XController
     from com.sun.star.ui import XUIElement
 
 from ..dialog import input as mInput
 from ..utils import lo as mLo
@@ -1243,20 +1245,20 @@
             Exception: If unable to get XUIConfigurationManager from XUIConfigurationManagerSupplier instance.
 
         Returns:
             XUIConfigurationManager: ui config manager
         """
         doc_type = mInfo.Info.doc_type_service(doc)
 
-        xmodel = mLo.Lo.qi(XModel, doc)
-        if xmodel is None:
-            raise mEx.MissingInterfaceError(XModel)
-        xsupplier = mLo.Lo.qi(XUIConfigurationManagerSupplier, xmodel)
-        if xsupplier is None:
-            raise mEx.MissingInterfaceError(XUIConfigurationManagerSupplier)
+        xsupplier = mLo.Lo.create_instance_mcf(
+            XModuleUIConfigurationManagerSupplier,
+            "com.sun.star.ui.ModuleUIConfigurationManagerSupplier",
+            raise_err=True,
+        )
+
         try:
             return xsupplier.getUIConfigurationManager(str(doc_type))
         except Exception as e:
             raise Exception(f"Could not create a config manager using '{doc_type}'") from e
 
     # region print_ui_cmds()
 
@@ -1342,15 +1344,15 @@
             for i in range(num_settings):
                 # line from java
                 # PropertyValue[] settingProps =  Lo.qi(PropertyValue[].class, settings.getByIndex(i));
                 setting_props = mLo.Lo.qi(XPropertySet, settings.getByIndex(i))
                 val = mProps.Props.get_value(name="CommandURL", props=setting_props)
                 print(f"{i}) {mProps.Props.prop_value_to_string(val)}")
             print()
-        except exception as e:
+        except Exception as e:
             print(e)
 
     @classmethod
     def _print_ui_cmds2(cls, ui_elem_name: str, doc: XComponent) -> None:
         config_man = cls.get_ui_config_manager(doc)
         if config_man is None:
             print("Cannot create configuration manager")
```

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/image_transferable.py` & `ooo_dev_tools-0.9.7/ooodev/utils/image_transferable.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/images.py` & `ooo_dev_tools-0.9.7/ooodev/utils/images.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/images_lo.py` & `ooo_dev_tools-0.9.7/ooodev/utils/images_lo.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/info.py` & `ooo_dev_tools-0.9.7/ooodev/utils/info.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/axis_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/axis_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/chart2_data_role_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/chart2_data_role_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/chart2_types.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/chart2_types.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/chart_diagram_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/chart_diagram_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/curve_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/curve_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/data_point_label_type_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/data_point_label_type_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/data_point_lable_placement_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/data_point_lable_placement_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_bitmap_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_bitmap_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_gradient_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_gradient_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_hatching_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_hatching_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_layer_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_layer_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_name_space_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_name_space_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_shape_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_shape_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/drawing_slide_show_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/drawing_slide_show_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/form_component_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/form_component_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/form_control_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/form_control_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/gallery_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/gallery_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/gallery_search_by_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/gallery_search_by_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/glue_points_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/glue_points_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/graphic_arrow_style_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/graphic_arrow_style_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/graphic_style_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/graphic_style_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/info_paths_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/info_paths_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/kind_helper.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/kind_helper.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/line_style_name_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/line_style_name_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/presentation_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/presentation_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/presentation_layout_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/presentation_layout_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/search_match_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/search_match_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/shape_base_point_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/shape_base_point_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/kind/shape_comb_kind.py` & `ooo_dev_tools-0.9.7/ooodev/utils/kind/shape_comb_kind.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/lo.py` & `ooo_dev_tools-0.9.7/ooodev/utils/lo.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/lo_util.py` & `ooo_dev_tools-0.9.7/ooodev/utils/lo_util.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/paths.py` & `ooo_dev_tools-0.9.7/ooodev/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/props.py` & `ooo_dev_tools-0.9.7/ooodev/utils/props.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/script_context.py` & `ooo_dev_tools-0.9.7/ooodev/utils/script_context.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/selection.py` & `ooo_dev_tools-0.9.7/ooodev/utils/selection.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/session.py` & `ooo_dev_tools-0.9.7/ooodev/utils/session.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/sys_info.py` & `ooo_dev_tools-0.9.7/ooodev/utils/sys_info.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/table_helper.py` & `ooo_dev_tools-0.9.7/ooodev/utils/table_helper.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/text_transferable.py` & `ooo_dev_tools-0.9.7/ooodev/utils/text_transferable.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/type_var.py` & `ooo_dev_tools-0.9.7/ooodev/utils/type_var.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/uno_const.py` & `ooo_dev_tools-0.9.7/ooodev/utils/uno_const.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/uno_enum.py` & `ooo_dev_tools-0.9.7/ooodev/utils/uno_enum.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/validation.py` & `ooo_dev_tools-0.9.7/ooodev/utils/validation.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/view_state.py` & `ooo_dev_tools-0.9.7/ooodev/utils/view_state.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/utils/xml_util.py` & `ooo_dev_tools-0.9.7/ooodev/utils/xml_util.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/ooodev/wrapper/break_context.py` & `ooo_dev_tools-0.9.7/ooodev/wrapper/break_context.py`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/pyproject.toml` & `ooo_dev_tools-0.9.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ooo-dev-tools"
-version = "0.9.6"
+version = "0.9.7"
 description = "LibreOffice Developer Tools"
 license = "Apache Software License"
 readme = "README.rst"
 authors = [
     ":Barry-Thomas-Paul: Moss <bigbytetech@gmail.com>"
 ]
 keywords = ["odev", "libreoffice", "openoffice", "macro", "uno", "ooouno", "pyuno"]
```

### Comparing `ooo_dev_tools-0.9.6/README.rst` & `ooo_dev_tools-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `ooo_dev_tools-0.9.6/PKG-INFO` & `ooo_dev_tools-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooo-dev-tools
-Version: 0.9.6
+Version: 0.9.7
 Summary: LibreOffice Developer Tools
 Home-page: https://github.com/Amourspirit/python_ooo_dev_tools
 License: Apache Software License
 Keywords: odev,libreoffice,openoffice,macro,uno,ooouno,pyuno
 Author: :Barry-Thomas-Paul: Moss
 Author-email: bigbytetech@gmail.com
 Requires-Python: >=3.7,<4.0
```

