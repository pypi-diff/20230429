# Comparing `tmp/openram-1.2.8.tar.gz` & `tmp/openram-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openram-1.2.8.tar", last modified: Fri Mar 31 06:11:42 2023, max compression
+gzip compressed data, was "openram-1.2.9.tar", last modified: Sat Apr 15 02:20:11 2023, max compression
```

## Comparing `openram-1.2.8.tar` & `openram-1.2.9.tar`

### file list

```diff
@@ -1,934 +1,934 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.590113 openram-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-31 06:11:27.000000 openram-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-31 06:11:27.000000 openram-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-03-31 06:11:27.000000 openram-1.2.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-03-31 06:11:42.590113 openram-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-03-31 06:11:27.000000 openram-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 06:11:27.000000 openram-1.2.8/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-31 06:11:27.000000 openram-1.2.8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-31 06:11:27.000000 openram-1.2.8/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.430112 openram-1.2.8/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.434111 openram-1.2.8/compiler/base/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16740 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/channel_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    14016 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/delay_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/design.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/hierarchy_design.py
--rw-r--r--   0 runner    (1001) docker     (123)    94366 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/hierarchy_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    32494 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/hierarchy_spice.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/lef.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/logical_effort.py
--rw-r--r--   0 runner    (1001) docker     (123)    20974 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/pin_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/power_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/timing_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/vector3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/verilog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/wire.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/wire_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/base/wire_spice_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.438112 openram-1.2.8/compiler/characterizer/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/analytical_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/bit_polarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/cacti.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/charutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68113 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/elmore.py
--rw-r--r--   0 runner    (1001) docker     (123)    24348 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    42276 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    25169 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/model_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/regression_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/setup_hold.py
--rw-r--r--   0 runner    (1001) docker     (123)    28548 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/sram_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/stimuli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/characterizer/trim_spice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.438112 openram-1.2.8/compiler/datasheet/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/datasheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/datasheet/add_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.438112 openram-1.2.8/compiler/datasheet/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    17185 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/datasheet/assets/OpenRAM_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/datasheet/assets/datasheet.css
--rw-r--r--   0 runner    (1001) docker     (123)    43292 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/datasheet/assets/vlsi_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/datasheet/datasheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    27250 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/datasheet/datasheet_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/datasheet/table_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.438112 openram-1.2.8/compiler/drc/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/drc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/drc/custom_cell_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/drc/custom_layer_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/drc/design_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/drc/drc_lut.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/drc/drc_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/drc/module_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.438112 openram-1.2.8/compiler/gdsMill/
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.442112 openram-1.2.8/compiler/gdsMill/exampleUserDir/
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/exampleUserDir/arrayDemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/exampleUserDir/fillerDemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.442112 openram-1.2.8/compiler/gdsMill/exampleUserDir/gdsFiles/
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/exampleUserDir/gdsFiles/testLayoutA.gds
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/exampleUserDir/gdsMill.cshrc
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/exampleUserDir/quickStart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.442112 openram-1.2.8/compiler/gdsMill/gdsMill/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/gdsMill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41615 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/gdsMill/gds2reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    25325 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/gdsMill/gds2writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/gdsMill/gdsPrimitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/gdsMill/gdsStreamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/gdsMill/pdfLayout.py
--rw-r--r--   0 runner    (1001) docker     (123)    44476 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/gdsMill/vlsiLayout.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/gdsMill.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.450112 openram-1.2.8/compiler/gdsMill/pyx/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/attr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12332 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    19146 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/bitmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/box.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)    17865 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    22242 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/deco.py
--rw-r--r--   0 runner    (1001) docker     (123)    61971 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/deformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/document.py
--rw-r--r--   0 runner    (1001) docker     (123)    53533 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/dvifile.py
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/epsfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.450112 openram-1.2.8/compiler/gdsMill/pyx/font/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/font/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/font/_t1code.c
--rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/font/afm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/font/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/font/t1code.py
--rw-r--r--   0 runner    (1001) docker     (123)    37471 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/font/t1font.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.450112 openram-1.2.8/compiler/gdsMill/pyx/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.450112 openram-1.2.8/compiler/gdsMill/pyx/graph/axis/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/axis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/axis/axis.py
--rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/axis/painter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/axis/parter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/axis/positioner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/axis/rater.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/axis/texter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/axis/tick.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/axis/timeaxis.py
--rw-r--r--   0 runner    (1001) docker     (123)    23774 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    40360 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/key.py
--rw-r--r--   0 runner    (1001) docker     (123)    92795 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/graph/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.454112 openram-1.2.8/compiler/gdsMill/pyx/lfs/
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/lfs/10pt.lfs
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/lfs/10ptex.lfs
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/lfs/11pt.lfs
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/lfs/11ptex.lfs
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/lfs/12pt.lfs
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/lfs/12ptex.lfs
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/lfs/createlfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/lfs/createlfs.tex
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/lfs/foils17pt.lfs
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/lfs/foils20pt.lfs
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/lfs/foils25pt.lfs
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/lfs/foils30pt.lfs
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/mathutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    80796 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/normpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    45535 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/pdfwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/pswriter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.454112 openram-1.2.8/compiler/gdsMill/pyx/pykpathsea/
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/pykpathsea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/pykpathsea/pykpathsea.c
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/siteconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    60590 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/trafo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/type1font.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/pyx/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.454112 openram-1.2.8/compiler/gdsMill/sram_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/sram_examples/cell6tDemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/sram_examples/fillerDemo.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/sram_examples/gdsMill.sh
--rw-r--r--   0 runner    (1001) docker     (123)   148563 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/sram_examples/layoutB.gds
--rw-r--r--   0 runner    (1001) docker     (123)   148637 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/sram_examples/newcell.gds
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/sram_examples/newcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/sram_examples/printGDS.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/sram_examples/quickStart.py
--rw-r--r--   0 runner    (1001) docker     (123)    83968 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/sram_examples/sram_lib16.gds
--rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/sram_examples/sram_lib2.gds
--rw-r--r--   0 runner    (1001) docker     (123)  1242610 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/gdsMill/sram_examples/sys
--rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.462112 openram-1.2.8/compiler/model_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/shared_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_10b_64w_4wpr_21las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_128b_1024_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_12b_128w_4wpr_38las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_12b_16w_1wpr_1las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_12b_256w_16wpr_186las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_12b_256w_8wpr_17las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_14b_32w_2wpr_23las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_15b_512w_8wpr_85las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_16b_1024w_16wpr_40las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_17b_1024w_16wpr_86las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_17b_256w_16wpr_49las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_18b_128w_2wpr_7las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_18b_32w_1wpr_18las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_21b_1024w_4wpr_54las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_22b_512w_16wpr_249las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_23b_1024w_16wpr_118las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_26b_64w_4wpr_23las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_27b_1024w_4wpr_89las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_27b_256w_8wpr_191las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_27b_512w_4wpr_60las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_32b_1024_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_32b_2048_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_32b_256_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_32b_32w_1wpr_31las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_32b_512_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_4b_16w_1wpr_4las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_4b_32w_2wpr_5las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_4b_64w_4wpr_14las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_5b_256w_16wpr_75las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_64b_1024_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_64b_512_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_6b_16w_1wpr_1las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_7b_256w_4wpr_25las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_7b_64w_2wpr_10las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_8b_1024_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_8b_256_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_8b_256w_1wpr_1las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_8b_512_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_9b_1024w_4wpr_3las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_9b_128w_1wpr_4las_1rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/model_configs/sram_9b_256w_4wpr_15las_1rw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.478112 openram-1.2.8/compiler/modules/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2493 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/and2_dec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/and3_dec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/and4_dec.py
--rw-r--r--   0 runner    (1001) docker     (123)    48455 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/bitcell_1port.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/bitcell_2port.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/bitcell_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/bitcell_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/bitcell_base_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    25131 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/capped_replica_bitcell_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/col_cap_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/col_cap_bitcell_1port.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/col_cap_bitcell_2port.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/column_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/column_mux.py
--rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/column_mux_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/control_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)    22562 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/control_logic_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/delay_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/dff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/dff_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/dff_buf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/dff_buf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/dff_inv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/dff_inv_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/dummy_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/dummy_bitcell_1port.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/dummy_bitcell_2port.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/dummy_pbitcell.py
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/global_bitcell_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    29879 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/hierarchical_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19075 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/hierarchical_predecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/hierarchical_predecode2x4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/hierarchical_predecode3x8.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/hierarchical_predecode4x16.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      446 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/internal_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/inv_dec.py
--rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/local_bitcell_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    35512 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/multibank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/nand2_dec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/nand3_dec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/nand4_dec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/orig_bitcell_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pand2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pand3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pand4.py
--rw-r--r--   0 runner    (1001) docker     (123)    57136 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pbitcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pbuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pbuf_dec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pgate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pinv.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pinv_dec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pinvbuf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pnand2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15690 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pnand3.py
--rw-r--r--   0 runner    (1001) docker     (123)    16410 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pnand4.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pnor2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/port_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    38273 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/port_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/precharge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/precharge_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/ptristate_inv.py
--rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/ptx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/pwrite_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/replica_bitcell_1port.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/replica_bitcell_2port.py
--rw-r--r--   0 runner    (1001) docker     (123)    18232 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/replica_bitcell_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/replica_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/replica_pbitcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/rom_address_control_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/rom_address_control_buf.py
--rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/rom_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/rom_base_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/rom_base_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/rom_column_mux.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/rom_column_mux_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/rom_control_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/rom_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/rom_poly_tap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/rom_precharge_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/rom_precharge_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/rom_wordline_driver_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/row_cap_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/row_cap_bitcell_1port.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/row_cap_bitcell_2port.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/sense_amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/sense_amp_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    63865 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/sram_1bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/sram_multibank.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/sram_multibank_template.v
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/tri_gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/tri_gate_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/wordline_buffer_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/wordline_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/wordline_driver_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/write_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/write_driver_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/modules/write_mask_and_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/rom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/rom_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.482112 openram-1.2.8/compiler/router/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/grid_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/grid_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/grid_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25423 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/pin_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    59690 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/router.py
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/router_tech.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/signal_escape_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/signal_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/signal_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/supply_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/supply_grid_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/router/supply_tree_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/sram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/sram_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/sram_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.526113 openram-1.2.8/compiler/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6605 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/00_code_format_check_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2806 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/01_library_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3928 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/03_contact_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3704 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/03_path_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1234 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/03_ptx_1finger_nmos_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1234 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/03_ptx_1finger_pmos_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1386 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/03_ptx_3finger_nmos_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1386 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/03_ptx_3finger_pmos_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1387 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/03_ptx_4finger_nmos_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1373 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/03_ptx_4finger_pmos_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2062 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/03_ptx_no_contacts_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2212 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/03_wire_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1495 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_and2_dec_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1495 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_and3_dec_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_and4_dec_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_column_mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1518 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_column_mux_pbitcell_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_column_mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1055 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_dff_buf_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1234 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_dummy_pbitcell_1rw1r1w_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_dummy_pbitcell_1rw_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pand2_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pand3_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pand4_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3212 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pbitcell_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1196 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pbuf_dec_8x_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1053 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pbuf_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1657 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pdriver_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1037 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pinv_100x_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pinv_10x_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1053 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pinv_1x_beta_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1038 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pinv_1x_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1038 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pinv_2x_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1178 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pinv_dec_1x_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1046 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pinvbuf_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1267 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pnand2_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1267 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pnand3_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pnand4_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1040 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pnor2_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1449 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_precharge_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1702 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_precharge_pbitcell_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_precharge_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1038 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_pwrite_driver_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1240 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_replica_pbitcell_1rw1r1w_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1240 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_replica_pbitcell_1rw_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1141 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/04_wordline_driver_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1197 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/05_bitcell_array_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1271 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/05_bitcell_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/05_dummy_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1968 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/05_pbitcell_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_column_decoder_16row_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1292 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_132row_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1292 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_132row_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1264 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_16row_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1264 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_16row_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_17row_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_17row_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1273 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_32row_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1273 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_32row_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_4096row_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_4096row_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1270 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_512row_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1270 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_512row_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_64row_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_64row_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2688 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_decoder_pbitcell_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_predecode2x4_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_predecode2x4_pbitcell_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1086 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_predecode2x4_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1278 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_predecode3x8_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_predecode3x8_pbitcell_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1086 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_predecode3x8_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1274 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_hierarchical_predecode4x16_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/06_rom_decoder_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/07_column_mux_array_16mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1072 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/07_column_mux_array_16mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1456 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/07_column_mux_array_2mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/07_column_mux_array_2mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1456 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/07_column_mux_array_4mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/07_column_mux_array_4mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1458 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/07_column_mux_array_8mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/07_column_mux_array_8mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2071 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/07_column_mux_array_pbitcell_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/07_rom_column_mux_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1543 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/08_precharge_array_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/08_precharge_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/08_rom_decoder_buffer_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1088 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/08_rom_precharge_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/08_wordline_buffer_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/08_wordline_driver_array_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/08_wordline_driver_array_pbitcell_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/08_wordline_driver_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/09_sense_amp_array_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1517 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/09_sense_amp_array_pbitcell_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2123 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/09_sense_amp_array_spare_cols_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1503 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/09_sense_amp_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/10_rom_wordline_driver_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1418 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/10_write_driver_array_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/10_write_driver_array_pbitcell_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2116 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/10_write_driver_array_spare_cols_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/10_write_driver_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1571 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/10_write_driver_array_wmask_pbitcell_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/10_write_driver_array_wmask_spare_cols_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1629 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/10_write_driver_array_wmask_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/10_write_mask_and_array_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/10_write_mask_and_array_pbitcell_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/10_write_mask_and_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/11_dff_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1387 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/11_dff_buf_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1333 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/12_tri_gate_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1062 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/13_delay_chain_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_capped_replica_bitcell_array_bothrbl_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1244 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_capped_replica_bitcell_array_leftrbl_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_capped_replica_bitcell_array_leftrbl_1rw_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1203 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_capped_replica_bitcell_array_norbl_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_capped_replica_bitcell_array_norbl_1rw_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1245 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_capped_replica_bitcell_array_rightrbl_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1283 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_replica_bitcell_array_bothrbl_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_replica_bitcell_array_leftrbl_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_replica_bitcell_array_leftrbl_1rw_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1189 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_replica_bitcell_array_norbl_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_replica_bitcell_array_norbl_1rw_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1231 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_replica_bitcell_array_rightrbl_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1695 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_replica_column_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1302 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_replica_column_1rw_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1218 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_replica_pbitcell_1rw1r_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1203 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_replica_pbitcell_1rw_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/14_rom_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1512 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/15_global_bitcell_array_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/15_global_bitcell_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2003 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/15_local_bitcell_array_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1399 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/15_local_bitcell_array_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2019 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/16_control_logic_multiport_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/16_control_logic_r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/16_control_logic_rw_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/16_control_logic_w_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1097 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/16_rom_control_logic_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_address_16rows_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      927 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_address_16rows_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1122 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_address_256rows_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_address_512rows_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_data_16mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1425 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_data_16mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_data_2mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1397 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_data_2mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1329 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_data_4mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_data_4mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1353 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_data_8mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1422 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_data_8mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_data_nomux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1369 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_data_nomux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3211 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_data_spare_cols_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3296 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_data_wmask_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3456 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/18_port_data_wmask_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1889 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_multi_bank_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2098 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_pmulti_bank_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2118 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_psingle_bank_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1375 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_rom_bank_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_16mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1540 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_16mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1997 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_1w_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1364 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_2mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_2mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_4mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_4mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_8mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1537 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_8mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_global_bitline_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_nomux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1484 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_nomux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1875 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_spare_cols_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2009 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_wmask_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/19_single_bank_wmask_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_psram_1bank_2mux_1rw_1w_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2022 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_psram_1bank_2mux_1rw_1w_wmask_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2385 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_psram_1bank_2mux_1w_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1943 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_psram_1bank_2mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_psram_1bank_4mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_16mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2054 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_16mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2232 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_2mux_1rw_1r_spare_cols_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1891 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_2mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2253 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_2mux_1w_1r_spare_cols_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1914 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_2mux_1w_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_2mux_global_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2052 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_2mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_2mux_wmask_spare_cols_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2279 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_2mux_wmask_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2233 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_32b_1024_wmask_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1975 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_4mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_4mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1976 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_8mux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_8mux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2150 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_nomux_1rw_1r_spare_cols_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1893 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_nomux_1rw_1r_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2170 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_nomux_spare_cols_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_nomux_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2519 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_nomux_wmask_sparecols_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2199 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_nomux_wmask_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2091 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_1bank_ring_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3997 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/20_sram_2bank_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4754 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/21_hspice_delay_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2598 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/21_hspice_setuphold_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4099 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/21_model_delay_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4437 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/21_ngspice_delay_extra_rows_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4972 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/21_ngspice_delay_global_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4705 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/21_ngspice_delay_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2561 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/21_ngspice_setuphold_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2750 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/21_regression_delay_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4680 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/21_xyce_delay_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2544 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/21_xyce_setuphold_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2585 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_psram_1bank_2mux_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2779 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_psram_1bank_4mux_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2644 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_psram_1bank_8mux_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2645 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_psram_1bank_nomux_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2408 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_sram_1bank_2mux_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_sram_1bank_2mux_global_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2616 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_sram_1bank_2mux_sparecols_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2409 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_sram_1bank_4mux_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2524 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_sram_1bank_8mux_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_sram_1bank_nomux_1rw_1r_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2398 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_sram_1bank_nomux_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2409 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_sram_1bank_nomux_sparecols_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2418 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_sram_1bank_wmask_1rw_1r_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2601 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/22_sram_wmask_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2682 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/23_lib_sram_linear_regression_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3052 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/23_lib_sram_model_corners_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2612 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/23_lib_sram_model_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2974 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/23_lib_sram_prune_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2813 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/23_lib_sram_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1906 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/24_lef_sram_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2048 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/25_verilog_multibank_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1783 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/25_verilog_sram_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5357 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/26_hspice_pex_pinv_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5684 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/26_ngspice_pex_pinv_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2216 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/26_sram_pex_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3454 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/30_openram_back_end_library_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4384 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/30_openram_back_end_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3178 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/30_openram_front_end_library_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4109 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/30_openram_front_end_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2381 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_1k_1rw1r_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2463 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_1k_1rw_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_1rw1r_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2097 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_1rw1r_phys_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2719 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_1rw_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2382 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_1rw_phys_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2381 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_2k_1rw1r_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2465 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_2k_1rw_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2370 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_4k_1rw1r_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2454 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_4k_1rw_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2381 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_512b_1rw1r_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2464 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_512b_1rw_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2381 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_8k_1rw1r_func_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2465 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/50_riscv_8k_1rw_func_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.530113 openram-1.2.8/compiler/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/configs/config_back_end.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/configs/config_front_end.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/configs/rom_data_64B
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.534113 openram-1.2.8/compiler/tests/golden/
--rw-r--r--   0 runner    (1001) docker     (123)   380535 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45.lef
--rw-r--r--   0 runner    (1001) docker     (123)    24717 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45.sp
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45.v
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45_FF_1p0V_25C_analytical.lib
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45_SS_1p0V_25C_analytical.lib
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45_TT_1p0V_25C.lib
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45_TT_1p0V_25C_analytical.lib
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45_TT_1p0V_25C_pruned.lib
--rw-r--r--   0 runner    (1001) docker     (123)   259340 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm.lef
--rw-r--r--   0 runner    (1001) docker     (123)    24481 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm.sp
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm.v
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm_FF_5p0V_25C_analytical.lib
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm_SS_5p0V_25C_analytical.lib
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm_TT_5p0V_25C.lib
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm_TT_5p0V_25C_analytical.lib
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm_TT_5p0V_25C_pruned.lib
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_2_freepdk45.v
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_2_freepdk45_top.v
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_2_scn4m_subm.v
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/golden/sram_2_16_2_scn4m_subm_top.v
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/sram_1rw_1r_tb.v
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/sram_1rw_tb.v
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/sram_1rw_wmask_tb.v
--rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/tests/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.534113 openram-1.2.8/compiler/verify/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/verify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/verify/assura.py
--rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/verify/calibre.py
--rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/verify/klayout.py
--rw-r--r--   0 runner    (1001) docker     (123)    20854 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/verify/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/verify/none.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-03-31 06:11:27.000000 openram-1.2.8/compiler/verify/run_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.538113 openram-1.2.8/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-03-31 06:11:27.000000 openram-1.2.8/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-31 06:11:27.000000 openram-1.2.8/docker/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-03-31 06:11:27.000000 openram-1.2.8/docker/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-31 06:11:27.000000 openram-1.2.8/docker/mrg.patch
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-31 06:11:27.000000 openram-1.2.8/docker/set-paths.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      888 2023-03-31 06:11:27.000000 openram-1.2.8/install_conda.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.422111 openram-1.2.8/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.538113 openram-1.2.8/macros/rom_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-31 06:11:27.000000 openram-1.2.8/macros/rom_configs/sky130_rom_1kbyte.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-31 06:11:27.000000 openram-1.2.8/macros/rom_configs/sky130_rom_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.542113 openram-1.2.8/macros/sram_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/example_config_1rw_1r_scn4m_subm.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/example_config_1rw_1w_scn4m_subm.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/example_config_1rw_2mux_scn4m_subm.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/example_config_1w_1r_scn4m_subm.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/example_config_2rw_scn4m_subm.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/example_config_big_scn4m_subm.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/example_config_freepdk45.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/example_config_giant_scn4m_subm.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/example_config_medium_scn4m_subm.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/example_config_scn4m_subm.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/freepdk45_sram_1rw1r_32x2048_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/scn4m_subm_sram_16kbyte_1rw1r_32x4096_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/scn4m_subm_sram_1kbyte_1rw1r_32x256_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/scn4m_subm_sram_2kbyte_1rw1r_32x512_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/scn4m_subm_sram_32kbyte_1rw1r_2x32x4096_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/scn4m_subm_sram_4kbyte_1rw1r_32x1024_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/scn4m_subm_sram_8kbyte_1rw1r_32x2048_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/sky130_sram_1kbyte_1r1w_8x1024_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/sky130_sram_1kbyte_1rw1r_32x256_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/sky130_sram_1kbyte_1rw1r_8x1024_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/sky130_sram_1kbyte_1rw_32x256_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/sky130_sram_1rw1r_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/sky130_sram_1rw_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/sky130_sram_2kbyte_1rw1r_32x512_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/sky130_sram_2kbyte_1rw_32x512_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/sky130_sram_4kbyte_1rw1r_32x1024_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/sky130_sram_4kbyte_1rw_32x1024_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/sky130_sram_4kbyte_1rw_64x512_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-31 06:11:27.000000 openram-1.2.8/macros/sram_configs/sky130_sram_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.546113 openram-1.2.8/openram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-03-31 06:11:42.000000 openram-1.2.8/openram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36522 2023-03-31 06:11:42.000000 openram-1.2.8/openram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 06:11:42.000000 openram-1.2.8/openram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 06:11:42.000000 openram-1.2.8/openram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-31 06:11:42.000000 openram-1.2.8/openram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-31 06:11:27.000000 openram-1.2.8/openram.mk
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-31 06:11:27.000000 openram-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 06:11:27.000000 openram-1.2.8/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-03-31 06:11:27.000000 openram-1.2.8/rom_compiler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      285 2023-03-31 06:11:27.000000 openram-1.2.8/setpaths.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 06:11:42.590113 openram-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-03-31 06:11:27.000000 openram-1.2.8/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2223 2023-03-31 06:11:27.000000 openram-1.2.8/sram_compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.426112 openram-1.2.8/technology/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.546113 openram-1.2.8/technology/freepdk45/
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.546113 openram-1.2.8/technology/freepdk45/gds_lib/
--rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/gds_lib/cell_1rw.gds
--rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/gds_lib/cell_2rw.gds
--rw-r--r--   0 runner    (1001) docker     (123)    22182 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/gds_lib/dff.gds
--rw-r--r--   0 runner    (1001) docker     (123)    18510 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/gds_lib/dummy_cell_1rw.gds
--rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/gds_lib/dummy_cell_2rw.gds
--rw-r--r--   0 runner    (1001) docker     (123)    18512 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/gds_lib/replica_cell_1rw.gds
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/gds_lib/replica_cell_2rw.gds
--rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/gds_lib/sense_amp.gds
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/gds_lib/tri_gate.gds
--rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/gds_lib/write_driver.gds
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/layers.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.546113 openram-1.2.8/technology/freepdk45/models/
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/APACHE-LICENSE-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/hspice_ff.include
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/hspice_nom.include
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/hspice_ss.include
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.422111 openram-1.2.8/technology/freepdk45/models/tran_models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.550113 openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/NMOS_THKOX.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/NMOS_VTG.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/NMOS_VTH.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/NMOS_VTL.inc
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/PMOS_THKOX.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/PMOS_VTG.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/PMOS_VTH.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/PMOS_VTL.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.550113 openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/NMOS_THKOX.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/NMOS_VTG.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/NMOS_VTH.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/NMOS_VTL.inc
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/PMOS_THKOX.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/PMOS_VTG.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/PMOS_VTH.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/PMOS_VTL.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.554113 openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/NMOS_THKOX.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/NMOS_VTG.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/NMOS_VTH.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/NMOS_VTL.inc
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/PMOS_THKOX.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/PMOS_VTG.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/PMOS_VTH.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/PMOS_VTL.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.554113 openram-1.2.8/technology/freepdk45/sim_data/
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/sim_data/leakage_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    54213 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/sim_data/sim_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.554113 openram-1.2.8/technology/freepdk45/sp_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/sp_lib/cell_1rw.sp
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/sp_lib/cell_2rw.sp
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/sp_lib/dff.sp
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/sp_lib/dummy_cell_1rw.sp
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/sp_lib/dummy_cell_2rw.sp
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/sp_lib/replica_cell_1rw.sp
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/sp_lib/replica_cell_2rw.sp
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/sp_lib/sense_amp.sp
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/sp_lib/tri_gate.sp
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/sp_lib/write_driver.sp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.558113 openram-1.2.8/technology/freepdk45/tech/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26612 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tech/freepdk45.lydrc
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tech/freepdk45.lylvs
--rw-r--r--   0 runner    (1001) docker     (123)    74031 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tech/freepdk45.lyp
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tech/freepdk45.lyt
--rw-r--r--   0 runner    (1001) docker     (123)    72337 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tech/scn4m_subm.lyp
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tech/scn4m_subm.lyt
--rw-r--r--   0 runner    (1001) docker     (123)    17785 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tech/tech.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.558113 openram-1.2.8/technology/freepdk45/tf/
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tf/APACHE-LICENSE-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    53870 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tf/FreePDK45.tf
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tf/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tf/SVRF_EULA_06Feb09.txt
--rw-r--r--   0 runner    (1001) docker     (123)   235961 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tf/display.drf
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-31 06:11:27.000000 openram-1.2.8/technology/freepdk45/tf/layers.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.558113 openram-1.2.8/technology/scn3me_subm/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.562113 openram-1.2.8/technology/scn3me_subm/gds_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/gds_lib/cell_1rw_1r.gds
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/gds_lib/cell_1w_1r.gds
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/gds_lib/cell_6t.gds
--rw-r--r--   0 runner    (1001) docker     (123)    16622 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/gds_lib/dff.gds
--rw-r--r--   0 runner    (1001) docker     (123)    18934 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/gds_lib/ms_flop.gds
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/gds_lib/replica_cell_1rw_1r.gds
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/gds_lib/replica_cell_1w_1r.gds
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/gds_lib/replica_cell_6t.gds
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/gds_lib/sense_amp.gds
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/gds_lib/tri_gate.gds
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/gds_lib/write_driver.gds
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.566113 openram-1.2.8/technology/scn3me_subm/mag_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/mag_lib/cell_1rw_1r.mag
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/mag_lib/cell_1w_1r.mag
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/mag_lib/cell_6t.mag
--rwxr-xr-x   0 runner    (1001) docker     (123)      453 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/mag_lib/convertall.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/mag_lib/dff.mag
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/mag_lib/ms_flop.mag
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/mag_lib/replica_cell_1rw_1r.mag
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/mag_lib/replica_cell_1w_1r.mag
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/mag_lib/replica_cell_6t.mag
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/mag_lib/sense_amp.mag
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/mag_lib/tri_gate.mag
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/mag_lib/write_driver.mag
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.426112 openram-1.2.8/technology/scn3me_subm/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.566113 openram-1.2.8/technology/scn3me_subm/models/ff/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/models/ff/nmos.sp
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/models/ff/pmos.sp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.566113 openram-1.2.8/technology/scn3me_subm/models/nom/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/models/nom/nmos.sp
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/models/nom/pmos.sp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.566113 openram-1.2.8/technology/scn3me_subm/models/ss/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/models/ss/nmos.sp
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/models/ss/pmos.sp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.570113 openram-1.2.8/technology/scn3me_subm/sp_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/cell_1rw_1r.sp
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/cell_1w_1r.sp
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/cell_6t.sp
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/dff.sp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.570113 openram-1.2.8/technology/scn3me_subm/sp_lib/incorrect/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/incorrect/cell_1rw_1r.sp
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/incorrect/cell_1w_1r.sp
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/incorrect/replica_cell_1rw_1r.sp
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/incorrect/replica_cell_1w_1r.sp
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/ms_flop.sp
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/replica_cell_1rw_1r.sp
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/replica_cell_1w_1r.sp
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/replica_cell_6t.sp
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/sense_amp.sp
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/tri_gate.sp
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sp_lib/write_driver.sp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.570113 openram-1.2.8/technology/scn3me_subm/sue_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sue_lib/cell_6t.sue
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sue_lib/ms_flop.sue
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sue_lib/replica_cell_6t.sue
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sue_lib/sense_amp.sue
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sue_lib/tri_gate.sue
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/sue_lib/write_driver.sue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.574113 openram-1.2.8/technology/scn3me_subm/tech/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/tech/.magicrc
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/tech/README
--rw-r--r--   0 runner    (1001) docker     (123)   111763 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/tech/SCN3ME_SUBM.30.tech
--rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/tech/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4620 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/tech/calibreDRC_scn3me_subm.rul
--rwxr-xr-x   0 runner    (1001) docker     (123)     3100 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/tech/calibreLVS_scn3me_subm.rul
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/tech/setup.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)    11221 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/tech/tech.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.574113 openram-1.2.8/technology/scn3me_subm/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/tf/README
--rw-r--r--   0 runner    (1001) docker     (123)    52482 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/tf/display.drf
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/tf/glade_scn3me_subm.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/tf/layers.map
--rw-r--r--   0 runner    (1001) docker     (123)    41609 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn3me_subm/tf/mosis.tf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.574113 openram-1.2.8/technology/scn4m_subm/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.578113 openram-1.2.8/technology/scn4m_subm/gds_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/gds_lib/cell_1rw.gds
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/gds_lib/cell_2rw.gds
--rw-r--r--   0 runner    (1001) docker     (123)    16622 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/gds_lib/dff.gds
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/gds_lib/dummy_cell_1rw.gds
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/gds_lib/dummy_cell_2rw.gds
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/gds_lib/replica_cell_1rw.gds
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/gds_lib/replica_cell_2rw.gds
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/gds_lib/sense_amp.gds
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/gds_lib/tri_gate.gds
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/gds_lib/write_driver.gds
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.578113 openram-1.2.8/technology/scn4m_subm/mag_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/mag_lib/cell_1rw.mag
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/mag_lib/cell_2rw.mag
--rwxr-xr-x   0 runner    (1001) docker     (123)      269 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/mag_lib/convertall.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/mag_lib/dff.mag
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/mag_lib/dummy_cell_1rw.mag
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/mag_lib/dummy_cell_2rw.mag
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/mag_lib/replica_cell_1rw.mag
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/mag_lib/replica_cell_2rw.mag
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/mag_lib/sense_amp.mag
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/mag_lib/tri_gate.mag
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/mag_lib/write_driver.mag
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.426112 openram-1.2.8/technology/scn4m_subm/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.578113 openram-1.2.8/technology/scn4m_subm/models/ff/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/models/ff/nmos.sp
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/models/ff/pmos.sp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.578113 openram-1.2.8/technology/scn4m_subm/models/nom/
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/models/nom/nmos.sp
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/models/nom/pmos.sp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.578113 openram-1.2.8/technology/scn4m_subm/models/ss/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/models/ss/nmos.sp
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/models/ss/pmos.sp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.578113 openram-1.2.8/technology/scn4m_subm/sim_data/
--rw-r--r--   0 runner    (1001) docker     (123)    60092 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/sim_data/sim_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.582113 openram-1.2.8/technology/scn4m_subm/sp_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/sp_lib/cell_1rw.sp
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/sp_lib/cell_2rw.sp
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/sp_lib/cell_6t.st0
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/sp_lib/dff.sp
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/sp_lib/dummy_cell_1rw.sp
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/sp_lib/dummy_cell_2rw.sp
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/sp_lib/replica_cell_1rw.sp
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/sp_lib/replica_cell_2rw.sp
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/sp_lib/sense_amp.sp
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/sp_lib/tri_gate.sp
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/sp_lib/write_driver.sp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.582113 openram-1.2.8/technology/scn4m_subm/tech/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tech/.magicrc
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tech/README
--rw-r--r--   0 runner    (1001) docker     (123)   126929 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tech/SCN4M_SUBM.20.tech
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38092 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tech/scn4m_subm.lydrc
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tech/scn4m_subm.lylvs
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tech/setup.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tech/tech.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.586114 openram-1.2.8/technology/scn4m_subm/tf/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tf/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)    52861 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tf/display.drf
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tf/glade_scn4m_subm.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tf/layers.map
--rw-r--r--   0 runner    (1001) docker     (123)    73395 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tf/mosis.lyp
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tf/mosis.lyt
--rw-r--r--   0 runner    (1001) docker     (123)    42749 2023-03-31 06:11:27.000000 openram-1.2.8/technology/scn4m_subm/tf/mosis.tf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.586114 openram-1.2.8/technology/setup_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-31 06:11:27.000000 openram-1.2.8/technology/setup_scripts/gen_analytical_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.586114 openram-1.2.8/technology/sky130/
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.590113 openram-1.2.8/technology/sky130/custom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_bitcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_bitcell_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_bitcell_base_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_col_cap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_col_cap_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_corner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_dummy_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_dummy_bitcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_replica_bitcell.py
--rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_replica_bitcell_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_replica_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_row_cap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/custom/sky130_row_cap_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 06:11:42.590113 openram-1.2.8/technology/sky130/tech/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/tech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63904 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/tech/sky130.lydrc
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/tech/sky130.lylvs
--rwxr-xr-x   0 runner    (1001) docker     (123)    32157 2023-03-31 06:11:27.000000 openram-1.2.8/technology/sky130/tech/tech.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.017502 openram-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-15 02:20:03.000000 openram-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-15 02:20:03.000000 openram-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-15 02:20:03.000000 openram-1.2.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-04-15 02:20:11.017502 openram-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-04-15 02:20:03.000000 openram-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 02:20:03.000000 openram-1.2.9/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-15 02:20:03.000000 openram-1.2.9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-15 02:20:03.000000 openram-1.2.9/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.857500 openram-1.2.9/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.865500 openram-1.2.9/compiler/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16740 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/channel_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14016 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/delay_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/hierarchy_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94366 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/hierarchy_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32494 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/hierarchy_spice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/lef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/logical_effort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20974 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/pin_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/power_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/timing_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/vector3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/verilog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/wire.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/wire_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/base/wire_spice_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.869500 openram-1.2.9/compiler/characterizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/analytical_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/bit_polarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/cacti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/charutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68113 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/elmore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24348 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42276 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25169 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/setup_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28548 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/sram_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/stimuli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/characterizer/trim_spice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.869500 openram-1.2.9/compiler/datasheet/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/datasheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/datasheet/add_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.869500 openram-1.2.9/compiler/datasheet/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    17185 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/datasheet/assets/OpenRAM_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/datasheet/assets/datasheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)    43292 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/datasheet/assets/vlsi_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/datasheet/datasheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27250 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/datasheet/datasheet_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/datasheet/table_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.869500 openram-1.2.9/compiler/drc/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/drc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/drc/custom_cell_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/drc/custom_layer_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/drc/design_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/drc/drc_lut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/drc/drc_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/drc/module_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.869500 openram-1.2.9/compiler/gdsMill/
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.869500 openram-1.2.9/compiler/gdsMill/exampleUserDir/
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/exampleUserDir/arrayDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/exampleUserDir/fillerDemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.873500 openram-1.2.9/compiler/gdsMill/exampleUserDir/gdsFiles/
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/exampleUserDir/gdsFiles/testLayoutA.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/exampleUserDir/gdsMill.cshrc
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/exampleUserDir/quickStart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.873500 openram-1.2.9/compiler/gdsMill/gdsMill/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/gdsMill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41615 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/gdsMill/gds2reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25325 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/gdsMill/gds2writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/gdsMill/gdsPrimitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/gdsMill/gdsStreamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/gdsMill/pdfLayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44476 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/gdsMill/vlsiLayout.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/gdsMill.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.877500 openram-1.2.9/compiler/gdsMill/pyx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12332 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19146 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17865 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22242 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/deco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61971 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/deformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53533 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/dvifile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/epsfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.881500 openram-1.2.9/compiler/gdsMill/pyx/font/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/font/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/font/_t1code.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/font/afm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/font/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/font/t1code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37471 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/font/t1font.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.881500 openram-1.2.9/compiler/gdsMill/pyx/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.881500 openram-1.2.9/compiler/gdsMill/pyx/graph/axis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/axis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/axis/axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/axis/painter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/axis/parter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/axis/positioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/axis/rater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/axis/texter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/axis/tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/axis/timeaxis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23774 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40360 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92795 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/graph/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.885500 openram-1.2.9/compiler/gdsMill/pyx/lfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/lfs/10pt.lfs
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/lfs/10ptex.lfs
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/lfs/11pt.lfs
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/lfs/11ptex.lfs
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/lfs/12pt.lfs
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/lfs/12ptex.lfs
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/lfs/createlfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/lfs/createlfs.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/lfs/foils17pt.lfs
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/lfs/foils20pt.lfs
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/lfs/foils25pt.lfs
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/lfs/foils30pt.lfs
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/mathutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80796 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/normpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45535 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/pdfwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/pswriter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.885500 openram-1.2.9/compiler/gdsMill/pyx/pykpathsea/
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/pykpathsea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/pykpathsea/pykpathsea.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/siteconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60590 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/trafo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/type1font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/pyx/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.889500 openram-1.2.9/compiler/gdsMill/sram_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/sram_examples/cell6tDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/sram_examples/fillerDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/sram_examples/gdsMill.sh
+-rw-r--r--   0 runner    (1001) docker     (123)   148563 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/sram_examples/layoutB.gds
+-rw-r--r--   0 runner    (1001) docker     (123)   148637 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/sram_examples/newcell.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/sram_examples/newcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/sram_examples/printGDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/sram_examples/quickStart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83968 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/sram_examples/sram_lib16.gds
+-rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/sram_examples/sram_lib2.gds
+-rw-r--r--   0 runner    (1001) docker     (123)  1242610 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/gdsMill/sram_examples/sys
+-rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.897501 openram-1.2.9/compiler/model_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/shared_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_10b_64w_4wpr_21las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_128b_1024_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_12b_128w_4wpr_38las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_12b_16w_1wpr_1las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_12b_256w_16wpr_186las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_12b_256w_8wpr_17las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_14b_32w_2wpr_23las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_15b_512w_8wpr_85las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_16b_1024w_16wpr_40las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_17b_1024w_16wpr_86las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_17b_256w_16wpr_49las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_18b_128w_2wpr_7las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_18b_32w_1wpr_18las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_21b_1024w_4wpr_54las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_22b_512w_16wpr_249las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_23b_1024w_16wpr_118las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_26b_64w_4wpr_23las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_27b_1024w_4wpr_89las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_27b_256w_8wpr_191las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_27b_512w_4wpr_60las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_32b_1024_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_32b_2048_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_32b_256_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_32b_32w_1wpr_31las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_32b_512_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_4b_16w_1wpr_4las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_4b_32w_2wpr_5las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_4b_64w_4wpr_14las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_5b_256w_16wpr_75las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_64b_1024_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_64b_512_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_6b_16w_1wpr_1las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_7b_256w_4wpr_25las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_7b_64w_2wpr_10las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_8b_1024_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_8b_256_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_8b_256w_1wpr_1las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_8b_512_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_9b_1024w_4wpr_3las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_9b_128w_1wpr_4las_1rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/model_configs/sram_9b_256w_4wpr_15las_1rw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.917501 openram-1.2.9/compiler/modules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2493 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/and2_dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/and3_dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/and4_dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48455 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/bitcell_1port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/bitcell_2port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/bitcell_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/bitcell_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/bitcell_base_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25131 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/capped_replica_bitcell_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/col_cap_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/col_cap_bitcell_1port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/col_cap_bitcell_2port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/column_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/column_mux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/column_mux_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/control_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22562 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/control_logic_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/delay_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/dff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/dff_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/dff_buf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/dff_buf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/dff_inv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/dff_inv_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/dummy_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/dummy_bitcell_1port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/dummy_bitcell_2port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/dummy_pbitcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/global_bitcell_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29879 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/hierarchical_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19075 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/hierarchical_predecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/hierarchical_predecode2x4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/hierarchical_predecode3x8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/hierarchical_predecode4x16.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      446 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/internal_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/inv_dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/local_bitcell_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35512 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/multibank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/nand2_dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/nand3_dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/nand4_dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/orig_bitcell_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pand2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pand3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pand4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57136 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pbitcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pbuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pbuf_dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pinv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pinv_dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pinvbuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pnand2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15690 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pnand3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16410 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pnand4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pnor2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/port_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38273 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/port_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/precharge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/precharge_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/ptristate_inv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/ptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/pwrite_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/replica_bitcell_1port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/replica_bitcell_2port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18232 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/replica_bitcell_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/replica_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/replica_pbitcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/rom_address_control_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/rom_address_control_buf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/rom_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/rom_base_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/rom_base_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/rom_column_mux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/rom_column_mux_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/rom_control_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/rom_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/rom_poly_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/rom_precharge_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/rom_precharge_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/rom_wordline_driver_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/row_cap_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/row_cap_bitcell_1port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/row_cap_bitcell_2port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/sense_amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/sense_amp_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63865 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/sram_1bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/sram_multibank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/sram_multibank_template.v
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/tri_gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/tri_gate_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/wordline_buffer_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/wordline_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/wordline_driver_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/write_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/write_driver_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/modules/write_mask_and_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/rom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/rom_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.921501 openram-1.2.9/compiler/router/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/grid_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/grid_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/grid_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25423 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/pin_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59690 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/router_tech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/signal_escape_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/signal_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/signal_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/supply_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/supply_grid_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/router/supply_tree_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/sram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/sram_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/sram_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.969501 openram-1.2.9/compiler/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6605 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/00_code_format_check_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2806 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/01_library_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3928 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/03_contact_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3704 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/03_path_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1234 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/03_ptx_1finger_nmos_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1234 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/03_ptx_1finger_pmos_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1386 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/03_ptx_3finger_nmos_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1386 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/03_ptx_3finger_pmos_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1387 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/03_ptx_4finger_nmos_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1373 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/03_ptx_4finger_pmos_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2062 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/03_ptx_no_contacts_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2212 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/03_wire_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1495 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_and2_dec_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1495 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_and3_dec_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_and4_dec_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_column_mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1518 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_column_mux_pbitcell_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_column_mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1055 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_dff_buf_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1234 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_dummy_pbitcell_1rw1r1w_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_dummy_pbitcell_1rw_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pand2_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pand3_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pand4_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3212 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pbitcell_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1196 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pbuf_dec_8x_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1053 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pbuf_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1657 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pdriver_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1037 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pinv_100x_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pinv_10x_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1053 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pinv_1x_beta_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1038 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pinv_1x_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1038 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pinv_2x_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1178 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pinv_dec_1x_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1046 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pinvbuf_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1267 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pnand2_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1267 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pnand3_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pnand4_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1040 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pnor2_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1449 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_precharge_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1702 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_precharge_pbitcell_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_precharge_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1038 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_pwrite_driver_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1240 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_replica_pbitcell_1rw1r1w_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1240 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_replica_pbitcell_1rw_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1141 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/04_wordline_driver_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1197 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/05_bitcell_array_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1271 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/05_bitcell_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/05_dummy_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1968 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/05_pbitcell_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_column_decoder_16row_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1292 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_132row_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1292 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_132row_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1264 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_16row_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1264 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_16row_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_17row_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_17row_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1273 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_32row_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1273 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_32row_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_4096row_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_4096row_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1270 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_512row_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1270 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_512row_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_64row_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_64row_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2688 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_decoder_pbitcell_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_predecode2x4_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_predecode2x4_pbitcell_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1086 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_predecode2x4_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1278 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_predecode3x8_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_predecode3x8_pbitcell_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1086 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_predecode3x8_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1274 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_hierarchical_predecode4x16_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/06_rom_decoder_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/07_column_mux_array_16mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1072 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/07_column_mux_array_16mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1456 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/07_column_mux_array_2mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/07_column_mux_array_2mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1456 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/07_column_mux_array_4mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/07_column_mux_array_4mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1458 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/07_column_mux_array_8mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/07_column_mux_array_8mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2071 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/07_column_mux_array_pbitcell_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/07_rom_column_mux_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1543 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/08_precharge_array_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/08_precharge_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/08_rom_decoder_buffer_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1088 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/08_rom_precharge_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/08_wordline_buffer_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/08_wordline_driver_array_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/08_wordline_driver_array_pbitcell_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/08_wordline_driver_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/09_sense_amp_array_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1517 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/09_sense_amp_array_pbitcell_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2123 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/09_sense_amp_array_spare_cols_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1503 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/09_sense_amp_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/10_rom_wordline_driver_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1418 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/10_write_driver_array_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/10_write_driver_array_pbitcell_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2116 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/10_write_driver_array_spare_cols_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/10_write_driver_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1571 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/10_write_driver_array_wmask_pbitcell_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/10_write_driver_array_wmask_spare_cols_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1629 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/10_write_driver_array_wmask_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/10_write_mask_and_array_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/10_write_mask_and_array_pbitcell_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/10_write_mask_and_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/11_dff_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1387 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/11_dff_buf_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1333 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/12_tri_gate_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1062 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/13_delay_chain_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_capped_replica_bitcell_array_bothrbl_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1244 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_capped_replica_bitcell_array_leftrbl_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_capped_replica_bitcell_array_leftrbl_1rw_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1203 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_capped_replica_bitcell_array_norbl_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_capped_replica_bitcell_array_norbl_1rw_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1245 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_capped_replica_bitcell_array_rightrbl_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1283 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_replica_bitcell_array_bothrbl_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_replica_bitcell_array_leftrbl_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_replica_bitcell_array_leftrbl_1rw_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1189 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_replica_bitcell_array_norbl_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_replica_bitcell_array_norbl_1rw_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1231 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_replica_bitcell_array_rightrbl_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1695 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_replica_column_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1302 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_replica_column_1rw_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1218 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_replica_pbitcell_1rw1r_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1203 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_replica_pbitcell_1rw_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/14_rom_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1512 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/15_global_bitcell_array_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/15_global_bitcell_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2003 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/15_local_bitcell_array_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1399 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/15_local_bitcell_array_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2019 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/16_control_logic_multiport_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/16_control_logic_r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/16_control_logic_rw_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/16_control_logic_w_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1097 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/16_rom_control_logic_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_address_16rows_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      927 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_address_16rows_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1122 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_address_256rows_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_address_512rows_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_data_16mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1425 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_data_16mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_data_2mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1397 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_data_2mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1329 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_data_4mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_data_4mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1353 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_data_8mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1422 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_data_8mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_data_nomux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1369 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_data_nomux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3211 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_data_spare_cols_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3296 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_data_wmask_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3456 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/18_port_data_wmask_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1889 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_multi_bank_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2098 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_pmulti_bank_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2118 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_psingle_bank_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1375 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_rom_bank_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_16mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1540 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_16mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1997 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_1w_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1364 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_2mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_2mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_4mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_4mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_8mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1537 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_8mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_global_bitline_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_nomux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1484 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_nomux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1875 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_spare_cols_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2009 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_wmask_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/19_single_bank_wmask_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_psram_1bank_2mux_1rw_1w_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2022 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_psram_1bank_2mux_1rw_1w_wmask_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2385 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_psram_1bank_2mux_1w_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1943 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_psram_1bank_2mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_psram_1bank_4mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_16mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2054 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_16mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2232 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_2mux_1rw_1r_spare_cols_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1891 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_2mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2253 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_2mux_1w_1r_spare_cols_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1914 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_2mux_1w_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_2mux_global_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2052 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_2mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_2mux_wmask_spare_cols_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2279 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_2mux_wmask_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2233 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_32b_1024_wmask_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1975 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_4mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_4mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1976 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_8mux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_8mux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2150 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_nomux_1rw_1r_spare_cols_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1893 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_nomux_1rw_1r_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2170 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_nomux_spare_cols_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2053 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_nomux_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2519 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_nomux_wmask_sparecols_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2199 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_nomux_wmask_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2091 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_1bank_ring_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3997 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/20_sram_2bank_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4754 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/21_hspice_delay_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2598 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/21_hspice_setuphold_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4099 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/21_model_delay_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4437 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/21_ngspice_delay_extra_rows_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4972 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/21_ngspice_delay_global_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4705 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/21_ngspice_delay_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2561 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/21_ngspice_setuphold_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2750 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/21_regression_delay_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4680 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/21_xyce_delay_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2544 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/21_xyce_setuphold_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2585 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_psram_1bank_2mux_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2779 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_psram_1bank_4mux_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2644 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_psram_1bank_8mux_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2645 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_psram_1bank_nomux_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2408 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_sram_1bank_2mux_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_sram_1bank_2mux_global_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2616 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_sram_1bank_2mux_sparecols_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2409 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_sram_1bank_4mux_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2524 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_sram_1bank_8mux_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_sram_1bank_nomux_1rw_1r_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2398 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_sram_1bank_nomux_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2409 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_sram_1bank_nomux_sparecols_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2418 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_sram_1bank_wmask_1rw_1r_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2601 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/22_sram_wmask_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2682 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/23_lib_sram_linear_regression_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3052 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/23_lib_sram_model_corners_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2612 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/23_lib_sram_model_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2974 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/23_lib_sram_prune_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2813 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/23_lib_sram_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1906 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/24_lef_sram_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2048 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/25_verilog_multibank_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1783 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/25_verilog_sram_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5357 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/26_hspice_pex_pinv_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5684 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/26_ngspice_pex_pinv_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2216 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/26_sram_pex_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3454 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/30_openram_back_end_library_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4384 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/30_openram_back_end_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3178 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/30_openram_front_end_library_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4109 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/30_openram_front_end_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2381 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_1k_1rw1r_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2463 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_1k_1rw_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_1rw1r_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2097 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_1rw1r_phys_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2719 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_1rw_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2382 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_1rw_phys_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2381 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_2k_1rw1r_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2465 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_2k_1rw_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2370 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_4k_1rw1r_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2454 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_4k_1rw_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2381 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_512b_1rw1r_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2464 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_512b_1rw_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2381 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_8k_1rw1r_func_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2465 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/50_riscv_8k_1rw_func_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.969501 openram-1.2.9/compiler/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/configs/config_back_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/configs/config_front_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/configs/rom_data_64B
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.973501 openram-1.2.9/compiler/tests/golden/
+-rw-r--r--   0 runner    (1001) docker     (123)   380535 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45.lef
+-rw-r--r--   0 runner    (1001) docker     (123)    24717 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45.sp
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45.v
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45_FF_1p0V_25C_analytical.lib
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45_SS_1p0V_25C_analytical.lib
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45_TT_1p0V_25C.lib
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45_TT_1p0V_25C_analytical.lib
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45_TT_1p0V_25C_pruned.lib
+-rw-r--r--   0 runner    (1001) docker     (123)   259340 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm.lef
+-rw-r--r--   0 runner    (1001) docker     (123)    24481 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm.sp
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm.v
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm_FF_5p0V_25C_analytical.lib
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm_SS_5p0V_25C_analytical.lib
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm_TT_5p0V_25C.lib
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm_TT_5p0V_25C_analytical.lib
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm_TT_5p0V_25C_pruned.lib
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_2_freepdk45.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_2_freepdk45_top.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_2_scn4m_subm.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/golden/sram_2_16_2_scn4m_subm_top.v
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/sram_1rw_1r_tb.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/sram_1rw_tb.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/sram_1rw_wmask_tb.v
+-rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/tests/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.973501 openram-1.2.9/compiler/verify/
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/verify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/verify/assura.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/verify/calibre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/verify/klayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20854 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/verify/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/verify/none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-15 02:20:03.000000 openram-1.2.9/compiler/verify/run_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.973501 openram-1.2.9/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-15 02:20:03.000000 openram-1.2.9/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-15 02:20:03.000000 openram-1.2.9/docker/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-15 02:20:03.000000 openram-1.2.9/docker/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-15 02:20:03.000000 openram-1.2.9/docker/mrg.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-15 02:20:03.000000 openram-1.2.9/docker/set-paths.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      888 2023-04-15 02:20:03.000000 openram-1.2.9/install_conda.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.853500 openram-1.2.9/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.973501 openram-1.2.9/macros/rom_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-15 02:20:03.000000 openram-1.2.9/macros/rom_configs/sky130_rom_1kbyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-15 02:20:03.000000 openram-1.2.9/macros/rom_configs/sky130_rom_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.977501 openram-1.2.9/macros/sram_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/example_config_1rw_1r_scn4m_subm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/example_config_1rw_1w_scn4m_subm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/example_config_1rw_2mux_scn4m_subm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/example_config_1w_1r_scn4m_subm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/example_config_2rw_scn4m_subm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/example_config_big_scn4m_subm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/example_config_freepdk45.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/example_config_giant_scn4m_subm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/example_config_medium_scn4m_subm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/example_config_scn4m_subm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/freepdk45_sram_1rw1r_32x2048_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/scn4m_subm_sram_16kbyte_1rw1r_32x4096_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/scn4m_subm_sram_1kbyte_1rw1r_32x256_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/scn4m_subm_sram_2kbyte_1rw1r_32x512_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/scn4m_subm_sram_32kbyte_1rw1r_2x32x4096_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/scn4m_subm_sram_4kbyte_1rw1r_32x1024_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/scn4m_subm_sram_8kbyte_1rw1r_32x2048_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/sky130_sram_1kbyte_1r1w_8x1024_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/sky130_sram_1kbyte_1rw1r_32x256_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/sky130_sram_1kbyte_1rw1r_8x1024_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/sky130_sram_1kbyte_1rw_32x256_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/sky130_sram_1rw1r_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/sky130_sram_1rw_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/sky130_sram_2kbyte_1rw1r_32x512_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/sky130_sram_2kbyte_1rw_32x512_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/sky130_sram_4kbyte_1rw1r_32x1024_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/sky130_sram_4kbyte_1rw_32x1024_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/sky130_sram_4kbyte_1rw_64x512_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-15 02:20:03.000000 openram-1.2.9/macros/sram_configs/sky130_sram_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.977501 openram-1.2.9/openram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-04-15 02:20:10.000000 openram-1.2.9/openram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36522 2023-04-15 02:20:10.000000 openram-1.2.9/openram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 02:20:10.000000 openram-1.2.9/openram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-15 02:20:10.000000 openram-1.2.9/openram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 02:20:10.000000 openram-1.2.9/openram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-15 02:20:03.000000 openram-1.2.9/openram.mk
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 02:20:03.000000 openram-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-15 02:20:03.000000 openram-1.2.9/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-04-15 02:20:03.000000 openram-1.2.9/rom_compiler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      285 2023-04-15 02:20:03.000000 openram-1.2.9/setpaths.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 02:20:11.017502 openram-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-15 02:20:03.000000 openram-1.2.9/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2223 2023-04-15 02:20:03.000000 openram-1.2.9/sram_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.857500 openram-1.2.9/technology/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.977501 openram-1.2.9/technology/freepdk45/
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.981501 openram-1.2.9/technology/freepdk45/gds_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/gds_lib/cell_1rw.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/gds_lib/cell_2rw.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    22182 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/gds_lib/dff.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    18510 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/gds_lib/dummy_cell_1rw.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/gds_lib/dummy_cell_2rw.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    18512 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/gds_lib/replica_cell_1rw.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/gds_lib/replica_cell_2rw.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/gds_lib/sense_amp.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/gds_lib/tri_gate.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/gds_lib/write_driver.gds
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/layers.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.981501 openram-1.2.9/technology/freepdk45/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/APACHE-LICENSE-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/hspice_ff.include
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/hspice_nom.include
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/hspice_ss.include
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.853500 openram-1.2.9/technology/freepdk45/models/tran_models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.981501 openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/NMOS_THKOX.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/NMOS_VTG.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/NMOS_VTH.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/NMOS_VTL.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/PMOS_THKOX.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/PMOS_VTG.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/PMOS_VTH.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/PMOS_VTL.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.985501 openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/NMOS_THKOX.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/NMOS_VTG.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/NMOS_VTH.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/NMOS_VTL.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/PMOS_THKOX.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/PMOS_VTG.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/PMOS_VTH.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/PMOS_VTL.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.985501 openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/NMOS_THKOX.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/NMOS_VTG.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/NMOS_VTH.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/NMOS_VTL.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/PMOS_THKOX.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/PMOS_VTG.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/PMOS_VTH.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/PMOS_VTL.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.985501 openram-1.2.9/technology/freepdk45/sim_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/sim_data/leakage_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    54213 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/sim_data/sim_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.985501 openram-1.2.9/technology/freepdk45/sp_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/sp_lib/cell_1rw.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/sp_lib/cell_2rw.sp
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/sp_lib/dff.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/sp_lib/dummy_cell_1rw.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/sp_lib/dummy_cell_2rw.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/sp_lib/replica_cell_1rw.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/sp_lib/replica_cell_2rw.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/sp_lib/sense_amp.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/sp_lib/tri_gate.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/sp_lib/write_driver.sp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.989502 openram-1.2.9/technology/freepdk45/tech/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26612 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tech/freepdk45.lydrc
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tech/freepdk45.lylvs
+-rw-r--r--   0 runner    (1001) docker     (123)    74031 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tech/freepdk45.lyp
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tech/freepdk45.lyt
+-rw-r--r--   0 runner    (1001) docker     (123)    72337 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tech/scn4m_subm.lyp
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tech/scn4m_subm.lyt
+-rw-r--r--   0 runner    (1001) docker     (123)    17785 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tech/tech.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.989502 openram-1.2.9/technology/freepdk45/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tf/APACHE-LICENSE-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    53870 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tf/FreePDK45.tf
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tf/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tf/SVRF_EULA_06Feb09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   235961 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tf/display.drf
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-15 02:20:03.000000 openram-1.2.9/technology/freepdk45/tf/layers.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.989502 openram-1.2.9/technology/scn3me_subm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.993502 openram-1.2.9/technology/scn3me_subm/gds_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/gds_lib/cell_1rw_1r.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/gds_lib/cell_1w_1r.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/gds_lib/cell_6t.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    16622 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/gds_lib/dff.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    18934 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/gds_lib/ms_flop.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/gds_lib/replica_cell_1rw_1r.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/gds_lib/replica_cell_1w_1r.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/gds_lib/replica_cell_6t.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/gds_lib/sense_amp.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/gds_lib/tri_gate.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/gds_lib/write_driver.gds
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.993502 openram-1.2.9/technology/scn3me_subm/mag_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/mag_lib/cell_1rw_1r.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/mag_lib/cell_1w_1r.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/mag_lib/cell_6t.mag
+-rwxr-xr-x   0 runner    (1001) docker     (123)      453 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/mag_lib/convertall.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/mag_lib/dff.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/mag_lib/ms_flop.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/mag_lib/replica_cell_1rw_1r.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/mag_lib/replica_cell_1w_1r.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/mag_lib/replica_cell_6t.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/mag_lib/sense_amp.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/mag_lib/tri_gate.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/mag_lib/write_driver.mag
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.853500 openram-1.2.9/technology/scn3me_subm/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.993502 openram-1.2.9/technology/scn3me_subm/models/ff/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/models/ff/nmos.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/models/ff/pmos.sp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.993502 openram-1.2.9/technology/scn3me_subm/models/nom/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/models/nom/nmos.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/models/nom/pmos.sp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.993502 openram-1.2.9/technology/scn3me_subm/models/ss/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/models/ss/nmos.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/models/ss/pmos.sp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.997501 openram-1.2.9/technology/scn3me_subm/sp_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/cell_1rw_1r.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/cell_1w_1r.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/cell_6t.sp
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/dff.sp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.997501 openram-1.2.9/technology/scn3me_subm/sp_lib/incorrect/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/incorrect/cell_1rw_1r.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/incorrect/cell_1w_1r.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/incorrect/replica_cell_1rw_1r.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/incorrect/replica_cell_1w_1r.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/ms_flop.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/replica_cell_1rw_1r.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/replica_cell_1w_1r.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/replica_cell_6t.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/sense_amp.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/tri_gate.sp
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sp_lib/write_driver.sp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.997501 openram-1.2.9/technology/scn3me_subm/sue_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sue_lib/cell_6t.sue
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sue_lib/ms_flop.sue
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sue_lib/replica_cell_6t.sue
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sue_lib/sense_amp.sue
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sue_lib/tri_gate.sue
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/sue_lib/write_driver.sue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.001502 openram-1.2.9/technology/scn3me_subm/tech/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/tech/.magicrc
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/tech/README
+-rw-r--r--   0 runner    (1001) docker     (123)   111763 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/tech/SCN3ME_SUBM.30.tech
+-rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/tech/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4620 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/tech/calibreDRC_scn3me_subm.rul
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3100 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/tech/calibreLVS_scn3me_subm.rul
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/tech/setup.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11221 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/tech/tech.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.001502 openram-1.2.9/technology/scn3me_subm/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/tf/README
+-rw-r--r--   0 runner    (1001) docker     (123)    52482 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/tf/display.drf
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/tf/glade_scn3me_subm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/tf/layers.map
+-rw-r--r--   0 runner    (1001) docker     (123)    41609 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn3me_subm/tf/mosis.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.001502 openram-1.2.9/technology/scn4m_subm/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.005502 openram-1.2.9/technology/scn4m_subm/gds_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/gds_lib/cell_1rw.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/gds_lib/cell_2rw.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    16622 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/gds_lib/dff.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/gds_lib/dummy_cell_1rw.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/gds_lib/dummy_cell_2rw.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/gds_lib/replica_cell_1rw.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/gds_lib/replica_cell_2rw.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/gds_lib/sense_amp.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/gds_lib/tri_gate.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/gds_lib/write_driver.gds
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.005502 openram-1.2.9/technology/scn4m_subm/mag_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/mag_lib/cell_1rw.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/mag_lib/cell_2rw.mag
+-rwxr-xr-x   0 runner    (1001) docker     (123)      269 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/mag_lib/convertall.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/mag_lib/dff.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/mag_lib/dummy_cell_1rw.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/mag_lib/dummy_cell_2rw.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/mag_lib/replica_cell_1rw.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/mag_lib/replica_cell_2rw.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/mag_lib/sense_amp.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/mag_lib/tri_gate.mag
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/mag_lib/write_driver.mag
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:10.853500 openram-1.2.9/technology/scn4m_subm/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.005502 openram-1.2.9/technology/scn4m_subm/models/ff/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/models/ff/nmos.sp
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/models/ff/pmos.sp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.005502 openram-1.2.9/technology/scn4m_subm/models/nom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/models/nom/nmos.sp
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/models/nom/pmos.sp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.005502 openram-1.2.9/technology/scn4m_subm/models/ss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/models/ss/nmos.sp
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/models/ss/pmos.sp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.009502 openram-1.2.9/technology/scn4m_subm/sim_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    60092 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/sim_data/sim_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.009502 openram-1.2.9/technology/scn4m_subm/sp_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/sp_lib/cell_1rw.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/sp_lib/cell_2rw.sp
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/sp_lib/cell_6t.st0
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/sp_lib/dff.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/sp_lib/dummy_cell_1rw.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/sp_lib/dummy_cell_2rw.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/sp_lib/replica_cell_1rw.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/sp_lib/replica_cell_2rw.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/sp_lib/sense_amp.sp
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/sp_lib/tri_gate.sp
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/sp_lib/write_driver.sp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.009502 openram-1.2.9/technology/scn4m_subm/tech/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tech/.magicrc
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tech/README
+-rw-r--r--   0 runner    (1001) docker     (123)   126929 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tech/SCN4M_SUBM.20.tech
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38092 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tech/scn4m_subm.lydrc
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tech/scn4m_subm.lylvs
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tech/setup.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tech/tech.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.013502 openram-1.2.9/technology/scn4m_subm/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tf/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    52861 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tf/display.drf
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tf/glade_scn4m_subm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tf/layers.map
+-rw-r--r--   0 runner    (1001) docker     (123)    73395 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tf/mosis.lyp
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tf/mosis.lyt
+-rw-r--r--   0 runner    (1001) docker     (123)    42749 2023-04-15 02:20:03.000000 openram-1.2.9/technology/scn4m_subm/tf/mosis.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.013502 openram-1.2.9/technology/setup_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 02:20:03.000000 openram-1.2.9/technology/setup_scripts/gen_analytical_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.013502 openram-1.2.9/technology/sky130/
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.017502 openram-1.2.9/technology/sky130/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_bitcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_bitcell_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_bitcell_base_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_col_cap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_col_cap_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_corner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_dummy_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_dummy_bitcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_replica_bitcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_replica_bitcell_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_replica_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_row_cap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/custom/sky130_row_cap_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:20:11.017502 openram-1.2.9/technology/sky130/tech/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/tech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63904 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/tech/sky130.lydrc
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/tech/sky130.lylvs
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32157 2023-04-15 02:20:03.000000 openram-1.2.9/technology/sky130/tech/tech.py
```

### Comparing `openram-1.2.8/LICENSE` & `openram-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/MANIFEST.in` & `openram-1.2.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/Makefile` & `openram-1.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/PKG-INFO` & `openram-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openram
-Version: 1.2.8
+Version: 1.2.9
 Summary: An open-source static random access memory (SRAM) compiler
 Home-page: https://openram.org/
 Download-URL: https://github.com/VLSIDA/OpenRAM/releases
 Author: Matthew Guthaus
 Author-email: mrg+vlsida@ucsc.edu
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/VLSIDA/OpenRAM/issues
@@ -82,15 +82,15 @@
 
 
 
 # Publications
 
 + [M. R. Guthaus, J. E. Stine, S. Ataei, B. Chen, B. Wu, M. Sarwar, "OpenRAM: An Open-Source Memory Compiler," Proceedings of the 35th International Conference on Computer-Aided Design (ICCAD), 2016.](https://escholarship.org/content/qt8x19c778/qt8x19c778_noSplash_b2b3fbbb57f1269f86d0de77865b0691.pdf)
 + [S. Ataei, J. Stine, M. Guthaus, “A 64 kb differential single-port 12T SRAM design with a bit-interleaving scheme for low-voltage operation in 32 nm SOI CMOS,” International Conference on Computer Design (ICCD), 2016, pp. 499-506.](https://escholarship.org/uc/item/99f6q9c9)
-+ [E. Ebrahimi, M. Guthaus, J. Renau, “Timing Speculative SRAM”, IEEE In- ternational Symposium on Circuits and Systems (ISCAS), 2017.](https://escholarship.org/content/qt7nn0j5x3/qt7nn0j5x3_noSplash_172457455e1aceba20694c3d7aa489b4.pdf)
++ [E. Ebrahimi, M. Guthaus, J. Renau, “Timing Speculative SRAM”, IEEE International Symposium on Circuits and Systems (ISCAS), 2017.](https://escholarship.org/content/qt7nn0j5x3/qt7nn0j5x3_noSplash_172457455e1aceba20694c3d7aa489b4.pdf)
 + [B. Wu, J.E. Stine, M.R. Guthaus, "Fast and Area-Efficient Word-Line Optimization",  IEEE International Symposium on Circuits and Systems (ISCAS), 2019.](https://escholarship.org/content/qt98s4c1hp/qt98s4c1hp_noSplash_753dcc3e218f60aafff98ef77fb56384.pdf)
 + [B. Wu, M. Guthaus, "Bottom Up Approach for High Speed SRAM Word-line Buffer Insertion Optimization", IFIP/IEEE International Conference on Very Large Scale Integration (VLSI-SoC), 2019.](https://ieeexplore.ieee.org/document/8920325)
 + [H. Nichols, M. Grimes, J. Sowash, J. Cirimelli-Low, M. Guthaus "Automated Synthesis of Multi-Port Memories and Control", IFIP/IEEE International Conference on Very Large Scale Integration (VLSI-SoC), 2019.](https://escholarship.org/content/qt7047n3k0/qt7047n3k0.pdf?t=q4gcij)
 + [H. Nichols, "Statistical Modeling of SRAMs", M.S. Thesis, UCSC, 2022.](https://escholarship.org/content/qt7vx9n089/qt7vx9n089_noSplash_cfc4ba479d8eb1b6ec25d7c92357bc18.pdf?t=ra9wzr)
 + [M. Guthaus, H. Nichols, J. Cirimelli-Low, J. Kunzler, B. Wu, "Enabling Design Technology Co-Optimization of SRAMs though Open-Source Software", IEEE International Electron Devices Meeting (IEDM), 2020.](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9372047)
```

### Comparing `openram-1.2.8/README.md` & `openram-1.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 
 
 # Publications
 
 + [M. R. Guthaus, J. E. Stine, S. Ataei, B. Chen, B. Wu, M. Sarwar, "OpenRAM: An Open-Source Memory Compiler," Proceedings of the 35th International Conference on Computer-Aided Design (ICCAD), 2016.](https://escholarship.org/content/qt8x19c778/qt8x19c778_noSplash_b2b3fbbb57f1269f86d0de77865b0691.pdf)
 + [S. Ataei, J. Stine, M. Guthaus, “A 64 kb differential single-port 12T SRAM design with a bit-interleaving scheme for low-voltage operation in 32 nm SOI CMOS,” International Conference on Computer Design (ICCD), 2016, pp. 499-506.](https://escholarship.org/uc/item/99f6q9c9)
-+ [E. Ebrahimi, M. Guthaus, J. Renau, “Timing Speculative SRAM”, IEEE In- ternational Symposium on Circuits and Systems (ISCAS), 2017.](https://escholarship.org/content/qt7nn0j5x3/qt7nn0j5x3_noSplash_172457455e1aceba20694c3d7aa489b4.pdf)
++ [E. Ebrahimi, M. Guthaus, J. Renau, “Timing Speculative SRAM”, IEEE International Symposium on Circuits and Systems (ISCAS), 2017.](https://escholarship.org/content/qt7nn0j5x3/qt7nn0j5x3_noSplash_172457455e1aceba20694c3d7aa489b4.pdf)
 + [B. Wu, J.E. Stine, M.R. Guthaus, "Fast and Area-Efficient Word-Line Optimization",  IEEE International Symposium on Circuits and Systems (ISCAS), 2019.](https://escholarship.org/content/qt98s4c1hp/qt98s4c1hp_noSplash_753dcc3e218f60aafff98ef77fb56384.pdf)
 + [B. Wu, M. Guthaus, "Bottom Up Approach for High Speed SRAM Word-line Buffer Insertion Optimization", IFIP/IEEE International Conference on Very Large Scale Integration (VLSI-SoC), 2019.](https://ieeexplore.ieee.org/document/8920325)
 + [H. Nichols, M. Grimes, J. Sowash, J. Cirimelli-Low, M. Guthaus "Automated Synthesis of Multi-Port Memories and Control", IFIP/IEEE International Conference on Very Large Scale Integration (VLSI-SoC), 2019.](https://escholarship.org/content/qt7047n3k0/qt7047n3k0.pdf?t=q4gcij)
 + [H. Nichols, "Statistical Modeling of SRAMs", M.S. Thesis, UCSC, 2022.](https://escholarship.org/content/qt7vx9n089/qt7vx9n089_noSplash_cfc4ba479d8eb1b6ec25d7c92357bc18.pdf?t=ra9wzr)
 + [M. Guthaus, H. Nichols, J. Cirimelli-Low, J. Kunzler, B. Wu, "Enabling Design Technology Co-Optimization of SRAMs though Open-Source Software", IEEE International Electron Devices Meeting (IEDM), 2020.](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9372047)
```

### Comparing `openram-1.2.8/common.py` & `openram-1.2.9/common.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/Makefile` & `openram-1.2.9/compiler/Makefile`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/__init__.py` & `openram-1.2.9/compiler/base/__init__.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/channel_route.py` & `openram-1.2.9/compiler/base/channel_route.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/contact.py` & `openram-1.2.9/compiler/base/contact.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/delay_data.py` & `openram-1.2.9/compiler/base/delay_data.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/design.py` & `openram-1.2.9/compiler/base/design.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/errors.py` & `openram-1.2.9/compiler/base/errors.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/geometry.py` & `openram-1.2.9/compiler/base/geometry.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/hierarchy_design.py` & `openram-1.2.9/compiler/base/hierarchy_design.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/hierarchy_layout.py` & `openram-1.2.9/compiler/base/hierarchy_layout.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/hierarchy_spice.py` & `openram-1.2.9/compiler/base/hierarchy_spice.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/lef.py` & `openram-1.2.9/compiler/base/lef.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/logical_effort.py` & `openram-1.2.9/compiler/base/logical_effort.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/pin_layout.py` & `openram-1.2.9/compiler/base/pin_layout.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/power_data.py` & `openram-1.2.9/compiler/base/power_data.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/route.py` & `openram-1.2.9/compiler/base/route.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/timing_graph.py` & `openram-1.2.9/compiler/base/timing_graph.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/utils.py` & `openram-1.2.9/compiler/base/utils.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/vector.py` & `openram-1.2.9/compiler/base/vector.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/vector3d.py` & `openram-1.2.9/compiler/base/vector3d.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/verilog.py` & `openram-1.2.9/compiler/base/verilog.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/wire.py` & `openram-1.2.9/compiler/base/wire.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/wire_path.py` & `openram-1.2.9/compiler/base/wire_path.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/base/wire_spice_model.py` & `openram-1.2.9/compiler/base/wire_spice_model.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/__init__.py` & `openram-1.2.9/compiler/characterizer/__init__.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/analytical_util.py` & `openram-1.2.9/compiler/characterizer/analytical_util.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/cacti.py` & `openram-1.2.9/compiler/characterizer/cacti.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/charutils.py` & `openram-1.2.9/compiler/characterizer/charutils.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/delay.py` & `openram-1.2.9/compiler/characterizer/delay.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/elmore.py` & `openram-1.2.9/compiler/characterizer/elmore.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/functional.py` & `openram-1.2.9/compiler/characterizer/functional.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/lib.py` & `openram-1.2.9/compiler/characterizer/lib.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/linear_regression.py` & `openram-1.2.9/compiler/characterizer/linear_regression.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/measurements.py` & `openram-1.2.9/compiler/characterizer/measurements.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/model_check.py` & `openram-1.2.9/compiler/characterizer/model_check.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/neural_network.py` & `openram-1.2.9/compiler/characterizer/neural_network.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/regression_model.py` & `openram-1.2.9/compiler/characterizer/regression_model.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/setup_hold.py` & `openram-1.2.9/compiler/characterizer/setup_hold.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/simulation.py` & `openram-1.2.9/compiler/characterizer/simulation.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/stimuli.py` & `openram-1.2.9/compiler/characterizer/stimuli.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/characterizer/trim_spice.py` & `openram-1.2.9/compiler/characterizer/trim_spice.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/datasheet/add_db.py` & `openram-1.2.9/compiler/datasheet/add_db.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/datasheet/assets/OpenRAM_logo.png` & `openram-1.2.9/compiler/datasheet/assets/OpenRAM_logo.png`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/datasheet/assets/vlsi_logo.png` & `openram-1.2.9/compiler/datasheet/assets/vlsi_logo.png`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/datasheet/datasheet.py` & `openram-1.2.9/compiler/datasheet/datasheet.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/datasheet/datasheet_gen.py` & `openram-1.2.9/compiler/datasheet/datasheet_gen.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/datasheet/table_gen.py` & `openram-1.2.9/compiler/datasheet/table_gen.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/debug.py` & `openram-1.2.9/compiler/debug.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/drc/custom_cell_properties.py` & `openram-1.2.9/compiler/drc/custom_cell_properties.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/drc/custom_layer_properties.py` & `openram-1.2.9/compiler/drc/custom_layer_properties.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/drc/design_rules.py` & `openram-1.2.9/compiler/drc/design_rules.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/drc/drc_lut.py` & `openram-1.2.9/compiler/drc/drc_lut.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/drc/module_type.py` & `openram-1.2.9/compiler/drc/module_type.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/README` & `openram-1.2.9/compiler/gdsMill/README`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/exampleUserDir/arrayDemo.py` & `openram-1.2.9/compiler/gdsMill/exampleUserDir/arrayDemo.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/exampleUserDir/fillerDemo.py` & `openram-1.2.9/compiler/gdsMill/exampleUserDir/fillerDemo.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/exampleUserDir/gdsFiles/testLayoutA.gds` & `openram-1.2.9/compiler/gdsMill/exampleUserDir/gdsFiles/testLayoutA.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/exampleUserDir/gdsMill.cshrc` & `openram-1.2.9/compiler/gdsMill/exampleUserDir/gdsMill.cshrc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/exampleUserDir/quickStart.py` & `openram-1.2.9/compiler/gdsMill/exampleUserDir/quickStart.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/gdsMill/gds2reader.py` & `openram-1.2.9/compiler/gdsMill/gdsMill/gds2reader.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/gdsMill/gds2writer.py` & `openram-1.2.9/compiler/gdsMill/gdsMill/gds2writer.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/gdsMill/gdsPrimitives.py` & `openram-1.2.9/compiler/gdsMill/gdsMill/gdsPrimitives.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/gdsMill/gdsStreamer.py` & `openram-1.2.9/compiler/gdsMill/gdsMill/gdsStreamer.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/gdsMill/pdfLayout.py` & `openram-1.2.9/compiler/gdsMill/gdsMill/pdfLayout.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/gdsMill/vlsiLayout.py` & `openram-1.2.9/compiler/gdsMill/gdsMill/vlsiLayout.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/__init__.py` & `openram-1.2.9/compiler/gdsMill/pyx/__init__.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/attr.py` & `openram-1.2.9/compiler/gdsMill/pyx/attr.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/bbox.py` & `openram-1.2.9/compiler/gdsMill/pyx/bbox.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/bitmap.py` & `openram-1.2.9/compiler/gdsMill/pyx/bitmap.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/box.py` & `openram-1.2.9/compiler/gdsMill/pyx/box.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/canvas.py` & `openram-1.2.9/compiler/gdsMill/pyx/canvas.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/color.py` & `openram-1.2.9/compiler/gdsMill/pyx/color.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/config.py` & `openram-1.2.9/compiler/gdsMill/pyx/config.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/connector.py` & `openram-1.2.9/compiler/gdsMill/pyx/connector.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/deco.py` & `openram-1.2.9/compiler/gdsMill/pyx/deco.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/deformer.py` & `openram-1.2.9/compiler/gdsMill/pyx/deformer.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/document.py` & `openram-1.2.9/compiler/gdsMill/pyx/document.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/dvifile.py` & `openram-1.2.9/compiler/gdsMill/pyx/dvifile.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/epsfile.py` & `openram-1.2.9/compiler/gdsMill/pyx/epsfile.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/font/__init__.py` & `openram-1.2.9/compiler/gdsMill/pyx/font/__init__.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/font/_t1code.c` & `openram-1.2.9/compiler/gdsMill/pyx/font/_t1code.c`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/font/afm.py` & `openram-1.2.9/compiler/gdsMill/pyx/font/afm.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/font/encoding.py` & `openram-1.2.9/compiler/gdsMill/pyx/font/encoding.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/font/t1code.py` & `openram-1.2.9/compiler/gdsMill/pyx/font/t1code.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/font/t1font.py` & `openram-1.2.9/compiler/gdsMill/pyx/font/t1font.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/__init__.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/axis/__init__.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/axis/__init__.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/axis/axis.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/axis/axis.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/axis/painter.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/axis/painter.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/axis/parter.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/axis/parter.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/axis/positioner.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/axis/positioner.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/axis/rater.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/axis/rater.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/axis/texter.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/axis/texter.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/axis/tick.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/axis/tick.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/axis/timeaxis.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/axis/timeaxis.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/data.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/data.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/graph.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/graph.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/key.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/key.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/graph/style.py` & `openram-1.2.9/compiler/gdsMill/pyx/graph/style.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/lfs/10pt.lfs` & `openram-1.2.9/compiler/gdsMill/pyx/lfs/10pt.lfs`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/lfs/10ptex.lfs` & `openram-1.2.9/compiler/gdsMill/pyx/lfs/10ptex.lfs`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/lfs/11pt.lfs` & `openram-1.2.9/compiler/gdsMill/pyx/lfs/11pt.lfs`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/lfs/11ptex.lfs` & `openram-1.2.9/compiler/gdsMill/pyx/lfs/11ptex.lfs`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/lfs/12pt.lfs` & `openram-1.2.9/compiler/gdsMill/pyx/lfs/12pt.lfs`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/lfs/12ptex.lfs` & `openram-1.2.9/compiler/gdsMill/pyx/lfs/12ptex.lfs`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/lfs/createlfs.py` & `openram-1.2.9/compiler/gdsMill/pyx/lfs/createlfs.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/lfs/createlfs.tex` & `openram-1.2.9/compiler/gdsMill/pyx/lfs/createlfs.tex`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/lfs/foils17pt.lfs` & `openram-1.2.9/compiler/gdsMill/pyx/lfs/foils17pt.lfs`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/lfs/foils20pt.lfs` & `openram-1.2.9/compiler/gdsMill/pyx/lfs/foils20pt.lfs`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/lfs/foils25pt.lfs` & `openram-1.2.9/compiler/gdsMill/pyx/lfs/foils25pt.lfs`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/lfs/foils30pt.lfs` & `openram-1.2.9/compiler/gdsMill/pyx/lfs/foils30pt.lfs`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/mathutils.py` & `openram-1.2.9/compiler/gdsMill/pyx/mathutils.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/mesh.py` & `openram-1.2.9/compiler/gdsMill/pyx/mesh.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/normpath.py` & `openram-1.2.9/compiler/gdsMill/pyx/normpath.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/path.py` & `openram-1.2.9/compiler/gdsMill/pyx/path.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/pattern.py` & `openram-1.2.9/compiler/gdsMill/pyx/pattern.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/pdfwriter.py` & `openram-1.2.9/compiler/gdsMill/pyx/pdfwriter.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/pswriter.py` & `openram-1.2.9/compiler/gdsMill/pyx/pswriter.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/pykpathsea/__init__.py` & `openram-1.2.9/compiler/gdsMill/pyx/pykpathsea/__init__.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/pykpathsea/pykpathsea.c` & `openram-1.2.9/compiler/gdsMill/pyx/pykpathsea/pykpathsea.c`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/siteconfig.py` & `openram-1.2.9/compiler/gdsMill/pyx/siteconfig.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/style.py` & `openram-1.2.9/compiler/gdsMill/pyx/style.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/text.py` & `openram-1.2.9/compiler/gdsMill/pyx/text.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/trafo.py` & `openram-1.2.9/compiler/gdsMill/pyx/trafo.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/type1font.py` & `openram-1.2.9/compiler/gdsMill/pyx/type1font.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/unit.py` & `openram-1.2.9/compiler/gdsMill/pyx/unit.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/pyx/version.py` & `openram-1.2.9/compiler/gdsMill/pyx/version.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/sram_examples/cell6tDemo.py` & `openram-1.2.9/compiler/gdsMill/sram_examples/cell6tDemo.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/sram_examples/fillerDemo.py` & `openram-1.2.9/compiler/gdsMill/sram_examples/fillerDemo.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/sram_examples/layoutB.gds` & `openram-1.2.9/compiler/gdsMill/sram_examples/layoutB.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/sram_examples/newcell.gds` & `openram-1.2.9/compiler/gdsMill/sram_examples/newcell.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/sram_examples/newcell.py` & `openram-1.2.9/compiler/gdsMill/sram_examples/newcell.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/sram_examples/quickStart.py` & `openram-1.2.9/compiler/gdsMill/sram_examples/quickStart.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/sram_examples/sram_lib16.gds` & `openram-1.2.9/compiler/gdsMill/sram_examples/sram_lib16.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/sram_examples/sram_lib2.gds` & `openram-1.2.9/compiler/gdsMill/sram_examples/sram_lib2.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/gdsMill/sram_examples/sys` & `openram-1.2.9/compiler/gdsMill/sram_examples/sys`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/globals.py` & `openram-1.2.9/compiler/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 from openram import OPENRAM_HOME
 VERSION = open(OPENRAM_HOME + "/../VERSION").read().rstrip()
 NAME = "OpenRAM v{}".format(VERSION)
 USAGE = "sram_compiler.py [options] <config file>\nUse -h for help.\n"
 
 OPTS = options.options()
-CHECKPOINT_OPTS = None
 
 
 def parse_args():
     """ Parse the optional arguments for OpenRAM """
 
     global OPTS
 
@@ -205,36 +204,21 @@
 
     init_paths()
 
     from openram.sram_factory import factory
     factory.reset()
 
     global OPTS
-    global CHECKPOINT_OPTS
-
-    # This is a hack. If we are running a unit test and have checkpointed
-    # the options, load them rather than reading the config file.
-    # This way, the configuration is reloaded at the start of every unit test.
-    # If a unit test fails,
-    # we don't have to worry about restoring the old config values
-    # that may have been tested.
-    if is_unit_test and CHECKPOINT_OPTS:
-        OPTS.__dict__ = CHECKPOINT_OPTS.__dict__.copy()
-        return
 
     # Setup correct bitcell names
     setup_bitcell()
 
     # Import these to find the executables for checkpointing
     from openram import characterizer
     from openram import verify
-    # Make a checkpoint of the options so we can restore
-    # after each unit test
-    if not CHECKPOINT_OPTS:
-        CHECKPOINT_OPTS = copy.copy(OPTS)
 
 
 def install_conda():
     """ Setup conda for default tools. """
 
     # Don't setup conda if not used
     if not OPTS.use_conda or OPTS.is_unit_test:
@@ -577,16 +561,17 @@
     except:
         if OPENRAM_TECH == "":
             debug.warning("Couldn't find a tech directory. "
                           "Install openram library or set $OPENRAM_TECH.")
 
     debug.info(1, "Tech directory found in {}".format(OPENRAM_TECH))
 
-    # Add this environment variable to os.environ
+    # Add this environment variable to os.environ and openram namespace
     os.environ["OPENRAM_TECH"] = OPENRAM_TECH
+    openram.OPENRAM_TECH = OPENRAM_TECH
 
     # Add all of the paths
     for tech_path in OPENRAM_TECH.split(":"):
         debug.check(os.path.isdir(tech_path),
                     "$OPENRAM_TECH does not exist: {0}".format(tech_path))
         sys.path.append(tech_path)
         debug.info(1, "Adding technology path: {}".format(tech_path))
```

### Comparing `openram-1.2.8/compiler/modules/__init__.py` & `openram-1.2.9/compiler/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/and2_dec.py` & `openram-1.2.9/compiler/modules/and2_dec.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/and3_dec.py` & `openram-1.2.9/compiler/modules/and3_dec.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/and4_dec.py` & `openram-1.2.9/compiler/modules/and4_dec.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/bank.py` & `openram-1.2.9/compiler/modules/bank.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/bitcell_1port.py` & `openram-1.2.9/compiler/modules/bitcell_1port.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/bitcell_2port.py` & `openram-1.2.9/compiler/modules/bitcell_2port.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/bitcell_array.py` & `openram-1.2.9/compiler/modules/bitcell_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/bitcell_base.py` & `openram-1.2.9/compiler/modules/bitcell_base.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/bitcell_base_array.py` & `openram-1.2.9/compiler/modules/bitcell_base_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/capped_replica_bitcell_array.py` & `openram-1.2.9/compiler/modules/capped_replica_bitcell_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/col_cap_array.py` & `openram-1.2.9/compiler/modules/col_cap_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/col_cap_bitcell_1port.py` & `openram-1.2.9/compiler/modules/col_cap_bitcell_1port.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/col_cap_bitcell_2port.py` & `openram-1.2.9/compiler/modules/col_cap_bitcell_2port.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/column_decoder.py` & `openram-1.2.9/compiler/modules/column_decoder.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/column_mux.py` & `openram-1.2.9/compiler/modules/column_mux.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/column_mux_array.py` & `openram-1.2.9/compiler/modules/column_mux_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/control_logic.py` & `openram-1.2.9/compiler/modules/control_logic.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/control_logic_base.py` & `openram-1.2.9/compiler/modules/control_logic_base.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/delay_chain.py` & `openram-1.2.9/compiler/modules/delay_chain.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/dff.py` & `openram-1.2.9/compiler/modules/dff.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/dff_array.py` & `openram-1.2.9/compiler/modules/dff_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/dff_buf.py` & `openram-1.2.9/compiler/modules/dff_buf.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/dff_buf_array.py` & `openram-1.2.9/compiler/modules/dff_buf_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/dff_inv.py` & `openram-1.2.9/compiler/modules/dff_inv.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/dff_inv_array.py` & `openram-1.2.9/compiler/modules/dff_inv_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/dummy_array.py` & `openram-1.2.9/compiler/modules/dummy_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/dummy_bitcell_1port.py` & `openram-1.2.9/compiler/modules/dummy_bitcell_1port.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/dummy_bitcell_2port.py` & `openram-1.2.9/compiler/modules/dummy_bitcell_2port.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/dummy_pbitcell.py` & `openram-1.2.9/compiler/modules/dummy_pbitcell.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/global_bitcell_array.py` & `openram-1.2.9/compiler/modules/global_bitcell_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/hierarchical_decoder.py` & `openram-1.2.9/compiler/modules/hierarchical_decoder.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/hierarchical_predecode.py` & `openram-1.2.9/compiler/modules/hierarchical_predecode.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/hierarchical_predecode2x4.py` & `openram-1.2.9/compiler/modules/hierarchical_predecode2x4.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/hierarchical_predecode3x8.py` & `openram-1.2.9/compiler/modules/hierarchical_predecode3x8.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/hierarchical_predecode4x16.py` & `openram-1.2.9/compiler/modules/hierarchical_predecode4x16.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/inv_dec.py` & `openram-1.2.9/compiler/modules/inv_dec.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/local_bitcell_array.py` & `openram-1.2.9/compiler/modules/local_bitcell_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/multibank.py` & `openram-1.2.9/compiler/modules/multibank.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/nand2_dec.py` & `openram-1.2.9/compiler/modules/nand2_dec.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/nand3_dec.py` & `openram-1.2.9/compiler/modules/nand3_dec.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/nand4_dec.py` & `openram-1.2.9/compiler/modules/nand4_dec.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/orig_bitcell_array.py` & `openram-1.2.9/compiler/modules/orig_bitcell_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pand2.py` & `openram-1.2.9/compiler/modules/pand2.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pand3.py` & `openram-1.2.9/compiler/modules/pand3.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pand4.py` & `openram-1.2.9/compiler/modules/pand4.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pbitcell.py` & `openram-1.2.9/compiler/modules/pbitcell.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pbuf.py` & `openram-1.2.9/compiler/modules/pbuf.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pbuf_dec.py` & `openram-1.2.9/compiler/modules/pbuf_dec.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pdriver.py` & `openram-1.2.9/compiler/modules/pdriver.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pgate.py` & `openram-1.2.9/compiler/modules/pgate.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pinv.py` & `openram-1.2.9/compiler/modules/pinv.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pinv_dec.py` & `openram-1.2.9/compiler/modules/pinv_dec.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pinvbuf.py` & `openram-1.2.9/compiler/modules/pinvbuf.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pnand2.py` & `openram-1.2.9/compiler/modules/pnand2.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pnand3.py` & `openram-1.2.9/compiler/modules/pnand3.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pnand4.py` & `openram-1.2.9/compiler/modules/pnand4.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pnor2.py` & `openram-1.2.9/compiler/modules/pnor2.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/port_address.py` & `openram-1.2.9/compiler/modules/port_address.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/port_data.py` & `openram-1.2.9/compiler/modules/port_data.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/precharge.py` & `openram-1.2.9/compiler/modules/precharge.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/precharge_array.py` & `openram-1.2.9/compiler/modules/precharge_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/ptristate_inv.py` & `openram-1.2.9/compiler/modules/ptristate_inv.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/ptx.py` & `openram-1.2.9/compiler/modules/ptx.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/pwrite_driver.py` & `openram-1.2.9/compiler/modules/pwrite_driver.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/replica_bitcell_1port.py` & `openram-1.2.9/compiler/modules/replica_bitcell_1port.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/replica_bitcell_2port.py` & `openram-1.2.9/compiler/modules/replica_bitcell_2port.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/replica_bitcell_array.py` & `openram-1.2.9/compiler/modules/replica_bitcell_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/replica_column.py` & `openram-1.2.9/compiler/modules/replica_column.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/replica_pbitcell.py` & `openram-1.2.9/compiler/modules/replica_pbitcell.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/rom_address_control_array.py` & `openram-1.2.9/compiler/modules/rom_address_control_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/rom_address_control_buf.py` & `openram-1.2.9/compiler/modules/rom_address_control_buf.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/rom_bank.py` & `openram-1.2.9/compiler/modules/rom_bank.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/rom_base_array.py` & `openram-1.2.9/compiler/modules/rom_base_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/rom_base_cell.py` & `openram-1.2.9/compiler/modules/rom_base_cell.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/rom_column_mux.py` & `openram-1.2.9/compiler/modules/rom_column_mux.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/rom_column_mux_array.py` & `openram-1.2.9/compiler/modules/rom_column_mux_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/rom_control_logic.py` & `openram-1.2.9/compiler/modules/rom_control_logic.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/rom_decoder.py` & `openram-1.2.9/compiler/modules/rom_decoder.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/rom_poly_tap.py` & `openram-1.2.9/compiler/modules/rom_poly_tap.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/rom_precharge_array.py` & `openram-1.2.9/compiler/modules/rom_precharge_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/rom_precharge_cell.py` & `openram-1.2.9/compiler/modules/rom_precharge_cell.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/rom_wordline_driver_array.py` & `openram-1.2.9/compiler/modules/rom_wordline_driver_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/row_cap_array.py` & `openram-1.2.9/compiler/modules/row_cap_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/row_cap_bitcell_1port.py` & `openram-1.2.9/compiler/modules/row_cap_bitcell_1port.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/row_cap_bitcell_2port.py` & `openram-1.2.9/compiler/modules/row_cap_bitcell_2port.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/sense_amp.py` & `openram-1.2.9/compiler/modules/sense_amp.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/sense_amp_array.py` & `openram-1.2.9/compiler/modules/sense_amp_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/sram_1bank.py` & `openram-1.2.9/compiler/modules/sram_1bank.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/sram_multibank.py` & `openram-1.2.9/compiler/modules/sram_multibank.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/sram_multibank_template.v` & `openram-1.2.9/compiler/modules/sram_multibank_template.v`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/template.py` & `openram-1.2.9/compiler/modules/template.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/tri_gate.py` & `openram-1.2.9/compiler/modules/tri_gate.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/tri_gate_array.py` & `openram-1.2.9/compiler/modules/tri_gate_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/wordline_buffer_array.py` & `openram-1.2.9/compiler/modules/wordline_buffer_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/wordline_driver.py` & `openram-1.2.9/compiler/modules/wordline_driver.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/wordline_driver_array.py` & `openram-1.2.9/compiler/modules/wordline_driver_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/write_driver.py` & `openram-1.2.9/compiler/modules/write_driver.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/write_driver_array.py` & `openram-1.2.9/compiler/modules/write_driver_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/modules/write_mask_and_array.py` & `openram-1.2.9/compiler/modules/write_mask_and_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/options.py` & `openram-1.2.9/compiler/options.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/rom.py` & `openram-1.2.9/compiler/rom.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/rom_config.py` & `openram-1.2.9/compiler/rom_config.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/direction.py` & `openram-1.2.9/compiler/router/direction.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/grid.py` & `openram-1.2.9/compiler/router/grid.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/grid_cell.py` & `openram-1.2.9/compiler/router/grid_cell.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/grid_path.py` & `openram-1.2.9/compiler/router/grid_path.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/grid_utils.py` & `openram-1.2.9/compiler/router/grid_utils.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/pin_group.py` & `openram-1.2.9/compiler/router/pin_group.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/router.py` & `openram-1.2.9/compiler/router/router.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/router_tech.py` & `openram-1.2.9/compiler/router/router_tech.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/signal_escape_router.py` & `openram-1.2.9/compiler/router/signal_escape_router.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/signal_grid.py` & `openram-1.2.9/compiler/router/signal_grid.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/signal_router.py` & `openram-1.2.9/compiler/router/signal_router.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/supply_grid.py` & `openram-1.2.9/compiler/router/supply_grid.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/supply_grid_router.py` & `openram-1.2.9/compiler/router/supply_grid_router.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/router/supply_tree_router.py` & `openram-1.2.9/compiler/router/supply_tree_router.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/sram.py` & `openram-1.2.9/compiler/sram.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/sram_config.py` & `openram-1.2.9/compiler/sram_config.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/sram_factory.py` & `openram-1.2.9/compiler/sram_factory.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/00_code_format_check_test.py` & `openram-1.2.9/compiler/tests/00_code_format_check_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/01_library_test.py` & `openram-1.2.9/compiler/tests/01_library_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/03_contact_test.py` & `openram-1.2.9/compiler/tests/03_contact_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/03_path_test.py` & `openram-1.2.9/compiler/tests/03_path_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/03_ptx_1finger_nmos_test.py` & `openram-1.2.9/compiler/tests/03_ptx_1finger_nmos_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/03_ptx_1finger_pmos_test.py` & `openram-1.2.9/compiler/tests/03_ptx_1finger_pmos_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/03_ptx_3finger_nmos_test.py` & `openram-1.2.9/compiler/tests/03_ptx_3finger_nmos_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/03_ptx_3finger_pmos_test.py` & `openram-1.2.9/compiler/tests/03_ptx_3finger_pmos_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/03_ptx_4finger_nmos_test.py` & `openram-1.2.9/compiler/tests/03_ptx_4finger_nmos_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/03_ptx_4finger_pmos_test.py` & `openram-1.2.9/compiler/tests/03_ptx_4finger_pmos_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/03_ptx_no_contacts_test.py` & `openram-1.2.9/compiler/tests/03_ptx_no_contacts_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/03_wire_test.py` & `openram-1.2.9/compiler/tests/03_wire_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_and2_dec_test.py` & `openram-1.2.9/compiler/tests/04_and2_dec_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_and3_dec_test.py` & `openram-1.2.9/compiler/tests/04_and3_dec_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_and4_dec_test.py` & `openram-1.2.9/compiler/tests/04_and4_dec_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_column_mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/04_column_mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_column_mux_pbitcell_test.py` & `openram-1.2.9/compiler/tests/04_column_mux_pbitcell_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_column_mux_test.py` & `openram-1.2.9/compiler/tests/04_column_mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_dff_buf_test.py` & `openram-1.2.9/compiler/tests/04_dff_buf_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_dummy_pbitcell_1rw1r1w_test.py` & `openram-1.2.9/compiler/tests/04_dummy_pbitcell_1rw1r1w_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_dummy_pbitcell_1rw_test.py` & `openram-1.2.9/compiler/tests/04_dummy_pbitcell_1rw_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pand2_test.py` & `openram-1.2.9/compiler/tests/04_pand2_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pand3_test.py` & `openram-1.2.9/compiler/tests/04_pand3_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pand4_test.py` & `openram-1.2.9/compiler/tests/04_pand4_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pbitcell_test.py` & `openram-1.2.9/compiler/tests/04_pbitcell_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pbuf_dec_8x_test.py` & `openram-1.2.9/compiler/tests/04_pbuf_dec_8x_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pbuf_test.py` & `openram-1.2.9/compiler/tests/04_pbuf_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pdriver_test.py` & `openram-1.2.9/compiler/tests/04_pdriver_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pinv_100x_test.py` & `openram-1.2.9/compiler/tests/04_pinv_100x_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pinv_10x_test.py` & `openram-1.2.9/compiler/tests/04_pinv_10x_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pinv_1x_beta_test.py` & `openram-1.2.9/compiler/tests/04_pinv_1x_beta_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pinv_1x_test.py` & `openram-1.2.9/compiler/tests/04_pinv_1x_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pinv_2x_test.py` & `openram-1.2.9/compiler/tests/04_pinv_2x_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pinv_dec_1x_test.py` & `openram-1.2.9/compiler/tests/04_pinv_dec_1x_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pinvbuf_test.py` & `openram-1.2.9/compiler/tests/04_pinvbuf_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pnand2_test.py` & `openram-1.2.9/compiler/tests/04_pnand2_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pnand3_test.py` & `openram-1.2.9/compiler/tests/04_pnand3_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pnand4_test.py` & `openram-1.2.9/compiler/tests/04_pnand4_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pnor2_test.py` & `openram-1.2.9/compiler/tests/04_pnor2_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_precharge_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/04_precharge_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_precharge_pbitcell_test.py` & `openram-1.2.9/compiler/tests/04_precharge_pbitcell_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_precharge_test.py` & `openram-1.2.9/compiler/tests/04_precharge_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_pwrite_driver_test.py` & `openram-1.2.9/compiler/tests/04_pwrite_driver_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_replica_pbitcell_1rw1r1w_test.py` & `openram-1.2.9/compiler/tests/04_replica_pbitcell_1rw1r1w_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_replica_pbitcell_1rw_test.py` & `openram-1.2.9/compiler/tests/04_replica_pbitcell_1rw_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/04_wordline_driver_test.py` & `openram-1.2.9/compiler/tests/04_wordline_driver_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/05_bitcell_array_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/05_bitcell_array_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/05_bitcell_array_test.py` & `openram-1.2.9/compiler/tests/05_bitcell_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/05_dummy_array_test.py` & `openram-1.2.9/compiler/tests/05_dummy_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/05_pbitcell_array_test.py` & `openram-1.2.9/compiler/tests/05_pbitcell_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_column_decoder_16row_test.py` & `openram-1.2.9/compiler/tests/06_column_decoder_16row_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_132row_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_132row_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_132row_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_132row_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_16row_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_16row_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_16row_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_16row_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_17row_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_17row_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_17row_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_17row_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_32row_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_32row_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_32row_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_32row_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_4096row_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_4096row_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_4096row_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_4096row_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_512row_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_512row_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_512row_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_512row_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_64row_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_64row_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_64row_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_64row_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_decoder_pbitcell_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_decoder_pbitcell_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_predecode2x4_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_predecode2x4_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_predecode2x4_pbitcell_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_predecode2x4_pbitcell_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_predecode2x4_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_predecode2x4_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_predecode3x8_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_predecode3x8_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_predecode3x8_pbitcell_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_predecode3x8_pbitcell_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_predecode3x8_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_predecode3x8_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_hierarchical_predecode4x16_test.py` & `openram-1.2.9/compiler/tests/06_hierarchical_predecode4x16_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/06_rom_decoder_test.py` & `openram-1.2.9/compiler/tests/06_rom_decoder_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/07_column_mux_array_16mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/07_column_mux_array_16mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/07_column_mux_array_16mux_test.py` & `openram-1.2.9/compiler/tests/07_column_mux_array_16mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/07_column_mux_array_2mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/07_column_mux_array_2mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/07_column_mux_array_2mux_test.py` & `openram-1.2.9/compiler/tests/07_column_mux_array_2mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/07_column_mux_array_4mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/07_column_mux_array_4mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/07_column_mux_array_4mux_test.py` & `openram-1.2.9/compiler/tests/07_column_mux_array_4mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/07_column_mux_array_8mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/07_column_mux_array_8mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/07_column_mux_array_8mux_test.py` & `openram-1.2.9/compiler/tests/07_column_mux_array_8mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/07_column_mux_array_pbitcell_test.py` & `openram-1.2.9/compiler/tests/07_column_mux_array_pbitcell_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/07_rom_column_mux_array_test.py` & `openram-1.2.9/compiler/tests/07_rom_column_mux_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/08_precharge_array_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/08_precharge_array_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/08_precharge_array_test.py` & `openram-1.2.9/compiler/tests/08_precharge_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/08_rom_decoder_buffer_array_test.py` & `openram-1.2.9/compiler/tests/08_rom_decoder_buffer_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/08_rom_precharge_array_test.py` & `openram-1.2.9/compiler/tests/08_rom_precharge_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/08_wordline_buffer_array_test.py` & `openram-1.2.9/compiler/tests/08_wordline_buffer_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/08_wordline_driver_array_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/08_wordline_driver_array_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/08_wordline_driver_array_pbitcell_test.py` & `openram-1.2.9/compiler/tests/08_wordline_driver_array_pbitcell_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/08_wordline_driver_array_test.py` & `openram-1.2.9/compiler/tests/08_wordline_driver_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/09_sense_amp_array_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/09_sense_amp_array_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/09_sense_amp_array_pbitcell_test.py` & `openram-1.2.9/compiler/tests/09_sense_amp_array_pbitcell_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/09_sense_amp_array_spare_cols_test.py` & `openram-1.2.9/compiler/tests/09_sense_amp_array_spare_cols_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/09_sense_amp_array_test.py` & `openram-1.2.9/compiler/tests/09_sense_amp_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/10_rom_wordline_driver_array_test.py` & `openram-1.2.9/compiler/tests/10_rom_wordline_driver_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/10_write_driver_array_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/10_write_driver_array_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/10_write_driver_array_pbitcell_test.py` & `openram-1.2.9/compiler/tests/10_write_driver_array_pbitcell_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/10_write_driver_array_spare_cols_test.py` & `openram-1.2.9/compiler/tests/10_write_driver_array_spare_cols_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/10_write_driver_array_test.py` & `openram-1.2.9/compiler/tests/10_write_driver_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/10_write_driver_array_wmask_pbitcell_test.py` & `openram-1.2.9/compiler/tests/10_write_driver_array_wmask_pbitcell_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/10_write_driver_array_wmask_spare_cols_test.py` & `openram-1.2.9/compiler/tests/10_write_driver_array_wmask_spare_cols_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/10_write_driver_array_wmask_test.py` & `openram-1.2.9/compiler/tests/10_write_driver_array_wmask_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/10_write_mask_and_array_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/10_write_mask_and_array_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/10_write_mask_and_array_pbitcell_test.py` & `openram-1.2.9/compiler/tests/10_write_mask_and_array_pbitcell_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/10_write_mask_and_array_test.py` & `openram-1.2.9/compiler/tests/10_write_mask_and_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/11_dff_array_test.py` & `openram-1.2.9/compiler/tests/11_dff_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/11_dff_buf_array_test.py` & `openram-1.2.9/compiler/tests/11_dff_buf_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/12_tri_gate_array_test.py` & `openram-1.2.9/compiler/tests/12_tri_gate_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/13_delay_chain_test.py` & `openram-1.2.9/compiler/tests/13_delay_chain_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_capped_replica_bitcell_array_bothrbl_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/14_capped_replica_bitcell_array_bothrbl_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_capped_replica_bitcell_array_leftrbl_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/14_capped_replica_bitcell_array_leftrbl_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_capped_replica_bitcell_array_leftrbl_1rw_test.py` & `openram-1.2.9/compiler/tests/14_capped_replica_bitcell_array_leftrbl_1rw_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_capped_replica_bitcell_array_norbl_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/14_capped_replica_bitcell_array_norbl_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_capped_replica_bitcell_array_norbl_1rw_test.py` & `openram-1.2.9/compiler/tests/14_capped_replica_bitcell_array_norbl_1rw_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_capped_replica_bitcell_array_rightrbl_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/14_capped_replica_bitcell_array_rightrbl_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_replica_bitcell_array_bothrbl_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/14_replica_bitcell_array_bothrbl_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_replica_bitcell_array_leftrbl_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/14_replica_bitcell_array_leftrbl_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_replica_bitcell_array_leftrbl_1rw_test.py` & `openram-1.2.9/compiler/tests/14_replica_bitcell_array_leftrbl_1rw_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_replica_bitcell_array_norbl_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/14_replica_bitcell_array_norbl_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_replica_bitcell_array_norbl_1rw_test.py` & `openram-1.2.9/compiler/tests/14_replica_bitcell_array_norbl_1rw_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_replica_bitcell_array_rightrbl_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/14_replica_bitcell_array_rightrbl_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_replica_column_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/14_replica_column_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_replica_column_1rw_test.py` & `openram-1.2.9/compiler/tests/14_replica_column_1rw_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_replica_pbitcell_1rw1r_array_test.py` & `openram-1.2.9/compiler/tests/14_replica_pbitcell_1rw1r_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_replica_pbitcell_1rw_array_test.py` & `openram-1.2.9/compiler/tests/14_replica_pbitcell_1rw_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/14_rom_array_test.py` & `openram-1.2.9/compiler/tests/14_rom_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/15_global_bitcell_array_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/15_global_bitcell_array_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/15_global_bitcell_array_test.py` & `openram-1.2.9/compiler/tests/15_global_bitcell_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/15_local_bitcell_array_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/15_local_bitcell_array_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/15_local_bitcell_array_test.py` & `openram-1.2.9/compiler/tests/15_local_bitcell_array_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/16_control_logic_multiport_test.py` & `openram-1.2.9/compiler/tests/16_control_logic_multiport_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/16_control_logic_r_test.py` & `openram-1.2.9/compiler/tests/16_control_logic_r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/16_control_logic_rw_test.py` & `openram-1.2.9/compiler/tests/16_control_logic_rw_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/16_control_logic_w_test.py` & `openram-1.2.9/compiler/tests/16_control_logic_w_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/16_rom_control_logic_test.py` & `openram-1.2.9/compiler/tests/16_rom_control_logic_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_address_16rows_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/18_port_address_16rows_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_address_16rows_test.py` & `openram-1.2.9/compiler/tests/18_port_address_16rows_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_address_256rows_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/18_port_address_256rows_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_address_512rows_test.py` & `openram-1.2.9/compiler/tests/18_port_address_512rows_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_data_16mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/18_port_data_16mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_data_16mux_test.py` & `openram-1.2.9/compiler/tests/18_port_data_16mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_data_2mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/18_port_data_2mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_data_2mux_test.py` & `openram-1.2.9/compiler/tests/18_port_data_2mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_data_4mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/18_port_data_4mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_data_4mux_test.py` & `openram-1.2.9/compiler/tests/18_port_data_4mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_data_8mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/18_port_data_8mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_data_8mux_test.py` & `openram-1.2.9/compiler/tests/18_port_data_8mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_data_nomux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/18_port_data_nomux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_data_nomux_test.py` & `openram-1.2.9/compiler/tests/18_port_data_nomux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_data_spare_cols_test.py` & `openram-1.2.9/compiler/tests/18_port_data_spare_cols_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_data_wmask_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/18_port_data_wmask_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/18_port_data_wmask_test.py` & `openram-1.2.9/compiler/tests/18_port_data_wmask_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_multi_bank_test.py` & `openram-1.2.9/compiler/tests/19_multi_bank_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_pmulti_bank_test.py` & `openram-1.2.9/compiler/tests/19_pmulti_bank_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_psingle_bank_test.py` & `openram-1.2.9/compiler/tests/19_psingle_bank_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_rom_bank_test.py` & `openram-1.2.9/compiler/tests/19_rom_bank_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_16mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_16mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_16mux_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_16mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_1w_1r_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_1w_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_2mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_2mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_2mux_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_2mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_4mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_4mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_4mux_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_4mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_8mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_8mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_8mux_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_8mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_global_bitline_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_global_bitline_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_nomux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_nomux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_nomux_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_nomux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_spare_cols_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_spare_cols_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_wmask_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_wmask_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/19_single_bank_wmask_test.py` & `openram-1.2.9/compiler/tests/19_single_bank_wmask_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_psram_1bank_2mux_1rw_1w_test.py` & `openram-1.2.9/compiler/tests/20_psram_1bank_2mux_1rw_1w_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_psram_1bank_2mux_1rw_1w_wmask_test.py` & `openram-1.2.9/compiler/tests/20_psram_1bank_2mux_1rw_1w_wmask_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_psram_1bank_2mux_1w_1r_test.py` & `openram-1.2.9/compiler/tests/20_psram_1bank_2mux_1w_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_psram_1bank_2mux_test.py` & `openram-1.2.9/compiler/tests/20_psram_1bank_2mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_psram_1bank_4mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/20_psram_1bank_4mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_16mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_16mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_16mux_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_16mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_2mux_1rw_1r_spare_cols_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_2mux_1rw_1r_spare_cols_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_2mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_2mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_2mux_1w_1r_spare_cols_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_2mux_1w_1r_spare_cols_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_2mux_1w_1r_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_2mux_1w_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_2mux_global_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_2mux_global_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_2mux_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_2mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_2mux_wmask_spare_cols_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_2mux_wmask_spare_cols_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_2mux_wmask_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_2mux_wmask_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_32b_1024_wmask_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_32b_1024_wmask_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_4mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_4mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_4mux_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_4mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_8mux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_8mux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_8mux_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_8mux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_nomux_1rw_1r_spare_cols_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_nomux_1rw_1r_spare_cols_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_nomux_1rw_1r_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_nomux_1rw_1r_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_nomux_spare_cols_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_nomux_spare_cols_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_nomux_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_nomux_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_nomux_wmask_sparecols_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_nomux_wmask_sparecols_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_nomux_wmask_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_nomux_wmask_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_1bank_ring_test.py` & `openram-1.2.9/compiler/tests/20_sram_1bank_ring_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/20_sram_2bank_test.py` & `openram-1.2.9/compiler/tests/20_sram_2bank_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/21_hspice_delay_test.py` & `openram-1.2.9/compiler/tests/21_hspice_delay_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/21_hspice_setuphold_test.py` & `openram-1.2.9/compiler/tests/21_hspice_setuphold_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/21_model_delay_test.py` & `openram-1.2.9/compiler/tests/21_model_delay_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/21_ngspice_delay_extra_rows_test.py` & `openram-1.2.9/compiler/tests/21_ngspice_delay_extra_rows_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/21_ngspice_delay_global_test.py` & `openram-1.2.9/compiler/tests/21_ngspice_delay_global_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/21_ngspice_delay_test.py` & `openram-1.2.9/compiler/tests/21_ngspice_delay_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/21_ngspice_setuphold_test.py` & `openram-1.2.9/compiler/tests/21_ngspice_setuphold_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/21_regression_delay_test.py` & `openram-1.2.9/compiler/tests/21_regression_delay_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/21_xyce_delay_test.py` & `openram-1.2.9/compiler/tests/21_xyce_delay_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/21_xyce_setuphold_test.py` & `openram-1.2.9/compiler/tests/21_xyce_setuphold_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_psram_1bank_2mux_func_test.py` & `openram-1.2.9/compiler/tests/22_psram_1bank_2mux_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_psram_1bank_4mux_func_test.py` & `openram-1.2.9/compiler/tests/22_psram_1bank_4mux_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_psram_1bank_8mux_func_test.py` & `openram-1.2.9/compiler/tests/22_psram_1bank_8mux_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_psram_1bank_nomux_func_test.py` & `openram-1.2.9/compiler/tests/22_psram_1bank_nomux_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_sram_1bank_2mux_func_test.py` & `openram-1.2.9/compiler/tests/22_sram_1bank_2mux_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_sram_1bank_2mux_global_func_test.py` & `openram-1.2.9/compiler/tests/22_sram_1bank_2mux_global_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_sram_1bank_2mux_sparecols_func_test.py` & `openram-1.2.9/compiler/tests/22_sram_1bank_2mux_sparecols_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_sram_1bank_4mux_func_test.py` & `openram-1.2.9/compiler/tests/22_sram_1bank_4mux_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_sram_1bank_8mux_func_test.py` & `openram-1.2.9/compiler/tests/22_sram_1bank_8mux_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_sram_1bank_nomux_1rw_1r_func_test.py` & `openram-1.2.9/compiler/tests/22_sram_1bank_nomux_1rw_1r_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_sram_1bank_nomux_func_test.py` & `openram-1.2.9/compiler/tests/22_sram_1bank_nomux_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_sram_1bank_nomux_sparecols_func_test.py` & `openram-1.2.9/compiler/tests/22_sram_1bank_nomux_sparecols_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_sram_1bank_wmask_1rw_1r_func_test.py` & `openram-1.2.9/compiler/tests/22_sram_1bank_wmask_1rw_1r_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/22_sram_wmask_func_test.py` & `openram-1.2.9/compiler/tests/22_sram_wmask_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/23_lib_sram_linear_regression_test.py` & `openram-1.2.9/compiler/tests/23_lib_sram_linear_regression_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/23_lib_sram_model_corners_test.py` & `openram-1.2.9/compiler/tests/23_lib_sram_model_corners_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/23_lib_sram_model_test.py` & `openram-1.2.9/compiler/tests/23_lib_sram_model_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/23_lib_sram_prune_test.py` & `openram-1.2.9/compiler/tests/23_lib_sram_prune_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/23_lib_sram_test.py` & `openram-1.2.9/compiler/tests/23_lib_sram_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/24_lef_sram_test.py` & `openram-1.2.9/compiler/tests/24_lef_sram_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/25_verilog_multibank_test.py` & `openram-1.2.9/compiler/tests/25_verilog_multibank_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/25_verilog_sram_test.py` & `openram-1.2.9/compiler/tests/25_verilog_sram_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/26_hspice_pex_pinv_test.py` & `openram-1.2.9/compiler/tests/26_hspice_pex_pinv_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/26_ngspice_pex_pinv_test.py` & `openram-1.2.9/compiler/tests/26_ngspice_pex_pinv_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/26_sram_pex_test.py` & `openram-1.2.9/compiler/tests/26_sram_pex_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/30_openram_back_end_library_test.py` & `openram-1.2.9/compiler/tests/30_openram_back_end_library_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/30_openram_back_end_test.py` & `openram-1.2.9/compiler/tests/30_openram_back_end_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/30_openram_front_end_library_test.py` & `openram-1.2.9/compiler/tests/30_openram_front_end_library_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/30_openram_front_end_test.py` & `openram-1.2.9/compiler/tests/30_openram_front_end_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_1k_1rw1r_func_test.py` & `openram-1.2.9/compiler/tests/50_riscv_1k_1rw1r_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_1k_1rw_func_test.py` & `openram-1.2.9/compiler/tests/50_riscv_1k_1rw_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_1rw1r_func_test.py` & `openram-1.2.9/compiler/tests/50_riscv_1rw1r_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_1rw1r_phys_test.py` & `openram-1.2.9/compiler/tests/50_riscv_1rw1r_phys_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_1rw_func_test.py` & `openram-1.2.9/compiler/tests/50_riscv_1rw_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_1rw_phys_test.py` & `openram-1.2.9/compiler/tests/50_riscv_1rw_phys_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_2k_1rw1r_func_test.py` & `openram-1.2.9/compiler/tests/50_riscv_2k_1rw1r_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_2k_1rw_func_test.py` & `openram-1.2.9/compiler/tests/50_riscv_2k_1rw_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_4k_1rw1r_func_test.py` & `openram-1.2.9/compiler/tests/50_riscv_4k_1rw1r_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_4k_1rw_func_test.py` & `openram-1.2.9/compiler/tests/50_riscv_4k_1rw_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_512b_1rw1r_func_test.py` & `openram-1.2.9/compiler/tests/50_riscv_512b_1rw1r_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_512b_1rw_func_test.py` & `openram-1.2.9/compiler/tests/50_riscv_512b_1rw_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_8k_1rw1r_func_test.py` & `openram-1.2.9/compiler/tests/50_riscv_8k_1rw1r_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/50_riscv_8k_1rw_func_test.py` & `openram-1.2.9/compiler/tests/50_riscv_8k_1rw_func_test.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/Makefile` & `openram-1.2.9/compiler/tests/Makefile`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45.lef` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45.lef`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45.sp` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45.v` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45.v`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45_FF_1p0V_25C_analytical.lib` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45_FF_1p0V_25C_analytical.lib`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45_SS_1p0V_25C_analytical.lib` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45_SS_1p0V_25C_analytical.lib`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45_TT_1p0V_25C.lib` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45_TT_1p0V_25C.lib`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45_TT_1p0V_25C_analytical.lib` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45_TT_1p0V_25C_analytical.lib`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_freepdk45_TT_1p0V_25C_pruned.lib` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_freepdk45_TT_1p0V_25C_pruned.lib`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm.lef` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm.lef`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm.sp` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm.v` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm.v`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm_FF_5p0V_25C_analytical.lib` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm_FF_5p0V_25C_analytical.lib`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm_SS_5p0V_25C_analytical.lib` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm_SS_5p0V_25C_analytical.lib`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm_TT_5p0V_25C.lib` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm_TT_5p0V_25C.lib`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm_TT_5p0V_25C_analytical.lib` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm_TT_5p0V_25C_analytical.lib`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_1_scn4m_subm_TT_5p0V_25C_pruned.lib` & `openram-1.2.9/compiler/tests/golden/sram_2_16_1_scn4m_subm_TT_5p0V_25C_pruned.lib`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_2_freepdk45.v` & `openram-1.2.9/compiler/tests/golden/sram_2_16_2_freepdk45.v`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_2_freepdk45_top.v` & `openram-1.2.9/compiler/tests/golden/sram_2_16_2_freepdk45_top.v`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_2_scn4m_subm.v` & `openram-1.2.9/compiler/tests/golden/sram_2_16_2_scn4m_subm.v`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/golden/sram_2_16_2_scn4m_subm_top.v` & `openram-1.2.9/compiler/tests/golden/sram_2_16_2_scn4m_subm_top.v`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/sram_1rw_1r_tb.v` & `openram-1.2.9/compiler/tests/sram_1rw_1r_tb.v`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/sram_1rw_tb.v` & `openram-1.2.9/compiler/tests/sram_1rw_tb.v`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/sram_1rw_wmask_tb.v` & `openram-1.2.9/compiler/tests/sram_1rw_wmask_tb.v`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/tests/testutils.py` & `openram-1.2.9/compiler/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/verify/__init__.py` & `openram-1.2.9/compiler/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/verify/assura.py` & `openram-1.2.9/compiler/verify/assura.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/verify/calibre.py` & `openram-1.2.9/compiler/verify/calibre.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/verify/klayout.py` & `openram-1.2.9/compiler/verify/klayout.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/verify/magic.py` & `openram-1.2.9/compiler/verify/magic.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/verify/none.py` & `openram-1.2.9/compiler/verify/none.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/compiler/verify/run_script.py` & `openram-1.2.9/compiler/verify/run_script.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/docker/Dockerfile` & `openram-1.2.9/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/docker/README.md` & `openram-1.2.9/docker/README.md`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/docker/mrg.patch` & `openram-1.2.9/docker/mrg.patch`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/install_conda.sh` & `openram-1.2.9/install_conda.sh`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/rom_configs/sky130_rom_1kbyte.py` & `openram-1.2.9/macros/rom_configs/sky130_rom_1kbyte.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/example_config_1rw_1r_scn4m_subm.py` & `openram-1.2.9/macros/sram_configs/example_config_1rw_1r_scn4m_subm.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/example_config_1rw_1w_scn4m_subm.py` & `openram-1.2.9/macros/sram_configs/example_config_1rw_1w_scn4m_subm.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/example_config_1rw_2mux_scn4m_subm.py` & `openram-1.2.9/macros/sram_configs/example_config_1rw_2mux_scn4m_subm.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/example_config_1w_1r_scn4m_subm.py` & `openram-1.2.9/macros/sram_configs/example_config_1w_1r_scn4m_subm.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/example_config_2rw_scn4m_subm.py` & `openram-1.2.9/macros/sram_configs/example_config_2rw_scn4m_subm.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/example_config_big_scn4m_subm.py` & `openram-1.2.9/macros/sram_configs/example_config_big_scn4m_subm.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/example_config_freepdk45.py` & `openram-1.2.9/macros/sram_configs/example_config_freepdk45.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/example_config_giant_scn4m_subm.py` & `openram-1.2.9/macros/sram_configs/example_config_giant_scn4m_subm.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/example_config_medium_scn4m_subm.py` & `openram-1.2.9/macros/sram_configs/example_config_medium_scn4m_subm.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/example_config_scn4m_subm.py` & `openram-1.2.9/macros/sram_configs/example_config_scn4m_subm.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/freepdk45_sram_1rw1r_32x2048_8.py` & `openram-1.2.9/macros/sram_configs/freepdk45_sram_1rw1r_32x2048_8.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/scn4m_subm_sram_16kbyte_1rw1r_32x4096_8.py` & `openram-1.2.9/macros/sram_configs/scn4m_subm_sram_16kbyte_1rw1r_32x4096_8.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/scn4m_subm_sram_1kbyte_1rw1r_32x256_8.py` & `openram-1.2.9/macros/sram_configs/scn4m_subm_sram_1kbyte_1rw1r_32x256_8.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/scn4m_subm_sram_2kbyte_1rw1r_32x512_8.py` & `openram-1.2.9/macros/sram_configs/scn4m_subm_sram_2kbyte_1rw1r_32x512_8.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/scn4m_subm_sram_32kbyte_1rw1r_2x32x4096_8.py` & `openram-1.2.9/macros/sram_configs/scn4m_subm_sram_32kbyte_1rw1r_2x32x4096_8.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/scn4m_subm_sram_4kbyte_1rw1r_32x1024_8.py` & `openram-1.2.9/macros/sram_configs/scn4m_subm_sram_4kbyte_1rw1r_32x1024_8.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/scn4m_subm_sram_8kbyte_1rw1r_32x2048_8.py` & `openram-1.2.9/macros/sram_configs/scn4m_subm_sram_8kbyte_1rw1r_32x2048_8.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/sky130_sram_1rw_tiny.py` & `openram-1.2.9/macros/sram_configs/sky130_sram_1rw_tiny.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/macros/sram_configs/sky130_sram_common.py` & `openram-1.2.9/macros/sram_configs/sky130_sram_common.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/openram.egg-info/PKG-INFO` & `openram-1.2.9/openram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openram
-Version: 1.2.8
+Version: 1.2.9
 Summary: An open-source static random access memory (SRAM) compiler
 Home-page: https://openram.org/
 Download-URL: https://github.com/VLSIDA/OpenRAM/releases
 Author: Matthew Guthaus
 Author-email: mrg+vlsida@ucsc.edu
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/VLSIDA/OpenRAM/issues
@@ -82,15 +82,15 @@
 
 
 
 # Publications
 
 + [M. R. Guthaus, J. E. Stine, S. Ataei, B. Chen, B. Wu, M. Sarwar, "OpenRAM: An Open-Source Memory Compiler," Proceedings of the 35th International Conference on Computer-Aided Design (ICCAD), 2016.](https://escholarship.org/content/qt8x19c778/qt8x19c778_noSplash_b2b3fbbb57f1269f86d0de77865b0691.pdf)
 + [S. Ataei, J. Stine, M. Guthaus, “A 64 kb differential single-port 12T SRAM design with a bit-interleaving scheme for low-voltage operation in 32 nm SOI CMOS,” International Conference on Computer Design (ICCD), 2016, pp. 499-506.](https://escholarship.org/uc/item/99f6q9c9)
-+ [E. Ebrahimi, M. Guthaus, J. Renau, “Timing Speculative SRAM”, IEEE In- ternational Symposium on Circuits and Systems (ISCAS), 2017.](https://escholarship.org/content/qt7nn0j5x3/qt7nn0j5x3_noSplash_172457455e1aceba20694c3d7aa489b4.pdf)
++ [E. Ebrahimi, M. Guthaus, J. Renau, “Timing Speculative SRAM”, IEEE International Symposium on Circuits and Systems (ISCAS), 2017.](https://escholarship.org/content/qt7nn0j5x3/qt7nn0j5x3_noSplash_172457455e1aceba20694c3d7aa489b4.pdf)
 + [B. Wu, J.E. Stine, M.R. Guthaus, "Fast and Area-Efficient Word-Line Optimization",  IEEE International Symposium on Circuits and Systems (ISCAS), 2019.](https://escholarship.org/content/qt98s4c1hp/qt98s4c1hp_noSplash_753dcc3e218f60aafff98ef77fb56384.pdf)
 + [B. Wu, M. Guthaus, "Bottom Up Approach for High Speed SRAM Word-line Buffer Insertion Optimization", IFIP/IEEE International Conference on Very Large Scale Integration (VLSI-SoC), 2019.](https://ieeexplore.ieee.org/document/8920325)
 + [H. Nichols, M. Grimes, J. Sowash, J. Cirimelli-Low, M. Guthaus "Automated Synthesis of Multi-Port Memories and Control", IFIP/IEEE International Conference on Very Large Scale Integration (VLSI-SoC), 2019.](https://escholarship.org/content/qt7047n3k0/qt7047n3k0.pdf?t=q4gcij)
 + [H. Nichols, "Statistical Modeling of SRAMs", M.S. Thesis, UCSC, 2022.](https://escholarship.org/content/qt7vx9n089/qt7vx9n089_noSplash_cfc4ba479d8eb1b6ec25d7c92357bc18.pdf?t=ra9wzr)
 + [M. Guthaus, H. Nichols, J. Cirimelli-Low, J. Kunzler, B. Wu, "Enabling Design Technology Co-Optimization of SRAMs though Open-Source Software", IEEE International Electron Devices Meeting (IEDM), 2020.](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9372047)
```

### Comparing `openram-1.2.8/openram.egg-info/SOURCES.txt` & `openram-1.2.9/openram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/openram.mk` & `openram-1.2.9/openram.mk`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/rom_compiler.py` & `openram-1.2.9/rom_compiler.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/setup.py` & `openram-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/sram_compiler.py` & `openram-1.2.9/sram_compiler.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/__init__.py` & `openram-1.2.9/technology/freepdk45/__init__.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/gds_lib/cell_1rw.gds` & `openram-1.2.9/technology/freepdk45/gds_lib/cell_1rw.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/gds_lib/cell_2rw.gds` & `openram-1.2.9/technology/freepdk45/gds_lib/cell_2rw.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/gds_lib/dff.gds` & `openram-1.2.9/technology/freepdk45/gds_lib/dff.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/gds_lib/dummy_cell_1rw.gds` & `openram-1.2.9/technology/freepdk45/gds_lib/dummy_cell_1rw.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/gds_lib/dummy_cell_2rw.gds` & `openram-1.2.9/technology/freepdk45/gds_lib/dummy_cell_2rw.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/gds_lib/replica_cell_1rw.gds` & `openram-1.2.9/technology/freepdk45/gds_lib/replica_cell_1rw.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/gds_lib/replica_cell_2rw.gds` & `openram-1.2.9/technology/freepdk45/gds_lib/replica_cell_2rw.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/gds_lib/sense_amp.gds` & `openram-1.2.9/technology/freepdk45/gds_lib/sense_amp.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/gds_lib/tri_gate.gds` & `openram-1.2.9/technology/freepdk45/gds_lib/tri_gate.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/gds_lib/write_driver.gds` & `openram-1.2.9/technology/freepdk45/gds_lib/write_driver.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/layers.map` & `openram-1.2.9/technology/freepdk45/layers.map`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/APACHE-LICENSE-2.0.txt` & `openram-1.2.9/technology/freepdk45/models/APACHE-LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/hspice_ff.include` & `openram-1.2.9/technology/freepdk45/models/hspice_ff.include`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/hspice_nom.include` & `openram-1.2.9/technology/freepdk45/models/hspice_nom.include`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/hspice_ss.include` & `openram-1.2.9/technology/freepdk45/models/hspice_ss.include`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/NMOS_THKOX.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/NMOS_THKOX.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/NMOS_VTG.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/NMOS_VTG.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/NMOS_VTH.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/NMOS_VTH.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/NMOS_VTL.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/NMOS_VTL.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/PMOS_THKOX.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/PMOS_THKOX.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/PMOS_VTG.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/PMOS_VTG.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/PMOS_VTH.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/PMOS_VTH.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ff/PMOS_VTL.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ff/PMOS_VTL.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/NMOS_THKOX.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/NMOS_THKOX.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/NMOS_VTG.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/NMOS_VTG.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/NMOS_VTH.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/NMOS_VTH.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/NMOS_VTL.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/NMOS_VTL.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/PMOS_THKOX.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/PMOS_THKOX.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/PMOS_VTG.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/PMOS_VTG.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/PMOS_VTH.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/PMOS_VTH.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_nom/PMOS_VTL.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_nom/PMOS_VTL.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/NMOS_THKOX.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/NMOS_THKOX.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/NMOS_VTG.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/NMOS_VTG.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/NMOS_VTH.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/NMOS_VTH.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/NMOS_VTL.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/NMOS_VTL.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/PMOS_THKOX.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/PMOS_THKOX.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/PMOS_VTG.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/PMOS_VTG.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/PMOS_VTH.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/PMOS_VTH.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/models/tran_models/models_ss/PMOS_VTL.inc` & `openram-1.2.9/technology/freepdk45/models/tran_models/models_ss/PMOS_VTL.inc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/sim_data/leakage_data.csv` & `openram-1.2.9/technology/freepdk45/sim_data/leakage_data.csv`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/sim_data/sim_data.csv` & `openram-1.2.9/technology/freepdk45/sim_data/sim_data.csv`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/sp_lib/cell_2rw.sp` & `openram-1.2.9/technology/freepdk45/sp_lib/cell_2rw.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/sp_lib/dff.sp` & `openram-1.2.9/technology/freepdk45/sp_lib/dff.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/sp_lib/dummy_cell_2rw.sp` & `openram-1.2.9/technology/freepdk45/sp_lib/dummy_cell_2rw.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/sp_lib/replica_cell_2rw.sp` & `openram-1.2.9/technology/freepdk45/sp_lib/replica_cell_2rw.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/sp_lib/write_driver.sp` & `openram-1.2.9/technology/freepdk45/sp_lib/write_driver.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/tech/freepdk45.lydrc` & `openram-1.2.9/technology/freepdk45/tech/freepdk45.lydrc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/tech/freepdk45.lylvs` & `openram-1.2.9/technology/freepdk45/tech/freepdk45.lylvs`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/tech/freepdk45.lyp` & `openram-1.2.9/technology/freepdk45/tech/freepdk45.lyp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/tech/freepdk45.lyt` & `openram-1.2.9/technology/freepdk45/tech/freepdk45.lyt`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/tech/scn4m_subm.lyp` & `openram-1.2.9/technology/freepdk45/tech/scn4m_subm.lyp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/tech/scn4m_subm.lyt` & `openram-1.2.9/technology/freepdk45/tech/scn4m_subm.lyt`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/tech/tech.py` & `openram-1.2.9/technology/freepdk45/tech/tech.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/tf/APACHE-LICENSE-2.0.txt` & `openram-1.2.9/technology/freepdk45/tf/APACHE-LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/tf/FreePDK45.tf` & `openram-1.2.9/technology/freepdk45/tf/FreePDK45.tf`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/tf/README.txt` & `openram-1.2.9/technology/freepdk45/tf/README.txt`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/tf/SVRF_EULA_06Feb09.txt` & `openram-1.2.9/technology/freepdk45/tf/SVRF_EULA_06Feb09.txt`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/tf/display.drf` & `openram-1.2.9/technology/freepdk45/tf/display.drf`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/freepdk45/tf/layers.map` & `openram-1.2.9/technology/freepdk45/tf/layers.map`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/__init__.py` & `openram-1.2.9/technology/scn3me_subm/__init__.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/gds_lib/cell_1rw_1r.gds` & `openram-1.2.9/technology/scn3me_subm/gds_lib/cell_1rw_1r.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/gds_lib/cell_1w_1r.gds` & `openram-1.2.9/technology/scn3me_subm/gds_lib/cell_1w_1r.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/gds_lib/cell_6t.gds` & `openram-1.2.9/technology/scn3me_subm/gds_lib/cell_6t.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/gds_lib/dff.gds` & `openram-1.2.9/technology/scn3me_subm/gds_lib/dff.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/gds_lib/ms_flop.gds` & `openram-1.2.9/technology/scn3me_subm/gds_lib/ms_flop.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/gds_lib/replica_cell_1rw_1r.gds` & `openram-1.2.9/technology/scn3me_subm/gds_lib/replica_cell_1rw_1r.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/gds_lib/replica_cell_1w_1r.gds` & `openram-1.2.9/technology/scn3me_subm/gds_lib/replica_cell_1w_1r.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/gds_lib/replica_cell_6t.gds` & `openram-1.2.9/technology/scn3me_subm/gds_lib/replica_cell_6t.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/gds_lib/sense_amp.gds` & `openram-1.2.9/technology/scn3me_subm/gds_lib/sense_amp.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/gds_lib/tri_gate.gds` & `openram-1.2.9/technology/scn3me_subm/gds_lib/tri_gate.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/gds_lib/write_driver.gds` & `openram-1.2.9/technology/scn3me_subm/gds_lib/write_driver.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/mag_lib/cell_1rw_1r.mag` & `openram-1.2.9/technology/scn3me_subm/mag_lib/cell_1rw_1r.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/mag_lib/cell_1w_1r.mag` & `openram-1.2.9/technology/scn3me_subm/mag_lib/cell_1w_1r.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/mag_lib/cell_6t.mag` & `openram-1.2.9/technology/scn3me_subm/mag_lib/cell_6t.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/mag_lib/dff.mag` & `openram-1.2.9/technology/scn3me_subm/mag_lib/dff.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/mag_lib/ms_flop.mag` & `openram-1.2.9/technology/scn3me_subm/mag_lib/ms_flop.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/mag_lib/replica_cell_1rw_1r.mag` & `openram-1.2.9/technology/scn3me_subm/mag_lib/replica_cell_1rw_1r.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/mag_lib/replica_cell_1w_1r.mag` & `openram-1.2.9/technology/scn3me_subm/mag_lib/replica_cell_1w_1r.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/mag_lib/replica_cell_6t.mag` & `openram-1.2.9/technology/scn3me_subm/mag_lib/replica_cell_6t.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/mag_lib/sense_amp.mag` & `openram-1.2.9/technology/scn3me_subm/mag_lib/sense_amp.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/mag_lib/tri_gate.mag` & `openram-1.2.9/technology/scn3me_subm/mag_lib/tri_gate.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/mag_lib/write_driver.mag` & `openram-1.2.9/technology/scn3me_subm/mag_lib/write_driver.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/sp_lib/dff.sp` & `openram-1.2.9/technology/scn3me_subm/sp_lib/dff.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/sp_lib/ms_flop.sp` & `openram-1.2.9/technology/scn3me_subm/sp_lib/ms_flop.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/sp_lib/write_driver.sp` & `openram-1.2.9/technology/scn3me_subm/sp_lib/write_driver.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/sue_lib/cell_6t.sue` & `openram-1.2.9/technology/scn3me_subm/sue_lib/cell_6t.sue`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/sue_lib/ms_flop.sue` & `openram-1.2.9/technology/scn3me_subm/sue_lib/ms_flop.sue`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/sue_lib/replica_cell_6t.sue` & `openram-1.2.9/technology/scn3me_subm/sue_lib/replica_cell_6t.sue`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/sue_lib/sense_amp.sue` & `openram-1.2.9/technology/scn3me_subm/sue_lib/sense_amp.sue`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/sue_lib/tri_gate.sue` & `openram-1.2.9/technology/scn3me_subm/sue_lib/tri_gate.sue`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/sue_lib/write_driver.sue` & `openram-1.2.9/technology/scn3me_subm/sue_lib/write_driver.sue`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/tech/SCN3ME_SUBM.30.tech` & `openram-1.2.9/technology/scn3me_subm/tech/SCN3ME_SUBM.30.tech`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/tech/calibreDRC_scn3me_subm.rul` & `openram-1.2.9/technology/scn3me_subm/tech/calibreDRC_scn3me_subm.rul`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/tech/calibreLVS_scn3me_subm.rul` & `openram-1.2.9/technology/scn3me_subm/tech/calibreLVS_scn3me_subm.rul`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/tech/setup.tcl` & `openram-1.2.9/technology/scn3me_subm/tech/setup.tcl`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/tech/tech.py` & `openram-1.2.9/technology/scn3me_subm/tech/tech.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/tf/README` & `openram-1.2.9/technology/scn3me_subm/tf/README`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/tf/display.drf` & `openram-1.2.9/technology/scn3me_subm/tf/display.drf`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn3me_subm/tf/mosis.tf` & `openram-1.2.9/technology/scn3me_subm/tf/mosis.tf`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/__init__.py` & `openram-1.2.9/technology/scn4m_subm/__init__.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/gds_lib/cell_1rw.gds` & `openram-1.2.9/technology/scn4m_subm/gds_lib/cell_1rw.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/gds_lib/cell_2rw.gds` & `openram-1.2.9/technology/scn4m_subm/gds_lib/cell_2rw.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/gds_lib/dff.gds` & `openram-1.2.9/technology/scn4m_subm/gds_lib/dff.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/gds_lib/dummy_cell_1rw.gds` & `openram-1.2.9/technology/scn4m_subm/gds_lib/dummy_cell_1rw.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/gds_lib/dummy_cell_2rw.gds` & `openram-1.2.9/technology/scn4m_subm/gds_lib/dummy_cell_2rw.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/gds_lib/replica_cell_1rw.gds` & `openram-1.2.9/technology/scn4m_subm/gds_lib/replica_cell_1rw.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/gds_lib/replica_cell_2rw.gds` & `openram-1.2.9/technology/scn4m_subm/gds_lib/replica_cell_2rw.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/gds_lib/sense_amp.gds` & `openram-1.2.9/technology/scn4m_subm/gds_lib/sense_amp.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/gds_lib/tri_gate.gds` & `openram-1.2.9/technology/scn4m_subm/gds_lib/tri_gate.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/gds_lib/write_driver.gds` & `openram-1.2.9/technology/scn4m_subm/gds_lib/write_driver.gds`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/mag_lib/cell_1rw.mag` & `openram-1.2.9/technology/scn4m_subm/mag_lib/cell_1rw.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/mag_lib/cell_2rw.mag` & `openram-1.2.9/technology/scn4m_subm/mag_lib/cell_2rw.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/mag_lib/dff.mag` & `openram-1.2.9/technology/scn4m_subm/mag_lib/dff.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/mag_lib/dummy_cell_1rw.mag` & `openram-1.2.9/technology/scn4m_subm/mag_lib/dummy_cell_1rw.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/mag_lib/dummy_cell_2rw.mag` & `openram-1.2.9/technology/scn4m_subm/mag_lib/dummy_cell_2rw.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/mag_lib/replica_cell_1rw.mag` & `openram-1.2.9/technology/scn4m_subm/mag_lib/replica_cell_1rw.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/mag_lib/replica_cell_2rw.mag` & `openram-1.2.9/technology/scn4m_subm/mag_lib/replica_cell_2rw.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/mag_lib/sense_amp.mag` & `openram-1.2.9/technology/scn4m_subm/mag_lib/sense_amp.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/mag_lib/tri_gate.mag` & `openram-1.2.9/technology/scn4m_subm/mag_lib/tri_gate.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/mag_lib/write_driver.mag` & `openram-1.2.9/technology/scn4m_subm/mag_lib/write_driver.mag`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/models/ff/nmos.sp` & `openram-1.2.9/technology/scn4m_subm/models/ff/nmos.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/models/ff/pmos.sp` & `openram-1.2.9/technology/scn4m_subm/models/ff/pmos.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/models/nom/nmos.sp` & `openram-1.2.9/technology/scn4m_subm/models/nom/nmos.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/models/nom/pmos.sp` & `openram-1.2.9/technology/scn4m_subm/models/nom/pmos.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/models/ss/nmos.sp` & `openram-1.2.9/technology/scn4m_subm/models/ss/nmos.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/models/ss/pmos.sp` & `openram-1.2.9/technology/scn4m_subm/models/ss/pmos.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/sim_data/sim_data.csv` & `openram-1.2.9/technology/scn4m_subm/sim_data/sim_data.csv`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/sp_lib/cell_6t.st0` & `openram-1.2.9/technology/scn4m_subm/sp_lib/cell_6t.st0`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/sp_lib/dff.sp` & `openram-1.2.9/technology/scn4m_subm/sp_lib/dff.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/sp_lib/write_driver.sp` & `openram-1.2.9/technology/scn4m_subm/sp_lib/write_driver.sp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/tech/.magicrc` & `openram-1.2.9/technology/scn4m_subm/tech/.magicrc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/tech/SCN4M_SUBM.20.tech` & `openram-1.2.9/technology/scn4m_subm/tech/SCN4M_SUBM.20.tech`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/tech/scn4m_subm.lydrc` & `openram-1.2.9/technology/scn4m_subm/tech/scn4m_subm.lydrc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/tech/scn4m_subm.lylvs` & `openram-1.2.9/technology/scn4m_subm/tech/scn4m_subm.lylvs`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/tech/setup.tcl` & `openram-1.2.9/technology/scn4m_subm/tech/setup.tcl`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/tech/tech.py` & `openram-1.2.9/technology/scn4m_subm/tech/tech.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/tf/README.txt` & `openram-1.2.9/technology/scn4m_subm/tf/README.txt`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/tf/display.drf` & `openram-1.2.9/technology/scn4m_subm/tf/display.drf`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/tf/layers.map` & `openram-1.2.9/technology/scn4m_subm/tf/layers.map`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/tf/mosis.lyp` & `openram-1.2.9/technology/scn4m_subm/tf/mosis.lyp`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/tf/mosis.lyt` & `openram-1.2.9/technology/scn4m_subm/tf/mosis.lyt`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/scn4m_subm/tf/mosis.tf` & `openram-1.2.9/technology/scn4m_subm/tf/mosis.tf`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/setup_scripts/gen_analytical_model.py` & `openram-1.2.9/technology/setup_scripts/gen_analytical_model.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/__init__.py` & `openram-1.2.9/technology/sky130/__init__.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_bitcell.py` & `openram-1.2.9/technology/sky130/custom/sky130_bitcell.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_bitcell_array.py` & `openram-1.2.9/technology/sky130/custom/sky130_bitcell_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_bitcell_base_array.py` & `openram-1.2.9/technology/sky130/custom/sky130_bitcell_base_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_col_cap.py` & `openram-1.2.9/technology/sky130/custom/sky130_col_cap.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_col_cap_array.py` & `openram-1.2.9/technology/sky130/custom/sky130_col_cap_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_corner.py` & `openram-1.2.9/technology/sky130/custom/sky130_corner.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_dummy_array.py` & `openram-1.2.9/technology/sky130/custom/sky130_dummy_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_dummy_bitcell.py` & `openram-1.2.9/technology/sky130/custom/sky130_dummy_bitcell.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_internal.py` & `openram-1.2.9/technology/sky130/custom/sky130_internal.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_replica_bitcell.py` & `openram-1.2.9/technology/sky130/custom/sky130_replica_bitcell.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_replica_bitcell_array.py` & `openram-1.2.9/technology/sky130/custom/sky130_replica_bitcell_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_replica_column.py` & `openram-1.2.9/technology/sky130/custom/sky130_replica_column.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_row_cap.py` & `openram-1.2.9/technology/sky130/custom/sky130_row_cap.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/custom/sky130_row_cap_array.py` & `openram-1.2.9/technology/sky130/custom/sky130_row_cap_array.py`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/tech/sky130.lydrc` & `openram-1.2.9/technology/sky130/tech/sky130.lydrc`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/tech/sky130.lylvs` & `openram-1.2.9/technology/sky130/tech/sky130.lylvs`

 * *Files identical despite different names*

### Comparing `openram-1.2.8/technology/sky130/tech/tech.py` & `openram-1.2.9/technology/sky130/tech/tech.py`

 * *Files identical despite different names*

