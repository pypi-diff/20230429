# Comparing `tmp/rocketsim-0.2.4.tar.gz` & `tmp/rocketsim-0.3.0.tar.gz`

## Comparing `rocketsim-0.2.4.tar` & `rocketsim-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 rocketsim-0.2.4/Cargo.toml
--rw-r--r--   0     1001      123     1078 2023-02-27 02:18:43.000000 rocketsim-0.2.4/LICENSE
--rw-r--r--   0     1001      123     2352 2023-02-27 02:18:43.000000 rocketsim-0.2.4/README.md
--rw-r--r--   0     1001      123      664 2023-02-27 02:18:43.000000 rocketsim-0.2.4/pyproject.toml
--rw-r--r--   0     1001      123      195 2023-02-27 02:18:43.000000 rocketsim-0.2.4/rocketsim/__init__.py
--rw-r--r--   0     1001      123      670 2023-02-27 02:18:43.000000 rocketsim-0.2.4/rocketsim/__init__.pyi
--rw-r--r--   0     1001      123        0 2023-02-27 02:18:43.000000 rocketsim-0.2.4/rocketsim/py.typed
--rw-r--r--   0     1001      123       80 2023-02-27 02:18:43.000000 rocketsim-0.2.4/rocketsim/sim.py
--rw-r--r--   0     1001      123     2807 2023-02-27 02:18:43.000000 rocketsim-0.2.4/rocketsim/sim.pyi
--rw-r--r--   0     1001      123      916 2023-02-27 02:18:43.000000 rocketsim-0.2.4/src/lib.rs
--rw-r--r--   0     1001      123    22202 2023-02-27 02:18:43.000000 rocketsim-0.2.4/src/python.rs
--rw-r--r--   0     1001      123    29727 2023-02-27 02:18:43.000000 rocketsim-0.2.4/Cargo.lock
--rw-r--r--   0        0        0     3074 1970-01-01 00:00:00.000000 rocketsim-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 rocketsim-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123     1078 2023-04-29 18:12:40.000000 rocketsim-0.3.0/LICENSE
+-rw-r--r--   0     1001      123     2352 2023-04-29 18:12:40.000000 rocketsim-0.3.0/README.md
+-rw-r--r--   0     1001      123      664 2023-04-29 18:12:40.000000 rocketsim-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123      213 2023-04-29 18:12:40.000000 rocketsim-0.3.0/rocketsim/__init__.py
+-rw-r--r--   0     1001      123      854 2023-04-29 18:12:40.000000 rocketsim-0.3.0/rocketsim/__init__.pyi
+-rw-r--r--   0     1001      123        0 2023-04-29 18:12:40.000000 rocketsim-0.3.0/rocketsim/py.typed
+-rw-r--r--   0     1001      123       80 2023-04-29 18:12:40.000000 rocketsim-0.3.0/rocketsim/sim.py
+-rw-r--r--   0     1001      123     3378 2023-04-29 18:12:40.000000 rocketsim-0.3.0/rocketsim/sim.pyi
+-rw-r--r--   0     1001      123     3580 2023-04-29 18:12:40.000000 rocketsim-0.3.0/src/base.rs
+-rw-r--r--   0     1001      123      993 2023-04-29 18:12:40.000000 rocketsim-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123    17475 2023-04-29 18:12:40.000000 rocketsim-0.3.0/src/python.rs
+-rw-r--r--   0     1001      123     1528 2023-04-29 18:12:40.000000 rocketsim-0.3.0/src/state.rs
+-rw-r--r--   0     1001      123    33119 2023-04-29 18:12:40.000000 rocketsim-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     3074 1970-01-01 00:00:00.000000 rocketsim-0.3.0/PKG-INFO
```

### Comparing `rocketsim-0.2.4/LICENSE` & `rocketsim-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketsim-0.2.4/README.md` & `rocketsim-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rocketsim-0.2.4/pyproject.toml` & `rocketsim-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rocketsim-0.2.4/rocketsim/sim.pyi` & `rocketsim-0.3.0/rocketsim/sim.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 from enum import Enum
-from typing import Optional
+from typing import Optional, Tuple, Callable
 
-from rocketsim import Angle, Vec3
+from rocketsim import RotMat, Vec3
 
 class Team(Enum):
     Blue = 0
     Orange = 1
 
 class GameMode(Enum):
     Soccar = 0
+    TheVoid = 1
+
+class BallHitInfo:
+    relative_pos_on_ball: Vec3
+    ball_pos: Vec3
+    extra_hit_vel: Vec3
+    tick_count_when_hit: int
+    tick_count_when_extra_impulse_applied: int
+
+    def __init__() -> BallHitInfo: ...
+    def __str__(self) -> str: ...
 
 class Ball:
     pos: Vec3
     vel: Vec3
-    angvel: Vec3
+    ang_vel: Vec3
 
+    def __init__() -> Ball: ...
     def __str__(self) -> str: ...
 
-    def get_pos(self) -> Vec3: ...
-    def get_vel(self) -> Vec3: ...
-    def get_angvel(self) -> Vec3: ...
-
 class CarControls:
     throttle: float
     steer: float
     pitch: float
     yaw: float
     roll: float
     jump: bool
@@ -33,43 +41,47 @@
 
     def __init__(throttle: float = 0, steer: float = 0, pitch: float = 0, yaw: float = 0, roll: float = 0, jump: bool = False, boost: bool = False, handbrake: bool = False) -> CarControls: ...
     def __str__(self) -> str: ...
     def __repr__(self) -> str: ...
 
 class Car:
     pos: Vec3
+    rot_mat: RotMat
     vel: Vec3
-    angles: Angle
-    angvel: Vec3
-    last_rel_dodge_torque: Vec3
-    boost: float
-    time_spent_boosting: float
+    ang_vel: Vec3
     is_on_ground: bool
-    is_supersonic: bool
-    supersonic_time: float
-    is_jumping: bool
     has_jumped: bool
     has_double_jumped: bool
     has_flipped: bool
-    jump_timer: float
-    flip_timer: float
+    last_rel_dodge_torque: Vec3
+    jump_time: float
+    flip_time: float
+    is_jumping: bool
     air_time_since_jump: float
+    boost: float
+    time_spent_boosting: float
+    is_supersonic: bool
+    supersonic_time: float
+    handbrake_val: float
     is_auto_flipping: bool
     auto_flip_timer: float
     auto_flip_torque_scale: float
     has_contact: bool
-    handbrake_val: float
+    contact_normal: Vec3
+    other_car_id: int
+    cooldown_timer: float
+    is_demoed: bool
+    demo_respawn_timer: float
+    ball_hit_info: BallHitInfo
     last_controls: CarControls
 
+    def __init__() -> Car: ...
     def __str__(self) -> str: ...
-    def get_pos(self) -> Vec3: ...
-    def get_vel(self) -> Vec3: ...
-    def get_angles(self) -> Angle: ...
-    def get_angvel(self) -> Vec3: ...
-    def get_last_rel_dodge_torque(self) -> Vec3: ...
+
+    def get_contacting_car(self, arena: Arena) -> Optional[Car]: ...
 
 class CarConfig(Enum):
     Octane = 0
     Dominus = 1
     Plank = 2
     Breakout = 3
     Hybrid = 4
@@ -78,32 +90,38 @@
 class BoostPad:
     pos: Vec3
     is_big: bool
 
     def __str__(self) -> str: ...
 
 class BoostPadState:
-    id: int
     is_active: bool
     cooldown: float
+    cur_locked_car_id: int
+    prev_locked_car_id: int
 
-    def __init__(id: int, is_active: bool, cooldown: float) -> BoostPadState: ...
+    def __init__(is_active: bool, cooldown: float, cur_locked_car_id: int, prev_locked_car_id: int) -> BoostPadState: ...
     def __str__(self) -> str: ...
     def __repr__(self) -> str: ...
 
 class Arena:
-    ball: Ball
-
     def __init__(gamemode: Optional[GameMode] = GameMode.Soccar, tick_rate: Optional[float] = 120) -> Arena: ...
     def get_tick_rate(self) -> float: ...
+    def get_tick_count(self) -> int: ...
+    def step(self, ticks_to_simulate: int = 1): ...
+
     def get_ball(self) -> Ball: ...
+    def set_ball(self, ball: Ball): ...
+    def get_ball_rotation(self) -> RotMat: ...
+
     def num_cars(self) -> int: ...
-    def get_car_from_index(self, index: int) -> Car: ...
-    def get_car_id_from_index(self, index: int) -> int: ...
     def add_car(self, team: Team, config: CarConfig) -> int: ...
     def get_car(self, id: int) -> Car: ...
     def set_car(self, id: int, car: Car): ...
     def set_car_controls(self, id: int, controls: CarControls): ...
+    def set_all_controls(self, controls: list[Tuple[int, CarControls]]): ...
+
     def num_pads(self) -> int: ...
-    def get_pad_static(self, id: int) -> BoostPad: ...
-    def get_pad_state(self, id: int) -> BoostPadState: ...
-    def step(self, ticks_to_simulate: int = 1): ...
+    def get_pad_static(self, index: int) -> BoostPad: ...
+    def get_pad_state(self, index: int) -> BoostPadState: ...
+    def set_pad_state(self, index: int, boost_pad: BoostPadState): ...
+    def set_goal_scored_callback(self, callback: Callable[[Team], None]): ...
```

### Comparing `rocketsim-0.2.4/src/lib.rs` & `rocketsim-0.3.0/src/lib.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+mod base;
 mod python;
+mod state;
 
+use base::*;
 use pyo3::prelude::*;
 use python::*;
+use state::*;
 
 macro_rules! pynamedmodule {
     (doc: $doc:literal, name: $name:tt, funcs: [$($func_name:path),*], classes: [$($class_name:ident),*], submodules: [$($submodule_name:ident),*]) => {
         #[doc = $doc]
         #[pymodule]
         #[allow(unused_variables)]
         #[allow(redundant_semicolons)]
@@ -18,18 +22,18 @@
     };
 }
 
 pynamedmodule! {
     doc: "",
     name: sim,
     funcs: [],
-    classes: [Arena, GameMode, Team, CarConfig, Car, Ball, CarControls],
+    classes: [Arena, GameMode, Team, CarConfig, Car, Ball, CarControls, BallHitInfo],
     submodules: []
 }
 
 pynamedmodule! {
     doc: "",
     name: rocketsim,
-    funcs: [],
-    classes: [Vec3, Angle],
+    funcs: [init],
+    classes: [Vec3, RotMat, GameState],
     submodules: [sim]
 }
```

### Comparing `rocketsim-0.2.4/Cargo.lock` & `rocketsim-0.3.0/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -26,56 +26,56 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "aquamarine"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a941c39708478e8eea39243b5983f1c42d2717b3620ee91f4a52115fd02ac43f"
 dependencies = [
  "itertools 0.9.0",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
- "hermit-abi",
+ "hermit-abi 0.1.19",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "autocxx"
-version = "0.24.0"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c3621dadf601792243257fe956578abed662504c296e22f537433381a9a8026"
+checksum = "9a19c80ba8384f11f11024462523829c2989a3fd7afb8ac70637abdd25bd3b8a"
 dependencies = [
  "aquamarine",
  "autocxx-macro",
  "cxx",
  "moveit",
 ]
 
@@ -94,35 +94,35 @@
  "log",
  "peeking_take_while",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn",
+ "syn 1.0.109",
  "which",
 ]
 
 [[package]]
 name = "autocxx-build"
-version = "0.24.0"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc5ed44575f2fc241b990e03909634301c9c49f1ff3d921631fdca752c33e297"
+checksum = "37823c07a43c1a8d09aaad7ba8785df1b3160dcf0ee1c4e7e83177e9ebc2d804"
 dependencies = [
  "autocxx-engine",
  "env_logger",
  "indexmap",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "autocxx-engine"
-version = "0.24.0"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf6a27d1fcc45584c0b7fe5ce06b7b26cefe72cfa55e5a94264be5e427a418e3"
+checksum = "aa19cbb6614361e61806db4526bd373415dfe0cb95f6bf811a2ddbd6fa4a8115"
 dependencies = [
  "aquamarine",
  "autocxx-bindgen",
  "autocxx-parser",
  "cc",
  "cxx-gen",
  "indexmap",
@@ -134,48 +134,48 @@
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustversion",
  "serde_json",
  "strum_macros",
- "syn",
+ "syn 1.0.109",
  "tempfile",
  "thiserror",
  "version_check",
 ]
 
 [[package]]
 name = "autocxx-macro"
-version = "0.24.0"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6022ff3a7c5d5cf54cf37f3dabb54c1bdcbeecb3fab3937903dd0bc562ef7fb6"
+checksum = "7313f823cd7e017cf80b46254d9bd78e4cb86b33b7e2cd08e1af312ee7bc77cf"
 dependencies = [
  "autocxx-parser",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "autocxx-parser"
-version = "0.24.0"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "884eef6d9cc6d89a2ca043fad1c17424f857c6082db4122dc7f2fb7e5ec5ff74"
+checksum = "a16532d5349c8f165534d95ce2cf70a4aefaf1f33146fe8273f77d3a2f817796"
 dependencies = [
  "indexmap",
  "itertools 0.10.5",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
  "serde",
  "serde_json",
- "syn",
+ "syn 1.0.109",
  "thiserror",
 ]
 
 [[package]]
 name = "backtrace"
 version = "0.3.67"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -187,14 +187,23 @@
  "libc",
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
+name = "backtrace-ext"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "537beee3be4a18fb023b570f80e3ae28003db9167a751266b259926e25539d50"
+dependencies = [
+ "backtrace",
+]
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "cc"
@@ -215,17 +224,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clang-sys"
-version = "1.6.0"
+version = "1.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ed9a53e5d4d9c573ae844bfac6872b159cb1d1585a83b29e7a64b7eef7332a"
+checksum = "c688fc74432808e3eb684cae8830a86be1d66a2bd58e1f248ed0960a590baf6f"
 dependencies = [
  "glob",
  "libc",
  "libloading",
 ]
 
 [[package]]
@@ -236,51 +245,51 @@
 dependencies = [
  "termcolor",
  "unicode-width",
 ]
 
 [[package]]
 name = "cxx"
-version = "1.0.91"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86d3488e7665a7a483b57e25bdd90d0aeb2bc7608c8d0346acf2ad3f1caf1d62"
+checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
 dependencies = [
  "cc",
  "cxxbridge-flags",
  "cxxbridge-macro",
  "link-cplusplus",
 ]
 
 [[package]]
 name = "cxx-gen"
-version = "0.7.91"
+version = "0.7.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "406f2c382fded54902d17a552e7a221121fc5cc2abc39653b323394117330feb"
+checksum = "ee165c38de64e6761c2f38b7e9beee0721110f8585165987ef9db2a753ee4176"
 dependencies = [
  "codespan-reporting",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
-version = "1.0.91"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2ef98b8b717a829ca5603af80e1f9e2e48013ab227b68ef37872ef84ee479bf"
+checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
 
 [[package]]
 name = "cxxbridge-macro"
-version = "1.0.91"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "086c685979a698443656e5cf7856c95c642295a38599f12fb1ff76fb28d19892"
+checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
@@ -296,21 +305,21 @@
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
 name = "errno"
-version = "0.2.8"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "winapi",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -326,30 +335,36 @@
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "gimli"
 version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad0a93d233ebf96623465aad4046a8d3aa4da22d4f4beba5388838c8a434bbb4"
 
 [[package]]
+name = "glam"
+version = "0.23.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e4afd9ad95555081e109fe1d21f2a30c691b5f0919c67dfa690a2e1eb6bd51c"
+
+[[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "hashbrown"
@@ -372,24 +387,30 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "hermit-abi"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+
+[[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
  "serde",
 ]
 
 [[package]]
@@ -405,20 +426,33 @@
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.5"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1abeb7a0dd0f8181267ff8adc397075586500b81b28a73e8a0208b00fc170fb3"
+checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
 dependencies = [
+ "hermit-abi 0.3.1",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "is-terminal"
+version = "0.4.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+dependencies = [
+ "hermit-abi 0.3.1",
+ "io-lifetimes",
+ "rustix",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "is_ci"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "616cde7c720bb2bb5824a224687d8f77bfd38922027f01d825cd7453be5099fb"
@@ -439,17 +473,17 @@
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.5"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
@@ -457,17 +491,17 @@
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libloading"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
@@ -482,17 +516,17 @@
 checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.1.4"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
+checksum = "36eb31c1778188ae1e64398743890d0877fef36d11521ac60406b42016e8c2cf"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -522,41 +556,42 @@
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miette"
-version = "5.5.0"
+version = "5.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4afd9b301defa984bbdbe112b4763e093ed191750a0d914a78c1106b2d0fe703"
+checksum = "92a992891d5579caa9efd8e601f82e30a1caa79a27a5db075dde30ecb9eab357"
 dependencies = [
- "atty",
  "backtrace",
+ "backtrace-ext",
+ "is-terminal",
  "miette-derive",
  "once_cell",
  "owo-colors",
  "supports-color",
  "supports-hyperlinks",
  "supports-unicode",
  "terminal_size",
  "textwrap",
  "thiserror",
  "unicode-width",
 ]
 
 [[package]]
 name = "miette-derive"
-version = "5.5.0"
+version = "5.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97c2401ab7ac5282ca5c8b518a87635b1a93762b0b90b9990c509888eeccba29"
+checksum = "4c65c625186a9bcce6699394bee511e1b1aec689aa7e3be1bf4e996e75834153"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
@@ -624,45 +659,45 @@
 name = "parking_lot_core"
 version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "peeking_take_while"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
 
 [[package]]
 name = "prettyplease"
-version = "0.1.23"
+version = "0.1.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e97e3215779627f01ee256d2fad52f3d95e8e1c11e9fc6fd08f7cd455d5d5c78"
+checksum = "6c8646e95016a7a6c4adea95bafa8a16baab64b583356217f2c85db4a39d9a86"
 dependencies = [
  "proc-macro2",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro-error-attr"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -671,206 +706,216 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "rocketsim"
-version = "0.2.4"
+version = "0.3.0"
 dependencies = [
  "pyo3",
  "rocketsim_rs",
 ]
 
 [[package]]
 name = "rocketsim_rs"
-version = "0.4.3"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86a8b04bbdd2b30e479a27d8367da21a527e65ac676ec42040cfde39c3f69427"
+checksum = "13a8973b1236905de3be29252a67974552d0d338f5d4287cdafd1884ea643933"
 dependencies = [
  "autocxx",
  "autocxx-build",
  "cxx",
+ "glam",
  "glob",
  "miette",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.21"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ef03e0a2b150c7a90d01faf6254c9c48a41e95fb2a8c2ac1c6f0d2b9aefc342"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.36.8"
+version = "0.37.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f43abb88211988493c1abb44a70efa56ff0ce98f233b7b276146f1f3f7ba9644"
+checksum = "a0661814f891c57c930a610266415528da53c4933e6dea5fb350cbfe048a9ece"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.11"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5583e89e108996506031660fe09baa5011b9dd0341b89029313006d1fb508d70"
+checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
 
 [[package]]
 name = "ryu"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b4b9743ed687d4b4bcedf9ff5eaa7398495ae14e61cba0a295704edbc7decde"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.152"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.93"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cad406b69c91885b5107daf2c29572f6c8cdb3c66826821e286c533490c0bc76"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -897,73 +942,84 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e385be0d24f186b4ce2f9982191e7101bb737312ad61c1f2f984f34bcf85d59"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "supports-color"
-version = "1.3.1"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ba6faf2ca7ee42fdd458f4347ae0a9bd6bcc445ad7cb57ad82b383f18870d6f"
+checksum = "4950e7174bffabe99455511c39707310e7e9b440364a2fcb1cc21521be57b354"
 dependencies = [
- "atty",
+ "is-terminal",
  "is_ci",
 ]
 
 [[package]]
 name = "supports-hyperlinks"
-version = "1.2.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "590b34f7c5f01ecc9d78dba4b3f445f31df750a67621cf31626f3b7441ce6406"
+checksum = "f84231692eb0d4d41e4cdd0cabfdd2e6cd9e255e65f80c9aa7c98dd502b4233d"
 dependencies = [
- "atty",
+ "is-terminal",
 ]
 
 [[package]]
 name = "supports-unicode"
-version = "1.0.2"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8b945e45b417b125a8ec51f1b7df2f8df7920367700d1f98aedd21e5735f8b2"
+checksum = "4b6c2cb240ab5dd21ed4906895ee23fe5a48acdbd15a3ce388e7b62a9b66baf7"
 dependencies = [
- "atty",
+ "is-terminal",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
-version = "3.4.0"
+version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af18f7ae1acd354b992402e9ec5864359d693cd8a79dcbef59f76891701c1e95"
+checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
  "cfg-if",
  "fastrand",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "rustix",
- "windows-sys 0.42.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
@@ -990,37 +1046,37 @@
  "smawk",
  "unicode-linebreak",
  "unicode-width",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fb327af4685e4d03fa8cbcf1716380da910eeb2bb8be417e7f9fd3fb164f36f"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unicode-linebreak"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5faade31a542b8b35855fff6e8def199853b2da8da256da52f52f1316ee3137"
 dependencies = [
@@ -1092,85 +1148,136 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows-targets 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows-targets",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `rocketsim-0.2.4/PKG-INFO` & `rocketsim-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketsim
-Version: 0.2.4
+Version: 0.3.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
```

