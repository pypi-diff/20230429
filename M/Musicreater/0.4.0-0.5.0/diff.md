# Comparing `tmp/Musicreater-0.4.0.tar.gz` & `tmp/Musicreater-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Musicreater-0.4.0.tar", last modified: Wed Apr 19 13:14:24 2023, max compression
+gzip compressed data, was "Musicreater-0.5.0.tar", last modified: Sat Apr 29 11:21:32 2023, max compression
```

## Comparing `Musicreater-0.4.0.tar` & `Musicreater-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 13:14:24.544093 Musicreater-0.4.0/
--rw-rw-rw-   0        0        0    13085 2023-02-12 08:13:49.000000 Musicreater-0.4.0/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-04-19 13:14:24.530093 Musicreater-0.4.0/Musicreater/
--rw-rw-rw-   0        0        0      899 2023-04-19 13:14:14.000000 Musicreater-0.4.0/Musicreater/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-02-12 08:13:49.000000 Musicreater-0.4.0/Musicreater/exceptions.py
--rw-rw-rw-   0        0        0     4847 2023-02-12 08:13:49.000000 Musicreater-0.4.0/Musicreater/instConstants.py
--rw-rw-rw-   0        0        0     7611 2023-02-12 08:13:49.000000 Musicreater-0.4.0/Musicreater/magicmain.py
--rw-rw-rw-   0        0        0    67997 2023-02-12 09:37:40.000000 Musicreater-0.4.0/Musicreater/main.py
--rw-rw-rw-   0        0        0     6643 2023-02-12 08:13:49.000000 Musicreater-0.4.0/Musicreater/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-19 13:14:24.541094 Musicreater-0.4.0/Musicreater.egg-info/
--rw-rw-rw-   0        0        0     6321 2023-04-19 13:14:23.000000 Musicreater-0.4.0/Musicreater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-19 13:14:24.000000 Musicreater-0.4.0/Musicreater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 13:14:23.000000 Musicreater-0.4.0/Musicreater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-19 13:14:23.000000 Musicreater-0.4.0/Musicreater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-19 13:14:23.000000 Musicreater-0.4.0/Musicreater.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6321 2023-04-19 13:14:24.543094 Musicreater-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     5252 2023-02-12 08:13:49.000000 Musicreater-0.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 13:14:24.545093 Musicreater-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1533 2023-02-12 08:24:01.000000 Musicreater-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:21:32.918646 Musicreater-0.5.0/
+-rw-rw-rw-   0        0        0    13085 2023-02-05 09:39:58.000000 Musicreater-0.5.0/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-04-29 11:21:32.904692 Musicreater-0.5.0/Musicreater/
+-rw-rw-rw-   0        0        0      890 2023-04-29 11:13:55.000000 Musicreater-0.5.0/Musicreater/__init__.py
+-rw-rw-rw-   0        0        0     3195 2023-04-29 11:13:55.000000 Musicreater-0.5.0/Musicreater/exceptions.py
+-rw-rw-rw-   0        0        0     5479 2023-04-29 11:13:55.000000 Musicreater-0.5.0/Musicreater/instConstants.py
+-rw-rw-rw-   0        0        0    10696 2023-04-29 11:13:55.000000 Musicreater-0.5.0/Musicreater/magicmain.py
+-rw-rw-rw-   0        0        0    79538 2023-04-29 11:13:55.000000 Musicreater-0.5.0/Musicreater/main.py
+-rw-rw-rw-   0        0        0    13358 2023-04-29 11:13:55.000000 Musicreater-0.5.0/Musicreater/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:21:32.915655 Musicreater-0.5.0/Musicreater.egg-info/
+-rw-rw-rw-   0        0        0     7616 2023-04-29 11:21:32.000000 Musicreater-0.5.0/Musicreater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-29 11:21:32.000000 Musicreater-0.5.0/Musicreater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:21:32.000000 Musicreater-0.5.0/Musicreater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-29 11:21:32.000000 Musicreater-0.5.0/Musicreater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 11:21:32.000000 Musicreater-0.5.0/Musicreater.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7616 2023-04-29 11:21:32.917650 Musicreater-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6547 2023-04-29 11:13:55.000000 Musicreater-0.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 11:21:32.918646 Musicreater-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1533 2023-04-25 15:21:09.000000 Musicreater-0.5.0/setup.py
```

### Comparing `Musicreater-0.4.0/LICENSE.md` & `Musicreater-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Musicreater-0.4.0/Musicreater/__init__.py` & `Musicreater-0.5.0/Musicreater/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # -*- coding: utf-8 -*-
 """一个简单的我的世界音频转换库
-音·创 库版 (Musicreater)
+音·创 (Musicreater)
 是一款免费开源的针对《我的世界》的midi音乐转换库
 Musicreater(音·创)
 A free open source library used for convert midi file into formats that is suitable for **Minecraft**.
 
 版权所有 © 2023 音·创 开发者
 Copyright © 2023 all the developers of Musicreater
 
 开源相关声明请见 ../License.md
 Terms & Conditions: ../License.md
 """
 
-# 音·创 开发交流群 861684859
-# Email EillesWan2006@163.com W-YI_DoctorYI@outlook.com EillesWan@outlook.com
+# 睿穆组织 开发交流群 861684859
+# Email TriM-Organization@hotmail.com
 # 版权所有 金羿("Eilles Wan") & 诸葛亮与八卦阵("bgArray") & 鸣凤鸽子("MingFengPigeon")
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 from .main import *
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __all__ = []
-__author__ = (("金羿", "Eilles Wan"), ("诸葛亮与八卦阵", "bgArray"))
-
-
+__author__ = (("金羿", "Eilles Wan"), ("诸葛亮与八卦阵", "bgArray"), ("鸣凤鸽子", "MingFengPigeon"))
```

### Comparing `Musicreater-0.4.0/Musicreater/instConstants.py` & `Musicreater-0.5.0/Musicreater/instConstants.py`

 * *Files 14% similar despite different names*

```diff
@@ -172,8 +172,29 @@
     73: ("note.hat", 7),
     74: ("note.xylophone", 4),
     75: ("note.hat", 7),
     76: ("note.hat", 7),
     77: ("note.xylophone", 4),
     78: ("note.xylophone", 4),
     79: ("note.bell", 4),
-    80: ("note.bell", 4), }
+    80: ("note.bell", 4),
+}
+
+instrument_to_blocks_list = {
+    "note.bass": ("planks",),
+    "note.snare": ("sand",),
+    "note.hat": ("glass",),
+    "note.bd": ("stone",),
+    "note.bell": ("gold_block",),
+    "note.flute": ("clay",),
+    "note.chime": ("packed_ice",),
+    "note.guitar": ("wool",),
+    "note.xylobone": ("bone_block",),
+    "note.iron_xylophone": ("iron_block",),
+    "note.cow_bell": ("soul_sand",),
+    "note.didgeridoo": ("pumpkin",),
+    "note.bit": ("emerald_block",),
+    "note.banjo": ("hay_block",),
+    "note.pling": ("glowstone",),
+    "note.bassattack": ("command_block",),  # 无法找到此音效
+    "note.harp": ("glass",),
+}
```

### Comparing `Musicreater-0.4.0/Musicreater/main.py` & `Musicreater-0.5.0/Musicreater/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 
 # 音·创 开发交流群 861684859
-# Email EillesWan2006@163.com W-YI_DoctorYI@outlook.com EillesWan@outlook.com
+# Email TriM-Organization@hotmail.com
 # 版权所有 金羿("Eilles Wan") & 诸葛亮与八卦阵("bgArray") & 鸣凤鸽子("MingFengPigeon")
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
 """
 音·创 (Musicreater)
 是一款免费开源的针对《我的世界》的midi音乐转换库
@@ -31,14 +31,19 @@
 from .instConstants import *
 
 from typing import TypeVar, Union
 
 T = TypeVar("T")  # Declare type variable
 VM = TypeVar("VM", mido.MidiFile, None)  # void mido
 
+DEFAULT_PROGRESSBAR_STYLE = (
+    r"▶ %%N [ %%s/%^s %%% __________ %%t|%^t ]",
+    ("§e=§r", "§7=§r"),
+)
+
 
 class SingleNote:
     def __init__(
         self, instrument: int, pitch: int, velocity: int, startTime: int, lastTime: int
     ):
         """用于存储单个音符的类
         :param instrument 乐器编号
@@ -88,21 +93,24 @@
             "velocity": self.velocity,
             "startTime": self.startTime,
             "lastTime": self.lastTime,
         }
 
 
 class MethodList(list):
+    """函数列表，列表中的所有元素均为函数"""
+
     def __init__(self, in_=()):
+        """函数列表，列表中的所有元素均为函数"""
         super().__init__()
         self._T = [_x for _x in in_]
 
     def __getitem__(self, item) -> T:
         return self._T[item]
-    
+
     def __len__(self) -> int:
         return self._T.__len__()
 
 
 """
 学习笔记：
 tempo:  microseconds per quarter note 毫秒每四分音符，换句话说就是一拍占多少毫秒
@@ -134,80 +142,125 @@
 tick * tempo / 1000000.0 / ticks_per_beat * 一秒多少游戏刻
 
 
 """
 
 
 class midiConvert:
-    def __init__(self, debug: bool = False):
+    def __init__(self, enable_old_exe_format: bool = True, debug: bool = False):
         """简单的midi转换类，将midi文件转换为我的世界结构或者包"""
-        self.debugMode: bool = debug
 
-        self.midiFile: str = ""
+        self.debug_mode: bool = debug
+        """是否开启调试模式"""
+
+        self.midi_file: str = ""
+        """Midi文件路径"""
+
         self.midi: VM = None
-        self.outputPath: str = ""
-        self.midFileName: str = ""
-        self.exeHead = ""
+        """MidiFile对象"""
+
+        self.output_path: str = ""
+        """输出路径"""
+
+        self.mid_file_name: str = ""
+        """文件名，不含路径且不含后缀"""
+
+        self.execute_cmd_head = ""
+        """execute 指令的执行开头，用于被format"""
+
         self.methods = MethodList(
-            [self._toCmdList_m1, self._toCmdList_m2, self._toCmdList_m3, self._toCmdList_m4]
+            [
+                self._toCmdList_m1,
+                self._toCmdList_m2,
+                self._toCmdList_m3,
+                self._toCmdList_m4,
+            ]
         )
+        """转换算法列表，你觉得我为什么要这样调用函数？"""
 
         self.methods_byDelay = MethodList(
             [
                 self._toCmdList_withDelay_m1,
                 self._toCmdList_withDelay_m2,
+                self._toCmdList_withDelay_m3,
             ]
         )
+        """转换算法列表，但是是对于延迟播放器的，你觉得我为什么要这样调用函数？"""
 
-    def convert(self, midiFile: str, outputPath: str, oldExeFormat: bool = True):
+        self.enable_old_exe_format = enable_old_exe_format
+        """是否启用旧版指令格式"""
+
+        self.execute_cmd_head = (
+            "execute {} ~ ~ ~ "
+            if enable_old_exe_format
+            else "execute as {} at @s positioned ~ ~ ~ run "
+        )
+        """execute指令的应用，两个版本提前决定。"""
+
+    def convert(self, midi_file: str, output_path: str):
         """转换前需要先运行此函数来获取基本信息"""
 
-        self.midiFile = midiFile
+        self.midi_file = midi_file
         """midi文件路径"""
 
         try:
-            self.midi = mido.MidiFile(self.midiFile)
+            self.midi = mido.MidiFile(self.midi_file)
             """MidiFile对象"""
         except Exception as E:
-            raise MidiDestroyedError(f"文件{self.midiFile}损坏：{E}")
+            raise MidiDestroyedError(f"文件{self.midi_file}损坏：{E}")
 
-        self.outputPath = os.path.abspath(outputPath)
+        self.output_path = os.path.abspath(output_path)
         """输出路径"""
         # 将self.midiFile的文件名，不含路径且不含后缀存入self.midiFileName
-        self.midFileName = os.path.splitext(os.path.basename(self.midiFile))[0]
+        self.mid_file_name = os.path.splitext(os.path.basename(self.midi_file))[0]
         """文件名，不含路径且不含后缀"""
 
-        self.exeHead = (
-            "execute {} ~ ~ ~ "
-            if oldExeFormat
-            else "execute as {} at @s positioned ~ ~ ~ run "
-        )
-        """execute指令的应用，两个版本提前决定。"""
-
     @staticmethod
-    def __Inst2soundID_withX(instrumentID):
-        """返回midi的乐器ID对应的我的世界乐器名，对于音域转换算法，如下：
-            2**( ( msg.note - 60 - X ) / 12 ) 即为MC的音高，其中
-            X的取值随乐器不同而变化：
-            竖琴harp、电钢琴pling、班卓琴banjo、方波bit、颤音琴iron_xylophone 的时候为6
-            吉他的时候为7
-            贝斯bass、迪吉里杜管didgeridoo的时候为8
-            长笛flute、牛铃cou_bell的时候为5
-            钟琴bell、管钟chime、木琴xylophone的时候为4
-            而存在一些打击乐器bd(basedrum)、hat、snare，没有音域，则没有X，那么我们返回7即可
-        :param instrumentID: midi的乐器ID
-        default: 如果instrumentID不在范围内，返回的默认我的世界乐器名称
-        :return: (str我的世界乐器名, int转换算法中的X)"""
+    def __Inst2soundID_withX(
+        instrumentID: int,
+    ):
+        """
+        返回midi的乐器ID对应的我的世界乐器名，对于音域转换算法，如下：
+        2**( ( msg.note - 60 - X ) / 12 ) 即为MC的音高，其中
+        X的取值随乐器不同而变化：
+        竖琴harp、电钢琴pling、班卓琴banjo、方波bit、颤音琴iron_xylophone 的时候为6
+        吉他的时候为7
+        贝斯bass、迪吉里杜管didgeridoo的时候为8
+        长笛flute、牛铃cou_bell的时候为5
+        钟琴bell、管钟chime、木琴xylophone的时候为4
+        而存在一些打击乐器bd(basedrum)、hat、snare，没有音域，则没有X，那么我们返回7即可
+
+        Parameters
+        ----------
+        instrumentID: int
+            midi的乐器ID
+
+        Returns
+        -------
+        tuple(str我的世界乐器名, int转换算法中的X)
+        """
         try:
             return pitched_instrument_list[instrumentID]
         except KeyError:
             return "note.flute", 5
 
     @staticmethod
-    def __bitInst2ID_withX(instrumentID):
+    def __bitInst2ID_withX(instrumentID: int):
+        """
+        对于Midi第10通道所对应的打击乐器，返回我的世界乐器名
+
+        Parameters
+        ----------
+        instrumentID: int
+            midi的乐器ID
+
+        Returns
+        -------
+        tuple(str我的世界乐器名, int转换算法中的X)
+        """
         try:
             return percussion_instrument_list[instrumentID]
         except KeyError:
             print("WARN", "无法使用打击乐器列表库，或者使用了不存在的乐器，打击乐器使用Dislink算法代替。{instrumentID}")
             if instrumentID == 55:
                 return "note.cow_bell", 5
             elif instrumentID in [41, 43, 45]:
@@ -215,146 +268,163 @@
             elif instrumentID in [36, 37, 39]:
                 return "note.snare", 7
             else:
                 return "note.bd", 7
 
     @staticmethod
     def score2time(score: int):
+        """
+        将《我的世界》的计分（以游戏刻计）转为表示时间的字符串
+        """
         return str(int(int(score / 20) / 60)) + ":" + str(int(int(score / 20) % 60))
 
-    def __formProgressBar(
+    def __form_progress_bar(
         self,
-        maxscore: int,
+        max_score: int,
         scoreboard_name: str,
-        progressbar: tuple = (
-            r"▶ %%N [ %%s/%^s %%% __________ %%t|%^t ]",
-            ("§e=§r", "§7=§r"),
-        ),
+        progressbar_style: tuple = DEFAULT_PROGRESSBAR_STYLE,
     ) -> list:
+        """
+        生成进度条
+
+        Parameters
+        ----------
+        maxscore: int
+            midi的乐器ID
+
+        scoreboard_name: str
+            所使用的计分板名称
 
-        pgs_style = progressbar[0]
+        progressbar_style: tuple
+            此参数详见 ../docs/库的生成与功能文档.md#进度条自定义
+
+        Returns
+        -------
+        list[str"指令",]
+        """
+        pgs_style = progressbar_style[0]
         """用于被替换的进度条原始样式"""
 
         """
         | 标识符   | 指定的可变量     |
         |---------|----------------|
         | `%%N`   | 乐曲名(即传入的文件名)|
         | `%%s`   | 当前计分板值     |
         | `%^s`   | 计分板最大值     |
         | `%%t`   | 当前播放时间     |
         | `%^t`   | 曲目总时长       |
         | `%%%`   | 当前进度比率     |
         | `_`     | 用以表示进度条占位|
         """
-        perEach = maxscore / pgs_style.count("_")
+        perEach = max_score / pgs_style.count("_")
 
         result = []
 
         if r"%^s" in pgs_style:
-            pgs_style = pgs_style.replace(r"%^s", str(maxscore))
+            pgs_style = pgs_style.replace(r"%^s", str(max_score))
 
         if r"%^t" in pgs_style:
-            pgs_style = pgs_style.replace(r"%^t", self.score2time(maxscore))
+            pgs_style = pgs_style.replace(r"%^t", self.score2time(max_score))
 
         sbn_pc = scoreboard_name[:2]
         if r"%%%" in pgs_style:
             result.append(
                 'scoreboard objectives add {}PercT dummy "百分比计算"'.format(sbn_pc)
             )
             result.append(
-                self.exeHead.format("@a[scores={" + scoreboard_name + "=1..}]")
+                self.execute_cmd_head.format("@a[scores={" + scoreboard_name + "=1..}]")
                 + "scoreboard players set MaxScore {} {}".format(
-                    scoreboard_name, maxscore
+                    scoreboard_name, max_score
                 )
             )
             result.append(
-                self.exeHead.format("@a[scores={" + scoreboard_name + "=1..}]")
+                self.execute_cmd_head.format("@a[scores={" + scoreboard_name + "=1..}]")
                 + "scoreboard players set n100 {} 100".format(scoreboard_name)
             )
             result.append(
-                self.exeHead.format("@a[scores={" + scoreboard_name + "=1..}]")
+                self.execute_cmd_head.format("@a[scores={" + scoreboard_name + "=1..}]")
                 + "scoreboard players operation @s {} = @s {}".format(
                     sbn_pc + "PercT", scoreboard_name
                 )
             )
             result.append(
-                self.exeHead.format("@a[scores={" + scoreboard_name + "=1..}]")
+                self.execute_cmd_head.format("@a[scores={" + scoreboard_name + "=1..}]")
                 + "scoreboard players operation @s {} *= n100 {}".format(
                     sbn_pc + "PercT", scoreboard_name
                 )
             )
             result.append(
-                self.exeHead.format("@a[scores={" + scoreboard_name + "=1..}]")
+                self.execute_cmd_head.format("@a[scores={" + scoreboard_name + "=1..}]")
                 + "scoreboard players operation @s {} /= MaxScore {}".format(
                     sbn_pc + "PercT", scoreboard_name
                 )
             )
 
         if r"%%t" in pgs_style:
             result.append(
                 'scoreboard objectives add {}TMinT dummy "时间计算：分"'.format(sbn_pc)
             )
             result.append(
                 'scoreboard objectives add {}TSecT dummy "时间计算：秒"'.format(sbn_pc)
             )
             result.append(
-                self.exeHead.format("@a[scores={" + scoreboard_name + "=1..}]")
+                self.execute_cmd_head.format("@a[scores={" + scoreboard_name + "=1..}]")
                 + "scoreboard players set n20 {} 20".format(scoreboard_name)
             )
             result.append(
-                self.exeHead.format("@a[scores={" + scoreboard_name + "=1..}]")
+                self.execute_cmd_head.format("@a[scores={" + scoreboard_name + "=1..}]")
                 + "scoreboard players set n60 {} 60".format(scoreboard_name)
             )
 
             result.append(
-                self.exeHead.format("@a[scores={" + scoreboard_name + "=1..}]")
+                self.execute_cmd_head.format("@a[scores={" + scoreboard_name + "=1..}]")
                 + "scoreboard players operation @s {} = @s {}".format(
                     sbn_pc + "TMinT", scoreboard_name
                 )
             )
             result.append(
-                self.exeHead.format("@a[scores={" + scoreboard_name + "=1..}]")
+                self.execute_cmd_head.format("@a[scores={" + scoreboard_name + "=1..}]")
                 + "scoreboard players operation @s {} /= n20 {}".format(
                     sbn_pc + "TMinT", scoreboard_name
                 )
             )
             result.append(
-                self.exeHead.format("@a[scores={" + scoreboard_name + "=1..}]")
+                self.execute_cmd_head.format("@a[scores={" + scoreboard_name + "=1..}]")
                 + "scoreboard players operation @s {} /= n60 {}".format(
                     sbn_pc + "TMinT", scoreboard_name
                 )
             )
 
             result.append(
-                self.exeHead.format("@a[scores={" + scoreboard_name + "=1..}]")
+                self.execute_cmd_head.format("@a[scores={" + scoreboard_name + "=1..}]")
                 + "scoreboard players operation @s {} = @s {}".format(
                     sbn_pc + "TSecT", scoreboard_name
                 )
             )
             result.append(
-                self.exeHead.format("@a[scores={" + scoreboard_name + "=1..}]")
+                self.execute_cmd_head.format("@a[scores={" + scoreboard_name + "=1..}]")
                 + "scoreboard players operation @s {} /= n20 {}".format(
                     sbn_pc + "TSecT", scoreboard_name
                 )
             )
             result.append(
-                self.exeHead.format("@a[scores={" + scoreboard_name + "=1..}]")
+                self.execute_cmd_head.format("@a[scores={" + scoreboard_name + "=1..}]")
                 + "scoreboard players operation @s {} %= n60 {}".format(
                     sbn_pc + "TSecT", scoreboard_name
                 )
             )
 
         for i in range(pgs_style.count("_")):
             npg_stl = (
-                pgs_style.replace("_", progressbar[1][0], i + 1)
-                .replace("_", progressbar[1][1])
-                .replace(r"%%N", self.midFileName)
+                pgs_style.replace("_", progressbar_style[1][0], i + 1)
+                .replace("_", progressbar_style[1][1])
+                .replace(r"%%N", self.mid_file_name)
                 if r"%%N" in pgs_style
-                else pgs_style.replace("_", progressbar[1][0], i + 1).replace(
-                    "_", progressbar[1][1]
+                else pgs_style.replace("_", progressbar_style[1][0], i + 1).replace(
+                    "_", progressbar_style[1][1]
                 )
             )
             if r"%%s" in npg_stl:
                 npg_stl = npg_stl.replace(
                     r"%%s",
                     '"},{"score":{"name":"*","objective":"'
                     + scoreboard_name
@@ -372,15 +442,15 @@
                     r"%%t",
                     r'"},{"score":{"name":"*","objective":"{-}TMinT"}},{"text":":"},'
                     r'{"score":{"name":"*","objective":"{-}TSecT"}},{"text":"'.replace(
                         r"{-}", sbn_pc
                     ),
                 )
             result.append(
-                self.exeHead.format(
+                self.execute_cmd_head.format(
                     r"@a[scores={"
                     + scoreboard_name
                     + f"={int(i * perEach)}..{math.ceil((i + 1) * perEach)}"
                     + r"}]"
                 )
                 + r'titleraw @s actionbar {"rawtext":[{"text":"'
                 + npg_stl
@@ -406,26 +476,25 @@
         :param scoreboard_name: 我的世界的计分板名称
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :return: tuple(命令列表, 命令个数, 计分板最大值)
         """
         # :param volume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         tracks = []
         if speed == 0:
-            if self.debugMode:
+            if self.debug_mode:
                 raise ZeroSpeedError("播放速度仅可为正实数")
             speed = 1
         MaxVolume = 1 if MaxVolume > 1 else (0.001 if MaxVolume <= 0 else MaxVolume)
 
         commands = 0
         maxscore = 0
 
         # 分轨的思路其实并不好，但这个算法就是这样
         # 所以我建议用第二个方法 _toCmdList_m2
         for i, track in enumerate(self.midi.tracks):
-
             ticks = 0
             instrumentID = 0
             singleTrack = []
 
             for msg in track:
                 ticks += msg.time
                 if msg.is_meta:
@@ -476,15 +545,15 @@
         :param scoreboard_name: 我的世界的计分板名称
         :param MaxVolume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :return: tuple(命令列表, 命令个数, 计分板最大值)
         """
 
         if speed == 0:
-            if self.debugMode:
+            if self.debug_mode:
                 raise ZeroSpeedError("播放速度仅可为正实数")
             speed = 1
         MaxVolume = 1 if MaxVolume > 1 else (0.001 if MaxVolume <= 0 else MaxVolume)
 
         # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
         channels = {
             0: [],
@@ -508,15 +577,15 @@
 
         microseconds = 0
 
         # 我们来用通道统计音乐信息
         for msg in self.midi:
             microseconds += msg.time * 1000  # 任何人都tm不要动这里，这里循环方式不是track，所以，这里的计时方式不一样
             if not msg.is_meta:
-                if self.debugMode:
+                if self.debug_mode:
                     try:
                         if msg.channel > 15:
                             raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
                     except AttributeError:
                         pass
 
                 if msg.type == "program_change":
@@ -558,39 +627,38 @@
                 SpecialBits = True
             else:
                 SpecialBits = False
 
             nowTrack = []
 
             for msg in channels[i]:
-
                 if msg[0] == "PgmC":
                     InstID = msg[1]
 
                 elif msg[0] == "NoteS":
                     try:
                         soundID, _X = (
                             self.__bitInst2ID_withX(InstID)
                             if SpecialBits
                             else self.__Inst2soundID_withX(InstID)
                         )
                     except UnboundLocalError as E:
-                        if self.debugMode:
+                        if self.debug_mode:
                             raise NotDefineProgramError(f"未定义乐器便提前演奏。\n{E}")
                         else:
                             soundID, _X = (
                                 self.__bitInst2ID_withX(-1)
                                 if SpecialBits
                                 else self.__Inst2soundID_withX(-1)
                             )
                     score_now = round(msg[-1] / float(speed) / 50)
                     maxScore = max(maxScore, score_now)
 
                     nowTrack.append(
-                        self.exeHead.format(
+                        self.execute_cmd_head.format(
                             "@a[scores=({}={})]".format(scoreboard_name, score_now)
                             .replace("(", r"{")
                             .replace(")", r"}")
                         )
                         + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
                         f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                     )
@@ -613,68 +681,93 @@
         :param scoreboard_name: 我的世界的计分板名称
         :param MaxVolume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :return: tuple(命令列表, 命令个数, 计分板最大值)
         """
 
         if speed == 0:
-            if self.debugMode:
+            if self.debug_mode:
                 raise ZeroSpeedError("播放速度仅可为正实数")
             speed = 1
         MaxVolume = 1 if MaxVolume > 1 else (0.001 if MaxVolume <= 0 else MaxVolume)
 
         # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
-        channels = {0: {}, 1: {}, 2: {}, 3: {}, 4: {}, 5: {}, 6: {}, 7: {}, 8: {}, 9: {}, 10: {}, 11: {}, 12: {}, 13: {}, 14: {}, 15: {}, 16: {}}
+        channels = {
+            0: {},
+            1: {},
+            2: {},
+            3: {},
+            4: {},
+            5: {},
+            6: {},
+            7: {},
+            8: {},
+            9: {},
+            10: {},
+            11: {},
+            12: {},
+            13: {},
+            14: {},
+            15: {},
+            16: {},
+        }
 
         # 我们来用通道统计音乐信息
         # 但是是用分轨的思路的
         for track_no, track in enumerate(self.midi.tracks):
-            
             microseconds = 0
 
             for msg in track:
-
                 if msg.time != 0:
                     try:
-                        microseconds += msg.time * tempo / self.midi.ticks_per_beat / 1000
+                        microseconds += (
+                            msg.time * tempo / self.midi.ticks_per_beat / 1000
+                        )
                         # print(microseconds)
                     except NameError:
-                        if self.debugMode:
+                        if self.debug_mode:
                             raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
                         else:
-                            microseconds += (msg.time * mido.midifiles.midifiles.DEFAULT_TEMPO / self.midi.ticks_per_beat) / 1000
+                            microseconds += (
+                                msg.time
+                                * mido.midifiles.midifiles.DEFAULT_TEMPO
+                                / self.midi.ticks_per_beat
+                            ) / 1000
 
                 if msg.is_meta:
                     if msg.type == "set_tempo":
                         tempo = msg.tempo
-                        if self.debugMode:
+                        if self.debug_mode:
                             self.prt(f"TEMPO更改：{tempo}（毫秒每拍）")
                 else:
-
-                    if self.debugMode:
+                    if self.debug_mode:
                         try:
                             if msg.channel > 15:
                                 raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
                         except AttributeError:
                             pass
-                    
+
                     if not track_no in channels[msg.channel].keys():
                         channels[msg.channel][track_no] = []
                     if msg.type == "program_change":
-                        channels[msg.channel][track_no].append(("PgmC", msg.program, microseconds))
+                        channels[msg.channel][track_no].append(
+                            ("PgmC", msg.program, microseconds)
+                        )
 
                     elif msg.type == "note_on" and msg.velocity != 0:
                         channels[msg.channel][track_no].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
                         msg.type == "note_off"
                     ):
-                        channels[msg.channel][track_no].append(("NoteE", msg.note, microseconds))
+                        channels[msg.channel][track_no].append(
+                            ("NoteE", msg.note, microseconds)
+                        )
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
 
         1 切换乐器消息
         ("PgmC", 切换后的乐器ID: int, 距离演奏开始的毫秒)
 
@@ -689,49 +782,48 @@
         maxScore = 0
 
         # 此处 我们把通道视为音轨
         for i in channels.keys():
             # 如果当前通道为空 则跳过
             if not channels[i]:
                 continue
-            
+
             # 第十通道是打击乐通道
             SpecialBits = True if i == 9 else False
 
             # nowChannel = []
 
-            for track_no,track in channels[i].items():
-
+            for track_no, track in channels[i].items():
                 nowTrack = []
 
                 for msg in track:
                     if msg[0] == "PgmC":
                         InstID = msg[1]
 
                     elif msg[0] == "NoteS":
                         try:
                             soundID, _X = (
                                 self.__bitInst2ID_withX(InstID)
                                 if SpecialBits
                                 else self.__Inst2soundID_withX(InstID)
                             )
                         except UnboundLocalError as E:
-                            if self.debugMode:
+                            if self.debug_mode:
                                 raise NotDefineProgramError(f"未定义乐器便提前演奏。\n{E}")
                             else:
                                 soundID, _X = (
                                     self.__bitInst2ID_withX(-1)
                                     if SpecialBits
                                     else self.__Inst2soundID_withX(-1)
                                 )
                         score_now = round(msg[-1] / float(speed) / 50)
                         maxScore = max(maxScore, score_now)
 
                         nowTrack.append(
-                            self.exeHead.format(
+                            self.execute_cmd_head.format(
                                 "@a[scores=({}={})]".format(scoreboard_name, score_now)
                                 .replace("(", r"{")
                                 .replace(")", r"}")
                             )
                             + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
                             f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                         )
@@ -756,41 +848,38 @@
         :param MaxVolume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :return: tuple(命令列表, 命令个数, 计分板最大值)
         """
         # TODO: 这里的时间转换不知道有没有问题
 
         if speed == 0:
-            if self.debugMode:
+            if self.debug_mode:
                 raise ZeroSpeedError("播放速度仅可为正实数")
             speed = 1
         MaxVolume = 1 if MaxVolume > 1 else (0.001 if MaxVolume <= 0 else MaxVolume)
 
         # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
         channels = [[], [], [], [], [], [], [], [], [], [], [], [], [], [], [], []]
 
         # 我们来用通道统计音乐信息
         for i, track in enumerate(self.midi.tracks):
-
             microseconds = 0
 
             for msg in track:
-
                 if msg.time != 0:
                     try:
                         microseconds += msg.time * tempo / self.midi.ticks_per_beat
                     except NameError:
                         raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
 
                 if msg.is_meta:
                     if msg.type == "set_tempo":
                         tempo = msg.tempo
                 else:
-
-                    if self.debugMode:
+                    if self.debug_mode:
                         try:
                             if msg.channel > 15:
                                 raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
                         except AttributeError:
                             pass
 
                     if msg.type == "program_change":
@@ -829,15 +918,14 @@
         for i in range(len(channels)):
             # 如果当前通道为空 则跳过
 
             noteMsgs = []
             MsgIndex = []
 
             for msg in channels[i]:
-
                 if msg[0] == "PgmC":
                     InstID = msg[1]
 
                 elif msg[0] == "NoteS":
                     noteMsgs.append(msg[1:])
                     MsgIndex.append(msg[1])
 
@@ -897,15 +985,14 @@
             else:
                 CheckFirstChannel = False
                 SpecialBits = False
 
             nowTrack = []
 
             for note in track:
-
                 for every_note in _linearFun(note):
                     # 应该是计算的时候出了点小问题
                     # 我们应该用一个MC帧作为时间单位而不是半秒
 
                     if SpecialBits:
                         soundID, _X = self.__bitInst2ID_withX(InstID)
                     else:
@@ -942,22 +1029,21 @@
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :param player: 玩家选择器，默认为`@a`
         :return: 全部指令列表[ ( str指令, int距离上一个指令的延迟 ),...]
         """
         tracks = {}
 
         if speed == 0:
-            if self.debugMode:
+            if self.debug_mode:
                 raise ZeroSpeedError("播放速度仅可为正实数")
             speed = 1
 
         MaxVolume = 1 if MaxVolume > 1 else (0.001 if MaxVolume <= 0 else MaxVolume)
 
         for i, track in enumerate(self.midi.tracks):
-
             instrumentID = 0
             ticks = 0
 
             for msg in track:
                 ticks += msg.time
                 if msg.is_meta:
                     if msg.type == "set_tempo":
@@ -969,21 +1055,21 @@
                         now_tick = round(
                             (ticks * tempo)
                             / ((self.midi.ticks_per_beat * float(speed)) * 50000)
                         )
                         soundID, _X = self.__Inst2soundID_withX(instrumentID)
                         try:
                             tracks[now_tick].append(
-                                self.exeHead.format(player)
+                                self.execute_cmd_head.format(player)
                                 + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg.velocity / 128} "
                                 f"{2 ** ((msg.note - 60 - _X) / 12)}"
                             )
                         except KeyError:
                             tracks[now_tick] = [
-                                self.exeHead.format(player)
+                                self.execute_cmd_head.format(player)
                                 + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg.velocity / 128} "
                                 f"{2 ** ((msg.note - 60 - _X) / 12)}"
                             ]
 
         results = []
 
         all_ticks = list(tracks.keys())
@@ -1014,15 +1100,15 @@
         :param MaxVolume: 最大播放音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :param player: 玩家选择器，默认为`@a`
         :return: 全部指令列表[ ( str指令, int距离上一个指令的延迟 ),...]
         """
         tracks = {}
         if speed == 0:
-            if self.debugMode:
+            if self.debug_mode:
                 raise ZeroSpeedError("播放速度仅可为正实数")
             speed = 1
 
         MaxVolume = 1 if MaxVolume > 1 else (0.001 if MaxVolume <= 0 else MaxVolume)
 
         # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
         channels = {
@@ -1046,29 +1132,32 @@
         }
 
         microseconds = 0
 
         # 我们来用通道统计音乐信息
         for msg in self.midi:
             try:
-                microseconds += msg.time * 1000  # 任何人都tm不要动这里，这里循环方式不是track，所以，这里的计时方式不一样
+                microseconds += (
+                    msg.time * 1000
+                )  # 任何人都tm不要动这里，这里循环方式不是track，所以，这里的计时方式不一样
 
                 # print(microseconds)
             except NameError:
-                if self.debugMode:
+                if self.debug_mode:
                     raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
                 else:
-                    microseconds += msg.time * 1000  # 任何人都tm不要动这里，这里循环方式不是track，所以，这里的计时方式不一样
+                    microseconds += (
+                        msg.time * 1000
+                    )  # 任何人都tm不要动这里，这里循环方式不是track，所以，这里的计时方式不一样
 
             if msg.is_meta:
                 if msg.type == "set_tempo":
                     tempo = msg.tempo
             else:
-
-                if self.debugMode:
+                if self.debug_mode:
                     try:
                         if msg.channel > 15:
                             raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
                     except AttributeError:
                         pass
 
                 if msg.type == "program_change":
@@ -1105,45 +1194,44 @@
 
             if i == 9:
                 SpecialBits = True
             else:
                 SpecialBits = False
 
             for msg in channels[i]:
-
                 if msg[0] == "PgmC":
                     InstID = msg[1]
 
                 elif msg[0] == "NoteS":
                     try:
                         soundID, _X = (
                             self.__bitInst2ID_withX(InstID)
                             if SpecialBits
                             else self.__Inst2soundID_withX(InstID)
                         )
                     except UnboundLocalError as E:
-                        if self.debugMode:
+                        if self.debug_mode:
                             raise NotDefineProgramError(f"未定义乐器便提前演奏。\n{E}")
                         else:
                             soundID, _X = (
                                 self.__bitInst2ID_withX(-1)
                                 if SpecialBits
                                 else self.__Inst2soundID_withX(-1)
                             )
                     score_now = round(msg[-1] / float(speed) / 50)
 
                     try:
                         tracks[score_now].append(
-                            self.exeHead.format(player)
+                            self.execute_cmd_head.format(player)
                             + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
                             f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                         )
                     except KeyError:
                         tracks[score_now] = [
-                            self.exeHead.format(player)
+                            self.execute_cmd_head.format(player)
                             + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
                             f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                         ]
 
         all_ticks = list(tracks.keys())
 
         for i in range(len(all_ticks)):
@@ -1174,70 +1262,95 @@
         """
         使用金羿的转换思路，将midi转换为我的世界命令列表，并输出每个音符之后的延迟
         :param MaxVolume: 最大播放音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :param player: 玩家选择器，默认为`@a`
         :return: 全部指令列表[ ( str指令, int距离上一个指令的延迟 ),...]
         """
-        
+
         if speed == 0:
-            if self.debugMode:
+            if self.debug_mode:
                 raise ZeroSpeedError("播放速度仅可为正实数")
             speed = 1
         MaxVolume = 1 if MaxVolume > 1 else (0.001 if MaxVolume <= 0 else MaxVolume)
 
         # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
-        channels = {0: {}, 1: {}, 2: {}, 3: {}, 4: {}, 5: {}, 6: {}, 7: {}, 8: {}, 9: {}, 10: {}, 11: {}, 12: {}, 13: {}, 14: {}, 15: {}, 16: {}}
+        channels = {
+            0: {},
+            1: {},
+            2: {},
+            3: {},
+            4: {},
+            5: {},
+            6: {},
+            7: {},
+            8: {},
+            9: {},
+            10: {},
+            11: {},
+            12: {},
+            13: {},
+            14: {},
+            15: {},
+            16: {},
+        }
 
         # 我们来用通道统计音乐信息
         # 但是是用分轨的思路的
         for track_no, track in enumerate(self.midi.tracks):
-            
             microseconds = 0
 
             for msg in track:
-
                 if msg.time != 0:
                     try:
-                        microseconds += msg.time * tempo / self.midi.ticks_per_beat / 1000
+                        microseconds += (
+                            msg.time * tempo / self.midi.ticks_per_beat / 1000
+                        )
                         # print(microseconds)
                     except NameError:
-                        if self.debugMode:
+                        if self.debug_mode:
                             raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
                         else:
-                            microseconds += (msg.time * mido.midifiles.midifiles.DEFAULT_TEMPO / self.midi.ticks_per_beat) / 1000
+                            microseconds += (
+                                msg.time
+                                * mido.midifiles.midifiles.DEFAULT_TEMPO
+                                / self.midi.ticks_per_beat
+                            ) / 1000
 
                 if msg.is_meta:
                     if msg.type == "set_tempo":
                         tempo = msg.tempo
-                        if self.debugMode:
+                        if self.debug_mode:
                             self.prt(f"TEMPO更改：{tempo}（毫秒每拍）")
                 else:
-
-                    if self.debugMode:
+                    if self.debug_mode:
                         try:
                             if msg.channel > 15:
                                 raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
                         except AttributeError:
                             pass
-                    
+
                     if not track_no in channels[msg.channel].keys():
                         channels[msg.channel][track_no] = []
                     if msg.type == "program_change":
-                        channels[msg.channel][track_no].append(("PgmC", msg.program, microseconds))
+                        channels[msg.channel][track_no].append(
+                            ("PgmC", msg.program, microseconds)
+                        )
 
                     elif msg.type == "note_on" and msg.velocity != 0:
                         channels[msg.channel][track_no].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
                         msg.type == "note_off"
                     ):
-                        channels[msg.channel][track_no].append(("NoteE", msg.note, microseconds))
+                        channels[msg.channel][track_no].append(
+                            ("NoteE", msg.note, microseconds)
+                        )
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
 
         1 切换乐器消息
         ("PgmC", 切换后的乐器ID: int, 距离演奏开始的毫秒)
 
@@ -1250,67 +1363,73 @@
         tracks = {}
 
         # 此处 我们把通道视为音轨
         for i in channels.keys():
             # 如果当前通道为空 则跳过
             if not channels[i]:
                 continue
-            
+
             # 第十通道是打击乐通道
             SpecialBits = True if i == 9 else False
 
             # nowChannel = []
 
-            for track_no,track in channels[i].items():
-
+            for track_no, track in channels[i].items():
                 for msg in track:
-
                     if msg[0] == "PgmC":
                         InstID = msg[1]
 
                     elif msg[0] == "NoteS":
                         try:
                             soundID, _X = (
                                 self.__bitInst2ID_withX(InstID)
                                 if SpecialBits
                                 else self.__Inst2soundID_withX(InstID)
                             )
                         except UnboundLocalError as E:
-                            if self.debugMode:
+                            if self.debug_mode:
                                 raise NotDefineProgramError(f"未定义乐器便提前演奏。\n{E}")
                             else:
                                 soundID, _X = (
                                     self.__bitInst2ID_withX(-1)
                                     if SpecialBits
                                     else self.__Inst2soundID_withX(-1)
                                 )
                         score_now = round(msg[-1] / float(speed) / 50)
 
                         try:
                             tracks[score_now].append(
-                                self.exeHead.format(player)
+                                self.execute_cmd_head.format(player)
                                 + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
                                 f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                             )
                         except KeyError:
                             tracks[score_now] = [
-                                self.exeHead.format(player)
+                                self.execute_cmd_head.format(player)
                                 + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
                                 f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                             ]
 
         all_ticks = list(tracks.keys())
         results = []
 
         for i in range(len(all_ticks)):
             for j in range(len(tracks[all_ticks[i]])):
                 results.append(
                     (
                         tracks[all_ticks[i]][j],
-                        (0 if j != 0 else (all_ticks[i] - all_ticks[i - 1] if i != 0 else all_ticks[i])),
+                        (
+                            0
+                            if j != 0
+                            else (
+                                all_ticks[i] - all_ticks[i - 1]
+                                if i != 0
+                                else all_ticks[i]
+                            )
+                        ),
                     )
                 )
 
         return [results, max(all_ticks)]
 
     def to_mcpack(
         self,
@@ -1336,63 +1455,63 @@
         cmdlist, maxlen, maxscore = self.methods[method - 1](
             scoreboard_name, volume, speed
         )
         # except:
         #     return (False, f"无法找到算法ID{method}对应的转换算法")
 
         # 当文件f夹{self.outputPath}/temp/functions存在时清空其下所有项目，然后创建
-        if os.path.exists(f"{self.outputPath}/temp/functions/"):
-            shutil.rmtree(f"{self.outputPath}/temp/functions/")
-        os.makedirs(f"{self.outputPath}/temp/functions/mscplay")
+        if os.path.exists(f"{self.output_path}/temp/functions/"):
+            shutil.rmtree(f"{self.output_path}/temp/functions/")
+        os.makedirs(f"{self.output_path}/temp/functions/mscplay")
 
         # 写入manifest.json
-        if not os.path.exists(f"{self.outputPath}/temp/manifest.json"):
+        if not os.path.exists(f"{self.output_path}/temp/manifest.json"):
             with open(
-                f"{self.outputPath}/temp/manifest.json", "w", encoding="utf-8"
+                f"{self.output_path}/temp/manifest.json", "w", encoding="utf-8"
             ) as f:
                 f.write(
                     '{\n  "format_version": 1,\n  "header": {\n    "description": "'
-                    + self.midFileName
+                    + self.mid_file_name
                     + ' Pack : behavior pack",\n    "version": [ 0, 0, 1 ],\n    "name": "'
-                    + self.midFileName
+                    + self.mid_file_name
                     + 'Pack",\n    "uuid": "'
                     + str(uuid.uuid4())
                     + '"\n  },\n  "modules": [\n    {\n      "description": "'
-                    + f"the Player of the Music {self.midFileName}"
+                    + f"the Player of the Music {self.mid_file_name}"
                     + '",\n      "type": "data",\n      "version": [ 0, 0, 1 ],\n      "uuid": "'
                     + str(uuid.uuid4())
                     + '"\n    }\n  ]\n}'
                 )
         else:
             with open(
-                f"{self.outputPath}/temp/manifest.json", "r", encoding="utf-8"
+                f"{self.output_path}/temp/manifest.json", "r", encoding="utf-8"
             ) as manifest:
                 data = json.loads(manifest.read())
                 data["header"][
                     "description"
-                ] = f"the Player of the Music {self.midFileName}"
-                data["header"]["name"] = self.midFileName
+                ] = f"the Player of the Music {self.mid_file_name}"
+                data["header"]["name"] = self.mid_file_name
                 data["header"]["uuid"] = str(uuid.uuid4())
                 data["modules"][0]["description"] = "None"
                 data["modules"][0]["uuid"] = str(uuid.uuid4())
                 manifest.close()
-            open(f"{self.outputPath}/temp/manifest.json", "w", encoding="utf-8").write(
+            open(f"{self.output_path}/temp/manifest.json", "w", encoding="utf-8").write(
                 json.dumps(data)
             )
 
         # 将命令列表写入文件
         index_file = open(
-            f"{self.outputPath}/temp/functions/index.mcfunction", "w", encoding="utf-8"
+            f"{self.output_path}/temp/functions/index.mcfunction", "w", encoding="utf-8"
         )
         for track in cmdlist:
             index_file.write(
                 "function mscplay/track" + str(cmdlist.index(track) + 1) + "\n"
             )
             with open(
-                f"{self.outputPath}/temp/functions/mscplay/track{cmdlist.index(track) + 1}.mcfunction",
+                f"{self.output_path}/temp/functions/mscplay/track{cmdlist.index(track) + 1}.mcfunction",
                 "w",
                 encoding="utf-8",
             ) as f:
                 f.write("\n".join(track))
         index_file.writelines(
             (
                 "scoreboard players add @a[scores={"
@@ -1411,71 +1530,290 @@
                 if isAutoReset
                 else "",
                 f"function mscplay/progressShow\n" if progressbar else "",
             )
         )
 
         if progressbar:
-            if progressbar:
+            # 此处是对于仅有 True 的参数和自定义参数的判断
+            # 改这一行没🐎
+            if progressbar is True:
                 with open(
-                    f"{self.outputPath}/temp/functions/mscplay/progressShow.mcfunction",
+                    f"{self.output_path}/temp/functions/mscplay/progressShow.mcfunction",
                     "w",
                     encoding="utf-8",
                 ) as f:
                     f.writelines(
-                        "\n".join(self.__formProgressBar(maxscore, scoreboard_name))
+                        "\n".join(self.__form_progress_bar(maxscore, scoreboard_name))
                     )
             else:
                 with open(
-                    f"{self.outputPath}/temp/functions/mscplay/progressShow.mcfunction",
+                    f"{self.output_path}/temp/functions/mscplay/progressShow.mcfunction",
                     "w",
                     encoding="utf-8",
                 ) as f:
                     f.writelines(
                         "\n".join(
-                            self.__formProgressBar(
+                            self.__form_progress_bar(
                                 maxscore, scoreboard_name, progressbar
                             )
                         )
                     )
 
         index_file.close()
 
-        if os.path.exists(f"{self.outputPath}/{self.midFileName}.mcpack"):
-            os.remove(f"{self.outputPath}/{self.midFileName}.mcpack")
+        if os.path.exists(f"{self.output_path}/{self.mid_file_name}.mcpack"):
+            os.remove(f"{self.output_path}/{self.mid_file_name}.mcpack")
         compress_zipfile(
-            f"{self.outputPath}/temp/", f"{self.outputPath}/{self.midFileName}.mcpack"
+            f"{self.output_path}/temp/",
+            f"{self.output_path}/{self.mid_file_name}.mcpack",
         )
 
-        shutil.rmtree(f"{self.outputPath}/temp/")
+        shutil.rmtree(f"{self.output_path}/temp/")
 
         return True, maxlen, maxscore
 
-    def to_mcstructure_file_with_delay(
+    def to_mcpack_with_delay(
         self,
         method: int = 1,
         volume: float = 1.0,
         speed: float = 1.0,
         progressbar: Union[bool, tuple] = False,
         player: str = "@a",
-        author: str = "Eilles",
         max_height: int = 64,
     ):
         """
-        使用method指定的转换算法，将midi转换为BDX结构文件
+        使用method指定的转换算法，将midi转换为mcstructure结构文件后打包成mcpack文件
         :param method: 转换算法
         :param author: 作者名称
         :param progressbar: 进度条，（当此参数为True时使用默认进度条，为其他的值为真的参数时识别为进度条自定义参数，为其他值为假的时候不生成进度条）
         :param max_height: 生成结构最大高度
         :param volume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :param player: 玩家选择器，默认为`@a`
         :return 成功与否，成功返回(True,未经过压缩的源,结构占用大小)，失败返回(False,str失败原因)
         """
-        pass
+
+        if self.enable_old_exe_format:
+            raise CommandFormatError("使用mcstructure结构文件导出时不支持旧版本的指令格式。")
+
+        command_list, max_delay = self.methods_byDelay[method - 1](
+            volume,
+            speed,
+            player,
+        )
+
+        # 此处是对于仅有 True 的参数和自定义参数的判断
+        # 改这一行没🐎
+        if progressbar is True:
+            progressbar = DEFAULT_PROGRESSBAR_STYLE
+
+        if not os.path.exists(self.output_path):
+            os.makedirs(self.output_path)
+
+        # 当文件f夹{self.outputPath}/temp/存在时清空其下所有项目，然后创建
+        if os.path.exists(f"{self.output_path}/temp/"):
+            shutil.rmtree(f"{self.output_path}/temp/")
+        os.makedirs(f"{self.output_path}/temp/functions/")
+        os.makedirs(f"{self.output_path}/temp/structures/")
+
+        # 写入manifest.json
+        with open(f"{self.output_path}/temp/manifest.json", "w", encoding="utf-8") as f:
+            json.dump(
+                {
+                    "format_version": 1,
+                    "header": {
+                        "description": f"the Music {self.mid_file_name}",
+                        "version": [0, 0, 1],
+                        "name": self.mid_file_name,
+                        "uuid": str(uuid.uuid4()),
+                    },
+                    "modules": [
+                        {
+                            "description": "Ryoun mub Pack : behavior pack",
+                            "type": "data",
+                            "version": [0, 0, 1],
+                            "uuid": str(uuid.uuid4()),
+                        }
+                    ],
+                },
+                fp=f,
+            )
+
+        # 将命令列表写入文件
+        index_file = open(
+            f"{self.output_path}/temp/functions/index.mcfunction", "w", encoding="utf-8"
+        )
+
+        struct, size, end_pos = commands_to_structure(command_list, max_height - 1)
+        with open(
+            os.path.abspath(
+                os.path.join(
+                    self.output_path,
+                    "temp/structures/",
+                    f"{self.mid_file_name}_main.mcstructure",
+                )
+            ),
+            "wb+",
+        ) as f:
+            struct.dump(f)
+
+        del struct
+
+        if progressbar:
+            scb_name = self.mid_file_name[:5] + "Pgb"
+            index_file.write(
+                "scoreboard objectives add {0} dummy {0}计\n".format(scb_name)
+            )
+
+            struct_a = Structure(
+                (1, 1, 1),
+            )
+            struct_a.set_block(
+                (0, 0, 0),
+                form_command_block_in_NBT_struct(
+                    r"scoreboard players add {} {} 1".format(player, scb_name),
+                    (0, 0, 0),
+                    1,
+                    1,
+                    customName="显示进度条并加分",
+                ),
+            )
+
+            with open(
+                os.path.abspath(
+                    os.path.join(
+                        self.output_path,
+                        "temp/structures/",
+                        f"{self.mid_file_name}_start.mcstructure",
+                    )
+                ),
+                "wb+",
+            ) as f:
+                struct_a.dump(f)
+
+            index_file.write(f"structure load {self.mid_file_name}_start ~ ~ ~1\n")
+
+            pgb_struct, pgbSize, pgbNowPos = commands_to_structure(
+                [
+                    (i, 0)
+                    for i in self.__form_progress_bar(max_delay, scb_name, progressbar)
+                ],
+                max_height - 1,
+            )
+
+            with open(
+                os.path.abspath(
+                    os.path.join(
+                        self.output_path,
+                        "temp/structures/",
+                        f"{self.mid_file_name}_pgb.mcstructure",
+                    )
+                ),
+                "wb+",
+            ) as f:
+                pgb_struct.dump(f)
+
+            index_file.write(f"structure load {self.mid_file_name}_pgb ~ ~1 ~1\n")
+
+            struct_a = Structure(
+                (1, 1, 1),
+            )
+            struct_a.set_block(
+                (0, 0, 0),
+                form_command_block_in_NBT_struct(
+                    r"scoreboard players reset {} {}".format(player, scb_name),
+                    (0, 0, 0),
+                    1,
+                    1,
+                    customName="重置进度条计分板",
+                ),
+            )
+
+            with open(
+                os.path.abspath(
+                    os.path.join(
+                        self.output_path,
+                        "temp/structures/",
+                        f"{self.mid_file_name}_reset.mcstructure",
+                    )
+                ),
+                "wb+",
+            ) as f:
+                struct_a.dump(f)
+
+            del struct_a, pgb_struct
+
+            index_file.write(
+                f"structure load {self.mid_file_name}_reset ~{pgbSize[0]+2} ~ ~1\n"
+            )
+
+            index_file.write(
+                f"structure load {self.mid_file_name}_main ~{pgbSize[0]+2} ~1 ~1\n"
+            )
+
+        else:
+            index_file.write(f"structure load {self.mid_file_name}_main ~ ~ ~1\n")
+
+        index_file.close()
+
+        if os.path.exists(f"{self.output_path}/{self.mid_file_name}.mcpack"):
+            os.remove(f"{self.output_path}/{self.mid_file_name}.mcpack")
+        compress_zipfile(
+            f"{self.output_path}/temp/",
+            f"{self.output_path}/{self.mid_file_name}.mcpack",
+        )
+
+        shutil.rmtree(f"{self.output_path}/temp/")
+
+        return True, len(command_list), max_delay
+
+    def to_mcstructure_file_with_delay(
+        self,
+        method: int = 1,
+        volume: float = 1.0,
+        speed: float = 1.0,
+        player: str = "@a",
+        max_height: int = 64,
+    ):
+        """
+        使用method指定的转换算法，将midi转换为mcstructure结构文件
+        :param method: 转换算法
+        :param author: 作者名称
+        :param progressbar: 进度条，（当此参数为True时使用默认进度条，为其他的值为真的参数时识别为进度条自定义参数，为其他值为假的时候不生成进度条）
+        :param max_height: 生成结构最大高度
+        :param volume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
+        :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
+        :param player: 玩家选择器，默认为`@a`
+        :return 成功与否，成功返回(True,未经过压缩的源,结构占用大小)，失败返回(False,str失败原因)
+        """
+
+        if self.enable_old_exe_format:
+            raise CommandFormatError("使用mcstructure结构文件导出时不支持旧版本的指令格式。")
+
+        cmd_list, max_delay = self.methods_byDelay[method - 1](
+            volume,
+            speed,
+            player,
+        )
+
+        if not os.path.exists(self.output_path):
+            os.makedirs(self.output_path)
+
+        struct, size, end_pos = commands_to_structure(cmd_list, max_height - 1)
+
+        with open(
+            os.path.abspath(
+                os.path.join(self.output_path, f"{self.mid_file_name}.mcstructure")
+            ),
+            "wb+",
+        ) as f:
+            struct.dump(f)
+
+        return True, size, max_delay
 
     def to_BDX_file(
         self,
         method: int = 1,
         volume: float = 1.0,
         speed: float = 1.0,
         progressbar: Union[bool, tuple] = False,
@@ -1499,19 +1837,21 @@
         # try:
         cmdlist, total_count, maxScore = self.methods[method - 1](
             scoreboard_name, volume, speed
         )
         # except Exception as E:
         #     return (False, f"无法找到算法ID{method}对应的转换算法: {E}")
 
-        if not os.path.exists(self.outputPath):
-            os.makedirs(self.outputPath)
+        if not os.path.exists(self.output_path):
+            os.makedirs(self.output_path)
 
         with open(
-            os.path.abspath(os.path.join(self.outputPath, f"{self.midFileName}.bdx")),
+            os.path.abspath(
+                os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
+            ),
             "w+",
         ) as f:
             f.write("BD@")
 
         _bytes = (
             b"BDX\x00"
             + author.encode("utf-8")
@@ -1529,45 +1869,49 @@
                 + scoreboard_name
                 + "="
                 + str(maxScore + 20)
                 + "}] "
                 + scoreboard_name,
             )
 
-        cmdBytes, size, finalPos = to_BDX_bytes(
+        cmdBytes, size, finalPos = commands_to_BDX_bytes(
             [(i, 0) for i in commands], max_height - 1
         )
-        # 此处是对于仅有 True 的参数和自定义参数的判断
+
         if progressbar:
-            pgbBytes, pgbSize, pgbNowPos = to_BDX_bytes(
+            pgbBytes, pgbSize, pgbNowPos = commands_to_BDX_bytes(
                 [
                     (i, 0)
                     for i in (
-                        self.__formProgressBar(maxScore, scoreboard_name)
-                        if progressbar
-                        else self.__formProgressBar(
+                        self.__form_progress_bar(maxScore, scoreboard_name)
+                        # 此处是对于仅有 True 的参数和自定义参数的判断
+                        # 改这一行没🐎
+                        if progressbar is True
+                        else self.__form_progress_bar(
                             maxScore, scoreboard_name, progressbar
                         )
                     )
                 ],
                 max_height - 1,
             )
             _bytes += pgbBytes
-            _bytes += move(y, -pgbNowPos[1])
-            _bytes += move(z, -pgbNowPos[2])
-            _bytes += move(x, 2)
+            _bytes += bdx_move(y, -pgbNowPos[1])
+            _bytes += bdx_move(z, -pgbNowPos[2])
+            _bytes += bdx_move(x, 2)
 
             size[0] += 2 + pgbSize[0]
             size[1] = max(size[1], pgbSize[1])
             size[2] = max(size[2], pgbSize[2])
 
         _bytes += cmdBytes
 
         with open(
-            os.path.abspath(os.path.join(self.outputPath, f"{self.midFileName}.bdx")),
+            os.path.abspath(
+                os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
+            ),
             "ab+",
         ) as f:
             f.write(brotli.compress(_bytes + b"XE"))
 
         return True, total_count, maxScore, size, finalPos
 
     def to_BDX_file_with_delay(
@@ -1597,79 +1941,81 @@
             volume,
             speed,
             player,
         )
         # except Exception as E:
         #     return (False, f"无法找到算法ID{method}对应的转换算法\n{E}")
 
-        if not os.path.exists(self.outputPath):
-            os.makedirs(self.outputPath)
+        if not os.path.exists(self.output_path):
+            os.makedirs(self.output_path)
 
         with open(
-            os.path.abspath(os.path.join(self.outputPath, f"{self.midFileName}.bdx")),
+            os.path.abspath(
+                os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
+            ),
             "w+",
         ) as f:
             f.write("BD@")
 
         _bytes = (
             b"BDX\x00"
             + author.encode("utf-8")
             + b" & Musicreater\x00\x01command_block\x00"
         )
 
         # 此处是对于仅有 True 的参数和自定义参数的判断
-        if progressbar:
-            progressbar = (
-                r"▶ %%N [ %%s/%^s %%% __________ %%t|%^t ]",
-                ("§e=§r", "§7=§r"),
-            )
+        # 改这一行没🐎
+        if progressbar is True:
+            progressbar = DEFAULT_PROGRESSBAR_STYLE
 
-        cmdBytes, size, finalPos = to_BDX_bytes(cmdlist, max_height - 1)
+        cmdBytes, size, finalPos = commands_to_BDX_bytes(cmdlist, max_height - 1)
 
         if progressbar:
-            scb_name = self.midFileName[:5] + "Pgb"
+            scb_name = self.mid_file_name[:5] + "Pgb"
             _bytes += form_command_block_in_BDX_bytes(
-                r"scoreboard objectives add {} dummy {}播放用".replace(r"{}", scb_name),
+                r"scoreboard objectives add {} dummy {}计".replace(r"{}", scb_name),
                 1,
                 customName="初始化进度条",
             )
-            _bytes += move(z, 2)
+            _bytes += bdx_move(z, 2)
             _bytes += form_command_block_in_BDX_bytes(
                 r"scoreboard players add {} {} 1".format(player, scb_name),
                 1,
                 1,
                 customName="显示进度条并加分",
             )
-            _bytes += move(y, 1)
-            pgbBytes, pgbSize, pgbNowPos = to_BDX_bytes(
+            _bytes += bdx_move(y, 1)
+            pgbBytes, pgbSize, pgbNowPos = commands_to_BDX_bytes(
                 [
                     (i, 0)
-                    for i in self.__formProgressBar(max_delay, scb_name, progressbar)
+                    for i in self.__form_progress_bar(max_delay, scb_name, progressbar)
                 ],
                 max_height - 1,
             )
             _bytes += pgbBytes
-            _bytes += move(y, -1 - pgbNowPos[1])
-            _bytes += move(z, -2 - pgbNowPos[2])
-            _bytes += move(x, 2)
+            _bytes += bdx_move(y, -1 - pgbNowPos[1])
+            _bytes += bdx_move(z, -2 - pgbNowPos[2])
+            _bytes += bdx_move(x, 2)
             _bytes += form_command_block_in_BDX_bytes(
                 r"scoreboard players reset {} {}".format(player, scb_name),
                 1,
                 customName="置零进度条",
             )
-            _bytes += move(y, 1)
+            _bytes += bdx_move(y, 1)
             size[0] += 2 + pgbSize[0]
             size[1] = max(size[1], pgbSize[1])
             size[2] = max(size[2], pgbSize[2])
 
         size[1] += 1
         _bytes += cmdBytes
 
         with open(
-            os.path.abspath(os.path.join(self.outputPath, f"{self.midFileName}.bdx")),
+            os.path.abspath(
+                os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
+            ),
             "ab+",
         ) as f:
             f.write(brotli.compress(_bytes + b"XE"))
 
         return True, len(cmdlist), max_delay, size, finalPos
 
     def toDICT(
@@ -1677,62 +2023,85 @@
     ) -> dict:
         """
         使用金羿的转换思路，将midi转换为字典
         :return: dict()
         """
 
         # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
-        channels = {0: {}, 1: {}, 2: {}, 3: {}, 4: {}, 5: {}, 6: {}, 7: {}, 8: {}, 9: {}, 10: {}, 11: {}, 12: {}, 13: {}, 14: {}, 15: {}, 16: {}}
+        channels = {
+            0: {},
+            1: {},
+            2: {},
+            3: {},
+            4: {},
+            5: {},
+            6: {},
+            7: {},
+            8: {},
+            9: {},
+            10: {},
+            11: {},
+            12: {},
+            13: {},
+            14: {},
+            15: {},
+            16: {},
+        }
 
         # 我们来用通道统计音乐信息
         # 但是是用分轨的思路的
         for track_no, track in enumerate(self.midi.tracks):
-            
             microseconds = 0
 
             for msg in track:
-
                 if msg.time != 0:
                     try:
                         microseconds += msg.time * tempo / self.midi.ticks_per_beat
                         # print(microseconds)
                     except NameError:
-                        if self.debugMode:
+                        if self.debug_mode:
                             raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
                         else:
-                            microseconds += (msg.time * mido.midifiles.midifiles.DEFAULT_TEMPO / self.midi.ticks_per_beat)
+                            microseconds += (
+                                msg.time
+                                * mido.midifiles.midifiles.DEFAULT_TEMPO
+                                / self.midi.ticks_per_beat
+                            )
 
                 if msg.is_meta:
                     if msg.type == "set_tempo":
                         tempo = msg.tempo
-                        if self.debugMode:
+                        if self.debug_mode:
                             self.prt(f"TEMPO更改：{tempo}（毫秒每拍）")
                 else:
-
-                    if self.debugMode:
+                    if self.debug_mode:
                         try:
                             if msg.channel > 15:
                                 raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
                         except AttributeError:
                             pass
-                    
+
                     if not track_no in channels[msg.channel].keys():
                         channels[msg.channel][track_no] = []
                     if msg.type == "program_change":
-                        channels[msg.channel][track_no].append(("PgmC", msg.program, microseconds))
+                        channels[msg.channel][track_no].append(
+                            ("PgmC", msg.program, microseconds)
+                        )
 
                     elif msg.type == "note_on" and msg.velocity != 0:
                         channels[msg.channel][track_no].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
                         msg.type == "note_off"
                     ):
-                        channels[msg.channel][track_no].append(("NoteE", msg.note, microseconds))
+                        channels[msg.channel][track_no].append(
+                            ("NoteE", msg.note, microseconds)
+                        )
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
 
         1 切换乐器消息
         ("PgmC", 切换后的乐器ID: int, 距离演奏开始的毫秒)
```

### Comparing `Musicreater-0.4.0/Musicreater.egg-info/PKG-INFO` & `Musicreater-0.5.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,396 +1,410 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 204d 7573  : 2.1..Name: Mus
-00000020: 6963 7265 6174 6572 0d0a 5665 7273 696f  icreater..Versio
-00000030: 6e3a 2030 2e34 2e30 0d0a 5375 6d6d 6172  n: 0.4.0..Summar
-00000040: 793a 20e4 b880 e6ac bee5 858d e8b4 b9e5  y: .............
-00000050: bc80 e6ba 90e7 9a84 20e3 808a e688 91e7  ........ .......
-00000060: 9a84 e4b8 96e7 958c e380 8b20 6d69 64e9  ........... mid.
-00000070: 9fb3 e4b9 90e8 bdac e68d a2e5 ba93 e380  ................
-00000080: 820d 0a48 6f6d 652d 7061 6765 3a20 6874  ...Home-page: ht
-00000090: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000000a0: 2f54 7269 4d2d 4f72 6761 6e69 7a61 7469  /TriM-Organizati
-000000b0: 6f6e 2f4d 7573 6963 7265 6174 6572 0d0a  on/Musicreater..
-000000c0: 4175 7468 6f72 3a20 4569 6c6c 6573 2057  Author: Eilles W
-000000d0: 616e 2c20 6267 4172 7261 790d 0a41 7574  an, bgArray..Aut
-000000e0: 686f 722d 656d 6169 6c3a 2054 7269 4d2d  hor-email: TriM-
-000000f0: 4f72 6761 6e69 7a61 7469 6f6e 4068 6f74  Organization@hot
-00000100: 6d61 696c 2e63 6f6d 0d0a 436c 6173 7369  mail.com..Classi
-00000110: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-00000120: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
-00000130: 6f70 6572 730d 0a43 6c61 7373 6966 6965  opers..Classifie
-00000140: 723a 204e 6174 7572 616c 204c 616e 6775  r: Natural Langu
-00000150: 6167 6520 3a3a 2043 6869 6e65 7365 2028  age :: Chinese (
-00000160: 5369 6d70 6c69 6669 6564 290d 0a43 6c61  Simplified)..Cla
-00000170: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
-00000180: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000190: 203a 3a20 4170 6163 6865 2053 6f66 7477   :: Apache Softw
-000001a0: 6172 6520 4c69 6365 6e73 650d 0a43 6c61  are License..Cla
-000001b0: 7373 6966 6965 723a 204f 7065 7261 7469  ssifier: Operati
-000001c0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-000001d0: 496e 6465 7065 6e64 656e 740d 0a43 6c61  Independent..Cla
-000001e0: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
-000001f0: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000200: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
-00000210: 6965 730d 0a43 6c61 7373 6966 6965 723a  ies..Classifier:
-00000220: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000230: 6775 6167 6520 3a3a 2050 7974 686f 6e0d  guage :: Python.
-00000240: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000250: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000260: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000270: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-00000280: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000290: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000002a0: 332e 360d 0a43 6c61 7373 6966 6965 723a  3.6..Classifier:
-000002b0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000002c0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002d0: 3a3a 2033 2e37 0d0a 436c 6173 7369 6669  :: 3.7..Classifi
-000002e0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-000002f0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000300: 6f6e 203a 3a20 332e 380d 0a43 6c61 7373  on :: 3.8..Class
-00000310: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000320: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000330: 7974 686f 6e20 3a3a 2033 2e39 0d0a 436c  ython :: 3.9..Cl
-00000340: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000350: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000360: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000370: 0d0a 4465 7363 7269 7074 696f 6e2d 436f  ..Description-Co
-00000380: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-00000390: 2f6d 6172 6b64 6f77 6e0d 0a4c 6963 656e  /markdown..Licen
-000003a0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-000003b0: 2e6d 640d 0a0d 0a3c 6831 2061 6c69 676e  .md....<h1 align
-000003c0: 3d22 6365 6e74 6572 223e e99f b3c2 b7e5  ="center">......
-000003d0: 889b 204d 7573 6963 7265 6174 6572 3c2f  .. Musicreater</
-000003e0: 6831 3e0d 0a0d 0a3c 7020 616c 6967 6e3d  h1>....<p align=
-000003f0: 2263 656e 7465 7222 3e0d 0a3c 696d 6720  "center">..<img 
-00000400: 7769 6474 683d 2231 3238 2220 6865 6967  width="128" heig
-00000410: 6874 3d22 3132 3822 2073 7263 3d22 6874  ht="128" src="ht
-00000420: 7470 733a 2f2f 7331 2e61 7831 782e 636f  tps://s1.ax1x.co
-00000430: 6d2f 3230 3232 2f30 352f 3036 2f4f 7568  m/2022/05/06/Ouh
-00000440: 6768 6a2e 6d64 2e70 6e67 2220 3e0d 0a3c  ghj.md.png" >..<
-00000450: 2f70 3e0d 0a0d 0a3c 6833 2061 6c69 676e  /p>....<h3 align
-00000460: 3d22 6365 6e74 6572 223e e4b8 80e6 acbe  ="center">......
-00000470: e585 8de8 b4b9 e5bc 80e6 ba90 e79a 8420  ............... 
-00000480: e380 8ae6 8891 e79a 84e4 b896 e795 8ce3  ................
-00000490: 808b 204d 4944 49e9 9fb3 e4b9 90e8 bdac  .. MIDI.........
-000004a0: e68d a2e5 ba93 e380 823c 2f68 333e 0d0a  .........</h3>..
-000004b0: 0d0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
-000004c0: 6572 223e 0d0a 3c69 6d67 2073 7263 3d22  er">..<img src="
-000004d0: 6874 7470 733a 2f2f 666f 7274 6865 6261  https://fortheba
-000004e0: 6467 652e 636f 6d2f 696d 6167 6573 2f62  dge.com/images/b
-000004f0: 6164 6765 732f 6275 696c 742d 7769 7468  adges/built-with
-00000500: 2d6c 6f76 652e 7376 6722 3e0d 0a3c 703e  -love.svg">..<p>
-00000510: 0d0a 0d0a 0d0a 5b21 5b5d 5b42 696c 6962  ......[![][Bilib
-00000520: 696c 693a 20e5 878c e4ba 91e9 8791 e7be  ili: ...........
-00000530: bf5d 5d28 6874 7470 733a 2f2f 7370 6163  .]](https://spac
-00000540: 652e 6269 6c69 6269 6c69 2e63 6f6d 2f33  e.bilibili.com/3
-00000550: 3937 3336 3930 3032 2f29 0d0a 5b21 5b5d  97369002/)..[![]
-00000560: 5b42 696c 6962 696c 693a 20e8 afb8 e891  [Bilibili: .....
-00000570: 9be4 baae e4b8 8ee5 85ab e58d a6e9 98b5  ................
-00000580: 5d5d 2868 7474 7073 3a2f 2f73 7061 6365  ]](https://space
-00000590: 2e62 696c 6962 696c 692e 636f 6d2f 3630  .bilibili.com/60
-000005a0: 3430 3732 3437 3429 200d 0a5b 215b 436f  4072474) ..[![Co
-000005b0: 6465 5374 796c 653a 2062 6c61 636b 5d5d  deStyle: black]]
-000005c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000005d0: 636f 6d2f 7073 662f 626c 6163 6b29 0d0a  com/psf/black)..
-000005e0: 5b21 5b5d 5b70 7974 686f 6e5d 5d28 6874  [![][python]](ht
-000005f0: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
-00000600: 2e6f 7267 2f29 0d0a 5b21 5b5d 5b6c 6963  .org/)..[![][lic
-00000610: 656e 7365 5d5d 284c 4943 454e 5345 290d  ense]](LICENSE).
-00000620: 0a5b 215b 5d5b 7265 6c65 6173 655d 5d28  .[![][release]](
-00000630: 2e2e 2f2e 2e2f 7265 6c65 6173 6573 290d  ../../releases).
-00000640: 0a0d 0a0d 0ae7 ae80 e4bd 93e4 b8ad e696  ................
-00000650: 87f0 9f87 a8f0 9f87 b320 7c20 5b45 6e67  ......... | [Eng
-00000660: 6c69 7368 f09f 87ac f09f 87a7 5d28 5245  lish........](RE
-00000670: 4144 4d45 5f45 4e2e 6d64 290d 0a0d 0a0d  ADME_EN.md).....
-00000680: 0a23 2320 e4bb 8be7 bb8d f09f 9a80 0d0a  .## ............
-00000690: 0d0a e99f b3c2 b7e5 889b 20e6 98af e4b8  .......... .....
-000006a0: 80e4 b8aa e585 8de8 b4b9 e5bc 80e6 ba90  ................
-000006b0: e79a 84e9 9288 e5af b920 2a2a e380 8ae6  ......... **....
-000006c0: 8891 e79a 84e4 b896 e795 8ce3 808b 2a2a  ..............**
-000006d0: 20e7 9a84 4d49 4449 e99f b3e4 b990 e8bd   ...MIDI........
-000006e0: ace6 8da2 e5ba 930d 0a0d 0ae6 aca2 e8bf  ................
-000006f0: 8ee5 8aa0 e7be a4ef bc9a 5b38 3631 3638  ..........[86168
-00000700: 3438 3539 5d28 6874 7470 733a 2f2f 6a71  4859](https://jq
-00000710: 2e71 712e 636f 6d2f 3f5f 7776 3d31 3032  .qq.com/?_wv=102
-00000720: 3726 6b3d 6870 6552 7872 5972 290d 0a0d  7&k=hpeRxrYr)...
-00000730: 0a23 2320 e4b8 8be8 bdbd e5ae 89e8 a385  .## ............
-00000740: 0d0a 0d0a 2d20 e4bd bfe7 94a8 7079 7069  ....- ......pypi
-00000750: 0d0a 2020 2020 6060 6062 6173 680d 0a20  ..    ```bash.. 
-00000760: 2020 2070 6970 2069 6e73 7461 6c6c 204d     pip install M
-00000770: 7573 6963 7265 6174 6572 0d0a 2020 2020  usicreater..    
-00000780: 6060 600d 0a0d 0a2d 20e5 a682 e69e 9ce5  ```....- .......
-00000790: 87ba e78e b0e9 9499 e8af afef bc8c e58f  ................
-000007a0: afe4 bba5 e5b0 9de8 af95 efbc 9a0d 0a20  ............... 
-000007b0: 2020 2060 6060 6261 7368 0d0a 2020 2020     ```bash..    
-000007c0: 7069 7020 696e 7374 616c 6c20 2d69 2068  pip install -i h
-000007d0: 7474 7073 3a2f 2f70 7970 692e 7079 7468  ttps://pypi.pyth
-000007e0: 6f6e 2e6f 7267 2f73 696d 706c 6520 4d75  on.org/simple Mu
-000007f0: 7369 6372 6561 7465 720d 0a20 2020 2060  sicreater..    `
-00000800: 6060 0d0a 2d20 efbc 88e5 afb9 e4ba 8ee5  ``..- ..........
-00000810: bc80 e58f 91e8 8085 e69d a5e8 afb4 efbc  ................
-00000820: 89e5 8d87 e7ba a7ef bc9a 0d0a 2020 2020  ............    
-00000830: 6060 6062 6173 680d 0a20 2020 2070 6970  ```bash..    pip
-00000840: 2069 6e73 7461 6c6c 202d 6920 6874 7470   install -i http
-00000850: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
-00000860: 6f72 672f 7369 6d70 6c65 204d 7573 6963  org/simple Music
-00000870: 7265 6174 6572 202d 2d75 7067 7261 6465  reater --upgrade
-00000880: 0d0a 2020 2020 6060 600d 0a0d 0a2d 20e5  ..    ```....- .
-00000890: 858b e99a 86e4 bb93 e5ba 93e5 b9b6 e5ae  ................
-000008a0: 89e8 a385 0d0a 2020 2020 6060 6062 6173  ......    ```bas
-000008b0: 680d 0a20 2020 2067 6974 2063 6c6f 6e65  h..    git clone
-000008c0: 2068 7474 7073 3a2f 2f67 6974 6565 2e63   https://gitee.c
-000008d0: 6f6d 2f54 7269 4d2d 4f72 6761 6e69 7a61  om/TriM-Organiza
-000008e0: 7469 6f6e 2f4d 7573 6963 7265 6174 6572  tion/Musicreater
-000008f0: 2e67 6974 0d0a 2020 2020 6364 204d 7573  .git..    cd Mus
-00000900: 6963 7265 6174 6572 0d0a 2020 2020 7079  icreater..    py
-00000910: 7468 6f6e 2073 6574 7570 2e70 7920 696e  thon setup.py in
-00000920: 7374 616c 6c0d 0a20 2020 2060 6060 0d0a  stall..    ```..
-00000930: 0d0a e4bb a5e4 b88a e591 bde4 bba4 e7a7  ................
-00000940: 8d20 6070 7974 686f 6e60 e380 8160 7069  . `python`...`pi
-00000950: 7060 20e8 afb7 e4be 9de7 85a7 e590 84e4  p` .............
-00000960: b8aa e78e afe5 a283 e4b8 8de5 908c e781  ................
-00000970: b5e6 b4bb e69b b4e6 8da2 efbc 8ce5 8faf  ................
-00000980: e883 bde4 b8ba 6070 7974 686f 6e33 60e6  ......`python3`.
-00000990: 8896 6070 6970 3360 e4b9 8be7 b1bb e380  ..`pip3`........
-000009a0: 820d 0a0d 0a23 2320 e696 87e6 a1a3 f09f  .....## ........
-000009b0: 9384 0d0a 0d0a 5be7 949f e688 90e6 9687  ......[.........
-000009c0: e4bb b6e7 9a84 e4bd bfe7 94a8 5d28 6874  ............](ht
-000009d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000009e0: 2f54 7269 4d2d 4f72 6761 6e69 7a61 7469  /TriM-Organizati
-000009f0: 6f6e 2f4d 7573 6963 7265 6174 6572 2f62  on/Musicreater/b
-00000a00: 6c6f 622f 6d61 7374 6572 2f64 6f63 732f  lob/master/docs/
-00000a10: 2545 3725 3934 2539 4625 4536 2538 3825  %E7%94%9F%E6%88%
-00000a20: 3930 2545 3625 3936 2538 3725 4534 2542  90%E6%96%87%E4%B
-00000a30: 4225 4236 2545 3725 3941 2538 3425 4534  B%B6%E7%9A%84%E4
-00000a40: 2542 4425 4246 2545 3725 3934 2541 3825  %BD%BF%E7%94%A8%
-00000a50: 4538 2541 4625 4234 2545 3625 3938 2538  E8%AF%B4%E6%98%8
-00000a60: 452e 6d64 290d 0a0d 0a5b e4bb 93e5 ba93  E.md)....[......
-00000a70: 4150 49e6 9687 e6a1 a35d 2868 7474 7073  API......](https
-00000a80: 3a2f 2f67 6974 6875 622e 636f 6d2f 5472  ://github.com/Tr
-00000a90: 694d 2d4f 7267 616e 697a 6174 696f 6e2f  iM-Organization/
-00000aa0: 4d75 7369 6372 6561 7465 722f 626c 6f62  Musicreater/blob
-00000ab0: 2f6d 6173 7465 722f 646f 6373 2f25 4535  /master/docs/%E5
-00000ac0: 2542 4125 3933 2545 3725 3941 2538 3425  %BA%93%E7%9A%84%
-00000ad0: 4537 2539 3425 3946 2545 3625 3838 2539  E7%94%9F%E6%88%9
-00000ae0: 3025 4534 2542 3825 3845 2545 3525 3841  0%E4%B8%8E%E5%8A
-00000af0: 2539 4625 4538 2538 3325 4244 2545 3625  %9F%E8%83%BD%E6%
-00000b00: 3936 2538 3725 4536 2541 3125 4133 2e6d  96%87%E6%A1%A3.m
-00000b10: 6429 0d0a 0d0a 2323 20e4 bd9c e880 85e2  d)....## .......
-00000b20: 9c92 0d0a 0d0a e987 91e7 bebf 2045 696c  ............ Eil
-00000b30: 6c65 73ef bc9a e688 91e7 9a84 e4b8 96e7  les.............
-00000b40: 958c e59f bae5 b2a9 e789 88e6 8c87 e4bb  ................
-00000b50: a4e5 b888 efbc 8ce4 b8aa e4ba bae5 bc80  ................
-00000b60: e58f 91e8 8085 efbc 8c42 e7ab 99e4 b88d  .........B......
-00000b70: e79f a5e5 908d 5550 e4b8 bbef bc8c e6b1  ......UP........
-00000b80: 9fe8 a5bf e59c a8e6 a0a1 e9ab 98e4 b8ad  ................
-00000b90: e794 9fe3 8082 0d0a 0d0a e8af b8e8 919b  ................
-00000ba0: e4ba aee4 b88e e585 abe5 8da6 e998 b520  ............... 
-00000bb0: 6267 4172 7261 79ef bc9a e688 91e7 9a84  bgArray.........
-00000bc0: e4b8 96e7 958c e59f bae5 b2a9 e789 88e7  ................
-00000bd0: 8ea9 e5ae b6ef bc8c e596 9ce6 aca2 e7bc  ................
-00000be0: 96e7 a88b e592 8ce9 9fb3 e4b9 90ef bc8c  ................
-00000bf0: e6b7 b1e5 9cb3 e588 9de4 ba8c e5ad a6e7  ................
-00000c00: 949f e380 820d 0a0d 0a23 2320 e887 b4e8  .........## ....
-00000c10: b0a2 f09f 998f 0d0a e69c ace8 87b4 e8b0  ................
-00000c20: a2e5 8897 e8a1 a8e6 8e92 e590 8de6 97a0  ................
-00000c30: e9a1 bae5 ba8f e380 820d 0a0d 0a2d 20e6  .............- .
-00000c40: 849f e8b0 a220 2a2a e698 80e6 a2a6 2a2a  ..... **......**
-00000c50: 5c3c 5151 3135 3135 3339 3938 3835 5c3e  \<QQ1515399885\>
-00000c60: 20e6 89be e587 bae6 8c87 e4bb a4e7 949f   ...............
-00000c70: e688 90e9 9499 e8af af62 7567 e5b9 b6e6  .........bug....
-00000c80: 8c87 e6ad a30d 0a2d 20e6 849f e8b0 a2e7  .......- .......
-00000c90: 94b1 202a 2a43 6861 726c 6965 5f50 696e  .. **Charlie_Pin
-00000ca0: 6720 e280 9ce6 9fa5 e790 86e5 b9b3 e280  g ..............
-00000cb0: 9d2a 2a20 e5b8 a6e6 9da5 e79a 8442 4458  .** .........BDX
-00000cc0: e696 87e4 bbb6 e8bd ace6 8da2 e58f 82e8  ................
-00000cd0: 8083 efbc 8ce4 bba5 e58f 8a4d 4944 492d  ...........MIDI-
-00000ce0: e688 91e7 9a84 e4b8 96e7 958c e5af b9e5  ................
-00000cf0: ba94 e4b9 90e5 99a8 e58f 82e8 8083 e8a1  ................
-00000d00: a8e6 a0bc 0d0a 2d20 e684 9fe8 b0a2 e794  ......- ........
-00000d10: b120 2a2a 5b43 4d41 5f32 3430 3150 545d  . **[CMA_2401PT]
-00000d20: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000d30: 636f 6d2f 434d 4132 3430 3150 5429 2a2a  com/CMA2401PT)**
-00000d40: 20e4 b8ba e688 91e4 bbac e79a 84e8 bdaf   ...............
-00000d50: e4bb b6e5 bc80 e58f 91e7 9a84 e4b8 80e4  ................
-00000d60: ba9b e696 b9e9 9da2 e8bf 9be8 a18c e68c  ................
-00000d70: 87e5 afbc efbc 8ce5 908c e697 b6e6 8891  ................
-00000d80: e4bb ace5 8f82 e880 83e4 ba86 e4bb 96e7  ................
-00000d90: 9a84 4244 5877 6f72 6b73 686f 70e4 bd9c  ..BDXworkshop...
-00000da0: e4b8 ba42 4458 e7bb 93e6 9e84 e7bc 96e8  ...BDX..........
-00000db0: be91 e79a 84e5 8f82 e880 830d 0a2d 20e6  .............- .
-00000dc0: 849f e8b0 a2e7 94b1 202a 2a5b 4469 736c  ........ **[Disl
-00000dd0: 696e 6b20 5366 6f72 7a61 5d28 6874 7470  ink Sforza](http
-00000de0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f44  s://github.com/D
-00000df0: 6973 6c69 6e6b 2920 e280 9ce6 96ad e881  islink) ........
-00000e00: 94c2 b7e6 96af e7a6 8fe5 b094 e689 8ee2  ................
-00000e10: 809d 2a2a 5c3c 5151 3136 3030 3531 3533  ..**\<QQ16005153
-00000e20: 3134 5c3e 20e5 b8a6 e69d a5e7 9a84 6d69  14\> .........mi
-00000e30: 6469 e99f b3e8 89b2 e8a7 a3e6 9e90 e4bb  di..............
-00000e40: a5e5 8f8a e8bd ace6 8da2 e68c 87e4 bba4  ................
-00000e50: e79a 84e7 ae97 e6b3 95ef bc8c e688 91e4  ................
-00000e60: bbac e5b0 86e5 85b6 e694 b9e7 bc96 e5b9  ................
-00000e70: b6e5 ba94 e794 a8ef bc9b e590 8ce6 97b6  ................
-00000e80: efbc 8ce6 849f e8b0 a2e4 bb96 e79a 845b  ...............[
-00000e90: e7bd 91e9 a1b5 e789 88e8 bdac e68d a2e5  ................
-00000ea0: 99a8 5d28 6874 7470 733a 2f2f 6469 736c  ..](https://disl
-00000eb0: 696e 6b2e 6769 7468 7562 2e69 6f2f 6d69  ink.github.io/mi
-00000ec0: 6469 3262 6478 2f29 e7bb 99e6 8891 e4bb  di2bdx/)........
-00000ed0: ace7 9a84 e5bc 80e5 8f91 e4b8 8ee6 9bb4  ................
-00000ee0: e696 b0e5 b8a6 e69d a5e5 b7a8 e5a4 a7e7  ................
-00000ef0: 9a84 e58e 8be5 8a9b e592 8ce5 8aa8 e58a  ................
-00000f00: 9bef bc8c e8ae a9e6 8891 e4bb ace5 9ca8  ................
-00000f10: e58e 9fe6 9cac e4b8 80e9 aa91 e7bb 9de5  ................
-00000f20: b098 e79a 84e6 91b8 e9b1 bce9 8193 e8b7  ................
-00000f30: afe4 b88a e8bd ace5 9091 e5bc 80e5 8f91  ................
-00000f40: efbc 8ce5 b88c e69c 9be4 bb96 e883 bde8  ................
-00000f50: 8083 e4b8 8ae4 b880 e4b8 aae7 9086 e683  ................
-00000f60: b3e7 9a84 e5a4 a7e5 ada6 efbc 810d 0a2d  ...............-
-00000f70: 20e6 849f e8b0 a220 2a2a 546f 7563 6820   ...... **Touch 
-00000f80: e280 9ce5 81b7 e590 83e2 809d 2a2a 5c3c  ............**\<
-00000f90: 5151 3137 3933 3533 3731 3634 5c3e 20e6  QQ1793537164\> .
-00000fa0: 8f90 e4be 9be7 9a84 4244 58e5 afbc e585  ........BDX.....
-00000fb0: a5e6 b58b e8af 95e6 94af e68c 81ef bc8c  ................
-00000fc0: e5b9 b6e5 afb9 e7a8 8be5 ba8f e79a 84e6  ................
-00000fd0: 94b9 e8bf 9be6 8f90 e4be 9be4 ba86 e4b8  ................
-00000fe0: b0e5 af8c e79a 84e6 848f e8a7 81ef bc9b  ................
-00000ff0: e590 8ce6 97b6 e4b9 9fe6 849f e8b0 a2e4  ................
-00001000: bb96 e79a 84e4 b88d e696 ade5 b09d e8af  ................
-00001010: 95e6 96b0 e79a 84e5 8685 e5ae b9ef bc8c  ................
-00001020: e4bd bfe6 8891 e4bb ace7 9a84 e68e 92e9  ................
-00001030: 9499 e69b b4e8 bf9b e4b8 80e6 ada5 0d0a  ................
-00001040: 2d20 e684 9fe8 b0a2 202a 2a4d 6f6e 6f2a  - ...... **Mono*
-00001050: 2a5c 3c51 5137 3338 3839 3330 3837 5c3e  *\<QQ738893087\>
-00001060: 20e5 8f8d e9a6 88e5 ae89 e8a3 85e6 97b6   ...............
-00001070: e79a 84e9 97ae e9a2 98ef bc8c e8be 85e5  ................
-00001080: 8aa9 e688 91e4 bbac e689 bee5 88b0 e4ba  ................
-00001090: 86e8 a786 e7aa 97e6 938d e4bd 9ce7 b3bb  ................
-000010a0: e7bb 9fe4 b88b e79a 84e5 85bc e5ae b9e6  ................
-000010b0: 80a7 e997 aee9 a298 0d0a 2d20 e684 9fe8  ..........- ....
-000010c0: b0a2 202a 2a41 6d6d 656c 6961 20e2 809c  .. **Ammelia ...
-000010d0: e889 bee7 b1b3 e588 a9e4 ba9a e280 9d2a  ...............*
-000010e0: 2a5c 3c51 5132 3833 3833 3334 3633 375c  *\<QQ2838334637\
-000010f0: 3e20 e695 a6e4 bf83 e688 91e4 bbac e8bf  > ..............
-00001100: 9be8 a18c e696 b0e7 9a84 e58a 9fe8 83bd  ................
-00001110: e5bc 80e5 8f91 efbc 8ce5 b9b6 e4b8 bae6  ................
-00001120: 96b0 e58a 9fe8 83bd e68f 90e5 87ba e4ba  ................
-00001130: 86e9 9d9e e5b8 b8e4 bc98 e7a7 80e7 9a84  ................
-00001140: e5a4 a7e9 878f e5bb bae8 aeae efbc 8ce4  ................
-00001150: bba5 e58f 8ae6 8f90 e4be 9be7 9a84 4244  ..............BD
-00001160: 58e5 afbc e585 a5e6 b58b e8af 95e6 94af  X...............
-00001170: e68c 81ef bc8c e4b8 bae6 8891 e4bb ace7  ................
-00001180: 9a84 e696 b0e7 bb93 e69e 84e7 949f e688  ................
-00001190: 90e7 ae97 e6b3 95e6 8f90 e4be 9be4 ba86  ................
-000011a0: e5a4 a7e9 878f e79a 84e5 ae9e e999 85e7  ................
-000011b0: 9086 e8ae bae6 94af e68c 810d 0a2d 20e6  .............- .
-000011c0: 849f e8b0 a220 2a2a 5be7 a59e e7be bd5d  ..... **[......]
-000011d0: 2868 7474 7073 3a2f 2f67 6974 6565 2e63  (https://gitee.c
-000011e0: 6f6d 2f73 6e6f 7779 6b61 6d69 2920 e280  om/snowykami) ..
-000011f0: 9c5b 536e 6f77 794b 616d 695d 2868 7474  .[SnowyKami](htt
-00001200: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001210: 736e 6f77 7966 6972 6566 6c79 29e2 809d  snowyfirefly)...
-00001220: 2a2a 20e5 afb9 e688 91e4 bbac e9a1 b9e7  ** .............
-00001230: 9bae e79a 84e6 94af e68c 81e4 b88e e5ae  ................
-00001240: a3e4 bca0 efbc 8ce5 b88c e69c 9be4 bb96  ................
-00001250: e883 bde8 8083 e79a 84e4 b880 e689 80e4  ................
-00001260: bc98 e7a7 80e7 9a84 e5a4 a7e5 ada6 efbc  ................
-00001270: 810d 0a2d 20e6 849f e8b0 a220 2a2a e68c  ...- ...... **..
-00001280: 87e4 bba4 e5b8 885f e88b a6e5 8a9b e680  ......._........
-00001290: 9520 706c 6179 6a75 6963 6531 3233 2a2a  . playjuice123**
-000012a0: 5c3c 5151 3234 3036 3637 3139 375c 3ee4  \<QQ240667197\>.
-000012b0: b8ba e688 91e4 bbac e79a 84e7 a88b e5ba  ................
-000012c0: 8fe6 89be e587 bae9 9499 e8af afef bc8c  ................
-000012d0: e5b9 b6e6 8f90 e986 92e6 8891 e4bb ace4  ................
-000012e0: bfae e5a4 8de4 b880 e4b8 aae4 b880 e79b  ................
-000012f0: b4e5 ad98 e59c a8e7 9a84 e5a4 a762 7567  .............bug
-00001300: e380 820d 0a2d 20e6 849f e8b0 a220 2a2a  .....- ...... **
-00001310: e99b b7e9 9c86 2a2a 5c3c 5151 3335 3535  ......**\<QQ3555
-00001320: 3236 3835 3139 5c3e e4b8 bae6 8891 e4bb  268519\>........
-00001330: ace7 9a84 e7a8 8be5 ba8f e689 bee5 87ba  ................
-00001340: e994 99e8 afaf efbc 8ce5 b9b6 e68f 90e9  ................
-00001350: 8692 e4bf aee5 a48d 6275 67e3 8082 0d0a  ........bug.....
-00001360: 0d0a 3e09 e684 9fe8 b0a2 e5b9 bfe5 a4a7  ..>.............
-00001370: e7be a4e5 8f8b e4b8 bae6 ada4 e7a8 8be5  ................
-00001380: ba8f e68f 90e4 be9b e79a 84e6 b58b e8af  ................
-00001390: 95e7 ad89 e694 afe6 8c81 0d0a 3e0d 0a3e  ............>..>
-000013a0: 09e8 8ba5 e682 a8e5 afb9 e688 91e4 bbac  ................
-000013b0: e69c 89e6 8980 e8b4 a1e7 8cae e4bd 86e6  ................
-000013c0: 82a8 e79a 84e5 908d e5ad 97e6 b2a1 e69c  ................
-000013d0: 89e6 98be e7a4 bae5 9ca8 e6ad a4e5 8897  ................
-000013e0: e8a1 a8e4 b8ad efbc 8ce8 afb7 e881 94e7  ................
-000013f0: b3bb e688 91e4 bbac efbc 810d 0a0d 0a23  ...............#
-00001400: 2320 e881 94e7 b3bb f09f 939e 0d0a 0d0a  # ..............
-00001410: e88b a5e9 8187 e588 b0e5 ba93 e4b8 ade7  ................
-00001420: 9a84 e997 aee9 a298 efbc 8ce6 aca2 e8bf  ................
-00001430: 8ee5 9ca8 5be6 ada4 5d28 6874 7470 733a  ....[...](https:
-00001440: 2f2f 6769 7465 652e 636f 6d2f 5472 694d  //gitee.com/TriM
-00001450: 2d4f 7267 616e 697a 6174 696f 6e2f 4d75  -Organization/Mu
-00001460: 7369 6372 6561 7465 722f 6973 7375 6573  sicreater/issues
-00001470: 2f6e 6577 29e6 8f90 e587 bae4 bda0 e79a  /new)...........
-00001480: 8469 7373 7565 e380 820d 0a0d 0ae5 a682  .issue..........
-00001490: e69e 9ce9 9c80 e8a6 81e4 b88e e5bc 80e5  ................
-000014a0: 8f91 e7bb 84e8 bf9b e8a1 8ce4 baa4 e6b5  ................
-000014b0: 81ef bc8c e6ac a2e8 bf8e e58a a0e5 85a5  ................
-000014c0: e688 91e4 bbac e79a 845b e5bc 80e5 8f91  .........[......
-000014d0: e997 b2e8 818a 51e7 bea4 5d28 6874 7470  ......Q...](http
-000014e0: 733a 2f2f 6a71 2e71 712e 636f 6d2f 3f5f  s://jq.qq.com/?_
-000014f0: 7776 3d31 3032 3726 6b3d 6870 6552 7872  wv=1027&k=hpeRxr
-00001500: 5972 29e3 8082 0d0a 0d0a 2d2d 2d2d 2d2d  Yr).......------
-00001510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001530: 2d2d 2d2d 2d2d 0d0a 0d0a 4e4f 5420 414e  ------....NOT AN
-00001540: 204f 4646 4943 4941 4c20 4d49 4e45 4352   OFFICIAL MINECR
-00001550: 4146 5420 5052 4f44 5543 542e 0d0a 0d0a  AFT PRODUCT.....
-00001560: 4e4f 5420 4150 5052 4f56 4544 2042 5920  NOT APPROVED BY 
-00001570: 4f52 2041 5353 4f43 4941 5445 4420 5749  OR ASSOCIATED WI
-00001580: 5448 204d 4f4a 414e 4720 4f52 204d 4943  TH MOJANG OR MIC
-00001590: 524f 534f 4654 2e0d 0a0d 0ae6 ada4 e9a1  ROSOFT..........
-000015a0: b9e7 9bae e5b9 b6e9 9d9e e4b8 80e4 b8aa  ................
-000015b0: e5ae 98e6 96b9 20e3 808a e688 91e7 9a84  ...... .........
-000015c0: e4b8 96e7 958c e380 8bef bc88 2a4d 696e  ............*Min
-000015d0: 6563 7261 6674 2aef bc89 e9a1 b9e7 9bae  ecraft*.........
-000015e0: 0d0a 0d0a e6ad a4e9 a1b9 e79b aee4 b88d  ................
-000015f0: e99a b6e5 b19e e688 96e5 85b3 e881 94e4  ................
-00001600: ba8e 204d 6f6a 616e 6720 5374 7564 696f  .. Mojang Studio
-00001610: 7320 e688 9620 e5be aee8 bdaf 0d0a 0d0a  s ... ..........
-00001620: 0d0a 0d0a 0d0a 0d0a 5b42 696c 6962 696c  ........[Bilibil
-00001630: 693a 20e5 878c e4ba 91e9 8791 e7be bf5d  i: ............]
-00001640: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00001650: 6965 6c64 732e 696f 2f62 6164 6765 2f42  ields.io/badge/B
-00001660: 696c 6962 696c 692d 2545 3525 3837 2538  ilibili-%E5%87%8
-00001670: 4325 4534 2542 4125 3931 2545 3925 3837  C%E4%BA%91%E9%87
-00001680: 2539 3125 4537 2542 4525 4246 2d30 3041  %91%E7%BE%BF-00A
-00001690: 3145 373f 7374 796c 653d 666f 722d 7468  1E7?style=for-th
-000016a0: 652d 6261 6467 650d 0a5b 4269 6c69 6269  e-badge..[Bilibi
-000016b0: 6c69 3a20 e8af b8e8 919b e4ba aee4 b88e  li: ............
-000016c0: e585 abe5 8da6 e998 b55d 3a20 6874 7470  .........]: http
-000016d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000016e0: 696f 2f62 6164 6765 2f42 696c 6962 696c  io/badge/Bilibil
-000016f0: 692d 2545 3825 4146 2542 3825 4538 2539  i-%E8%AF%B8%E8%9
-00001700: 3125 3942 2545 3425 4241 2541 4525 4534  1%9B%E4%BA%AE%E4
-00001710: 2542 3825 3845 2545 3525 3835 2541 4225  %B8%8E%E5%85%AB%
-00001720: 4535 2538 4425 4136 2545 3925 3938 2542  E5%8D%A6%E9%98%B
-00001730: 352d 3030 4131 4537 3f73 7479 6c65 3d66  5-00A1E7?style=f
-00001740: 6f72 2d74 6865 2d62 6164 6765 0d0a 5b43  or-the-badge..[C
-00001750: 6f64 6553 7479 6c65 3a20 626c 6163 6b5d  odeStyle: black]
-00001760: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00001770: 6965 6c64 732e 696f 2f62 6164 6765 2f63  ields.io/badge/c
-00001780: 6f64 6525 3230 7374 796c 652d 626c 6163  ode%20style-blac
-00001790: 6b2d 3132 3131 3130 2e73 7667 3f73 7479  k-121110.svg?sty
-000017a0: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
-000017b0: 0d0a 5b70 7974 686f 6e5d 3a20 6874 7470  ..[python]: http
-000017c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000017d0: 696f 2f62 6164 6765 2f70 7974 686f 6e2d  io/badge/python-
-000017e0: 332e 362d 4142 3730 4646 3f73 7479 6c65  3.6-AB70FF?style
-000017f0: 3d66 6f72 2d74 6865 2d62 6164 6765 0d0a  =for-the-badge..
-00001800: 5b72 656c 6561 7365 5d3a 2068 7474 7073  [release]: https
-00001810: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00001820: 6f2f 6769 7468 7562 2f76 2f72 656c 6561  o/github/v/relea
-00001830: 7365 2f45 696c 6c65 7357 616e 2f4d 7573  se/EillesWan/Mus
-00001840: 6963 7265 6174 6572 3f73 7479 6c65 3d66  icreater?style=f
-00001850: 6f72 2d74 6865 2d62 6164 6765 0d0a 5b6c  or-the-badge..[l
-00001860: 6963 656e 7365 5d3a 2068 7474 7073 3a2f  icense]: https:/
-00001870: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00001880: 6261 6467 652f 4c69 6365 6e63 652d 4170  badge/Licence-Ap
-00001890: 6163 6865 2d32 3238 4232 323f 7374 796c  ache-228B22?styl
-000018a0: 653d 666f 722d 7468 652d 6261 6467 650d  e=for-the-badge.
-000018b0: 0a                                       .
+00000000: 0d0a 3c68 3120 616c 6967 6e3d 2263 656e  ..<h1 align="cen
+00000010: 7465 7222 3e0d 0a20 2020 20e9 9fb3 c2b7  ter">..    .....
+00000020: e588 9b20 4d75 7369 6372 6561 7465 720d  ... Musicreater.
+00000030: 0a3c 2f68 313e 0d0a 0d0a 3c70 2061 6c69  .</h1>....<p ali
+00000040: 676e 3d22 6365 6e74 6572 223e 0d0a 2020  gn="center">..  
+00000050: 2020 3c69 6d67 2077 6964 7468 3d22 3132    <img width="12
+00000060: 3822 2068 6569 6768 743d 2231 3238 2220  8" height="128" 
+00000070: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00000080: 6565 2e63 6f6d 2f54 7269 4d2d 4f72 6761  ee.com/TriM-Orga
+00000090: 6e69 7a61 7469 6f6e 2f4d 7573 6963 7265  nization/Musicre
+000000a0: 6174 6572 2f72 6177 2f6d 6173 7465 722f  ater/raw/master/
+000000b0: 7265 736f 7572 6365 732f 6d73 6374 4963  resources/msctIc
+000000c0: 6f6e 2e69 636f 223e 0d0a 2020 2020 3c2f  on.ico">..    </
+000000d0: 696d 673e 0d0a 3c2f 703e 0d0a 0d0a 3c68  img>..</p>....<h
+000000e0: 3320 616c 6967 6e3d 2263 656e 7465 7222  3 align="center"
+000000f0: 3ee4 b880 e6ac bee5 858d e8b4 b9e5 bc80  >...............
+00000100: e6ba 90e7 9a84 20e3 808a e688 91e7 9a84  ...... .........
+00000110: e4b8 96e7 958c e380 8b20 4d49 4449 e99f  ......... MIDI..
+00000120: b3e4 b990 e8bd ace6 8da2 e5ba 93e3 8082  ................
+00000130: 3c2f 6833 3e0d 0a0d 0a3c 7020 616c 6967  </h3>....<p alig
+00000140: 6e3d 2263 656e 7465 7222 3e0d 0a20 2020  n="center">..   
+00000150: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000160: 3a2f 2f66 6f72 7468 6562 6164 6765 2e63  ://forthebadge.c
+00000170: 6f6d 2f69 6d61 6765 732f 6261 6467 6573  om/images/badges
+00000180: 2f62 7569 6c74 2d77 6974 682d 6c6f 7665  /built-with-love
+00000190: 2e73 7667 223e 0d0a 2020 2020 3c61 2068  .svg">..    <a h
+000001a0: 7265 663d 2768 7474 7073 3a2f 2f67 6974  ref='https://git
+000001b0: 6565 2e63 6f6d 2f54 7269 4d2d 4f72 6761  ee.com/TriM-Orga
+000001c0: 6e69 7a61 7469 6f6e 2f4d 7573 6963 7265  nization/Musicre
+000001d0: 6174 6572 273e 0d0a 2020 2020 2020 2020  ater'>..        
+000001e0: 3c69 6d67 2061 6c69 676e 3d22 7269 6768  <img align="righ
+000001f0: 7422 2073 7263 3d27 6874 7470 733a 2f2f  t" src='https://
+00000200: 6769 7465 652e 636f 6d2f 5472 694d 2d4f  gitee.com/TriM-O
+00000210: 7267 616e 697a 6174 696f 6e2f 4d75 7369  rganization/Musi
+00000220: 6372 6561 7465 722f 7769 6467 6574 732f  creater/widgets/
+00000230: 7769 6467 6574 5f31 2e73 7667 2720 616c  widget_1.svg' al
+00000240: 743d 2746 6f72 6b20 6d65 206f 6e20 4769  t='Fork me on Gi
+00000250: 7465 6527 3e0d 0a20 2020 2020 2020 203c  tee'>..        <
+00000260: 2f69 6d67 3e0d 0a20 2020 203c 2f61 3e0d  /img>..    </a>.
+00000270: 0a3c 703e 0d0a 0d0a 0d0a 0d0a 0d0a 0d0a  .<p>............
+00000280: 5b21 5b5d 5b42 696c 6962 696c 693a 20e9  [![][Bilibili: .
+00000290: 8791 e7be bf45 4c53 5d5d 2868 7474 7073  .....ELS]](https
+000002a0: 3a2f 2f73 7061 6365 2e62 696c 6962 696c  ://space.bilibil
+000002b0: 692e 636f 6d2f 3339 3733 3639 3030 322f  i.com/397369002/
+000002c0: 290d 0a5b 215b 5d5b 4269 6c69 6269 6c69  )..[![][Bilibili
+000002d0: 3a20 e8af b8e8 919b e4ba aee4 b88e e585  : ..............
+000002e0: abe5 8da6 e998 b55d 5d28 6874 7470 733a  .......]](https:
+000002f0: 2f2f 7370 6163 652e 6269 6c69 6269 6c69  //space.bilibili
+00000300: 2e63 6f6d 2f36 3034 3037 3234 3734 2920  .com/604072474) 
+00000310: 0d0a 5b21 5b43 6f64 6553 7479 6c65 3a20  ..[![CodeStyle: 
+00000320: 626c 6163 6b5d 5d28 6874 7470 733a 2f2f  black]](https://
+00000330: 6769 7468 7562 2e63 6f6d 2f70 7366 2f62  github.com/psf/b
+00000340: 6c61 636b 290d 0a5b 215b 5d5b 7079 7468  lack)..[![][pyth
+00000350: 6f6e 5d5d 2868 7474 7073 3a2f 2f77 7777  on]](https://www
+00000360: 2e70 7974 686f 6e2e 6f72 672f 290d 0a5b  .python.org/)..[
+00000370: 215b 5d5b 6c69 6365 6e73 655d 5d28 4c49  ![][license]](LI
+00000380: 4345 4e53 4529 0d0a 5b21 5b5d 5b72 656c  CENSE)..[![][rel
+00000390: 6561 7365 5d5d 282e 2e2f 2e2e 2f72 656c  ease]](../../rel
+000003a0: 6561 7365 7329 0d0a 0d0a 5b21 5b47 6974  eases)....[![Git
+000003b0: 6565 5374 6172 5d28 6874 7470 733a 2f2f  eeStar](https://
+000003c0: 6769 7465 652e 636f 6d2f 5472 694d 2d4f  gitee.com/TriM-O
+000003d0: 7267 616e 697a 6174 696f 6e2f 4d75 7369  rganization/Musi
+000003e0: 6372 6561 7465 722f 6261 6467 652f 7374  creater/badge/st
+000003f0: 6172 2e73 7667 3f74 6865 6d65 3d67 7261  ar.svg?theme=gra
+00000400: 7929 5d28 6874 7470 733a 2f2f 6769 7465  y)](https://gite
+00000410: 652e 636f 6d2f 5472 694d 2d4f 7267 616e  e.com/TriM-Organ
+00000420: 697a 6174 696f 6e2f 4d75 7369 6372 6561  ization/Musicrea
+00000430: 7465 722f 7374 6172 6761 7a65 7273 290d  ter/stargazers).
+00000440: 0a5b 215b 4769 7465 6546 6f72 6b5d 2868  .[![GiteeFork](h
+00000450: 7474 7073 3a2f 2f67 6974 6565 2e63 6f6d  ttps://gitee.com
+00000460: 2f54 7269 4d2d 4f72 6761 6e69 7a61 7469  /TriM-Organizati
+00000470: 6f6e 2f4d 7573 6963 7265 6174 6572 2f62  on/Musicreater/b
+00000480: 6164 6765 2f66 6f72 6b2e 7376 673f 7468  adge/fork.svg?th
+00000490: 656d 653d 6772 6179 295d 2868 7474 7073  eme=gray)](https
+000004a0: 3a2f 2f67 6974 6565 2e63 6f6d 2f54 7269  ://gitee.com/Tri
+000004b0: 4d2d 4f72 6761 6e69 7a61 7469 6f6e 2f4d  M-Organization/M
+000004c0: 7573 6963 7265 6174 6572 2f6d 656d 6265  usicreater/membe
+000004d0: 7273 290d 0a5b 215b 4769 7448 7562 2052  rs)..[![GitHub R
+000004e0: 6570 6f20 7374 6172 735d 2868 7474 7073  epo stars](https
+000004f0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000500: 6f2f 6769 7468 7562 2f73 7461 7273 2f54  o/github/stars/T
+00000510: 7269 4d2d 4f72 6761 6e69 7a61 7469 6f6e  riM-Organization
+00000520: 2f4d 7573 6963 7265 6174 6572 3f63 6f6c  /Musicreater?col
+00000530: 6f72 3d77 6869 7465 266c 6f67 6f3d 4769  or=white&logo=Gi
+00000540: 7448 7562 2673 7479 6c65 3d70 6c61 7374  tHub&style=plast
+00000550: 6963 295d 2868 7474 7073 3a2f 2f67 6974  ic)](https://git
+00000560: 6875 622e 636f 6d2f 5472 694d 2d4f 7267  hub.com/TriM-Org
+00000570: 616e 697a 6174 696f 6e2f 4d75 7369 6372  anization/Musicr
+00000580: 6561 7465 722f 7374 6172 6761 7a65 7273  eater/stargazers
+00000590: 290d 0a5b 215b 4769 7448 7562 2052 6570  )..[![GitHub Rep
+000005a0: 6f20 466f 726b 735d 2868 7474 7073 3a2f  o Forks](https:/
+000005b0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000005c0: 6769 7468 7562 2f66 6f72 6b73 2f54 7269  github/forks/Tri
+000005d0: 4d2d 4f72 6761 6e69 7a61 7469 6f6e 2f4d  M-Organization/M
+000005e0: 7573 6963 7265 6174 6572 3f63 6f6c 6f72  usicreater?color
+000005f0: 3d77 6869 7465 266c 6f67 6f3d 4769 7448  =white&logo=GitH
+00000600: 7562 2673 7479 6c65 3d70 6c61 7374 6963  ub&style=plastic
+00000610: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000620: 622e 636f 6d2f 5472 694d 2d4f 7267 616e  b.com/TriM-Organ
+00000630: 697a 6174 696f 6e2f 4d75 7369 6372 6561  ization/Musicrea
+00000640: 7465 722f 666f 726b 7329 0d0a 0d0a 0d0a  ter/forks)......
+00000650: e7ae 80e4 bd93 e4b8 ade6 9687 f09f 87a8  ................
+00000660: f09f 87b3 207c 205b 456e 676c 6973 68f0  .... | [English.
+00000670: 9f87 acf0 9f87 a75d 2852 4541 444d 455f  .......](README_
+00000680: 454e 2e6d 6429 0d0a 0d0a 0d0a 2323 20e4  EN.md)......## .
+00000690: bb8b e7bb 8df0 9f9a 800d 0a0d 0ae9 9fb3  ................
+000006a0: c2b7 e588 9b20 e698 afe4 b880 e4b8 aae5  ..... ..........
+000006b0: 858d e8b4 b9e5 bc80 e6ba 90e7 9a84 e992  ................
+000006c0: 88e5 afb9 202a 2ae3 808a e688 91e7 9a84  .... **.........
+000006d0: e4b8 96e7 958c e380 8b2a 2a20 e79a 844d  .........** ...M
+000006e0: 4944 49e9 9fb3 e4b9 90e8 bdac e68d a2e5  IDI.............
+000006f0: ba93 0d0a 0d0a e6ac a2e8 bf8e e58a a0e7  ................
+00000700: bea4 efbc 9a5b 3836 3136 3834 3835 395d  .....[861684859]
+00000710: 2868 7474 7073 3a2f 2f6a 712e 7171 2e63  (https://jq.qq.c
+00000720: 6f6d 2f3f 5f77 763d 3130 3237 266b 3d68  om/?_wv=1027&k=h
+00000730: 7065 5278 7259 7229 0d0a 0d0a 2323 20e4  peRxrYr)....## .
+00000740: b88b e8bd bde5 ae89 e8a3 850d 0a0d 0a2d  ...............-
+00000750: 20e4 bdbf e794 a870 7970 690d 0a20 2020   ......pypi..   
+00000760: 2060 6060 6261 7368 0d0a 2020 2020 7069   ```bash..    pi
+00000770: 7020 696e 7374 616c 6c20 4d75 7369 6372  p install Musicr
+00000780: 6561 7465 720d 0a20 2020 2060 6060 0d0a  eater..    ```..
+00000790: 0d0a 2d20 e5a6 82e6 9e9c e587 bae7 8eb0  ..- ............
+000007a0: e994 99e8 afaf efbc 8ce5 8faf e4bb a5e5  ................
+000007b0: b09d e8af 95ef bc9a 0d0a 2020 2020 6060  ..........    ``
+000007c0: 6062 6173 680d 0a20 2020 2070 6970 2069  `bash..    pip i
+000007d0: 6e73 7461 6c6c 202d 6920 6874 7470 733a  nstall -i https:
+000007e0: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
+000007f0: 672f 7369 6d70 6c65 204d 7573 6963 7265  g/simple Musicre
+00000800: 6174 6572 0d0a 2020 2020 6060 600d 0a2d  ater..    ```..-
+00000810: 20ef bc88 e5af b9e4 ba8e e5bc 80e5 8f91   ...............
+00000820: e880 85e6 9da5 e8af b4ef bc89 e58d 87e7  ................
+00000830: baa7 efbc 9a0d 0a20 2020 2060 6060 6261  .......    ```ba
+00000840: 7368 0d0a 2020 2020 7069 7020 696e 7374  sh..    pip inst
+00000850: 616c 6c20 2d69 2068 7474 7073 3a2f 2f70  all -i https://p
+00000860: 7970 692e 7079 7468 6f6e 2e6f 7267 2f73  ypi.python.org/s
+00000870: 696d 706c 6520 4d75 7369 6372 6561 7465  imple Musicreate
+00000880: 7220 2d2d 7570 6772 6164 650d 0a20 2020  r --upgrade..   
+00000890: 2060 6060 0d0a 0d0a 2d20 e585 8be9 9a86   ```....- ......
+000008a0: e4bb 93e5 ba93 e5b9 b6e5 ae89 e8a3 850d  ................
+000008b0: 0a20 2020 2060 6060 6261 7368 0d0a 2020  .    ```bash..  
+000008c0: 2020 6769 7420 636c 6f6e 6520 6874 7470    git clone http
+000008d0: 733a 2f2f 6769 7465 652e 636f 6d2f 5472  s://gitee.com/Tr
+000008e0: 694d 2d4f 7267 616e 697a 6174 696f 6e2f  iM-Organization/
+000008f0: 4d75 7369 6372 6561 7465 722e 6769 740d  Musicreater.git.
+00000900: 0a20 2020 2063 6420 4d75 7369 6372 6561  .    cd Musicrea
+00000910: 7465 720d 0a20 2020 2070 7974 686f 6e20  ter..    python 
+00000920: 7365 7475 702e 7079 2069 6e73 7461 6c6c  setup.py install
+00000930: 0d0a 2020 2020 6060 600d 0a0d 0ae4 bba5  ..    ```.......
+00000940: e4b8 8ae5 91bd e4bb a4e7 a78d 2060 7079  ............ `py
+00000950: 7468 6f6e 60e3 8081 6070 6970 6020 e8af  thon`...`pip` ..
+00000960: b7e4 be9d e785 a7e5 9084 e4b8 aae7 8eaf  ................
+00000970: e5a2 83e4 b88d e590 8ce7 81b5 e6b4 bbe6  ................
+00000980: 9bb4 e68d a2ef bc8c e58f afe8 83bd e4b8  ................
+00000990: ba60 7079 7468 6f6e 3360 e688 9660 7069  .`python3`...`pi
+000009a0: 7033 60e4 b98b e7b1 bbe3 8082 0d0a 0d0a  p3`.............
+000009b0: 2323 20e6 9687 e6a1 a3f0 9f93 840d 0a0d  ## .............
+000009c0: 0a5b e794 9fe6 8890 e696 87e4 bbb6 e79a  .[..............
+000009d0: 84e4 bdbf e794 a85d 282e 2f64 6f63 732f  .......](./docs/
+000009e0: 2545 3725 3934 2539 4625 4536 2538 3825  %E7%94%9F%E6%88%
+000009f0: 3930 2545 3625 3936 2538 3725 4534 2542  90%E6%96%87%E4%B
+00000a00: 4225 4236 2545 3725 3941 2538 3425 4534  B%B6%E7%9A%84%E4
+00000a10: 2542 4425 4246 2545 3725 3934 2541 3825  %BD%BF%E7%94%A8%
+00000a20: 4538 2541 4625 4234 2545 3625 3938 2538  E8%AF%B4%E6%98%8
+00000a30: 452e 6d64 290d 0a0d 0a5b e4bb 93e5 ba93  E.md)....[......
+00000a40: 4150 49e6 9687 e6a1 a35d 282e 2f64 6f63  API......](./doc
+00000a50: 732f 2545 3525 4241 2539 3325 4537 2539  s/%E5%BA%93%E7%9
+00000a60: 4125 3834 2545 3725 3934 2539 4625 4536  A%84%E7%94%9F%E6
+00000a70: 2538 3825 3930 2545 3425 4238 2538 4525  %88%90%E4%B8%8E%
+00000a80: 4535 2538 4125 3946 2545 3825 3833 2542  E5%8A%9F%E8%83%B
+00000a90: 4425 4536 2539 3625 3837 2545 3625 4131  D%E6%96%87%E6%A1
+00000aa0: 2541 332e 6d64 290d 0a0d 0a23 2320 e4bd  %A3.md)....## ..
+00000ab0: 9ce8 8085 e29c 920d 0a0d 0ae9 8791 e7be  ................
+00000ac0: bf20 4569 6c6c 6573 efbc 9ae6 8891 e79a  . Eilles........
+00000ad0: 84e4 b896 e795 8ce5 9fba e5b2 a9e7 8988  ................
+00000ae0: e68c 87e4 bba4 e5b8 88ef bc8c e4b8 aae4  ................
+00000af0: baba e5bc 80e5 8f91 e880 85ef bc8c 42e7  ..............B.
+00000b00: ab99 e4b8 8de7 9fa5 e590 8d55 50e4 b8bb  ...........UP...
+00000b10: efbc 8ce6 b19f e8a5 bfe5 9ca8 e6a0 a1e9  ................
+00000b20: ab98 e4b8 ade7 949f e380 820d 0a0d 0ae8  ................
+00000b30: afb8 e891 9be4 baae e4b8 8ee5 85ab e58d  ................
+00000b40: a6e9 98b5 2062 6741 7272 6179 efbc 9ae6  .... bgArray....
+00000b50: 8891 e79a 84e4 b896 e795 8ce5 9fba e5b2  ................
+00000b60: a9e7 8988 e78e a9e5 aeb6 efbc 8ce5 969c  ................
+00000b70: e6ac a2e7 bc96 e7a8 8be5 928c e99f b3e4  ................
+00000b80: b990 efbc 8ce6 b7b1 e59c b3e5 889d e4ba  ................
+00000b90: 8ce5 ada6 e794 9fe3 8082 0d0a 0d0a 2323  ..............##
+00000ba0: 20e8 87b4 e8b0 a2f0 9f99 8f0d 0ae6 9cac   ...............
+00000bb0: e887 b4e8 b0a2 e588 97e8 a1a8 e68e 92e5  ................
+00000bc0: 908d e697 a0e9 a1ba e5ba 8fe3 8082 0d0a  ................
+00000bd0: 0d0a 2d20 e684 9fe8 b0a2 202a 2ae6 9880  ..- ...... **...
+00000be0: e6a2 a62a 2a5c 3c51 5131 3531 3533 3939  ...**\<QQ1515399
+00000bf0: 3838 355c 3e20 e689 bee5 87ba e68c 87e4  885\> ..........
+00000c00: bba4 e794 9fe6 8890 e994 99e8 afaf 6275  ..............bu
+00000c10: 67e5 b9b6 e68c 87e6 ada3 0d0a 2d20 e684  g...........- ..
+00000c20: 9fe8 b0a2 e794 b120 2a2a 4368 6172 6c69  ....... **Charli
+00000c30: 655f 5069 6e67 20e2 809c e69f a5e7 9086  e_Ping .........
+00000c40: e5b9 b3e2 809d 2a2a 20e5 b8a6 e69d a5e7  ......** .......
+00000c50: 9a84 4244 58e6 9687 e4bb b6e8 bdac e68d  ..BDX...........
+00000c60: a2e5 8f82 e880 83ef bc8c e4bb a5e5 8f8a  ................
+00000c70: 4d49 4449 2de6 8891 e79a 84e4 b896 e795  MIDI-...........
+00000c80: 8ce5 afb9 e5ba 94e4 b990 e599 a8e5 8f82  ................
+00000c90: e880 83e8 a1a8 e6a0 bc0d 0a2d 20e6 849f  ...........- ...
+00000ca0: e8b0 a2e7 94b1 202a 2a5b 434d 415f 3234  ...... **[CMA_24
+00000cb0: 3031 5054 5d28 6874 7470 733a 2f2f 6769  01PT](https://gi
+00000cc0: 7468 7562 2e63 6f6d 2f43 4d41 3234 3031  thub.com/CMA2401
+00000cd0: 5054 292a 2a20 e4b8 bae6 8891 e4bb ace7  PT)** ..........
+00000ce0: 9a84 e8bd afe4 bbb6 e5bc 80e5 8f91 e79a  ................
+00000cf0: 84e4 b880 e4ba 9be6 96b9 e99d a2e8 bf9b  ................
+00000d00: e8a1 8ce6 8c87 e5af bcef bc8c e590 8ce6  ................
+00000d10: 97b6 e688 91e4 bbac e58f 82e8 8083 e4ba  ................
+00000d20: 86e4 bb96 e79a 8442 4458 776f 726b 7368  .......BDXworksh
+00000d30: 6f70 e4bd 9ce4 b8ba 4244 58e7 bb93 e69e  op......BDX.....
+00000d40: 84e7 bc96 e8be 91e7 9a84 e58f 82e8 8083  ................
+00000d50: 0d0a 2d20 e684 9fe8 b0a2 e794 b120 2a2a  ..- ......... **
+00000d60: 5b44 6973 6c69 6e6b 2053 666f 727a 615d  [Dislink Sforza]
+00000d70: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000d80: 636f 6d2f 4469 736c 696e 6b29 20e2 809c  com/Dislink) ...
+00000d90: e696 ade8 8194 c2b7 e696 afe7 a68f e5b0  ................
+00000da0: 94e6 898e e280 9d2a 2a5c 3c51 5131 3630  .......**\<QQ160
+00000db0: 3035 3135 3331 345c 3e20 e5b8 a6e6 9da5  0515314\> ......
+00000dc0: e79a 846d 6964 69e9 9fb3 e889 b2e8 a7a3  ...midi.........
+00000dd0: e69e 90e4 bba5 e58f 8ae8 bdac e68d a2e6  ................
+00000de0: 8c87 e4bb a4e7 9a84 e7ae 97e6 b395 efbc  ................
+00000df0: 8ce6 8891 e4bb ace5 b086 e585 b6e6 94b9  ................
+00000e00: e7bc 96e5 b9b6 e5ba 94e7 94a8 efbc 9be5  ................
+00000e10: 908c e697 b6ef bc8c e684 9fe8 b0a2 e4bb  ................
+00000e20: 96e7 9a84 5be7 bd91 e9a1 b5e7 8988 e8bd  ....[...........
+00000e30: ace6 8da2 e599 a85d 2868 7474 7073 3a2f  .......](https:/
+00000e40: 2f64 6973 6c69 6e6b 2e67 6974 6875 622e  /dislink.github.
+00000e50: 696f 2f6d 6964 6932 6264 782f 29e7 bb99  io/midi2bdx/)...
+00000e60: e688 91e4 bbac e79a 84e5 bc80 e58f 91e4  ................
+00000e70: b88e e69b b4e6 96b0 e5b8 a6e6 9da5 e5b7  ................
+00000e80: a8e5 a4a7 e79a 84e5 8e8b e58a 9be5 928c  ................
+00000e90: e58a a8e5 8a9b efbc 8ce8 aea9 e688 91e4  ................
+00000ea0: bbac e59c a8e5 8e9f e69c ace4 b880 e9aa  ................
+00000eb0: 91e7 bb9d e5b0 98e7 9a84 e691 b8e9 b1bc  ................
+00000ec0: e981 93e8 b7af e4b8 8ae8 bdac e590 91e5  ................
+00000ed0: bc80 e58f 91ef bc8c e5b8 8ce6 9c9b e4bb  ................
+00000ee0: 96e8 83bd e880 83e4 b88a e4b8 80e4 b8aa  ................
+00000ef0: e790 86e6 83b3 e79a 84e5 a4a7 e5ad a6ef  ................
+00000f00: bc81 0d0a 2d20 e684 9fe8 b0a2 202a 2a54  ....- ...... **T
+00000f10: 6f75 6368 20e2 809c e581 b7e5 9083 e280  ouch ...........
+00000f20: 9d2a 2a5c 3c51 5131 3739 3335 3337 3136  .**\<QQ179353716
+00000f30: 345c 3e20 e68f 90e4 be9b e79a 8442 4458  4\> .........BDX
+00000f40: e5af bce5 85a5 e6b5 8be8 af95 e694 afe6  ................
+00000f50: 8c81 efbc 8ce5 b9b6 e5af b9e7 a88b e5ba  ................
+00000f60: 8fe7 9a84 e694 b9e8 bf9b e68f 90e4 be9b  ................
+00000f70: e4ba 86e4 b8b0 e5af 8ce7 9a84 e684 8fe8  ................
+00000f80: a781 efbc 9be5 908c e697 b6e4 b99f e684  ................
+00000f90: 9fe8 b0a2 e4bb 96e7 9a84 e4b8 8de6 96ad  ................
+00000fa0: e5b0 9de8 af95 e696 b0e7 9a84 e586 85e5  ................
+00000fb0: aeb9 efbc 8ce4 bdbf e688 91e4 bbac e79a  ................
+00000fc0: 84e6 8e92 e994 99e6 9bb4 e8bf 9be4 b880  ................
+00000fd0: e6ad a50d 0a2d 20e6 849f e8b0 a220 2a2a  .....- ...... **
+00000fe0: 4d6f 6e6f 2a2a 5c3c 5151 3733 3838 3933  Mono**\<QQ738893
+00000ff0: 3038 375c 3e20 e58f 8de9 a688 e5ae 89e8  087\> ..........
+00001000: a385 e697 b6e7 9a84 e997 aee9 a298 efbc  ................
+00001010: 8ce8 be85 e58a a9e6 8891 e4bb ace6 89be  ................
+00001020: e588 b0e4 ba86 e8a7 86e7 aa97 e693 8de4  ................
+00001030: bd9c e7b3 bbe7 bb9f e4b8 8be7 9a84 e585  ................
+00001040: bce5 aeb9 e680 a7e9 97ae e9a2 980d 0a2d  ...............-
+00001050: 20e6 849f e8b0 a220 2a2a 416d 6d65 6c69   ...... **Ammeli
+00001060: 6120 e280 9ce8 89be e7b1 b3e5 88a9 e4ba  a ..............
+00001070: 9ae2 809d 2a2a 5c3c 5151 3238 3338 3333  ....**\<QQ283833
+00001080: 3436 3337 5c3e 20e6 95a6 e4bf 83e6 8891  4637\> .........
+00001090: e4bb ace8 bf9b e8a1 8ce6 96b0 e79a 84e5  ................
+000010a0: 8a9f e883 bde5 bc80 e58f 91ef bc8c e5b9  ................
+000010b0: b6e4 b8ba e696 b0e5 8a9f e883 bde6 8f90  ................
+000010c0: e587 bae4 ba86 e99d 9ee5 b8b8 e4bc 98e7  ................
+000010d0: a780 e79a 84e5 a4a7 e987 8fe5 bbba e8ae  ................
+000010e0: aeef bc8c e4bb a5e5 8f8a e68f 90e4 be9b  ................
+000010f0: e79a 8442 4458 e5af bce5 85a5 e6b5 8be8  ...BDX..........
+00001100: af95 e694 afe6 8c81 efbc 8ce4 b8ba e688  ................
+00001110: 91e4 bbac e79a 84e6 96b0 e7bb 93e6 9e84  ................
+00001120: e794 9fe6 8890 e7ae 97e6 b395 e68f 90e4  ................
+00001130: be9b e4ba 86e5 a4a7 e987 8fe7 9a84 e5ae  ................
+00001140: 9ee9 9985 e790 86e8 aeba e694 afe6 8c81  ................
+00001150: 0d0a 2d20 e684 9fe8 b0a2 202a 2a5b e7a5  ..- ...... **[..
+00001160: 9ee7 bebd 5d28 6874 7470 733a 2f2f 6769  ....](https://gi
+00001170: 7465 652e 636f 6d2f 736e 6f77 796b 616d  tee.com/snowykam
+00001180: 6929 20e2 809c 5b53 6e6f 7779 4b61 6d69  i) ...[SnowyKami
+00001190: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000011a0: 2e63 6f6d 2f73 6e6f 7779 6669 7265 666c  .com/snowyfirefl
+000011b0: 7929 e280 9d2a 2a20 e5af b9e6 8891 e4bb  y)...** ........
+000011c0: ace9 a1b9 e79b aee7 9a84 e694 afe6 8c81  ................
+000011d0: e4b8 8ee5 aea3 e4bc a0ef bc8c e5b8 8ce6  ................
+000011e0: 9c9b e4bb 96e8 83bd e880 83e7 9a84 e4b8  ................
+000011f0: 80e6 8980 e4bc 98e7 a780 e79a 84e5 a4a7  ................
+00001200: e5ad a6ef bc81 0d0a 2d20 e684 9fe8 b0a2  ........- ......
+00001210: 202a 2ae6 8c87 e4bb a4e5 b888 5fe8 8ba6   **........._...
+00001220: e58a 9be6 8095 2070 6c61 796a 7569 6365  ...... playjuice
+00001230: 3132 332a 2a5c 3c51 5132 3430 3636 3731  123**\<QQ2406671
+00001240: 3937 5c3e e4b8 bae6 8891 e4bb ace7 9a84  97\>............
+00001250: e7a8 8be5 ba8f e689 bee5 87ba e994 99e8  ................
+00001260: afaf efbc 8ce5 b9b6 e68f 90e9 8692 e688  ................
+00001270: 91e4 bbac e4bf aee5 a48d e4b8 80e4 b8aa  ................
+00001280: e4b8 80e7 9bb4 e5ad 98e5 9ca8 e79a 84e5  ................
+00001290: a4a7 6275 67e3 8082 0d0a 2d20 e684 9fe8  ..bug.....- ....
+000012a0: b0a2 202a 2ae9 9bb7 e99c 862a 2a5c 3c51  .. **......**\<Q
+000012b0: 5133 3535 3532 3638 3531 395c 3ee4 b8ba  Q3555268519\>...
+000012c0: e688 91e4 bbac e79a 84e7 a88b e5ba 8fe6  ................
+000012d0: 89be e587 bae9 9499 e8af afef bc8c e5b9  ................
+000012e0: b6e6 8f90 e986 92e4 bfae e5a4 8d62 7567  .............bug
+000012f0: e380 820d 0a0d 0a3e 09e6 849f e8b0 a2e5  .......>........
+00001300: b9bf e5a4 a7e7 bea4 e58f 8be4 b8ba e6ad  ................
+00001310: a4e7 a88b e5ba 8fe6 8f90 e4be 9be7 9a84  ................
+00001320: e6b5 8be8 af95 e7ad 89e6 94af e68c 810d  ................
+00001330: 0a3e 0d0a 3e09 e88b a5e6 82a8 e5af b9e6  .>..>...........
+00001340: 8891 e4bb ace6 9c89 e689 80e8 b4a1 e78c  ................
+00001350: aee4 bd86 e682 a8e7 9a84 e590 8de5 ad97  ................
+00001360: e6b2 a1e6 9c89 e698 bee7 a4ba e59c a8e6  ................
+00001370: ada4 e588 97e8 a1a8 e4b8 adef bc8c e8af  ................
+00001380: b7e8 8194 e7b3 bbe6 8891 e4bb acef bc81  ................
+00001390: 0d0a 0d0a 2323 20e8 8194 e7b3 bbf0 9f93  ....## .........
+000013a0: 9e0d 0a0d 0ae8 8ba5 e981 87e5 88b0 e5ba  ................
+000013b0: 93e4 b8ad e79a 84e9 97ae e9a2 98ef bc8c  ................
+000013c0: e6ac a2e8 bf8e e59c a85b e6ad a45d 2868  .........[...](h
+000013d0: 7474 7073 3a2f 2f67 6974 6565 2e63 6f6d  ttps://gitee.com
+000013e0: 2f54 7269 4d2d 4f72 6761 6e69 7a61 7469  /TriM-Organizati
+000013f0: 6f6e 2f4d 7573 6963 7265 6174 6572 2f69  on/Musicreater/i
+00001400: 7373 7565 732f 6e65 7729 e68f 90e5 87ba  ssues/new)......
+00001410: e4bd a0e7 9a84 6973 7375 65e3 8082 0d0a  ......issue.....
+00001420: 0d0a e5a6 82e6 9e9c e99c 80e8 a681 e4b8  ................
+00001430: 8ee5 bc80 e58f 91e7 bb84 e8bf 9be8 a18c  ................
+00001440: e4ba a4e6 b581 efbc 8ce6 aca2 e8bf 8ee5  ................
+00001450: 8aa0 e585 a5e6 8891 e4bb ace7 9a84 5be5  ..............[.
+00001460: bc80 e58f 91e9 97b2 e881 8a51 e7be a45d  ...........Q...]
+00001470: 2868 7474 7073 3a2f 2f6a 712e 7171 2e63  (https://jq.qq.c
+00001480: 6f6d 2f3f 5f77 763d 3130 3237 266b 3d68  om/?_wv=1027&k=h
+00001490: 7065 5278 7259 7229 e380 820d 0a0d 0a2d  peRxrYr).......-
+000014a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000014b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000014c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0ae6  -----------.....
+000014d0: ada4 e9a1 b9e7 9bae e5b9 b6e9 9d9e e4b8  ................
+000014e0: 80e4 b8aa e5ae 98e6 96b9 20e3 808a e688  .......... .....
+000014f0: 91e7 9a84 e4b8 96e7 958c e380 8bef bc88  ................
+00001500: 2a4d 696e 6563 7261 6674 2aef bc89 e9a1  *Minecraft*.....
+00001510: b9e7 9bae 0d0a 0d0a e6ad a4e9 a1b9 e79b  ................
+00001520: aee4 b88d e99a b6e5 b19e e688 96e5 85b3  ................
+00001530: e881 94e4 ba8e 204d 6f6a 616e 6720 5374  ...... Mojang St
+00001540: 7564 696f 7320 e688 9620 e5be aee8 bdaf  udios ... ......
+00001550: 0d0a 0d0a e6ad a4e9 a1b9 e79b aee4 baa6  ................
+00001560: e4b8 8de4 b88e 20e7 bd91 e698 9320 e79b  ...... ...... ..
+00001570: b8e5 85b3 0d0a 0d0a e280 9c4d 696e 6563  ...........Minec
+00001580: 7261 6674 e280 9de6 98af 204d 6f6a 616e  raft...... Mojan
+00001590: 6720 5379 6e65 7267 6965 7320 4142 20e7  g Synergies AB .
+000015a0: 9a84 e595 86e6 a087 efbc 8ce6 ada4 e9a1  ................
+000015b0: b9e7 9bae e4b8 ade6 8980 e69c 89e5 afb9  ................
+000015c0: e4ba 8ee2 809c e688 91e7 9a84 e4b8 96e7  ................
+000015d0: 958c e280 9de3 8081 e280 9c4d 696e 6563  ...........Minec
+000015e0: 7261 6674 e280 9de7 ad89 e79b b8e5 85b3  raft............
+000015f0: e7a7 b0e5 91bc e59d 87e4 b8ba e5bc 95e7  ................
+00001600: 94a8 e680 a7e4 bdbf e794 a80d 0a0d 0a2a  ...............*
+00001610: 20e4 b88a e696 87e6 8f90 e58f 8ae7 9a84   ...............
+00001620: 20e7 bd91 e698 9320 e585 ace5 8fb8 efbc   ...... ........
+00001630: 8ce6 8c87 e4bb a3e7 9a84 e698 afe5 9ca8  ................
+00001640: e4b8 ade5 9bbd e5a4 a7e9 9986 e8bf 90e8  ................
+00001650: 90a5 e380 8ae6 8891 e79a 84e4 b896 e795  ................
+00001660: 8cef bc9a e4b8 ade5 9bbd e789 88e3 808b  ................
+00001670: e79a 84e4 b88a e6b5 b7e7 bd91 e4b9 8be6  ................
+00001680: 9893 e7bd 91e7 bb9c e7a7 91e6 8a80 e58f  ................
+00001690: 91e5 b195 e69c 89e9 9990 e585 ace5 8fb8  ................
+000016a0: 0d0a 0d0a 4e4f 5420 414e 204f 4646 4943  ....NOT AN OFFIC
+000016b0: 4941 4c20 4d49 4e45 4352 4146 5420 5052  IAL MINECRAFT PR
+000016c0: 4f44 5543 542e 0d0a 0d0a 4e4f 5420 4150  ODUCT.....NOT AP
+000016d0: 5052 4f56 4544 2042 5920 4f52 2041 5353  PROVED BY OR ASS
+000016e0: 4f43 4941 5445 4420 5749 5448 204d 4f4a  OCIATED WITH MOJ
+000016f0: 414e 4720 4f52 204d 4943 524f 534f 4654  ANG OR MICROSOFT
+00001700: 2e0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a5b 4269  .............[Bi
+00001710: 6c69 6269 6c69 3a20 e987 91e7 bebf 454c  libili: ......EL
+00001720: 535d 3a20 6874 7470 733a 2f2f 696d 672e  S]: https://img.
+00001730: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00001740: 2f42 696c 6962 696c 692d 2545 3525 3837  /Bilibili-%E5%87
+00001750: 2538 4325 4534 2542 4125 3931 2545 3925  %8C%E4%BA%91%E9%
+00001760: 3837 2539 3125 4537 2542 4525 4246 2d30  87%91%E7%BE%BF-0
+00001770: 3041 3145 373f 7374 796c 653d 666f 722d  0A1E7?style=for-
+00001780: 7468 652d 6261 6467 650d 0a5b 4269 6c69  the-badge..[Bili
+00001790: 6269 6c69 3a20 e8af b8e8 919b e4ba aee4  bili: ..........
+000017a0: b88e e585 abe5 8da6 e998 b55d 3a20 6874  ...........]: ht
+000017b0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000017c0: 732e 696f 2f62 6164 6765 2f42 696c 6962  s.io/badge/Bilib
+000017d0: 696c 692d 2545 3825 4146 2542 3825 4538  ili-%E8%AF%B8%E8
+000017e0: 2539 3125 3942 2545 3425 4241 2541 4525  %91%9B%E4%BA%AE%
+000017f0: 4534 2542 3825 3845 2545 3525 3835 2541  E4%B8%8E%E5%85%A
+00001800: 4225 4535 2538 4425 4136 2545 3925 3938  B%E5%8D%A6%E9%98
+00001810: 2542 352d 3030 4131 4537 3f73 7479 6c65  %B5-00A1E7?style
+00001820: 3d66 6f72 2d74 6865 2d62 6164 6765 0d0a  =for-the-badge..
+00001830: 5b43 6f64 6553 7479 6c65 3a20 626c 6163  [CodeStyle: blac
+00001840: 6b5d 3a20 6874 7470 733a 2f2f 696d 672e  k]: https://img.
+00001850: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00001860: 2f63 6f64 6525 3230 7374 796c 652d 626c  /code%20style-bl
+00001870: 6163 6b2d 3132 3131 3130 2e73 7667 3f73  ack-121110.svg?s
+00001880: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
+00001890: 6765 0d0a 5b70 7974 686f 6e5d 3a20 6874  ge..[python]: ht
+000018a0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000018b0: 732e 696f 2f62 6164 6765 2f70 7974 686f  s.io/badge/pytho
+000018c0: 6e2d 332e 362d 4142 3730 4646 3f73 7479  n-3.6-AB70FF?sty
+000018d0: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+000018e0: 0d0a 5b72 656c 6561 7365 5d3a 2068 7474  ..[release]: htt
+000018f0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00001900: 2e69 6f2f 6769 7468 7562 2f76 2f72 656c  .io/github/v/rel
+00001910: 6561 7365 2f45 696c 6c65 7357 616e 2f4d  ease/EillesWan/M
+00001920: 7573 6963 7265 6174 6572 3f73 7479 6c65  usicreater?style
+00001930: 3d66 6f72 2d74 6865 2d62 6164 6765 0d0a  =for-the-badge..
+00001940: 5b6c 6963 656e 7365 5d3a 2068 7474 7073  [license]: https
+00001950: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00001960: 6f2f 6261 6467 652f 4c69 6365 6e63 652d  o/badge/Licence-
+00001970: 4170 6163 6865 2d32 3238 4232 323f 7374  Apache-228B22?st
+00001980: 796c 653d 666f 722d 7468 652d 6261 6467  yle=for-the-badg
+00001990: 650d 0a                                  e..
```

### Comparing `Musicreater-0.4.0/PKG-INFO` & `Musicreater-0.5.0/Musicreater.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 204d 7573  : 2.1..Name: Mus
 00000020: 6963 7265 6174 6572 0d0a 5665 7273 696f  icreater..Versio
-00000030: 6e3a 2030 2e34 2e30 0d0a 5375 6d6d 6172  n: 0.4.0..Summar
+00000030: 6e3a 2030 2e35 2e30 0d0a 5375 6d6d 6172  n: 0.5.0..Summar
 00000040: 793a 20e4 b880 e6ac bee5 858d e8b4 b9e5  y: .............
 00000050: bc80 e6ba 90e7 9a84 20e3 808a e688 91e7  ........ .......
 00000060: 9a84 e4b8 96e7 958c e380 8b20 6d69 64e9  ........... mid.
 00000070: 9fb3 e4b9 90e8 bdac e68d a2e5 ba93 e380  ................
 00000080: 820d 0a48 6f6d 652d 7061 6765 3a20 6874  ...Home-page: ht
 00000090: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000000a0: 2f54 7269 4d2d 4f72 6761 6e69 7a61 7469  /TriM-Organizati
@@ -53,344 +53,424 @@
 00000340: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
 00000350: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
 00000360: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
 00000370: 0d0a 4465 7363 7269 7074 696f 6e2d 436f  ..Description-Co
 00000380: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
 00000390: 2f6d 6172 6b64 6f77 6e0d 0a4c 6963 656e  /markdown..Licen
 000003a0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-000003b0: 2e6d 640d 0a0d 0a3c 6831 2061 6c69 676e  .md....<h1 align
-000003c0: 3d22 6365 6e74 6572 223e e99f b3c2 b7e5  ="center">......
-000003d0: 889b 204d 7573 6963 7265 6174 6572 3c2f  .. Musicreater</
-000003e0: 6831 3e0d 0a0d 0a3c 7020 616c 6967 6e3d  h1>....<p align=
-000003f0: 2263 656e 7465 7222 3e0d 0a3c 696d 6720  "center">..<img 
-00000400: 7769 6474 683d 2231 3238 2220 6865 6967  width="128" heig
-00000410: 6874 3d22 3132 3822 2073 7263 3d22 6874  ht="128" src="ht
-00000420: 7470 733a 2f2f 7331 2e61 7831 782e 636f  tps://s1.ax1x.co
-00000430: 6d2f 3230 3232 2f30 352f 3036 2f4f 7568  m/2022/05/06/Ouh
-00000440: 6768 6a2e 6d64 2e70 6e67 2220 3e0d 0a3c  ghj.md.png" >..<
-00000450: 2f70 3e0d 0a0d 0a3c 6833 2061 6c69 676e  /p>....<h3 align
-00000460: 3d22 6365 6e74 6572 223e e4b8 80e6 acbe  ="center">......
-00000470: e585 8de8 b4b9 e5bc 80e6 ba90 e79a 8420  ............... 
-00000480: e380 8ae6 8891 e79a 84e4 b896 e795 8ce3  ................
-00000490: 808b 204d 4944 49e9 9fb3 e4b9 90e8 bdac  .. MIDI.........
-000004a0: e68d a2e5 ba93 e380 823c 2f68 333e 0d0a  .........</h3>..
-000004b0: 0d0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
-000004c0: 6572 223e 0d0a 3c69 6d67 2073 7263 3d22  er">..<img src="
-000004d0: 6874 7470 733a 2f2f 666f 7274 6865 6261  https://fortheba
-000004e0: 6467 652e 636f 6d2f 696d 6167 6573 2f62  dge.com/images/b
-000004f0: 6164 6765 732f 6275 696c 742d 7769 7468  adges/built-with
-00000500: 2d6c 6f76 652e 7376 6722 3e0d 0a3c 703e  -love.svg">..<p>
-00000510: 0d0a 0d0a 0d0a 5b21 5b5d 5b42 696c 6962  ......[![][Bilib
-00000520: 696c 693a 20e5 878c e4ba 91e9 8791 e7be  ili: ...........
-00000530: bf5d 5d28 6874 7470 733a 2f2f 7370 6163  .]](https://spac
-00000540: 652e 6269 6c69 6269 6c69 2e63 6f6d 2f33  e.bilibili.com/3
-00000550: 3937 3336 3930 3032 2f29 0d0a 5b21 5b5d  97369002/)..[![]
-00000560: 5b42 696c 6962 696c 693a 20e8 afb8 e891  [Bilibili: .....
-00000570: 9be4 baae e4b8 8ee5 85ab e58d a6e9 98b5  ................
-00000580: 5d5d 2868 7474 7073 3a2f 2f73 7061 6365  ]](https://space
-00000590: 2e62 696c 6962 696c 692e 636f 6d2f 3630  .bilibili.com/60
-000005a0: 3430 3732 3437 3429 200d 0a5b 215b 436f  4072474) ..[![Co
-000005b0: 6465 5374 796c 653a 2062 6c61 636b 5d5d  deStyle: black]]
-000005c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000005d0: 636f 6d2f 7073 662f 626c 6163 6b29 0d0a  com/psf/black)..
-000005e0: 5b21 5b5d 5b70 7974 686f 6e5d 5d28 6874  [![][python]](ht
-000005f0: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
-00000600: 2e6f 7267 2f29 0d0a 5b21 5b5d 5b6c 6963  .org/)..[![][lic
-00000610: 656e 7365 5d5d 284c 4943 454e 5345 290d  ense]](LICENSE).
-00000620: 0a5b 215b 5d5b 7265 6c65 6173 655d 5d28  .[![][release]](
-00000630: 2e2e 2f2e 2e2f 7265 6c65 6173 6573 290d  ../../releases).
-00000640: 0a0d 0a0d 0ae7 ae80 e4bd 93e4 b8ad e696  ................
-00000650: 87f0 9f87 a8f0 9f87 b320 7c20 5b45 6e67  ......... | [Eng
-00000660: 6c69 7368 f09f 87ac f09f 87a7 5d28 5245  lish........](RE
-00000670: 4144 4d45 5f45 4e2e 6d64 290d 0a0d 0a0d  ADME_EN.md).....
-00000680: 0a23 2320 e4bb 8be7 bb8d f09f 9a80 0d0a  .## ............
-00000690: 0d0a e99f b3c2 b7e5 889b 20e6 98af e4b8  .......... .....
-000006a0: 80e4 b8aa e585 8de8 b4b9 e5bc 80e6 ba90  ................
-000006b0: e79a 84e9 9288 e5af b920 2a2a e380 8ae6  ......... **....
-000006c0: 8891 e79a 84e4 b896 e795 8ce3 808b 2a2a  ..............**
-000006d0: 20e7 9a84 4d49 4449 e99f b3e4 b990 e8bd   ...MIDI........
-000006e0: ace6 8da2 e5ba 930d 0a0d 0ae6 aca2 e8bf  ................
-000006f0: 8ee5 8aa0 e7be a4ef bc9a 5b38 3631 3638  ..........[86168
-00000700: 3438 3539 5d28 6874 7470 733a 2f2f 6a71  4859](https://jq
-00000710: 2e71 712e 636f 6d2f 3f5f 7776 3d31 3032  .qq.com/?_wv=102
-00000720: 3726 6b3d 6870 6552 7872 5972 290d 0a0d  7&k=hpeRxrYr)...
-00000730: 0a23 2320 e4b8 8be8 bdbd e5ae 89e8 a385  .## ............
-00000740: 0d0a 0d0a 2d20 e4bd bfe7 94a8 7079 7069  ....- ......pypi
-00000750: 0d0a 2020 2020 6060 6062 6173 680d 0a20  ..    ```bash.. 
-00000760: 2020 2070 6970 2069 6e73 7461 6c6c 204d     pip install M
-00000770: 7573 6963 7265 6174 6572 0d0a 2020 2020  usicreater..    
-00000780: 6060 600d 0a0d 0a2d 20e5 a682 e69e 9ce5  ```....- .......
-00000790: 87ba e78e b0e9 9499 e8af afef bc8c e58f  ................
-000007a0: afe4 bba5 e5b0 9de8 af95 efbc 9a0d 0a20  ............... 
-000007b0: 2020 2060 6060 6261 7368 0d0a 2020 2020     ```bash..    
-000007c0: 7069 7020 696e 7374 616c 6c20 2d69 2068  pip install -i h
-000007d0: 7474 7073 3a2f 2f70 7970 692e 7079 7468  ttps://pypi.pyth
-000007e0: 6f6e 2e6f 7267 2f73 696d 706c 6520 4d75  on.org/simple Mu
-000007f0: 7369 6372 6561 7465 720d 0a20 2020 2060  sicreater..    `
-00000800: 6060 0d0a 2d20 efbc 88e5 afb9 e4ba 8ee5  ``..- ..........
-00000810: bc80 e58f 91e8 8085 e69d a5e8 afb4 efbc  ................
-00000820: 89e5 8d87 e7ba a7ef bc9a 0d0a 2020 2020  ............    
-00000830: 6060 6062 6173 680d 0a20 2020 2070 6970  ```bash..    pip
-00000840: 2069 6e73 7461 6c6c 202d 6920 6874 7470   install -i http
-00000850: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
-00000860: 6f72 672f 7369 6d70 6c65 204d 7573 6963  org/simple Music
-00000870: 7265 6174 6572 202d 2d75 7067 7261 6465  reater --upgrade
-00000880: 0d0a 2020 2020 6060 600d 0a0d 0a2d 20e5  ..    ```....- .
-00000890: 858b e99a 86e4 bb93 e5ba 93e5 b9b6 e5ae  ................
-000008a0: 89e8 a385 0d0a 2020 2020 6060 6062 6173  ......    ```bas
-000008b0: 680d 0a20 2020 2067 6974 2063 6c6f 6e65  h..    git clone
-000008c0: 2068 7474 7073 3a2f 2f67 6974 6565 2e63   https://gitee.c
-000008d0: 6f6d 2f54 7269 4d2d 4f72 6761 6e69 7a61  om/TriM-Organiza
-000008e0: 7469 6f6e 2f4d 7573 6963 7265 6174 6572  tion/Musicreater
-000008f0: 2e67 6974 0d0a 2020 2020 6364 204d 7573  .git..    cd Mus
-00000900: 6963 7265 6174 6572 0d0a 2020 2020 7079  icreater..    py
-00000910: 7468 6f6e 2073 6574 7570 2e70 7920 696e  thon setup.py in
-00000920: 7374 616c 6c0d 0a20 2020 2060 6060 0d0a  stall..    ```..
-00000930: 0d0a e4bb a5e4 b88a e591 bde4 bba4 e7a7  ................
-00000940: 8d20 6070 7974 686f 6e60 e380 8160 7069  . `python`...`pi
-00000950: 7060 20e8 afb7 e4be 9de7 85a7 e590 84e4  p` .............
-00000960: b8aa e78e afe5 a283 e4b8 8de5 908c e781  ................
-00000970: b5e6 b4bb e69b b4e6 8da2 efbc 8ce5 8faf  ................
-00000980: e883 bde4 b8ba 6070 7974 686f 6e33 60e6  ......`python3`.
-00000990: 8896 6070 6970 3360 e4b9 8be7 b1bb e380  ..`pip3`........
-000009a0: 820d 0a0d 0a23 2320 e696 87e6 a1a3 f09f  .....## ........
-000009b0: 9384 0d0a 0d0a 5be7 949f e688 90e6 9687  ......[.........
-000009c0: e4bb b6e7 9a84 e4bd bfe7 94a8 5d28 6874  ............](ht
-000009d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000009e0: 2f54 7269 4d2d 4f72 6761 6e69 7a61 7469  /TriM-Organizati
-000009f0: 6f6e 2f4d 7573 6963 7265 6174 6572 2f62  on/Musicreater/b
-00000a00: 6c6f 622f 6d61 7374 6572 2f64 6f63 732f  lob/master/docs/
-00000a10: 2545 3725 3934 2539 4625 4536 2538 3825  %E7%94%9F%E6%88%
-00000a20: 3930 2545 3625 3936 2538 3725 4534 2542  90%E6%96%87%E4%B
-00000a30: 4225 4236 2545 3725 3941 2538 3425 4534  B%B6%E7%9A%84%E4
-00000a40: 2542 4425 4246 2545 3725 3934 2541 3825  %BD%BF%E7%94%A8%
-00000a50: 4538 2541 4625 4234 2545 3625 3938 2538  E8%AF%B4%E6%98%8
-00000a60: 452e 6d64 290d 0a0d 0a5b e4bb 93e5 ba93  E.md)....[......
-00000a70: 4150 49e6 9687 e6a1 a35d 2868 7474 7073  API......](https
-00000a80: 3a2f 2f67 6974 6875 622e 636f 6d2f 5472  ://github.com/Tr
-00000a90: 694d 2d4f 7267 616e 697a 6174 696f 6e2f  iM-Organization/
-00000aa0: 4d75 7369 6372 6561 7465 722f 626c 6f62  Musicreater/blob
-00000ab0: 2f6d 6173 7465 722f 646f 6373 2f25 4535  /master/docs/%E5
-00000ac0: 2542 4125 3933 2545 3725 3941 2538 3425  %BA%93%E7%9A%84%
-00000ad0: 4537 2539 3425 3946 2545 3625 3838 2539  E7%94%9F%E6%88%9
-00000ae0: 3025 4534 2542 3825 3845 2545 3525 3841  0%E4%B8%8E%E5%8A
-00000af0: 2539 4625 4538 2538 3325 4244 2545 3625  %9F%E8%83%BD%E6%
-00000b00: 3936 2538 3725 4536 2541 3125 4133 2e6d  96%87%E6%A1%A3.m
-00000b10: 6429 0d0a 0d0a 2323 20e4 bd9c e880 85e2  d)....## .......
-00000b20: 9c92 0d0a 0d0a e987 91e7 bebf 2045 696c  ............ Eil
-00000b30: 6c65 73ef bc9a e688 91e7 9a84 e4b8 96e7  les.............
-00000b40: 958c e59f bae5 b2a9 e789 88e6 8c87 e4bb  ................
-00000b50: a4e5 b888 efbc 8ce4 b8aa e4ba bae5 bc80  ................
-00000b60: e58f 91e8 8085 efbc 8c42 e7ab 99e4 b88d  .........B......
-00000b70: e79f a5e5 908d 5550 e4b8 bbef bc8c e6b1  ......UP........
-00000b80: 9fe8 a5bf e59c a8e6 a0a1 e9ab 98e4 b8ad  ................
-00000b90: e794 9fe3 8082 0d0a 0d0a e8af b8e8 919b  ................
-00000ba0: e4ba aee4 b88e e585 abe5 8da6 e998 b520  ............... 
-00000bb0: 6267 4172 7261 79ef bc9a e688 91e7 9a84  bgArray.........
-00000bc0: e4b8 96e7 958c e59f bae5 b2a9 e789 88e7  ................
-00000bd0: 8ea9 e5ae b6ef bc8c e596 9ce6 aca2 e7bc  ................
-00000be0: 96e7 a88b e592 8ce9 9fb3 e4b9 90ef bc8c  ................
-00000bf0: e6b7 b1e5 9cb3 e588 9de4 ba8c e5ad a6e7  ................
-00000c00: 949f e380 820d 0a0d 0a23 2320 e887 b4e8  .........## ....
-00000c10: b0a2 f09f 998f 0d0a e69c ace8 87b4 e8b0  ................
-00000c20: a2e5 8897 e8a1 a8e6 8e92 e590 8de6 97a0  ................
-00000c30: e9a1 bae5 ba8f e380 820d 0a0d 0a2d 20e6  .............- .
-00000c40: 849f e8b0 a220 2a2a e698 80e6 a2a6 2a2a  ..... **......**
-00000c50: 5c3c 5151 3135 3135 3339 3938 3835 5c3e  \<QQ1515399885\>
-00000c60: 20e6 89be e587 bae6 8c87 e4bb a4e7 949f   ...............
-00000c70: e688 90e9 9499 e8af af62 7567 e5b9 b6e6  .........bug....
-00000c80: 8c87 e6ad a30d 0a2d 20e6 849f e8b0 a2e7  .......- .......
-00000c90: 94b1 202a 2a43 6861 726c 6965 5f50 696e  .. **Charlie_Pin
-00000ca0: 6720 e280 9ce6 9fa5 e790 86e5 b9b3 e280  g ..............
-00000cb0: 9d2a 2a20 e5b8 a6e6 9da5 e79a 8442 4458  .** .........BDX
-00000cc0: e696 87e4 bbb6 e8bd ace6 8da2 e58f 82e8  ................
-00000cd0: 8083 efbc 8ce4 bba5 e58f 8a4d 4944 492d  ...........MIDI-
-00000ce0: e688 91e7 9a84 e4b8 96e7 958c e5af b9e5  ................
-00000cf0: ba94 e4b9 90e5 99a8 e58f 82e8 8083 e8a1  ................
-00000d00: a8e6 a0bc 0d0a 2d20 e684 9fe8 b0a2 e794  ......- ........
-00000d10: b120 2a2a 5b43 4d41 5f32 3430 3150 545d  . **[CMA_2401PT]
-00000d20: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000d30: 636f 6d2f 434d 4132 3430 3150 5429 2a2a  com/CMA2401PT)**
-00000d40: 20e4 b8ba e688 91e4 bbac e79a 84e8 bdaf   ...............
-00000d50: e4bb b6e5 bc80 e58f 91e7 9a84 e4b8 80e4  ................
-00000d60: ba9b e696 b9e9 9da2 e8bf 9be8 a18c e68c  ................
-00000d70: 87e5 afbc efbc 8ce5 908c e697 b6e6 8891  ................
-00000d80: e4bb ace5 8f82 e880 83e4 ba86 e4bb 96e7  ................
-00000d90: 9a84 4244 5877 6f72 6b73 686f 70e4 bd9c  ..BDXworkshop...
-00000da0: e4b8 ba42 4458 e7bb 93e6 9e84 e7bc 96e8  ...BDX..........
-00000db0: be91 e79a 84e5 8f82 e880 830d 0a2d 20e6  .............- .
-00000dc0: 849f e8b0 a2e7 94b1 202a 2a5b 4469 736c  ........ **[Disl
-00000dd0: 696e 6b20 5366 6f72 7a61 5d28 6874 7470  ink Sforza](http
-00000de0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f44  s://github.com/D
-00000df0: 6973 6c69 6e6b 2920 e280 9ce6 96ad e881  islink) ........
-00000e00: 94c2 b7e6 96af e7a6 8fe5 b094 e689 8ee2  ................
-00000e10: 809d 2a2a 5c3c 5151 3136 3030 3531 3533  ..**\<QQ16005153
-00000e20: 3134 5c3e 20e5 b8a6 e69d a5e7 9a84 6d69  14\> .........mi
-00000e30: 6469 e99f b3e8 89b2 e8a7 a3e6 9e90 e4bb  di..............
-00000e40: a5e5 8f8a e8bd ace6 8da2 e68c 87e4 bba4  ................
-00000e50: e79a 84e7 ae97 e6b3 95ef bc8c e688 91e4  ................
-00000e60: bbac e5b0 86e5 85b6 e694 b9e7 bc96 e5b9  ................
-00000e70: b6e5 ba94 e794 a8ef bc9b e590 8ce6 97b6  ................
-00000e80: efbc 8ce6 849f e8b0 a2e4 bb96 e79a 845b  ...............[
-00000e90: e7bd 91e9 a1b5 e789 88e8 bdac e68d a2e5  ................
-00000ea0: 99a8 5d28 6874 7470 733a 2f2f 6469 736c  ..](https://disl
-00000eb0: 696e 6b2e 6769 7468 7562 2e69 6f2f 6d69  ink.github.io/mi
-00000ec0: 6469 3262 6478 2f29 e7bb 99e6 8891 e4bb  di2bdx/)........
-00000ed0: ace7 9a84 e5bc 80e5 8f91 e4b8 8ee6 9bb4  ................
-00000ee0: e696 b0e5 b8a6 e69d a5e5 b7a8 e5a4 a7e7  ................
-00000ef0: 9a84 e58e 8be5 8a9b e592 8ce5 8aa8 e58a  ................
-00000f00: 9bef bc8c e8ae a9e6 8891 e4bb ace5 9ca8  ................
-00000f10: e58e 9fe6 9cac e4b8 80e9 aa91 e7bb 9de5  ................
-00000f20: b098 e79a 84e6 91b8 e9b1 bce9 8193 e8b7  ................
-00000f30: afe4 b88a e8bd ace5 9091 e5bc 80e5 8f91  ................
-00000f40: efbc 8ce5 b88c e69c 9be4 bb96 e883 bde8  ................
-00000f50: 8083 e4b8 8ae4 b880 e4b8 aae7 9086 e683  ................
-00000f60: b3e7 9a84 e5a4 a7e5 ada6 efbc 810d 0a2d  ...............-
-00000f70: 20e6 849f e8b0 a220 2a2a 546f 7563 6820   ...... **Touch 
-00000f80: e280 9ce5 81b7 e590 83e2 809d 2a2a 5c3c  ............**\<
-00000f90: 5151 3137 3933 3533 3731 3634 5c3e 20e6  QQ1793537164\> .
-00000fa0: 8f90 e4be 9be7 9a84 4244 58e5 afbc e585  ........BDX.....
-00000fb0: a5e6 b58b e8af 95e6 94af e68c 81ef bc8c  ................
-00000fc0: e5b9 b6e5 afb9 e7a8 8be5 ba8f e79a 84e6  ................
-00000fd0: 94b9 e8bf 9be6 8f90 e4be 9be4 ba86 e4b8  ................
-00000fe0: b0e5 af8c e79a 84e6 848f e8a7 81ef bc9b  ................
-00000ff0: e590 8ce6 97b6 e4b9 9fe6 849f e8b0 a2e4  ................
-00001000: bb96 e79a 84e4 b88d e696 ade5 b09d e8af  ................
-00001010: 95e6 96b0 e79a 84e5 8685 e5ae b9ef bc8c  ................
-00001020: e4bd bfe6 8891 e4bb ace7 9a84 e68e 92e9  ................
-00001030: 9499 e69b b4e8 bf9b e4b8 80e6 ada5 0d0a  ................
-00001040: 2d20 e684 9fe8 b0a2 202a 2a4d 6f6e 6f2a  - ...... **Mono*
-00001050: 2a5c 3c51 5137 3338 3839 3330 3837 5c3e  *\<QQ738893087\>
-00001060: 20e5 8f8d e9a6 88e5 ae89 e8a3 85e6 97b6   ...............
-00001070: e79a 84e9 97ae e9a2 98ef bc8c e8be 85e5  ................
-00001080: 8aa9 e688 91e4 bbac e689 bee5 88b0 e4ba  ................
-00001090: 86e8 a786 e7aa 97e6 938d e4bd 9ce7 b3bb  ................
-000010a0: e7bb 9fe4 b88b e79a 84e5 85bc e5ae b9e6  ................
-000010b0: 80a7 e997 aee9 a298 0d0a 2d20 e684 9fe8  ..........- ....
-000010c0: b0a2 202a 2a41 6d6d 656c 6961 20e2 809c  .. **Ammelia ...
-000010d0: e889 bee7 b1b3 e588 a9e4 ba9a e280 9d2a  ...............*
-000010e0: 2a5c 3c51 5132 3833 3833 3334 3633 375c  *\<QQ2838334637\
-000010f0: 3e20 e695 a6e4 bf83 e688 91e4 bbac e8bf  > ..............
-00001100: 9be8 a18c e696 b0e7 9a84 e58a 9fe8 83bd  ................
-00001110: e5bc 80e5 8f91 efbc 8ce5 b9b6 e4b8 bae6  ................
-00001120: 96b0 e58a 9fe8 83bd e68f 90e5 87ba e4ba  ................
-00001130: 86e9 9d9e e5b8 b8e4 bc98 e7a7 80e7 9a84  ................
-00001140: e5a4 a7e9 878f e5bb bae8 aeae efbc 8ce4  ................
-00001150: bba5 e58f 8ae6 8f90 e4be 9be7 9a84 4244  ..............BD
-00001160: 58e5 afbc e585 a5e6 b58b e8af 95e6 94af  X...............
-00001170: e68c 81ef bc8c e4b8 bae6 8891 e4bb ace7  ................
-00001180: 9a84 e696 b0e7 bb93 e69e 84e7 949f e688  ................
-00001190: 90e7 ae97 e6b3 95e6 8f90 e4be 9be4 ba86  ................
-000011a0: e5a4 a7e9 878f e79a 84e5 ae9e e999 85e7  ................
-000011b0: 9086 e8ae bae6 94af e68c 810d 0a2d 20e6  .............- .
-000011c0: 849f e8b0 a220 2a2a 5be7 a59e e7be bd5d  ..... **[......]
-000011d0: 2868 7474 7073 3a2f 2f67 6974 6565 2e63  (https://gitee.c
-000011e0: 6f6d 2f73 6e6f 7779 6b61 6d69 2920 e280  om/snowykami) ..
-000011f0: 9c5b 536e 6f77 794b 616d 695d 2868 7474  .[SnowyKami](htt
-00001200: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001210: 736e 6f77 7966 6972 6566 6c79 29e2 809d  snowyfirefly)...
-00001220: 2a2a 20e5 afb9 e688 91e4 bbac e9a1 b9e7  ** .............
-00001230: 9bae e79a 84e6 94af e68c 81e4 b88e e5ae  ................
-00001240: a3e4 bca0 efbc 8ce5 b88c e69c 9be4 bb96  ................
-00001250: e883 bde8 8083 e79a 84e4 b880 e689 80e4  ................
-00001260: bc98 e7a7 80e7 9a84 e5a4 a7e5 ada6 efbc  ................
-00001270: 810d 0a2d 20e6 849f e8b0 a220 2a2a e68c  ...- ...... **..
-00001280: 87e4 bba4 e5b8 885f e88b a6e5 8a9b e680  ......._........
-00001290: 9520 706c 6179 6a75 6963 6531 3233 2a2a  . playjuice123**
-000012a0: 5c3c 5151 3234 3036 3637 3139 375c 3ee4  \<QQ240667197\>.
-000012b0: b8ba e688 91e4 bbac e79a 84e7 a88b e5ba  ................
-000012c0: 8fe6 89be e587 bae9 9499 e8af afef bc8c  ................
-000012d0: e5b9 b6e6 8f90 e986 92e6 8891 e4bb ace4  ................
-000012e0: bfae e5a4 8de4 b880 e4b8 aae4 b880 e79b  ................
-000012f0: b4e5 ad98 e59c a8e7 9a84 e5a4 a762 7567  .............bug
-00001300: e380 820d 0a2d 20e6 849f e8b0 a220 2a2a  .....- ...... **
-00001310: e99b b7e9 9c86 2a2a 5c3c 5151 3335 3535  ......**\<QQ3555
-00001320: 3236 3835 3139 5c3e e4b8 bae6 8891 e4bb  268519\>........
-00001330: ace7 9a84 e7a8 8be5 ba8f e689 bee5 87ba  ................
-00001340: e994 99e8 afaf efbc 8ce5 b9b6 e68f 90e9  ................
-00001350: 8692 e4bf aee5 a48d 6275 67e3 8082 0d0a  ........bug.....
-00001360: 0d0a 3e09 e684 9fe8 b0a2 e5b9 bfe5 a4a7  ..>.............
-00001370: e7be a4e5 8f8b e4b8 bae6 ada4 e7a8 8be5  ................
-00001380: ba8f e68f 90e4 be9b e79a 84e6 b58b e8af  ................
-00001390: 95e7 ad89 e694 afe6 8c81 0d0a 3e0d 0a3e  ............>..>
-000013a0: 09e8 8ba5 e682 a8e5 afb9 e688 91e4 bbac  ................
-000013b0: e69c 89e6 8980 e8b4 a1e7 8cae e4bd 86e6  ................
-000013c0: 82a8 e79a 84e5 908d e5ad 97e6 b2a1 e69c  ................
-000013d0: 89e6 98be e7a4 bae5 9ca8 e6ad a4e5 8897  ................
-000013e0: e8a1 a8e4 b8ad efbc 8ce8 afb7 e881 94e7  ................
-000013f0: b3bb e688 91e4 bbac efbc 810d 0a0d 0a23  ...............#
-00001400: 2320 e881 94e7 b3bb f09f 939e 0d0a 0d0a  # ..............
-00001410: e88b a5e9 8187 e588 b0e5 ba93 e4b8 ade7  ................
-00001420: 9a84 e997 aee9 a298 efbc 8ce6 aca2 e8bf  ................
-00001430: 8ee5 9ca8 5be6 ada4 5d28 6874 7470 733a  ....[...](https:
-00001440: 2f2f 6769 7465 652e 636f 6d2f 5472 694d  //gitee.com/TriM
-00001450: 2d4f 7267 616e 697a 6174 696f 6e2f 4d75  -Organization/Mu
-00001460: 7369 6372 6561 7465 722f 6973 7375 6573  sicreater/issues
-00001470: 2f6e 6577 29e6 8f90 e587 bae4 bda0 e79a  /new)...........
-00001480: 8469 7373 7565 e380 820d 0a0d 0ae5 a682  .issue..........
-00001490: e69e 9ce9 9c80 e8a6 81e4 b88e e5bc 80e5  ................
-000014a0: 8f91 e7bb 84e8 bf9b e8a1 8ce4 baa4 e6b5  ................
-000014b0: 81ef bc8c e6ac a2e8 bf8e e58a a0e5 85a5  ................
-000014c0: e688 91e4 bbac e79a 845b e5bc 80e5 8f91  .........[......
-000014d0: e997 b2e8 818a 51e7 bea4 5d28 6874 7470  ......Q...](http
-000014e0: 733a 2f2f 6a71 2e71 712e 636f 6d2f 3f5f  s://jq.qq.com/?_
-000014f0: 7776 3d31 3032 3726 6b3d 6870 6552 7872  wv=1027&k=hpeRxr
-00001500: 5972 29e3 8082 0d0a 0d0a 2d2d 2d2d 2d2d  Yr).......------
-00001510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001530: 2d2d 2d2d 2d2d 0d0a 0d0a 4e4f 5420 414e  ------....NOT AN
-00001540: 204f 4646 4943 4941 4c20 4d49 4e45 4352   OFFICIAL MINECR
-00001550: 4146 5420 5052 4f44 5543 542e 0d0a 0d0a  AFT PRODUCT.....
-00001560: 4e4f 5420 4150 5052 4f56 4544 2042 5920  NOT APPROVED BY 
-00001570: 4f52 2041 5353 4f43 4941 5445 4420 5749  OR ASSOCIATED WI
-00001580: 5448 204d 4f4a 414e 4720 4f52 204d 4943  TH MOJANG OR MIC
-00001590: 524f 534f 4654 2e0d 0a0d 0ae6 ada4 e9a1  ROSOFT..........
-000015a0: b9e7 9bae e5b9 b6e9 9d9e e4b8 80e4 b8aa  ................
-000015b0: e5ae 98e6 96b9 20e3 808a e688 91e7 9a84  ...... .........
-000015c0: e4b8 96e7 958c e380 8bef bc88 2a4d 696e  ............*Min
-000015d0: 6563 7261 6674 2aef bc89 e9a1 b9e7 9bae  ecraft*.........
-000015e0: 0d0a 0d0a e6ad a4e9 a1b9 e79b aee4 b88d  ................
-000015f0: e99a b6e5 b19e e688 96e5 85b3 e881 94e4  ................
-00001600: ba8e 204d 6f6a 616e 6720 5374 7564 696f  .. Mojang Studio
-00001610: 7320 e688 9620 e5be aee8 bdaf 0d0a 0d0a  s ... ..........
-00001620: 0d0a 0d0a 0d0a 0d0a 5b42 696c 6962 696c  ........[Bilibil
-00001630: 693a 20e5 878c e4ba 91e9 8791 e7be bf5d  i: ............]
-00001640: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00001650: 6965 6c64 732e 696f 2f62 6164 6765 2f42  ields.io/badge/B
-00001660: 696c 6962 696c 692d 2545 3525 3837 2538  ilibili-%E5%87%8
-00001670: 4325 4534 2542 4125 3931 2545 3925 3837  C%E4%BA%91%E9%87
-00001680: 2539 3125 4537 2542 4525 4246 2d30 3041  %91%E7%BE%BF-00A
-00001690: 3145 373f 7374 796c 653d 666f 722d 7468  1E7?style=for-th
-000016a0: 652d 6261 6467 650d 0a5b 4269 6c69 6269  e-badge..[Bilibi
-000016b0: 6c69 3a20 e8af b8e8 919b e4ba aee4 b88e  li: ............
-000016c0: e585 abe5 8da6 e998 b55d 3a20 6874 7470  .........]: http
-000016d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000016e0: 696f 2f62 6164 6765 2f42 696c 6962 696c  io/badge/Bilibil
-000016f0: 692d 2545 3825 4146 2542 3825 4538 2539  i-%E8%AF%B8%E8%9
-00001700: 3125 3942 2545 3425 4241 2541 4525 4534  1%9B%E4%BA%AE%E4
-00001710: 2542 3825 3845 2545 3525 3835 2541 4225  %B8%8E%E5%85%AB%
-00001720: 4535 2538 4425 4136 2545 3925 3938 2542  E5%8D%A6%E9%98%B
-00001730: 352d 3030 4131 4537 3f73 7479 6c65 3d66  5-00A1E7?style=f
-00001740: 6f72 2d74 6865 2d62 6164 6765 0d0a 5b43  or-the-badge..[C
-00001750: 6f64 6553 7479 6c65 3a20 626c 6163 6b5d  odeStyle: black]
-00001760: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00001770: 6965 6c64 732e 696f 2f62 6164 6765 2f63  ields.io/badge/c
-00001780: 6f64 6525 3230 7374 796c 652d 626c 6163  ode%20style-blac
-00001790: 6b2d 3132 3131 3130 2e73 7667 3f73 7479  k-121110.svg?sty
-000017a0: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
-000017b0: 0d0a 5b70 7974 686f 6e5d 3a20 6874 7470  ..[python]: http
-000017c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000017d0: 696f 2f62 6164 6765 2f70 7974 686f 6e2d  io/badge/python-
-000017e0: 332e 362d 4142 3730 4646 3f73 7479 6c65  3.6-AB70FF?style
-000017f0: 3d66 6f72 2d74 6865 2d62 6164 6765 0d0a  =for-the-badge..
-00001800: 5b72 656c 6561 7365 5d3a 2068 7474 7073  [release]: https
-00001810: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00001820: 6f2f 6769 7468 7562 2f76 2f72 656c 6561  o/github/v/relea
-00001830: 7365 2f45 696c 6c65 7357 616e 2f4d 7573  se/EillesWan/Mus
-00001840: 6963 7265 6174 6572 3f73 7479 6c65 3d66  icreater?style=f
-00001850: 6f72 2d74 6865 2d62 6164 6765 0d0a 5b6c  or-the-badge..[l
-00001860: 6963 656e 7365 5d3a 2068 7474 7073 3a2f  icense]: https:/
-00001870: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00001880: 6261 6467 652f 4c69 6365 6e63 652d 4170  badge/Licence-Ap
-00001890: 6163 6865 2d32 3238 4232 323f 7374 796c  ache-228B22?styl
-000018a0: 653d 666f 722d 7468 652d 6261 6467 650d  e=for-the-badge.
-000018b0: 0a                                       .
+000003b0: 2e6d 640d 0a0d 0a0d 0a3c 6831 2061 6c69  .md......<h1 ali
+000003c0: 676e 3d22 6365 6e74 6572 223e 0d0a 2020  gn="center">..  
+000003d0: 2020 e99f b3c2 b7e5 889b 204d 7573 6963    ........ Music
+000003e0: 7265 6174 6572 0d0a 3c2f 6831 3e0d 0a0d  reater..</h1>...
+000003f0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000400: 7222 3e0d 0a20 2020 203c 696d 6720 7769  r">..    <img wi
+00000410: 6474 683d 2231 3238 2220 6865 6967 6874  dth="128" height
+00000420: 3d22 3132 3822 2073 7263 3d22 6874 7470  ="128" src="http
+00000430: 733a 2f2f 6769 7465 652e 636f 6d2f 5472  s://gitee.com/Tr
+00000440: 694d 2d4f 7267 616e 697a 6174 696f 6e2f  iM-Organization/
+00000450: 4d75 7369 6372 6561 7465 722f 7261 772f  Musicreater/raw/
+00000460: 6d61 7374 6572 2f72 6573 6f75 7263 6573  master/resources
+00000470: 2f6d 7363 7449 636f 6e2e 6963 6f22 3e0d  /msctIcon.ico">.
+00000480: 0a20 2020 203c 2f69 6d67 3e0d 0a3c 2f70  .    </img>..</p
+00000490: 3e0d 0a0d 0a3c 6833 2061 6c69 676e 3d22  >....<h3 align="
+000004a0: 6365 6e74 6572 223e e4b8 80e6 acbe e585  center">........
+000004b0: 8de8 b4b9 e5bc 80e6 ba90 e79a 8420 e380  ............. ..
+000004c0: 8ae6 8891 e79a 84e4 b896 e795 8ce3 808b  ................
+000004d0: 204d 4944 49e9 9fb3 e4b9 90e8 bdac e68d   MIDI...........
+000004e0: a2e5 ba93 e380 823c 2f68 333e 0d0a 0d0a  .......</h3>....
+000004f0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000500: 223e 0d0a 2020 2020 3c69 6d67 2073 7263  ">..    <img src
+00000510: 3d22 6874 7470 733a 2f2f 666f 7274 6865  ="https://forthe
+00000520: 6261 6467 652e 636f 6d2f 696d 6167 6573  badge.com/images
+00000530: 2f62 6164 6765 732f 6275 696c 742d 7769  /badges/built-wi
+00000540: 7468 2d6c 6f76 652e 7376 6722 3e0d 0a20  th-love.svg">.. 
+00000550: 2020 203c 6120 6872 6566 3d27 6874 7470     <a href='http
+00000560: 733a 2f2f 6769 7465 652e 636f 6d2f 5472  s://gitee.com/Tr
+00000570: 694d 2d4f 7267 616e 697a 6174 696f 6e2f  iM-Organization/
+00000580: 4d75 7369 6372 6561 7465 7227 3e0d 0a20  Musicreater'>.. 
+00000590: 2020 2020 2020 203c 696d 6720 616c 6967         <img alig
+000005a0: 6e3d 2272 6967 6874 2220 7372 633d 2768  n="right" src='h
+000005b0: 7474 7073 3a2f 2f67 6974 6565 2e63 6f6d  ttps://gitee.com
+000005c0: 2f54 7269 4d2d 4f72 6761 6e69 7a61 7469  /TriM-Organizati
+000005d0: 6f6e 2f4d 7573 6963 7265 6174 6572 2f77  on/Musicreater/w
+000005e0: 6964 6765 7473 2f77 6964 6765 745f 312e  idgets/widget_1.
+000005f0: 7376 6727 2061 6c74 3d27 466f 726b 206d  svg' alt='Fork m
+00000600: 6520 6f6e 2047 6974 6565 273e 0d0a 2020  e on Gitee'>..  
+00000610: 2020 2020 2020 3c2f 696d 673e 0d0a 2020        </img>..  
+00000620: 2020 3c2f 613e 0d0a 3c70 3e0d 0a0d 0a0d    </a>..<p>.....
+00000630: 0a0d 0a0d 0a0d 0a5b 215b 5d5b 4269 6c69  .......[![][Bili
+00000640: 6269 6c69 3a20 e987 91e7 bebf 454c 535d  bili: ......ELS]
+00000650: 5d28 6874 7470 733a 2f2f 7370 6163 652e  ](https://space.
+00000660: 6269 6c69 6269 6c69 2e63 6f6d 2f33 3937  bilibili.com/397
+00000670: 3336 3930 3032 2f29 0d0a 5b21 5b5d 5b42  369002/)..[![][B
+00000680: 696c 6962 696c 693a 20e8 afb8 e891 9be4  ilibili: .......
+00000690: baae e4b8 8ee5 85ab e58d a6e9 98b5 5d5d  ..............]]
+000006a0: 2868 7474 7073 3a2f 2f73 7061 6365 2e62  (https://space.b
+000006b0: 696c 6962 696c 692e 636f 6d2f 3630 3430  ilibili.com/6040
+000006c0: 3732 3437 3429 200d 0a5b 215b 436f 6465  72474) ..[![Code
+000006d0: 5374 796c 653a 2062 6c61 636b 5d5d 2868  Style: black]](h
+000006e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000006f0: 6d2f 7073 662f 626c 6163 6b29 0d0a 5b21  m/psf/black)..[!
+00000700: 5b5d 5b70 7974 686f 6e5d 5d28 6874 7470  [][python]](http
+00000710: 733a 2f2f 7777 772e 7079 7468 6f6e 2e6f  s://www.python.o
+00000720: 7267 2f29 0d0a 5b21 5b5d 5b6c 6963 656e  rg/)..[![][licen
+00000730: 7365 5d5d 284c 4943 454e 5345 290d 0a5b  se]](LICENSE)..[
+00000740: 215b 5d5b 7265 6c65 6173 655d 5d28 2e2e  ![][release]](..
+00000750: 2f2e 2e2f 7265 6c65 6173 6573 290d 0a0d  /../releases)...
+00000760: 0a5b 215b 4769 7465 6553 7461 725d 2868  .[![GiteeStar](h
+00000770: 7474 7073 3a2f 2f67 6974 6565 2e63 6f6d  ttps://gitee.com
+00000780: 2f54 7269 4d2d 4f72 6761 6e69 7a61 7469  /TriM-Organizati
+00000790: 6f6e 2f4d 7573 6963 7265 6174 6572 2f62  on/Musicreater/b
+000007a0: 6164 6765 2f73 7461 722e 7376 673f 7468  adge/star.svg?th
+000007b0: 656d 653d 6772 6179 295d 2868 7474 7073  eme=gray)](https
+000007c0: 3a2f 2f67 6974 6565 2e63 6f6d 2f54 7269  ://gitee.com/Tri
+000007d0: 4d2d 4f72 6761 6e69 7a61 7469 6f6e 2f4d  M-Organization/M
+000007e0: 7573 6963 7265 6174 6572 2f73 7461 7267  usicreater/starg
+000007f0: 617a 6572 7329 0d0a 5b21 5b47 6974 6565  azers)..[![Gitee
+00000800: 466f 726b 5d28 6874 7470 733a 2f2f 6769  Fork](https://gi
+00000810: 7465 652e 636f 6d2f 5472 694d 2d4f 7267  tee.com/TriM-Org
+00000820: 616e 697a 6174 696f 6e2f 4d75 7369 6372  anization/Musicr
+00000830: 6561 7465 722f 6261 6467 652f 666f 726b  eater/badge/fork
+00000840: 2e73 7667 3f74 6865 6d65 3d67 7261 7929  .svg?theme=gray)
+00000850: 5d28 6874 7470 733a 2f2f 6769 7465 652e  ](https://gitee.
+00000860: 636f 6d2f 5472 694d 2d4f 7267 616e 697a  com/TriM-Organiz
+00000870: 6174 696f 6e2f 4d75 7369 6372 6561 7465  ation/Musicreate
+00000880: 722f 6d65 6d62 6572 7329 0d0a 5b21 5b47  r/members)..[![G
+00000890: 6974 4875 6220 5265 706f 2073 7461 7273  itHub Repo stars
+000008a0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+000008b0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+000008c0: 7374 6172 732f 5472 694d 2d4f 7267 616e  stars/TriM-Organ
+000008d0: 697a 6174 696f 6e2f 4d75 7369 6372 6561  ization/Musicrea
+000008e0: 7465 723f 636f 6c6f 723d 7768 6974 6526  ter?color=white&
+000008f0: 6c6f 676f 3d47 6974 4875 6226 7374 796c  logo=GitHub&styl
+00000900: 653d 706c 6173 7469 6329 5d28 6874 7470  e=plastic)](http
+00000910: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
+00000920: 7269 4d2d 4f72 6761 6e69 7a61 7469 6f6e  riM-Organization
+00000930: 2f4d 7573 6963 7265 6174 6572 2f73 7461  /Musicreater/sta
+00000940: 7267 617a 6572 7329 0d0a 5b21 5b47 6974  rgazers)..[![Git
+00000950: 4875 6220 5265 706f 2046 6f72 6b73 5d28  Hub Repo Forks](
+00000960: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000970: 6c64 732e 696f 2f67 6974 6875 622f 666f  lds.io/github/fo
+00000980: 726b 732f 5472 694d 2d4f 7267 616e 697a  rks/TriM-Organiz
+00000990: 6174 696f 6e2f 4d75 7369 6372 6561 7465  ation/Musicreate
+000009a0: 723f 636f 6c6f 723d 7768 6974 6526 6c6f  r?color=white&lo
+000009b0: 676f 3d47 6974 4875 6226 7374 796c 653d  go=GitHub&style=
+000009c0: 706c 6173 7469 6329 5d28 6874 7470 733a  plastic)](https:
+000009d0: 2f2f 6769 7468 7562 2e63 6f6d 2f54 7269  //github.com/Tri
+000009e0: 4d2d 4f72 6761 6e69 7a61 7469 6f6e 2f4d  M-Organization/M
+000009f0: 7573 6963 7265 6174 6572 2f66 6f72 6b73  usicreater/forks
+00000a00: 290d 0a0d 0a0d 0ae7 ae80 e4bd 93e4 b8ad  )...............
+00000a10: e696 87f0 9f87 a8f0 9f87 b320 7c20 5b45  ........... | [E
+00000a20: 6e67 6c69 7368 f09f 87ac f09f 87a7 5d28  nglish........](
+00000a30: 5245 4144 4d45 5f45 4e2e 6d64 290d 0a0d  README_EN.md)...
+00000a40: 0a0d 0a23 2320 e4bb 8be7 bb8d f09f 9a80  ...## ..........
+00000a50: 0d0a 0d0a e99f b3c2 b7e5 889b 20e6 98af  ............ ...
+00000a60: e4b8 80e4 b8aa e585 8de8 b4b9 e5bc 80e6  ................
+00000a70: ba90 e79a 84e9 9288 e5af b920 2a2a e380  ........... **..
+00000a80: 8ae6 8891 e79a 84e4 b896 e795 8ce3 808b  ................
+00000a90: 2a2a 20e7 9a84 4d49 4449 e99f b3e4 b990  ** ...MIDI......
+00000aa0: e8bd ace6 8da2 e5ba 930d 0a0d 0ae6 aca2  ................
+00000ab0: e8bf 8ee5 8aa0 e7be a4ef bc9a 5b38 3631  ............[861
+00000ac0: 3638 3438 3539 5d28 6874 7470 733a 2f2f  684859](https://
+00000ad0: 6a71 2e71 712e 636f 6d2f 3f5f 7776 3d31  jq.qq.com/?_wv=1
+00000ae0: 3032 3726 6b3d 6870 6552 7872 5972 290d  027&k=hpeRxrYr).
+00000af0: 0a0d 0a23 2320 e4b8 8be8 bdbd e5ae 89e8  ...## ..........
+00000b00: a385 0d0a 0d0a 2d20 e4bd bfe7 94a8 7079  ......- ......py
+00000b10: 7069 0d0a 2020 2020 6060 6062 6173 680d  pi..    ```bash.
+00000b20: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+00000b30: 204d 7573 6963 7265 6174 6572 0d0a 2020   Musicreater..  
+00000b40: 2020 6060 600d 0a0d 0a2d 20e5 a682 e69e    ```....- .....
+00000b50: 9ce5 87ba e78e b0e9 9499 e8af afef bc8c  ................
+00000b60: e58f afe4 bba5 e5b0 9de8 af95 efbc 9a0d  ................
+00000b70: 0a20 2020 2060 6060 6261 7368 0d0a 2020  .    ```bash..  
+00000b80: 2020 7069 7020 696e 7374 616c 6c20 2d69    pip install -i
+00000b90: 2068 7474 7073 3a2f 2f70 7970 692e 7079   https://pypi.py
+00000ba0: 7468 6f6e 2e6f 7267 2f73 696d 706c 6520  thon.org/simple 
+00000bb0: 4d75 7369 6372 6561 7465 720d 0a20 2020  Musicreater..   
+00000bc0: 2060 6060 0d0a 2d20 efbc 88e5 afb9 e4ba   ```..- ........
+00000bd0: 8ee5 bc80 e58f 91e8 8085 e69d a5e8 afb4  ................
+00000be0: efbc 89e5 8d87 e7ba a7ef bc9a 0d0a 2020  ..............  
+00000bf0: 2020 6060 6062 6173 680d 0a20 2020 2070    ```bash..    p
+00000c00: 6970 2069 6e73 7461 6c6c 202d 6920 6874  ip install -i ht
+00000c10: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
+00000c20: 6e2e 6f72 672f 7369 6d70 6c65 204d 7573  n.org/simple Mus
+00000c30: 6963 7265 6174 6572 202d 2d75 7067 7261  icreater --upgra
+00000c40: 6465 0d0a 2020 2020 6060 600d 0a0d 0a2d  de..    ```....-
+00000c50: 20e5 858b e99a 86e4 bb93 e5ba 93e5 b9b6   ...............
+00000c60: e5ae 89e8 a385 0d0a 2020 2020 6060 6062  ........    ```b
+00000c70: 6173 680d 0a20 2020 2067 6974 2063 6c6f  ash..    git clo
+00000c80: 6e65 2068 7474 7073 3a2f 2f67 6974 6565  ne https://gitee
+00000c90: 2e63 6f6d 2f54 7269 4d2d 4f72 6761 6e69  .com/TriM-Organi
+00000ca0: 7a61 7469 6f6e 2f4d 7573 6963 7265 6174  zation/Musicreat
+00000cb0: 6572 2e67 6974 0d0a 2020 2020 6364 204d  er.git..    cd M
+00000cc0: 7573 6963 7265 6174 6572 0d0a 2020 2020  usicreater..    
+00000cd0: 7079 7468 6f6e 2073 6574 7570 2e70 7920  python setup.py 
+00000ce0: 696e 7374 616c 6c0d 0a20 2020 2060 6060  install..    ```
+00000cf0: 0d0a 0d0a e4bb a5e4 b88a e591 bde4 bba4  ................
+00000d00: e7a7 8d20 6070 7974 686f 6e60 e380 8160  ... `python`...`
+00000d10: 7069 7060 20e8 afb7 e4be 9de7 85a7 e590  pip` ...........
+00000d20: 84e4 b8aa e78e afe5 a283 e4b8 8de5 908c  ................
+00000d30: e781 b5e6 b4bb e69b b4e6 8da2 efbc 8ce5  ................
+00000d40: 8faf e883 bde4 b8ba 6070 7974 686f 6e33  ........`python3
+00000d50: 60e6 8896 6070 6970 3360 e4b9 8be7 b1bb  `...`pip3`......
+00000d60: e380 820d 0a0d 0a23 2320 e696 87e6 a1a3  .......## ......
+00000d70: f09f 9384 0d0a 0d0a 5be7 949f e688 90e6  ........[.......
+00000d80: 9687 e4bb b6e7 9a84 e4bd bfe7 94a8 5d28  ..............](
+00000d90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000da0: 6f6d 2f54 7269 4d2d 4f72 6761 6e69 7a61  om/TriM-Organiza
+00000db0: 7469 6f6e 2f4d 7573 6963 7265 6174 6572  tion/Musicreater
+00000dc0: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
+00000dd0: 732f 2545 3725 3934 2539 4625 4536 2538  s/%E7%94%9F%E6%8
+00000de0: 3825 3930 2545 3625 3936 2538 3725 4534  8%90%E6%96%87%E4
+00000df0: 2542 4225 4236 2545 3725 3941 2538 3425  %BB%B6%E7%9A%84%
+00000e00: 4534 2542 4425 4246 2545 3725 3934 2541  E4%BD%BF%E7%94%A
+00000e10: 3825 4538 2541 4625 4234 2545 3625 3938  8%E8%AF%B4%E6%98
+00000e20: 2538 452e 6d64 290d 0a0d 0a5b e4bb 93e5  %8E.md)....[....
+00000e30: ba93 4150 49e6 9687 e6a1 a35d 2868 7474  ..API......](htt
+00000e40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000e50: 5472 694d 2d4f 7267 616e 697a 6174 696f  TriM-Organizatio
+00000e60: 6e2f 4d75 7369 6372 6561 7465 722f 626c  n/Musicreater/bl
+00000e70: 6f62 2f6d 6173 7465 722f 646f 6373 2f25  ob/master/docs/%
+00000e80: 4535 2542 4125 3933 2545 3725 3941 2538  E5%BA%93%E7%9A%8
+00000e90: 3425 4537 2539 3425 3946 2545 3625 3838  4%E7%94%9F%E6%88
+00000ea0: 2539 3025 4534 2542 3825 3845 2545 3525  %90%E4%B8%8E%E5%
+00000eb0: 3841 2539 4625 4538 2538 3325 4244 2545  8A%9F%E8%83%BD%E
+00000ec0: 3625 3936 2538 3725 4536 2541 3125 4133  6%96%87%E6%A1%A3
+00000ed0: 2e6d 6429 0d0a 0d0a 2323 20e4 bd9c e880  .md)....## .....
+00000ee0: 85e2 9c92 0d0a 0d0a e987 91e7 bebf 2045  .............. E
+00000ef0: 696c 6c65 73ef bc9a e688 91e7 9a84 e4b8  illes...........
+00000f00: 96e7 958c e59f bae5 b2a9 e789 88e6 8c87  ................
+00000f10: e4bb a4e5 b888 efbc 8ce4 b8aa e4ba bae5  ................
+00000f20: bc80 e58f 91e8 8085 efbc 8c42 e7ab 99e4  ...........B....
+00000f30: b88d e79f a5e5 908d 5550 e4b8 bbef bc8c  ........UP......
+00000f40: e6b1 9fe8 a5bf e59c a8e6 a0a1 e9ab 98e4  ................
+00000f50: b8ad e794 9fe3 8082 0d0a 0d0a e8af b8e8  ................
+00000f60: 919b e4ba aee4 b88e e585 abe5 8da6 e998  ................
+00000f70: b520 6267 4172 7261 79ef bc9a e688 91e7  . bgArray.......
+00000f80: 9a84 e4b8 96e7 958c e59f bae5 b2a9 e789  ................
+00000f90: 88e7 8ea9 e5ae b6ef bc8c e596 9ce6 aca2  ................
+00000fa0: e7bc 96e7 a88b e592 8ce9 9fb3 e4b9 90ef  ................
+00000fb0: bc8c e6b7 b1e5 9cb3 e588 9de4 ba8c e5ad  ................
+00000fc0: a6e7 949f e380 820d 0a0d 0a23 2320 e887  ...........## ..
+00000fd0: b4e8 b0a2 f09f 998f 0d0a e69c ace8 87b4  ................
+00000fe0: e8b0 a2e5 8897 e8a1 a8e6 8e92 e590 8de6  ................
+00000ff0: 97a0 e9a1 bae5 ba8f e380 820d 0a0d 0a2d  ...............-
+00001000: 20e6 849f e8b0 a220 2a2a e698 80e6 a2a6   ...... **......
+00001010: 2a2a 5c3c 5151 3135 3135 3339 3938 3835  **\<QQ1515399885
+00001020: 5c3e 20e6 89be e587 bae6 8c87 e4bb a4e7  \> .............
+00001030: 949f e688 90e9 9499 e8af af62 7567 e5b9  ...........bug..
+00001040: b6e6 8c87 e6ad a30d 0a2d 20e6 849f e8b0  .........- .....
+00001050: a2e7 94b1 202a 2a43 6861 726c 6965 5f50  .... **Charlie_P
+00001060: 696e 6720 e280 9ce6 9fa5 e790 86e5 b9b3  ing ............
+00001070: e280 9d2a 2a20 e5b8 a6e6 9da5 e79a 8442  ...** .........B
+00001080: 4458 e696 87e4 bbb6 e8bd ace6 8da2 e58f  DX..............
+00001090: 82e8 8083 efbc 8ce4 bba5 e58f 8a4d 4944  .............MID
+000010a0: 492d e688 91e7 9a84 e4b8 96e7 958c e5af  I-..............
+000010b0: b9e5 ba94 e4b9 90e5 99a8 e58f 82e8 8083  ................
+000010c0: e8a1 a8e6 a0bc 0d0a 2d20 e684 9fe8 b0a2  ........- ......
+000010d0: e794 b120 2a2a 5b43 4d41 5f32 3430 3150  ... **[CMA_2401P
+000010e0: 545d 2868 7474 7073 3a2f 2f67 6974 6875  T](https://githu
+000010f0: 622e 636f 6d2f 434d 4132 3430 3150 5429  b.com/CMA2401PT)
+00001100: 2a2a 20e4 b8ba e688 91e4 bbac e79a 84e8  ** .............
+00001110: bdaf e4bb b6e5 bc80 e58f 91e7 9a84 e4b8  ................
+00001120: 80e4 ba9b e696 b9e9 9da2 e8bf 9be8 a18c  ................
+00001130: e68c 87e5 afbc efbc 8ce5 908c e697 b6e6  ................
+00001140: 8891 e4bb ace5 8f82 e880 83e4 ba86 e4bb  ................
+00001150: 96e7 9a84 4244 5877 6f72 6b73 686f 70e4  ....BDXworkshop.
+00001160: bd9c e4b8 ba42 4458 e7bb 93e6 9e84 e7bc  .....BDX........
+00001170: 96e8 be91 e79a 84e5 8f82 e880 830d 0a2d  ...............-
+00001180: 20e6 849f e8b0 a2e7 94b1 202a 2a5b 4469   ......... **[Di
+00001190: 736c 696e 6b20 5366 6f72 7a61 5d28 6874  slink Sforza](ht
+000011a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000011b0: 2f44 6973 6c69 6e6b 2920 e280 9ce6 96ad  /Dislink) ......
+000011c0: e881 94c2 b7e6 96af e7a6 8fe5 b094 e689  ................
+000011d0: 8ee2 809d 2a2a 5c3c 5151 3136 3030 3531  ....**\<QQ160051
+000011e0: 3533 3134 5c3e 20e5 b8a6 e69d a5e7 9a84  5314\> .........
+000011f0: 6d69 6469 e99f b3e8 89b2 e8a7 a3e6 9e90  midi............
+00001200: e4bb a5e5 8f8a e8bd ace6 8da2 e68c 87e4  ................
+00001210: bba4 e79a 84e7 ae97 e6b3 95ef bc8c e688  ................
+00001220: 91e4 bbac e5b0 86e5 85b6 e694 b9e7 bc96  ................
+00001230: e5b9 b6e5 ba94 e794 a8ef bc9b e590 8ce6  ................
+00001240: 97b6 efbc 8ce6 849f e8b0 a2e4 bb96 e79a  ................
+00001250: 845b e7bd 91e9 a1b5 e789 88e8 bdac e68d  .[..............
+00001260: a2e5 99a8 5d28 6874 7470 733a 2f2f 6469  ....](https://di
+00001270: 736c 696e 6b2e 6769 7468 7562 2e69 6f2f  slink.github.io/
+00001280: 6d69 6469 3262 6478 2f29 e7bb 99e6 8891  midi2bdx/)......
+00001290: e4bb ace7 9a84 e5bc 80e5 8f91 e4b8 8ee6  ................
+000012a0: 9bb4 e696 b0e5 b8a6 e69d a5e5 b7a8 e5a4  ................
+000012b0: a7e7 9a84 e58e 8be5 8a9b e592 8ce5 8aa8  ................
+000012c0: e58a 9bef bc8c e8ae a9e6 8891 e4bb ace5  ................
+000012d0: 9ca8 e58e 9fe6 9cac e4b8 80e9 aa91 e7bb  ................
+000012e0: 9de5 b098 e79a 84e6 91b8 e9b1 bce9 8193  ................
+000012f0: e8b7 afe4 b88a e8bd ace5 9091 e5bc 80e5  ................
+00001300: 8f91 efbc 8ce5 b88c e69c 9be4 bb96 e883  ................
+00001310: bde8 8083 e4b8 8ae4 b880 e4b8 aae7 9086  ................
+00001320: e683 b3e7 9a84 e5a4 a7e5 ada6 efbc 810d  ................
+00001330: 0a2d 20e6 849f e8b0 a220 2a2a 546f 7563  .- ...... **Touc
+00001340: 6820 e280 9ce5 81b7 e590 83e2 809d 2a2a  h ............**
+00001350: 5c3c 5151 3137 3933 3533 3731 3634 5c3e  \<QQ1793537164\>
+00001360: 20e6 8f90 e4be 9be7 9a84 4244 58e5 afbc   .........BDX...
+00001370: e585 a5e6 b58b e8af 95e6 94af e68c 81ef  ................
+00001380: bc8c e5b9 b6e5 afb9 e7a8 8be5 ba8f e79a  ................
+00001390: 84e6 94b9 e8bf 9be6 8f90 e4be 9be4 ba86  ................
+000013a0: e4b8 b0e5 af8c e79a 84e6 848f e8a7 81ef  ................
+000013b0: bc9b e590 8ce6 97b6 e4b9 9fe6 849f e8b0  ................
+000013c0: a2e4 bb96 e79a 84e4 b88d e696 ade5 b09d  ................
+000013d0: e8af 95e6 96b0 e79a 84e5 8685 e5ae b9ef  ................
+000013e0: bc8c e4bd bfe6 8891 e4bb ace7 9a84 e68e  ................
+000013f0: 92e9 9499 e69b b4e8 bf9b e4b8 80e6 ada5  ................
+00001400: 0d0a 2d20 e684 9fe8 b0a2 202a 2a4d 6f6e  ..- ...... **Mon
+00001410: 6f2a 2a5c 3c51 5137 3338 3839 3330 3837  o**\<QQ738893087
+00001420: 5c3e 20e5 8f8d e9a6 88e5 ae89 e8a3 85e6  \> .............
+00001430: 97b6 e79a 84e9 97ae e9a2 98ef bc8c e8be  ................
+00001440: 85e5 8aa9 e688 91e4 bbac e689 bee5 88b0  ................
+00001450: e4ba 86e8 a786 e7aa 97e6 938d e4bd 9ce7  ................
+00001460: b3bb e7bb 9fe4 b88b e79a 84e5 85bc e5ae  ................
+00001470: b9e6 80a7 e997 aee9 a298 0d0a 2d20 e684  ............- ..
+00001480: 9fe8 b0a2 202a 2a41 6d6d 656c 6961 20e2  .... **Ammelia .
+00001490: 809c e889 bee7 b1b3 e588 a9e4 ba9a e280  ................
+000014a0: 9d2a 2a5c 3c51 5132 3833 3833 3334 3633  .**\<QQ283833463
+000014b0: 375c 3e20 e695 a6e4 bf83 e688 91e4 bbac  7\> ............
+000014c0: e8bf 9be8 a18c e696 b0e7 9a84 e58a 9fe8  ................
+000014d0: 83bd e5bc 80e5 8f91 efbc 8ce5 b9b6 e4b8  ................
+000014e0: bae6 96b0 e58a 9fe8 83bd e68f 90e5 87ba  ................
+000014f0: e4ba 86e9 9d9e e5b8 b8e4 bc98 e7a7 80e7  ................
+00001500: 9a84 e5a4 a7e9 878f e5bb bae8 aeae efbc  ................
+00001510: 8ce4 bba5 e58f 8ae6 8f90 e4be 9be7 9a84  ................
+00001520: 4244 58e5 afbc e585 a5e6 b58b e8af 95e6  BDX.............
+00001530: 94af e68c 81ef bc8c e4b8 bae6 8891 e4bb  ................
+00001540: ace7 9a84 e696 b0e7 bb93 e69e 84e7 949f  ................
+00001550: e688 90e7 ae97 e6b3 95e6 8f90 e4be 9be4  ................
+00001560: ba86 e5a4 a7e9 878f e79a 84e5 ae9e e999  ................
+00001570: 85e7 9086 e8ae bae6 94af e68c 810d 0a2d  ...............-
+00001580: 20e6 849f e8b0 a220 2a2a 5be7 a59e e7be   ...... **[.....
+00001590: bd5d 2868 7474 7073 3a2f 2f67 6974 6565  .](https://gitee
+000015a0: 2e63 6f6d 2f73 6e6f 7779 6b61 6d69 2920  .com/snowykami) 
+000015b0: e280 9c5b 536e 6f77 794b 616d 695d 2868  ...[SnowyKami](h
+000015c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000015d0: 6d2f 736e 6f77 7966 6972 6566 6c79 29e2  m/snowyfirefly).
+000015e0: 809d 2a2a 20e5 afb9 e688 91e4 bbac e9a1  ..** ...........
+000015f0: b9e7 9bae e79a 84e6 94af e68c 81e4 b88e  ................
+00001600: e5ae a3e4 bca0 efbc 8ce5 b88c e69c 9be4  ................
+00001610: bb96 e883 bde8 8083 e79a 84e4 b880 e689  ................
+00001620: 80e4 bc98 e7a7 80e7 9a84 e5a4 a7e5 ada6  ................
+00001630: efbc 810d 0a2d 20e6 849f e8b0 a220 2a2a  .....- ...... **
+00001640: e68c 87e4 bba4 e5b8 885f e88b a6e5 8a9b  ........._......
+00001650: e680 9520 706c 6179 6a75 6963 6531 3233  ... playjuice123
+00001660: 2a2a 5c3c 5151 3234 3036 3637 3139 375c  **\<QQ240667197\
+00001670: 3ee4 b8ba e688 91e4 bbac e79a 84e7 a88b  >...............
+00001680: e5ba 8fe6 89be e587 bae9 9499 e8af afef  ................
+00001690: bc8c e5b9 b6e6 8f90 e986 92e6 8891 e4bb  ................
+000016a0: ace4 bfae e5a4 8de4 b880 e4b8 aae4 b880  ................
+000016b0: e79b b4e5 ad98 e59c a8e7 9a84 e5a4 a762  ...............b
+000016c0: 7567 e380 820d 0a2d 20e6 849f e8b0 a220  ug.....- ...... 
+000016d0: 2a2a e99b b7e9 9c86 2a2a 5c3c 5151 3335  **......**\<QQ35
+000016e0: 3535 3236 3835 3139 5c3e e4b8 bae6 8891  55268519\>......
+000016f0: e4bb ace7 9a84 e7a8 8be5 ba8f e689 bee5  ................
+00001700: 87ba e994 99e8 afaf efbc 8ce5 b9b6 e68f  ................
+00001710: 90e9 8692 e4bf aee5 a48d 6275 67e3 8082  ..........bug...
+00001720: 0d0a 0d0a 3e09 e684 9fe8 b0a2 e5b9 bfe5  ....>...........
+00001730: a4a7 e7be a4e5 8f8b e4b8 bae6 ada4 e7a8  ................
+00001740: 8be5 ba8f e68f 90e4 be9b e79a 84e6 b58b  ................
+00001750: e8af 95e7 ad89 e694 afe6 8c81 0d0a 3e0d  ..............>.
+00001760: 0a3e 09e8 8ba5 e682 a8e5 afb9 e688 91e4  .>..............
+00001770: bbac e69c 89e6 8980 e8b4 a1e7 8cae e4bd  ................
+00001780: 86e6 82a8 e79a 84e5 908d e5ad 97e6 b2a1  ................
+00001790: e69c 89e6 98be e7a4 bae5 9ca8 e6ad a4e5  ................
+000017a0: 8897 e8a1 a8e4 b8ad efbc 8ce8 afb7 e881  ................
+000017b0: 94e7 b3bb e688 91e4 bbac efbc 810d 0a0d  ................
+000017c0: 0a23 2320 e881 94e7 b3bb f09f 939e 0d0a  .## ............
+000017d0: 0d0a e88b a5e9 8187 e588 b0e5 ba93 e4b8  ................
+000017e0: ade7 9a84 e997 aee9 a298 efbc 8ce6 aca2  ................
+000017f0: e8bf 8ee5 9ca8 5be6 ada4 5d28 6874 7470  ......[...](http
+00001800: 733a 2f2f 6769 7465 652e 636f 6d2f 5472  s://gitee.com/Tr
+00001810: 694d 2d4f 7267 616e 697a 6174 696f 6e2f  iM-Organization/
+00001820: 4d75 7369 6372 6561 7465 722f 6973 7375  Musicreater/issu
+00001830: 6573 2f6e 6577 29e6 8f90 e587 bae4 bda0  es/new).........
+00001840: e79a 8469 7373 7565 e380 820d 0a0d 0ae5  ...issue........
+00001850: a682 e69e 9ce9 9c80 e8a6 81e4 b88e e5bc  ................
+00001860: 80e5 8f91 e7bb 84e8 bf9b e8a1 8ce4 baa4  ................
+00001870: e6b5 81ef bc8c e6ac a2e8 bf8e e58a a0e5  ................
+00001880: 85a5 e688 91e4 bbac e79a 845b e5bc 80e5  ...........[....
+00001890: 8f91 e997 b2e8 818a 51e7 bea4 5d28 6874  ........Q...](ht
+000018a0: 7470 733a 2f2f 6a71 2e71 712e 636f 6d2f  tps://jq.qq.com/
+000018b0: 3f5f 7776 3d31 3032 3726 6b3d 6870 6552  ?_wv=1027&k=hpeR
+000018c0: 7872 5972 29e3 8082 0d0a 0d0a 2d2d 2d2d  xrYr).......----
+000018d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000018e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000018f0: 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a e6ad a4e9  --------........
+00001900: a1b9 e79b aee5 b9b6 e99d 9ee4 b880 e4b8  ................
+00001910: aae5 ae98 e696 b920 e380 8ae6 8891 e79a  ....... ........
+00001920: 84e4 b896 e795 8ce3 808b efbc 882a 4d69  .............*Mi
+00001930: 6e65 6372 6166 742a efbc 89e9 a1b9 e79b  necraft*........
+00001940: ae0d 0a0d 0ae6 ada4 e9a1 b9e7 9bae e4b8  ................
+00001950: 8de9 9ab6 e5b1 9ee6 8896 e585 b3e8 8194  ................
+00001960: e4ba 8e20 4d6f 6a61 6e67 2053 7475 6469  ... Mojang Studi
+00001970: 6f73 20e6 8896 20e5 beae e8bd af0d 0a0d  os ... .........
+00001980: 0ae6 ada4 e9a1 b9e7 9bae e4ba a6e4 b88d  ................
+00001990: e4b8 8e20 e7bd 91e6 9893 20e7 9bb8 e585  ... ...... .....
+000019a0: b30d 0a0d 0ae2 809c 4d69 6e65 6372 6166  ........Minecraf
+000019b0: 74e2 809d e698 af20 4d6f 6a61 6e67 2053  t...... Mojang S
+000019c0: 796e 6572 6769 6573 2041 4220 e79a 84e5  ynergies AB ....
+000019d0: 9586 e6a0 87ef bc8c e6ad a4e9 a1b9 e79b  ................
+000019e0: aee4 b8ad e689 80e6 9c89 e5af b9e4 ba8e  ................
+000019f0: e280 9ce6 8891 e79a 84e4 b896 e795 8ce2  ................
+00001a00: 809d e380 81e2 809c 4d69 6e65 6372 6166  ........Minecraf
+00001a10: 74e2 809d e7ad 89e7 9bb8 e585 b3e7 a7b0  t...............
+00001a20: e591 bce5 9d87 e4b8 bae5 bc95 e794 a8e6  ................
+00001a30: 80a7 e4bd bfe7 94a8 0d0a 0d0a 2a20 e4b8  ............* ..
+00001a40: 8ae6 9687 e68f 90e5 8f8a e79a 8420 e7bd  ............. ..
+00001a50: 91e6 9893 20e5 85ac e58f b8ef bc8c e68c  .... ...........
+00001a60: 87e4 bba3 e79a 84e6 98af e59c a8e4 b8ad  ................
+00001a70: e59b bde5 a4a7 e999 86e8 bf90 e890 a5e3  ................
+00001a80: 808a e688 91e7 9a84 e4b8 96e7 958c efbc  ................
+00001a90: 9ae4 b8ad e59b bde7 8988 e380 8be7 9a84  ................
+00001aa0: e4b8 8ae6 b5b7 e7bd 91e4 b98b e698 93e7  ................
+00001ab0: bd91 e7bb 9ce7 a791 e68a 80e5 8f91 e5b1  ................
+00001ac0: 95e6 9c89 e999 90e5 85ac e58f b80d 0a0d  ................
+00001ad0: 0a4e 4f54 2041 4e20 4f46 4649 4349 414c  .NOT AN OFFICIAL
+00001ae0: 204d 494e 4543 5241 4654 2050 524f 4455   MINECRAFT PRODU
+00001af0: 4354 2e0d 0a0d 0a4e 4f54 2041 5050 524f  CT.....NOT APPRO
+00001b00: 5645 4420 4259 204f 5220 4153 534f 4349  VED BY OR ASSOCI
+00001b10: 4154 4544 2057 4954 4820 4d4f 4a41 4e47  ATED WITH MOJANG
+00001b20: 204f 5220 4d49 4352 4f53 4f46 542e 0d0a   OR MICROSOFT...
+00001b30: 0d0a 0d0a 0d0a 0d0a 0d0a 5b42 696c 6962  ..........[Bilib
+00001b40: 696c 693a 20e9 8791 e7be bf45 4c53 5d3a  ili: ......ELS]:
+00001b50: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
+00001b60: 656c 6473 2e69 6f2f 6261 6467 652f 4269  elds.io/badge/Bi
+00001b70: 6c69 6269 6c69 2d25 4535 2538 3725 3843  libili-%E5%87%8C
+00001b80: 2545 3425 4241 2539 3125 4539 2538 3725  %E4%BA%91%E9%87%
+00001b90: 3931 2545 3725 4245 2542 462d 3030 4131  91%E7%BE%BF-00A1
+00001ba0: 4537 3f73 7479 6c65 3d66 6f72 2d74 6865  E7?style=for-the
+00001bb0: 2d62 6164 6765 0d0a 5b42 696c 6962 696c  -badge..[Bilibil
+00001bc0: 693a 20e8 afb8 e891 9be4 baae e4b8 8ee5  i: .............
+00001bd0: 85ab e58d a6e9 98b5 5d3a 2068 7474 7073  ........]: https
+00001be0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00001bf0: 6f2f 6261 6467 652f 4269 6c69 6269 6c69  o/badge/Bilibili
+00001c00: 2d25 4538 2541 4625 4238 2545 3825 3931  -%E8%AF%B8%E8%91
+00001c10: 2539 4225 4534 2542 4125 4145 2545 3425  %9B%E4%BA%AE%E4%
+00001c20: 4238 2538 4525 4535 2538 3525 4142 2545  B8%8E%E5%85%AB%E
+00001c30: 3525 3844 2541 3625 4539 2539 3825 4235  5%8D%A6%E9%98%B5
+00001c40: 2d30 3041 3145 373f 7374 796c 653d 666f  -00A1E7?style=fo
+00001c50: 722d 7468 652d 6261 6467 650d 0a5b 436f  r-the-badge..[Co
+00001c60: 6465 5374 796c 653a 2062 6c61 636b 5d3a  deStyle: black]:
+00001c70: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
+00001c80: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
+00001c90: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
+00001ca0: 2d31 3231 3131 302e 7376 673f 7374 796c  -121110.svg?styl
+00001cb0: 653d 666f 722d 7468 652d 6261 6467 650d  e=for-the-badge.
+00001cc0: 0a5b 7079 7468 6f6e 5d3a 2068 7474 7073  .[python]: https
+00001cd0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00001ce0: 6f2f 6261 6467 652f 7079 7468 6f6e 2d33  o/badge/python-3
+00001cf0: 2e36 2d41 4237 3046 463f 7374 796c 653d  .6-AB70FF?style=
+00001d00: 666f 722d 7468 652d 6261 6467 650d 0a5b  for-the-badge..[
+00001d10: 7265 6c65 6173 655d 3a20 6874 7470 733a  release]: https:
+00001d20: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00001d30: 2f67 6974 6875 622f 762f 7265 6c65 6173  /github/v/releas
+00001d40: 652f 4569 6c6c 6573 5761 6e2f 4d75 7369  e/EillesWan/Musi
+00001d50: 6372 6561 7465 723f 7374 796c 653d 666f  creater?style=fo
+00001d60: 722d 7468 652d 6261 6467 650d 0a5b 6c69  r-the-badge..[li
+00001d70: 6365 6e73 655d 3a20 6874 7470 733a 2f2f  cense]: https://
+00001d80: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00001d90: 6164 6765 2f4c 6963 656e 6365 2d41 7061  adge/Licence-Apa
+00001da0: 6368 652d 3232 3842 3232 3f73 7479 6c65  che-228B22?style
+00001db0: 3d66 6f72 2d74 6865 2d62 6164 6765 0d0a  =for-the-badge..
```

### Comparing `Musicreater-0.4.0/setup.py` & `Musicreater-0.5.0/setup.py`

 * *Files identical despite different names*

