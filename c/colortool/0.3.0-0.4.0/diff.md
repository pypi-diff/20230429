# Comparing `tmp/colortool-0.3.0.tar.gz` & `tmp/colortool-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colortool-0.3.0.tar", last modified: Sun Jan 22 22:42:05 2023, max compression
+gzip compressed data, was "colortool-0.4.0.tar", last modified: Sat Apr 29 10:46:44 2023, max compression
```

## Comparing `colortool-0.3.0.tar` & `colortool-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 22:42:05.898690 colortool-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-01-22 22:42:05.898690 colortool-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-01-22 22:41:56.000000 colortool-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 22:42:05.898690 colortool-0.3.0/colortool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-01-22 22:42:05.000000 colortool-0.3.0/colortool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-22 22:42:05.000000 colortool-0.3.0/colortool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 22:42:05.000000 colortool-0.3.0/colortool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-22 22:42:05.000000 colortool-0.3.0/colortool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-22 22:42:05.000000 colortool-0.3.0/colortool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-01-22 22:41:56.000000 colortool-0.3.0/colortool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-01-22 22:42:05.898690 colortool-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-22 22:41:56.000000 colortool-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:46:44.240223 colortool-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-29 10:46:44.240223 colortool-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-29 10:46:29.000000 colortool-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:46:44.240223 colortool-0.4.0/colortool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-29 10:46:44.000000 colortool-0.4.0/colortool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-29 10:46:44.000000 colortool-0.4.0/colortool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:46:44.000000 colortool-0.4.0/colortool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 10:46:44.000000 colortool-0.4.0/colortool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 10:46:44.000000 colortool-0.4.0/colortool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-29 10:46:29.000000 colortool-0.4.0/colortool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-29 10:46:29.000000 colortool-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 10:46:44.240223 colortool-0.4.0/setup.cfg
```

### Comparing `colortool-0.3.0/PKG-INFO` & `colortool-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,88 @@
-Metadata-Version: 2.1
-Name: colortool
-Version: 0.3.0
-Summary: set of tools to work with different color formats
-Home-page: https://github.com/tandav/colortool
-Author: Alexander Rodionov
-Author-email: tandav@tandav.me
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # colortool
 set of tools to work with different color formats
 
 ## install from [pypi](https://pypi.org/project/colortool/)
 ```shell
 pip install colortool
 ```
 
 ## examples
 ```python
 >>> from colortool import Color
 
-# convert color to different formats
+```
+
+### convert color to different formats
+```python
 >>> green = Color.from_hex(0x00FF00)
 >>> green.css_hex
 '#00FF00'
 >>> green.rgb_int
 (0, 255, 0)
 >>> green.rgb_float
 (0.0, 1.0, 0.0)
 >>> green.hsl
-(0.3333333333333333, 1.0, 0.5)
+(0.33333333333333, 1.0, 0.5)
+
+```
 
-# create color from different formats
+### create color from different formats
+```python
 >>> Color.from_css_hex('#00FF00')
 Color(0x00FF00)
 >>> Color.from_rgb_int((0, 255, 0))
 Color(0x00FF00)
 >>> Color.from_rgb_float((0.0, 1.0, 0.0))
 Color(0x00FF00)
 >>> Color.from_hsl((0.3333333333333333, 1.0, 0.5))
 Color(0x00FF00)
 
-# rgba colors
+```
+
+### rgba colors
+```python
 >>> Color.from_rgba_int_float((0, 255, 0, 0.5))
 Color(0x00FF00, alpha=0.5)
 
 >>> Color.from_rgba_int_float((0, 255, 0, 0.5)).css_rgba
 'rgba(0, 255, 0, 0.5)'
 
-# convert RGBA color on RGB background to RGB color
+```
+
+```python
+### convert RGBA color on RGB background to RGB color
 >>> Color.from_background_and_color_alpha(
-        background=Color.from_hex(0x00FF00),
-        color=Color(0x000000, alpha=0.5),
-    )
+...     background=Color.from_hex(0x00FF00),
+...     color=Color(0x000000,alpha=0.5),
+... )
 Color(0x007F00)
 
-# make color darker or lighter
+```
+
+### make color darker or lighter
+```python
 >>> green.darker(ratio=0.5) # lightness = lightness * ratio
 Color(0x007F00)
 >>> green.lighter(ratio=0.5) # lightness = lightness + (1 - lightness) * ratio
 Color(0x7FFF7F)
 
-#  determine the font color to be either black or white depending on the background color
-# https://css-tricks.com/switch-font-color-for-different-backgrounds-with-css/
+```
+###  [determine the font color to be either black or white depending on the background color](https://css-tricks.com/switch-font-color-for-different-backgrounds-with-css/)
+```python
 >>> white = Color.from_hex(0xFFFFFF)
 >>> black = Color.from_hex(0x000000)
 >>> white.font_color()
 Color(0x000000)
 >>> black.font_color()
 Color(0xFFFFFF)
 >>> green.font_color()
 Color(0x000000)
 
-# also return darker variation of color if it is really light (see same css-tricks article)
+```
+
+### also return darker variation of color if it is really light (see same css-tricks article)
+```python
 >>> green.font_border_colors()
 (Color(0x000000), Color(0x00FF00))
+
 ```
```

### Comparing `colortool-0.3.0/colortool.egg-info/PKG-INFO` & `colortool-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: colortool
-Version: 0.3.0
+Version: 0.4.0
 Summary: set of tools to work with different color formats
-Home-page: https://github.com/tandav/colortool
-Author: Alexander Rodionov
-Author-email: tandav@tandav.me
+Author-email: Alexander Rodionov <tandav@tandav.me>
+Project-URL: source, https://github.com/tandav/colortool
+Project-URL: issues, https://tandav.github.io/colortool/issues
+Project-URL: release notes, https://tandav.github.io/colortool/releases
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # colortool
 set of tools to work with different color formats
 
@@ -17,63 +18,83 @@
 pip install colortool
 ```
 
 ## examples
 ```python
 >>> from colortool import Color
 
-# convert color to different formats
+```
+
+### convert color to different formats
+```python
 >>> green = Color.from_hex(0x00FF00)
 >>> green.css_hex
 '#00FF00'
 >>> green.rgb_int
 (0, 255, 0)
 >>> green.rgb_float
 (0.0, 1.0, 0.0)
 >>> green.hsl
-(0.3333333333333333, 1.0, 0.5)
+(0.33333333333333, 1.0, 0.5)
 
-# create color from different formats
+```
+
+### create color from different formats
+```python
 >>> Color.from_css_hex('#00FF00')
 Color(0x00FF00)
 >>> Color.from_rgb_int((0, 255, 0))
 Color(0x00FF00)
 >>> Color.from_rgb_float((0.0, 1.0, 0.0))
 Color(0x00FF00)
 >>> Color.from_hsl((0.3333333333333333, 1.0, 0.5))
 Color(0x00FF00)
 
-# rgba colors
+```
+
+### rgba colors
+```python
 >>> Color.from_rgba_int_float((0, 255, 0, 0.5))
 Color(0x00FF00, alpha=0.5)
 
 >>> Color.from_rgba_int_float((0, 255, 0, 0.5)).css_rgba
 'rgba(0, 255, 0, 0.5)'
 
-# convert RGBA color on RGB background to RGB color
+```
+
+```python
+### convert RGBA color on RGB background to RGB color
 >>> Color.from_background_and_color_alpha(
-        background=Color.from_hex(0x00FF00),
-        color=Color(0x000000, alpha=0.5),
-    )
+...     background=Color.from_hex(0x00FF00),
+...     color=Color(0x000000,alpha=0.5),
+... )
 Color(0x007F00)
 
-# make color darker or lighter
+```
+
+### make color darker or lighter
+```python
 >>> green.darker(ratio=0.5) # lightness = lightness * ratio
 Color(0x007F00)
 >>> green.lighter(ratio=0.5) # lightness = lightness + (1 - lightness) * ratio
 Color(0x7FFF7F)
 
-#  determine the font color to be either black or white depending on the background color
-# https://css-tricks.com/switch-font-color-for-different-backgrounds-with-css/
+```
+###  [determine the font color to be either black or white depending on the background color](https://css-tricks.com/switch-font-color-for-different-backgrounds-with-css/)
+```python
 >>> white = Color.from_hex(0xFFFFFF)
 >>> black = Color.from_hex(0x000000)
 >>> white.font_color()
 Color(0x000000)
 >>> black.font_color()
 Color(0xFFFFFF)
 >>> green.font_color()
 Color(0x000000)
 
-# also return darker variation of color if it is really light (see same css-tricks article)
+```
+
+### also return darker variation of color if it is really light (see same css-tricks article)
+```python
 >>> green.font_border_colors()
 (Color(0x000000), Color(0x00FF00))
+
 ```
```

### Comparing `colortool-0.3.0/colortool.py` & `colortool-0.4.0/colortool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from __future__ import annotations
 
 import colorsys
 import functools
+import math
 import random
 import string
+import typing as tp
 
-__version__ = '0.3.0'
+from dsplib.scale import minmax_scaler
 
-Float3 = tuple[float, float, float]
-Float4 = tuple[float, float, float, float]
-Int3 = tuple[int, int, int]
-Int4 = tuple[int, int, int, int]
-Int3Float = tuple[int, int, int, float]
+__version__ = '0.4.0'
+
+Float3 = tp.Tuple[float, float, float]
+Float4 = tp.Tuple[float, float, float, float]
+Int3 = tp.Tuple[int, int, int]
+Int4 = tp.Tuple[int, int, int, int]
+Int3Float = tp.Tuple[int, int, int, float]
 
 
 def is_css_hex_color(v: str) -> bool:
     return len(v) == 7 and v.startswith('#') and set(v[1:]) <= set(string.hexdigits)
 
 
 class Color:
     """
     supported formats:
     hex, css_hex, rgb_int, rgb_float, hls
     """
 
     def __init__(self, color: int, alpha: float | None = None):
-        if not (0 <= color <= 0xFFFFFF):
+        if not 0 <= color <= 0xFFFFFF:
             raise ValueError('color must be in range [0, 0xFFFFFF]')
-        if alpha is not None and not (0 <= alpha <= 1):
+        if alpha is not None and not 0 <= alpha <= 1:
             raise ValueError('alpha must be in range [0, 1]')
         self.color = color
         self.alpha = alpha
 
     def __repr__(self) -> str:
         if self.alpha is None:
             return f'Color(0x{self.color:06X})'
@@ -169,15 +173,15 @@
         if self.alpha is None:
             raise ValueError('alpha is None')
         return f'rgba{self.rgba_int_float}'
 
     @functools.cached_property
     def hsl(self) -> Float3:
         h, l, s = colorsys.rgb_to_hls(*self.rgb_float)
-        return h, s, l
+        return round(h, 14), round(s, 14), round(l, 14)
 
     def lighter(self, ratio: float = 0.5) -> Color:
         h, s, l = self.hsl
         return Color.from_hsl((h, s, l + (1 - l) * ratio))
 
     def darker(self, ratio: float = 0.5) -> Color:
         h, s, l = self.hsl
@@ -187,38 +191,57 @@
         """
         determine the font color to be either black or white depending on the background color
         https://css-tricks.com/switch-font-color-for-different-backgrounds-with-css/
 
         :param threshold: 0..1 float. lightness value below the threshold will result in white, any above will result in black
         :return: font_color in css hex string format
         """
-        h, s, l = self.hsl
+        h, s, l = self.hsl  # pylint: disable=unused-variable
         return WHITE_BRIGHT if l < threshold else BLACK_BRIGHT
 
     def font_border_colors(
         self,
         font_threshold: float = 0.5,
         border_threshold: float = 0.9,
-    ) -> tuple[Color, Color]:
+    ) -> tp.Tuple[Color, Color]:
         """
         determine the font color to be either black or white depending on the background color
         https://css-tricks.com/switch-font-color-for-different-backgrounds-with-css/
 
         :param color: hex string in #4bb9ac format
         :param font_threshold: 0..1 float. lightness value below the threshold will result in white, any above will result in black
         :param border_threshold: 0..1 float. lightness value below the threshold will result the border-color as same, any above 30% darker shade of the same color
         :return: font_color, border_color in css hex string format #4bb9ac
         """
-        # rgb = to_rgb_float(to_rgb_int(color))
-        # h, l, s = colorsys.rgb_to_hls(*rgb)
         h, s, l = self.hsl
         border_color = self if l < border_threshold else Color.from_hsl((h, s, l * 0.7))
         return self.font_color(font_threshold), border_color
 
 
+class Gradient:
+    def __init__(self, colors: tp.List[Color]) -> None:
+        self.colors = colors
+
+    def __call__(self, i: float) -> Color:
+        if not 0 <= i <= 1:
+            raise ValueError('i must be in 0..1 range')
+        j = minmax_scaler(i, 0, 1, 0, len(self.colors) - 1)
+        ja = int(j)
+        jb = min(ja + 1, len(self.colors) - 1)
+        k, _ = math.modf(j)
+        kb = minmax_scaler(k, 0, 1, 0, 0xFF)
+        rgb_a = self.colors[ja].rgb_int
+        rgb_b = self.colors[jb].rgb_int
+        rgb = tuple(
+            int(minmax_scaler(kb, 0, 0xFF, channel_a, channel_b))
+            for channel_a, channel_b in zip(rgb_a, rgb_b)
+        )
+        return Color.from_rgb_int(rgb)  # type: ignore[arg-type]
+
+
 WHITE_BRIGHT = Color.from_hex(0xFFFFFF)
 BLACK_BRIGHT = Color.from_hex(0x000000)
 MAGENTA = Color.from_hex(0x4457e5)
 RED = Color.from_hex(0xFF0000)
 GREEN = Color.from_hex(0x00FF00)
 BLUE = Color.from_hex(0x4f88ea)
 RED_PALE = Color.from_hex(0xe2c5c5)
```

