# Comparing `tmp/Musicreater-0.5.0.tar.gz` & `tmp/Musicreater-0.5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Musicreater-0.5.0.tar", last modified: Sat Apr 29 11:21:32 2023, max compression
+gzip compressed data, was "Musicreater-0.5.0.1.tar", last modified: Sat Apr 29 14:03:46 2023, max compression
```

## Comparing `Musicreater-0.5.0.tar` & `Musicreater-0.5.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 11:21:32.918646 Musicreater-0.5.0/
--rw-rw-rw-   0        0        0    13085 2023-02-05 09:39:58.000000 Musicreater-0.5.0/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-04-29 11:21:32.904692 Musicreater-0.5.0/Musicreater/
--rw-rw-rw-   0        0        0      890 2023-04-29 11:13:55.000000 Musicreater-0.5.0/Musicreater/__init__.py
--rw-rw-rw-   0        0        0     3195 2023-04-29 11:13:55.000000 Musicreater-0.5.0/Musicreater/exceptions.py
--rw-rw-rw-   0        0        0     5479 2023-04-29 11:13:55.000000 Musicreater-0.5.0/Musicreater/instConstants.py
--rw-rw-rw-   0        0        0    10696 2023-04-29 11:13:55.000000 Musicreater-0.5.0/Musicreater/magicmain.py
--rw-rw-rw-   0        0        0    79538 2023-04-29 11:13:55.000000 Musicreater-0.5.0/Musicreater/main.py
--rw-rw-rw-   0        0        0    13358 2023-04-29 11:13:55.000000 Musicreater-0.5.0/Musicreater/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:21:32.915655 Musicreater-0.5.0/Musicreater.egg-info/
--rw-rw-rw-   0        0        0     7616 2023-04-29 11:21:32.000000 Musicreater-0.5.0/Musicreater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-29 11:21:32.000000 Musicreater-0.5.0/Musicreater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:21:32.000000 Musicreater-0.5.0/Musicreater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-29 11:21:32.000000 Musicreater-0.5.0/Musicreater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 11:21:32.000000 Musicreater-0.5.0/Musicreater.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7616 2023-04-29 11:21:32.917650 Musicreater-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     6547 2023-04-29 11:13:55.000000 Musicreater-0.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 11:21:32.918646 Musicreater-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1533 2023-04-25 15:21:09.000000 Musicreater-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 14:03:46.510571 Musicreater-0.5.0.1/
+-rw-rw-rw-   0        0        0    13085 2023-02-05 09:39:58.000000 Musicreater-0.5.0.1/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-04-29 14:03:46.497614 Musicreater-0.5.0.1/Musicreater/
+-rw-rw-rw-   0        0        0      892 2023-04-29 13:59:22.000000 Musicreater-0.5.0.1/Musicreater/__init__.py
+-rw-rw-rw-   0        0        0     3197 2023-04-29 13:59:22.000000 Musicreater-0.5.0.1/Musicreater/exceptions.py
+-rw-rw-rw-   0        0        0     5479 2023-04-29 11:13:55.000000 Musicreater-0.5.0.1/Musicreater/instConstants.py
+-rw-rw-rw-   0        0        0    10696 2023-04-29 11:13:55.000000 Musicreater-0.5.0.1/Musicreater/magicmain.py
+-rw-rw-rw-   0        0        0    80322 2023-04-29 13:59:22.000000 Musicreater-0.5.0.1/Musicreater/main.py
+-rw-rw-rw-   0        0        0    13451 2023-04-29 13:59:22.000000 Musicreater-0.5.0.1/Musicreater/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 14:03:46.507581 Musicreater-0.5.0.1/Musicreater.egg-info/
+-rw-rw-rw-   0        0        0     7618 2023-04-29 14:03:46.000000 Musicreater-0.5.0.1/Musicreater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-29 14:03:46.000000 Musicreater-0.5.0.1/Musicreater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 14:03:46.000000 Musicreater-0.5.0.1/Musicreater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-29 14:03:46.000000 Musicreater-0.5.0.1/Musicreater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 14:03:46.000000 Musicreater-0.5.0.1/Musicreater.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7618 2023-04-29 14:03:46.509574 Musicreater-0.5.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6547 2023-04-29 11:13:55.000000 Musicreater-0.5.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 14:03:46.510571 Musicreater-0.5.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1597 2023-04-29 13:59:22.000000 Musicreater-0.5.0.1/setup.py
```

### Comparing `Musicreater-0.5.0/LICENSE.md` & `Musicreater-0.5.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Musicreater-0.5.0/Musicreater/__init__.py` & `Musicreater-0.5.0.1/Musicreater/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 版权所有 金羿("Eilles Wan") & 诸葛亮与八卦阵("bgArray") & 鸣凤鸽子("MingFengPigeon")
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 from .main import *
 
-__version__ = "0.5.0"
+__version__ = "0.5.0.1"
 __all__ = []
 __author__ = (("金羿", "Eilles Wan"), ("诸葛亮与八卦阵", "bgArray"), ("鸣凤鸽子", "MingFengPigeon"))
```

### Comparing `Musicreater-0.5.0/Musicreater/exceptions.py` & `Musicreater-0.5.0.1/Musicreater/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """音·创库版本的所有错误均继承于此"""
 
     def __init__(self, *args):
         """音·创库版本的所有错误均继承于此"""
         super().__init__(*args)
 
     def miao(
-        self,
+            self,
     ):
         for i in self.args:
             print(i + "喵！")
 
     def crash_it(self):
         raise self
 
@@ -77,15 +77,15 @@
         """没有Tempo设定导致时间无法计算的错误"""
         super().__init__("在曲目开始时没有声明Tempo（未指定拍长）", *args)
 
 
 class ChannelOverFlowError(MidiFormatException):
     """一个midi中含有过多的通道"""
 
-    def __init__(self, max_channel = 16, *args):
+    def __init__(self, max_channel=16, *args):
         """一个midi中含有过多的通道"""
         super().__init__("含有过多的通道（数量应≤{}）".format(max_channel), *args)
 
 
 class NotDefineProgramError(MidiFormatException):
     """没有Program设定导致没有乐器可以选择的错误"""
```

### Comparing `Musicreater-0.5.0/Musicreater/instConstants.py` & `Musicreater-0.5.0.1/Musicreater/instConstants.py`

 * *Files identical despite different names*

### Comparing `Musicreater-0.5.0/Musicreater/magicmain.py` & `Musicreater-0.5.0.1/Musicreater/magicmain.py`

 * *Files identical despite different names*

### Comparing `Musicreater-0.5.0/Musicreater/main.py` & `Musicreater-0.5.0.1/Musicreater/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,38 +16,38 @@
 版权所有 © 2023 音·创 开发者
 Copyright © 2023 all the developers of Musicreater
 
 开源相关声明请见 ../License.md
 Terms & Conditions: ../License.md
 """
 
-import mido
-import brotli
 import json
-import uuid
 import shutil
+import uuid
+from typing import TypeVar, Union
+
+import brotli
+import mido
 
-from .utils import *
 from .exceptions import *
 from .instConstants import *
-
-from typing import TypeVar, Union
+from .utils import *
 
 T = TypeVar("T")  # Declare type variable
 VM = TypeVar("VM", mido.MidiFile, None)  # void mido
 
 DEFAULT_PROGRESSBAR_STYLE = (
     r"▶ %%N [ %%s/%^s %%% __________ %%t|%^t ]",
     ("§e=§r", "§7=§r"),
 )
 
 
 class SingleNote:
     def __init__(
-        self, instrument: int, pitch: int, velocity: int, startTime: int, lastTime: int
+            self, instrument: int, pitch: int, velocity: int, startTime: int, lastTime: int
     ):
         """用于存储单个音符的类
         :param instrument 乐器编号
         :param pitch 音符编号
         :param velocity 力度/响度
         :param startTime 开始之时(ms)
             注：此处的时间是用从乐曲开始到当前的毫秒数
@@ -212,15 +212,15 @@
         """输出路径"""
         # 将self.midiFile的文件名，不含路径且不含后缀存入self.midiFileName
         self.mid_file_name = os.path.splitext(os.path.basename(self.midi_file))[0]
         """文件名，不含路径且不含后缀"""
 
     @staticmethod
     def __Inst2soundID_withX(
-        instrumentID: int,
+            instrumentID: int,
     ):
         """
         返回midi的乐器ID对应的我的世界乐器名，对于音域转换算法，如下：
         2**( ( msg.note - 60 - X ) / 12 ) 即为MC的音高，其中
         X的取值随乐器不同而变化：
         竖琴harp、电钢琴pling、班卓琴banjo、方波bit、颤音琴iron_xylophone 的时候为6
         吉他的时候为7
@@ -274,18 +274,18 @@
     def score2time(score: int):
         """
         将《我的世界》的计分（以游戏刻计）转为表示时间的字符串
         """
         return str(int(int(score / 20) / 60)) + ":" + str(int(int(score / 20) % 60))
 
     def __form_progress_bar(
-        self,
-        max_score: int,
-        scoreboard_name: str,
-        progressbar_style: tuple = DEFAULT_PROGRESSBAR_STYLE,
+            self,
+            max_score: int,
+            scoreboard_name: str,
+            progressbar_style: tuple = DEFAULT_PROGRESSBAR_STYLE,
     ) -> list:
         """
         生成进度条
 
         Parameters
         ----------
         maxscore: int
@@ -462,18 +462,18 @@
         if r"%%t" in pgs_style:
             result.append("scoreboard objectives remove {}TMinT".format(sbn_pc))
             result.append("scoreboard objectives remove {}TSecT".format(sbn_pc))
 
         return result
 
     def _toCmdList_m1(
-        self,
-        scoreboard_name: str = "mscplay",
-        MaxVolume: float = 1.0,
-        speed: float = 1.0,
+            self,
+            scoreboard_name: str = "mscplay",
+            MaxVolume: float = 1.0,
+            speed: float = 1.0,
     ) -> list:
         """
         使用Dislink Sforza的转换思路，将midi转换为我的世界命令列表
         :param scoreboard_name: 我的世界的计分板名称
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :return: tuple(命令列表, 命令个数, 计分板最大值)
         """
@@ -521,28 +521,28 @@
                         singleTrack.append(
                             "execute @a[scores={"
                             + str(scoreboard_name)
                             + "="
                             + str(nowscore)
                             + "}"
                             + f"] ~ ~ ~ playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg.velocity / 128} "
-                            f"{2 ** ((msg.note - 60 - _X) / 12)}"
+                              f"{2 ** ((msg.note - 60 - _X) / 12)}"
                         )
                         commands += 1
             if len(singleTrack) != 0:
                 tracks.append(singleTrack)
 
         return [tracks, commands, maxscore]
 
     # 原本这个算法的转换效果应该和上面的算法相似的
     def _toCmdList_m2(
-        self,
-        scoreboard_name: str = "mscplay",
-        MaxVolume: float = 1.0,
-        speed: float = 1.0,
+            self,
+            scoreboard_name: str = "mscplay",
+            MaxVolume: float = 1.0,
+            speed: float = 1.0,
     ) -> list:
         """
         使用神羽和金羿的转换思路，将midi转换为我的世界命令列表
         :param scoreboard_name: 我的世界的计分板名称
         :param MaxVolume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :return: tuple(命令列表, 命令个数, 计分板最大值)
@@ -593,15 +593,15 @@
 
                 elif msg.type == "note_on" and msg.velocity != 0:
                     channels[msg.channel].append(
                         ("NoteS", msg.note, msg.velocity, microseconds)
                     )
 
                 elif (msg.type == "note_on" and msg.velocity == 0) or (
-                    msg.type == "note_off"
+                        msg.type == "note_off"
                 ):
                     channels[msg.channel].append(("NoteE", msg.note, microseconds))
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
 
         1 切换乐器消息
@@ -656,29 +656,29 @@
                     nowTrack.append(
                         self.execute_cmd_head.format(
                             "@a[scores=({}={})]".format(scoreboard_name, score_now)
                             .replace("(", r"{")
                             .replace(")", r"}")
                         )
                         + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
-                        f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                          f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                     )
 
                     cmdAmount += 1
 
             if nowTrack:
                 tracks.append(nowTrack)
 
         return [tracks, cmdAmount, maxScore]
 
     def _toCmdList_m3(
-        self,
-        scoreboard_name: str = "mscplay",
-        MaxVolume: float = 1.0,
-        speed: float = 1.0,
+            self,
+            scoreboard_name: str = "mscplay",
+            MaxVolume: float = 1.0,
+            speed: float = 1.0,
     ) -> list:
         """
         使用金羿的转换思路，将midi转换为我的世界命令列表
         :param scoreboard_name: 我的世界的计分板名称
         :param MaxVolume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :return: tuple(命令列表, 命令个数, 计分板最大值)
@@ -716,26 +716,26 @@
         for track_no, track in enumerate(self.midi.tracks):
             microseconds = 0
 
             for msg in track:
                 if msg.time != 0:
                     try:
                         microseconds += (
-                            msg.time * tempo / self.midi.ticks_per_beat / 1000
+                                msg.time * tempo / self.midi.ticks_per_beat / 1000
                         )
                         # print(microseconds)
                     except NameError:
                         if self.debug_mode:
                             raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
                         else:
                             microseconds += (
-                                msg.time
-                                * mido.midifiles.midifiles.DEFAULT_TEMPO
-                                / self.midi.ticks_per_beat
-                            ) / 1000
+                                                    msg.time
+                                                    * mido.midifiles.midifiles.DEFAULT_TEMPO
+                                                    / self.midi.ticks_per_beat
+                                            ) / 1000
 
                 if msg.is_meta:
                     if msg.type == "set_tempo":
                         tempo = msg.tempo
                         if self.debug_mode:
                             self.prt(f"TEMPO更改：{tempo}（毫秒每拍）")
                 else:
@@ -755,15 +755,15 @@
 
                     elif msg.type == "note_on" and msg.velocity != 0:
                         channels[msg.channel][track_no].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
-                        msg.type == "note_off"
+                            msg.type == "note_off"
                     ):
                         channels[msg.channel][track_no].append(
                             ("NoteE", msg.note, microseconds)
                         )
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
@@ -821,30 +821,30 @@
                         nowTrack.append(
                             self.execute_cmd_head.format(
                                 "@a[scores=({}={})]".format(scoreboard_name, score_now)
                                 .replace("(", r"{")
                                 .replace(")", r"}")
                             )
                             + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
-                            f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                              f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                         )
 
                         cmdAmount += 1
 
                 if nowTrack:
                     tracks.append(nowTrack)
 
         return [tracks, cmdAmount, maxScore]
 
     # 简单的单音填充
     def _toCmdList_m4(
-        self,
-        scoreboard_name: str = "mscplay",
-        MaxVolume: float = 1.0,
-        speed: float = 1.0,
+            self,
+            scoreboard_name: str = "mscplay",
+            MaxVolume: float = 1.0,
+            speed: float = 1.0,
     ) -> list:
         """
         使用金羿的转换思路，将midi转换为我的世界命令列表，并使用完全填充算法优化音感
         :param scoreboard_name: 我的世界的计分板名称
         :param MaxVolume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :return: tuple(命令列表, 命令个数, 计分板最大值)
@@ -889,15 +889,15 @@
 
                     elif msg.type == "note_on" and msg.velocity != 0:
                         channels[msg.channel].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
-                        msg.type == "note_off"
+                            msg.type == "note_off"
                     ):
                         channels[msg.channel].append(("NoteE", msg.note, microseconds))
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
 
         1 切换乐器消息
@@ -1005,27 +1005,27 @@
                     nowTrack.append(
                         "execute @a[scores={"
                         + str(scoreboard_name)
                         + "="
                         + str(score_now)
                         + "}"
                         + f"] ~ ~ ~ playsound {soundID} @s ~ ~{1 / every_note[4] - 1} ~ "
-                        f"{note.velocity * (0.7 if CheckFirstChannel else 0.9)} {2 ** ((note.pitch - 60 - _X) / 12)}"
+                          f"{note.velocity * (0.7 if CheckFirstChannel else 0.9)} {2 ** ((note.pitch - 60 - _X) / 12)}"
                     )
 
                     cmdAmount += 1
             tracks.append(nowTrack)
 
         return [tracks, cmdAmount, maxScore]
 
     def _toCmdList_withDelay_m1(
-        self,
-        MaxVolume: float = 1.0,
-        speed: float = 1.0,
-        player: str = "@a",
+            self,
+            MaxVolume: float = 1.0,
+            speed: float = 1.0,
+            player: str = "@a",
     ) -> list:
         """
         使用Dislink Sforza的转换思路，将midi转换为我的世界命令列表，并输出每个音符之后的延迟
         :param MaxVolume: 最大播放音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :param player: 玩家选择器，默认为`@a`
         :return: 全部指令列表[ ( str指令, int距离上一个指令的延迟 ),...]
@@ -1057,21 +1057,21 @@
                             / ((self.midi.ticks_per_beat * float(speed)) * 50000)
                         )
                         soundID, _X = self.__Inst2soundID_withX(instrumentID)
                         try:
                             tracks[now_tick].append(
                                 self.execute_cmd_head.format(player)
                                 + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg.velocity / 128} "
-                                f"{2 ** ((msg.note - 60 - _X) / 12)}"
+                                  f"{2 ** ((msg.note - 60 - _X) / 12)}"
                             )
                         except KeyError:
                             tracks[now_tick] = [
                                 self.execute_cmd_head.format(player)
                                 + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg.velocity / 128} "
-                                f"{2 ** ((msg.note - 60 - _X) / 12)}"
+                                  f"{2 ** ((msg.note - 60 - _X) / 12)}"
                             ]
 
         results = []
 
         all_ticks = list(tracks.keys())
 
         for i in range(len(all_ticks)):
@@ -1086,18 +1086,18 @@
             else:
                 for j in range(len(tracks[all_ticks[i]])):
                     results.append((tracks[all_ticks[i]][j], all_ticks[i]))
 
         return [results, max(all_ticks)]
 
     def _toCmdList_withDelay_m2(
-        self,
-        MaxVolume: float = 1.0,
-        speed: float = 1.0,
-        player: str = "@a",
+            self,
+            MaxVolume: float = 1.0,
+            speed: float = 1.0,
+            player: str = "@a",
     ) -> list:
         """
         使用神羽和金羿的转换思路，将midi转换为我的世界命令列表，并输出每个音符之后的延迟
         :param MaxVolume: 最大播放音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :param player: 玩家选择器，默认为`@a`
         :return: 全部指令列表[ ( str指令, int距离上一个指令的延迟 ),...]
@@ -1133,24 +1133,24 @@
 
         microseconds = 0
 
         # 我们来用通道统计音乐信息
         for msg in self.midi:
             try:
                 microseconds += (
-                    msg.time * 1000
+                        msg.time * 1000
                 )  # 任何人都tm不要动这里，这里循环方式不是track，所以，这里的计时方式不一样
 
                 # print(microseconds)
             except NameError:
                 if self.debug_mode:
                     raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
                 else:
                     microseconds += (
-                        msg.time * 1000
+                            msg.time * 1000
                     )  # 任何人都tm不要动这里，这里循环方式不是track，所以，这里的计时方式不一样
 
             if msg.is_meta:
                 if msg.type == "set_tempo":
                     tempo = msg.tempo
             else:
                 if self.debug_mode:
@@ -1165,15 +1165,15 @@
 
                 elif msg.type == "note_on" and msg.velocity != 0:
                     channels[msg.channel].append(
                         ("NoteS", msg.note, msg.velocity, microseconds)
                     )
 
                 elif (msg.type == "note_on" and msg.velocity == 0) or (
-                    msg.type == "note_off"
+                        msg.type == "note_off"
                 ):
                     channels[msg.channel].append(("NoteE", msg.note, microseconds))
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
 
         1 切换乐器消息
@@ -1219,21 +1219,21 @@
                             )
                     score_now = round(msg[-1] / float(speed) / 50)
 
                     try:
                         tracks[score_now].append(
                             self.execute_cmd_head.format(player)
                             + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
-                            f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                              f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                         )
                     except KeyError:
                         tracks[score_now] = [
                             self.execute_cmd_head.format(player)
                             + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
-                            f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                              f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                         ]
 
         all_ticks = list(tracks.keys())
 
         for i in range(len(all_ticks)):
             for j in range(len(tracks[all_ticks[i]])):
                 results.append(
@@ -1250,18 +1250,18 @@
                         ),
                     )
                 )
 
         return [results, max(all_ticks)]
 
     def _toCmdList_withDelay_m3(
-        self,
-        MaxVolume: float = 1.0,
-        speed: float = 1.0,
-        player: str = "@a",
+            self,
+            MaxVolume: float = 1.0,
+            speed: float = 1.0,
+            player: str = "@a",
     ) -> list:
         """
         使用金羿的转换思路，将midi转换为我的世界命令列表，并输出每个音符之后的延迟
         :param MaxVolume: 最大播放音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :param player: 玩家选择器，默认为`@a`
         :return: 全部指令列表[ ( str指令, int距离上一个指令的延迟 ),...]
@@ -1299,26 +1299,26 @@
         for track_no, track in enumerate(self.midi.tracks):
             microseconds = 0
 
             for msg in track:
                 if msg.time != 0:
                     try:
                         microseconds += (
-                            msg.time * tempo / self.midi.ticks_per_beat / 1000
+                                msg.time * tempo / self.midi.ticks_per_beat / 1000
                         )
                         # print(microseconds)
                     except NameError:
                         if self.debug_mode:
                             raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
                         else:
                             microseconds += (
-                                msg.time
-                                * mido.midifiles.midifiles.DEFAULT_TEMPO
-                                / self.midi.ticks_per_beat
-                            ) / 1000
+                                                    msg.time
+                                                    * mido.midifiles.midifiles.DEFAULT_TEMPO
+                                                    / self.midi.ticks_per_beat
+                                            ) / 1000
 
                 if msg.is_meta:
                     if msg.type == "set_tempo":
                         tempo = msg.tempo
                         if self.debug_mode:
                             self.prt(f"TEMPO更改：{tempo}（毫秒每拍）")
                 else:
@@ -1338,15 +1338,15 @@
 
                     elif msg.type == "note_on" and msg.velocity != 0:
                         channels[msg.channel][track_no].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
-                        msg.type == "note_off"
+                            msg.type == "note_off"
                     ):
                         channels[msg.channel][track_no].append(
                             ("NoteE", msg.note, microseconds)
                         )
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
@@ -1396,21 +1396,21 @@
                                 )
                         score_now = round(msg[-1] / float(speed) / 50)
 
                         try:
                             tracks[score_now].append(
                                 self.execute_cmd_head.format(player)
                                 + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
-                                f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                                  f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                             )
                         except KeyError:
                             tracks[score_now] = [
                                 self.execute_cmd_head.format(player)
                                 + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
-                                f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                                  f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                             ]
 
         all_ticks = list(tracks.keys())
         results = []
 
         for i in range(len(all_ticks)):
             for j in range(len(tracks[all_ticks[i]])):
@@ -1428,21 +1428,21 @@
                         ),
                     )
                 )
 
         return [results, max(all_ticks)]
 
     def to_mcpack(
-        self,
-        method: int = 1,
-        volume: float = 1.0,
-        speed: float = 1.0,
-        progressbar: Union[bool, tuple] = None,
-        scoreboard_name: str = "mscplay",
-        isAutoReset: bool = False,
+            self,
+            method: int = 1,
+            volume: float = 1.0,
+            speed: float = 1.0,
+            progressbar: Union[bool, tuple] = None,
+            scoreboard_name: str = "mscplay",
+            isAutoReset: bool = False,
     ) -> tuple:
         """
         使用method指定的转换算法，将midi转换为我的世界mcpack格式的包
         :param method: 转换算法
         :param isAutoReset: 是否自动重置计分板
         :param progressbar: 进度条，（当此参数为True时使用默认进度条，为其他的值为真的参数时识别为进度条自定义参数，为其他值为假的时候不生成进度条）
         :param scoreboard_name: 我的世界的计分板名称
@@ -1462,15 +1462,15 @@
         if os.path.exists(f"{self.output_path}/temp/functions/"):
             shutil.rmtree(f"{self.output_path}/temp/functions/")
         os.makedirs(f"{self.output_path}/temp/functions/mscplay")
 
         # 写入manifest.json
         if not os.path.exists(f"{self.output_path}/temp/manifest.json"):
             with open(
-                f"{self.output_path}/temp/manifest.json", "w", encoding="utf-8"
+                    f"{self.output_path}/temp/manifest.json", "w", encoding="utf-8"
             ) as f:
                 f.write(
                     '{\n  "format_version": 1,\n  "header": {\n    "description": "'
                     + self.mid_file_name
                     + ' Pack : behavior pack",\n    "version": [ 0, 0, 1 ],\n    "name": "'
                     + self.mid_file_name
                     + 'Pack",\n    "uuid": "'
@@ -1479,15 +1479,15 @@
                     + f"the Player of the Music {self.mid_file_name}"
                     + '",\n      "type": "data",\n      "version": [ 0, 0, 1 ],\n      "uuid": "'
                     + str(uuid.uuid4())
                     + '"\n    }\n  ]\n}'
                 )
         else:
             with open(
-                f"{self.output_path}/temp/manifest.json", "r", encoding="utf-8"
+                    f"{self.output_path}/temp/manifest.json", "r", encoding="utf-8"
             ) as manifest:
                 data = json.loads(manifest.read())
                 data["header"][
                     "description"
                 ] = f"the Player of the Music {self.mid_file_name}"
                 data["header"]["name"] = self.mid_file_name
                 data["header"]["uuid"] = str(uuid.uuid4())
@@ -1503,57 +1503,57 @@
             f"{self.output_path}/temp/functions/index.mcfunction", "w", encoding="utf-8"
         )
         for track in cmdlist:
             index_file.write(
                 "function mscplay/track" + str(cmdlist.index(track) + 1) + "\n"
             )
             with open(
-                f"{self.output_path}/temp/functions/mscplay/track{cmdlist.index(track) + 1}.mcfunction",
-                "w",
-                encoding="utf-8",
+                    f"{self.output_path}/temp/functions/mscplay/track{cmdlist.index(track) + 1}.mcfunction",
+                    "w",
+                    encoding="utf-8",
             ) as f:
                 f.write("\n".join(track))
         index_file.writelines(
             (
                 "scoreboard players add @a[scores={"
                 + scoreboard_name
                 + "=1..}] "
                 + scoreboard_name
                 + " 1\n",
                 (
-                    "scoreboard players reset @a[scores={"
-                    + scoreboard_name
-                    + "="
-                    + str(maxscore + 20)
-                    + "..}]"
-                    + f" {scoreboard_name}\n"
+                        "scoreboard players reset @a[scores={"
+                        + scoreboard_name
+                        + "="
+                        + str(maxscore + 20)
+                        + "..}]"
+                        + f" {scoreboard_name}\n"
                 )
                 if isAutoReset
                 else "",
                 f"function mscplay/progressShow\n" if progressbar else "",
             )
         )
 
         if progressbar:
             # 此处是对于仅有 True 的参数和自定义参数的判断
             # 改这一行没🐎
             if progressbar is True:
                 with open(
-                    f"{self.output_path}/temp/functions/mscplay/progressShow.mcfunction",
-                    "w",
-                    encoding="utf-8",
+                        f"{self.output_path}/temp/functions/mscplay/progressShow.mcfunction",
+                        "w",
+                        encoding="utf-8",
                 ) as f:
                     f.writelines(
                         "\n".join(self.__form_progress_bar(maxscore, scoreboard_name))
                     )
             else:
                 with open(
-                    f"{self.output_path}/temp/functions/mscplay/progressShow.mcfunction",
-                    "w",
-                    encoding="utf-8",
+                        f"{self.output_path}/temp/functions/mscplay/progressShow.mcfunction",
+                        "w",
+                        encoding="utf-8",
                 ) as f:
                     f.writelines(
                         "\n".join(
                             self.__form_progress_bar(
                                 maxscore, scoreboard_name, progressbar
                             )
                         )
@@ -1569,21 +1569,21 @@
         )
 
         shutil.rmtree(f"{self.output_path}/temp/")
 
         return True, maxlen, maxscore
 
     def to_mcpack_with_delay(
-        self,
-        method: int = 1,
-        volume: float = 1.0,
-        speed: float = 1.0,
-        progressbar: Union[bool, tuple] = False,
-        player: str = "@a",
-        max_height: int = 64,
+            self,
+            method: int = 1,
+            volume: float = 1.0,
+            speed: float = 1.0,
+            progressbar: Union[bool, tuple] = False,
+            player: str = "@a",
+            max_height: int = 64,
     ):
         """
         使用method指定的转换算法，将midi转换为mcstructure结构文件后打包成mcpack文件
         :param method: 转换算法
         :param author: 作者名称
         :param progressbar: 进度条，（当此参数为True时使用默认进度条，为其他的值为真的参数时识别为进度条自定义参数，为其他值为假的时候不生成进度条）
         :param max_height: 生成结构最大高度
@@ -1642,22 +1642,22 @@
         # 将命令列表写入文件
         index_file = open(
             f"{self.output_path}/temp/functions/index.mcfunction", "w", encoding="utf-8"
         )
 
         struct, size, end_pos = commands_to_structure(command_list, max_height - 1)
         with open(
-            os.path.abspath(
-                os.path.join(
-                    self.output_path,
-                    "temp/structures/",
-                    f"{self.mid_file_name}_main.mcstructure",
-                )
-            ),
-            "wb+",
+                os.path.abspath(
+                    os.path.join(
+                        self.output_path,
+                        "temp/structures/",
+                        f"{self.mid_file_name}_main.mcstructure",
+                    )
+                ),
+                "wb+",
         ) as f:
             struct.dump(f)
 
         del struct
 
         if progressbar:
             scb_name = self.mid_file_name[:5] + "Pgb"
@@ -1676,44 +1676,44 @@
                     1,
                     1,
                     customName="显示进度条并加分",
                 ),
             )
 
             with open(
-                os.path.abspath(
-                    os.path.join(
-                        self.output_path,
-                        "temp/structures/",
-                        f"{self.mid_file_name}_start.mcstructure",
-                    )
-                ),
-                "wb+",
+                    os.path.abspath(
+                        os.path.join(
+                            self.output_path,
+                            "temp/structures/",
+                            f"{self.mid_file_name}_start.mcstructure",
+                        )
+                    ),
+                    "wb+",
             ) as f:
                 struct_a.dump(f)
 
             index_file.write(f"structure load {self.mid_file_name}_start ~ ~ ~1\n")
 
             pgb_struct, pgbSize, pgbNowPos = commands_to_structure(
                 [
                     (i, 0)
                     for i in self.__form_progress_bar(max_delay, scb_name, progressbar)
                 ],
                 max_height - 1,
             )
 
             with open(
-                os.path.abspath(
-                    os.path.join(
-                        self.output_path,
-                        "temp/structures/",
-                        f"{self.mid_file_name}_pgb.mcstructure",
-                    )
-                ),
-                "wb+",
+                    os.path.abspath(
+                        os.path.join(
+                            self.output_path,
+                            "temp/structures/",
+                            f"{self.mid_file_name}_pgb.mcstructure",
+                        )
+                    ),
+                    "wb+",
             ) as f:
                 pgb_struct.dump(f)
 
             index_file.write(f"structure load {self.mid_file_name}_pgb ~ ~1 ~1\n")
 
             struct_a = Structure(
                 (1, 1, 1),
@@ -1726,33 +1726,33 @@
                     1,
                     1,
                     customName="重置进度条计分板",
                 ),
             )
 
             with open(
-                os.path.abspath(
-                    os.path.join(
-                        self.output_path,
-                        "temp/structures/",
-                        f"{self.mid_file_name}_reset.mcstructure",
-                    )
-                ),
-                "wb+",
+                    os.path.abspath(
+                        os.path.join(
+                            self.output_path,
+                            "temp/structures/",
+                            f"{self.mid_file_name}_reset.mcstructure",
+                        )
+                    ),
+                    "wb+",
             ) as f:
                 struct_a.dump(f)
 
             del struct_a, pgb_struct
 
             index_file.write(
-                f"structure load {self.mid_file_name}_reset ~{pgbSize[0]+2} ~ ~1\n"
+                f"structure load {self.mid_file_name}_reset ~{pgbSize[0] + 2} ~ ~1\n"
             )
 
             index_file.write(
-                f"structure load {self.mid_file_name}_main ~{pgbSize[0]+2} ~1 ~1\n"
+                f"structure load {self.mid_file_name}_main ~{pgbSize[0] + 2} ~1 ~1\n"
             )
 
         else:
             index_file.write(f"structure load {self.mid_file_name}_main ~ ~ ~1\n")
 
         index_file.close()
 
@@ -1764,20 +1764,20 @@
         )
 
         shutil.rmtree(f"{self.output_path}/temp/")
 
         return True, len(command_list), max_delay
 
     def to_mcstructure_file_with_delay(
-        self,
-        method: int = 1,
-        volume: float = 1.0,
-        speed: float = 1.0,
-        player: str = "@a",
-        max_height: int = 64,
+            self,
+            method: int = 1,
+            volume: float = 1.0,
+            speed: float = 1.0,
+            player: str = "@a",
+            max_height: int = 64,
     ):
         """
         使用method指定的转换算法，将midi转换为mcstructure结构文件
         :param method: 转换算法
         :param author: 作者名称
         :param progressbar: 进度条，（当此参数为True时使用默认进度条，为其他的值为真的参数时识别为进度条自定义参数，为其他值为假的时候不生成进度条）
         :param max_height: 生成结构最大高度
@@ -1798,33 +1798,33 @@
 
         if not os.path.exists(self.output_path):
             os.makedirs(self.output_path)
 
         struct, size, end_pos = commands_to_structure(cmd_list, max_height - 1)
 
         with open(
-            os.path.abspath(
-                os.path.join(self.output_path, f"{self.mid_file_name}.mcstructure")
-            ),
-            "wb+",
+                os.path.abspath(
+                    os.path.join(self.output_path, f"{self.mid_file_name}.mcstructure")
+                ),
+                "wb+",
         ) as f:
             struct.dump(f)
 
         return True, size, max_delay
 
     def to_BDX_file(
-        self,
-        method: int = 1,
-        volume: float = 1.0,
-        speed: float = 1.0,
-        progressbar: Union[bool, tuple] = False,
-        scoreboard_name: str = "mscplay",
-        isAutoReset: bool = False,
-        author: str = "Eilles",
-        max_height: int = 64,
+            self,
+            method: int = 1,
+            volume: float = 1.0,
+            speed: float = 1.0,
+            progressbar: Union[bool, tuple] = False,
+            scoreboard_name: str = "mscplay",
+            isAutoReset: bool = False,
+            author: str = "Eilles",
+            max_height: int = 64,
     ):
         """
         使用method指定的转换算法，将midi转换为BDX结构文件
         :param method: 转换算法
         :param author: 作者名称
         :param progressbar: 进度条，（当此参数为True时使用默认进度条，为其他的值为真的参数时识别为进度条自定义参数，为其他值为假的时候不生成进度条）
         :param max_height: 生成结构最大高度
@@ -1841,25 +1841,25 @@
         # except Exception as E:
         #     return (False, f"无法找到算法ID{method}对应的转换算法: {E}")
 
         if not os.path.exists(self.output_path):
             os.makedirs(self.output_path)
 
         with open(
-            os.path.abspath(
-                os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
-            ),
-            "w+",
+                os.path.abspath(
+                    os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
+                ),
+                "w+",
         ) as f:
             f.write("BD@")
 
         _bytes = (
-            b"BDX\x00"
-            + author.encode("utf-8")
-            + b" & Musicreater\x00\x01command_block\x00"
+                b"BDX\x00"
+                + author.encode("utf-8")
+                + b" & Musicreater\x00\x01command_block\x00"
         )
 
         commands = []
 
         for track in cmdlist:
             commands += track
 
@@ -1878,22 +1878,22 @@
         )
 
         if progressbar:
             pgbBytes, pgbSize, pgbNowPos = commands_to_BDX_bytes(
                 [
                     (i, 0)
                     for i in (
-                        self.__form_progress_bar(maxScore, scoreboard_name)
-                        # 此处是对于仅有 True 的参数和自定义参数的判断
-                        # 改这一行没🐎
-                        if progressbar is True
-                        else self.__form_progress_bar(
-                            maxScore, scoreboard_name, progressbar
-                        )
+                    self.__form_progress_bar(maxScore, scoreboard_name)
+                    # 此处是对于仅有 True 的参数和自定义参数的判断
+                    # 改这一行没🐎
+                    if progressbar is True
+                    else self.__form_progress_bar(
+                        maxScore, scoreboard_name, progressbar
                     )
+                )
                 ],
                 max_height - 1,
             )
             _bytes += pgbBytes
             _bytes += bdx_move(y, -pgbNowPos[1])
             _bytes += bdx_move(z, -pgbNowPos[2])
             _bytes += bdx_move(x, 2)
@@ -1901,32 +1901,32 @@
             size[0] += 2 + pgbSize[0]
             size[1] = max(size[1], pgbSize[1])
             size[2] = max(size[2], pgbSize[2])
 
         _bytes += cmdBytes
 
         with open(
-            os.path.abspath(
-                os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
-            ),
-            "ab+",
+                os.path.abspath(
+                    os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
+                ),
+                "ab+",
         ) as f:
             f.write(brotli.compress(_bytes + b"XE"))
 
         return True, total_count, maxScore, size, finalPos
 
     def to_BDX_file_with_delay(
-        self,
-        method: int = 1,
-        volume: float = 1.0,
-        speed: float = 1.0,
-        progressbar: Union[bool, tuple] = False,
-        player: str = "@a",
-        author: str = "Eilles",
-        max_height: int = 64,
+            self,
+            method: int = 1,
+            volume: float = 1.0,
+            speed: float = 1.0,
+            progressbar: Union[bool, tuple] = False,
+            player: str = "@a",
+            author: str = "Eilles",
+            max_height: int = 64,
     ):
         """
         使用method指定的转换算法，将midi转换为BDX结构文件
         :param method: 转换算法
         :param author: 作者名称
         :param progressbar: 进度条，（当此参数为True时使用默认进度条，为其他的值为真的参数时识别为进度条自定义参数，为其他值为假的时候不生成进度条）
         :param max_height: 生成结构最大高度
@@ -1945,25 +1945,25 @@
         # except Exception as E:
         #     return (False, f"无法找到算法ID{method}对应的转换算法\n{E}")
 
         if not os.path.exists(self.output_path):
             os.makedirs(self.output_path)
 
         with open(
-            os.path.abspath(
-                os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
-            ),
-            "w+",
+                os.path.abspath(
+                    os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
+                ),
+                "w+",
         ) as f:
             f.write("BD@")
 
         _bytes = (
-            b"BDX\x00"
-            + author.encode("utf-8")
-            + b" & Musicreater\x00\x01command_block\x00"
+                b"BDX\x00"
+                + author.encode("utf-8")
+                + b" & Musicreater\x00\x01command_block\x00"
         )
 
         # 此处是对于仅有 True 的参数和自定义参数的判断
         # 改这一行没🐎
         if progressbar is True:
             progressbar = DEFAULT_PROGRESSBAR_STYLE
 
@@ -2005,25 +2005,25 @@
             size[1] = max(size[1], pgbSize[1])
             size[2] = max(size[2], pgbSize[2])
 
         size[1] += 1
         _bytes += cmdBytes
 
         with open(
-            os.path.abspath(
-                os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
-            ),
-            "ab+",
+                os.path.abspath(
+                    os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
+                ),
+                "ab+",
         ) as f:
             f.write(brotli.compress(_bytes + b"XE"))
 
         return True, len(cmdlist), max_delay, size, finalPos
 
     def toDICT(
-        self,
+            self,
     ) -> dict:
         """
         使用金羿的转换思路，将midi转换为字典
         :return: dict()
         """
 
         # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
@@ -2058,17 +2058,17 @@
                         microseconds += msg.time * tempo / self.midi.ticks_per_beat
                         # print(microseconds)
                     except NameError:
                         if self.debug_mode:
                             raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
                         else:
                             microseconds += (
-                                msg.time
-                                * mido.midifiles.midifiles.DEFAULT_TEMPO
-                                / self.midi.ticks_per_beat
+                                    msg.time
+                                    * mido.midifiles.midifiles.DEFAULT_TEMPO
+                                    / self.midi.ticks_per_beat
                             )
 
                 if msg.is_meta:
                     if msg.type == "set_tempo":
                         tempo = msg.tempo
                         if self.debug_mode:
                             self.prt(f"TEMPO更改：{tempo}（毫秒每拍）")
@@ -2089,15 +2089,15 @@
 
                     elif msg.type == "note_on" and msg.velocity != 0:
                         channels[msg.channel][track_no].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
-                        msg.type == "note_off"
+                            msg.type == "note_off"
                     ):
                         channels[msg.channel][track_no].append(
                             ("NoteE", msg.note, microseconds)
                         )
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
```

### Comparing `Musicreater-0.5.0/Musicreater/utils.py` & `Musicreater-0.5.0.1/Musicreater/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 import os
-from typing import Union
+
 from TrimMCStruct import Structure, Block, TAG_Long, TAG_Byte
 
 bdx_key = {
     "x": [b"\x0f", b"\x0e", b"\x1c", b"\x14", b"\x15"],
     "y": [b"\x11", b"\x10", b"\x1d", b"\x16", b"\x17"],
     "z": [b"\x13", b"\x12", b"\x1e", b"\x18", b"\x19"],
 }
@@ -22,19 +22,19 @@
     if abs(value) == 1:
         return bdx_key[axis][0 if value == -1 else 1]
 
     pointer = sum(
         [
             1 if i else 0
             for i in (
-                value != -1,
-                value < -1 or value > 1,
-                value < -128 or value > 127,
-                value < -32768 or value > 32767,
-            )
+            value != -1,
+            value < -1 or value > 1,
+            value < -128 or value > 127,
+            value < -32768 or value > 32767,
+        )
         ]
     )
 
     return bdx_key[axis][pointer] + value.to_bytes(
         2 ** (pointer - 2), "big", signed=True
     )
 
@@ -58,23 +58,23 @@
             pathfile = os.path.join(parent, filename)
             arc_name = pathfile[pre_len:].strip(os.path.sep)  # 相对路径
             zipf.write(pathfile, arc_name)
     zipf.close()
 
 
 def form_command_block_in_BDX_bytes(
-    command: str,
-    particularValue: int,
-    impluse: int = 0,
-    condition: bool = False,
-    needRedstone: bool = True,
-    tickDelay: int = 0,
-    customName: str = "",
-    executeOnFirstTick: bool = False,
-    trackOutput: bool = True,
+        command: str,
+        particularValue: int,
+        impluse: int = 0,
+        condition: bool = False,
+        needRedstone: bool = True,
+        tickDelay: int = 0,
+        customName: str = "",
+        executeOnFirstTick: bool = False,
+        trackOutput: bool = True,
 ):
     """
     使用指定项目返回指定的指令方块放置指令项
     :param command: `str`
         指令
     :param particularValue:
         方块特殊值，即朝向
@@ -138,16 +138,16 @@
     :param total: 总方块数量
     :param maxHeight: 最大高度
     :return: 外切正方形的边长 int"""
     return math.ceil(math.sqrt(math.ceil(total / maxHeight)))
 
 
 def commands_to_BDX_bytes(
-    commands: list,
-    max_height: int = 64,
+        commands: list,
+        max_height: int = 64,
 ):
     """
     :param commands: 指令列表(指令, 延迟)
     :param max_height: 生成结构最大高度
     :return 成功与否，成功返回(True,未经过压缩的源,结构占用大小)，失败返回(False,str失败原因)
     """
 
@@ -171,21 +171,21 @@
         customName = ""
         executeOnFirstTick = False
         trackOutput = True
         _bytes += form_command_block_in_BDX_bytes(
             cmd,
             (1 if y_forward else 0)
             if (
-                ((now_y != 0) and (not y_forward))
-                or (y_forward and (now_y != (max_height - 1)))
+                    ((now_y != 0) and (not y_forward))
+                    or (y_forward and (now_y != (max_height - 1)))
             )
             else (3 if z_forward else 2)
             if (
-                ((now_z != 0) and (not z_forward))
-                or (z_forward and (now_z != _sideLength - 1))
+                    ((now_z != 0) and (not z_forward))
+                    or (z_forward and (now_z != _sideLength - 1))
             )
             else 5,
             impluse=impluse,
             condition=condition,
             needRedstone=needRedstone,
             tickDelay=tickDelay,
             customName=customName,
@@ -199,15 +199,15 @@
             now_y -= 1 if y_forward else -1
 
             y_forward = not y_forward
 
             now_z += 1 if z_forward else -1
 
             if ((now_z >= _sideLength) and z_forward) or (
-                (now_z < 0) and (not z_forward)
+                    (now_z < 0) and (not z_forward)
             ):
                 now_z -= 1 if z_forward else -1
                 z_forward = not z_forward
                 _bytes += bdx_key[x][1]
                 now_x += 1
             else:
                 _bytes += bdx_key[z][int(z_forward)]
@@ -223,15 +223,15 @@
             _sideLength if now_x else now_z,
         ],
         [now_x, now_y, now_z],
     )
 
 
 def form_note_block_in_NBT_struct(
-    note: int, coordinate: tuple, instrument: str = "note.harp", powered: bool = False
+        note: int, coordinate: tuple, instrument: str = "note.harp", powered: bool = False
 ):
     """生成音符盒方块
     :param note: `int`(0~24)
         音符的音高
     :param coordinate: `tuple[int,int,int]`
         此方块所在之相对坐标
     :param instrument: `str`
@@ -258,43 +258,44 @@
                 "z": coordinate[2],
             }
         },
     )
 
 
 def form_repeater_in_NBT_struct(
-    delay: int, facing: int
+        delay: int, facing: int
 ):
     """生成中继器方块
     :param powered:
     :param locked:
     :param facing:
     :param delay: 1~4
     :return Block()"""
-    
+
     return Block(
         "minecraft",
         "unpowered_repeater",
         {
             "repeater_delay": delay,
             "direction": facing,
         },
     )
 
+
 def form_command_block_in_NBT_struct(
-    command: str,
-    coordinate: tuple,
-    particularValue: int,
-    impluse: int = 0,
-    condition: bool = False,
-    alwaysRun: bool = True,
-    tickDelay: int = 0,
-    customName: str = "",
-    executeOnFirstTick: bool = False,
-    trackOutput: bool = True,
+        command: str,
+        coordinate: tuple,
+        particularValue: int,
+        impluse: int = 0,
+        condition: bool = False,
+        alwaysRun: bool = True,
+        tickDelay: int = 0,
+        customName: str = "",
+        executeOnFirstTick: bool = False,
+        trackOutput: bool = True,
 ):
     """
     使用指定项目返回指定的指令方块结构
     :param command: `str`
         指令
     :param coordinate: `tuple[int,int,int]`
         此方块所在之相对坐标
@@ -368,17 +369,18 @@
                 "y": coordinate[1],
                 "z": coordinate[2],
             }
         },
         compability_version=17959425,
     )
 
+
 def commands_to_structure(
-    commands: list,
-    max_height: int = 64,
+        commands: list,
+        max_height: int = 64,
 ):
     """
     :param commands: 指令列表(指令, 延迟)
     :param max_height: 生成结构最大高度
     :return 成功与否，成功返回(结构类,结构占用大小)，失败返回(False,str失败原因)
     """
 
@@ -402,22 +404,22 @@
         struct.set_block(
             coordinate,
             form_command_block_in_NBT_struct(
                 command=cmd,
                 coordinate=coordinate,
                 particularValue=(1 if y_forward else 0)
                 if (
-                    ((now_y != 0) and (not y_forward))
-                    or (y_forward and (now_y != (max_height - 1)))
+                        ((now_y != 0) and (not y_forward))
+                        or (y_forward and (now_y != (max_height - 1)))
                 )
                 else (
                     (3 if z_forward else 2)
                     if (
-                        ((now_z != 0) and (not z_forward))
-                        or (z_forward and (now_z != _sideLength - 1))
+                            ((now_z != 0) and (not z_forward))
+                            or (z_forward and (now_z != _sideLength - 1))
                     )
                     else 5
                 ),
                 impluse=2,
                 condition=False,
                 alwaysRun=True,
                 tickDelay=delay,
@@ -433,23 +435,22 @@
             now_y -= 1 if y_forward else -1
 
             y_forward = not y_forward
 
             now_z += 1 if z_forward else -1
 
             if ((now_z >= _sideLength) and z_forward) or (
-                (now_z < 0) and (not z_forward)
+                    (now_z < 0) and (not z_forward)
             ):
                 now_z -= 1 if z_forward else -1
                 z_forward = not z_forward
                 now_x += 1
 
     return (
         struct,
         (
             now_x + 1,
             max_height if now_x or now_z else now_y,
             _sideLength if now_x else now_z,
         ),
         (now_x, now_y, now_z),
     )
-
```

### Comparing `Musicreater-0.5.0/Musicreater.egg-info/PKG-INFO` & `Musicreater-0.5.0.1/Musicreater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 0.5.0
+Version: 0.5.0.1
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Musicreater Version: 0.5.0 Summary:
+Metadata-Version: 2.1 Name: Musicreater Version: 0.5.0.1 Summary:
 ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã midé³ä¹è½¬æ¢åºã Home-page:
 https://github.com/TriM-Organization/Musicreater Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: Chinese (Simplified) Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `Musicreater-0.5.0/PKG-INFO` & `Musicreater-0.5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 0.5.0
+Version: 0.5.0.1
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Musicreater Version: 0.5.0 Summary:
+Metadata-Version: 2.1 Name: Musicreater Version: 0.5.0.1 Summary:
 ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã midé³ä¹è½¬æ¢åºã Home-page:
 https://github.com/TriM-Organization/Musicreater Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: Chinese (Simplified) Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `Musicreater-0.5.0/README.md` & `Musicreater-0.5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Musicreater-0.5.0/setup.py` & `Musicreater-0.5.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # -*- coding: utf-8 -*-
 import setuptools
 import Musicreater
 
+with open("requirements.txt", "r", encoding="utf-8") as fh:
+    dependences = fh.read().strip().split("\n")
+
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read().replace(
         "./docs/", "https://github.com/TriM-Organization/Musicreater/blob/master/docs/"
     )
 
 setuptools.setup(
     name="Musicreater",
@@ -29,12 +32,9 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     # 需要安装的依赖
-    install_requires=[
-        "Brotli>=1.0.9",
-        "mido>=1.2.10",
-    ],
+    install_requires=dependences,
 )
```

