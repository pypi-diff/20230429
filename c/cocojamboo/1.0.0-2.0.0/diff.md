# Comparing `tmp/cocojamboo-1.0.0.tar.gz` & `tmp/cocojamboo-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocojamboo-1.0.0.tar", last modified: Wed Apr 12 07:22:49 2023, max compression
+gzip compressed data, was "cocojamboo-2.0.0.tar", last modified: Sat Apr 29 08:36:41 2023, max compression
```

## Comparing `cocojamboo-1.0.0.tar` & `cocojamboo-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-12 07:22:49.044160 cocojamboo-1.0.0/
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)    19334 2023-01-10 14:44:25.000000 cocojamboo-1.0.0/LICENSE
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-12 07:22:49.043241 cocojamboo-1.0.0/PKG-INFO
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)      122 2023-03-31 12:26:52.000000 cocojamboo-1.0.0/README.md
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-12 07:22:49.038777 cocojamboo-1.0.0/cocojamboo/
--rw-rw-r--   0 georgianamanolache   (501) staff       (20)       98 2023-04-12 07:04:01.000000 cocojamboo-1.0.0/cocojamboo/__init__.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     6548 2023-03-25 21:14:27.000000 cocojamboo-1.0.0/cocojamboo/coco_eval2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     8893 2023-02-17 12:32:17.000000 cocojamboo-1.0.0/cocojamboo/coco_utils.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    39402 2023-03-31 12:44:20.000000 cocojamboo-1.0.0/cocojamboo/cocoeval2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     4492 2023-03-31 12:01:07.000000 cocojamboo-1.0.0/cocojamboo/engine2.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23337 2023-02-17 12:32:17.000000 cocojamboo-1.0.0/cocojamboo/transforms.py
--rw-r--r--   0 georgianamanolache   (501) staff       (20)     8388 2023-02-17 12:32:17.000000 cocojamboo-1.0.0/cocojamboo/utils.py
-drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-12 07:22:49.041925 cocojamboo-1.0.0/cocojamboo.egg-info/
--rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-12 07:22:49.000000 cocojamboo-1.0.0/cocojamboo.egg-info/PKG-INFO
--rw-r--r--   0 georgianamanolache   (501) staff       (20)      332 2023-04-12 07:22:49.000000 cocojamboo-1.0.0/cocojamboo.egg-info/SOURCES.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)        1 2023-04-12 07:22:49.000000 cocojamboo-1.0.0/cocojamboo.egg-info/dependency_links.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)       11 2023-04-12 07:22:49.000000 cocojamboo-1.0.0/cocojamboo.egg-info/top_level.txt
--rw-r--r--   0 georgianamanolache   (501) staff       (20)      646 2023-04-12 07:08:25.000000 cocojamboo-1.0.0/pyproject.toml
--rw-r--r--   0 georgianamanolache   (501) staff       (20)       38 2023-04-12 07:22:49.044369 cocojamboo-1.0.0/setup.cfg
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 08:36:41.640563 cocojamboo-2.0.0/
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)    19334 2023-01-10 14:44:25.000000 cocojamboo-2.0.0/LICENSE
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 08:36:41.640054 cocojamboo-2.0.0/PKG-INFO
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)      122 2023-03-31 12:26:52.000000 cocojamboo-2.0.0/README.md
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 08:36:41.637594 cocojamboo-2.0.0/cocojamboo/
+-rw-rw-r--   0 georgianamanolache   (501) staff       (20)       98 2023-04-29 08:21:40.000000 cocojamboo-2.0.0/cocojamboo/__init__.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     6637 2023-04-28 20:14:14.000000 cocojamboo-2.0.0/cocojamboo/coco_eval2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     8893 2023-02-17 12:32:17.000000 cocojamboo-2.0.0/cocojamboo/coco_utils.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    45829 2023-04-29 07:00:48.000000 cocojamboo-2.0.0/cocojamboo/cocoeval2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     4561 2023-04-28 20:14:17.000000 cocojamboo-2.0.0/cocojamboo/engine2.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23337 2023-02-17 12:32:17.000000 cocojamboo-2.0.0/cocojamboo/transforms.py
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)     8388 2023-02-17 12:32:17.000000 cocojamboo-2.0.0/cocojamboo/utils.py
+drwxr-xr-x   0 georgianamanolache   (501) staff       (20)        0 2023-04-29 08:36:41.639250 cocojamboo-2.0.0/cocojamboo.egg-info/
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)    23184 2023-04-29 08:36:41.000000 cocojamboo-2.0.0/cocojamboo.egg-info/PKG-INFO
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)      332 2023-04-29 08:36:41.000000 cocojamboo-2.0.0/cocojamboo.egg-info/SOURCES.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)        1 2023-04-29 08:36:41.000000 cocojamboo-2.0.0/cocojamboo.egg-info/dependency_links.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)       11 2023-04-29 08:36:41.000000 cocojamboo-2.0.0/cocojamboo.egg-info/top_level.txt
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)      661 2023-04-29 08:27:05.000000 cocojamboo-2.0.0/pyproject.toml
+-rw-r--r--   0 georgianamanolache   (501) staff       (20)       38 2023-04-29 08:36:41.640678 cocojamboo-2.0.0/setup.cfg
```

### Comparing `cocojamboo-1.0.0/LICENSE` & `cocojamboo-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cocojamboo-1.0.0/PKG-INFO` & `cocojamboo-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocojamboo
-Version: 1.0.0
+Version: 2.0.0
 Summary: An extension to COCO evaluation metric to provide mAP scores with custom paramters.
 Author: Georgiana Manolache
 License: 
         Attribution-NonCommercial 4.0 International
         
         =======================================================================
```

### Comparing `cocojamboo-1.0.0/cocojamboo/coco_eval2.py` & `cocojamboo-2.0.0/cocojamboo/coco_eval2.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from contextlib import redirect_stdout
 
 import numpy as np
 import pycocotools.mask as mask_util
 import torch
 import utils
 from pycocotools.coco import COCO
-from cocoeval2 import COCOeval2
+from cocoeval2 import COCOeval2 # maybe comment out
 
 
 class CocoEvaluator:
     def __init__(self, coco_gt, iou_types):
         if not isinstance(iou_types, (list, tuple)):
             raise TypeError(f"This constructor expects iou_types of type list or tuple, instead  got {type(iou_types)}")
         coco_gt = copy.deepcopy(coco_gt)
@@ -47,18 +47,18 @@
             self.eval_imgs[iou_type] = np.concatenate(self.eval_imgs[iou_type], 2)
             create_common_coco_eval(self.coco_eval[iou_type], self.img_ids, self.eval_imgs[iou_type])
 
     def accumulate(self):
         for coco_eval in self.coco_eval.values():
             coco_eval.accumulate()
 
-    def summarize(self, ap=None, iouThr=None, labels=None):
+    def summarize(self, ap=None, iouThr=None, areaRng=None, maxDets=None, classes=None, labels=None):
         for iou_type, coco_eval in self.coco_eval.items():
             print(f"IoU metric: {iou_type}")
-            self.stats = coco_eval.summarize(ap, iouThr, labels)
+            self.stats = coco_eval.summarize(ap, iouThr, areaRng, maxDets, classes, labels)
         
     def prepare(self, predictions, iou_type):
         if iou_type == "bbox":
             return self.prepare_for_coco_detection(predictions)
         if iou_type == "segm":
             return self.prepare_for_coco_segmentation(predictions)
         if iou_type == "keypoints":
```

### Comparing `cocojamboo-1.0.0/cocojamboo/coco_utils.py` & `cocojamboo-2.0.0/cocojamboo/coco_utils.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-1.0.0/cocojamboo/cocoeval2.py` & `cocojamboo-2.0.0/cocojamboo/cocoeval2.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     #
     # See also coco, mask, pycocoDemo, pycocoEvalDemo
     #
     # Microsoft COCO Toolbox.      version 2.0
     # Data, paper, and tutorials available at:  http://mscoco.org/
     # Code written by Piotr Dollar and Tsung-Yi Lin, 2015.
     # Licensed under the Simplified BSD License [see coco/license.txt]
-    def __init__(self, cocoGt=None, cocoDt=None, iouType='segm', class_names = None):
+    def __init__(self, cocoGt=None, cocoDt=None, iouType='segm'):
         '''
         Initialize CocoEval using coco APIs for gt and dt
         :param cocoGt: coco object with ground truth annotations
         :param cocoDt: coco object with detection results
         :param class_names: list of class names 
         :return: None
         '''
@@ -77,15 +77,14 @@
         self._paramsEval = {}               # parameters for evaluation
         self.stats = []                     # result summarization
         self.stats_info = []
         self.ious = {}                      # ious between all gts and dts
         if not cocoGt is None:
             self.params.imgIds = sorted(cocoGt.getImgIds())
             self.params.catIds = sorted(cocoGt.getCatIds())
-        self.class_names = class_names               # class names given
 
 
     def _prepare(self):
         '''
         Prepare ._gts and ._dts for evaluation based on params
         :return: None
         '''
@@ -418,33 +417,48 @@
             'precision': precision,
             'recall':   recall,
             'scores': scores,
         }
         toc = time.time()
         print('DONE (t={:0.2f}s).'.format( toc-tic))
 
-    def summarize(self, ap = None, iouThr=None, labels = None):
+    def summarize(self, ap = None, iouThr=None, givenAreaRng=None, givenMaxDets=None, classes = None, labels = None):
         '''
         Compute and display summary metrics for evaluation results.
 
         ap = [1, 0] 1 for AP, AR otherwise
         iouThr = [.5, .75, .95]
-        lables = [0,1,....n] array of indexes, or None otherwise 
+        classes = [0,1,...n] array of indexes, or None otherwise 
+        labels = ['name0', 'name1',...'namen'] or None otherwise
+        richOutout = [True, False], False by default
 
         '''
-        def _summarize( ap=1, iouThr=None, areaRng='all', maxDets=100, cat=-1):
+        def _summarize( ap=1, iouThr=None, areaRng='all', maxDets=100, cat=-1, iStr=None, iStrCat=None):
+            
             p = self.params
-            iStr = ' {:<18} {} @[ IoU={:<9} | area={:>6s} | maxDets={:>3d} ]'
+
+            #base
+            if iStr is None:
+                iStr = ' {:<18} {} @[ IoU={IoUStr:<9} | area={areaStr:>6s} | maxDets={maxDetsStr:>3d} ]'
+    
             titleStr = 'Average Precision' if ap == 1 else 'Average Recall'
             typeStr = '(AP)' if ap==1 else '(AR)'
+
             iouStr = '{:0.2f}:{:0.2f}'.format(p.iouThrs[0], p.iouThrs[-1]) \
                 if iouThr is None else '{:0.2f}'.format(iouThr)
 
             aind = [i for i, aRng in enumerate(p.areaRngLbl) if aRng == areaRng]
             mind = [i for i, mDet in enumerate(p.maxDets) if mDet == maxDets]
+
+            if givenAreaRng is not None:
+                aind = [i for i, aRng in enumerate(p.areaRngLbl) if aRng == givenAreaRng]
+
+            if givenMaxDets is not None:
+                mind = [i for i, mDet in enumerate(p.maxDets) if mDet == givenMaxDets]
+            
             if ap == 1:
                 # dimension of precision: [TxRxKxAxM]
                 s = self.eval['precision']
                 # IoU
                 if iouThr is not None:
                     t = np.where(iouThr == p.iouThrs)[0]
                     s = s[t]
@@ -469,49 +483,50 @@
                 # if ap == 1:
                 #     for i in range(num_classes):
                 #         #print('category : {0} : {1}'.format(i, np.mean(s[:,:,i,:])))
                 #         avg_ap += np.mean(s[:,:,i,:]) # same as mean_s 
                 #     #print('(all categories) mAP : {}'.format(avg_ap / num_classes)) # same as mean_s 
 
 ###########################################################################################
-
-            iStrCat = ' {:<18} {} @[ IoU={:<9} | area={:>6s} | maxDets={:>3d} | class={} ]'
+            
             info = ''
-
             iStrValue = '{} = {:0.3f}'
 
+            if iStrCat is None:
+                iStrCat = ' {:<18} {} @[ IoU={IoUStr:<9} | area={areaStr:>6s} | maxDets={maxDetsStr:>3d} | label={labelStr} ]'
+
             if cat == -1:
-                info = iStr.format(titleStr, typeStr, iouStr, areaRng, maxDets)
+                info = iStr.format(titleStr, typeStr, IoUStr=iouStr, areaStr=areaRng, maxDetsStr=maxDets)
                 print(iStrValue.format(info, mean_s))
                 return info, mean_s
             
             else:
                 if ap==1: 
                     # AP
                     value = np.mean(s[:,:,cat,:])
 
-                    if self.class_names is None: # check if class names is given
-                        info = iStrCat.format(titleStr, typeStr, iouStr, areaRng, maxDets, cat)
+                    if labels is None: # check if class names is given
+                        info = iStrCat.format(titleStr, typeStr, IoUStr=iouStr, areaStr=areaRng, maxDetsStr=maxDets, labelStr=cat)
                         print(iStrValue.format(info, value))
                         return info, value
                     else:
-                        info = iStrCat.format(titleStr, typeStr, iouStr, areaRng, maxDets, self.class_names[cat])
+                        info = iStrCat.format(titleStr, typeStr, IoUStr=iouStr, areaStr=areaRng, maxDetsStr=maxDets, labelStr=labels[cat])
                         print(iStrValue.format(info, value))
                         return info, value
                 
                 else: 
                     #AR
                     value = np.mean(s[:,cat,:])
 
-                    if self.class_names is None: # check if class names is given
-                        info = iStrCat.format(titleStr, typeStr, iouStr, areaRng, maxDets, cat)
+                    if labels is None: # check if class names is given
+                        info = iStrCat.format(titleStr, typeStr, IoUStr=iouStr, areaStr=areaRng, maxDetsStr=maxDets, labelStr=cat)
                         print(iStrValue.format(info, value))
                         return info, value
                     else: 
-                        info = iStrCat.format(titleStr, typeStr, iouStr, areaRng, maxDets, self.class_names[cat])
+                        info = iStrCat.format(titleStr, typeStr, IoUStr=iouStr, areaStr=areaRng, maxDetsStr=maxDets, labelStr=labels[cat])
                         print(iStrValue.format(info, value))
                         return info, value
 
         def _summarizeDets():
 
             stats = np.zeros((12 + len(self.params.catIds) * 12)) # added classes * 12 for AP and AR 
             info_stats = [x for x in range(12 + len(self.params.catIds) * 12)]
@@ -544,25 +559,28 @@
                 info_stats[index + 9], stats[index + 9] = _summarize(0, areaRng='small', maxDets=self.params.maxDets[2], cat = i)
                 info_stats[index + 10], stats[index + 10] = _summarize(0, areaRng='medium', maxDets=self.params.maxDets[2], cat = i)
                 info_stats[index + 11], stats[index + 11] = _summarize(0, areaRng='large', maxDets=self.params.maxDets[2], cat = i)
                 index += 12
 
             return info_stats, stats
         
-        def _summarizeCustom(ap=None, iouThr=None, labels=None):
+        def _summarizeCustomCOCO(ap=None, iouThr=None, classes=None):
 
             num_cat = 0 # number of categories
             cat_indexs = [] #index of the categories
 
-            if labels is None:
-                num_cat = self.params.catIds
-                cat_indexs = range(len(self.params.catIds))
+            if classes is None:
+                num_cat = len(self.params.catIds)
+                cat_indexs = range(num_cat)
             else:
-                num_cat = len(labels)
-                cat_indexs = labels
+                num_cat = len(classes)
+                cat_indexs = classes
+
+            iStr = ' {:<18} {} @[ area={areaStr:>6s} | maxDets={maxDetsStr:>3d} ]'
+            iStrCat = ' {:<18} {} @[ area={areaStr:>6s} | maxDets={maxDetsStr:>3d} | label={labelStr} ]'
         
             if ap == 1 and iouThr is None:
                 stats = np.zeros((6 + num_cat*6)) # added classes * 6 for AP and AR 
                 info_stats =[x for x in range(6 + num_cat * 6)]
 
                 info_stats[0], stats[0] = _summarize(1)
                 info_stats[1], stats[1] = _summarize(1, iouThr=.5, maxDets=self.params.maxDets[2])
@@ -607,86 +625,184 @@
 
                 return info_stats, stats
             
             elif ap == 1 and iouThr is not None: # 4 rows
 
                 stats = np.zeros((4 + num_cat * 4)) # added classes * 4 for AP and AR
                 info_stats =[x for x in range(4 + num_cat * 4)]
-
-                info_stats[0], stats[0] = _summarize(1, iouThr=iouThr, maxDets=self.params.maxDets[2])
-                info_stats[1], stats[1] = _summarize(1, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2])
-                info_stats[2], stats[2] = _summarize(1, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2])
-                info_stats[3], stats[3] = _summarize(1, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2])
+              
+                info_stats[0], stats[0] = _summarize(1, iouThr=iouThr, maxDets=self.params.maxDets[2], iStr=iStr)
+                info_stats[1], stats[1] = _summarize(1, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2], iStr=iStr)
+                info_stats[2], stats[2] = _summarize(1, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2], iStr=iStr)
+                info_stats[3], stats[3] = _summarize(1, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2], iStr=iStr)
                 index = 4
 
                 for i in cat_indexs:
-                    info_stats[index + 0], stats[index + 0] = _summarize(1, iouThr=iouThr, maxDets=self.params.maxDets[2], cat = i)
-                    info_stats[index + 1], stats[index + 1] = _summarize(1, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2], cat = i)
-                    info_stats[index + 2], stats[index + 2] = _summarize(1, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2], cat = i)
-                    info_stats[index + 3], stats[index + 3] = _summarize(1, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2], cat = i)
+                    info_stats[index + 0], stats[index + 0] = _summarize(1, iouThr=iouThr, maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 1], stats[index + 1] = _summarize(1, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 2], stats[index + 2] = _summarize(1, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 3], stats[index + 3] = _summarize(1, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
                     index += 4
 
                 return info_stats, stats
             
             elif ap == 0 and iouThr is not None:
 
                 stats = np.zeros((6 + num_cat * 6)) # added classes * 6 for AP and AR 
                 info_stats =[x for x in range(6 + num_cat * 6)]
-
-                info_stats[0], stats[0] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[0])
-                info_stats[1], stats[1] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[1])
-                info_stats[2], stats[2] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[2])
-                info_stats[3], stats[3] = _summarize(0, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2])
-                info_stats[4], stats[4] = _summarize(0, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2])
-                info_stats[5], stats[5] = _summarize(0, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2])
+                
+                info_stats[0], stats[0] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[0], iStr=iStr)
+                info_stats[1], stats[1] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[1], iStr=iStr)
+                info_stats[2], stats[2] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[2], iStr=iStr)
+                info_stats[3], stats[3] = _summarize(0, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2], iStr=iStr)
+                info_stats[4], stats[4] = _summarize(0, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2], iStr=iStr)
+                info_stats[5], stats[5] = _summarize(0, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2], iStr=iStr)
                 index = 6
                 
                 for i in cat_indexs:
-                    info_stats[index + 0], stats[index + 0] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[0], cat = i)
-                    info_stats[index + 1], stats[index + 1] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[1], cat = i)
-                    info_stats[index + 2], stats[index + 2] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[2], cat = i)
-                    info_stats[index + 3], stats[index + 3] = _summarize(0, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2], cat = i)
-                    info_stats[index + 4], stats[index + 4] = _summarize(0, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2], cat = i)
-                    info_stats[index + 5], stats[index + 5] = _summarize(0, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2], cat = i)
+                    info_stats[index + 0], stats[index + 0] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[0], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 1], stats[index + 1] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[1], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 2], stats[index + 2] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 3], stats[index + 3] = _summarize(0, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 4], stats[index + 4] = _summarize(0, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 5], stats[index + 5] = _summarize(0, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
                     index += 6
 
                 return info_stats, stats
             
             else:
+
                 stats = np.zeros((10 + num_cat * 10)) # added classes * 10 for AP and AR 
                 info_stats =[x for x in range(10 + num_cat * 10)]
-
-                info_stats[0], stats[0] = _summarize(1, iouThr=iouThr, maxDets=self.params.maxDets[2])
-                info_stats[1], stats[1] = _summarize(1, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2])
-                info_stats[2], stats[2] = _summarize(1, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2])
-                info_stats[3], stats[3] = _summarize(1, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2])
-                info_stats[4], stats[4] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[0])
-                info_stats[5], stats[5] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[1])
-                info_stats[5], stats[6] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[2])
-                info_stats[6], stats[7] = _summarize(0, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2])
-                info_stats[8], stats[8] = _summarize(0, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2])
-                info_stats[9], stats[9] = _summarize(0, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2])
+                
+                info_stats[0], stats[0] = _summarize(1, iouThr=iouThr, maxDets=self.params.maxDets[2], iStr=iStr)
+                info_stats[1], stats[1] = _summarize(1, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2], iStr=iStr)
+                info_stats[2], stats[2] = _summarize(1, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2], iStr=iStr)
+                info_stats[3], stats[3] = _summarize(1, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2], iStr=iStr)
+                info_stats[4], stats[4] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[0], iStr=iStr)
+                info_stats[5], stats[5] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[1], iStr=iStr)
+                info_stats[5], stats[6] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[2], iStr=iStr)
+                info_stats[6], stats[7] = _summarize(0, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2], iStr=iStr)
+                info_stats[8], stats[8] = _summarize(0, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2], iStr=iStr)
+                info_stats[9], stats[9] = _summarize(0, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2], iStr=iStr)
                 
                 index = 10
             
                 for i in cat_indexs:
-                    info_stats[index + 0], stats[index + 0] = _summarize(1, iouThr=iouThr, maxDets=self.params.maxDets[2], cat = i)
-                    info_stats[index + 1], stats[index + 1] = _summarize(1, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2], cat = i)
-                    info_stats[index + 2], stats[index + 2] = _summarize(1, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2], cat = i)
-                    info_stats[index + 3], stats[index + 3] = _summarize(1, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2], cat = i)
-                    info_stats[index + 4], stats[index + 4] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[0], cat = i)
-                    info_stats[index + 5], stats[index + 5] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[1], cat = i)
-                    info_stats[index + 6], stats[index + 6] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[2], cat = i)
-                    info_stats[index + 7], stats[index + 7] = _summarize(0, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2], cat = i)
-                    info_stats[index + 8], stats[index + 8] = _summarize(0, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2], cat = i)
-                    info_stats[index + 9], stats[index + 9] = _summarize(0, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2], cat = i)
+                    info_stats[index + 0], stats[index + 0] = _summarize(1, iouThr=iouThr, maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 1], stats[index + 1] = _summarize(1, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 2], stats[index + 2] = _summarize(1, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 3], stats[index + 3] = _summarize(1, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 4], stats[index + 4] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[0], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 5], stats[index + 5] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[1], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 6], stats[index + 6] = _summarize(0, iouThr=iouThr, maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 7], stats[index + 7] = _summarize(0, iouThr=iouThr, areaRng='small', maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 8], stats[index + 8] = _summarize(0, iouThr=iouThr, areaRng='medium', maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
+                    info_stats[index + 9], stats[index + 9] = _summarize(0, iouThr=iouThr, areaRng='large', maxDets=self.params.maxDets[2], cat = i, iStrCat=iStrCat)
                     index += 10
 
                 return info_stats, stats
 
+        def _summarizeCustom(ap=None, iouThr=None, areaRng='all', maxDets=10, classes=None):
+            
+            num_cat = 0 # number of categories
+            cat_indexs = [] #index of the categories
+
+            if classes is None:
+                num_cat = len(self.params.catIds)
+                cat_indexs = range(num_cat)
+            else:
+                num_cat = len(classes)
+                cat_indexs = classes
+
+            iStr = ' {:<18} {} '
+            iStrCat = ' {:<18} {} @[ label={labelStr} ]'
+
+            if ap == 1 and iouThr is None:
+                stats = np.zeros((3 + num_cat *  3)) # added classes * 6 for AP and AR 
+                info_stats =[x for x in range(3 + num_cat * 3)]
+                
+                iStr = ' {:<18} {} @[ IoU={IoUStr:<9} ]'
+                iStrCat = ' {:<18} {} @[ IoU={IoUStr:<9} label={labelStr} ]'
+
+                info_stats[0], stats[0] = _summarize(1, areaRng=areaRng, maxDets=maxDets, iStr=iStr)
+                info_stats[1], stats[1] = _summarize(1, iouThr=.5, areaRng=areaRng, maxDets=maxDets, iStr=iStr)
+                info_stats[2], stats[2] = _summarize(1, iouThr=.75, areaRng=areaRng, maxDets=maxDets, iStr=iStr)
+                index = 3
+
+                #for each category
+                for i in cat_indexs:
+                    info_stats[index + 0], stats[index + 0] = _summarize(1, areaRng=areaRng, maxDets=maxDets, cat = i, iStrCat=iStrCat)
+                    info_stats[index + 1], stats[index + 1] = _summarize(1, iouThr=.5, areaRng=areaRng, maxDets=maxDets, cat = i, iStrCat=iStrCat)
+                    info_stats[index + 2], stats[index + 2] = _summarize(1, iouThr=.75, areaRng=areaRng, maxDets=maxDets, cat = i, iStrCat=iStrCat)
+                    index += 3
+
+                return info_stats, stats
+            
+            elif ap == 0 and iouThr is None:
+                stats = np.zeros((1 + num_cat * 1)) # added classes * 1 for AP and AR 
+                info_stats =[x for x in range(1 + num_cat * 1)]
+
+                iStr = ' {:<18} {} @[ IoU={IoUStr:<9} ]'
+                iStrCat = ' {:<18} {} @[ IoU={IoUStr:<9} label={labelStr} ]'
+
+                info_stats[0], stats[0] = _summarize(0, areaRng=areaRng, maxDets=maxDets, iStr=iStr)
+                index = 1
+
+                for i in cat_indexs:
+                    info_stats[index + 0], stats[index + 0] = _summarize(0, areaRng=areaRng, maxDets=maxDets, cat = i, iStrCat=iStrCat)
+                    index += 1
+
+                return info_stats, stats
+            
+            elif ap == 1 and iouThr is not None: # 1 rows
+
+                stats = np.zeros((1 + num_cat * 1)) # added classes * 1 for AP and AR
+                info_stats =[x for x in range(1 + num_cat * 1)]
+              
+                info_stats[0], stats[0] = _summarize(1, iouThr=iouThr, areaRng=areaRng, maxDets=maxDets, iStr=iStr)
+                index = 1
+
+                for i in cat_indexs:
+                    info_stats[index + 0], stats[index + 0] = _summarize(1, iouThr=iouThr, areaRng=areaRng, maxDets=maxDets, cat = i, iStrCat=iStrCat)
+                    index += 1
+
+                return info_stats, stats
+            
+            elif ap == 0 and iouThr is not None:
+
+                stats = np.zeros((1 + num_cat * 1)) # added classes * 1 for AP and AR 
+                info_stats =[x for x in range(1 + num_cat * 1)]
+                
+                info_stats[0], stats[0] = _summarize(0, iouThr=iouThr, areaRng=areaRng, maxDets=maxDets, iStr=iStr)
+                index = 1
+                
+                for i in cat_indexs:
+                    info_stats[index + 0], stats[index + 0] = _summarize(0, iouThr=iouThr, areaRng=areaRng, maxDets=maxDets, cat = i, iStrCat=iStrCat)
+                    index += 1
+
+                return info_stats, stats  
+
+            else:
+
+                stats = np.zeros((2 + num_cat * 2)) # added classes * 2 for AP and AR 
+                info_stats =[x for x in range(2 + num_cat * 2)]
+                
+                info_stats[0], stats[0] = _summarize(1, iouThr=iouThr, areaRng=areaRng, maxDets=maxDets, iStr=iStr)
+                info_stats[1], stats[1] = _summarize(0, iouThr=iouThr, areaRng=areaRng, maxDets=maxDets, iStr=iStr)
+                
+                index = 2
+            
+                for i in cat_indexs:
+                    info_stats[index + 0], stats[index + 0] = _summarize(1, iouThr=iouThr, areaRng=areaRng, maxDets=maxDets, cat = i, iStrCat=iStrCat)
+                    info_stats[index + 1], stats[index + 1] = _summarize(1, iouThr=iouThr, areaRng=areaRng, maxDets=maxDets, cat = i, iStrCat=iStrCat)
+                    index += 2
+
+                return info_stats, stats   
+
         def _summarizeKps():
             stats = np.zeros((10,))
             info_stats = [x for x in range(10)]
 
             info_stats[0], stats[0] = _summarize(1, maxDets=20)
             info_stats[0], stats[1] = _summarize(1, maxDets=20, iouThr=.5)
             info_stats[0], stats[2] = _summarize(1, maxDets=20, iouThr=.75)
@@ -699,19 +815,22 @@
             info_stats[0], stats[9] = _summarize(0, maxDets=20, areaRng='large')
             return info_stats, stats
         
         if not self.eval:
             raise Exception('Please run accumulate() first')
         iouType = self.params.iouType
         if iouType == 'segm' or iouType == 'bbox':
-            if ap is None and iouThr is None:
+            if ap is None and iouThr is None and givenAreaRng is None and givenMaxDets is None:
                 stats_info, summarize = _summarizeDets()
             else:
                 # summarize specifics
-                stats_info, summarize = _summarizeCustom(ap, iouThr, labels)
+                if givenAreaRng is None and givenMaxDets is None:
+                    stats_info, summarize = _summarizeCustomCOCO(ap, iouThr, classes)
+                else:
+                    stats_info, summarize = _summarizeCustom(ap, iouThr, givenAreaRng, givenMaxDets, classes)
 
         elif iouType == 'keypoints':
             stats_info, summarize = _summarizeKps()
 
         self.stats = summarize
         self.stats_info = stats_info
```

### Comparing `cocojamboo-1.0.0/cocojamboo/engine2.py` & `cocojamboo-2.0.0/cocojamboo/engine2.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         iou_types.append("segm")
     if isinstance(model_without_ddp, torchvision.models.detection.KeypointRCNN):
         iou_types.append("keypoints")
     return iou_types
 
 
 @torch.inference_mode()
-def evaluate(model, data_loader, device, ap=None, iouThr=None, labels=None):
+def evaluate(model, data_loader, device, ap=None, iouThr=None, areaRng=None, maxDets=None, classes=None, labels=None):
     n_threads = torch.get_num_threads()
     # FIXME remove this and make paste_masks_in_image run on the GPU
     torch.set_num_threads(1)
     cpu_device = torch.device("cpu")
     model.eval()
     metric_logger = utils.MetricLogger(delimiter="  ")
     header = "Test:"
@@ -106,15 +106,15 @@
     # gather the stats from all processes
     metric_logger.synchronize_between_processes()
     print("Averaged stats:", metric_logger)
     coco_evaluator.synchronize_between_processes()
 
     # accumulate predictions from all images
     coco_evaluator.accumulate()
-    coco_evaluator.summarize(ap, iouThr, labels)
+    coco_evaluator.summarize(ap, iouThr, areaRng, maxDets, classes, labels)
     torch.set_num_threads(n_threads)
 
     return coco_evaluator
 
 def summarize(epoch, train_metrics, eval_result):
     import re
     record = dict()
```

### Comparing `cocojamboo-1.0.0/cocojamboo/transforms.py` & `cocojamboo-2.0.0/cocojamboo/transforms.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-1.0.0/cocojamboo/utils.py` & `cocojamboo-2.0.0/cocojamboo/utils.py`

 * *Files identical despite different names*

### Comparing `cocojamboo-1.0.0/cocojamboo.egg-info/PKG-INFO` & `cocojamboo-2.0.0/cocojamboo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocojamboo
-Version: 1.0.0
+Version: 2.0.0
 Summary: An extension to COCO evaluation metric to provide mAP scores with custom paramters.
 Author: Georgiana Manolache
 License: 
         Attribution-NonCommercial 4.0 International
         
         =======================================================================
```

### Comparing `cocojamboo-1.0.0/pyproject.toml` & `cocojamboo-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
+requires = ["setuptools>=61.0.0", "wheel", "pycocotools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cocojamboo"
-version = "1.0.0"
+version = "2.0.0"
 description = "An extension to COCO evaluation metric to provide mAP scores with custom paramters."
 readme = "README.md"
 authors = [{ name = "Georgiana Manolache" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: Free for non-commercial use",
     "Programming Language :: Python",
```

