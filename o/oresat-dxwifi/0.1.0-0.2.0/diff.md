# Comparing `tmp/oresat-dxwifi-0.1.0.tar.gz` & `tmp/oresat-dxwifi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat-dxwifi-0.1.0.tar", last modified: Sun Jan 29 23:56:48 2023, max compression
+gzip compressed data, was "oresat-dxwifi-0.2.0.tar", last modified: Sat Apr 29 16:26:36 2023, max compression
```

## Comparing `oresat-dxwifi-0.1.0.tar` & `oresat-dxwifi-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 23:56:48.260929 oresat-dxwifi-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-29 23:56:39.000000 oresat-dxwifi-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-29 23:56:48.260929 oresat-dxwifi-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-01-29 23:56:39.000000 oresat-dxwifi-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 23:56:48.260929 oresat-dxwifi-0.1.0/oresat_dxwifi/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-29 23:56:39.000000 oresat-dxwifi-0.1.0/oresat_dxwifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-29 23:56:39.000000 oresat-dxwifi-0.1.0/oresat_dxwifi/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 23:56:48.260929 oresat-dxwifi-0.1.0/oresat_dxwifi/data/
--rw-r--r--   0 runner    (1001) docker     (123)    81782 2023-01-29 23:56:39.000000 oresat-dxwifi-0.1.0/oresat_dxwifi/data/oresat_dxwifi.dcf
--rw-r--r--   0 runner    (1001) docker     (123)    81659 2023-01-29 23:56:39.000000 oresat-dxwifi-0.1.0/oresat_dxwifi/data/oresat_dxwifi.eds
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 23:56:48.260929 oresat-dxwifi-0.1.0/oresat_dxwifi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-29 23:56:48.000000 oresat-dxwifi-0.1.0/oresat_dxwifi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-01-29 23:56:48.000000 oresat-dxwifi-0.1.0/oresat_dxwifi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 23:56:48.000000 oresat-dxwifi-0.1.0/oresat_dxwifi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-29 23:56:48.000000 oresat-dxwifi-0.1.0/oresat_dxwifi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-29 23:56:48.000000 oresat-dxwifi-0.1.0/oresat_dxwifi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-29 23:56:48.000000 oresat-dxwifi-0.1.0/oresat_dxwifi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-29 23:56:39.000000 oresat-dxwifi-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-01-29 23:56:48.260929 oresat-dxwifi-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:26:36.448094 oresat-dxwifi-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-29 16:26:36.448094 oresat-dxwifi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:26:36.444094 oresat-dxwifi-0.2.0/oresat_dxwifi/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/oresat_dxwifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/oresat_dxwifi/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:26:36.448094 oresat-dxwifi-0.2.0/oresat_dxwifi/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    82338 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/oresat_dxwifi/data/oresat_dxwifi.dcf
+-rw-r--r--   0 runner    (1001) docker     (123)    82187 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/oresat_dxwifi/data/oresat_dxwifi.eds
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:26:36.448094 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-29 16:26:36.000000 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-29 16:26:36.000000 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:26:36.000000 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 16:26:36.000000 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-29 16:26:36.000000 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-29 16:26:36.000000 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-29 16:26:36.448094 oresat-dxwifi-0.2.0/setup.cfg
```

### Comparing `oresat-dxwifi-0.1.0/LICENSE` & `oresat-dxwifi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat-dxwifi-0.1.0/PKG-INFO` & `oresat-dxwifi-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-dxwifi
-Version: 0.1.0
+Version: 0.2.0
 Summary: OreSat DxWiFi app
 Home-page: https://github.com/oresat/oresat-dxwifi-software
 Author: PSAS
 Author-email: oresat@pdx.edu
 Maintainer: PSAS
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `oresat-dxwifi-0.1.0/oresat_dxwifi/data/oresat_dxwifi.dcf` & `oresat-dxwifi-0.2.0/oresat_dxwifi/data/oresat_dxwifi.dcf`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [FileInfo]
-FileName=oresat_dxwifi.eds
+FileName=oresat_dxwifi.dcf
 FileVersion=1
 FileRevision=1
+LastEDS=oresat_dxwifi.eds
 EDSVersion=4.0
 Description=OreSat DxWiFi
 CreationTime=10:41PM
 CreationDate=03-09-2021
 CreatedBy=PSAS
 ModificationTime=12:49PM
 ModificationDate=11-26-2021
@@ -32,15 +33,15 @@
 DynamicChannelsSupported=0
 GroupMessaging=0
 NrOfRXPDO=16
 NrOfTXPDO=16
 LSS_Supported=0
 
 [DeviceComissioning]
-NodeID=76
+NodeID=0x4C
 NodeName=DxWiFi
 BaudRate=1000
 NetNumber=0
 NetworkName=
 CANopenManager=0
 LSS_SerialNumber=0
 
@@ -115,15 +116,15 @@
 ParameterName=Serial number
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
 DefaultValue=0x00000000
 
 [OptionalObjects]
-SupportedObjects=84
+SupportedObjects=86
 1=0x1002
 2=0x1003
 3=0x1005
 4=0x1006
 5=0x1007
 6=0x1008
 7=0x1009
@@ -131,83 +132,85 @@
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
 
 [1002]
 ParameterName=Manufacturer status register
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
 DefaultValue=0
@@ -303,15 +306,15 @@
 DefaultValue=0
 
 [1008]
 ParameterName=Manufacturer device name
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=OreSat Linux Generic
+DefaultValue=OreSat DxWiFi
 
 [1009]
 ParameterName=Manufacturer hardware version
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
 DefaultValue=0.0
@@ -495,14 +498,30 @@
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
@@ -512,27 +531,29 @@
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
 DefaultValue=0
 
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
@@ -597,15 +618,15 @@
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
@@ -630,15 +651,15 @@
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
@@ -663,15 +684,15 @@
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
@@ -696,15 +717,15 @@
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
@@ -729,15 +750,15 @@
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
@@ -762,15 +783,15 @@
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
@@ -795,15 +816,15 @@
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
@@ -828,15 +849,15 @@
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
@@ -861,15 +882,15 @@
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
@@ -894,15 +915,15 @@
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
@@ -927,15 +948,15 @@
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
@@ -960,15 +981,15 @@
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
@@ -993,15 +1014,15 @@
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
@@ -1026,15 +1047,15 @@
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
@@ -1059,15 +1080,15 @@
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
@@ -1092,15 +1113,15 @@
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
@@ -3022,15 +3043,15 @@
 ObjectType=0x09
 SubNumber=7
 
 [180Fsub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
-AccessType=ro
+AccessType=const
 DefaultValue=0x06
 
 [180Fsub1]
 ParameterName=COB-ID used by TPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
@@ -4028,15 +4049,15 @@
 ObjectType=0x09
 SubNumber=9
 
 [1A0Esub0]
 ParameterName=Number of mapped application objects in PDO
 ObjectType=0x07
 DataType=0x0005
-AccessType=rw
+AccessType=const
 DefaultValue=0x08
 
 [1A0Esub1]
 ParameterName=Mapping object 1
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
@@ -4164,15 +4185,15 @@
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x00000008
 
 [6000]
 ParameterName=DxWiFi status
-ObjectType=0x7
+ObjectType=0x07
 DataType=0x0001
 AccessType=ro
 DefaultValue=0
 PDOMapping=1
 
 [ManufacturerObjects]
 SupportedObjects=12
@@ -4195,15 +4216,15 @@
 ObjectType=0x09
 SubNumber=5
 
 [2000sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
-AccessType=ro
+AccessType=const
 DefaultValue=0x04
 
 ;Bdefault specifies the bus to be considered active after a node power-on, node hardware reset.
 [2000sub1]
 ParameterName=Bdefault
 ObjectType=0x07
 DataType=0x0005
@@ -4319,59 +4340,47 @@
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
+ParameterName=Reset
 ObjectType=0x07
-DataType=0x0001
-AccessType=wo
-DefaultValue=0
-
-;Write true to have the OLAF app exit
-[3000sub3]
-ParameterName=Quit
-ObjectType=0x07
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
@@ -4723,14 +4732,15 @@
 
 ;Data of the file selected in subindex 1
 [3003sub2]
 ParameterName=File data
 ObjectType=0x07
 DataType=0x000F
 AccessType=ro
+DefaultValue=0
 
 ;Gets the CRC32 of the file
 [3003sub3]
 ParameterName=CRC32
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
@@ -4765,14 +4775,15 @@
 
 ;File data for the new file written. Must set subindex 1 before writing to this subindex.
 [3004sub2]
 ParameterName=File data
 ObjectType=0x07
 DataType=0x000F
 AccessType=wo
+DefaultValue=0
 
 [3005]
 ParameterName=App manager
 ObjectType=0x09
 SubNumber=7
 
 [3005sub0]
@@ -4822,32 +4833,51 @@
 [3005sub6]
 ParameterName=Daemon state
 ObjectType=0x07
 DataType=0x0005
 AccessType=rw
 DefaultValue=0
 
-;Write any non-zero number to get system logs. Log will be place in fread cache.
 [3006]
-ParameterName=Get log
+ParameterName=Log
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
 ObjectType=0x07
 DataType=0x0005
-AccessType=ro
+AccessType=const
 DefaultValue=0x05
 
 ;Get the status of updater
 ;
 ;States:
 ; * update-succesful: 0x00
 ; * pre-update-failed: 0x01
```

### Comparing `oresat-dxwifi-0.1.0/oresat_dxwifi/data/oresat_dxwifi.eds` & `oresat-dxwifi-0.2.0/oresat_dxwifi/data/oresat_dxwifi.eds`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 ParameterName=Serial number
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
 DefaultValue=0x00000000
 
 [OptionalObjects]
-SupportedObjects=84
+SupportedObjects=86
 1=0x1002
 2=0x1003
 3=0x1005
 4=0x1006
 5=0x1007
 6=0x1008
 7=0x1009
@@ -122,83 +122,85 @@
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
 
 [1002]
 ParameterName=Manufacturer status register
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
 DefaultValue=0
@@ -294,15 +296,15 @@
 DefaultValue=0
 
 [1008]
 ParameterName=Manufacturer device name
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
-DefaultValue=OreSat Linux Generic
+DefaultValue=OreSat DxWiFi
 
 [1009]
 ParameterName=Manufacturer hardware version
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
 DefaultValue=0.0
@@ -486,14 +488,30 @@
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
@@ -503,27 +521,29 @@
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
 DefaultValue=0
 
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
@@ -588,15 +608,15 @@
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
@@ -621,15 +641,15 @@
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
@@ -654,15 +674,15 @@
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
@@ -687,15 +707,15 @@
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
@@ -720,15 +740,15 @@
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
@@ -753,15 +773,15 @@
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
@@ -786,15 +806,15 @@
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
@@ -819,15 +839,15 @@
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
@@ -852,15 +872,15 @@
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
@@ -885,15 +905,15 @@
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
@@ -918,15 +938,15 @@
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
@@ -951,15 +971,15 @@
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
@@ -984,15 +1004,15 @@
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
@@ -1017,15 +1037,15 @@
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
@@ -1050,15 +1070,15 @@
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
@@ -1083,15 +1103,15 @@
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
@@ -3013,15 +3033,15 @@
 ObjectType=0x09
 SubNumber=7
 
 [180Fsub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
-AccessType=ro
+AccessType=const
 DefaultValue=0x06
 
 [180Fsub1]
 ParameterName=COB-ID used by TPDO
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
@@ -4019,15 +4039,15 @@
 ObjectType=0x09
 SubNumber=9
 
 [1A0Esub0]
 ParameterName=Number of mapped application objects in PDO
 ObjectType=0x07
 DataType=0x0005
-AccessType=rw
+AccessType=const
 DefaultValue=0x08
 
 [1A0Esub1]
 ParameterName=Mapping object 1
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
@@ -4155,15 +4175,15 @@
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x00000008
 
 [6000]
 ParameterName=DxWiFi status
-ObjectType=0x7
+ObjectType=0x07
 DataType=0x0001
 AccessType=ro
 DefaultValue=0
 PDOMapping=1
 
 [ManufacturerObjects]
 SupportedObjects=12
@@ -4186,15 +4206,15 @@
 ObjectType=0x09
 SubNumber=5
 
 [2000sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
-AccessType=ro
+AccessType=const
 DefaultValue=0x04
 
 ;Bdefault specifies the bus to be considered active after a node power-on, node hardware reset.
 [2000sub1]
 ParameterName=Bdefault
 ObjectType=0x07
 DataType=0x0005
@@ -4310,59 +4330,47 @@
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
+ParameterName=Reset
 ObjectType=0x07
-DataType=0x0001
-AccessType=wo
-DefaultValue=0
-
-;Write true to have the OLAF app exit
-[3000sub3]
-ParameterName=Quit
-ObjectType=0x07
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
@@ -4714,14 +4722,15 @@
 
 ;Data of the file selected in subindex 1
 [3003sub2]
 ParameterName=File data
 ObjectType=0x07
 DataType=0x000F
 AccessType=ro
+DefaultValue=0
 
 ;Gets the CRC32 of the file
 [3003sub3]
 ParameterName=CRC32
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
@@ -4756,14 +4765,15 @@
 
 ;File data for the new file written. Must set subindex 1 before writing to this subindex.
 [3004sub2]
 ParameterName=File data
 ObjectType=0x07
 DataType=0x000F
 AccessType=wo
+DefaultValue=0
 
 [3005]
 ParameterName=App manager
 ObjectType=0x09
 SubNumber=7
 
 [3005sub0]
@@ -4813,32 +4823,51 @@
 [3005sub6]
 ParameterName=Daemon state
 ObjectType=0x07
 DataType=0x0005
 AccessType=rw
 DefaultValue=0
 
-;Write any non-zero number to get system logs. Log will be place in fread cache.
 [3006]
-ParameterName=Get log
+ParameterName=Log
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
 ObjectType=0x07
 DataType=0x0005
-AccessType=ro
+AccessType=const
 DefaultValue=0x05
 
 ;Get the status of updater
 ;
 ;States:
 ; * update-succesful: 0x00
 ; * pre-update-failed: 0x01
```

### Comparing `oresat-dxwifi-0.1.0/oresat_dxwifi.egg-info/PKG-INFO` & `oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-dxwifi
-Version: 0.1.0
+Version: 0.2.0
 Summary: OreSat DxWiFi app
 Home-page: https://github.com/oresat/oresat-dxwifi-software
 Author: PSAS
 Author-email: oresat@pdx.edu
 Maintainer: PSAS
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `oresat-dxwifi-0.1.0/setup.cfg` & `oresat-dxwifi-0.2.0/setup.cfg`

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
 python_requires = >=3.7
 
 [options.package_data]
 oresat_dxwifi = data/*
 
 [options.entry_points]
 console_scripts =
```

