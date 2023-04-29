# Comparing `tmp/psd_export-1.0.8.tar.gz` & `tmp/psd_export-1.0.9.tar.gz`

## Comparing `psd_export-1.0.8.tar` & `psd_export-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 psd_export-1.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psd_export-1.0.8/src/psd_export/__init__.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 psd_export-1.0.8/src/psd_export/blendfuncs.py
--rw-r--r--   0        0        0    21901 2020-02-02 00:00:00.000000 psd_export-1.0.8/src/psd_export/composite.py
--rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 psd_export-1.0.8/src/psd_export/export.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 psd_export-1.0.8/src/psd_export/filters.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 psd_export-1.0.8/src/psd_export/util.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 psd_export-1.0.8/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 psd_export-1.0.8/LICENSE
--rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 psd_export-1.0.8/README.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 psd_export-1.0.8/pyproject.toml
--rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 psd_export-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 psd_export-1.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psd_export-1.0.9/src/psd_export/__init__.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 psd_export-1.0.9/src/psd_export/blendfuncs.py
+-rw-r--r--   0        0        0    23098 2020-02-02 00:00:00.000000 psd_export-1.0.9/src/psd_export/composite.py
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 psd_export-1.0.9/src/psd_export/export.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 psd_export-1.0.9/src/psd_export/filters.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 psd_export-1.0.9/src/psd_export/util.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 psd_export-1.0.9/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 psd_export-1.0.9/LICENSE
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 psd_export-1.0.9/README.md
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 psd_export-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 psd_export-1.0.9/PKG-INFO
```

### Comparing `psd_export-1.0.8/.github/workflows/python-publish.yml` & `psd_export-1.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.8/src/psd_export/blendfuncs.py` & `psd_export-1.0.9/src/psd_export/blendfuncs.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.8/src/psd_export/composite.py` & `psd_export-1.0.9/src/psd_export/composite.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,16 +155,18 @@
     flat_list = flattened_tree(layer)
     for sublayer in layer.descendants():
         sublayer.visibility_dependency = get_visibility_dependency(sublayer, possible_dependencies(sublayer, flat_list))
         if sublayer.custom_op is not None:
             sublayer.custom_op_barrier = asyncio.Barrier(tile_count)
             sublayer.custom_op_condition = asyncio.Condition()
             sublayer.custom_op_finished = False
-            sublayer.custom_op_color = np.zeros(size + (3,), dtype=dtype)
-            sublayer.custom_op_alpha = np.zeros(size + (1,), dtype=dtype)
+            sublayer.custom_op_color_dst = np.zeros(size + (3,), dtype=dtype)
+            sublayer.custom_op_color_src = np.zeros(size + (3,), dtype=dtype)
+            sublayer.custom_op_alpha_dst = np.zeros(size + (1,), dtype=dtype)
+            sublayer.custom_op_alpha_src = np.zeros(size + (1,), dtype=dtype)
 
 def increment_get_counter(counter, key):
     counter[key] += 1
 
 def decrement_get_counter(counter, cache, key):
     counter[key] -= 1
     if counter[key] == 0:
@@ -336,43 +338,60 @@
                 next_backdrop = None
                 if blend_mode == BlendMode.PASS_THROUGH:
                     next_backdrop = (color_dst, alpha_dst)
                 color_src, alpha_src = await composite_group_layer(sublayer, size, offset, next_backdrop)
             else:
                 color_src, alpha_src = await get_pixel_layer_data(sublayer, size, offset)
 
-            # Empty tile, can just ignore.
-            if color_src is None:
-                set_cached_composite(sublayer, offset, (color_dst, alpha_dst))
-                if sublayer.custom_op is not None:
-                    await barrier_skip(sublayer.custom_op_barrier)
-                # Need to enter the clip layers to make sure any barriers are hit.
-                if sublayer.clip_layers:
-                    await composite_group_layer(sublayer.clip_layers, size, offset)
-                continue
-
-            # Perform custom filter over the current color_dst
+            # Perform custom filter over the current src and dst
             if sublayer.custom_op is not None:
-                if not np.isscalar(color_dst):
-                    await peval(lambda: blit(sublayer.custom_op_color, color_dst, offset))
-                    await peval(lambda: blit(sublayer.custom_op_alpha, alpha_src, offset))
+                def ensure_array(src, shape):
+                    if src is None or np.isscalar(src):
+                        return np.zeros(shape, dtype=dtype)
+                    else:
+                        return src.copy()
+                color_dst = ensure_array(color_dst, size + (3,))
+                color_src = ensure_array(color_src, size + (3,))
+                alpha_dst = ensure_array(alpha_dst, size + (1,))
+                alpha_src = ensure_array(alpha_src, size + (1,))
+                await peval(lambda: blit(sublayer.custom_op_color_dst, color_dst, offset))
+                await peval(lambda: blit(sublayer.custom_op_color_src, color_src, offset))
+                await peval(lambda: blit(sublayer.custom_op_alpha_dst, alpha_dst, offset))
+                await peval(lambda: blit(sublayer.custom_op_alpha_src, alpha_src, offset))
                 await sublayer.custom_op_barrier.wait()
                 if not sublayer.custom_op_condition.locked():
                     if not sublayer.custom_op_finished:
                         async with sublayer.custom_op_condition:
-                            sublayer.custom_op_color, sublayer.custom_op_alpha = \
-                                await peval(lambda: sublayer.custom_op(sublayer.custom_op_color, sublayer.custom_op_alpha))
+                            sublayer.custom_op_color_dst, sublayer.custom_op_alpha_dst = \
+                                await peval(lambda: sublayer.custom_op(
+                                    sublayer.custom_op_color_dst,
+                                    sublayer.custom_op_color_src,
+                                    sublayer.custom_op_alpha_dst,
+                                    sublayer.custom_op_alpha_src))
                             sublayer.custom_op_finished = True
                             sublayer.custom_op_condition.notify_all()
                 else:
                     async with sublayer.custom_op_condition:
                         await sublayer.custom_op_condition.wait_for(lambda: sublayer.custom_op_finished)
                 neg_offset = -np.array(offset)
-                await peval(lambda: blit(color_src, sublayer.custom_op_color, neg_offset))
-                await peval(lambda: blit(alpha_src, sublayer.custom_op_alpha, neg_offset))
+                await peval(lambda: blit(color_dst, sublayer.custom_op_color_dst, neg_offset))
+                await peval(lambda: blit(alpha_dst, sublayer.custom_op_alpha_dst, neg_offset))
+                if not is_counter_zero(sublayer):
+                    set_cached_composite(sublayer, offset, (color_dst, alpha_dst))
+                continue
+
+            # Empty tile, can just ignore.
+            if color_src is None:
+                set_cached_composite(sublayer, offset, (color_dst, alpha_dst))
+                if sublayer.custom_op is not None:
+                    await barrier_skip(sublayer.custom_op_barrier)
+                # Need to enter the clip layers to make sure any barriers are hit.
+                if sublayer.clip_layers:
+                    await composite_group_layer(sublayer.clip_layers, size, offset)
+                continue
 
             # Opacity is actually FILL when special mode is true!
             opacity, special_mode = get_sai_special_mode_opacity(sublayer.layer)
 
             # A pass-through layer has already been blended, so just lerp instead.
             # NOTE: Clipping layers do not apply to pass layers, as if clipping were simply disabled.
             if blend_mode == BlendMode.PASS_THROUGH:
```

### Comparing `psd_export-1.0.8/src/psd_export/export.py` & `psd_export-1.0.9/src/psd_export/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
     # Configure tagged layers
     for layer in psd.descendants():
         custom_ops = []
         def add_op(tag):
             custom_op = filters.get_filter(tag.name)
             if custom_op:
-                custom_ops.append(lambda c, a: custom_op(c, a, *tag.args))
+                custom_ops.append(lambda *args: custom_op(*args, *tag.args))
 
         for tag in layer.tags:
             if not tag.ignore:
                 layer.visible = False
         for tag in layer.tags:
             if tag.ignore:
                 add_op(tag)
```

### Comparing `psd_export-1.0.8/src/psd_export/filters.py` & `psd_export-1.0.9/src/psd_export/filters.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,57 +13,62 @@
 
 def get_filter(name):
     return filter_names.get(name, None)
 
 def compose_ops(ops):
     if not ops:
         return None
-    def c(color, alpha):
+    def c(color_dst, color_src, alpha_dst, alpha_src):
         for op in ops:
-            color, alpha = op(color, alpha)
-        return color, alpha
+            color_dst, alpha_dst = op(color_dst, color_src, alpha_dst, alpha_src)
+        return color_dst, alpha_dst
     return c
 
 def mosaic(image, mosaic_factor):
     original_size = util.swap(image.shape[:2])
     min_dim = min(original_size) // mosaic_factor
     min_dim = max(4, min_dim)
     scale_dimension = (original_size[0] // min_dim, original_size[1] // min_dim)
     mosaic_image = cv2.resize(image, scale_dimension, interpolation=cv2.INTER_AREA)
     return cv2.resize(mosaic_image, original_size, interpolation=cv2.INTER_NEAREST).reshape(image.shape)
 
 mosaic_factor_default = 100
 
 @filter('censor')
-def mosaic_op(color, alpha, mosaic_factor=None, apply_to_alpha=False, *_):
+def mosaic_op(color_dst, color_src, alpha_dst, alpha_src, mosaic_factor=None, apply_to_alpha=False, *_):
     if mosaic_factor is None:
         mosaic_factor = mosaic_factor_default
     mosaic_factor = int(mosaic_factor)
-    color = mosaic(color, mosaic_factor)
+    color = mosaic(color_dst, mosaic_factor)
+    color = util.lerp(color_dst, color, alpha_src)
+    alpha = alpha_dst
     if apply_to_alpha:
-        alpha = mosaic(alpha, mosaic_factor)
+        alpha = mosaic(alpha_dst, mosaic_factor)
+        alpha = util.lerp(alpha_dst, alpha, alpha_src)
     return color, alpha
 
 @filter('blur')
-def blur_op(color, alpha, size=50, apply_to_alpha=False, *_):
+def blur_op(color_dst, color_src, alpha_dst, alpha_src, size=50, *_):
     size = float(size)
-    color = cv2.GaussianBlur(color, ksize=(0, 0), sigmaX=size, dst=color, borderType=cv2.BORDER_REPLICATE)
-    if apply_to_alpha:
-        alpha = cv2.GaussianBlur(alpha, ksize=(0, 0), sigmaX=size, dst=alpha, borderType=cv2.BORDER_REPLICATE)
+    color = cv2.GaussianBlur(color_dst, ksize=(0, 0), sigmaX=size, borderType=cv2.BORDER_REPLICATE)
+    alpha = cv2.GaussianBlur(alpha_dst, ksize=(0, 0), sigmaX=size, borderType=cv2.BORDER_REPLICATE).reshape(alpha_src.shape)
+    color = util.lerp(color_dst, color, alpha_src)
+    alpha = util.lerp(alpha_dst, alpha, alpha_src)
     return color, alpha
 
 def motion_blur(data, angle, size):
     kernel = np.zeros((size, size))
     kernel[(size - 1) // 2] = 1
     rotation = cv2.getRotationMatrix2D((size / 2, size / 2), angle, 1.0)
     kernel = cv2.warpAffine(kernel, rotation, (size, size))
     kernel *= (1.0 / np.sum(kernel))
     return cv2.filter2D(data, -1, kernel)
 
 @filter('motion-blur')
-def motion_blur_op(color, alpha, angle=0, size=50, apply_to_alpha=False, *_):
+def motion_blur_op(color_dst, color_src, alpha_dst, alpha_src, angle=0, size=50, *_):
     angle = float(angle)
     size = int(size)
-    color = motion_blur(color, angle, size)
-    if apply_to_alpha:
-        alpha = motion_blur(alpha, angle, size).reshape(alpha.shape)
+    color = motion_blur(color_dst, angle, size)
+    alpha = motion_blur(alpha_dst, angle, size).reshape(alpha_src.shape)
+    color = util.lerp(color_dst, color, alpha_src)
+    alpha = util.lerp(alpha_dst, alpha, alpha_src)
     return color, alpha
```

### Comparing `psd_export-1.0.8/src/psd_export/util.py` & `psd_export-1.0.9/src/psd_export/util.py`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.8/.gitignore` & `psd_export-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.8/LICENSE` & `psd_export-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `psd_export-1.0.8/README.md` & `psd_export-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,49 +43,52 @@
   - If there was a second primary tag `[2]` for example, the whole set of combinations would be exported again but with `2` instead of `1`
 
 #### Image filters
 - Tags with special names will be treated as filters on the colors below them.
 - Filters can double as export tags too.
 - If you want a filter to not be treated as an export tag, you can preceed it with `#` to set the ignore flag, for example `[#censor]`
 - Filters can have arguments as well to control their behavior, separated by spaces, for example `[#censor 50]`
-- If you want the filter to apply to layers outside of the group it is in, then the group blend mode should be set to `pass-through`, otherwise it may blend with transparent black pixels if the filter is over a transparent part of a group.
+- If you want the filter to apply to layers outside of the group it is in, then the group blend mode should be set to `pass-through`, otherwise it may blend with transparent black pixels if the filter is over a transparent part of a group. The blur and motion blur filters apply to alpha as well, so they should behave as expected in isolated groups.
 - If multiple filters are enabled in one layer, they will be applied from left to right on top of each result, example:
   - `[#censor][#blur]` will apply a mosaic, and then a blur on top of that mosaic.
+- Blend modes and clipping layers applied directly to filter layers are ignored.
 
 ##### Available default filters:
-- `[censor mosaic_factor]`
-  - If the mosaic_factor argument is omitted, then it is defaulted to 100, which means 1/100th the smallest dimension, (or 4 pixels, whichever is larger) in order to be Pixiv compliant.
+- `[censor mosaic_factor apply_to_alpha]`
+  - If the `mosaic_factor` argument is omitted, then it is defaulted to 100, which means 1/100th the smallest dimension, (or 4 pixels, whichever is larger) in order to be Pixiv compliant.
+  - `apply_to_alpha` defaults to False. Any value is treated as True.
   - Typically you will want this filter to be a secondary tag, for example: `[censor@]`, so you can have censored and uncensored outputs.
 - `[blur size]`
   - The `size` argument defaults to 50 if omitted.
   - This filter is best used to create a non-destructive blur, such as for a background layer. You can fill an entire layer and set it to `[#blur 8]` for example.
 - `[motion-blur angle size]`
   - `angle` is in degrees, starting from horizontal to the right; Default 0.
   - `size` defaults to 50.
   - Best used for non-destructive blur: `[#motion-blur 45 20]`
 
 ##### Adding a new filter:
 In your own script:
 ```py
 # my-export.py
-from psd_export import (export, filters)
+from psd_export import (export, filters, util)
 import numpy as np
 
 my_arg1_default = 1.0
 
 # Register the filter with this decorator:
 @filters.filter('my-filter')
-# Only positional arguments work right now.
-def some_filter(color, alpha, arg1=None, arg2=100, *_):
+# Only positional arguments work right now. The result of this function replaces the destination color and alpha.
+def some_filter(color_dst, color_src, alpha_dst, alpha_src, arg1=None, arg2=100, *_):
     # Cast arguments to your desired types, as they will come in as strings.
     if arg1 is None:
         arg1 = my_arg1_default
     arg1 = float(arg1)
     # Manipulate color and alpha numpy arrays, in-place if you want.
     color = np.subtract(arg1, color, out=color)
+    color = util.lerp(color_dst, color, alpha_src)
     # Always return the same shaped arrays as a tuple:
     return color, alpha
 
 if __name__ == '__main__':
     # Add your own command line arguments if needed.
     export.arg_parser.add_argument('--my-arg1', default=my_arg1_default, type=float,
         help='Set the arg1 default parameter.')
```

### Comparing `psd_export-1.0.8/pyproject.toml` & `psd_export-1.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "psd-export"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
     { name = "cromachina" }
 ]
 license = { file = "LICENSE" }
 description = "Fast exporting of PSDs with [tagged] layers for variants."
 readme = "README.md"
 requires-python = ">=3.0"
```

### Comparing `psd_export-1.0.8/PKG-INFO` & `psd_export-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psd-export
-Version: 1.0.8
+Version: 1.0.9
 Summary: Fast exporting of PSDs with [tagged] layers for variants.
 Project-URL: Homepage, https://github.com/cromachina/psd-export
 Author: cromachina
 License: MIT License
         
         Copyright (c) 2022 cromachina
         
@@ -87,49 +87,52 @@
   - If there was a second primary tag `[2]` for example, the whole set of combinations would be exported again but with `2` instead of `1`
 
 #### Image filters
 - Tags with special names will be treated as filters on the colors below them.
 - Filters can double as export tags too.
 - If you want a filter to not be treated as an export tag, you can preceed it with `#` to set the ignore flag, for example `[#censor]`
 - Filters can have arguments as well to control their behavior, separated by spaces, for example `[#censor 50]`
-- If you want the filter to apply to layers outside of the group it is in, then the group blend mode should be set to `pass-through`, otherwise it may blend with transparent black pixels if the filter is over a transparent part of a group.
+- If you want the filter to apply to layers outside of the group it is in, then the group blend mode should be set to `pass-through`, otherwise it may blend with transparent black pixels if the filter is over a transparent part of a group. The blur and motion blur filters apply to alpha as well, so they should behave as expected in isolated groups.
 - If multiple filters are enabled in one layer, they will be applied from left to right on top of each result, example:
   - `[#censor][#blur]` will apply a mosaic, and then a blur on top of that mosaic.
+- Blend modes and clipping layers applied directly to filter layers are ignored.
 
 ##### Available default filters:
-- `[censor mosaic_factor]`
-  - If the mosaic_factor argument is omitted, then it is defaulted to 100, which means 1/100th the smallest dimension, (or 4 pixels, whichever is larger) in order to be Pixiv compliant.
+- `[censor mosaic_factor apply_to_alpha]`
+  - If the `mosaic_factor` argument is omitted, then it is defaulted to 100, which means 1/100th the smallest dimension, (or 4 pixels, whichever is larger) in order to be Pixiv compliant.
+  - `apply_to_alpha` defaults to False. Any value is treated as True.
   - Typically you will want this filter to be a secondary tag, for example: `[censor@]`, so you can have censored and uncensored outputs.
 - `[blur size]`
   - The `size` argument defaults to 50 if omitted.
   - This filter is best used to create a non-destructive blur, such as for a background layer. You can fill an entire layer and set it to `[#blur 8]` for example.
 - `[motion-blur angle size]`
   - `angle` is in degrees, starting from horizontal to the right; Default 0.
   - `size` defaults to 50.
   - Best used for non-destructive blur: `[#motion-blur 45 20]`
 
 ##### Adding a new filter:
 In your own script:
 ```py
 # my-export.py
-from psd_export import (export, filters)
+from psd_export import (export, filters, util)
 import numpy as np
 
 my_arg1_default = 1.0
 
 # Register the filter with this decorator:
 @filters.filter('my-filter')
-# Only positional arguments work right now.
-def some_filter(color, alpha, arg1=None, arg2=100, *_):
+# Only positional arguments work right now. The result of this function replaces the destination color and alpha.
+def some_filter(color_dst, color_src, alpha_dst, alpha_src, arg1=None, arg2=100, *_):
     # Cast arguments to your desired types, as they will come in as strings.
     if arg1 is None:
         arg1 = my_arg1_default
     arg1 = float(arg1)
     # Manipulate color and alpha numpy arrays, in-place if you want.
     color = np.subtract(arg1, color, out=color)
+    color = util.lerp(color_dst, color, alpha_src)
     # Always return the same shaped arrays as a tuple:
     return color, alpha
 
 if __name__ == '__main__':
     # Add your own command line arguments if needed.
     export.arg_parser.add_argument('--my-arg1', default=my_arg1_default, type=float,
         help='Set the arg1 default parameter.')
```

