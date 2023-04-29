# Comparing `tmp/batdetect2-1.0.1.tar.gz` & `tmp/batdetect2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batdetect2-1.0.1.tar", last modified: Thu Apr 13 14:31:12 2023, max compression
+gzip compressed data, was "batdetect2-1.0.2.tar", last modified: Sat Apr 29 15:11:02 2023, max compression
```

## Comparing `batdetect2-1.0.1.tar` & `batdetect2-1.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    17694 2023-04-13 14:30:57.780691 batdetect2-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     5584 2023-04-13 14:30:57.784690 batdetect2-1.0.1/README.md
--rw-r--r--   0        0        0       22 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/__init__.py
--rw-r--r--   0        0        0    12537 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/api.py
--rw-r--r--   0        0        0     3522 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/cli.py
--rw-r--r--   0        0        0        0 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/detector/__init__.py
--rw-r--r--   0        0        0     4225 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/detector/compute_features.py
--rw-r--r--   0        0        0     4970 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/detector/model_helpers.py
--rw-r--r--   0        0        0    10568 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/detector/models.py
--rw-r--r--   0        0        0     7481 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/detector/parameters.py
--rw-r--r--   0        0        0     5830 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/detector/post_process.py
--rw-r--r--   0        0        0        0 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/evaluate/__init__.py
--rw-r--r--   0        0        0    25540 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/evaluate/evaluate_models.py
--rw-r--r--   0        0        0     2244 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/evaluate/readme.md
--rw-r--r--   0        0        0        0 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/finetune/__init__.py
--rw-r--r--   0        0        0     9902 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/finetune/finetune_model.py
--rw-r--r--   0        0        0     6324 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/finetune/prep_data_finetune.py
--rw-r--r--   0        0        0     3158 2023-04-13 14:30:57.784690 batdetect2-1.0.1/batdetect2/finetune/readme.md
--rw-r--r--   0        0        0  7600690 2023-04-13 14:30:57.840691 batdetect2-1.0.1/batdetect2/models/Net2DFast_UK_same.pth.tar
--rw-r--r--   0        0        0       25 2023-04-13 14:30:57.840691 batdetect2-1.0.1/batdetect2/models/readme.md
--rw-r--r--   0        0        0     9815 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/plot.py
--rw-r--r--   0        0        0        0 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/train/__init__.py
--rw-r--r--   0        0        0    20543 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/train/audio_dataloader.py
--rwxr-xr-x   0        0        0    13217 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/train/evaluate.py
--rw-r--r--   0        0        0     1580 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/train/losses.py
--rw-r--r--   0        0        0     1186 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/train/readme.md
--rw-r--r--   0        0        0    17521 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/train/train_model.py
--rw-r--r--   0        0        0    12533 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/train/train_split.py
--rw-r--r--   0        0        0     5961 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/train/train_utils.py
--rw-r--r--   0        0        0    11150 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/types.py
--rw-r--r--   0        0        0        0 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/utils/__init__.py
--rw-r--r--   0        0        0     8455 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/utils/audio_utils.py
--rw-r--r--   0        0        0    23243 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/utils/detector_utils.py
--rw-r--r--   0        0        0    16322 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/utils/plot_utils.py
--rw-r--r--   0        0        0     7940 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/utils/visualize.py
--rw-r--r--   0        0        0     8059 2023-04-13 14:30:57.844691 batdetect2-1.0.1/batdetect2/utils/wavfile.py
--rw-r--r--   0        0        0     1740 2023-04-13 14:30:57.860691 batdetect2-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-13 14:30:57.860691 batdetect2-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     8805 2023-04-13 14:30:57.860691 batdetect2-1.0.1/tests/test_api.py
--rw-r--r--   0        0        0     1223 2023-04-13 14:30:57.860691 batdetect2-1.0.1/tests/test_cli.py
--rw-r--r--   0        0        0     6537 1970-01-01 00:00:00.000000 batdetect2-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    17694 2023-04-29 15:10:53.237251 batdetect2-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     5584 2023-04-29 15:10:53.237251 batdetect2-1.0.2/README.md
+-rw-r--r--   0        0        0       22 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/__init__.py
+-rw-r--r--   0        0        0    12537 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/api.py
+-rw-r--r--   0        0        0     3522 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/cli.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/detector/__init__.py
+-rw-r--r--   0        0        0     4225 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/detector/compute_features.py
+-rw-r--r--   0        0        0     4970 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/detector/model_helpers.py
+-rw-r--r--   0        0        0    10568 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/detector/models.py
+-rw-r--r--   0        0        0     7481 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/detector/parameters.py
+-rw-r--r--   0        0        0     5873 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/detector/post_process.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/evaluate/__init__.py
+-rw-r--r--   0        0        0    25540 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/evaluate/evaluate_models.py
+-rw-r--r--   0        0        0     2244 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/evaluate/readme.md
+-rw-r--r--   0        0        0        0 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/finetune/__init__.py
+-rw-r--r--   0        0        0     9902 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/finetune/finetune_model.py
+-rw-r--r--   0        0        0     6324 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/finetune/prep_data_finetune.py
+-rw-r--r--   0        0        0     3158 2023-04-29 15:10:53.237251 batdetect2-1.0.2/batdetect2/finetune/readme.md
+-rw-r--r--   0        0        0  7600690 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/models/Net2DFast_UK_same.pth.tar
+-rw-r--r--   0        0        0       25 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/models/readme.md
+-rw-r--r--   0        0        0     9832 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/plot.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/train/__init__.py
+-rw-r--r--   0        0        0    20543 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/train/audio_dataloader.py
+-rwxr-xr-x   0        0        0    13217 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/train/evaluate.py
+-rw-r--r--   0        0        0     1580 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/train/losses.py
+-rw-r--r--   0        0        0     1186 2023-04-29 15:10:53.285252 batdetect2-1.0.2/batdetect2/train/readme.md
+-rw-r--r--   0        0        0    17515 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/train/train_model.py
+-rw-r--r--   0        0        0    12533 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/train/train_split.py
+-rw-r--r--   0        0        0     5961 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/train/train_utils.py
+-rw-r--r--   0        0        0    11150 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/types.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/utils/__init__.py
+-rw-r--r--   0        0        0     8455 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/utils/audio_utils.py
+-rw-r--r--   0        0        0    23308 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/utils/detector_utils.py
+-rw-r--r--   0        0        0    16322 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/utils/plot_utils.py
+-rw-r--r--   0        0        0     7940 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/utils/visualize.py
+-rw-r--r--   0        0        0     8059 2023-04-29 15:10:53.289252 batdetect2-1.0.2/batdetect2/utils/wavfile.py
+-rw-r--r--   0        0        0     1749 2023-04-29 15:10:53.301252 batdetect2-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-29 15:10:53.301252 batdetect2-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     8805 2023-04-29 15:10:53.305252 batdetect2-1.0.2/tests/test_api.py
+-rw-r--r--   0        0        0     1223 2023-04-29 15:10:53.305252 batdetect2-1.0.2/tests/test_cli.py
+-rw-r--r--   0        0        0     6537 1970-01-01 00:00:00.000000 batdetect2-1.0.2/PKG-INFO
```

### Comparing `batdetect2-1.0.1/LICENSE.md` & `batdetect2-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/README.md` & `batdetect2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/api.py` & `batdetect2-1.0.2/batdetect2/api.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/cli.py` & `batdetect2-1.0.2/batdetect2/cli.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/detector/compute_features.py` & `batdetect2-1.0.2/batdetect2/detector/compute_features.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/detector/model_helpers.py` & `batdetect2-1.0.2/batdetect2/detector/model_helpers.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/detector/models.py` & `batdetect2-1.0.2/batdetect2/detector/models.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/detector/parameters.py` & `batdetect2-1.0.2/batdetect2/detector/parameters.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/detector/post_process.py` & `batdetect2-1.0.2/batdetect2/detector/post_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,23 @@
     x_pos: float,
     sampling_rate: int,
     fft_win_length: float,
     fft_overlap: float,
 ) -> float:
     """Convert x coordinates of spectrogram to time in seconds.
 
-    Args:
+    Parameters
+    ----------
         x_pos: X position of the detection in pixels.
         sampling_rate: Sampling rate of the audio in Hz.
         fft_win_length: Length of the FFT window in seconds.
         fft_overlap: Overlap of the FFT windows in seconds.
 
-    Returns:
+    Returns
+    -------
         Time in seconds.
     """
     nfft = int(fft_win_length * sampling_rate)
     noverlap = int(fft_overlap * nfft)
     return ((x_pos * (nfft - noverlap)) + noverlap) / sampling_rate
 
 
@@ -130,20 +132,20 @@
         if features is not None:
             feat = features[
                 num_detection,
                 :,
                 y_pos[num_detection, valid_inds],
                 x_pos[num_detection, valid_inds],
             ].transpose(0, 1)
-            feat = feat.detach().numpy().astype(np.float32)
+            feat = feat.detach().cpu().numpy().astype(np.float32)
             feats.append(feat)
 
         # convert to numpy
         for key, value in pred.items():
-            pred[key] = value.detach().numpy().astype(np.float32)
+            pred[key] = value.detach().cpu().numpy().astype(np.float32)
 
         preds.append(pred)  # type: ignore
 
     return preds, feats
 
 
 def non_max_suppression(
```

### Comparing `batdetect2-1.0.1/batdetect2/evaluate/evaluate_models.py` & `batdetect2-1.0.2/batdetect2/evaluate/evaluate_models.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/evaluate/readme.md` & `batdetect2-1.0.2/batdetect2/evaluate/readme.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/finetune/finetune_model.py` & `batdetect2-1.0.2/batdetect2/finetune/finetune_model.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/finetune/prep_data_finetune.py` & `batdetect2-1.0.2/batdetect2/finetune/prep_data_finetune.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/finetune/readme.md` & `batdetect2-1.0.2/batdetect2/finetune/readme.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/models/Net2DFast_UK_same.pth.tar` & `batdetect2-1.0.2/batdetect2/models/Net2DFast_UK_same.pth.tar`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/plot.py` & `batdetect2-1.0.2/batdetect2/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     Raises
     ------
     ValueError: If the spectrogram is not of
         shape (1, T, F), (1, 1, T, F) or (T, F)
     """
     # Convert to numpy array if needed
     if isinstance(spec, torch.Tensor):
-        spec = spec.numpy()
+        spec = spec.detach().cpu().numpy()
 
     # Remove batch and channel dimensions if present
     spec = spec.squeeze()
 
     if spec.ndim != 2:
         raise ValueError(
             f"Expected a 2D tensor, got {spec.ndim}D tensor instead."
@@ -261,15 +261,15 @@
     )
     ax.add_patch(rect)
 
     if with_name:
         # Add class label
         txt = " ".join([sp[:3] for sp in det["class"].split(" ")])
         font_info = {
-            "color": "white",
+            "color": edgecolor,
             "size": 10,
             "weight": "bold",
             "alpha": rect.get_alpha(),
         }
         y_pos = rect.get_xy()[1] + rect.get_height()
         ax.text(rect.get_xy()[0], y_pos, txt, fontdict=font_info)
```

### Comparing `batdetect2-1.0.1/batdetect2/train/audio_dataloader.py` & `batdetect2-1.0.2/batdetect2/train/audio_dataloader.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/train/evaluate.py` & `batdetect2-1.0.2/batdetect2/train/evaluate.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/train/losses.py` & `batdetect2-1.0.2/batdetect2/train/losses.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/train/readme.md` & `batdetect2-1.0.2/batdetect2/train/readme.md`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/train/train_model.py` & `batdetect2-1.0.2/batdetect2/train/train_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 import warnings
 
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from torch.optim.lr_scheduler import CosineAnnealingLR
 
-from batdetect2.detector import models
-from batdetect2.detector import parameters
-from batdetect2.train import losses
 import batdetect2.detector.post_process as pp
 import batdetect2.train.audio_dataloader as adl
 import batdetect2.train.evaluate as evl
 import batdetect2.train.train_split as ts
 import batdetect2.train.train_utils as tu
 import batdetect2.utils.plot_utils as pu
+from batdetect2.detector import models, parameters
+from batdetect2.train import losses
 
 warnings.filterwarnings("ignore", category=UserWarning)
 
 
 def save_images_batch(model, data_loader, params):
     print("\nsaving images ...")
 
@@ -80,15 +79,14 @@
         fixed_aspect=False,
     )
 
 
 def loss_fun(
     outputs, gt_det, gt_size, gt_class, det_criterion, params, class_inv_freq
 ):
-
     # detection loss
     loss = params["det_loss_weight"] * det_criterion(
         outputs["pred_det"], gt_det
     )
 
     # bounding box size loss
     loss += params["size_loss_weight"] * losses.bbox_size_loss(
@@ -104,26 +102,24 @@
 
     return loss
 
 
 def train(
     model, epoch, data_loader, det_criterion, optimizer, scheduler, params
 ):
-
     model.train()
 
     train_loss = tu.AverageMeter()
     class_inv_freq = torch.from_numpy(
         np.array(params["class_inv_freq"], dtype=np.float32)
     ).to(params["device"])
     class_inv_freq = class_inv_freq.unsqueeze(0).unsqueeze(2).unsqueeze(2)
 
     print("\nEpoch", epoch)
     for batch_idx, inputs in enumerate(data_loader):
-
         data = inputs["spec"].to(params["device"])
         gt_det = inputs["y_2d_det"].to(params["device"])
         gt_size = inputs["y_2d_size"].to(params["device"])
         gt_class = inputs["y_2d_classes"].to(params["device"])
 
         optimizer.zero_grad()
         outputs = model(data)
@@ -168,15 +164,14 @@
     class_inv_freq = torch.from_numpy(
         np.array(params["class_inv_freq"], dtype=np.float32)
     ).to(params["device"])
     class_inv_freq = class_inv_freq.unsqueeze(0).unsqueeze(2).unsqueeze(2)
 
     with torch.no_grad():
         for batch_idx, inputs in enumerate(data_loader):
-
             data = inputs["spec"].to(params["device"])
             gt_det = inputs["y_2d_det"].to(params["device"])
             gt_size = inputs["y_2d_size"].to(params["device"])
             gt_class = inputs["y_2d_classes"].to(params["device"])
 
             outputs = model(data)
 
@@ -275,15 +270,15 @@
         "individual_ids",
     ]
     batch_data = []
     for ind in range(inputs["start_times"].shape[0]):
         is_valid = inputs["is_valid"][ind] == 1
         gt = {}
         for kk in keys:
-            gt[kk] = inputs[kk][ind][is_valid].numpy().astype(np.float32)
+            gt[kk] = inputs[kk][ind][is_valid].cpu().numpy().astype(np.float32)
         gt["duration"] = inputs["duration"][ind].item()
         gt["file_id"] = inputs["file_id"][ind].item()
         gt["class_id_file"] = inputs["class_id_file"][ind].item()
         batch_data.append(gt)
     return batch_data
 
 
@@ -314,16 +309,15 @@
             resize_factor=params["resize_factor"],
         )
     else:
         print("No valid network specified")
     return model
 
 
-if __name__ == "__main__":
-
+def main():
     plt.close("all")
 
     params = parameters.get_params(True)
 
     if torch.cuda.is_available():
         params["device"] = "cuda"
     else:
@@ -497,15 +491,14 @@
         params["class_names_short"],
         ["epoch", "avg_prec"],
     )
 
     #
     # main train loop
     for epoch in range(0, params["num_epochs"] + 1):
-
         train_loss = train(
             model,
             epoch,
             train_loader,
             det_criterion,
             optimizer,
             scheduler,
@@ -546,7 +539,11 @@
             }
             torch.save(op_state, params["model_file_name"])
 
     # save an image with associated prediction for each batch in the test set
     # TODO: args variable does not exist
     # if not args["do_not_save_images"]:
     #     save_images_batch(model, test_loader, params)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `batdetect2-1.0.1/batdetect2/train/train_split.py` & `batdetect2-1.0.2/batdetect2/train/train_split.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/train/train_utils.py` & `batdetect2-1.0.2/batdetect2/train/train_utils.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/types.py` & `batdetect2-1.0.2/batdetect2/types.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/utils/audio_utils.py` & `batdetect2-1.0.2/batdetect2/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/utils/detector_utils.py` & `batdetect2-1.0.2/batdetect2/utils/detector_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -727,14 +727,15 @@
     # store temporary results here
     predictions = []
     spec_feats = []
     cnn_feats = []
     spec_slices = []
 
     # load audio file
+    print("time_exp_fact", config.get("time_expansion", 1) or 1)
     sampling_rate, audio_full = au.load_audio(
         audio_file,
         time_exp_fact=config.get("time_expansion", 1) or 1,
         target_samp_rate=config["target_samp_rate"],
         scale=config["scale_raw_audio"],
         max_duration=config.get("max_duration"),
     )
```

### Comparing `batdetect2-1.0.1/batdetect2/utils/plot_utils.py` & `batdetect2-1.0.2/batdetect2/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/utils/visualize.py` & `batdetect2-1.0.2/batdetect2/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/batdetect2/utils/wavfile.py` & `batdetect2-1.0.2/batdetect2/utils/wavfile.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/pyproject.toml` & `batdetect2-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -27,28 +27,28 @@
     "tests",
 ]
 venvPath = "."
 venv = ".venv"
 
 [project]
 name = "batdetect2"
-version = "1.0.1"
+version = "1.0.2"
 description = "Deep learning model for detecting and classifying bat echolocation calls in high frequency audio recordings."
 authors = [
     { name = "Oisin Mac Aodha", email = "oisin.macaodha@ed.ac.uk" },
     { name = "Santiago Martinez Balvanera", email = "santiago.balvanera.20@ucl.ac.uk" },
 ]
 dependencies = [
     "librosa",
     "matplotlib",
     "numpy",
     "pandas",
     "scikit-learn",
     "scipy",
-    "torch<2",
+    "torch>=1.13.1,<2",
     "torchaudio",
     "torchvision",
     "click",
 ]
 requires-python = ">=3.8,<3.11"
 readme = "README.md"
 classifiers = [
```

### Comparing `batdetect2-1.0.1/tests/test_api.py` & `batdetect2-1.0.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/tests/test_cli.py` & `batdetect2-1.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `batdetect2-1.0.1/PKG-INFO` & `batdetect2-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batdetect2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Deep learning model for detecting and classifying bat echolocation calls in high frequency audio recordings.
 License: CC-by-nc-4
 Keywords: bat,echolocation,deep learning,audio,machine learning,classification,detection
 Author-email: Oisin Mac Aodha <oisin.macaodha@ed.ac.uk>,Santiago Martinez Balvanera <santiago.balvanera.20@ucl.ac.uk>
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

