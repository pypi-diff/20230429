# Comparing `tmp/oresat-gps-1.1.0.tar.gz` & `tmp/oresat-gps-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat-gps-1.1.0.tar", last modified: Sun Jan 29 22:20:25 2023, max compression
+gzip compressed data, was "oresat-gps-1.2.0.tar", last modified: Sat Apr 29 16:27:23 2023, max compression
```

## Comparing `oresat-gps-1.1.0.tar` & `oresat-gps-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:20:25.461979 oresat-gps-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-29 22:20:15.000000 oresat-gps-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-01-29 22:20:25.461979 oresat-gps-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-01-29 22:20:15.000000 oresat-gps-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:20:25.457979 oresat-gps-1.1.0/oresat_gps/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-29 22:20:15.000000 oresat-gps-1.1.0/oresat_gps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-29 22:20:15.000000 oresat-gps-1.1.0/oresat_gps/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:20:25.461979 oresat-gps-1.1.0/oresat_gps/data/
--rw-r--r--   0 runner    (1001) docker     (123)    86043 2023-01-29 22:20:15.000000 oresat-gps-1.1.0/oresat_gps/data/oresat_gps.dcf
--rw-r--r--   0 runner    (1001) docker     (123)    85914 2023-01-29 22:20:15.000000 oresat-gps-1.1.0/oresat_gps/data/oresat_gps.eds
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-01-29 22:20:15.000000 oresat-gps-1.1.0/oresat_gps/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-01-29 22:20:15.000000 oresat-gps-1.1.0/oresat_gps/gps_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-01-29 22:20:15.000000 oresat-gps-1.1.0/oresat_gps/skytraq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:20:25.461979 oresat-gps-1.1.0/oresat_gps/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-01-29 22:20:15.000000 oresat-gps-1.1.0/oresat_gps/templates/skytraq.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:20:25.461979 oresat-gps-1.1.0/oresat_gps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-01-29 22:20:25.000000 oresat-gps-1.1.0/oresat_gps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-01-29 22:20:25.000000 oresat-gps-1.1.0/oresat_gps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 22:20:25.000000 oresat-gps-1.1.0/oresat_gps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-29 22:20:25.000000 oresat-gps-1.1.0/oresat_gps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-29 22:20:25.000000 oresat-gps-1.1.0/oresat_gps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-29 22:20:25.000000 oresat-gps-1.1.0/oresat_gps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-29 22:20:15.000000 oresat-gps-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-29 22:20:25.461979 oresat-gps-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:27:23.884249 oresat-gps-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 16:27:10.000000 oresat-gps-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-29 16:27:23.884249 oresat-gps-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-29 16:27:10.000000 oresat-gps-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:27:23.884249 oresat-gps-1.2.0/oresat_gps/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 16:27:10.000000 oresat-gps-1.2.0/oresat_gps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-29 16:27:10.000000 oresat-gps-1.2.0/oresat_gps/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:27:23.884249 oresat-gps-1.2.0/oresat_gps/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    86303 2023-04-29 16:27:10.000000 oresat-gps-1.2.0/oresat_gps/data/oresat_gps.dcf
+-rw-r--r--   0 runner    (1001) docker     (123)    86158 2023-04-29 16:27:10.000000 oresat-gps-1.2.0/oresat_gps/data/oresat_gps.eds
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-29 16:27:10.000000 oresat-gps-1.2.0/oresat_gps/gps_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-29 16:27:10.000000 oresat-gps-1.2.0/oresat_gps/skytraq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:27:23.884249 oresat-gps-1.2.0/oresat_gps/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-04-29 16:27:10.000000 oresat-gps-1.2.0/oresat_gps/templates/skytraq.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:27:23.884249 oresat-gps-1.2.0/oresat_gps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-29 16:27:23.000000 oresat-gps-1.2.0/oresat_gps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-29 16:27:23.000000 oresat-gps-1.2.0/oresat_gps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:27:23.000000 oresat-gps-1.2.0/oresat_gps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-29 16:27:23.000000 oresat-gps-1.2.0/oresat_gps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-29 16:27:23.000000 oresat-gps-1.2.0/oresat_gps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 16:27:23.000000 oresat-gps-1.2.0/oresat_gps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-29 16:27:10.000000 oresat-gps-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-29 16:27:23.884249 oresat-gps-1.2.0/setup.cfg
```

### Comparing `oresat-gps-1.1.0/LICENSE` & `oresat-gps-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat-gps-1.1.0/PKG-INFO` & `oresat-gps-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-gps
-Version: 1.1.0
+Version: 1.2.0
 Summary: OreSat GPS app
 Home-page: https://github.com/oresat/oresat-gps-software
 Author: PSAS
 Author-email: oresat@pdx.edu
 Maintainer: PSAS
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `oresat-gps-1.1.0/README.rst` & `oresat-gps-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `oresat-gps-1.1.0/oresat_gps/data/oresat_gps.dcf` & `oresat-gps-1.2.0/oresat_gps/data/oresat_gps.dcf`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [FileInfo]
 FileName=oresat_gps.dcf
 FileVersion=1
 FileRevision=1
-LastEDS=
+LastEDS=oresat_gps.eds
 EDSVersion=4.0
 Description=OreSat GPS
 CreationTime=10:31PM
 CreationDate=03-09-2021
 CreatedBy=PSAS
 ModificationTime=11:13AM
 ModificationDate=04-03-2022
@@ -33,15 +33,15 @@
 DynamicChannelsSupported=0
 GroupMessaging=0
 NrOfRXPDO=16
 NrOfTXPDO=16
 LSS_Supported=0
 
 [DeviceComissioning]
-NodeID=52
+NodeID=0x34
 NodeName=GPS
 BaudRate=1000
 NetNumber=0
 NetworkName=
 CANopenManager=0
 LSS_SerialNumber=0
 
@@ -116,15 +116,15 @@
 ParameterName=Serial number
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
 DefaultValue=0x00000000
 
 [OptionalObjects]
-SupportedObjects=85
+SupportedObjects=87
 1=0x1002
 2=0x1003
 3=0x1005
 4=0x1006
 5=0x1007
 6=0x1008
 7=0x1009
@@ -132,84 +132,86 @@
 9=0x1010
 10=0x1011
 11=0x1014
 12=0x1015
 13=0x1016
 14=0x1017
 15=0x1019
-16=0x1023
-17=0x1029
-18=0x1200
-19=0x1400
-20=0x1401
-21=0x1402
-22=0x1403
-23=0x1404
-24=0x1405
-25=0x1406
-26=0x1407
-27=0x1408
-28=0x1409
-29=0x140A
-30=0x140B
-31=0x140C
-32=0x140D
-33=0x140E
-34=0x140F
-35=0x1600
-36=0x1601
-37=0x1602
-38=0x1603
-39=0x1604
-40=0x1605
-41=0x1606
-42=0x1607
-43=0x1608
-44=0x1609
-45=0x160A
-46=0x160B
-47=0x160C
-48=0x160D
-49=0x160E
-50=0x160F
-51=0x1800
-52=0x1801
-53=0x1802
-54=0x1803
-55=0x1804
-56=0x1805
-57=0x1806
-58=0x1807
-59=0x1808
-60=0x1809
-61=0x180A
-62=0x180B
-63=0x180C
-64=0x180D
-65=0x180E
-66=0x180F
-67=0x1A00
-68=0x1A01
-69=0x1A02
-70=0x1A03
-71=0x1A04
-72=0x1A05
-73=0x1A06
-74=0x1A07
-75=0x1A08
-76=0x1A09
-77=0x1A0A
-78=0x1A0B
-79=0x1A0C
-80=0x1A0D
-81=0x1A0E
-82=0x1A0F
-83=0x1F80
-84=0x6000
-85=0x6001
+16=0x1021
+17=0x1022
+18=0x1023
+19=0x1029
+20=0x1200
+21=0x1400
+22=0x1401
+23=0x1402
+24=0x1403
+25=0x1404
+26=0x1405
+27=0x1406
+28=0x1407
+29=0x1408
+30=0x1409
+31=0x140A
+32=0x140B
+33=0x140C
+34=0x140D
+35=0x140E
+36=0x140F
+37=0x1600
+38=0x1601
+39=0x1602
+40=0x1603
+41=0x1604
+42=0x1605
+43=0x1606
+44=0x1607
+45=0x1608
+46=0x1609
+47=0x160A
+48=0x160B
+49=0x160C
+50=0x160D
+51=0x160E
+52=0x160F
+53=0x1800
+54=0x1801
+55=0x1802
+56=0x1803
+57=0x1804
+58=0x1805
+59=0x1806
+60=0x1807
+61=0x1808
+62=0x1809
+63=0x180A
+64=0x180B
+65=0x180C
+66=0x180D
+67=0x180E
+68=0x180F
+69=0x1A00
+70=0x1A01
+71=0x1A02
+72=0x1A03
+73=0x1A04
+74=0x1A05
+75=0x1A06
+76=0x1A07
+77=0x1A08
+78=0x1A09
+79=0x1A0A
+80=0x1A0B
+81=0x1A0C
+82=0x1A0D
+83=0x1A0E
+84=0x1A0F
+85=0x1F80
+86=0x6000
+87=0x6001
 
 [1002]
 ParameterName=Manufacturer status register
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
 DefaultValue=0
@@ -497,14 +499,30 @@
 [1019]
 ParameterName=Synchronous counter overflow value
 ObjectType=0x07
 DataType=0x0005
 AccessType=rw
 DefaultValue=0
 
+;A master node can read this for a copy of the node's EDS file
+[1021]
+ParameterName=Store EDS
+ObjectType=0x07
+DataType=0x000F
+AccessType=ro
+DefaultValue=0
+
+;Indicate the format of the Store EDS
+[1022]
+ParameterName=Store format
+ObjectType=0x07
+DataType=0x0005
+AccessType=ro
+DefaultValue=0
+
 [1023]
 ParameterName=OS command
 ObjectType=0x09
 SubNumber=4
 
 [1023sub0]
 ParameterName=Highest sub-index supported
@@ -514,26 +532,29 @@
 DefaultValue=0x03
 
 [1023sub1]
 ParameterName=Command
 ObjectType=0x07
 DataType=0x000F
 AccessType=rw
+DefaultValue=0
 
 [1023sub2]
 ParameterName=Status
 ObjectType=0x07
 DataType=0x0005
 AccessType=ro
+DefaultValue=0
 
 [1023sub3]
 ParameterName=Reply
 ObjectType=0x07
 DataType=0x000F
 AccessType=ro
+DefaultValue=0
 
 [1029]
 ParameterName=Error behavior
 ObjectType=0x08
 SubNumber=3
 
 [1029sub0]
@@ -598,15 +619,15 @@
 SubNumber=4
 
 [1400sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1400sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x00000181
@@ -631,15 +652,15 @@
 SubNumber=4
 
 [1401sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1401sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000300+$NODEID
@@ -664,15 +685,15 @@
 SubNumber=4
 
 [1402sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1402sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000400+$NODEID
@@ -697,15 +718,15 @@
 SubNumber=4
 
 [1403sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1403sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000500+$NODEID
@@ -730,15 +751,15 @@
 SubNumber=4
 
 [1404sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1404sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000200+$NODEID
@@ -763,15 +784,15 @@
 SubNumber=4
 
 [1405sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1405sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000300+$NODEID
@@ -796,15 +817,15 @@
 SubNumber=4
 
 [1406sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1406sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000400+$NODEID
@@ -829,15 +850,15 @@
 SubNumber=4
 
 [1407sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1407sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000500+$NODEID
@@ -862,15 +883,15 @@
 SubNumber=4
 
 [1408sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1408sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000200+$NODEID
@@ -895,15 +916,15 @@
 SubNumber=4
 
 [1409sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1409sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000300+$NODEID
@@ -928,15 +949,15 @@
 SubNumber=4
 
 [140Asub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Asub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000400+$NODEID
@@ -961,15 +982,15 @@
 SubNumber=4
 
 [140Bsub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Bsub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000500+$NODEID
@@ -994,15 +1015,15 @@
 SubNumber=4
 
 [140Csub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Csub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000200+$NODEID
@@ -1027,15 +1048,15 @@
 SubNumber=4
 
 [140Dsub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Dsub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000300+$NODEID
@@ -1060,15 +1081,15 @@
 SubNumber=4
 
 [140Esub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Esub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000400+$NODEID
@@ -1093,15 +1114,15 @@
 SubNumber=4
 
 [140Fsub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Fsub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000500+$NODEID
@@ -4207,35 +4228,37 @@
 AccessType=const
 DefaultValue=0
 
 ;Status. read for current state, write commands
 ;
 ;States:
 ;  0x00: off
-;  0x01: searching to satellites
+;  0x01: searching for satellites
 ;  0x02: locked on >= 4 satellites
 ;  0xFF: failed
 ;
 ;Commands:
 ;  0: turn the skytraq off
 ;  1: turn the skytraq on
 [6000sub5]
 ParameterName=Status
 ObjectType=0x07
 DataType=0x0005
 AccessType=rw
 DefaultValue=0x01
+PDOMapping=1
 
 ;has the system time been sync'd to the time in the skytraq message
 [6000sub6]
 ParameterName=Time Syncd
 ObjectType=0x07
 DataType=0x0001
 AccessType=ro
 DefaultValue=0
+PDOMapping=1
 
 [6001]
 ParameterName=SkyTraq Data
 ObjectType=0x09
 SubNumber=21
 
 [6001sub0]
@@ -4572,59 +4595,47 @@
 ;Manufacturer specific errors:
 ;Manufacturer may define its own constants up to index 0xFF. Of course, they must then define large enough buffer for error status bits (up to 32 bytes).
 [2100]
 ParameterName=Error status bits
 ObjectType=0x07
 DataType=0x000A
 AccessType=ro
-DefaultValue=00000000000000000000
+DefaultValue=00 00 00 00 00 00 00 00 00 00
 
 [3000]
-ParameterName=OLAF app control
+ParameterName=Power control
 ObjectType=0x09
-SubNumber=5
+SubNumber=3
 
 [3000sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x04
+DefaultValue=0x02
 
-;Write true to restart the board
+;Write true to poweroff the system
 [3000sub1]
-ParameterName=Reboot Board
+ParameterName=Poweroff
 ObjectType=0x07
 DataType=0x0001
 AccessType=wo
 DefaultValue=0
 
-;Write true to poweroff the board
+;1 for a soft reset (restart daemon)
+;2 for hard reset (reboot the board)
+;3 to do a factory reset (clear all caches and reboot)
 [3000sub2]
-ParameterName=Poweroff Board
-ObjectType=0x07
-DataType=0x0001
-AccessType=wo
-DefaultValue=0
-
-;Write true to have the OLAF app exit
-[3000sub3]
-ParameterName=Quit
+ParameterName=Reset
 ObjectType=0x07
-DataType=0x0001
+DataType=0x0005
 AccessType=wo
 DefaultValue=0
-
-;Allow OLAF to control the board CPU frequency
-[3000sub4]
-ParameterName=CPU frequency
-ObjectType=0x07
-DataType=0x0001
-AccessType=rw
-DefaultValue=0
+LowLimit=0
+HighLimit=3
 
 [3001]
 ParameterName=System info
 ObjectType=0x09
 SubNumber=29
 
 [3001sub0]
@@ -4636,39 +4647,35 @@
 
 ;Get the name of the OS running on the board
 [3001sub1]
 ParameterName=OS name
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the name of the OS distro running on the board
 [3001sub2]
 ParameterName=OS distro
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the version of the OS running on the board
 [3001sub3]
 ParameterName=OS kernel version
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the board hostname
 [3001sub4]
 ParameterName=hostname
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the uptime
 [3001sub5]
 ParameterName=Uptime
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
@@ -4684,23 +4691,21 @@
 
 ;Get the architecture of CPUs on board
 [3001sub7]
 ParameterName=CPU architecture
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the CPU power governor of the board
 [3001sub8]
 ParameterName=CPU governor
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the CPU frequency of the board
 [3001sub9]
 ParameterName=CPU frequency
 ObjectType=0x07
 DataType=0x0006
 AccessType=ro
@@ -4729,23 +4734,21 @@
 
 ;Get the name of selected remoteproc
 [3001subC]
 ParameterName=RemoteprocX name
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the state of selected remoteproc
 [3001subD]
 ParameterName=RemoteprocX state
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the 1 minute load average
 [3001subE]
 ParameterName=Load average 1min
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
@@ -4915,15 +4918,14 @@
 ;
 ;Write an empty string or '\n' to have no filter.
 [3002sub4]
 ParameterName=Filter
 ObjectType=0x07
 DataType=0x0009
 AccessType=rw
-DefaultValue=x
 
 ;Length of the current cache selected with keyword filter
 [3002sub5]
 ParameterName=Cache len
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
@@ -4943,15 +4945,14 @@
 
 ;File name for the selected place in the selected cache
 [3002sub7]
 ParameterName=File name
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;File size for the selected place in the selected cache
 [3002sub8]
 ParameterName=File size
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
@@ -4979,72 +4980,64 @@
 
 ;Name of the file to read. Uses Index 3002 to find file names.
 [3003sub1]
 ParameterName=File name
 ObjectType=0x07
 DataType=0x0009
 AccessType=rw
-DefaultValue=x
 
 ;Data of the file selected in subindex 1
 [3003sub2]
 ParameterName=File data
 ObjectType=0x07
 DataType=0x000F
 AccessType=ro
+DefaultValue=0
 
-;Clear subindexes 1 and 2
+;Gets the CRC32 of the file
 [3003sub3]
-ParameterName=Reset
+ParameterName=CRC32
 ObjectType=0x07
-DataType=0x0001
-AccessType=wo
+DataType=0x0007
+AccessType=ro
 DefaultValue=0
 
 ;Delete the file selected in subindex 1
 [3003sub4]
 ParameterName=Delete file
 ObjectType=0x07
 DataType=0x0001
 AccessType=wo
 DefaultValue=0
 
 [3004]
 ParameterName=Fwrite
 ObjectType=0x09
-SubNumber=4
+SubNumber=3
 
 [3004sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x02
 
 ;Name of the file to be written. Must be set before index 2.
 [3004sub1]
 ParameterName=File name
 ObjectType=0x07
 DataType=0x0009
 AccessType=rw
-DefaultValue=x
 
 ;File data for the new file written. Must set subindex 1 before writing to this subindex.
 [3004sub2]
 ParameterName=File data
 ObjectType=0x07
 DataType=0x000F
 AccessType=wo
-
-;Clear subindexes 1 and 2
-[3004sub3]
-ParameterName=Reset
-ObjectType=0x07
-DataType=0x0001
-AccessType=wo
 DefaultValue=0
 
 [3005]
 ParameterName=App manager
 ObjectType=0x09
 SubNumber=7
 
@@ -5087,31 +5080,49 @@
 DefaultValue=0
 
 [3005sub5]
 ParameterName=App name
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 [3005sub6]
 ParameterName=Daemon state
 ObjectType=0x07
 DataType=0x0005
 AccessType=rw
 DefaultValue=0
 
-;Write any non-zero number to get system logs. Log will be place in fread cache.
 [3006]
-ParameterName=Get log
+ParameterName=New Record
+ObjectType=0x09
+SubNumber=3
+
+[3006sub0]
+ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
-AccessType=rw
+AccessType=const
+DefaultValue=0x02
+
+;This will make a compress tar archive of the full system logs. It will be add to the cache.
+[3006sub1]
+ParameterName=Make logs file
+ObjectType=0x07
+DataType=0x0001
+AccessType=wo
 DefaultValue=0
 
+;Get the logs since boot as a string.
+[3006sub2]
+ParameterName=Get logs
+ObjectType=0x07
+DataType=0x0009
+AccessType=ro
+
 [3100]
 ParameterName=Updater
 ObjectType=0x09
 SubNumber=6
 
 [3100sub0]
 ParameterName=Highest sub-index supported
@@ -5146,15 +5157,14 @@
 
 ;List the updates cached
 [3100sub3]
 ParameterName=List updates
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Write a non-zero value to start an update
 [3100sub4]
 ParameterName=Update
 ObjectType=0x07
 DataType=0x0001
 AccessType=wo
```

### Comparing `oresat-gps-1.1.0/oresat_gps/data/oresat_gps.eds` & `oresat-gps-1.2.0/oresat_gps/data/oresat_gps.eds`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 ParameterName=Serial number
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
 DefaultValue=0x00000000
 
 [OptionalObjects]
-SupportedObjects=85
+SupportedObjects=87
 1=0x1002
 2=0x1003
 3=0x1005
 4=0x1006
 5=0x1007
 6=0x1008
 7=0x1009
@@ -122,84 +122,86 @@
 9=0x1010
 10=0x1011
 11=0x1014
 12=0x1015
 13=0x1016
 14=0x1017
 15=0x1019
-16=0x1023
-17=0x1029
-18=0x1200
-19=0x1400
-20=0x1401
-21=0x1402
-22=0x1403
-23=0x1404
-24=0x1405
-25=0x1406
-26=0x1407
-27=0x1408
-28=0x1409
-29=0x140A
-30=0x140B
-31=0x140C
-32=0x140D
-33=0x140E
-34=0x140F
-35=0x1600
-36=0x1601
-37=0x1602
-38=0x1603
-39=0x1604
-40=0x1605
-41=0x1606
-42=0x1607
-43=0x1608
-44=0x1609
-45=0x160A
-46=0x160B
-47=0x160C
-48=0x160D
-49=0x160E
-50=0x160F
-51=0x1800
-52=0x1801
-53=0x1802
-54=0x1803
-55=0x1804
-56=0x1805
-57=0x1806
-58=0x1807
-59=0x1808
-60=0x1809
-61=0x180A
-62=0x180B
-63=0x180C
-64=0x180D
-65=0x180E
-66=0x180F
-67=0x1A00
-68=0x1A01
-69=0x1A02
-70=0x1A03
-71=0x1A04
-72=0x1A05
-73=0x1A06
-74=0x1A07
-75=0x1A08
-76=0x1A09
-77=0x1A0A
-78=0x1A0B
-79=0x1A0C
-80=0x1A0D
-81=0x1A0E
-82=0x1A0F
-83=0x1F80
-84=0x6000
-85=0x6001
+16=0x1021
+17=0x1022
+18=0x1023
+19=0x1029
+20=0x1200
+21=0x1400
+22=0x1401
+23=0x1402
+24=0x1403
+25=0x1404
+26=0x1405
+27=0x1406
+28=0x1407
+29=0x1408
+30=0x1409
+31=0x140A
+32=0x140B
+33=0x140C
+34=0x140D
+35=0x140E
+36=0x140F
+37=0x1600
+38=0x1601
+39=0x1602
+40=0x1603
+41=0x1604
+42=0x1605
+43=0x1606
+44=0x1607
+45=0x1608
+46=0x1609
+47=0x160A
+48=0x160B
+49=0x160C
+50=0x160D
+51=0x160E
+52=0x160F
+53=0x1800
+54=0x1801
+55=0x1802
+56=0x1803
+57=0x1804
+58=0x1805
+59=0x1806
+60=0x1807
+61=0x1808
+62=0x1809
+63=0x180A
+64=0x180B
+65=0x180C
+66=0x180D
+67=0x180E
+68=0x180F
+69=0x1A00
+70=0x1A01
+71=0x1A02
+72=0x1A03
+73=0x1A04
+74=0x1A05
+75=0x1A06
+76=0x1A07
+77=0x1A08
+78=0x1A09
+79=0x1A0A
+80=0x1A0B
+81=0x1A0C
+82=0x1A0D
+83=0x1A0E
+84=0x1A0F
+85=0x1F80
+86=0x6000
+87=0x6001
 
 [1002]
 ParameterName=Manufacturer status register
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
 DefaultValue=0
@@ -487,14 +489,30 @@
 [1019]
 ParameterName=Synchronous counter overflow value
 ObjectType=0x07
 DataType=0x0005
 AccessType=rw
 DefaultValue=0
 
+;A master node can read this for a copy of the node's EDS file
+[1021]
+ParameterName=Store EDS
+ObjectType=0x07
+DataType=0x000F
+AccessType=ro
+DefaultValue=0
+
+;Indicate the format of the Store EDS
+[1022]
+ParameterName=Store format
+ObjectType=0x07
+DataType=0x0005
+AccessType=ro
+DefaultValue=0
+
 [1023]
 ParameterName=OS command
 ObjectType=0x09
 SubNumber=4
 
 [1023sub0]
 ParameterName=Highest sub-index supported
@@ -504,26 +522,29 @@
 DefaultValue=0x03
 
 [1023sub1]
 ParameterName=Command
 ObjectType=0x07
 DataType=0x000F
 AccessType=rw
+DefaultValue=0
 
 [1023sub2]
 ParameterName=Status
 ObjectType=0x07
 DataType=0x0005
 AccessType=ro
+DefaultValue=0
 
 [1023sub3]
 ParameterName=Reply
 ObjectType=0x07
 DataType=0x000F
 AccessType=ro
+DefaultValue=0
 
 [1029]
 ParameterName=Error behavior
 ObjectType=0x08
 SubNumber=3
 
 [1029sub0]
@@ -588,15 +609,15 @@
 SubNumber=4
 
 [1400sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1400sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x00000181
@@ -621,15 +642,15 @@
 SubNumber=4
 
 [1401sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1401sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000300+$NODEID
@@ -654,15 +675,15 @@
 SubNumber=4
 
 [1402sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1402sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000400+$NODEID
@@ -687,15 +708,15 @@
 SubNumber=4
 
 [1403sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1403sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000500+$NODEID
@@ -720,15 +741,15 @@
 SubNumber=4
 
 [1404sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1404sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000200+$NODEID
@@ -753,15 +774,15 @@
 SubNumber=4
 
 [1405sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1405sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000300+$NODEID
@@ -786,15 +807,15 @@
 SubNumber=4
 
 [1406sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1406sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000400+$NODEID
@@ -819,15 +840,15 @@
 SubNumber=4
 
 [1407sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1407sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000500+$NODEID
@@ -852,15 +873,15 @@
 SubNumber=4
 
 [1408sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1408sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000200+$NODEID
@@ -885,15 +906,15 @@
 SubNumber=4
 
 [1409sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [1409sub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000300+$NODEID
@@ -918,15 +939,15 @@
 SubNumber=4
 
 [140Asub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Asub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000400+$NODEID
@@ -951,15 +972,15 @@
 SubNumber=4
 
 [140Bsub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Bsub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000500+$NODEID
@@ -984,15 +1005,15 @@
 SubNumber=4
 
 [140Csub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Csub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000200+$NODEID
@@ -1017,15 +1038,15 @@
 SubNumber=4
 
 [140Dsub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Dsub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000300+$NODEID
@@ -1050,15 +1071,15 @@
 SubNumber=4
 
 [140Esub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Esub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000400+$NODEID
@@ -1083,15 +1104,15 @@
 SubNumber=4
 
 [140Fsub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x05
 
 [140Fsub1]
 ParameterName=COB-ID used by RPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x80000500+$NODEID
@@ -4197,35 +4218,37 @@
 AccessType=const
 DefaultValue=0
 
 ;Status. read for current state, write commands
 ;
 ;States:
 ;  0x00: off
-;  0x01: searching to satellites
+;  0x01: searching for satellites
 ;  0x02: locked on >= 4 satellites
 ;  0xFF: failed
 ;
 ;Commands:
 ;  0: turn the skytraq off
 ;  1: turn the skytraq on
 [6000sub5]
 ParameterName=Status
 ObjectType=0x07
 DataType=0x0005
 AccessType=rw
 DefaultValue=0x01
+PDOMapping=1
 
 ;has the system time been sync'd to the time in the skytraq message
 [6000sub6]
 ParameterName=Time Syncd
 ObjectType=0x07
 DataType=0x0001
 AccessType=ro
 DefaultValue=0
+PDOMapping=1
 
 [6001]
 ParameterName=SkyTraq Data
 ObjectType=0x09
 SubNumber=21
 
 [6001sub0]
@@ -4562,59 +4585,47 @@
 ;Manufacturer specific errors:
 ;Manufacturer may define its own constants up to index 0xFF. Of course, they must then define large enough buffer for error status bits (up to 32 bytes).
 [2100]
 ParameterName=Error status bits
 ObjectType=0x07
 DataType=0x000A
 AccessType=ro
-DefaultValue=00000000000000000000
+DefaultValue=00 00 00 00 00 00 00 00 00 00
 
 [3000]
-ParameterName=OLAF app control
+ParameterName=Power control
 ObjectType=0x09
-SubNumber=5
+SubNumber=3
 
 [3000sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x04
+DefaultValue=0x02
 
-;Write true to restart the board
+;Write true to poweroff the system
 [3000sub1]
-ParameterName=Reboot Board
+ParameterName=Poweroff
 ObjectType=0x07
 DataType=0x0001
 AccessType=wo
 DefaultValue=0
 
-;Write true to poweroff the board
+;1 for a soft reset (restart daemon)
+;2 for hard reset (reboot the board)
+;3 to do a factory reset (clear all caches and reboot)
 [3000sub2]
-ParameterName=Poweroff Board
-ObjectType=0x07
-DataType=0x0001
-AccessType=wo
-DefaultValue=0
-
-;Write true to have the OLAF app exit
-[3000sub3]
-ParameterName=Quit
+ParameterName=Reset
 ObjectType=0x07
-DataType=0x0001
+DataType=0x0005
 AccessType=wo
 DefaultValue=0
-
-;Allow OLAF to control the board CPU frequency
-[3000sub4]
-ParameterName=CPU frequency
-ObjectType=0x07
-DataType=0x0001
-AccessType=rw
-DefaultValue=0
+LowLimit=0
+HighLimit=3
 
 [3001]
 ParameterName=System info
 ObjectType=0x09
 SubNumber=29
 
 [3001sub0]
@@ -4626,39 +4637,35 @@
 
 ;Get the name of the OS running on the board
 [3001sub1]
 ParameterName=OS name
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the name of the OS distro running on the board
 [3001sub2]
 ParameterName=OS distro
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the version of the OS running on the board
 [3001sub3]
 ParameterName=OS kernel version
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the board hostname
 [3001sub4]
 ParameterName=hostname
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the uptime
 [3001sub5]
 ParameterName=Uptime
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
@@ -4674,23 +4681,21 @@
 
 ;Get the architecture of CPUs on board
 [3001sub7]
 ParameterName=CPU architecture
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the CPU power governor of the board
 [3001sub8]
 ParameterName=CPU governor
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the CPU frequency of the board
 [3001sub9]
 ParameterName=CPU frequency
 ObjectType=0x07
 DataType=0x0006
 AccessType=ro
@@ -4719,23 +4724,21 @@
 
 ;Get the name of selected remoteproc
 [3001subC]
 ParameterName=RemoteprocX name
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the state of selected remoteproc
 [3001subD]
 ParameterName=RemoteprocX state
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Get the 1 minute load average
 [3001subE]
 ParameterName=Load average 1min
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
@@ -4905,15 +4908,14 @@
 ;
 ;Write an empty string or '\n' to have no filter.
 [3002sub4]
 ParameterName=Filter
 ObjectType=0x07
 DataType=0x0009
 AccessType=rw
-DefaultValue=x
 
 ;Length of the current cache selected with keyword filter
 [3002sub5]
 ParameterName=Cache len
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
@@ -4933,15 +4935,14 @@
 
 ;File name for the selected place in the selected cache
 [3002sub7]
 ParameterName=File name
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;File size for the selected place in the selected cache
 [3002sub8]
 ParameterName=File size
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
@@ -4969,72 +4970,64 @@
 
 ;Name of the file to read. Uses Index 3002 to find file names.
 [3003sub1]
 ParameterName=File name
 ObjectType=0x07
 DataType=0x0009
 AccessType=rw
-DefaultValue=x
 
 ;Data of the file selected in subindex 1
 [3003sub2]
 ParameterName=File data
 ObjectType=0x07
 DataType=0x000F
 AccessType=ro
+DefaultValue=0
 
-;Clear subindexes 1 and 2
+;Gets the CRC32 of the file
 [3003sub3]
-ParameterName=Reset
+ParameterName=CRC32
 ObjectType=0x07
-DataType=0x0001
-AccessType=wo
+DataType=0x0007
+AccessType=ro
 DefaultValue=0
 
 ;Delete the file selected in subindex 1
 [3003sub4]
 ParameterName=Delete file
 ObjectType=0x07
 DataType=0x0001
 AccessType=wo
 DefaultValue=0
 
 [3004]
 ParameterName=Fwrite
 ObjectType=0x09
-SubNumber=4
+SubNumber=3
 
 [3004sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x03
+DefaultValue=0x02
 
 ;Name of the file to be written. Must be set before index 2.
 [3004sub1]
 ParameterName=File name
 ObjectType=0x07
 DataType=0x0009
 AccessType=rw
-DefaultValue=x
 
 ;File data for the new file written. Must set subindex 1 before writing to this subindex.
 [3004sub2]
 ParameterName=File data
 ObjectType=0x07
 DataType=0x000F
 AccessType=wo
-
-;Clear subindexes 1 and 2
-[3004sub3]
-ParameterName=Reset
-ObjectType=0x07
-DataType=0x0001
-AccessType=wo
 DefaultValue=0
 
 [3005]
 ParameterName=App manager
 ObjectType=0x09
 SubNumber=7
 
@@ -5077,31 +5070,49 @@
 DefaultValue=0
 
 [3005sub5]
 ParameterName=App name
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 [3005sub6]
 ParameterName=Daemon state
 ObjectType=0x07
 DataType=0x0005
 AccessType=rw
 DefaultValue=0
 
-;Write any non-zero number to get system logs. Log will be place in fread cache.
 [3006]
-ParameterName=Get log
+ParameterName=New Record
+ObjectType=0x09
+SubNumber=3
+
+[3006sub0]
+ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
-AccessType=rw
+AccessType=const
+DefaultValue=0x02
+
+;This will make a compress tar archive of the full system logs. It will be add to the cache.
+[3006sub1]
+ParameterName=Make logs file
+ObjectType=0x07
+DataType=0x0001
+AccessType=wo
 DefaultValue=0
 
+;Get the logs since boot as a string.
+[3006sub2]
+ParameterName=Get logs
+ObjectType=0x07
+DataType=0x0009
+AccessType=ro
+
 [3100]
 ParameterName=Updater
 ObjectType=0x09
 SubNumber=6
 
 [3100sub0]
 ParameterName=Highest sub-index supported
@@ -5136,15 +5147,14 @@
 
 ;List the updates cached
 [3100sub3]
 ParameterName=List updates
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=x
 
 ;Write a non-zero value to start an update
 [3100sub4]
 ParameterName=Update
 ObjectType=0x07
 DataType=0x0001
 AccessType=wo
```

### Comparing `oresat-gps-1.1.0/oresat_gps/gps_resource.py` & `oresat-gps-1.2.0/oresat_gps/gps_resource.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from os import geteuid
 from enum import IntEnum
 from time import clock_settime, CLOCK_REALTIME
 
-from olaf import Resource, scet_int_from_time, logger
+from olaf import Resource, scet_int_from_time, logger, GPIO
 
-from .gpio import GPIO
 from .skytraq import SkyTraq, NavData, FixMode, gps_datetime
 
 
 class ControlSubindex(IntEnum):
     SERIAL_BUS = 0x1
     SKYTRAQ_PIN = 0x2
     LNA_PIN = 0x3
@@ -25,69 +24,73 @@
 
 
 class GPSResource(Resource):
 
     INDEX_SKYTRAQ_CONTROL = 0x6000
     INDEX_SKYTRAQ_DATA = 0x6001
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, mock_skytraq: bool):
+        super().__init__()
 
-        self._gpio0 = None
-        self._gpio1 = None
+        self._gpio_skytraq = None
+        self._gpio_lna = None
         self._skytraq = None
         self._state = States.OFF
+        self._mock_skytraq = mock_skytraq
+
+        if mock_skytraq:
+            logger.warning('mocking SkyTraq and GPIO power pins')
 
         self._uid = geteuid()
         if self._uid != 0:
             logger.warning('not running as root, cannot set system time to time from skytraq')
 
     def on_start(self):
 
-        self.control_rec = self.od[self.INDEX_SKYTRAQ_CONTROL]
-        self.data_rec = self.od[self.INDEX_SKYTRAQ_DATA]
+        self.control_rec = self.node.od[self.INDEX_SKYTRAQ_CONTROL]
+        self.data_rec = self.node.od[self.INDEX_SKYTRAQ_DATA]
+
+        self.node.add_sdo_read_callback(self.INDEX_SKYTRAQ_CONTROL, self._on_read)
+        self.node.add_sdo_write_callback(self.INDEX_SKYTRAQ_CONTROL, self._on_write)
+
+        self.control_rec[ControlSubindex.MOCK.value].value = self._mock_skytraq
 
         # control subindexes
-        self.mock_obj = self.control_rec[ControlSubindex.MOCK.value]
         self.is_syncd_obj = self.control_rec[ControlSubindex.IS_SYNCD.value]
         self.status_obj = self.control_rec[ControlSubindex.STATUS.value]
 
         # make sure the flag for the time has been syncd is set to false
         self.is_syncd_obj.value = False
 
-        self.mock_obj.value = self.mock_hw
-        if self.mock_hw:
-            logger.warning('mocking SkyTraq')
-        else:
-            skytraq_pin = self.control_rec[ControlSubindex.SKYTRAQ_PIN.value].value
-            lna_pin = self.control_rec[ControlSubindex.LNA_PIN.value].value
-            self._gpio_skytraq = GPIO(skytraq_pin)
-            self._gpio_lna = GPIO(lna_pin)
-            self._skytraq_power_on()
-
+        skytraq_pin = self.control_rec[ControlSubindex.SKYTRAQ_PIN.value].value
+        lna_pin = self.control_rec[ControlSubindex.LNA_PIN.value].value
+        self._gpio_skytraq = GPIO(skytraq_pin, self._mock_skytraq)
+        self._gpio_lna = GPIO(lna_pin, self._mock_skytraq)
         self._skytraq_power_on()
+
         serial_bus = self.control_rec[ControlSubindex.SERIAL_BUS.value].value
-        self._skytraq = SkyTraq(serial_bus, self._new_message, self._new_error, self.mock_hw)
+        self._skytraq = SkyTraq(serial_bus, self._new_message, self._new_error, self._mock_skytraq)
         self._skytraq.start()
         self._state = States.SEARCHING
 
     def on_end(self):
         self._skytraq.stop()
         self._skytraq_power_off()
         self._state = States.OFF
 
-    def on_read(self, index, subindex, od):
+    def _on_read(self, index: int, subindex: int):
+
         if index == self.INDEX_SKYTRAQ_CONTROL and subindex == ControlSubindex.STATUS:
             return self._state.value
 
-    def on_write(self, index, subindex, od, data):
+    def _on_write(self, index: int, subindex: int, value):
 
         if index == self.INDEX_SKYTRAQ_CONTROL and subindex == ControlSubindex.STATUS:
             # turn skytraq on/off
-            if od.decode_raw(data):
+            if value:
                 self._skytraq_power_on()
             else:
                 self._skytraq_power_off()
                 self.data_rec[NavData.NUMBER_OF_SV.value].value = 0  # zero this for TPDO
 
     def _new_message(self, nav_data: NavData):
 
@@ -105,18 +108,18 @@
 
             # add all skytraq data to OD
             for i in range(len(nav_data)):
                 self.data_rec[i].value = nav_data[i]
             self.data_rec[0x14].value = scet_int_from_time(dt)
 
             # send gps tpdos
-            self.send_tpdo(2)
-            self.send_tpdo(3)
-            self.send_tpdo(4)
-            self.send_tpdo(5)
+            self.node.send_tpdo(2)
+            self.node.send_tpdo(3)
+            self.node.send_tpdo(4)
+            self.node.send_tpdo(5)
 
         # update status
         if nav_data.number_of_sv >= 4 and nav_data.fix_mode >= FixMode.FIX_2D:
             self._state = States.LOCKED
         else:
             self._state = States.SEARCHING
 
@@ -124,19 +127,17 @@
 
         self._state = States.ERROR
         logger.error(error)
 
     def _skytraq_power_on(self):
 
         logger.info('turning SkyTraq on')
-        if not self.mock_hw:
-            self._gpio_skytraq.on()
-            self._gpio_lna.on()
+        self._gpio_skytraq.high()
+        self._gpio_lna.high()
         self._state = States.SEARCHING
 
     def _skytraq_power_off(self):
 
         logger.info('turning SkyTraq off')
-        if not self.mock_hw:
-            self._gpio_skytraq.off()
-            self._gpio_lna.off()
+        self._gpio_skytraq.low()
+        self._gpio_lna.low()
         self._state = States.OFF
```

### Comparing `oresat-gps-1.1.0/oresat_gps/skytraq.py` & `oresat-gps-1.2.0/oresat_gps/skytraq.py`

 * *Files identical despite different names*

### Comparing `oresat-gps-1.1.0/oresat_gps/templates/skytraq.html` & `oresat-gps-1.2.0/oresat_gps/templates/skytraq.html`

 * *Files 10% similar despite different names*

```diff
@@ -124,114 +124,117 @@
           <td><span id='ecefVy'></span> km / s</td>
         </tr>
         <tr>
           <td>ECEF VZ</td>
           <td><span id='ecefVz'></span> km / s</td>
         </tr>
         <tr>
-          <td>UTC Timestamp</td>
+          <td>Timestamp (Local TZ)</td>
           <td><span id='timestamp'></span></td>
         </tr>
       </table>
     </div>
   </div>
   <script>
     const FIX_MODES = {
       0: 'NO_FIX',
       1: '2D',
       2: '3D',
       3: '3D+DGPS',
     };
 
-  const indexNames = {
-    '0x01': 'fixMode',
-    '0x02': 'numSv',
-    '0x03': 'gpsWeek',
-    '0x04': 'tow',
-    '0x05': 'lat',
-    '0x06': 'long',
-    '0x07': 'ellipAlt',
-    '0x08': 'meanSeaLevelAlt',
-    '0x09': 'gdop',
-    '0x0A': 'pdop',
-    '0x0B': 'hdop',
-    '0x0C': 'vdop',
-    '0x0D': 'tdop',
-    '0x0E': 'ecefX',
-    '0x0F': 'ecefY',
-    '0x10': 'ecefZ',
-    '0x11': 'ecefVx',
-    '0x12': 'ecefVy',
-    '0x13': 'ecefVz',
-    '0x14': 'timestamp',
-  };
-    
-  const STATES = {
-    0: 'OFF',
-    1: 'SEARCHING',
-    2: 'LOCKED_ON',
-    255: 'FAILED',
-  };
-
-  async function updateStatic() {
-    let obj = await readValue('0x6000', '0x01');
-    document.getElementById('serialBus').textContent = obj['value'];
-    obj = await readValue('0x6000', '0x02');
-    document.getElementById('gpio0').textContent = obj['value'];
-    obj = await readValue('0x6000', '0x03');
-    document.getElementById('gpio1').textContent = obj['value'];
-    obj = await readValue('0x6000', '0x04');
-    document.getElementById('mock').textContent = obj['value'];
-  }
-
-  async function updateAll() {
-    for (const index in indexNames) {
-      const obj = await readValue('0x6001', index);
-      const tmp = document.getElementById(indexNames[index]);
-
-      switch(index) {
-      case '0x01':
-        tmp.textContent = FIX_MODES[obj['value']];
-        break;
-      case '0x05':
-      case '0x06':
-        tmp.textContent = (obj['value'] / 1e7).toFixed(3);
-        break;
-      case '0x07':
-      case '0x08':
-      case '0x09':
-      case '0x0A':
-      case '0x0B':
-      case '0x0C':
-      case '0x0D':
-        tmp.textContent = (obj['value'] * 0.01).toFixed(2);
-        break;
-      case '0x0E':
-      case '0x0F':
-      case '0x10':
-      case '0x11':
-      case '0x12':
-      case '0x13':
-        tmp.textContent = (obj['value'] / 100000).toFixed(3);
-        break;
-      case '0x14':
-        const d = scetToDate(obj['value']);
-        tmp.textContent = d.toLocaleString('en-US', { timeZone: 'UTC' });
-        break;
-      default:
-        tmp.textContent = obj['value'];
+    const subindexNames = {
+      0x01: 'fixMode',
+      0x02: 'numSv',
+      0x03: 'gpsWeek',
+      0x04: 'tow',
+      0x05: 'lat',
+      0x06: 'long',
+      0x07: 'ellipAlt',
+      0x08: 'meanSeaLevelAlt',
+      0x09: 'gdop',
+      0x0A: 'pdop',
+      0x0B: 'hdop',
+      0x0C: 'vdop',
+      0x0D: 'tdop',
+      0x0E: 'ecefX',
+      0x0F: 'ecefY',
+      0x10: 'ecefZ',
+      0x11: 'ecefVx',
+      0x12: 'ecefVy',
+      0x13: 'ecefVz',
+      0x14: 'timestamp',
+    };
+
+    const STATES = {
+      0: 'OFF',
+      1: 'SEARCHING',
+      2: 'LOCKED_ON',
+      255: 'FAILED',
+    };
+
+    async function updateStatic() {
+      let obj = await readValue('0x6000', '0x01');
+      document.getElementById('serialBus').textContent = obj['value'];
+      obj = await readValue('0x6000', '0x02');
+      document.getElementById('gpio0').textContent = obj['value'];
+      obj = await readValue('0x6000', '0x03');
+      document.getElementById('gpio1').textContent = obj['value'];
+      obj = await readValue('0x6000', '0x04');
+      document.getElementById('mock').textContent = obj['value'];
+    }
+
+    const timezone = Intl.DateTimeFormat().resolvedOptions().timeZone;
+
+    async function updateAll() {
+      let obj = await readValue('0x6001', null);
+      for (const subindex in subindexNames) {
+        const tmp = document.getElementById(subindexNames[subindex]);
+        let sub_obj = obj.subindexes[subindex];
+
+        switch(parseInt(subindex)) {
+        case 0x01:
+          tmp.textContent = FIX_MODES[sub_obj.value];
+          break;
+        case 0x05:
+        case 0x06:
+          tmp.textContent = (sub_obj.value / 1e7).toFixed(3);
+          break;
+        case 0x07:
+        case 0x08:
+        case 0x09:
+        case 0x0A:
+        case 0x0B:
+        case 0x0C:
+        case 0x0D:
+          tmp.textContent = (sub_obj.value * 0.01).toFixed(2);
+          break;
+        case 0x0E:
+        case 0x0F:
+        case 0x10:
+        case 0x11:
+        case 0x12:
+        case 0x13:
+          tmp.textContent = (sub_obj.value / 100000).toFixed(3);
+          break;
+        case 0x14:
+          const d = scetToDate(sub_obj.value);
+          tmp.textContent = d.toLocaleString('en-US', { timeZone: timezone });
+          break;
+        default:
+          tmp.textContent = sub_obj.value;
+        }
       }
+
+      obj = await readValue('0x6000', '0x05');
+      document.getElementById('status').textContent = STATES[obj.value];
+      obj = await readValue('0x6000', '0x06');
+      document.getElementById('timeSyncd').textContent = obj.value;
     }
-    
-    let obj = await readValue('0x6000', '0x05');
-    document.getElementById('status').textContent = STATES[obj['value']];
-    obj = await readValue('0x6000', '0x06');
-    document.getElementById('timeSyncd').textContent = obj['value'];
-  }
-
-  updateStatic();
-  updateAll();
-  const interval = setInterval(function() {
-    updateAll()
-  }, 10000);
-</script>
+
+    updateStatic();
+    updateAll();
+    const interval = setInterval(function() {
+      updateAll();
+    }, 10000);
+  </script>
 {% endblock %}
```

### Comparing `oresat-gps-1.1.0/oresat_gps.egg-info/PKG-INFO` & `oresat-gps-1.2.0/oresat_gps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-gps
-Version: 1.1.0
+Version: 1.2.0
 Summary: OreSat GPS app
 Home-page: https://github.com/oresat/oresat-gps-software
 Author: PSAS
 Author-email: oresat@pdx.edu
 Maintainer: PSAS
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `oresat-gps-1.1.0/setup.cfg` & `oresat-gps-1.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Software Development :: Embedded Systems
 
 [options]
 packages = find:
 install_requires = 
-	oresat-olaf>=1.0.0
+	oresat-olaf>=2.0.0
 	pyserial
 python_requires = >=3.7
 
 [options.package_data]
 oresat_gps = 
 	data/*
 	templates/*
```

