# Comparing `tmp/tkfly-0.1.0a1.tar.gz` & `tmp/tkfly-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkfly-0.1.0a1.tar", max compression
+gzip compressed data, was "tkfly-0.1.0a2.tar", max compression
```

## Comparing `tkfly-0.1.0a1.tar` & `tkfly-0.1.0a2.tar`

### file list

```diff
@@ -1,235 +1,328 @@
--rw-r--r--   0        0        0      281 2023-04-29 04:30:07.660748 tkfly-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      712 2023-04-19 14:52:15.664076 tkfly-0.1.0a1/README.md
--rw-r--r--   0        0        0       81 2023-04-19 12:43:56.199467 tkfly-0.1.0a1/tkfly/__init__.py
--rw-r--r--   0        0        0      224 2023-04-19 11:06:45.090485 tkfly-0.1.0a1/tkfly/_tklib/__init__.py
--rw-r--r--   0        0        0      677 2023-04-19 11:08:58.393781 tkfly-0.1.0a1/tkfly/_tklib/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1667 2023-04-14 12:45:42.167394 tkfly-0.1.0a1/tkfly/_tklib/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     7112 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/autoscroll/autoscroll.tcl
--rw-r--r--   0        0        0      611 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/autoscroll/pkgIndex.tcl
--rw-r--r--   0        0        0     7344 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_drag.tcl
--rw-r--r--   0        0        0    10374 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_epoints.tcl
--rw-r--r--   0        0        0    12828 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_epolyline.tcl
--rw-r--r--   0        0        0    11211 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_equad.tcl
--rw-r--r--   0        0        0     7467 2014-08-11 05:20:11.000000 tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_gradient.tcl
--rw-r--r--   0        0        0     2947 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_highlight.tcl
--rw-r--r--   0        0        0     9922 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_mvg.tcl
--rw-r--r--   0        0        0     2964 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_snap.tcl
--rw-r--r--   0        0        0    21321 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_sqmap.tcl
--rw-r--r--   0        0        0     1545 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_tags.tcl
--rw-r--r--   0        0        0     2195 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_trlines.tcl
--rw-r--r--   0        0        0     5161 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_zoom.tcl
--rw-r--r--   0        0        0     1295 2014-08-11 05:20:11.000000 tkfly-0.1.0a1/tkfly/_tklib/canvas/pkgIndex.tcl
--rw-r--r--   0        0        0    26671 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/chatwidget/chatwidget.tcl
--rw-r--r--   0        0        0       80 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/chatwidget/pkgIndex.tcl
--rw-r--r--   0        0        0     1365 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/controlwidget/bindDown.tcl
--rw-r--r--   0        0        0      381 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/controlwidget/controlwidget.tcl
--rw-r--r--   0        0        0     3401 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/controlwidget/led.tcl
--rw-r--r--   0        0        0      903 2018-05-11 03:56:07.000000 tkfly-0.1.0a1/tkfly/_tklib/controlwidget/pkgIndex.tcl
--rw-r--r--   0        0        0     7666 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/controlwidget/radioMatrix.tcl
--rw-r--r--   0        0        0    16186 2018-05-11 03:56:08.000000 tkfly-0.1.0a1/tkfly/_tklib/controlwidget/rdial.tcl
--rw-r--r--   0        0        0    12150 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/controlwidget/tachometer.tcl
--rw-r--r--   0        0        0    48034 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/controlwidget/vertical_meter.tcl
--rw-r--r--   0        0        0    11332 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/controlwidget/voltmeter.tcl
--rw-r--r--   0        0        0    16207 2014-08-11 05:20:11.000000 tkfly-0.1.0a1/tkfly/_tklib/crosshair/crosshair.tcl
--rw-r--r--   0        0        0      138 2013-05-10 05:18:16.000000 tkfly-0.1.0a1/tkfly/_tklib/crosshair/pkgIndex.tcl
--rw-r--r--   0        0        0    27293 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/ctext/ctext.tcl
--rw-r--r--   0        0        0       68 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/ctext/pkgIndex.tcl
--rw-r--r--   0        0        0     3924 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/cursor/cursor.tcl
--rw-r--r--   0        0        0       72 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/cursor/pkgIndex.tcl
--rw-r--r--   0        0        0    12481 2020-01-06 23:27:53.000000 tkfly-0.1.0a1/tkfly/_tklib/datefield/datefield.tcl
--rw-r--r--   0        0        0       76 2020-01-06 23:27:53.000000 tkfly-0.1.0a1/tkfly/_tklib/datefield/pkgIndex.tcl
--rw-r--r--   0        0        0    12537 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/diagrams/application.tcl
--rw-r--r--   0        0        0    10383 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/diagrams/attributes.tcl
--rw-r--r--   0        0        0    37096 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/diagrams/basic.tcl
--rw-r--r--   0        0        0    32433 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/diagrams/core.tcl
--rw-r--r--   0        0        0     1557 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/diagrams/diagram.tcl
--rw-r--r--   0        0        0     7807 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/diagrams/direction.tcl
--rw-r--r--   0        0        0     7931 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/diagrams/element.tcl
--rw-r--r--   0        0        0     3423 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/diagrams/navigation.tcl
--rw-r--r--   0        0        0      847 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/diagrams/pkgIndex.tcl
--rw-r--r--   0        0        0     4837 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/diagrams/point.tcl
--rw-r--r--   0        0        0      612 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/getstring/pkgIndex.tcl
--rw-r--r--   0        0        0     4224 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/getstring/tk_getString.tcl
--rw-r--r--   0        0        0     3187 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/history/history.tcl
--rw-r--r--   0        0        0      605 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/history/pkgIndex.tcl
--rw-r--r--   0        0        0    44954 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/ico/ico.tcl
--rw-r--r--   0        0        0    35176 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/ico/ico0.tcl
--rw-r--r--   0        0        0      292 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/ico/pkgIndex.tcl
--rw-r--r--   0        0        0    29231 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/ipentry/ipentry.tcl
--rw-r--r--   0        0        0      139 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/ipentry/pkgIndex.tcl
--rw-r--r--   0        0        0     3795 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/khim/cs.msg
--rw-r--r--   0        0        0     3718 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/khim/da.msg
--rw-r--r--   0        0        0     4409 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/khim/de.msg
--rw-r--r--   0        0        0     3918 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/khim/en.msg
--rw-r--r--   0        0        0     3979 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/khim/es.msg
--rw-r--r--   0        0        0    56665 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/khim/khim.tcl
--rw-r--r--   0        0        0      534 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/khim/pkgIndex.tcl
--rw-r--r--   0        0        0     4124 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/khim/pl.msg
--rw-r--r--   0        0        0     2937 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/khim/ROOT.msg
--rw-r--r--   0        0        0     6679 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/khim/ru.msg
--rw-r--r--   0        0        0     6361 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/khim/uk.msg
--rw-r--r--   0        0        0      444 2020-01-06 23:27:53.000000 tkfly-0.1.0a1/tkfly/_tklib/mentry/mentry.tcl
--rw-r--r--   0        0        0      737 2020-01-06 23:27:53.000000 tkfly-0.1.0a1/tkfly/_tklib/mentry/mentry_tile.tcl
--rw-r--r--   0        0        0     2592 2020-01-06 23:27:53.000000 tkfly-0.1.0a1/tkfly/_tklib/mentry/mentryPublic.tcl
--rw-r--r--   0        0        0      860 2020-01-06 23:27:53.000000 tkfly-0.1.0a1/tkfly/_tklib/mentry/pkgIndex.tcl
--rw-r--r--   0        0        0    25858 2019-08-21 18:42:16.000000 tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mentryDateTime.tcl
--rw-r--r--   0        0        0     4298 2019-08-21 18:42:16.000000 tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mentryFixedPoint.tcl
--rw-r--r--   0        0        0     5661 2019-08-21 18:42:16.000000 tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mentryIPAddr.tcl
--rw-r--r--   0        0        0     6884 2019-08-21 18:42:16.000000 tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mentryIPv6Addr.tcl
--rw-r--r--   0        0        0    18737 2019-08-21 18:42:16.000000 tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mentryThemes.tcl
--rw-r--r--   0        0        0    60325 2019-08-21 18:42:16.000000 tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mentryWidget.tcl
--rw-r--r--   0        0        0    19506 2020-01-06 23:27:53.000000 tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mwutil.tcl
--rw-r--r--   0        0        0    10636 2020-01-06 23:27:53.000000 tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/tclIndex
--rw-r--r--   0        0        0     5469 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/menubar/debug.tcl
--rw-r--r--   0        0        0    53951 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/menubar/menubar.tcl
--rw-r--r--   0        0        0     3859 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/menubar/node.tcl
--rw-r--r--   0        0        0      299 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/menubar/pkgIndex.tcl
--rw-r--r--   0        0        0    26016 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/menubar/tree.tcl
--rw-r--r--   0        0        0     4041 2020-01-06 23:27:53.000000 tkfly-0.1.0a1/tkfly/_tklib/notifywindow/notifywindow.tcl
--rw-r--r--   0        0        0      548 2016-07-14 05:57:54.000000 tkfly-0.1.0a1/tkfly/_tklib/notifywindow/pkgIndex.tcl
--rw-r--r--   0        0        0   120514 2018-05-11 03:56:08.000000 tkfly-0.1.0a1/tkfly/_tklib/ntext/ntext.tcl
--rw-r--r--   0        0        0      132 2020-02-09 20:50:00.000000 tkfly-0.1.0a1/tkfly/_tklib/ntext/pkgIndex.tcl
--rw-r--r--   0        0        0    30859 2020-02-09 20:50:00.000000 tkfly-0.1.0a1/tkfly/_tklib/persistentSelection/persistentSelection.tcl
--rw-r--r--   0        0        0      160 2020-02-09 20:50:00.000000 tkfly-0.1.0a1/tkfly/_tklib/persistentSelection/pkgIndex.tcl
--rw-r--r--   0        0        0     3291 2023-04-14 12:33:32.365933 tkfly-0.1.0a1/tkfly/_tklib/pkgIndex.tcl
--rw-r--r--   0        0        0      321 2018-05-11 03:56:08.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/pkgIndex.tcl
--rw-r--r--   0        0        0    13471 2015-04-21 06:10:00.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plot3d.tcl
--rw-r--r--   0        0        0    15740 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotanim.tcl
--rw-r--r--   0        0        0    12916 2018-05-11 03:56:08.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotannot.tcl
--rw-r--r--   0        0        0    67951 2018-05-11 03:56:08.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotaxis.tcl
--rw-r--r--   0        0        0     6478 2019-08-21 18:42:16.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotbind.tcl
--rw-r--r--   0        0        0    11059 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotbusiness.tcl
--rw-r--r--   0        0        0   108162 2019-08-21 18:42:16.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotchart.tcl
--rw-r--r--   0        0        0     5721 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotcombined.tcl
--rw-r--r--   0        0        0    16783 2015-04-21 06:10:00.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotconfig.tcl
--rw-r--r--   0        0        0    61163 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotcontour.tcl
--rw-r--r--   0        0        0    10041 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotgantt.tcl
--rw-r--r--   0        0        0     8895 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotobject.tcl
--rw-r--r--   0        0        0     9423 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotpack.tcl
--rw-r--r--   0        0        0   139321 2018-05-11 03:56:08.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotpriv.tcl
--rw-r--r--   0        0        0     8072 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotscada.tcl
--rw-r--r--   0        0        0     5697 2016-07-14 05:57:54.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotspecial.tcl
--rw-r--r--   0        0        0     7475 2014-08-11 05:20:12.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotstatustimeline.tcl
--rw-r--r--   0        0        0     9893 2015-04-21 06:10:00.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/plottable.tcl
--rw-r--r--   0        0        0     5215 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/scaling.tcl
--rw-r--r--   0        0        0    16372 2014-11-24 17:34:56.000000 tkfly-0.1.0a1/tkfly/_tklib/plotchart/xyplot.tcl
--rw-r--r--   0        0        0      833 2020-02-09 20:36:05.000000 tkfly-0.1.0a1/tkfly/_tklib/scrollutil/pkgIndex.tcl
--rw-r--r--   0        0        0    19506 2020-01-08 04:03:39.000000 tkfly-0.1.0a1/tkfly/_tklib/scrollutil/scripts/mwutil.tcl
--rw-r--r--   0        0        0    27093 2020-01-08 04:03:39.000000 tkfly-0.1.0a1/tkfly/_tklib/scrollutil/scripts/scrollableframe.tcl
--rw-r--r--   0        0        0    27166 2020-02-09 20:36:05.000000 tkfly-0.1.0a1/tkfly/_tklib/scrollutil/scripts/scrollarea.tcl
--rw-r--r--   0        0        0    17573 2020-01-08 04:03:39.000000 tkfly-0.1.0a1/tkfly/_tklib/scrollutil/scripts/scrollsync.tcl
--rw-r--r--   0        0        0     9299 2020-02-09 20:36:05.000000 tkfly-0.1.0a1/tkfly/_tklib/scrollutil/scripts/tclIndex
--rw-r--r--   0        0        0    20797 2020-02-09 20:36:05.000000 tkfly-0.1.0a1/tkfly/_tklib/scrollutil/scripts/wheelEvent.tcl
--rw-r--r--   0        0        0      632 2020-02-09 20:36:05.000000 tkfly-0.1.0a1/tkfly/_tklib/scrollutil/scrollutil.tcl
--rw-r--r--   0        0        0      772 2020-02-09 20:36:05.000000 tkfly-0.1.0a1/tkfly/_tklib/scrollutil/scrollutil_tile.tcl
--rw-r--r--   0        0        0     2517 2020-02-09 20:36:05.000000 tkfly-0.1.0a1/tkfly/_tklib/scrollutil/scrollutilCommon.tcl
--rw-r--r--   0        0        0    15316 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/style/as.tcl
--rw-r--r--   0        0        0     2848 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/style/lobster.tcl
--rw-r--r--   0        0        0      684 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/style/pkgIndex.tcl
--rw-r--r--   0        0        0      765 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/style/style.tcl
--rw-r--r--   0        0        0      607 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/swaplist/pkgIndex.tcl
--rw-r--r--   0        0        0    13365 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/swaplist/swaplist.tcl
--rw-r--r--   0        0        0      898 2020-01-06 23:27:54.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/pkgIndex.tcl
--rw-r--r--   0        0        0    19506 2020-01-06 23:27:54.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/mwutil.tcl
--rw-r--r--   0        0        0     4286 2015-04-21 06:10:00.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/pencil.cur
--rw-r--r--   0        0        0     2911 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/repair.tcl
--rw-r--r--   0        0        0   133438 2020-01-06 23:27:54.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistBind.tcl
--rw-r--r--   0        0        0   120387 2020-01-06 23:27:54.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistConfig.tcl
--rw-r--r--   0        0        0    93461 2020-01-06 23:27:54.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistEdit.tcl
--rw-r--r--   0        0        0   125609 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistImages.tcl
--rw-r--r--   0        0        0    17564 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistMove.tcl
--rw-r--r--   0        0        0    20512 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistSort.tcl
--rw-r--r--   0        0        0    68715 2020-01-06 23:27:54.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistThemes.tcl
--rw-r--r--   0        0        0   202524 2020-01-06 23:27:54.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistUtil.tcl
--rw-r--r--   0        0        0   267492 2020-01-06 23:27:54.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistWidget.tcl
--rw-r--r--   0        0        0    62720 2020-01-06 23:27:54.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tclIndex
--rw-r--r--   0        0        0      488 2020-01-06 23:27:54.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/tablelist.tcl
--rw-r--r--   0        0        0      763 2020-01-06 23:27:54.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/tablelist_tile.tcl
--rw-r--r--   0        0        0     3022 2020-01-06 23:27:54.000000 tkfly-0.1.0a1/tkfly/_tklib/tablelist/tablelistPublic.tcl
--rw-r--r--   0        0        0     4807 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/boxlabel.tcl
--rw-r--r--   0        0        0     7705 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/canlabel.tcl
--rw-r--r--   0        0        0     3303 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/labarray.tcl
--rw-r--r--   0        0        0     1185 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/objselec.tcl
--rw-r--r--   0        0        0     8331 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/perilabel.tcl
--rw-r--r--   0        0        0    15130 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/pie.tcl
--rw-r--r--   0        0        0     1231 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/pielabel.tcl
--rw-r--r--   0        0        0      154 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/pkgIndex.tcl
--rw-r--r--   0        0        0     4150 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/relirect.tcl
--rw-r--r--   0        0        0     4729 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/selector.tcl
--rw-r--r--   0        0        0    13055 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/slice.tcl
--rw-r--r--   0        0        0     4728 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/tkpiechart.tcl
--rw-r--r--   0        0        0      166 2018-05-11 03:56:08.000000 tkfly-0.1.0a1/tkfly/_tklib/tooltip/pkgIndex.tcl
--rw-r--r--   0        0        0     4021 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/tooltip/tipstack.tcl
--rw-r--r--   0        0        0    14446 2018-05-11 03:56:08.000000 tkfly-0.1.0a1/tkfly/_tklib/tooltip/tooltip.tcl
--rw-r--r--   0        0        0      427 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/wcb/pkgIndex.tcl
--rw-r--r--   0        0        0     3561 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/tclIndex
--rw-r--r--   0        0        0    14936 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/wcbCommon.tcl
--rw-r--r--   0        0        0    11684 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/wcbEntry.tcl
--rw-r--r--   0        0        0     2174 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/wcbListbox.tcl
--rw-r--r--   0        0        0     3247 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/wcbTablelist.tcl
--rw-r--r--   0        0        0     6860 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/wcbText.tcl
--rw-r--r--   0        0        0     2701 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/wcbTreeview.tcl
--rw-r--r--   0        0        0     1839 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/wcb/wcb.tcl
--rw-r--r--   0        0        0     3866 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/arrowb.tcl
--rw-r--r--   0        0        0    20697 2013-03-26 03:28:23.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/calendar.tcl
--rw-r--r--   0        0        0    10039 2013-03-26 03:28:23.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/dateentry.tcl
--rw-r--r--   0        0        0    14200 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/dialog.tcl
--rw-r--r--   0        0        0     9158 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/mentry.tcl
--rw-r--r--   0        0        0     6617 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/panelframe.tcl
--rw-r--r--   0        0        0     1144 2013-03-26 03:28:23.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/pkgIndex.tcl
--rw-r--r--   0        0        0    18647 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/ruler.tcl
--rw-r--r--   0        0        0     7563 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/scrollw.tcl
--rw-r--r--   0        0        0     8025 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/statusbar.tcl
--rw-r--r--   0        0        0     2093 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/stext.tcl
--rw-r--r--   0        0        0     3927 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/superframe.tcl
--rw-r--r--   0        0        0     7915 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/toolbar.tcl
--rw-r--r--   0        0        0     4374 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/widget/widget.tcl
--rw-r--r--   0        0        0    32987 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/widgetl/listentry.tcl
--rw-r--r--   0        0        0    18733 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/widgetl/listsimple.tcl
--rw-r--r--   0        0        0      237 2019-08-21 18:42:17.000000 tkfly-0.1.0a1/tkfly/_tklib/widgetl/pkgIndex.tcl
--rw-r--r--   0        0        0      142 2020-02-09 20:50:00.000000 tkfly-0.1.0a1/tkfly/_tklib/widgetPlus/pkgIndex.tcl
--rw-r--r--   0        0        0    57846 2020-02-09 20:50:00.000000 tkfly-0.1.0a1/tkfly/_tklib/widgetPlus/widgetPlus.tcl
--rw-r--r--   0        0        0      146 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/widgetv/pkgIndex.tcl
--rw-r--r--   0        0        0    12031 2013-02-14 03:37:16.000000 tkfly-0.1.0a1/tkfly/_tklib/widgetv/validator.tcl
--rw-r--r--   0        0        0     2217 2023-04-19 11:11:33.981831 tkfly-0.1.0a1/tkfly/core.py
--rw-r--r--   0        0        0      222 2023-04-14 12:59:16.512351 tkfly-0.1.0a1/tkfly/tkimg/__init__.py
--rw-r--r--   0        0        0   221710 2022-11-24 07:55:52.000000 tkfly-0.1.0a1/tkfly/tkimg/jpegtcl950.dll
--rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a1/tkfly/tkimg/libjpegtclstub950.a
--rw-r--r--   0        0        0     1220 2022-11-24 07:55:44.000000 tkfly-0.1.0a1/tkfly/tkimg/libpngtclstub1638.a
--rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a1/tkfly/tkimg/libtifftclstub440.a
--rw-r--r--   0        0        0     1220 2022-11-24 07:55:44.000000 tkfly-0.1.0a1/tkfly/tkimg/libtkimgstub1414.a
--rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a1/tkfly/tkimg/libzlibtclstub1213.a
--rw-r--r--   0        0        0     6851 2022-11-24 07:55:44.000000 tkfly-0.1.0a1/tkfly/tkimg/pkgIndex.tcl
--rw-r--r--   0        0        0   231950 2022-11-24 07:55:52.000000 tkfly-0.1.0a1/tkfly/tkimg/pngtcl1638.dll
--rw-r--r--   0        0        0   416782 2022-11-24 07:55:52.000000 tkfly-0.1.0a1/tkfly/tkimg/tifftcl440.dll
--rw-r--r--   0        0        0    40462 2022-11-24 07:55:54.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimg1414.dll
--rw-r--r--   0        0        0    25614 2022-11-24 07:55:54.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgbmp1414.dll
--rw-r--r--   0        0        0    22030 2022-11-24 07:55:54.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgdted1414.dll
--rw-r--r--   0        0        0    23566 2022-11-24 07:55:56.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgflir1414.dll
--rw-r--r--   0        0        0    24590 2022-11-24 07:55:56.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimggif1414.dll
--rw-r--r--   0        0        0    25614 2022-11-24 07:55:56.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgico1414.dll
--rw-r--r--   0        0        0    23054 2022-11-24 07:55:56.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgjpeg1414.dll
--rw-r--r--   0        0        0    23566 2022-11-24 07:55:58.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgpcx1414.dll
--rw-r--r--   0        0        0    25614 2022-11-24 07:55:58.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgpixmap1414.dll
--rw-r--r--   0        0        0    23566 2022-11-24 07:55:58.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgpng1414.dll
--rw-r--r--   0        0        0    25102 2022-11-24 07:56:00.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgppm1414.dll
--rw-r--r--   0        0        0    21006 2022-11-24 07:56:00.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgps1414.dll
--rw-r--r--   0        0        0    31758 2022-11-24 07:56:00.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgraw1414.dll
--rw-r--r--   0        0        0    28174 2022-11-24 07:56:02.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgsgi1414.dll
--rw-r--r--   0        0        0    25614 2022-11-24 07:56:02.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgsun1414.dll
--rw-r--r--   0        0        0    25102 2022-11-24 07:56:02.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgtga1414.dll
--rw-r--r--   0        0        0    70158 2022-11-24 07:56:04.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgtiff1414.dll
--rw-r--r--   0        0        0    17934 2022-11-24 07:56:04.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgwindow1414.dll
--rw-r--r--   0        0        0    19470 2022-11-24 07:56:04.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgxbm1414.dll
--rw-r--r--   0        0        0    23566 2022-11-24 07:56:06.000000 tkfly-0.1.0a1/tkfly/tkimg/tkimgxpm1414.dll
--rw-r--r--   0        0        0    91662 2022-11-24 07:56:06.000000 tkfly-0.1.0a1/tkfly/tkimg/zlibtcl1213.dll
--rw-r--r--   0        0        0        0 2023-04-19 11:17:10.457150 tkfly-0.1.0a1/tkfly/tklib/__init__.py
--rw-r--r--   0        0        0      141 2023-04-19 12:43:56.373512 tkfly-0.1.0a1/tkfly/tklib/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3960 2023-04-19 12:45:43.059958 tkfly-0.1.0a1/tkfly/tklib/__pycache__/tooltip.cpython-311.pyc
--rw-r--r--   0        0        0      500 2023-04-19 14:52:15.706184 tkfly-0.1.0a1/tkfly/tklib/autoscroll.py
--rw-r--r--   0        0        0      573 2023-04-19 14:52:50.309476 tkfly-0.1.0a1/tkfly/tklib/chatwidget.py
--rw-r--r--   0        0        0      583 2023-04-19 12:47:17.815625 tkfly-0.1.0a1/tkfly/tklib/menubar.py
--rw-r--r--   0        0        0     2066 2023-04-19 12:45:42.877555 tkfly-0.1.0a1/tkfly/tklib/tooltip.py
--rw-r--r--   0        0        0      902 2023-04-19 11:28:27.786655 tkfly-0.1.0a1/tkfly/tklib/wcb.py
--rw-r--r--   0        0        0      476 2023-04-19 13:13:41.356837 tkfly-0.1.0a1/tkfly/tklib/widget.py
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 tkfly-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      280 2023-04-29 10:08:50.067612 tkfly-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     6483 2023-04-29 11:37:28.438767 tkfly-0.1.0a2/README.md
+-rw-r--r--   0        0        0      713 2023-04-29 11:43:39.636888 tkfly-0.1.0a2/tkfly/__init__.py
+-rw-r--r--   0        0        0      673 2023-04-29 10:25:40.967581 tkfly-0.1.0a2/tkfly/__main__.py
+-rw-r--r--   0        0        0      224 2023-04-19 11:06:45.090485 tkfly-0.1.0a2/tkfly/_tklib/__init__.py
+-rw-r--r--   0        0        0      677 2023-04-19 11:08:58.393781 tkfly-0.1.0a2/tkfly/_tklib/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1667 2023-04-14 12:45:42.167394 tkfly-0.1.0a2/tkfly/_tklib/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     7112 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/autoscroll/autoscroll.tcl
+-rw-r--r--   0        0        0      611 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/autoscroll/pkgIndex.tcl
+-rw-r--r--   0        0        0     7344 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_drag.tcl
+-rw-r--r--   0        0        0    10374 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_epoints.tcl
+-rw-r--r--   0        0        0    12828 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_epolyline.tcl
+-rw-r--r--   0        0        0    11211 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_equad.tcl
+-rw-r--r--   0        0        0     7467 2014-08-11 05:20:11.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_gradient.tcl
+-rw-r--r--   0        0        0     2947 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_highlight.tcl
+-rw-r--r--   0        0        0     9922 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_mvg.tcl
+-rw-r--r--   0        0        0     2964 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_snap.tcl
+-rw-r--r--   0        0        0    21321 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_sqmap.tcl
+-rw-r--r--   0        0        0     1545 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_tags.tcl
+-rw-r--r--   0        0        0     2195 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_trlines.tcl
+-rw-r--r--   0        0        0     5161 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_zoom.tcl
+-rw-r--r--   0        0        0     1295 2014-08-11 05:20:11.000000 tkfly-0.1.0a2/tkfly/_tklib/canvas/pkgIndex.tcl
+-rw-r--r--   0        0        0    26671 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/chatwidget/chatwidget.tcl
+-rw-r--r--   0        0        0       80 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/chatwidget/pkgIndex.tcl
+-rw-r--r--   0        0        0     1365 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/bindDown.tcl
+-rw-r--r--   0        0        0      381 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/controlwidget.tcl
+-rw-r--r--   0        0        0     3401 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/led.tcl
+-rw-r--r--   0        0        0      903 2018-05-11 03:56:07.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/pkgIndex.tcl
+-rw-r--r--   0        0        0     7666 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/radioMatrix.tcl
+-rw-r--r--   0        0        0    16186 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/rdial.tcl
+-rw-r--r--   0        0        0    12150 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/tachometer.tcl
+-rw-r--r--   0        0        0    48034 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/vertical_meter.tcl
+-rw-r--r--   0        0        0    11332 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/controlwidget/voltmeter.tcl
+-rw-r--r--   0        0        0    16207 2014-08-11 05:20:11.000000 tkfly-0.1.0a2/tkfly/_tklib/crosshair/crosshair.tcl
+-rw-r--r--   0        0        0      138 2013-05-10 05:18:16.000000 tkfly-0.1.0a2/tkfly/_tklib/crosshair/pkgIndex.tcl
+-rw-r--r--   0        0        0    27293 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ctext/ctext.tcl
+-rw-r--r--   0        0        0       68 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ctext/pkgIndex.tcl
+-rw-r--r--   0        0        0     3924 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/cursor/cursor.tcl
+-rw-r--r--   0        0        0       72 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/cursor/pkgIndex.tcl
+-rw-r--r--   0        0        0    12481 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/datefield/datefield.tcl
+-rw-r--r--   0        0        0       76 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/datefield/pkgIndex.tcl
+-rw-r--r--   0        0        0    12537 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/application.tcl
+-rw-r--r--   0        0        0    10383 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/attributes.tcl
+-rw-r--r--   0        0        0    37096 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/basic.tcl
+-rw-r--r--   0        0        0    32433 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/core.tcl
+-rw-r--r--   0        0        0     1557 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/diagram.tcl
+-rw-r--r--   0        0        0     7807 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/direction.tcl
+-rw-r--r--   0        0        0     7931 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/element.tcl
+-rw-r--r--   0        0        0     3423 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/navigation.tcl
+-rw-r--r--   0        0        0      847 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/pkgIndex.tcl
+-rw-r--r--   0        0        0     4837 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/diagrams/point.tcl
+-rw-r--r--   0        0        0      612 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/getstring/pkgIndex.tcl
+-rw-r--r--   0        0        0     4224 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/getstring/tk_getString.tcl
+-rw-r--r--   0        0        0     3187 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/history/history.tcl
+-rw-r--r--   0        0        0      605 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/history/pkgIndex.tcl
+-rw-r--r--   0        0        0    44954 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ico/ico.tcl
+-rw-r--r--   0        0        0    35176 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ico/ico0.tcl
+-rw-r--r--   0        0        0      292 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ico/pkgIndex.tcl
+-rw-r--r--   0        0        0    29231 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ipentry/ipentry.tcl
+-rw-r--r--   0        0        0      139 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/ipentry/pkgIndex.tcl
+-rw-r--r--   0        0        0     3795 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/cs.msg
+-rw-r--r--   0        0        0     3718 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/da.msg
+-rw-r--r--   0        0        0     4409 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/de.msg
+-rw-r--r--   0        0        0     3918 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/en.msg
+-rw-r--r--   0        0        0     3979 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/es.msg
+-rw-r--r--   0        0        0    56665 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/khim.tcl
+-rw-r--r--   0        0        0      534 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/pkgIndex.tcl
+-rw-r--r--   0        0        0     4124 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/pl.msg
+-rw-r--r--   0        0        0     2937 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/ROOT.msg
+-rw-r--r--   0        0        0     6679 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/ru.msg
+-rw-r--r--   0        0        0     6361 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/khim/uk.msg
+-rw-r--r--   0        0        0      444 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/mentry.tcl
+-rw-r--r--   0        0        0      737 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/mentry_tile.tcl
+-rw-r--r--   0        0        0     2592 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/mentryPublic.tcl
+-rw-r--r--   0        0        0      860 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/pkgIndex.tcl
+-rw-r--r--   0        0        0    25858 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryDateTime.tcl
+-rw-r--r--   0        0        0     4298 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryFixedPoint.tcl
+-rw-r--r--   0        0        0     5661 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryIPAddr.tcl
+-rw-r--r--   0        0        0     6884 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryIPv6Addr.tcl
+-rw-r--r--   0        0        0    18737 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryThemes.tcl
+-rw-r--r--   0        0        0    60325 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryWidget.tcl
+-rw-r--r--   0        0        0    19506 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mwutil.tcl
+-rw-r--r--   0        0        0    10636 2020-01-06 23:27:53.000000 tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/tclIndex
+-rw-r--r--   0        0        0     5469 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/menubar/debug.tcl
+-rw-r--r--   0        0        0    53951 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/menubar/menubar.tcl
+-rw-r--r--   0        0        0     3859 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/menubar/node.tcl
+-rw-r--r--   0        0        0      299 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/menubar/pkgIndex.tcl
+-rw-r--r--   0        0        0    26016 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/menubar/tree.tcl
+-rw-r--r--   0        0        0     4015 2023-04-29 05:27:10.370187 tkfly-0.1.0a2/tkfly/_tklib/notifywindow/notifywindow.tcl
+-rw-r--r--   0        0        0      548 2016-07-14 05:57:54.000000 tkfly-0.1.0a2/tkfly/_tklib/notifywindow/pkgIndex.tcl
+-rw-r--r--   0        0        0   120514 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/ntext/ntext.tcl
+-rw-r--r--   0        0        0      132 2020-02-09 20:50:00.000000 tkfly-0.1.0a2/tkfly/_tklib/ntext/pkgIndex.tcl
+-rw-r--r--   0        0        0    30859 2020-02-09 20:50:00.000000 tkfly-0.1.0a2/tkfly/_tklib/persistentSelection/persistentSelection.tcl
+-rw-r--r--   0        0        0      160 2020-02-09 20:50:00.000000 tkfly-0.1.0a2/tkfly/_tklib/persistentSelection/pkgIndex.tcl
+-rw-r--r--   0        0        0     3291 2023-04-14 12:33:32.365933 tkfly-0.1.0a2/tkfly/_tklib/pkgIndex.tcl
+-rw-r--r--   0        0        0      321 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/pkgIndex.tcl
+-rw-r--r--   0        0        0    13471 2015-04-21 06:10:00.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plot3d.tcl
+-rw-r--r--   0        0        0    15740 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotanim.tcl
+-rw-r--r--   0        0        0    12916 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotannot.tcl
+-rw-r--r--   0        0        0    67951 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotaxis.tcl
+-rw-r--r--   0        0        0     6478 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotbind.tcl
+-rw-r--r--   0        0        0    11059 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotbusiness.tcl
+-rw-r--r--   0        0        0   108162 2019-08-21 18:42:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotchart.tcl
+-rw-r--r--   0        0        0     5721 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotcombined.tcl
+-rw-r--r--   0        0        0    16783 2015-04-21 06:10:00.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotconfig.tcl
+-rw-r--r--   0        0        0    61163 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotcontour.tcl
+-rw-r--r--   0        0        0    10041 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotgantt.tcl
+-rw-r--r--   0        0        0     8895 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotobject.tcl
+-rw-r--r--   0        0        0     9423 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotpack.tcl
+-rw-r--r--   0        0        0   139321 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotpriv.tcl
+-rw-r--r--   0        0        0     8072 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotscada.tcl
+-rw-r--r--   0        0        0     5697 2016-07-14 05:57:54.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotspecial.tcl
+-rw-r--r--   0        0        0     7475 2014-08-11 05:20:12.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotstatustimeline.tcl
+-rw-r--r--   0        0        0     9893 2015-04-21 06:10:00.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/plottable.tcl
+-rw-r--r--   0        0        0     5215 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/scaling.tcl
+-rw-r--r--   0        0        0    16372 2014-11-24 17:34:56.000000 tkfly-0.1.0a2/tkfly/_tklib/plotchart/xyplot.tcl
+-rw-r--r--   0        0        0      867 2022-07-14 16:02:02.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/pkgIndex.tcl
+-rw-r--r--   0        0        0     2420 2022-08-15 11:36:06.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/attrib.tcl
+-rw-r--r--   0        0        0    19506 2020-01-08 04:03:39.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/mwutil.tcl
+-rw-r--r--   0        0        0    16416 2022-04-25 10:54:58.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/notebookImages.tcl
+-rw-r--r--   0        0        0    25675 2022-08-23 17:53:48.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/pagesman.tcl
+-rw-r--r--   0        0        0    53698 2022-08-23 18:08:46.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/plainnotebook.tcl
+-rw-r--r--   0        0        0    36010 2022-08-17 10:02:40.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/scrollableframe.tcl
+-rw-r--r--   0        0        0    36693 2022-08-17 10:03:10.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/scrollarea.tcl
+-rw-r--r--   0        0        0    57949 2022-09-11 08:36:20.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/scrollednotebook.tcl
+-rw-r--r--   0        0        0    18623 2022-08-17 10:05:36.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/scrollsync.tcl
+-rw-r--r--   0        0        0    19056 2022-08-15 19:39:16.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/tclIndex
+-rw-r--r--   0        0        0        0 2022-10-29 06:04:07.908293 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/__init__.py
+-rw-r--r--   0        0        0    21894 2022-05-20 15:38:54.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/mwutil.tcl
+-rw-r--r--   0        0        0      537 2022-10-19 15:21:54.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/pkgIndex.tcl
+-rw-r--r--   0        0        0    22642 2022-05-29 18:19:18.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/scaleutil.tcl
+-rw-r--r--   0        0        0    51787 2022-10-22 15:11:52.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/utils/themepatch.tcl
+-rw-r--r--   0        0        0    27243 2022-04-10 15:20:18.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/wheelEvent.tcl
+-rw-r--r--   0        0        0      686 2022-07-14 16:02:24.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scrollutil.tcl
+-rw-r--r--   0        0        0     1138 2022-07-14 16:03:16.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scrollutil_tile.tcl
+-rw-r--r--   0        0        0     3214 2022-10-18 14:23:10.000000 tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scrollutilCommon.tcl
+-rw-r--r--   0        0        0    15316 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/style/as.tcl
+-rw-r--r--   0        0        0     2848 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/style/lobster.tcl
+-rw-r--r--   0        0        0      684 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/style/pkgIndex.tcl
+-rw-r--r--   0        0        0      765 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/style/style.tcl
+-rw-r--r--   0        0        0      607 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/swaplist/pkgIndex.tcl
+-rw-r--r--   0        0        0    13365 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/swaplist/swaplist.tcl
+-rw-r--r--   0        0        0      898 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/pkgIndex.tcl
+-rw-r--r--   0        0        0    19506 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/mwutil.tcl
+-rw-r--r--   0        0        0     4286 2015-04-21 06:10:00.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/pencil.cur
+-rw-r--r--   0        0        0     2911 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/repair.tcl
+-rw-r--r--   0        0        0   133438 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistBind.tcl
+-rw-r--r--   0        0        0   120387 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistConfig.tcl
+-rw-r--r--   0        0        0    93461 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistEdit.tcl
+-rw-r--r--   0        0        0   125609 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistImages.tcl
+-rw-r--r--   0        0        0    17564 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistMove.tcl
+-rw-r--r--   0        0        0    20512 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistSort.tcl
+-rw-r--r--   0        0        0    68715 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistThemes.tcl
+-rw-r--r--   0        0        0   202524 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistUtil.tcl
+-rw-r--r--   0        0        0   267492 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistWidget.tcl
+-rw-r--r--   0        0        0    62720 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tclIndex
+-rw-r--r--   0        0        0      488 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/tablelist.tcl
+-rw-r--r--   0        0        0      763 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/tablelist_tile.tcl
+-rw-r--r--   0        0        0     3022 2020-01-06 23:27:54.000000 tkfly-0.1.0a2/tkfly/_tklib/tablelist/tablelistPublic.tcl
+-rw-r--r--   0        0        0     4807 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/boxlabel.tcl
+-rw-r--r--   0        0        0     7705 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/canlabel.tcl
+-rw-r--r--   0        0        0     3303 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/labarray.tcl
+-rw-r--r--   0        0        0     1185 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/objselec.tcl
+-rw-r--r--   0        0        0     8331 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/perilabel.tcl
+-rw-r--r--   0        0        0    15130 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/pie.tcl
+-rw-r--r--   0        0        0     1231 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/pielabel.tcl
+-rw-r--r--   0        0        0      154 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/pkgIndex.tcl
+-rw-r--r--   0        0        0     4150 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/relirect.tcl
+-rw-r--r--   0        0        0     4729 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/selector.tcl
+-rw-r--r--   0        0        0    13055 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/slice.tcl
+-rw-r--r--   0        0        0     4728 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/tkpiechart.tcl
+-rw-r--r--   0        0        0      166 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/tooltip/pkgIndex.tcl
+-rw-r--r--   0        0        0     4021 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/tooltip/tipstack.tcl
+-rw-r--r--   0        0        0    14446 2018-05-11 03:56:08.000000 tkfly-0.1.0a2/tkfly/_tklib/tooltip/tooltip.tcl
+-rw-r--r--   0        0        0      427 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/pkgIndex.tcl
+-rw-r--r--   0        0        0     3561 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/tclIndex
+-rw-r--r--   0        0        0    14936 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbCommon.tcl
+-rw-r--r--   0        0        0    11684 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbEntry.tcl
+-rw-r--r--   0        0        0     2174 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbListbox.tcl
+-rw-r--r--   0        0        0     3247 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbTablelist.tcl
+-rw-r--r--   0        0        0     6860 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbText.tcl
+-rw-r--r--   0        0        0     2701 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbTreeview.tcl
+-rw-r--r--   0        0        0     1839 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/wcb/wcb.tcl
+-rw-r--r--   0        0        0     3866 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/arrowb.tcl
+-rw-r--r--   0        0        0    20697 2013-03-26 03:28:23.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/calendar.tcl
+-rw-r--r--   0        0        0    10039 2013-03-26 03:28:23.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/dateentry.tcl
+-rw-r--r--   0        0        0    14200 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/dialog.tcl
+-rw-r--r--   0        0        0     9158 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/mentry.tcl
+-rw-r--r--   0        0        0     6617 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/panelframe.tcl
+-rw-r--r--   0        0        0     1144 2013-03-26 03:28:23.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/pkgIndex.tcl
+-rw-r--r--   0        0        0    18647 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/ruler.tcl
+-rw-r--r--   0        0        0     7563 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/scrollw.tcl
+-rw-r--r--   0        0        0     8025 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/statusbar.tcl
+-rw-r--r--   0        0        0     2093 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/stext.tcl
+-rw-r--r--   0        0        0     3927 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/superframe.tcl
+-rw-r--r--   0        0        0     7915 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widget/toolbar.tcl
+-rw-r--r--   0        0        0     4374 2023-04-29 05:46:59.130164 tkfly-0.1.0a2/tkfly/_tklib/widget/widget.tcl
+-rw-r--r--   0        0        0    32987 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetl/listentry.tcl
+-rw-r--r--   0        0        0    18733 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetl/listsimple.tcl
+-rw-r--r--   0        0        0      237 2019-08-21 18:42:17.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetl/pkgIndex.tcl
+-rw-r--r--   0        0        0      142 2020-02-09 20:50:00.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetPlus/pkgIndex.tcl
+-rw-r--r--   0        0        0    57846 2020-02-09 20:50:00.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetPlus/widgetPlus.tcl
+-rw-r--r--   0        0        0      146 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetv/pkgIndex.tcl
+-rw-r--r--   0        0        0    12031 2013-02-14 03:37:16.000000 tkfly-0.1.0a2/tkfly/_tklib/widgetv/validator.tcl
+-rw-r--r--   0        0        0      224 2023-04-29 07:23:36.893330 tkfly-0.1.0a2/tkfly/_twapi/__init__.py
+-rw-r--r--   0        0        0      677 2023-04-29 07:27:32.485989 tkfly-0.1.0a2/tkfly/_twapi/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    35822 2021-11-07 07:09:24.000000 tkfly-0.1.0a2/tkfly/_twapi/account.tcl
+-rw-r--r--   0        0        0      721 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/adsi.tcl
+-rw-r--r--   0        0        0     3004 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/apputil.tcl
+-rw-r--r--   0        0        0    63943 2021-11-09 02:43:04.000000 tkfly-0.1.0a2/tkfly/_twapi/base.tcl
+-rw-r--r--   0        0        0     7099 2022-06-04 05:48:24.000000 tkfly-0.1.0a2/tkfly/_twapi/clipboard.tcl
+-rw-r--r--   0        0        0   149879 2021-11-02 05:34:50.000000 tkfly-0.1.0a2/tkfly/_twapi/com.tcl
+-rw-r--r--   0        0        0    24031 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/console.tcl
+-rw-r--r--   0        0        0   118653 2022-06-03 06:01:30.000000 tkfly-0.1.0a2/tkfly/_twapi/crypto.tcl
+-rw-r--r--   0        0        0    22667 2022-06-04 15:03:22.000000 tkfly-0.1.0a2/tkfly/_twapi/device.tcl
+-rw-r--r--   0        0        0    51643 2020-10-09 10:08:22.000000 tkfly-0.1.0a2/tkfly/_twapi/etw.tcl
+-rw-r--r--   0        0        0    14722 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/eventlog.tcl
+-rw-r--r--   0        0        0    23130 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/evt.tcl
+-rw-r--r--   0        0        0     7268 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/handle.tcl
+-rw-r--r--   0        0        0    24383 2020-06-24 02:08:54.000000 tkfly-0.1.0a2/tkfly/_twapi/input.tcl
+-rw-r--r--   0        0        0     1480 2019-07-25 11:50:02.000000 tkfly-0.1.0a2/tkfly/_twapi/LICENSE
+-rw-r--r--   0        0        0    23492 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/metoo.tcl
+-rw-r--r--   0        0        0    37265 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/msi.tcl
+-rw-r--r--   0        0        0    22693 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/mstask.tcl
+-rw-r--r--   0        0        0     1793 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/multimedia.tcl
+-rw-r--r--   0        0        0     3535 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/namedpipe.tcl
+-rw-r--r--   0        0        0    37061 2020-10-14 07:59:02.000000 tkfly-0.1.0a2/tkfly/_twapi/network.tcl
+-rw-r--r--   0        0        0    17196 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/nls.tcl
+-rw-r--r--   0        0        0    43660 2022-06-04 00:12:28.000000 tkfly-0.1.0a2/tkfly/_twapi/os.tcl
+-rw-r--r--   0        0        0    34543 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/pdh.tcl
+-rw-r--r--   0        0        0     7293 2022-06-22 13:03:38.000000 tkfly-0.1.0a2/tkfly/_twapi/pkgIndex.tcl
+-rw-r--r--   0        0        0     3758 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/power.tcl
+-rw-r--r--   0        0        0     1802 2020-06-23 03:12:46.000000 tkfly-0.1.0a2/tkfly/_twapi/printer.tcl
+-rw-r--r--   0        0        0    69738 2022-06-03 07:57:36.000000 tkfly-0.1.0a2/tkfly/_twapi/process.tcl
+-rw-r--r--   0        0        0     6602 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/rds.tcl
+-rw-r--r--   0        0        0     2037 2022-06-22 09:04:10.000000 tkfly-0.1.0a2/tkfly/_twapi/README.md
+-rw-r--r--   0        0        0    13900 2022-06-03 13:37:40.000000 tkfly-0.1.0a2/tkfly/_twapi/registry.tcl
+-rw-r--r--   0        0        0    18583 2022-06-04 12:13:10.000000 tkfly-0.1.0a2/tkfly/_twapi/resource.tcl
+-rw-r--r--   0        0        0    76964 2021-11-06 08:18:08.000000 tkfly-0.1.0a2/tkfly/_twapi/security.tcl
+-rw-r--r--   0        0        0    40542 2022-06-04 14:46:44.000000 tkfly-0.1.0a2/tkfly/_twapi/service.tcl
+-rw-r--r--   0        0        0    30062 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/share.tcl
+-rw-r--r--   0        0        0    19297 2020-12-15 00:37:00.000000 tkfly-0.1.0a2/tkfly/_twapi/shell.tcl
+-rw-r--r--   0        0        0    28334 2022-06-04 12:24:36.000000 tkfly-0.1.0a2/tkfly/_twapi/sspi.tcl
+-rw-r--r--   0        0        0    20059 2022-06-05 01:39:28.000000 tkfly-0.1.0a2/tkfly/_twapi/storage.tcl
+-rw-r--r--   0        0        0     2632 2020-07-01 00:57:00.000000 tkfly-0.1.0a2/tkfly/_twapi/synch.tcl
+-rw-r--r--   0        0        0    49870 2022-06-22 10:37:46.000000 tkfly-0.1.0a2/tkfly/_twapi/tls.tcl
+-rw-r--r--   0        0        0    26955 2020-06-22 09:54:26.000000 tkfly-0.1.0a2/tkfly/_twapi/twapi.tcl
+-rw-r--r--   0        0        0   389718 2022-06-22 13:03:36.000000 tkfly-0.1.0a2/tkfly/_twapi/twapi_base.dll
+-rw-r--r--   0        0        0   516096 2022-06-22 12:59:36.000000 tkfly-0.1.0a2/tkfly/_twapi/twapi_base64.dll
+-rw-r--r--   0        0        0    42512 2022-06-04 14:52:14.000000 tkfly-0.1.0a2/tkfly/_twapi/ui.tcl
+-rw-r--r--   0        0        0     4286 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/win.tcl
+-rw-r--r--   0        0        0    10975 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/winlog.tcl
+-rw-r--r--   0        0        0     3148 2022-06-04 03:20:02.000000 tkfly-0.1.0a2/tkfly/_twapi/winsta.tcl
+-rw-r--r--   0        0        0     6978 2019-07-25 11:50:04.000000 tkfly-0.1.0a2/tkfly/_twapi/wmi.tcl
+-rw-r--r--   0        0        0     2217 2023-04-19 11:11:33.981831 tkfly-0.1.0a2/tkfly/core.py
+-rw-r--r--   0        0        0      222 2023-04-14 12:59:16.512351 tkfly-0.1.0a2/tkfly/tkimg/__init__.py
+-rw-r--r--   0        0        0   221710 2022-11-24 07:55:52.000000 tkfly-0.1.0a2/tkfly/tkimg/jpegtcl950.dll
+-rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a2/tkfly/tkimg/libjpegtclstub950.a
+-rw-r--r--   0        0        0     1220 2022-11-24 07:55:44.000000 tkfly-0.1.0a2/tkfly/tkimg/libpngtclstub1638.a
+-rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a2/tkfly/tkimg/libtifftclstub440.a
+-rw-r--r--   0        0        0     1220 2022-11-24 07:55:44.000000 tkfly-0.1.0a2/tkfly/tkimg/libtkimgstub1414.a
+-rw-r--r--   0        0        0     1302 2022-11-24 07:55:44.000000 tkfly-0.1.0a2/tkfly/tkimg/libzlibtclstub1213.a
+-rw-r--r--   0        0        0     6851 2022-11-24 07:55:44.000000 tkfly-0.1.0a2/tkfly/tkimg/pkgIndex.tcl
+-rw-r--r--   0        0        0   231950 2022-11-24 07:55:52.000000 tkfly-0.1.0a2/tkfly/tkimg/pngtcl1638.dll
+-rw-r--r--   0        0        0   416782 2022-11-24 07:55:52.000000 tkfly-0.1.0a2/tkfly/tkimg/tifftcl440.dll
+-rw-r--r--   0        0        0    40462 2022-11-24 07:55:54.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimg1414.dll
+-rw-r--r--   0        0        0    25614 2022-11-24 07:55:54.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgbmp1414.dll
+-rw-r--r--   0        0        0    22030 2022-11-24 07:55:54.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgdted1414.dll
+-rw-r--r--   0        0        0    23566 2022-11-24 07:55:56.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgflir1414.dll
+-rw-r--r--   0        0        0    24590 2022-11-24 07:55:56.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimggif1414.dll
+-rw-r--r--   0        0        0    25614 2022-11-24 07:55:56.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgico1414.dll
+-rw-r--r--   0        0        0    23054 2022-11-24 07:55:56.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgjpeg1414.dll
+-rw-r--r--   0        0        0    23566 2022-11-24 07:55:58.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgpcx1414.dll
+-rw-r--r--   0        0        0    25614 2022-11-24 07:55:58.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgpixmap1414.dll
+-rw-r--r--   0        0        0    23566 2022-11-24 07:55:58.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgpng1414.dll
+-rw-r--r--   0        0        0    25102 2022-11-24 07:56:00.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgppm1414.dll
+-rw-r--r--   0        0        0    21006 2022-11-24 07:56:00.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgps1414.dll
+-rw-r--r--   0        0        0    31758 2022-11-24 07:56:00.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgraw1414.dll
+-rw-r--r--   0        0        0    28174 2022-11-24 07:56:02.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgsgi1414.dll
+-rw-r--r--   0        0        0    25614 2022-11-24 07:56:02.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgsun1414.dll
+-rw-r--r--   0        0        0    25102 2022-11-24 07:56:02.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgtga1414.dll
+-rw-r--r--   0        0        0    70158 2022-11-24 07:56:04.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgtiff1414.dll
+-rw-r--r--   0        0        0    17934 2022-11-24 07:56:04.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgwindow1414.dll
+-rw-r--r--   0        0        0    19470 2022-11-24 07:56:04.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgxbm1414.dll
+-rw-r--r--   0        0        0    23566 2022-11-24 07:56:06.000000 tkfly-0.1.0a2/tkfly/tkimg/tkimgxpm1414.dll
+-rw-r--r--   0        0        0    91662 2022-11-24 07:56:06.000000 tkfly-0.1.0a2/tkfly/tkimg/zlibtcl1213.dll
+-rw-r--r--   0        0        0        0 2023-04-19 11:17:10.457150 tkfly-0.1.0a2/tkfly/tklib/__init__.py
+-rw-r--r--   0        0        0      141 2023-04-19 12:43:56.373512 tkfly-0.1.0a2/tkfly/tklib/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2594 2023-04-29 11:00:59.295786 tkfly-0.1.0a2/tkfly/tklib/__pycache__/datefield.cpython-311.pyc
+-rw-r--r--   0        0        0     8914 2023-04-29 05:02:59.020777 tkfly-0.1.0a2/tkfly/tklib/__pycache__/history.cpython-311.pyc
+-rw-r--r--   0        0        0     3960 2023-04-19 12:45:43.059958 tkfly-0.1.0a2/tkfly/tklib/__pycache__/tooltip.cpython-311.pyc
+-rw-r--r--   0        0        0      538 2023-04-29 05:32:30.677805 tkfly-0.1.0a2/tkfly/tklib/autoscroll.py
+-rw-r--r--   0        0        0      573 2023-04-19 14:52:50.309476 tkfly-0.1.0a2/tkfly/tklib/chatwidget.py
+-rw-r--r--   0        0        0     1265 2023-04-29 10:59:14.922692 tkfly-0.1.0a2/tkfly/tklib/datefield.py
+-rw-r--r--   0        0        0     5389 2023-04-29 05:02:58.918925 tkfly-0.1.0a2/tkfly/tklib/history.py
+-rw-r--r--   0        0        0      583 2023-04-19 12:47:17.815625 tkfly-0.1.0a2/tkfly/tklib/menubar.py
+-rw-r--r--   0        0        0     1002 2023-04-29 05:26:07.066657 tkfly-0.1.0a2/tkfly/tklib/notifywindow.py
+-rw-r--r--   0        0        0     1331 2023-04-29 06:07:26.214511 tkfly-0.1.0a2/tkfly/tklib/plotchart.py
+-rw-r--r--   0        0        0     5389 2023-04-29 05:38:33.820659 tkfly-0.1.0a2/tkfly/tklib/shtmlview.py
+-rw-r--r--   0        0        0     2066 2023-04-19 12:45:42.877555 tkfly-0.1.0a2/tkfly/tklib/tooltip.py
+-rw-r--r--   0        0        0      902 2023-04-19 11:28:27.786655 tkfly-0.1.0a2/tkfly/tklib/wcb.py
+-rw-r--r--   0        0        0      523 2023-04-29 05:46:46.161323 tkfly-0.1.0a2/tkfly/tklib/widget.py
+-rw-r--r--   0        0        0      506 2023-04-29 11:29:28.404486 tkfly-0.1.0a2/tkfly/tkscrollutil/__init__.py
+-rw-r--r--   0        0        0      804 2023-04-29 11:29:28.606524 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1165 2023-04-29 11:09:26.181908 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/attrib.cpython-311.pyc
+-rw-r--r--   0        0        0     1258 2023-04-29 11:29:43.706687 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/load.cpython-311.pyc
+-rw-r--r--   0        0        0     3023 2023-04-29 11:14:55.822881 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/scrollarea.cpython-311.pyc
+-rw-r--r--   0        0        0     4204 2023-04-29 11:12:49.744284 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/scrollsync.cpython-311.pyc
+-rw-r--r--   0        0        0     3011 2023-04-29 11:29:28.610040 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/ttk_scrollarea.cpython-311.pyc
+-rw-r--r--   0        0        0     2069 2023-04-29 11:34:46.885357 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/ttk_scrollednotebook.cpython-311.pyc
+-rw-r--r--   0        0        0     3060 2023-04-29 11:26:17.297437 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/ttk_scrollsync.cpython-311.pyc
+-rw-r--r--   0        0        0     2903 2023-04-29 11:29:28.614038 tkfly-0.1.0a2/tkfly/tkscrollutil/__pycache__/wheelevent.cpython-311.pyc
+-rw-r--r--   0        0        0      413 2022-10-29 06:29:19.142527 tkfly-0.1.0a2/tkfly/tkscrollutil/attrib.py
+-rw-r--r--   0        0        0      458 2023-04-29 11:29:43.603589 tkfly-0.1.0a2/tkfly/tkscrollutil/load.py
+-rw-r--r--   0        0        0     1886 2023-04-29 11:24:25.427936 tkfly-0.1.0a2/tkfly/tkscrollutil/scrollableframe.py
+-rw-r--r--   0        0        0     1921 2023-04-29 11:14:55.722630 tkfly-0.1.0a2/tkfly/tkscrollutil/scrollarea.py
+-rw-r--r--   0        0        0     2480 2023-04-29 11:10:41.419659 tkfly-0.1.0a2/tkfly/tkscrollutil/scrollsync.py
+-rw-r--r--   0        0        0     1910 2023-04-29 11:29:28.409999 tkfly-0.1.0a2/tkfly/tkscrollutil/ttk_scrollarea.py
+-rw-r--r--   0        0        0     1142 2023-04-29 11:34:46.766705 tkfly-0.1.0a2/tkfly/tkscrollutil/ttk_scrollednotebook.py
+-rw-r--r--   0        0        0     1689 2023-04-29 11:26:17.197236 tkfly-0.1.0a2/tkfly/tkscrollutil/ttk_scrollsync.py
+-rw-r--r--   0        0        0     1435 2023-04-29 11:28:26.430882 tkfly-0.1.0a2/tkfly/tkscrollutil/wheelevent.py
+-rw-r--r--   0        0        0      544 2023-04-29 11:43:18.104764 tkfly-0.1.0a2/tkfly/twapi/__init__.py
+-rw-r--r--   0        0        0     1464 2023-04-29 11:43:18.209994 tkfly-0.1.0a2/tkfly/twapi/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      359 2023-04-29 07:58:45.679468 tkfly-0.1.0a2/tkfly/twapi/base.py
+-rw-r--r--   0        0        0      230 2023-04-29 07:58:45.713014 tkfly-0.1.0a2/tkfly/twapi/msi.py
+-rw-r--r--   0        0        0      704 2023-04-29 10:07:46.018924 tkfly-0.1.0a2/tkfly/twapi/ui.py
+-rw-r--r--   0        0        0      585 2023-04-29 08:16:43.020235 tkfly-0.1.0a2/tkfly/twapi/win.py
+-rw-r--r--   0        0        0     6773 1970-01-01 00:00:00.000000 tkfly-0.1.0a2/PKG-INFO
```

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/__pycache__/__init__.cpython-311.pyc` & `tkfly-0.1.0a2/tkfly/_tklib/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/__pycache__/__init__.cpython-312.pyc` & `tkfly-0.1.0a2/tkfly/_tklib/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/autoscroll/autoscroll.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/autoscroll/autoscroll.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/autoscroll/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/autoscroll/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_drag.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_drag.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_epoints.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_epoints.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_epolyline.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_epolyline.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_equad.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_equad.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_gradient.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_gradient.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_highlight.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_highlight.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_mvg.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_mvg.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_snap.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_snap.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_sqmap.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_sqmap.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_tags.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_tags.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_trlines.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_trlines.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/canvas/canvas_zoom.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/canvas/canvas_zoom.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/canvas/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/canvas/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/chatwidget/chatwidget.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/chatwidget/chatwidget.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/controlwidget/bindDown.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/bindDown.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/controlwidget/led.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/led.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/controlwidget/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/controlwidget/radioMatrix.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/radioMatrix.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/controlwidget/rdial.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/rdial.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/controlwidget/tachometer.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/tachometer.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/controlwidget/vertical_meter.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/vertical_meter.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/controlwidget/voltmeter.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/controlwidget/voltmeter.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/crosshair/crosshair.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/crosshair/crosshair.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/ctext/ctext.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/ctext/ctext.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/cursor/cursor.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/cursor/cursor.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/datefield/datefield.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/datefield/datefield.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/diagrams/application.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/diagrams/application.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/diagrams/attributes.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/diagrams/attributes.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/diagrams/basic.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/diagrams/basic.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/diagrams/core.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/diagrams/core.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/diagrams/diagram.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/diagrams/diagram.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/diagrams/direction.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/diagrams/direction.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/diagrams/element.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/diagrams/element.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/diagrams/navigation.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/diagrams/navigation.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/diagrams/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/diagrams/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/diagrams/point.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/diagrams/point.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/getstring/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/getstring/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/getstring/tk_getString.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/getstring/tk_getString.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/history/history.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/history/history.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/history/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/history/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/ico/ico.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/ico/ico.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/ico/ico0.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/ico/ico0.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/ipentry/ipentry.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/ipentry/ipentry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/khim/cs.msg` & `tkfly-0.1.0a2/tkfly/_tklib/khim/cs.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/khim/da.msg` & `tkfly-0.1.0a2/tkfly/_tklib/khim/da.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/khim/de.msg` & `tkfly-0.1.0a2/tkfly/_tklib/khim/de.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/khim/en.msg` & `tkfly-0.1.0a2/tkfly/_tklib/khim/en.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/khim/es.msg` & `tkfly-0.1.0a2/tkfly/_tklib/khim/es.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/khim/khim.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/khim/khim.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/khim/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/khim/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/khim/pl.msg` & `tkfly-0.1.0a2/tkfly/_tklib/khim/pl.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/khim/ROOT.msg` & `tkfly-0.1.0a2/tkfly/_tklib/khim/ROOT.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/khim/ru.msg` & `tkfly-0.1.0a2/tkfly/_tklib/khim/ru.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/khim/uk.msg` & `tkfly-0.1.0a2/tkfly/_tklib/khim/uk.msg`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/mentry/mentry_tile.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/mentry/mentry_tile.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/mentry/mentryPublic.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/mentry/mentryPublic.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/mentry/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/mentry/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mentryDateTime.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryDateTime.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mentryFixedPoint.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryFixedPoint.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mentryIPAddr.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryIPAddr.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mentryIPv6Addr.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryIPv6Addr.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mentryThemes.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryThemes.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mentryWidget.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mentryWidget.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/mwutil.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/mwutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/mentry/scripts/tclIndex` & `tkfly-0.1.0a2/tkfly/_tklib/mentry/scripts/tclIndex`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/menubar/debug.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/menubar/debug.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/menubar/menubar.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/menubar/menubar.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/menubar/node.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/menubar/node.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/menubar/tree.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/menubar/tree.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/notifywindow/notifywindow.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/notifywindow/notifywindow.tcl`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 	}
 	message $w.message -aspect 150 -bg gray30 -fg white -aspect 150 -text $msg -width 280
 	pack $w.message -side right -fill both -expand yes
 	if {[tk windowingsystem] eq "x11"} {
 	    wm overrideredirect $w true
 	}
 	wm attributes $w -alpha 0.0
-	puts [winfo reqwidth $w]
 	set xpos [expr [winfo screenwidth $w] - 325]
 	wm geometry $w +$xpos+30
 	notifywindow::fade_in $w
 	after 3000 notifywindow::fade_out $w
     }
 
     #Fade and destroy window
```

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/notifywindow/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/notifywindow/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/ntext/ntext.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/ntext/ntext.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/persistentSelection/persistentSelection.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/persistentSelection/persistentSelection.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plot3d.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plot3d.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotanim.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotanim.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotannot.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotannot.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotaxis.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotaxis.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotbind.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotbind.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotbusiness.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotbusiness.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotchart.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotchart.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotcombined.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotcombined.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotconfig.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotconfig.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotcontour.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotcontour.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotgantt.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotgantt.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotobject.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotobject.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotpack.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotpack.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotpriv.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotpriv.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotscada.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotscada.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotspecial.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotspecial.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plotstatustimeline.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plotstatustimeline.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/plottable.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/plottable.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/scaling.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/scaling.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/plotchart/xyplot.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/plotchart/xyplot.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/scrollutil/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/pkgIndex.tcl`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-#==============================================================================
-# Scrollutil and Scrollutil_tile package index file.
-#
-# Copyright (c) 2019-2020  Csaba Nemethi (E-mail: csaba.nemethi@t-online.de)
-#==============================================================================
-
-#
-# Regular packages:
-#
-package ifneeded scrollutil         1.5 \
-	[list source [file join $dir scrollutil.tcl]]
-package ifneeded scrollutil_tile    1.5 \
-	[list source [file join $dir scrollutil_tile.tcl]]
-
-#
-# Aliases:
-#
-package ifneeded Scrollutil         1.5 \
-	[list package require -exact scrollutil      1.5]
-package ifneeded Scrollutil_tile    1.5 \
-	[list package require -exact scrollutil_tile 1.5]
-
-#
-# Code common to all packages:
-#
-package ifneeded scrollutil::common 1.5 \
-	[list source [file join $dir scrollutilCommon.tcl]]
+#==============================================================================
+# Scrollutil and Scrollutil_tile package index file.
+#
+# Copyright (c) 2019-2022  Csaba Nemethi (E-mail: csaba.nemethi@t-online.de)
+#==============================================================================
+
+#
+# Regular packages:
+#
+package ifneeded scrollutil         1.17 \
+	[list source [file join $dir scrollutil.tcl]]
+package ifneeded scrollutil_tile    1.17 \
+	[list source [file join $dir scrollutil_tile.tcl]]
+
+#
+# Aliases:
+#
+package ifneeded Scrollutil         1.17 \
+	[list package require -exact scrollutil      1.17]
+package ifneeded Scrollutil_tile    1.17 \
+	[list package require -exact scrollutil_tile 1.17]
+
+#
+# Code common to all packages:
+#
+package ifneeded scrollutil::common 1.17 \
+	[list source [file join $dir scrollutilCommon.tcl]]
```

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/scrollutil/scripts/mwutil.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/mwutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/scrollutil/scripts/scrollsync.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scripts/scrollsync.tcl`

 * *Files 27% similar despite different names*

```diff
@@ -1,603 +1,625 @@
-#==============================================================================
-# Contains the implementation of the scrollsync widget.
-#
-# Structure of the module:
-#   - Namespace initialization
-#   - Private procedure creating the default bindings
-#   - Public procedures creating or quering a scrollsync widget
-#   - Private configuration procedures
-#   - Private procedures implementing the scrollsync widget command
-#   - Private callback procedure
-#   - Private procedures used in bindings
-#   - Private utility procedures
-#
-# Copyright (c) 2019-2020  Csaba Nemethi (E-mail: csaba.nemethi@t-online.de)
-#==============================================================================
-
-#
-# Namespace initialization
-# ========================
-#
-
-namespace eval scrollutil::ss {
-    #
-    # The array configSpecs is used to handle configuration options.  The names
-    # of its elements are the configuration options for the Scrollsync class.
-    # The value of an array element is either an alias name or a list
-    # containing the database name and class as well as an indicator specifying
-    # the widget to which the option applies: f stands for the frame and w for
-    # the scrollsync widget itself.
-    #
-    #	Command-Line Name	 {Database Name		  Database Class     W}
-    #	-----------------------------------------------------------------------
-    #
-    variable configSpecs
-    array set configSpecs {
-	-background		{background		Background	     f}
-	-bg			-background
-	-borderwidth		{borderWidth		BorderWidth	     f}
-	-bd			-borderwidth
-	-cursor			{cursor			Cursor		     f}
-	-highlightbackground	{highlightBackground	HighlightBackground  f}
-	-highlightcolor		{highlightColor		HighlightColor	     f}
-	-highlightthickness	{highlightThickness	HighlightThickness   f}
-	-relief			{relief			Relief		     f}
-	-takefocus		{takeFocus		TakeFocus	     f}
-	-xscrollcommand		{xScrollCommand		ScrollCommand	     w}
-	-yscrollcommand		{yScrollCommand		ScrollCommand	     w}
-    }
-
-    #
-    # Extend the elements of the array configSpecs
-    #
-    proc extendConfigSpecs {} {
-	variable ::scrollutil::usingTile
-	variable configSpecs
-
-	if {$usingTile} {
-	    foreach opt {-background -bg -highlightbackground -highlightcolor
-			 -highlightthickness} {
-		unset configSpecs($opt)
-	    }
-	} else {
-	    set helpFrm .__helpFrm
-	    for {set n 2} {[winfo exists $helpFrm]} {incr n} {
-		set helpFrm .__helpFrm$n
-	    }
-	    tk::frame $helpFrm
-	    foreach opt {-background -highlightbackground -highlightcolor
-			 -highlightthickness} {
-		set configSet [$helpFrm configure $opt]
-		lappend configSpecs($opt) [lindex $configSet 3]
-	    }
-	    destroy $helpFrm
-	}
-
-	lappend configSpecs(-borderwidth) 0
-	lappend configSpecs(-cursor) ""
-	lappend configSpecs(-relief) flat
-	lappend configSpecs(-takefocus) 0
-	lappend configSpecs(-xscrollcommand) ""
-	lappend configSpecs(-yscrollcommand) ""
-    }
-    extendConfigSpecs 
-
-    variable configOpts [lsort [array names configSpecs]]
-
-    #
-    # Use a list to facilitate the handling of the command options
-    #
-    variable cmdOpts [list cget configure setwidgets widgets xview yview]
-}
-
-#
-# Private procedure creating the default bindings
-# ===============================================
-#
-
-#------------------------------------------------------------------------------
-# scrollutil::ss::createBindings
-#
-# Creates the default bindings for the binding tags Scrollsync and
-# WidgetOfScrollsync.
-#------------------------------------------------------------------------------
-proc scrollutil::ss::createBindings {} {
-    bind Scrollsync <KeyPress> continue
-    bind Scrollsync <FocusIn> {
-        if {[string compare [focus -lastfor %W] %W] == 0} {
-            focus [lindex [%W widgets] 0]
-        }
-    }
-    bind Scrollsync <Configure> {
-	after 50 [list scrollutil::ss::updateMasterWidgets %W]
-    }
-    bind Scrollsync <Destroy> {
-	namespace delete scrollutil::ns%W
-	catch {rename %W ""}
-    }
-
-    bind WidgetOfScrollsync <Destroy> {
-	scrollutil::ss::onWidgetOfScrollsyncDestroy %W
-    }
-}
-
-#
-# Public procedures creating or quering a scrollsync widget
-# =========================================================
-#
-
-#------------------------------------------------------------------------------
-# scrollutil::scrollsync
-#
-# Creates a new scrollsync widget whose name is specified as the first command-
-# line argument, and configures it according to the options and their values
-# given on the command line.  Returns the name of the newly created widget.
-#------------------------------------------------------------------------------
-proc scrollutil::scrollsync args {
-    variable usingTile
-    variable ss::configSpecs
-    variable ss::configOpts
-
-    if {[llength $args] == 0} {
-	mwutil::wrongNumArgs "scrollsync pathName ?options?"
-    }
-
-    #
-    # Create a frame of the class Scrollsync
-    #
-    set win [lindex $args 0]
-    if {[catch {
-	if {$usingTile} {
-	    ttk::frame $win -class Scrollsync -padding 0
-	} else {
-	    tk::frame $win -class Scrollsync -container 0
-	    catch {$win configure -padx 0 -pady 0}
-	}
-	$win configure -height 0 -width 0
-    } result] != 0} {
-	return -code error $result
-    }
-
-    #
-    # Create a namespace within the current one to hold the data of the widget
-    #
-    namespace eval ns$win {
-	#
-	# The folowing array holds various data for this widget
-	#
-	variable data
-	array set data {
-	    xView		{-1 -1}
-	    yView		{-1 -1}
-	    xViewLocked		0
-	    yViewLocked		0
-	    widgetList		{}
-	    xScrollableList	{}
-	    yScrollableList	{}
-	}
-    }
-
-    #
-    # Initialize some further components of data
-    #
-    upvar ::scrollutil::ns${win}::data data
-    foreach opt $configOpts {
-	set data($opt) [lindex $configSpecs($opt) 3]
-    }
-
-    #
-    # Configure the widget according to the command-line
-    # arguments and to the available database options
-    #
-    if {[catch {
-	mwutil::configureWidget $win configSpecs scrollutil::ss::doConfig \
-				scrollutil::ss::doCget [lrange $args 1 end] 1
-    } result] != 0} {
-	destroy $win
-	return -code error $result
-    }
-
-    #
-    # Move the original widget command into the namespace ss within the current
-    # one and create an alias of the original name for a new widget procedure
-    #
-    rename ::$win ss::$win
-    interp alias {} ::$win {} scrollutil::ss::scrollsyncWidgetCmd $win
-
-    return $win
-}
-
-#------------------------------------------------------------------------------
-# scrollutil::getscrollsync
-#
-# Queries the scrollsync into which a given widget is embedded via the
-# scrollsync's setwidgets subcommand.
-#------------------------------------------------------------------------------
-proc scrollutil::getscrollsync widget {
-    variable ss::scrollsyncArr
-    if {[info exists scrollsyncArr($widget)]} {
-	set win $scrollsyncArr($widget)
-	if {[winfo exists $win] &&
-	    [string compare [winfo class $win] "Scrollsync"] == 0} {
-	    return $win
-	}
-    }
-
-    return ""
-}
-
-#
-# Private configuration procedures
-# ================================
-#
-
-#------------------------------------------------------------------------------
-# scrollutil::ss::doConfig
-#
-# Applies the value val of the configuration option opt to the scrollsync
-# widget win.
-#------------------------------------------------------------------------------
-proc scrollutil::ss::doConfig {win opt val} {
-    variable configSpecs
-    upvar ::scrollutil::ns${win}::data data
-
-    #
-    # Apply the value to the widget corresponding to the given option
-    #
-    switch [lindex $configSpecs($opt) 2] {
-	f {
-	    #
-	    # Apply the value to the frame and save the
-	    # properly formatted value of val in data($opt)
-	    #
-	    $win configure $opt $val
-	    set data($opt) [$win cget $opt]
-	}
-
-	w {
-	    switch -- $opt {
-		-xscrollcommand {
-		    set data($opt) $val
-		    set data(xView) {-1 -1}
-		}
-		-yscrollcommand {
-		    set data($opt) $val
-		    set data(yView) {-1 -1}
-		}
-	    }
-	}
-    }
-}
-
-#------------------------------------------------------------------------------
-# scrollutil::ss::doCget
-#
-# Returns the value of the configuration option opt for the scrollsync widget
-# win.
-#------------------------------------------------------------------------------
-proc scrollutil::ss::doCget {win opt} {
-    upvar ::scrollutil::ns${win}::data data
-    return $data($opt)
-}
-
-#
-# Private procedures implementing the scrollsync widget command
-# =============================================================
-#
-
-#------------------------------------------------------------------------------
-# scrollutil::ss::scrollsyncWidgetCmd
-#
-# Processes the Tcl command corresponding to a scrollsync widget.
-#------------------------------------------------------------------------------
-proc scrollutil::ss::scrollsyncWidgetCmd {win args} {
-    set argCount [llength $args]
-    if {$argCount == 0} {
-	mwutil::wrongNumArgs "$win option ?arg arg ...?"
-    }
-
-    variable cmdOpts
-    set cmd [mwutil::fullOpt "option" [lindex $args 0] $cmdOpts]
-    switch $cmd {
-	cget {
-	    if {$argCount != 2} {
-		mwutil::wrongNumArgs "$win $cmd option"
-	    }
-
-	    #
-	    # Return the value of the specified configuration option
-	    #
-	    upvar ::scrollutil::ns${win}::data data
-	    variable configSpecs
-	    set opt [mwutil::fullConfigOpt [lindex $args 1] configSpecs]
-	    return $data($opt)
-	}
-
-	configure {
-	    variable configSpecs
-	    return [mwutil::configureSubCmd $win configSpecs \
-		    scrollutil::ss::doConfig scrollutil::ss::doCget \
-		    [lrange $args 1 end]]
-	}
-
-	setwidgets {
-	    if {$argCount != 2} {
-		mwutil::wrongNumArgs "$win $cmd widgetList"
-	    }
-
-	    return [setwidgetsSubCmd $win [lindex $args 1]]
-	}
-
-	widgets {
-	    if {$argCount != 1} {
-		mwutil::wrongNumArgs "$win $cmd"
-	    }
-
-	    upvar ::scrollutil::ns${win}::data data
-	    return $data(widgetList)
-	}
-
-	xview { return [viewSubCmd $win x [lrange $args 1 end]] }
-
-	yview { return [viewSubCmd $win y [lrange $args 1 end]] }
-    }
-}
-
-#------------------------------------------------------------------------------
-# scrollutil::ss::setwidgetsSubCmd
-#
-# Processes the scrollsync setwidgets subcommmand.
-#------------------------------------------------------------------------------
-proc scrollutil::ss::setwidgetsSubCmd {win widgetList} {
-    foreach w $widgetList {
-	if {![winfo exists $w]} {
-	    return -code error "bad window path name \"$w\""
-	}
-
-	set ss [::scrollutil::getscrollsync $w]
-	if {[string length $ss] != 0 && [string compare $ss $win] != 0} {
-	    return -code error "widget $w already in another scrollsync $ss"
-	}
-    }
-
-    variable scrollsyncArr
-    variable xViewArr
-    variable yViewArr
-    upvar ::scrollutil::ns${win}::data data
-
-    set oldWidgetList $data(widgetList)
-    foreach w $oldWidgetList {
-	if {[winfo exists $w]} {
-	    set tagList [bindtags $w]
-	    set idx [lsearch -exact $tagList "WidgetOfScrollsync"]
-	    bindtags $w [lreplace $tagList $idx $idx]
-	}
-
-	if {[info exists scrollsyncArr($w)]} {
-	    unset scrollsyncArr($w)
-	}
-	if {[info exists xViewArr($w)]} {
-	    unset xViewArr($w)
-	}
-	if {[info exists yViewArr($w)]} {
-	    unset yViewArr($w)
-	}
-    }
-
-    array set data {xScrollableList {}  yScrollableList {}}
-
-    foreach w $widgetList {
-	set tagList [bindtags $w]
-	set idx [lsearch -exact $tagList "WidgetOfScrollsync"]
-	if {$idx < 0} {
-	    bindtags $w [linsert $tagList 1 WidgetOfScrollsync]
-	}
-
-	set scrollsyncArr($w) $win
-
-	foreach axis {x y} {
-	    if {[mwutil::isScrollable $w $axis]} {
-		lappend data(${axis}ScrollableList) $w
-		set ${axis}ViewArr($w) {-1 -1}
-		::$w ${axis}view moveto 0
-		::$w configure -${axis}scrollcommand \
-		    [list scrollutil::ss::scrollCmd $win $w $axis]
-	    }
-	}
-
-    }
-
-    set data(widgetList) $widgetList
-    return $oldWidgetList
-}
-
-#------------------------------------------------------------------------------
-# scrollutil::ss::viewSubCmd
-#
-# Processes the scrollsync xview and yview subcommmands.
-#------------------------------------------------------------------------------
-proc scrollutil::ss::viewSubCmd {win axis argList} {
-    upvar ::scrollutil::ns${win}::data data
-    set masterWidget [lindex $data(${axis}ScrollableList) 0]
-    set viewCmd ${axis}view
-
-    switch [llength $argList] {
-	0 {
-	    #
-	    # Command: $win (x|y)view
-	    #
-	    if {[string length $masterWidget] == 0} {
-		return [list 0 1]
-	    } else {
-		return [::$masterWidget $viewCmd]
-	    }
-	}
-
-	default {
-	    #
-	    # Command: $win (x|y)view moveto <fraction>
-	    #	       $win (x|y)view scroll <number> units|pages
-	    #
-	    set argList [mwutil::getScrollInfo2 "$win $viewCmd" $argList]
-	    if {[string length $masterWidget] != 0} {
-		eval [list ::$masterWidget] $viewCmd $argList
-	    }
-	    return ""
-	}
-    }
-}
-
-#
-# Private callback procedure
-# ==========================
-#
-
-#------------------------------------------------------------------------------
-# scrollutil::ss::scrollCmd
-#
-# Propagates the horizontal/vertical position of the view of a given widget
-# within the scrollsync widget win to the other horizontally/vertically
-# scrollable widgets and passes the data of the master widget's view to the
-# value of the -xscrollcommand/-yscrollcommand option.
-#------------------------------------------------------------------------------
-proc scrollutil::ss::scrollCmd {win widget axis first last} {
-    #
-    # Avoid a potential endless loop by making sure that
-    # the view's horizontal/vertical position will only be
-    # propagated to the other widgets if it has changed
-    #
-    variable ${axis}ViewArr
-    set view [set ${axis}ViewArr($widget)]
-    foreach {firstOld lastOld} $view {}
-    if {$first == $firstOld && $last == $lastOld} {
-	return ""
-    } else {
-	set ${axis}ViewArr($widget) [list $first $last]
-    }
-
-    set masterWidget [sortScrollableList $win $axis]
-    set isMasterWidget [expr {[string compare $widget $masterWidget] == 0}]
-    upvar ::scrollutil::ns${win}::data data
-    if {$data(${axis}ViewLocked) && !$isMasterWidget} {
-	return ""
-    }
-
-    foreach w $data(${axis}ScrollableList) {
-	if {[string compare $w $widget] == 0} {
-	    continue
-	}
-
-	if {$first != 0 && $last == 1} {
-	    ::$w ${axis}view moveto 1
-	} else {
-	    ::$w ${axis}view moveto $first
-	}
-    }
-
-    if {$isMasterWidget && [string length $data(-${axis}scrollcommand)] != 0} {
-	foreach {firstOld lastOld} $data(${axis}View) {}
-	if {$first != $firstOld || $last != $lastOld} {
-	    set data(${axis}View) [list $first $last]
-	    eval $data(-${axis}scrollcommand) $first $last
-	}
-    }
-
-    set data(${axis}ViewLocked) 1
-    after 1 [list scrollutil::ss::unlockView $win $axis]
-}
-
-#
-# Private procedures used in bindings
-# ===================================
-#
-
-#------------------------------------------------------------------------------
-# scrollutil::ss::updateMasterWidgets
-#------------------------------------------------------------------------------
-proc scrollutil::ss::updateMasterWidgets win {
-    if {![winfo exists $win] ||
-	[string compare [winfo class $win] "Scrollsync"] != 0} {
-	return ""
-    }
-
-    upvar ::scrollutil::ns${win}::data data
-    foreach axis {x y} {
-	set masterWidget [sortScrollableList $win $axis]
-	if {[string length $masterWidget] != 0 &&
-	    [string length $data(-${axis}scrollcommand)] != 0} {
-	    eval $data(-${axis}scrollcommand) [::$masterWidget ${axis}view]
-	}
-    }
-}
-
-#------------------------------------------------------------------------------
-# scrollutil::ss::onWidgetOfScrollsyncDestroy
-#------------------------------------------------------------------------------
-proc scrollutil::ss::onWidgetOfScrollsyncDestroy widget {
-    variable scrollsyncArr
-    if {[info exists scrollsyncArr($widget)]} {
-	unset scrollsyncArr($widget)
-    }
-
-    variable xViewArr
-    if {[info exists xViewArr($widget)]} {
-	unset xViewArr($widget)
-    }
-
-    variable yViewArr
-    if {[info exists yViewArr($widget)]} {
-	unset yViewArr($widget)
-    }
-
-    set win [::scrollutil::getscrollsync $widget]
-    if {[string length $win] != 0} {
-	set widgetList [::$win widgets]
-	set idx [lsearch -exact $widgetList $widget]
-	::$win setwidgets [lreplace $widgetList $idx $idx]
-    }
-}
-
-#
-# Private utility procedures
-# ==========================
-#
-
-#------------------------------------------------------------------------------
-# scrollutil::ss::sortScrollableList
-#------------------------------------------------------------------------------
-proc scrollutil::ss::sortScrollableList {win axis} {
-    upvar ::scrollutil::ns${win}::data data
-    set data(${axis}ScrollableList) \
-	[lsort -command "compareViews $axis" $data(${axis}ScrollableList)]
-    return [lindex $data(${axis}ScrollableList) 0]
-}
-
-#------------------------------------------------------------------------------
-# scrollutil::ss::compareViews
-#------------------------------------------------------------------------------
-proc scrollutil::ss::compareViews {axis w1 w2} {
-    foreach {first1 last1} [::$w1 ${axis}view] {}
-    foreach {first2 last2} [::$w2 ${axis}view] {}
-    set frac1 [expr {$last1 - $first1}]
-    set frac2 [expr {$last2 - $first2}]
-    set diff  [expr {$frac1 - $frac2}]
-
-    if {abs($diff) < 1.0e-15} {
-	return 0
-    } elseif {$diff < 0} {
-	return -1
-    } else {
-	return 1
-    }
-}
-
-#------------------------------------------------------------------------------
-# scrollutil::ss::unlockView
-#------------------------------------------------------------------------------
-proc scrollutil::ss::unlockView {win axis} {
-    if {[winfo exists $win] &&
-	[string compare [winfo class $win] "Scrollsync"] == 0} {
-	upvar ::scrollutil::ns${win}::data data
-	set data(${axis}ViewLocked) 0
-    }
-}
+#==============================================================================
+# Contains the implementation of the scrollsync widget.
+#
+# Structure of the module:
+#   - Namespace initialization
+#   - Private procedure creating the default bindings
+#   - Public procedures creating or querying a scrollsync widget
+#   - Private configuration procedures
+#   - Private procedures implementing the scrollsync widget command
+#   - Private callback procedure
+#   - Private procedures used in bindings
+#   - Private utility procedures
+#
+# Copyright (c) 2019-2022  Csaba Nemethi (E-mail: csaba.nemethi@t-online.de)
+#==============================================================================
+
+#
+# Namespace initialization
+# ========================
+#
+
+namespace eval scrollutil::ss {
+    #
+    # The array configSpecs is used to handle configuration options.  The names
+    # of its elements are the configuration options for the Scrollsync class.
+    # The value of an array element is either an alias name or a list
+    # containing the database name and class as well as an indicator specifying
+    # the widget to which the option applies: f stands for the frame and w for
+    # the scrollsync widget itself.
+    #
+    #	Command-Line Name	{Database Name		Database Class       W}
+    #	-----------------------------------------------------------------------
+    #
+    variable configSpecs
+    array set configSpecs {
+	-background		{background		Background	     f}
+	-bg			-background
+	-borderwidth		{borderWidth		BorderWidth	     f}
+	-bd			-borderwidth
+	-cursor			{cursor			Cursor		     f}
+	-highlightbackground	{highlightBackground	HighlightBackground  f}
+	-highlightcolor		{highlightColor		HighlightColor	     f}
+	-highlightthickness	{highlightThickness	HighlightThickness   f}
+	-relief			{relief			Relief		     f}
+	-takefocus		{takeFocus		TakeFocus	     f}
+	-xscrollcommand		{xScrollCommand		ScrollCommand	     w}
+	-yscrollcommand		{yScrollCommand		ScrollCommand	     w}
+    }
+
+    #
+    # Extend the elements of the array configSpecs
+    #
+    proc extendConfigSpecs {} {
+	variable ::scrollutil::usingTile
+	variable configSpecs
+
+	if {$usingTile} {
+	    foreach opt {-background -bg -highlightbackground -highlightcolor
+			 -highlightthickness} {
+		unset configSpecs($opt)
+	    }
+	} else {
+	    set helpFrm .__helpFrm
+	    for {set n 2} {[winfo exists $helpFrm]} {incr n} {
+		set helpFrm .__helpFrm$n
+	    }
+	    tk::frame $helpFrm
+	    foreach opt {-background -highlightbackground -highlightcolor
+			 -highlightthickness} {
+		set configSet [$helpFrm configure $opt]
+		lappend configSpecs($opt) [lindex $configSet 3]
+	    }
+	    destroy $helpFrm
+	}
+
+	lappend configSpecs(-borderwidth)	0
+	lappend configSpecs(-cursor)		""
+	lappend configSpecs(-relief)		flat
+	lappend configSpecs(-takefocus)		0
+	lappend configSpecs(-xscrollcommand)	""
+	lappend configSpecs(-yscrollcommand)	""
+    }
+    extendConfigSpecs
+
+    variable configOpts [lsort [array names configSpecs]]
+
+    #
+    # Use a list to facilitate the handling of the command options
+    #
+    variable cmdOpts [list attrib cget configure hasattrib setwidgets \
+		      unsetattrib widgets xview yview]
+}
+
+#
+# Private procedure creating the default bindings
+# ===============================================
+#
+
+#------------------------------------------------------------------------------
+# scrollutil::ss::createBindings
+#
+# Creates the default bindings for the binding tags Scrollsync and
+# WidgetOfScrollsync.
+#------------------------------------------------------------------------------
+proc scrollutil::ss::createBindings {} {
+    bind Scrollsync <KeyPress> continue
+    bind Scrollsync <FocusIn> {
+        if {[string compare [focus -lastfor %W] %W] == 0} {
+            focus [lindex [%W widgets] 0]
+        }
+    }
+    bind Scrollsync <Configure> {
+	after 50 [list scrollutil::ss::updateMasterWidgets %W]
+    }
+    bind Scrollsync <Destroy> {
+	namespace delete scrollutil::ns%W
+	catch {rename %W ""}
+    }
+
+    bind WidgetOfScrollsync <Destroy> {
+	scrollutil::ss::onWidgetOfScrollsyncDestroy %W
+    }
+}
+
+#
+# Public procedures creating or querying a scrollsync widget
+# ==========================================================
+#
+
+#------------------------------------------------------------------------------
+# scrollutil::scrollsync
+#
+# Creates a new scrollsync widget whose name is specified as the first command-
+# line argument, and configures it according to the options and their values
+# given on the command line.  Returns the name of the newly created widget.
+#------------------------------------------------------------------------------
+proc scrollutil::scrollsync args {
+    variable usingTile
+    variable ss::configSpecs
+    variable ss::configOpts
+
+    if {[llength $args] == 0} {
+	mwutil::wrongNumArgs "scrollsync pathName ?options?"
+    }
+
+    #
+    # Create a frame of the class Scrollsync
+    #
+    set win [lindex $args 0]
+    if {[catch {
+	if {$usingTile} {
+	    ttk::frame $win -class Scrollsync -padding 0
+	} else {
+	    tk::frame $win -class Scrollsync -container 0
+	    catch {$win configure -padx 0 -pady 0}
+	}
+	$win configure -height 0 -width 0
+    } result] != 0} {
+	return -code error $result
+    }
+
+    #
+    # Create a namespace within the current one to hold the data of the widget
+    #
+    namespace eval ns$win {
+	#
+	# The folowing array holds various data for this widget
+	#
+	variable data
+	array set data {
+	    xView		{-1 -1}
+	    yView		{-1 -1}
+	    xViewLocked		0
+	    yViewLocked		0
+	    widgetList		{}
+	    xScrollableList	{}
+	    yScrollableList	{}
+	}
+
+	#
+	# The following array is used to hold
+	# arbitrary attributes for this widget
+	#
+	variable attribs
+    }
+
+    #
+    # Initialize some further components of data
+    #
+    upvar ::scrollutil::ns${win}::data data
+    foreach opt $configOpts {
+	set data($opt) [lindex $configSpecs($opt) 3]
+    }
+
+    #
+    # Configure the widget according to the command-line
+    # arguments and to the available database options
+    #
+    if {[catch {
+	mwutil::configureWidget $win configSpecs scrollutil::ss::doConfig \
+				scrollutil::ss::doCget [lrange $args 1 end] 1
+    } result] != 0} {
+	destroy $win
+	return -code error $result
+    }
+
+    #
+    # Move the original widget command into the namespace ss within the current
+    # one and create an alias of the original name for a new widget procedure
+    #
+    rename ::$win ss::$win
+    interp alias {} ::$win {} scrollutil::ss::scrollsyncWidgetCmd $win
+
+    return $win
+}
+
+#------------------------------------------------------------------------------
+# scrollutil::getscrollsync
+#
+# Queries the scrollsync into which a given widget is embedded via the
+# scrollsync's setwidgets subcommand.
+#------------------------------------------------------------------------------
+proc scrollutil::getscrollsync widget {
+    variable ss::scrollsyncArr
+    if {[info exists scrollsyncArr($widget)]} {
+	set win $scrollsyncArr($widget)
+	if {[winfo exists $win] &&
+	    [string compare [winfo class $win] "Scrollsync"] == 0} {
+	    return $win
+	}
+    }
+
+    return ""
+}
+
+#
+# Private configuration procedures
+# ================================
+#
+
+#------------------------------------------------------------------------------
+# scrollutil::ss::doConfig
+#
+# Applies the value val of the configuration option opt to the scrollsync
+# widget win.
+#------------------------------------------------------------------------------
+proc scrollutil::ss::doConfig {win opt val} {
+    variable configSpecs
+    upvar ::scrollutil::ns${win}::data data
+
+    #
+    # Apply the value to the widget corresponding to the given option
+    #
+    switch [lindex $configSpecs($opt) 2] {
+	f {
+	    #
+	    # Apply the value to the frame and save the
+	    # properly formatted value of val in data($opt)
+	    #
+	    $win configure $opt $val
+	    set data($opt) [$win cget $opt]
+	}
+
+	w {
+	    switch -- $opt {
+		-xscrollcommand {
+		    set data($opt) $val
+		    set data(xView) {-1 -1}
+		}
+		-yscrollcommand {
+		    set data($opt) $val
+		    set data(yView) {-1 -1}
+		}
+	    }
+	}
+    }
+}
+
+#------------------------------------------------------------------------------
+# scrollutil::ss::doCget
+#
+# Returns the value of the configuration option opt for the scrollsync widget
+# win.
+#------------------------------------------------------------------------------
+proc scrollutil::ss::doCget {win opt} {
+    upvar ::scrollutil::ns${win}::data data
+    return $data($opt)
+}
+
+#
+# Private procedures implementing the scrollsync widget command
+# =============================================================
+#
+
+#------------------------------------------------------------------------------
+# scrollutil::ss::scrollsyncWidgetCmd
+#
+# Processes the Tcl command corresponding to a scrollsync widget.
+#------------------------------------------------------------------------------
+proc scrollutil::ss::scrollsyncWidgetCmd {win args} {
+    set argCount [llength $args]
+    if {$argCount == 0} {
+	mwutil::wrongNumArgs "$win option ?arg arg ...?"
+    }
+
+    variable cmdOpts
+    set cmd [mwutil::fullOpt "option" [lindex $args 0] $cmdOpts]
+
+    switch $cmd {
+	attrib {
+	    return [::scrollutil::attribSubCmd $win "widget" \
+		    [lrange $args 1 end]]
+	}
+
+	cget {
+	    if {$argCount != 2} {
+		mwutil::wrongNumArgs "$win $cmd option"
+	    }
+
+	    #
+	    # Return the value of the specified configuration option
+	    #
+	    upvar ::scrollutil::ns${win}::data data
+	    variable configSpecs
+	    set opt [mwutil::fullConfigOpt [lindex $args 1] configSpecs]
+	    return $data($opt)
+	}
+
+	configure {
+	    variable configSpecs
+	    return [mwutil::configureSubCmd $win configSpecs \
+		    scrollutil::ss::doConfig scrollutil::ss::doCget \
+		    [lrange $args 1 end]]
+	}
+
+	hasattrib -
+	unsetattrib {
+	    if {$argCount != 2} {
+		mwutil::wrongNumArgs "$win $cmd name"
+	    }
+
+	    return [::scrollutil::${cmd}SubCmd $win "widget" [lindex $args 1]]
+	}
+
+	setwidgets {
+	    if {$argCount != 2} {
+		mwutil::wrongNumArgs "$win $cmd widgetList"
+	    }
+
+	    return [setwidgetsSubCmd $win [lindex $args 1]]
+	}
+
+	widgets {
+	    if {$argCount != 1} {
+		mwutil::wrongNumArgs "$win $cmd"
+	    }
+
+	    upvar ::scrollutil::ns${win}::data data
+	    return $data(widgetList)
+	}
+
+	xview { return [viewSubCmd $win x [lrange $args 1 end]] }
+
+	yview { return [viewSubCmd $win y [lrange $args 1 end]] }
+    }
+}
+
+#------------------------------------------------------------------------------
+# scrollutil::ss::setwidgetsSubCmd
+#
+# Processes the scrollsync setwidgets subcommmand.
+#------------------------------------------------------------------------------
+proc scrollutil::ss::setwidgetsSubCmd {win widgetList} {
+    foreach w $widgetList {
+	if {![winfo exists $w]} {
+	    return -code error "bad window path name \"$w\""
+	}
+
+	set ss [::scrollutil::getscrollsync $w]
+	if {[string length $ss] != 0 && [string compare $ss $win] != 0} {
+	    return -code error "widget $w already in another scrollsync $ss"
+	}
+    }
+
+    variable scrollsyncArr
+    variable xViewArr
+    variable yViewArr
+    upvar ::scrollutil::ns${win}::data data
+
+    set oldWidgetList $data(widgetList)
+    foreach w $oldWidgetList {
+	if {[winfo exists $w]} {
+	    set tagList [bindtags $w]
+	    set idx [lsearch -exact $tagList "WidgetOfScrollsync"]
+	    bindtags $w [lreplace $tagList $idx $idx]
+	}
+
+	if {[info exists scrollsyncArr($w)]} {
+	    unset scrollsyncArr($w)
+	}
+	if {[info exists xViewArr($w)]} {
+	    unset xViewArr($w)
+	}
+	if {[info exists yViewArr($w)]} {
+	    unset yViewArr($w)
+	}
+    }
+
+    array set data {xScrollableList {}  yScrollableList {}}
+
+    foreach w $widgetList {
+	set tagList [bindtags $w]
+	set idx [lsearch -exact $tagList "WidgetOfScrollsync"]
+	if {$idx < 0} {
+	    bindtags $w [linsert $tagList 1 WidgetOfScrollsync]
+	}
+
+	set scrollsyncArr($w) $win
+
+	foreach axis {x y} {
+	    if {[mwutil::isScrollable $w $axis]} {
+		lappend data(${axis}ScrollableList) $w
+		set ${axis}ViewArr($w) {-1 -1}
+		::$w ${axis}view moveto 0
+		::$w configure -${axis}scrollcommand \
+		    [list scrollutil::ss::scrollCmd $win $w $axis]
+	    }
+	}
+
+    }
+
+    set data(widgetList) $widgetList
+    return $oldWidgetList
+}
+
+#------------------------------------------------------------------------------
+# scrollutil::ss::viewSubCmd
+#
+# Processes the scrollsync xview and yview subcommmands.
+#------------------------------------------------------------------------------
+proc scrollutil::ss::viewSubCmd {win axis argList} {
+    upvar ::scrollutil::ns${win}::data data
+    set masterWidget [lindex $data(${axis}ScrollableList) 0]
+    set viewCmd ${axis}view
+
+    switch [llength $argList] {
+	0 {
+	    #
+	    # Command: $win (x|y)view
+	    #
+	    if {[string length $masterWidget] == 0} {
+		return [list 0 1]
+	    } else {
+		return [::$masterWidget $viewCmd]
+	    }
+	}
+
+	default {
+	    #
+	    # Command: $win (x|y)view moveto <fraction>
+	    #	       $win (x|y)view scroll <number> units|pages
+	    #
+	    set argList [mwutil::getScrollInfo2 "$win $viewCmd" $argList]
+	    if {[string length $masterWidget] != 0} {
+		eval [list ::$masterWidget] $viewCmd $argList
+	    }
+	    return ""
+	}
+    }
+}
+
+#
+# Private callback procedure
+# ==========================
+#
+
+#------------------------------------------------------------------------------
+# scrollutil::ss::scrollCmd
+#
+# Propagates the horizontal/vertical position of the view of a given widget
+# within the scrollsync widget win to the other horizontally/vertically
+# scrollable widgets and passes the data of the master widget's view to the
+# value of the -xscrollcommand/-yscrollcommand option.
+#------------------------------------------------------------------------------
+proc scrollutil::ss::scrollCmd {win widget axis first last} {
+    #
+    # Avoid a potential endless loop by making sure that
+    # the view's horizontal/vertical position will only be
+    # propagated to the other widgets if it has changed
+    #
+    variable ${axis}ViewArr
+    set view [set ${axis}ViewArr($widget)]
+    foreach {firstOld lastOld} $view {}
+    if {$first == $firstOld && $last == $lastOld} {
+	return ""
+    } else {
+	set ${axis}ViewArr($widget) [list $first $last]
+    }
+
+    set masterWidget [sortScrollableList $win $axis]
+    set isMasterWidget [expr {[string compare $widget $masterWidget] == 0}]
+    upvar ::scrollutil::ns${win}::data data
+    if {$data(${axis}ViewLocked) && !$isMasterWidget} {
+	return ""
+    }
+
+    foreach w $data(${axis}ScrollableList) {
+	if {[string compare $w $widget] == 0} {
+	    continue
+	}
+
+	if {$first != 0 && $last == 1} {
+	    ::$w ${axis}view moveto 1
+	} else {
+	    ::$w ${axis}view moveto $first
+	}
+    }
+
+    if {$isMasterWidget && [string length $data(-${axis}scrollcommand)] != 0} {
+	foreach {firstOld lastOld} $data(${axis}View) {}
+	if {$first != $firstOld || $last != $lastOld} {
+	    set data(${axis}View) [list $first $last]
+	    eval $data(-${axis}scrollcommand) $first $last
+	}
+    }
+
+    set data(${axis}ViewLocked) 1
+    after 1 [list scrollutil::ss::unlockView $win $axis]
+}
+
+#
+# Private procedures used in bindings
+# ===================================
+#
+
+#------------------------------------------------------------------------------
+# scrollutil::ss::updateMasterWidgets
+#------------------------------------------------------------------------------
+proc scrollutil::ss::updateMasterWidgets win {
+    if {![winfo exists $win] ||
+	[string compare [winfo class $win] "Scrollsync"] != 0} {
+	return ""
+    }
+
+    upvar ::scrollutil::ns${win}::data data
+    foreach axis {x y} {
+	set masterWidget [sortScrollableList $win $axis]
+	if {[string length $masterWidget] != 0 &&
+	    [string length $data(-${axis}scrollcommand)] != 0} {
+	    eval $data(-${axis}scrollcommand) [::$masterWidget ${axis}view]
+	}
+    }
+}
+
+#------------------------------------------------------------------------------
+# scrollutil::ss::onWidgetOfScrollsyncDestroy
+#------------------------------------------------------------------------------
+proc scrollutil::ss::onWidgetOfScrollsyncDestroy widget {
+    variable xViewArr
+    if {[info exists xViewArr($widget)]} {
+	unset xViewArr($widget)
+    }
+
+    variable yViewArr
+    if {[info exists yViewArr($widget)]} {
+	unset yViewArr($widget)
+    }
+
+    set win [::scrollutil::getscrollsync $widget]
+    if {[string length $win] != 0} {
+	set widgetList [::$win widgets]
+	set idx [lsearch -exact $widgetList $widget]
+	::$win setwidgets [lreplace $widgetList $idx $idx]
+    }
+
+    variable scrollsyncArr
+    if {[info exists scrollsyncArr($widget)]} {
+	unset scrollsyncArr($widget)
+    }
+}
+
+#
+# Private utility procedures
+# ==========================
+#
+
+#------------------------------------------------------------------------------
+# scrollutil::ss::sortScrollableList
+#------------------------------------------------------------------------------
+proc scrollutil::ss::sortScrollableList {win axis} {
+    upvar ::scrollutil::ns${win}::data data
+    set data(${axis}ScrollableList) \
+	[lsort -command "compareViews $axis" $data(${axis}ScrollableList)]
+    return [lindex $data(${axis}ScrollableList) 0]
+}
+
+#------------------------------------------------------------------------------
+# scrollutil::ss::compareViews
+#------------------------------------------------------------------------------
+proc scrollutil::ss::compareViews {axis w1 w2} {
+    foreach {first1 last1} [::$w1 ${axis}view] {}
+    foreach {first2 last2} [::$w2 ${axis}view] {}
+    set frac1 [expr {$last1 - $first1}]
+    set frac2 [expr {$last2 - $first2}]
+    set diff  [expr {$frac1 - $frac2}]
+
+    if {abs($diff) < 1.0e-15} {
+	return 0
+    } elseif {$diff < 0} {
+	return -1
+    } else {
+	return 1
+    }
+}
+
+#------------------------------------------------------------------------------
+# scrollutil::ss::unlockView
+#------------------------------------------------------------------------------
+proc scrollutil::ss::unlockView {win axis} {
+    if {[winfo exists $win] &&
+	[string compare [winfo class $win] "Scrollsync"] == 0} {
+	upvar ::scrollutil::ns${win}::data data
+	set data(${axis}ViewLocked) 0
+    }
+}
```

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/scrollutil/scrollutil_tile.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/scrollutil/scrollutil.tcl`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-#==============================================================================
-# Main Scrollutil_tile package module.
-#
-# Copyright (c) 2019-2020  Csaba Nemethi (E-mail: csaba.nemethi@t-online.de)
-#==============================================================================
-
-package require Tk 8.4
-if {$::tk_version < 8.5 || [regexp {^8\.5a[1-5]$} $::tk_patchLevel]} {
-    package require tile 0.6
-}
-package require -exact scrollutil::common 1.5
-
-package provide scrollutil_tile $::scrollutil::version
-package provide Scrollutil_tile $::scrollutil::version
-
-::scrollutil::useTile 1
-
-::scrollutil::sa::createBindings
-::scrollutil::ss::createBindings
-::scrollutil::sf::createBindings
-if {[package vcompare $::tk_version "8.4"] >= 0} {
-    ::scrollutil::createBindings
-}
+#==============================================================================
+# Main Scrollutil package module.
+#
+# Copyright (c) 2019-2022  Csaba Nemethi (E-mail: csaba.nemethi@t-online.de)
+#==============================================================================
+
+package require -exact scrollutil::common 1.17
+
+package provide scrollutil $::scrollutil::version
+package provide Scrollutil $::scrollutil::version
+
+::scrollutil::useTile 0
+
+::scrollutil::sa::createBindings
+::scrollutil::ss::createBindings
+::scrollutil::sf::createBindings
+::scrollutil::pm::createBindings
+if {[package vcompare $::tk_version "8.4"] >= 0} {
+    ::scrollutil::createBindings
+}
```

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/style/as.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/style/as.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/style/lobster.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/style/lobster.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/style/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/style/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/style/style.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/style/style.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/swaplist/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/swaplist/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/swaplist/swaplist.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/swaplist/swaplist.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/mwutil.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/mwutil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/pencil.cur` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/pencil.cur`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/repair.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/repair.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistBind.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistBind.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistConfig.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistConfig.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistEdit.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistEdit.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistImages.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistImages.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistMove.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistMove.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistSort.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistSort.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistThemes.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistThemes.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistUtil.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistUtil.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tablelistWidget.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tablelistWidget.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/scripts/tclIndex` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/scripts/tclIndex`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/tablelist_tile.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/tablelist_tile.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tablelist/tablelistPublic.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tablelist/tablelistPublic.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/boxlabel.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/boxlabel.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/canlabel.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/canlabel.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/labarray.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/labarray.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/objselec.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/objselec.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/perilabel.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/perilabel.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/pie.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/pie.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/pielabel.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/pielabel.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/relirect.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/relirect.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/selector.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/selector.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/slice.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/slice.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tkpiechart/tkpiechart.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tkpiechart/tkpiechart.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tooltip/tipstack.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tooltip/tipstack.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/tooltip/tooltip.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/tooltip/tooltip.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/tclIndex` & `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/tclIndex`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/wcbCommon.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbCommon.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/wcbEntry.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbEntry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/wcbListbox.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbListbox.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/wcbTablelist.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbTablelist.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/wcbText.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbText.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/wcb/scripts/wcbTreeview.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/wcb/scripts/wcbTreeview.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/wcb/wcb.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/wcb/wcb.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/arrowb.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/arrowb.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/calendar.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/calendar.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/dateentry.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/dateentry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/dialog.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/dialog.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/mentry.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/mentry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/panelframe.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/panelframe.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/ruler.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/ruler.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/scrollw.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/scrollw.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/statusbar.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/statusbar.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/stext.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/stext.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/superframe.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/superframe.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/toolbar.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/toolbar.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widget/widget.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widget/widget.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widgetl/listentry.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widgetl/listentry.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widgetl/listsimple.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widgetl/listsimple.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widgetPlus/widgetPlus.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widgetPlus/widgetPlus.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/_tklib/widgetv/validator.tcl` & `tkfly-0.1.0a2/tkfly/_tklib/widgetv/validator.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/core.py` & `tkfly-0.1.0a2/tkfly/core.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/jpegtcl950.dll` & `tkfly-0.1.0a2/tkfly/tkimg/jpegtcl950.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/libjpegtclstub950.a` & `tkfly-0.1.0a2/tkfly/tkimg/libjpegtclstub950.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/libpngtclstub1638.a` & `tkfly-0.1.0a2/tkfly/tkimg/libpngtclstub1638.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/libtifftclstub440.a` & `tkfly-0.1.0a2/tkfly/tkimg/libtifftclstub440.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/libtkimgstub1414.a` & `tkfly-0.1.0a2/tkfly/tkimg/libtkimgstub1414.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/libzlibtclstub1213.a` & `tkfly-0.1.0a2/tkfly/tkimg/libzlibtclstub1213.a`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/pkgIndex.tcl` & `tkfly-0.1.0a2/tkfly/tkimg/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/pngtcl1638.dll` & `tkfly-0.1.0a2/tkfly/tkimg/pngtcl1638.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tifftcl440.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tifftcl440.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimg1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimg1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgbmp1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgbmp1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgdted1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgdted1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgflir1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgflir1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimggif1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimggif1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgico1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgico1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgjpeg1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgjpeg1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgpcx1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgpcx1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgpixmap1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgpixmap1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgpng1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgpng1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgppm1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgppm1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgps1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgps1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgraw1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgraw1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgsgi1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgsgi1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgsun1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgsun1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgtga1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgtga1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgtiff1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgtiff1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgwindow1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgwindow1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgxbm1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgxbm1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/tkimgxpm1414.dll` & `tkfly-0.1.0a2/tkfly/tkimg/tkimgxpm1414.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tkimg/zlibtcl1213.dll` & `tkfly-0.1.0a2/tkfly/tkimg/zlibtcl1213.dll`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tklib/__pycache__/tooltip.cpython-311.pyc` & `tkfly-0.1.0a2/tkfly/tklib/__pycache__/tooltip.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tklib/chatwidget.py` & `tkfly-0.1.0a2/tkfly/tklib/chatwidget.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tklib/menubar.py` & `tkfly-0.1.0a2/tkfly/tklib/menubar.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tklib/tooltip.py` & `tkfly-0.1.0a2/tkfly/tklib/tooltip.py`

 * *Files identical despite different names*

### Comparing `tkfly-0.1.0a1/tkfly/tklib/wcb.py` & `tkfly-0.1.0a2/tkfly/tklib/wcb.py`

 * *Files identical despite different names*

