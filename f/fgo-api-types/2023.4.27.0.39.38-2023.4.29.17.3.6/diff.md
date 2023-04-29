# Comparing `tmp/fgo_api_types-2023.4.27.0.39.38.tar.gz` & `tmp/fgo_api_types-2023.4.29.17.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.4.27.0.39.38.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.4.29.17.3.6.tar", max compression
```

## Comparing `fgo_api_types-2023.4.27.0.39.38.tar` & `fgo_api_types-2023.4.29.17.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-04-27 00:39:10.151042 fgo_api_types-2023.4.27.0.39.38/LICENSE
--rw-r--r--   0        0        0      449 2023-04-27 00:39:10.151042 fgo_api_types-2023.4.27.0.39.38/README.md
--rw-r--r--   0        0        0        0 2023-04-27 00:39:38.567201 fgo_api_types-2023.4.27.0.39.38/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-04-27 00:39:38.567201 fgo_api_types-2023.4.27.0.39.38/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-04-27 00:39:38.567201 fgo_api_types-2023.4.27.0.39.38/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-04-27 00:39:38.567201 fgo_api_types-2023.4.27.0.39.38/fgo_api_types/common.py
--rw-r--r--   0        0        0    37696 2023-04-27 00:39:38.567201 fgo_api_types-2023.4.27.0.39.38/fgo_api_types/enums.py
--rw-r--r--   0        0        0   155885 2023-04-27 00:39:38.567201 fgo_api_types-2023.4.27.0.39.38/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    74771 2023-04-27 00:39:38.567201 fgo_api_types-2023.4.27.0.39.38/fgo_api_types/nice.py
--rw-r--r--   0        0        0    50178 2023-04-27 00:39:38.567201 fgo_api_types-2023.4.27.0.39.38/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-04-27 00:39:38.567201 fgo_api_types-2023.4.27.0.39.38/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18464 2023-04-27 00:39:38.567201 fgo_api_types-2023.4.27.0.39.38/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-04-27 00:39:39.019203 fgo_api_types-2023.4.27.0.39.38/pyproject.toml
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.4.27.0.39.38/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-29 17:02:43.279729 fgo_api_types-2023.4.29.17.3.6/LICENSE
+-rw-r--r--   0        0        0      449 2023-04-29 17:02:43.279729 fgo_api_types-2023.4.29.17.3.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/common.py
+-rw-r--r--   0        0        0    37696 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   157289 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    74847 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    50178 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    18670 2023-04-29 17:03:06.163928 fgo_api_types-2023.4.29.17.3.6/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-04-29 17:03:06.491740 fgo_api_types-2023.4.29.17.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 fgo_api_types-2023.4.29.17.3.6/PKG-INFO
```

### Comparing `fgo_api_types-2023.4.27.0.39.38/LICENSE` & `fgo_api_types-2023.4.29.17.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.27.0.39.38/fgo_api_types/basic.py` & `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.27.0.39.38/fgo_api_types/common.py` & `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.27.0.39.38/fgo_api_types/enums.py` & `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.27.0.39.38/fgo_api_types/gameenums.py` & `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/gameenums.py`

 * *Files 1% similar despite different names*

```diff
@@ -4932,7 +4932,49 @@
     self_ = "self"
 
 
 BUFF_CONVERT_LIMIT_TYPE_NAME: dict[int, NiceBuffConvertLimitType] = {
     0: NiceBuffConvertLimitType.all,
     1: NiceBuffConvertLimitType.self_,
 }
+
+
+class NpcServantFollowerFlag(IntEnum):
+    NPC = 1
+    HIDE_SUPPORT = 2
+    NOT_USED_TREASURE_DEVICE = 4
+    NO_DISPLAY_BONUS_ICON = 8
+    APPLY_SVT_CHANGE = 16
+    HIDE_EQUIP = 32
+    NO_DISPLAY_BONUS_ICON_EQUIP = 64
+    HIDE_TREASURE_DEVICE_LV = 256
+    HIDE_TREASURE_DEVICE_DETAIL = 512
+    HIDE_RARITY = 1024
+
+
+class NiceNpcServantFollowerFlag(StrEnum):
+    """NPC Servant Follower Flag"""
+
+    npc = "npc"
+    hideSupport = "hideSupport"
+    notUsedTreasureDevice = "notUsedTreasureDevice"
+    noDisplayBonusIcon = "noDisplayBonusIcon"
+    applySvtChange = "applySvtChange"
+    hideEquip = "hideEquip"
+    noDisplayBonusIconEquip = "noDisplayBonusIconEquip"
+    hideTreasureDeviceLv = "hideTreasureDeviceLv"
+    hideTreasureDeviceDetail = "hideTreasureDeviceDetail"
+    hideRarity = "hideRarity"
+
+
+NPC_SERVANT_FOLLOWER_FLAG_NAME: dict[int, NiceNpcServantFollowerFlag] = {
+    1: NiceNpcServantFollowerFlag.npc,
+    2: NiceNpcServantFollowerFlag.hideSupport,
+    4: NiceNpcServantFollowerFlag.notUsedTreasureDevice,
+    8: NiceNpcServantFollowerFlag.noDisplayBonusIcon,
+    16: NiceNpcServantFollowerFlag.applySvtChange,
+    32: NiceNpcServantFollowerFlag.hideEquip,
+    64: NiceNpcServantFollowerFlag.noDisplayBonusIconEquip,
+    256: NiceNpcServantFollowerFlag.hideTreasureDeviceLv,
+    512: NiceNpcServantFollowerFlag.hideTreasureDeviceDetail,
+    1024: NiceNpcServantFollowerFlag.hideRarity,
+}
```

### Comparing `fgo_api_types-2023.4.27.0.39.38/fgo_api_types/nice.py` & `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     NiceFuncType,
     NiceGender,
     NiceGiftType,
     NiceItemType,
     NiceMissionProgressType,
     NiceMissionRewardType,
     NiceMissionType,
+    NiceNpcServantFollowerFlag,
     NicePayType,
     NicePurchaseType,
     NiceQuestAfterClearType,
     NiceQuestFlag,
     NiceQuestType,
     NiceRestrictionRangeType,
     NiceRestrictionType,
@@ -2256,14 +2257,15 @@
     lv: int
     atk: int
     hp: int
     traits: list[NiceTrait]
     skills: EnemySkill
     noblePhantasm: SupportServantTd
     limit: SupportServantLimit
+    flags: list[NiceNpcServantFollowerFlag]
 
 
 class SupportServant(BaseModelORJson):
     id: int
     priority: int
     name: str
     svt: BasicServant
```

### Comparing `fgo_api_types-2023.4.27.0.39.38/fgo_api_types/raw.py` & `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.27.0.39.38/fgo_api_types/rayshift.py` & `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.27.0.39.38/fgo_api_types/search.py` & `fgo_api_types-2023.4.29.17.3.6/fgo_api_types/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,14 +422,15 @@
     fieldAiId: Optional[int] = None
     enemySvtId: Optional[int] = None
     enemySvtAiId: Optional[int] = None
     enemyTrait: list[Union[Trait, int]] = Query([])
     enemyClassName: list[SvtClass] = Query([])
     enemySkillId: list[int] | None = Query(None)
     enemyNoblePhantasmId: list[int] | None = Query(None)
+    enemyScript: list[str] | None = Query(None, max_length=999)
 
     def hasSearchParams(self) -> bool:
         return any(
             [
                 self.name,
                 self.spotName,
                 self.warId,
@@ -441,14 +442,15 @@
                 self.enemySvtAiId,
                 self.enemySvtId,
                 self.fieldAiId,
                 self.enemyTrait,
                 self.enemyClassName,
                 self.enemySkillId,
                 self.enemyNoblePhantasmId,
+                self.enemyScript,
             ]
         )
 
     DESCRIPTION: ClassVar[str] = inspect.cleandoc(
         """
         Search and return the list of matched items.
 
@@ -463,14 +465,15 @@
         - **fieldAiId**: Field AI ID.
         - **enemySvtId**: Enemy's svt ID (Note that this is not `collectionNo`). Some quests use 99xxxxx svt ID instead of the playable svt ID.
         - **enemySvtAiId**: Enemy's servant AI ID.
         - **enemyTrait**: Enemy's Trait. Trait Enum or an Integer.
         - **enemyClassName**: Enemy's Class Name Enum.
         - **enemySkillId**: Enemy's Skill, Passive Skill,
         - **enemyNoblePhantasmId**: Enemy's NP
+        - **enemyScript**: JSON string of deckSvt's enemyScript to search. E.g. `enemyScript={"appear":1}`.
 
         At least one of the parameter is required for the query.
         """
     )
 
 
 @dataclass
```

### Comparing `fgo_api_types-2023.4.27.0.39.38/pyproject.toml` & `fgo_api_types-2023.4.29.17.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.04.27.00.39.38"
+version = "2023.04.29.17.03.06"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.4.27.0.39.38/PKG-INFO` & `fgo_api_types-2023.4.29.17.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.4.27.0.39.38
+Version: 2023.4.29.17.3.6
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

