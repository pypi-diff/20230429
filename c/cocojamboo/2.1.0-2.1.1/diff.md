# Comparing `tmp/cocojamboo-2.1.0.tar.gz` & `tmp/cocojamboo-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocojamboo-2.1.0.tar", last modified: Sat Apr 29 09:48:16 2023, max compression
+gzip compressed data, was "cocojamboo-2.1.1.tar", last modified: Sat Apr 29 10:25:47 2023, max compression
```

## Comparing `cocojamboo-2.1.0.tar` & `cocojamboo-2.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:48:16.313206 cocojamboo-2.1.0/
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)    19334 2023-01-10 14:44:25.000000 cocojamboo-2.1.0/LICENSE
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:48:16.312896 cocojamboo-2.1.0/PKG-INFO
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)      122 2023-03-31 12:26:52.000000 cocojamboo-2.1.0/README.md
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:48:16.310343 cocojamboo-2.1.0/cocojamboo/
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)       75 2023-04-29 09:47:42.000000 cocojamboo-2.1.0/cocojamboo/__init__.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    52494 2023-04-29 09:37:26.000000 cocojamboo-2.1.0/cocojamboo/coco_eval2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    32238 2023-04-29 09:46:46.000000 cocojamboo-2.1.0/cocojamboo/coco_utils.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    45829 2023-04-29 07:00:48.000000 cocojamboo-2.1.0/cocojamboo/cocoeval2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     4562 2023-04-29 09:03:23.000000 cocojamboo-2.1.0/cocojamboo/engine2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23337 2023-02-17 12:32:17.000000 cocojamboo-2.1.0/cocojamboo/transforms.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     8388 2023-02-17 12:32:17.000000 cocojamboo-2.1.0/cocojamboo/utils.py
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 09:48:16.312202 cocojamboo-2.1.0/cocojamboo.egg-info/
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 09:48:16.000000 cocojamboo-2.1.0/cocojamboo.egg-info/PKG-INFO
--rw-r--r--   0 georgianamanolache   (501) staff       (20)      332 2023-04-29 09:48:16.000000 cocojamboo-2.1.0/cocojamboo.egg-info/SOURCES.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)        1 2023-04-29 09:48:16.000000 cocojamboo-2.1.0/cocojamboo.egg-info/dependency_links.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)       11 2023-04-29 09:48:16.000000 cocojamboo-2.1.0/cocojamboo.egg-info/top_level.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)      670 2023-04-29 09:47:45.000000 cocojamboo-2.1.0/pyproject.toml
--rw-r--r--   0 georgianamanolache   (501) staff       (20)       38 2023-04-29 09:48:16.313296 cocojamboo-2.1.0/setup.cfg
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 10:25:47.475360 cocojamboo-2.1.1/
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)    19334 2023-01-10 14:44:25.000000 cocojamboo-2.1.1/LICENSE
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 10:25:47.474867 cocojamboo-2.1.1/PKG-INFO
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)      122 2023-03-31 12:26:52.000000 cocojamboo-2.1.1/README.md
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 10:25:47.472729 cocojamboo-2.1.1/cocojamboo/
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)      169 2023-04-29 10:18:07.000000 cocojamboo-2.1.1/cocojamboo/__init__.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     6646 2023-04-29 10:18:09.000000 cocojamboo-2.1.1/cocojamboo/coco_eval2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     8904 2023-04-29 10:18:01.000000 cocojamboo-2.1.1/cocojamboo/coco_utils.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    45829 2023-04-29 07:00:48.000000 cocojamboo-2.1.1/cocojamboo/cocoeval2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     4547 2023-04-29 10:17:58.000000 cocojamboo-2.1.1/cocojamboo/engine2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23337 2023-02-17 12:32:17.000000 cocojamboo-2.1.1/cocojamboo/transforms.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     8388 2023-02-17 12:32:17.000000 cocojamboo-2.1.1/cocojamboo/utils.py
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 10:25:47.474133 cocojamboo-2.1.1/cocojamboo.egg-info/
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 10:25:47.000000 cocojamboo-2.1.1/cocojamboo.egg-info/PKG-INFO
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)      332 2023-04-29 10:25:47.000000 cocojamboo-2.1.1/cocojamboo.egg-info/SOURCES.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)        1 2023-04-29 10:25:47.000000 cocojamboo-2.1.1/cocojamboo.egg-info/dependency_links.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)       11 2023-04-29 10:25:47.000000 cocojamboo-2.1.1/cocojamboo.egg-info/top_level.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)      670 2023-04-29 10:19:56.000000 cocojamboo-2.1.1/pyproject.toml
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)       38 2023-04-29 10:25:47.475504 cocojamboo-2.1.1/setup.cfg
```

### Comparing `cocojamboo-2.1.0/LICENSE` & `cocojamboo-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.1.0/PKG-INFO` & `cocojamboo-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocojamboo
-Version: 2.1.0
+Version: 2.1.1
 Summary: An extension to COCO evaluation metric to provide mAP scores with custom paramters.
 Author: Georgiana Manolache
 License: 
         Attribution-NonCommercial 4.0 International
         
         =======================================================================
```

### Comparing `cocojamboo-2.1.0/cocojamboo/coco_eval2.py` & `cocojamboo-2.1.1/cocojamboo/cocoeval2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,209 +1,7 @@
-import copy
-import io
-from contextlib import redirect_stdout
-
-import numpy as np
-import pycocotools.mask as mask_util
-import torch
-#import utils
-from pycocotools.coco import COCO
-
-#import cocoeval2
-#from cocoeval2 import COCOeval2 # maybe comment out
-
-class CocoEvaluator:
-    def __init__(self, coco_gt, iou_types):
-        if not isinstance(iou_types, (list, tuple)):
-            raise TypeError(f"This constructor expects iou_types of type list or tuple, instead  got {type(iou_types)}")
-        coco_gt = copy.deepcopy(coco_gt)
-        self.coco_gt = coco_gt
-
-        self.iou_types = iou_types
-        self.coco_eval = {}
-        for iou_type in iou_types:
-            self.coco_eval[iou_type] = COCOeval2(coco_gt, iouType=iou_type)
-            
-        self.img_ids = []
-        self.eval_imgs = {k: [] for k in iou_types}
-        self.stats = []
-
-    def update(self, predictions):
-        img_ids = list(np.unique(list(predictions.keys())))
-        self.img_ids.extend(img_ids)
-
-        for iou_type in self.iou_types:
-            results = self.prepare(predictions, iou_type)
-            with redirect_stdout(io.StringIO()):
-                coco_dt = COCO.loadRes(self.coco_gt, results) if results else COCO()
-            coco_eval = self.coco_eval[iou_type]
-
-            coco_eval.cocoDt = coco_dt
-            coco_eval.params.imgIds = list(img_ids)
-            img_ids, eval_imgs = evaluate(coco_eval)
-
-            self.eval_imgs[iou_type].append(eval_imgs)
-
-    def synchronize_between_processes(self):
-        for iou_type in self.iou_types:
-            self.eval_imgs[iou_type] = np.concatenate(self.eval_imgs[iou_type], 2)
-            create_common_coco_eval(self.coco_eval[iou_type], self.img_ids, self.eval_imgs[iou_type])
-
-    def accumulate(self):
-        for coco_eval in self.coco_eval.values():
-            coco_eval.accumulate()
-
-    def summarize(self, ap=None, iouThr=None, areaRng=None, maxDets=None, classes=None, labels=None):
-        for iou_type, coco_eval in self.coco_eval.items():
-            print(f"IoU metric: {iou_type}")
-            self.stats = coco_eval.summarize(ap, iouThr, areaRng, maxDets, classes, labels)
-        
-    def prepare(self, predictions, iou_type):
-        if iou_type == "bbox":
-            return self.prepare_for_coco_detection(predictions)
-        if iou_type == "segm":
-            return self.prepare_for_coco_segmentation(predictions)
-        if iou_type == "keypoints":
-            return self.prepare_for_coco_keypoint(predictions)
-        raise ValueError(f"Unknown iou type {iou_type}")
-
-    def prepare_for_coco_detection(self, predictions):
-        coco_results = []
-        for original_id, prediction in predictions.items():
-            if len(prediction) == 0:
-                continue
-
-            boxes = prediction["boxes"]
-            boxes = convert_to_xywh(boxes).tolist()
-            scores = prediction["scores"].tolist()
-            labels = prediction["labels"].tolist()
-
-            coco_results.extend(
-                [
-                    {
-                        "image_id": original_id,
-                        "category_id": labels[k],
-                        "bbox": box,
-                        "score": scores[k],
-                    }
-                    for k, box in enumerate(boxes)
-                ]
-            )
-        return coco_results
-
-    def prepare_for_coco_segmentation(self, predictions):
-        coco_results = []
-        for original_id, prediction in predictions.items():
-            if len(prediction) == 0:
-                continue
-
-            scores = prediction["scores"]
-            labels = prediction["labels"]
-            masks = prediction["masks"]
-
-            masks = masks > 0.5
-
-            scores = prediction["scores"].tolist()
-            labels = prediction["labels"].tolist()
-
-            rles = [
-                mask_util.encode(np.array(mask[0, :, :, np.newaxis], dtype=np.uint8, order="F"))[0] for mask in masks
-            ]
-            for rle in rles:
-                rle["counts"] = rle["counts"].decode("utf-8")
-
-            coco_results.extend(
-                [
-                    {
-                        "image_id": original_id,
-                        "category_id": labels[k],
-                        "segmentation": rle,
-                        "score": scores[k],
-                    }
-                    for k, rle in enumerate(rles)
-                ]
-            )
-        return coco_results
-
-    def prepare_for_coco_keypoint(self, predictions):
-        coco_results = []
-        for original_id, prediction in predictions.items():
-            if len(prediction) == 0:
-                continue
-
-            boxes = prediction["boxes"]
-            boxes = convert_to_xywh(boxes).tolist()
-            scores = prediction["scores"].tolist()
-            labels = prediction["labels"].tolist()
-            keypoints = prediction["keypoints"]
-            keypoints = keypoints.flatten(start_dim=1).tolist()
-
-            coco_results.extend(
-                [
-                    {
-                        "image_id": original_id,
-                        "category_id": labels[k],
-                        "keypoints": keypoint,
-                        "score": scores[k],
-                    }
-                    for k, keypoint in enumerate(keypoints)
-                ]
-            )
-        return coco_results
-
-
-def convert_to_xywh(boxes):
-    xmin, ymin, xmax, ymax = boxes.unbind(1)
-    return torch.stack((xmin, ymin, xmax - xmin, ymax - ymin), dim=1)
-
-
-def merge(img_ids, eval_imgs):
-    all_img_ids = utils.all_gather(img_ids)
-    all_eval_imgs = utils.all_gather(eval_imgs)
-
-    merged_img_ids = []
-    for p in all_img_ids:
-        merged_img_ids.extend(p)
-
-    merged_eval_imgs = []
-    for p in all_eval_imgs:
-        merged_eval_imgs.append(p)
-
-    merged_img_ids = np.array(merged_img_ids)
-    merged_eval_imgs = np.concatenate(merged_eval_imgs, 2)
-
-    # keep only unique (and in sorted order) images
-    merged_img_ids, idx = np.unique(merged_img_ids, return_index=True)
-    merged_eval_imgs = merged_eval_imgs[..., idx]
-
-    return merged_img_ids, merged_eval_imgs
-
-
-def create_common_coco_eval(coco_eval, img_ids, eval_imgs):
-    img_ids, eval_imgs = merge(img_ids, eval_imgs)
-    img_ids = list(img_ids)
-    eval_imgs = list(eval_imgs.flatten())
-
-    coco_eval.evalImgs = eval_imgs
-    coco_eval.params.imgIds = img_ids
-    coco_eval._paramsEval = copy.deepcopy(coco_eval.params)
-
-
-def evaluate(imgs):
-    with redirect_stdout(io.StringIO()):
-        imgs.evaluate()
-    return imgs.params.imgIds, np.asarray(imgs.evalImgs).reshape(-1, len(imgs.params.areaRng), len(imgs.params.imgIds))
-
-
-
-
-
-
-
-
 __author__ = 'tsungyi'
 
 import numpy as np
 import datetime
 import time
 from collections import defaultdict
 import pycocotools.mask as maskUtils
```

### Comparing `cocojamboo-2.1.0/cocojamboo/coco_utils.py` & `cocojamboo-2.1.1/cocojamboo/transforms.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,268 +1,7 @@
-import copy
-import os
-
-import torch
-import torch.utils.data
-import torchvision
-#import transforms as T
-from pycocotools import mask as coco_mask
-from pycocotools.coco import COCO
-
-
-class FilterAndRemapCocoCategories:
-    def __init__(self, categories, remap=True):
-        self.categories = categories
-        self.remap = remap
-
-    def __call__(self, image, target):
-        anno = target["annotations"]
-        anno = [obj for obj in anno if obj["category_id"] in self.categories]
-        if not self.remap:
-            target["annotations"] = anno
-            return image, target
-        anno = copy.deepcopy(anno)
-        for obj in anno:
-            obj["category_id"] = self.categories.index(obj["category_id"])
-        target["annotations"] = anno
-        return image, target
-
-
-def convert_coco_poly_to_mask(segmentations, height, width):
-    masks = []
-    for polygons in segmentations:
-        rles = coco_mask.frPyObjects(polygons, height, width)
-        mask = coco_mask.decode(rles)
-        if len(mask.shape) < 3:
-            mask = mask[..., None]
-        mask = torch.as_tensor(mask, dtype=torch.uint8)
-        mask = mask.any(dim=2)
-        masks.append(mask)
-    if masks:
-        masks = torch.stack(masks, dim=0)
-    else:
-        masks = torch.zeros((0, height, width), dtype=torch.uint8)
-    return masks
-
-
-class ConvertCocoPolysToMask:
-    def __call__(self, image, target):
-        w, h = image.size
-
-        image_id = target["image_id"]
-        image_id = torch.tensor([image_id])
-
-        anno = target["annotations"]
-
-        anno = [obj for obj in anno if obj["iscrowd"] == 0]
-
-        boxes = [obj["bbox"] for obj in anno]
-        # guard against no boxes via resizing
-        boxes = torch.as_tensor(boxes, dtype=torch.float32).reshape(-1, 4)
-        boxes[:, 2:] += boxes[:, :2]
-        boxes[:, 0::2].clamp_(min=0, max=w)
-        boxes[:, 1::2].clamp_(min=0, max=h)
-
-        classes = [obj["category_id"] for obj in anno]
-        classes = torch.tensor(classes, dtype=torch.int64)
-
-        segmentations = [obj["segmentation"] for obj in anno]
-        masks = convert_coco_poly_to_mask(segmentations, h, w)
-
-        keypoints = None
-        if anno and "keypoints" in anno[0]:
-            keypoints = [obj["keypoints"] for obj in anno]
-            keypoints = torch.as_tensor(keypoints, dtype=torch.float32)
-            num_keypoints = keypoints.shape[0]
-            if num_keypoints:
-                keypoints = keypoints.view(num_keypoints, -1, 3)
-
-        keep = (boxes[:, 3] > boxes[:, 1]) & (boxes[:, 2] > boxes[:, 0])
-        boxes = boxes[keep]
-        classes = classes[keep]
-        masks = masks[keep]
-        if keypoints is not None:
-            keypoints = keypoints[keep]
-
-        target = {}
-        target["boxes"] = boxes
-        target["labels"] = classes
-        target["masks"] = masks
-        target["image_id"] = image_id
-        if keypoints is not None:
-            target["keypoints"] = keypoints
-
-        # for conversion to coco api
-        area = torch.tensor([obj["area"] for obj in anno])
-        iscrowd = torch.tensor([obj["iscrowd"] for obj in anno])
-        target["area"] = area
-        target["iscrowd"] = iscrowd
-
-        return image, target
-
-
-def _coco_remove_images_without_annotations(dataset, cat_list=None):
-    def _has_only_empty_bbox(anno):
-        return all(any(o <= 1 for o in obj["bbox"][2:]) for obj in anno)
-
-    def _count_visible_keypoints(anno):
-        return sum(sum(1 for v in ann["keypoints"][2::3] if v > 0) for ann in anno)
-
-    min_keypoints_per_image = 10
-
-    def _has_valid_annotation(anno):
-        # if it's empty, there is no annotation
-        if len(anno) == 0:
-            return False
-        # if all boxes have close to zero area, there is no annotation
-        if _has_only_empty_bbox(anno):
-            return False
-        # keypoints task have a slight different criteria for considering
-        # if an annotation is valid
-        if "keypoints" not in anno[0]:
-            return True
-        # for keypoint detection tasks, only consider valid images those
-        # containing at least min_keypoints_per_image
-        if _count_visible_keypoints(anno) >= min_keypoints_per_image:
-            return True
-        return False
-
-    if not isinstance(dataset, torchvision.datasets.CocoDetection):
-        raise TypeError(
-            f"This function expects dataset of type torchvision.datasets.CocoDetection, instead  got {type(dataset)}"
-        )
-    ids = []
-    for ds_idx, img_id in enumerate(dataset.ids):
-        ann_ids = dataset.coco.getAnnIds(imgIds=img_id, iscrowd=None)
-        anno = dataset.coco.loadAnns(ann_ids)
-        if cat_list:
-            anno = [obj for obj in anno if obj["category_id"] in cat_list]
-        if _has_valid_annotation(anno):
-            ids.append(ds_idx)
-
-    dataset = torch.utils.data.Subset(dataset, ids)
-    return dataset
-
-
-def convert_to_coco_api(ds):
-    coco_ds = COCO()
-    # annotation IDs need to start at 1, not 0, see torchvision issue #1530
-    ann_id = 1
-    dataset = {"images": [], "categories": [], "annotations": []}
-    categories = set()
-    for img_idx in range(len(ds)):
-        # find better way to get target
-        # targets = ds.get_annotations(img_idx)
-        img, targets = ds[img_idx]
-        image_id = targets["image_id"].item()
-        img_dict = {}
-        img_dict["id"] = image_id
-        img_dict["height"] = img.shape[-2]
-        img_dict["width"] = img.shape[-1]
-        dataset["images"].append(img_dict)
-        bboxes = targets["boxes"].clone()
-        bboxes[:, 2:] -= bboxes[:, :2]
-        bboxes = bboxes.tolist()
-        labels = targets["labels"].tolist()
-        areas = targets["area"].tolist()
-        iscrowd = targets["iscrowd"].tolist()
-        if "masks" in targets:
-            masks = targets["masks"]
-            # make masks Fortran contiguous for coco_mask
-            masks = masks.permute(0, 2, 1).contiguous().permute(0, 2, 1)
-        if "keypoints" in targets:
-            keypoints = targets["keypoints"]
-            keypoints = keypoints.reshape(keypoints.shape[0], -1).tolist()
-        num_objs = len(bboxes)
-        for i in range(num_objs):
-            ann = {}
-            ann["image_id"] = image_id
-            ann["bbox"] = bboxes[i]
-            ann["category_id"] = labels[i]
-            categories.add(labels[i])
-            ann["area"] = areas[i]
-            ann["iscrowd"] = iscrowd[i]
-            ann["id"] = ann_id
-            if "masks" in targets:
-                ann["segmentation"] = coco_mask.encode(masks[i].numpy())
-            if "keypoints" in targets:
-                ann["keypoints"] = keypoints[i]
-                ann["num_keypoints"] = sum(k != 0 for k in keypoints[i][2::3])
-            dataset["annotations"].append(ann)
-            ann_id += 1
-    dataset["categories"] = [{"id": i} for i in sorted(categories)]
-    coco_ds.dataset = dataset
-    coco_ds.createIndex()
-    return coco_ds
-
-
-def get_coco_api_from_dataset(dataset):
-    for _ in range(10):
-        if isinstance(dataset, torchvision.datasets.CocoDetection):
-            break
-        if isinstance(dataset, torch.utils.data.Subset):
-            dataset = dataset.dataset
-    if isinstance(dataset, torchvision.datasets.CocoDetection):
-        return dataset.coco
-    return convert_to_coco_api(dataset)
-
-
-class CocoDetection(torchvision.datasets.CocoDetection):
-    def __init__(self, img_folder, ann_file, transforms):
-        super().__init__(img_folder, ann_file)
-        self._transforms = transforms
-
-    def __getitem__(self, idx):
-        img, target = super().__getitem__(idx)
-        image_id = self.ids[idx]
-        target = dict(image_id=image_id, annotations=target)
-        if self._transforms is not None:
-            img, target = self._transforms(img, target)
-        return img, target
-
-
-def get_coco(root, image_set, transforms, mode="instances"):
-    anno_file_template = "{}_{}2017.json"
-    PATHS = {
-        "train": ("train2017", os.path.join("annotations", anno_file_template.format(mode, "train"))),
-        "val": ("val2017", os.path.join("annotations", anno_file_template.format(mode, "val"))),
-        # "train": ("val2017", os.path.join("annotations", anno_file_template.format(mode, "val")))
-    }
-
-    t = [ConvertCocoPolysToMask()]
-
-    if transforms is not None:
-        t.append(transforms)
-    transforms = Compose(t)
-
-    img_folder, ann_file = PATHS[image_set]
-    img_folder = os.path.join(root, img_folder)
-    ann_file = os.path.join(root, ann_file)
-
-    dataset = CocoDetection(img_folder, ann_file, transforms=transforms)
-
-    if image_set == "train":
-        dataset = _coco_remove_images_without_annotations(dataset)
-
-    # dataset = torch.utils.data.Subset(dataset, [i for i in range(500)])
-
-    return dataset
-
-
-def get_coco_kp(root, image_set, transforms):
-    return get_coco(root, image_set, transforms, mode="person_keypoints")
-
-
-
-
-
-
-
-
-
 from typing import Dict, List, Optional, Tuple, Union
 
 import torch
 import torchvision
 from torch import nn, Tensor
 from torchvision import ops
 from torchvision.transforms import functional as F, InterpolationMode, transforms as T
```

### Comparing `cocojamboo-2.1.0/cocojamboo/engine2.py` & `cocojamboo-2.1.1/cocojamboo/engine2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import math
 import sys
 import time
 
 import torch
 import torchvision.models.detection.mask_rcnn
-#import utils
-from coco_eval2 import CocoEvaluator
-from coco_utils import get_coco_api_from_dataset
+from .utils import *
+from .coco_eval2 import CocoEvaluator
+from .coco_utils import get_coco_api_from_dataset
 
 
 def train_one_epoch(model, optimizer, data_loader, device, epoch, print_freq, scaler=None):
     model.train()
-    metric_logger = utils.MetricLogger(delimiter="  ")
-    metric_logger.add_meter("lr", utils.SmoothedValue(window_size=1, fmt="{value:.6f}"))
+    metric_logger = MetricLogger(delimiter="  ")
+    metric_logger.add_meter("lr", SmoothedValue(window_size=1, fmt="{value:.6f}"))
     header = f"Epoch: [{epoch}]"
 
     lr_scheduler = None
     if epoch == 0:
         warmup_factor = 1.0 / 1000
         warmup_iters = min(1000, len(data_loader) - 1)
 
@@ -28,15 +28,15 @@
         images = list(image.to(device) for image in images)
         targets = [{k: v.to(device) for k, v in t.items()} for t in targets]
         with torch.cuda.amp.autocast(enabled=scaler is not None):
             loss_dict = model(images, targets)
             losses = sum(loss for loss in loss_dict.values())
 
         # reduce losses over all GPUs for logging purposes
-        loss_dict_reduced = utils.reduce_dict(loss_dict)
+        loss_dict_reduced = reduce_dict(loss_dict)
         losses_reduced = sum(loss for loss in loss_dict_reduced.values())
 
         loss_value = losses_reduced.item()
 
         if not math.isfinite(loss_value):
             print(f"Loss is {loss_value}, stopping training")
             print(loss_dict_reduced)
@@ -75,15 +75,15 @@
 @torch.inference_mode()
 def evaluate(model, data_loader, device, ap=None, iouThr=None, areaRng=None, maxDets=None, classes=None, labels=None):
     n_threads = torch.get_num_threads()
     # FIXME remove this and make paste_masks_in_image run on the GPU
     torch.set_num_threads(1)
     cpu_device = torch.device("cpu")
     model.eval()
-    metric_logger = utils.MetricLogger(delimiter="  ")
+    metric_logger = MetricLogger(delimiter="  ")
     header = "Test:"
 
     coco = get_coco_api_from_dataset(data_loader.dataset)
     iou_types = _get_iou_types(model)
     coco_evaluator = CocoEvaluator(coco, iou_types)
 
     for images, targets in metric_logger.log_every(data_loader, 100, header):
```

### Comparing `cocojamboo-2.1.0/cocojamboo/utils.py` & `cocojamboo-2.1.1/cocojamboo/utils.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-2.1.0/cocojamboo.egg-info/PKG-INFO` & `cocojamboo-2.1.1/cocojamboo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocojamboo
-Version: 2.1.0
+Version: 2.1.1
 Summary: An extension to COCO evaluation metric to provide mAP scores with custom paramters.
 Author: Georgiana Manolache
 License: 
         Attribution-NonCommercial 4.0 International
         
         =======================================================================
```

### Comparing `cocojamboo-2.1.0/pyproject.toml` & `cocojamboo-2.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "numpy", "wheel", "pycocotools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cocojamboo"
-version = "2.1.0"
+version = "2.1.1"
 description = "An extension to COCO evaluation metric to provide mAP scores with custom paramters."
 readme = "README.md"
 authors = [{ name = "Georgiana Manolache" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: Free for non-commercial use",
     "Programming Language :: Python",
```

