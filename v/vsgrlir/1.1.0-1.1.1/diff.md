# Comparing `tmp/vsgrlir-1.1.0-py3-none-any.whl.zip` & `tmp/vsgrlir-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 36384 bytes, number of entries: 28
+Zip file size: 37199 bytes, number of entries: 28
 -rw-r--r--  2.0 fat    22319 b- defN 20-Feb-02 00:00 vsgrlir/__init__.py
 -rw-r--r--  2.0 fat     1379 b- defN 20-Feb-02 00:00 vsgrlir/__main__.py
--rw-r--r--  2.0 fat    32347 b- defN 20-Feb-02 00:00 vsgrlir/grl.py
+-rw-r--r--  2.0 fat    32376 b- defN 20-Feb-02 00:00 vsgrlir/grl.py
 -rw-r--r--  2.0 fat    40252 b- defN 20-Feb-02 00:00 vsgrlir/mixed_attn_block.py
--rw-r--r--  2.0 fat    20448 b- defN 20-Feb-02 00:00 vsgrlir/mixed_attn_block_efficient.py
+-rw-r--r--  2.0 fat    23299 b- defN 20-Feb-02 00:00 vsgrlir/mixed_attn_block_efficient.py
 -rw-r--r--  2.0 fat    17487 b- defN 20-Feb-02 00:00 vsgrlir/ops.py
 -rw-r--r--  2.0 fat    21228 b- defN 20-Feb-02 00:00 vsgrlir/swin_v1_block.py
 -rw-r--r--  2.0 fat     1660 b- defN 20-Feb-02 00:00 vsgrlir/upsample.py
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsgrlir/models/bsr_grl_base.ckpt
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsgrlir/models/db_defocus_single_pixel_grl_base.ckpt
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsgrlir/models/db_motion_grl_base_gopro.ckpt
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsgrlir/models/db_motion_grl_base_realblur_j.ckpt
@@ -19,12 +19,12 @@
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsgrlir/models/jpeg_grl_small_c3q10.ckpt
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsgrlir/models/jpeg_grl_small_c3q20.ckpt
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsgrlir/models/jpeg_grl_small_c3q30.ckpt
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsgrlir/models/jpeg_grl_small_c3q40.ckpt
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsgrlir/models/sr_grl_small_c3x2.ckpt
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsgrlir/models/sr_grl_small_c3x3.ckpt
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsgrlir/models/sr_grl_small_c3x4.ckpt
-?rw-r--r--  2.0 fat     2550 b- defN 20-Feb-02 00:00 vsgrlir-1.1.0.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 vsgrlir-1.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1084 b- defN 20-Feb-02 00:00 vsgrlir-1.1.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat     2445 b- defN 20-Feb-02 00:00 vsgrlir-1.1.0.dist-info/RECORD
-28 files, 163286 bytes uncompressed, 32340 bytes compressed:  80.2%
+?rw-r--r--  2.0 fat     2550 b- defN 20-Feb-02 00:00 vsgrlir-1.1.1.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 vsgrlir-1.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1084 b- defN 20-Feb-02 00:00 vsgrlir-1.1.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat     2445 b- defN 20-Feb-02 00:00 vsgrlir-1.1.1.dist-info/RECORD
+28 files, 166166 bytes uncompressed, 33155 bytes compressed:  80.0%
```

## zipnote {}

```diff
@@ -66,20 +66,20 @@
 
 Filename: vsgrlir/models/sr_grl_small_c3x3.ckpt
 Comment: 
 
 Filename: vsgrlir/models/sr_grl_small_c3x4.ckpt
 Comment: 
 
-Filename: vsgrlir-1.1.0.dist-info/METADATA
+Filename: vsgrlir-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: vsgrlir-1.1.0.dist-info/WHEEL
+Filename: vsgrlir-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: vsgrlir-1.1.0.dist-info/licenses/LICENSE
+Filename: vsgrlir-1.1.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: vsgrlir-1.1.0.dist-info/RECORD
+Filename: vsgrlir-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vsgrlir/__init__.py

```diff
@@ -9,15 +9,15 @@
 import torch
 import torch.nn.functional as F
 import vapoursynth as vs
 from vsutil import fallback
 
 from .grl import GRL
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 os.environ["CUDA_MODULE_LOADING"] = "LAZY"
 
 model_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "models")
 
 
 class Backend:
```

## vsgrlir/grl.py

```diff
@@ -123,15 +123,16 @@
                 args=args,
             )
             self.blocks.append(block)
 
         self.conv = build_last_conv(conv_type, dim)
 
     def _apply_half(self, fn):
-        self.blocks.half()
+        for blk in self.blocks:
+            blk.half()
 
         def compute_should_use_set_data(tensor, tensor_applied):
             if torch._has_compatible_shallow_copy_type(tensor, tensor_applied):
                 # If the new tensor has compatible tensor type as the existing tensor,
                 # the current behavior is to change the tensor in-place using `.data =`,
                 # and the future behavior is to overwrite the existing tensor. However,
                 # changing the current behavior is a BC-breaking change, and we want it
```

## vsgrlir/mixed_attn_block_efficient.py

```diff
@@ -497,14 +497,78 @@
             in_features=dim,
             hidden_features=int(dim * mlp_ratio),
             act_layer=act_layer,
             drop=drop,
         )
         self.norm2 = norm_layer(dim)
 
+    def _apply_half(self, fn):
+        self.attn.half()
+        self.norm1.half()
+
+        def compute_should_use_set_data(tensor, tensor_applied):
+            if torch._has_compatible_shallow_copy_type(tensor, tensor_applied):
+                # If the new tensor has compatible tensor type as the existing tensor,
+                # the current behavior is to change the tensor in-place using `.data =`,
+                # and the future behavior is to overwrite the existing tensor. However,
+                # changing the current behavior is a BC-breaking change, and we want it
+                # to happen in future releases. So for now we introduce the
+                # `torch.__future__.get_overwrite_module_params_on_conversion()`
+                # global flag to let the user control whether they want the future
+                # behavior of overwriting the existing tensor or not.
+                return not torch.__future__.get_overwrite_module_params_on_conversion()
+            else:
+                return False
+
+        for key, param in self._parameters.items():
+            if param is None:
+                continue
+            # Tensors stored in modules are graph leaves, and we don't want to
+            # track autograd history of `param_applied`, so we have to use
+            # `with torch.no_grad():`
+            with torch.no_grad():
+                param_applied = fn(param)
+            should_use_set_data = compute_should_use_set_data(param, param_applied)
+            if should_use_set_data:
+                param.data = param_applied
+                out_param = param
+            else:
+                assert isinstance(param, nn.Parameter)
+                assert param.is_leaf
+                out_param = nn.Parameter(param_applied, param.requires_grad)
+                self._parameters[key] = out_param
+
+            if param.grad is not None:
+                with torch.no_grad():
+                    grad_applied = fn(param.grad)
+                should_use_set_data = compute_should_use_set_data(param.grad, grad_applied)
+                if should_use_set_data:
+                    assert out_param.grad is not None
+                    out_param.grad.data = grad_applied
+                else:
+                    assert param.grad.is_leaf
+                    out_param.grad = grad_applied.requires_grad_(param.grad.requires_grad)
+
+        for key, buf in self._buffers.items():
+            if buf is not None:
+                self._buffers[key] = fn(buf)
+
+        return self
+
+    def half(self):
+        r"""Casts all floating point parameters and buffers to ``half`` datatype.
+
+        .. note::
+            This method modifies the module in-place.
+
+        Returns:
+            Module: self
+        """
+        return self._apply_half(lambda t: t.half() if t.is_floating_point() else t)
+
     def _get_table_index_mask(self, all_table_index_mask):
         table_index_mask = {
             "table_w": all_table_index_mask["table_w"],
             "index_w": all_table_index_mask["index_w"],
         }
         if self.stripe_type == "W":
             table_index_mask["table_s"] = all_table_index_mask["table_sv"]
@@ -533,23 +597,23 @@
     def forward(self, x, x_size, all_table_index_mask):
         # Mixed attention
         table_index_mask = self._get_table_index_mask(all_table_index_mask)
         if self.args.local_connection:
             x = (
                 x
                 + self.res_scale
-                * self.drop_path(self.norm1(self.attn(x.half() if self.fp16 else x, x_size, table_index_mask)))
-                + self.conv(x.half() if self.fp16 else x, x_size)
+                * self.drop_path(self.norm1(self.attn(x.half() if self.fp16 else x, x_size, table_index_mask)).float())
+                + self.conv(x, x_size)
             )
         else:
             x = x + self.res_scale * self.drop_path(
-                self.norm1(self.attn(x.half() if self.fp16 else x, x_size, table_index_mask))
+                self.norm1(self.attn(x.half() if self.fp16 else x, x_size, table_index_mask)).float()
             )
         # FFN
-        x = x + self.res_scale * self.drop_path(self.norm2(self.mlp(x.half() if self.fp16 else x)))
+        x = x + self.res_scale * self.drop_path(self.norm2(self.mlp(x)))
 
         return x
 
     def extra_repr(self) -> str:
         return (
             f"dim={self.dim}, input_resolution={self.input_resolution}, num_heads=({self.num_heads_w}, {self.num_heads_s}), "
             f"window_size={self.window_size}, window_shift={self.window_shift}, "
```

## Comparing `vsgrlir-1.1.0.dist-info/METADATA` & `vsgrlir-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsgrlir
-Version: 1.1.0
+Version: 1.1.1
 Summary: GRLIR function for VapourSynth
 Project-URL: Homepage, https://github.com/HolyWu/vs-grlir
 Project-URL: Bug Tracker, https://github.com/HolyWu/vs-grlir/issues
 Author-email: HolyWu <holywu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 HolyWu
```

## Comparing `vsgrlir-1.1.0.dist-info/licenses/LICENSE` & `vsgrlir-1.1.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `vsgrlir-1.1.0.dist-info/RECORD` & `vsgrlir-1.1.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-vsgrlir/__init__.py,sha256=3B2s4yDQf5q0Od9bJHZ9aEruT2EYzHiWjyDlSXQbj3c,22319
+vsgrlir/__init__.py,sha256=0UGHv4mZCx4f9TwnGW0xD8U87vxLuRJ--YUYzmAbcTw,22319
 vsgrlir/__main__.py,sha256=DOsmcCnxWZL-Q_U10qhwyExNviQkIfXB-auI--Q0gvg,1379
-vsgrlir/grl.py,sha256=F0EcvmmE5X06u55ez1u2DA-bZGjKf5eFk_XSxzz0HDM,32347
+vsgrlir/grl.py,sha256=ak4X8Z25JWY2lBDrdDht8ux0d5RJGCyukdWr4bja9EM,32376
 vsgrlir/mixed_attn_block.py,sha256=UiczScju4tuVNm5R0gdqG6UO0npfZz-mj4gRwhw9ot8,40252
-vsgrlir/mixed_attn_block_efficient.py,sha256=qOcB4gnAVMxqK4pQkzSHSH-Jiibpw6E88r8vuAi8eZ4,20448
+vsgrlir/mixed_attn_block_efficient.py,sha256=3oX0lhIWm2DWXYVHf6CDq_oVHMk9f1zUm5erOAdJ2CI,23299
 vsgrlir/ops.py,sha256=YfALYJKJgjuA-Lw9TU6ZtLgtfyblgDmiKh2zjLi-Xm4,17487
 vsgrlir/swin_v1_block.py,sha256=HLIpxL97TpiUj4QpvtqIHZ5Y_67pSbk7PT5I5iZdx9Q,21228
 vsgrlir/upsample.py,sha256=p5ICIh_kPjsGTj_vH5N78f52Ja613EaCtDSE20Kp5bU,1660
 vsgrlir/models/bsr_grl_base.ckpt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsgrlir/models/db_defocus_single_pixel_grl_base.ckpt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsgrlir/models/db_motion_grl_base_gopro.ckpt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsgrlir/models/db_motion_grl_base_realblur_j.ckpt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -18,11 +18,11 @@
 vsgrlir/models/jpeg_grl_small_c3q10.ckpt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsgrlir/models/jpeg_grl_small_c3q20.ckpt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsgrlir/models/jpeg_grl_small_c3q30.ckpt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsgrlir/models/jpeg_grl_small_c3q40.ckpt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsgrlir/models/sr_grl_small_c3x2.ckpt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsgrlir/models/sr_grl_small_c3x3.ckpt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsgrlir/models/sr_grl_small_c3x4.ckpt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-vsgrlir-1.1.0.dist-info/METADATA,sha256=2zdryJ1wyp0wVfXrUvwtDgta9vdfk6fXYEINwNkKSCQ,2550
-vsgrlir-1.1.0.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-vsgrlir-1.1.0.dist-info/licenses/LICENSE,sha256=BBSpLSdr1ObkSfndfyGXSX5Z_RsTREd53WTyNX7PMB0,1084
-vsgrlir-1.1.0.dist-info/RECORD,,
+vsgrlir-1.1.1.dist-info/METADATA,sha256=TmWShKNmt59lCFllTYHhbQPzNsXE_SJUVtyWABRq9aE,2550
+vsgrlir-1.1.1.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+vsgrlir-1.1.1.dist-info/licenses/LICENSE,sha256=BBSpLSdr1ObkSfndfyGXSX5Z_RsTREd53WTyNX7PMB0,1084
+vsgrlir-1.1.1.dist-info/RECORD,,
```

