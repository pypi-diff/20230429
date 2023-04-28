# Comparing `tmp/vodesfunc-1.3.2.tar.gz` & `tmp/vodesfunc-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vodesfunc-1.3.2.tar", last modified: Thu Apr  6 21:21:01 2023, max compression
+gzip compressed data, was "vodesfunc-1.3.3.tar", last modified: Fri Apr 28 23:08:39 2023, max compression
```

## Comparing `vodesfunc-1.3.2.tar` & `vodesfunc-1.3.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 21:21:01.935778 vodesfunc-1.3.2/
--rw-rw-rw-   0        0        0     1083 2022-09-09 23:13:19.000000 vodesfunc-1.3.2/LICENSE
--rw-rw-rw-   0        0        0       60 2022-12-04 22:36:49.000000 vodesfunc-1.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1196 2023-04-06 21:21:01.934778 vodesfunc-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      374 2022-12-04 22:36:49.000000 vodesfunc-1.3.2/README.md
--rw-rw-rw-   0        0        0      340 2022-12-11 22:06:28.000000 vodesfunc-1.3.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 21:21:01.935778 vodesfunc-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1760 2022-12-04 22:36:49.000000 vodesfunc-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:21:01.911215 vodesfunc-1.3.2/vodesfunc/
--rw-rw-rw-   0        0        0      328 2023-03-25 20:17:58.000000 vodesfunc-1.3.2/vodesfunc/__init__.py
--rw-rw-rw-   0        0        0      362 2023-04-06 21:20:30.000000 vodesfunc-1.3.2/vodesfunc/_metadata.py
--rw-rw-rw-   0        0        0     1777 2023-01-06 15:15:08.000000 vodesfunc-1.3.2/vodesfunc/aa.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:21:01.933778 vodesfunc-1.3.2/vodesfunc/auto/
--rw-rw-rw-   0        0        0     3883 2022-11-14 21:15:19.000000 vodesfunc-1.3.2/vodesfunc/auto/convert.py
--rw-rw-rw-   0        0        0     2859 2023-01-02 21:02:04.000000 vodesfunc-1.3.2/vodesfunc/auto/download.py
--rw-rw-rw-   0        0        0    18298 2023-02-11 15:17:49.000000 vodesfunc-1.3.2/vodesfunc/auto/fonts.py
--rw-rw-rw-   0        0        0    16967 2023-04-02 20:43:50.000000 vodesfunc-1.3.2/vodesfunc/auto/muxing.py
--rw-rw-rw-   0        0        0     4772 2022-12-25 22:08:09.000000 vodesfunc-1.3.2/vodesfunc/auto/parsing.py
--rw-rw-rw-   0        0        0     1850 2022-09-09 23:21:11.000000 vodesfunc-1.3.2/vodesfunc/auto/webhook.py
--rw-rw-rw-   0        0        0    32242 2023-04-06 21:19:38.000000 vodesfunc-1.3.2/vodesfunc/automation.py
--rw-rw-rw-   0        0        0     4743 2023-04-02 16:40:34.000000 vodesfunc-1.3.2/vodesfunc/denoise.py
--rw-rw-rw-   0        0        0    12477 2023-03-25 20:17:58.000000 vodesfunc-1.3.2/vodesfunc/descale.py
--rw-rw-rw-   0        0        0     3604 2022-11-26 23:27:32.000000 vodesfunc-1.3.2/vodesfunc/misc.py
--rw-rw-rw-   0        0        0     7305 2023-03-13 21:24:06.000000 vodesfunc-1.3.2/vodesfunc/noise.py
--rw-rw-rw-   0        0        0    11134 2023-04-06 21:20:11.000000 vodesfunc-1.3.2/vodesfunc/scale.py
--rw-rw-rw-   0        0        0      650 2022-12-26 01:30:13.000000 vodesfunc-1.3.2/vodesfunc/types.py
--rw-rw-rw-   0        0        0     7542 2023-02-25 18:27:53.000000 vodesfunc-1.3.2/vodesfunc/util.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:21:01.928221 vodesfunc-1.3.2/vodesfunc.egg-info/
--rw-rw-rw-   0        0        0     1196 2023-04-06 21:21:01.000000 vodesfunc-1.3.2/vodesfunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-04-06 21:21:01.000000 vodesfunc-1.3.2/vodesfunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 21:21:01.000000 vodesfunc-1.3.2/vodesfunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-04-06 21:21:01.000000 vodesfunc-1.3.2/vodesfunc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-06 21:21:01.000000 vodesfunc-1.3.2/vodesfunc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 23:08:39.016950 vodesfunc-1.3.3/
+-rw-rw-rw-   0        0        0     1083 2022-09-09 23:13:19.000000 vodesfunc-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0       60 2022-12-04 22:36:49.000000 vodesfunc-1.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1196 2023-04-28 23:08:39.016950 vodesfunc-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2022-12-04 22:36:49.000000 vodesfunc-1.3.3/README.md
+-rw-rw-rw-   0        0        0      340 2022-12-11 22:06:28.000000 vodesfunc-1.3.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 23:08:39.016950 vodesfunc-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1760 2022-12-04 22:36:49.000000 vodesfunc-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:08:38.999474 vodesfunc-1.3.3/vodesfunc/
+-rw-rw-rw-   0        0        0      328 2023-03-25 20:17:58.000000 vodesfunc-1.3.3/vodesfunc/__init__.py
+-rw-rw-rw-   0        0        0      362 2023-04-28 23:08:29.000000 vodesfunc-1.3.3/vodesfunc/_metadata.py
+-rw-rw-rw-   0        0        0     1777 2023-01-06 15:15:08.000000 vodesfunc-1.3.3/vodesfunc/aa.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:08:39.015950 vodesfunc-1.3.3/vodesfunc/auto/
+-rw-rw-rw-   0        0        0     3883 2022-11-14 21:15:19.000000 vodesfunc-1.3.3/vodesfunc/auto/convert.py
+-rw-rw-rw-   0        0        0     2859 2023-01-02 21:02:04.000000 vodesfunc-1.3.3/vodesfunc/auto/download.py
+-rw-rw-rw-   0        0        0    18298 2023-02-11 15:17:49.000000 vodesfunc-1.3.3/vodesfunc/auto/fonts.py
+-rw-rw-rw-   0        0        0    16967 2023-04-02 20:43:50.000000 vodesfunc-1.3.3/vodesfunc/auto/muxing.py
+-rw-rw-rw-   0        0        0     4772 2022-12-25 22:08:09.000000 vodesfunc-1.3.3/vodesfunc/auto/parsing.py
+-rw-rw-rw-   0        0        0     1850 2022-09-09 23:21:11.000000 vodesfunc-1.3.3/vodesfunc/auto/webhook.py
+-rw-rw-rw-   0        0        0    32242 2023-04-28 20:17:32.000000 vodesfunc-1.3.3/vodesfunc/automation.py
+-rw-rw-rw-   0        0        0     4743 2023-04-02 16:40:34.000000 vodesfunc-1.3.3/vodesfunc/denoise.py
+-rw-rw-rw-   0        0        0    12477 2023-04-28 20:16:26.000000 vodesfunc-1.3.3/vodesfunc/descale.py
+-rw-rw-rw-   0        0        0     3604 2022-11-26 23:27:32.000000 vodesfunc-1.3.3/vodesfunc/misc.py
+-rw-rw-rw-   0        0        0     7598 2023-04-06 21:35:28.000000 vodesfunc-1.3.3/vodesfunc/noise.py
+-rw-rw-rw-   0        0        0    14180 2023-04-28 23:07:12.000000 vodesfunc-1.3.3/vodesfunc/scale.py
+-rw-rw-rw-   0        0        0      650 2022-12-26 01:30:13.000000 vodesfunc-1.3.3/vodesfunc/types.py
+-rw-rw-rw-   0        0        0     7542 2023-04-28 20:15:55.000000 vodesfunc-1.3.3/vodesfunc/util.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:08:39.011947 vodesfunc-1.3.3/vodesfunc.egg-info/
+-rw-rw-rw-   0        0        0     1196 2023-04-28 23:08:38.000000 vodesfunc-1.3.3/vodesfunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-04-28 23:08:38.000000 vodesfunc-1.3.3/vodesfunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 23:08:38.000000 vodesfunc-1.3.3/vodesfunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-04-28 23:08:38.000000 vodesfunc-1.3.3/vodesfunc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-28 23:08:38.000000 vodesfunc-1.3.3/vodesfunc.egg-info/top_level.txt
```

### Comparing `vodesfunc-1.3.2/LICENSE` & `vodesfunc-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/PKG-INFO` & `vodesfunc-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.3.2
+Version: 1.3.3
 Summary: Vodes's Vapoursynth Functions.
 Author: Vodes
 Author-email: vodes.imp@gmail.com
 Maintainer: Vodes
 Maintainer-email: vodes.imp@gmail.com
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
```

### Comparing `vodesfunc-1.3.2/setup.py` & `vodesfunc-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc/aa.py` & `vodesfunc-1.3.3/vodesfunc/aa.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc/auto/convert.py` & `vodesfunc-1.3.3/vodesfunc/auto/convert.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc/auto/download.py` & `vodesfunc-1.3.3/vodesfunc/auto/download.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc/auto/fonts.py` & `vodesfunc-1.3.3/vodesfunc/auto/fonts.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc/auto/muxing.py` & `vodesfunc-1.3.3/vodesfunc/auto/muxing.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc/auto/parsing.py` & `vodesfunc-1.3.3/vodesfunc/auto/parsing.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc/auto/webhook.py` & `vodesfunc-1.3.3/vodesfunc/auto/webhook.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc/automation.py` & `vodesfunc-1.3.3/vodesfunc/automation.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc/denoise.py` & `vodesfunc-1.3.3/vodesfunc/denoise.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc/descale.py` & `vodesfunc-1.3.3/vodesfunc/descale.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc/misc.py` & `vodesfunc-1.3.3/vodesfunc/misc.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc/noise.py` & `vodesfunc-1.3.3/vodesfunc/noise.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,19 @@
 
     if scale >= 2:
         raise ValueError('adaptive_grain: Scale has to be a number below 2. (Default is 1, to disable scaling)')
 
     mask = core.adg.Mask(clip.std.PlaneStats() if luma_scaling >= 0 else clip.std.Invert().std.PlaneStats(), abs(luma_scaling))
     ogdepth = get_depth(clip)
 
+    # Type 4 depends on the input clip and as such should not be static, averaged or scaled
+    if type == 4:
+        grained = clip.noise.Add(strength[0], strength[1], type=type, xsize=size[0], ysize=size[1], constant=False, **kwargs)
+        return clip.std.MaskedMerge(grained, mask)
+
     def scale_val8x(value: int, chroma: bool = False) -> float:
         return scale_value(value, 8, ogdepth, scale_offsets=not tv_range, chroma=chroma)
 
     neutral = [get_neutral_value(clip), get_neutral_value(clip, True)]
 
     if not static and temporal_average > 0:
         length = clip.num_frames + temporal_radius - 1
```

### Comparing `vodesfunc-1.3.2/vodesfunc/scale.py` & `vodesfunc-1.3.3/vodesfunc/scale.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from typing import Any, Callable
-
-import vapoursynth as vs
 from vskernels import Catrom, Kernel, Scaler
-from vstools import depth, get_depth, get_y, Matrix
+from vstools import vs, core, depth, get_depth, get_y, Matrix, KwargsT, get_nvidia_version
 from vsrgtools.sharp import unsharp_masked
 from .types import PathLike
 from abc import ABC, abstractmethod
-core = vs.core
 
 
 __all__: list[str] = [
     'NNEDI_Doubler',
     'Clamped_Doubler',
     'Shader_Doubler',
     'Waifu2x_Doubler',
@@ -84,55 +81,123 @@
         doubled = core.std.ShufflePlanes([y, filler_chroma], [0, 1, 2], vs.YUV) \
             .placebo.Shader(self.shaderfile, filter='box', width=y.width*2, height=y.height*2)
         doubled_y = get_y(doubled)
         return depth(doubled_y, get_depth(clip))
 
 class Waifu2x_Doubler(Doubler):
     backend: any
-    kwargs: dict[str, Any]
+    kwargs: KwargsT
+    w2xargs: KwargsT = {}
 
-    def __init__(self, cuda: bool | str = 'trt', fp16: bool = True, num_streams: int = 1, **kwargs) -> None:
+    def __init__(self, cuda: bool | str | None = None, fp16: bool = True, num_streams: int = 1, tiles: int | tuple[int, int] | None = None, model: int = 6, **kwargs) -> None:
         """
             Simple utility class for doubling a clip using Waifu2x
 
-            :param cuda:            ORT-Cuda if True, NCNN-VK if False, TRT if some string
-            :param fp16:            Uses 16 bit floating point internally if True
-            :param num_streams:     Amount of streams to use for Waifu2x; Sacrifices a lot of vram for a speedup
-            :param w2xargs:         Args that get passed to Waifu2x
+            :param cuda:            ORT-Cuda if True, NCNN-VK or CPU (depending on what you have installed) if False, TRT if some string
+                                    Automatically chosen and tuned when None
+            :param fp16:            Uses 16 bit floating point internally if True.
+            :param num_streams:     Amount of streams to use for Waifu2x; Sacrifices a lot of vram for a speedup.
+            :param tiles:           Splits up the upscaling process into multiple tiles.
+                                    You will likely have to use atleast `2` if you have less than 16 GB of VRAM.
+            :param model:           Model to use from vsmlrt.
+            :param kwargs:          Args that get passed to both the Backend and actual scaling function.
         """
         from vsmlrt import Backend
-        self.backend = Backend.ORT_CUDA(num_streams=num_streams, fp16=fp16) if cuda == True else \
-            Backend.NCNN_VK(num_streams=num_streams, fp16=fp16) if cuda == False else Backend.TRT(num_streams=num_streams, fp16=fp16)
+
+        self.kwargs = {'num_streams': num_streams, 'fp16': fp16}
+
+        # Partially stolen from setsu but removed useless stuff that is default in mlrt already and added version checks
+        if cuda is None:
+            nv = get_nvidia_version()
+            cuda = nv is not None
+            try:
+                if nv is not None and not hasattr(core, 'trt') and hasattr(core, 'ort'):
+                    self.kwargs.update({'use_cuda_graph': True})
+                else:
+                    props: KwargsT = core.trt.DeviceProperties(kwargs.get('device_id', 0))
+                    version_props: KwargsT = core.trt.Version()
+
+                    vram = props.get('total_global_memory', 0)
+                    trt_version = float(version_props.get('tensorrt_version', 0))
+
+                    cuda = 'trt'
+
+                    presumedArgs = KwargsT(
+                        workspace=vram / (1 << 22) if vram else None,
+                        use_cuda_graph=True, use_cublas=True, use_cudnn=trt_version < 8400, 
+                        heuristic=trt_version >= 8500, output_format=int(fp16))
+                    
+                    # Swinunet doesn't like forced 16. Further testing for the other models needed.
+                    if model <= 6:
+                        presumedArgs.update({'tf32': not fp16, 'force_fp16': fp16})
+                        
+                    self.kwargs.update(presumedArgs)
+            except:
+                cuda = nv is not None
+
+        self.w2xargs = KwargsT(
+            model=model, tiles=tiles, preprocess=kwargs.pop('preprocess', True),
+            scale=kwargs.pop('scale', 2), tilesize=kwargs.pop('tilesize', None), overlap=kwargs.pop('overlap', None)
+        )
+
+        self.kwargs.update(kwargs)
+
+        if cuda is False:
+            if hasattr(core, 'ncnn'):
+                self.backend = Backend.NCNN_VK(**self.kwargs)
+            else:
+                self.kwargs.pop('device_id')
+                self.backend = Backend.ORT_CPU(**self.kwargs) if hasattr(core, 'ort') \
+                    else Backend.OV_CPU(**self.kwargs)
+        elif cuda is True:
+            self.backend = Backend.ORT_CUDA(**self.kwargs) if hasattr(core, 'ort') \
+                else Backend.OV_GPU(**self.kwargs)              
+        else:
+            self.backend = Backend.TRT(**self.kwargs)
+
         self.kwargs = kwargs
+        self.model = model
 
     def double(self, clip: vs.VideoNode) -> vs.VideoNode:
         from vsmlrt import Waifu2x
         pre = depth(clip, 32).std.Limiter()
 
         (left, right, top, bottom) = mod_padding(pre)
         width = pre.width + left + right
         height = pre.height + top + bottom
         pad = pre.resize.Point(width, height, src_left=-left, src_top=-top, src_width=width, src_height=height)
 
-        was_444 = pre.format.color_family == vs.YUV and pre.format.subsampling_w == 0 and pre.format.subsampling_h == 0
+        # Model 0 wants a gray input
+        needs_gray = self.w2xargs.get('model', 6) == 0
+        was_444 = pre.format.color_family == vs.YUV and pre.format.subsampling_w == 0 and pre.format.subsampling_h == 0 and not needs_gray
 
         if was_444:
             pad = Catrom().resample(pad, format=vs.RGBS, matrix=Matrix.RGB, matrix_in=Matrix.from_video(pre))
+        elif needs_gray is True:
+            pad = get_y(pad)
         else: 
             pad = get_y(pad).std.ShufflePlanes(0, vs.RGB)
 
-        up = Waifu2x(pad, noise=-1, model=6, backend=self.backend, **self.kwargs)
+        print(pad)
+
+        up = Waifu2x(pad, noise=-1, backend=self.backend, **self.w2xargs)
+
+        print(up)
 
         if was_444:
             up = Catrom().resample(up, format=vs.YUV444PS, matrix=Matrix.from_video(pre), matrix_in=Matrix.RGB)
-        else:
+        elif needs_gray is False:
             up = up.std.ShufflePlanes(0, vs.GRAY)
-
+        print(up.format)
         up = up.std.Crop(left * 2, right * 2, top * 2, bottom * 2)
-        up = up.std.Expr("x 0.5 255 / +")
+
+        # Only Model 6 has the tint
+        if self.w2xargs.get('model', 6) == 6:
+            up = up.std.Expr("x 0.5 255 / +")
+        
         return depth(up, get_depth(clip)).std.CopyFrameProps(pre)
  
 class Clamped_Doubler(Doubler):
 
     sharp_doubler: Doubler
     sharpen_smooth: bool | vs.VideoNode | Callable[[vs.VideoNode], vs.VideoNode] = None
```

### Comparing `vodesfunc-1.3.2/vodesfunc/types.py` & `vodesfunc-1.3.3/vodesfunc/types.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc/util.py` & `vodesfunc-1.3.3/vodesfunc/util.py`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.3.2/vodesfunc.egg-info/PKG-INFO` & `vodesfunc-1.3.3/vodesfunc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.3.2
+Version: 1.3.3
 Summary: Vodes's Vapoursynth Functions.
 Author: Vodes
 Author-email: vodes.imp@gmail.com
 Maintainer: Vodes
 Maintainer-email: vodes.imp@gmail.com
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
```

### Comparing `vodesfunc-1.3.2/vodesfunc.egg-info/SOURCES.txt` & `vodesfunc-1.3.3/vodesfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

