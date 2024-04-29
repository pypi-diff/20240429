# Comparing `tmp/detectools-0.1.2.tar.gz` & `tmp/detectools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detectools-0.1.2.tar", last modified: Tue Apr 23 09:25:00 2024, max compression
+gzip compressed data, was "detectools-0.1.3.tar", last modified: Mon Apr 29 10:29:39 2024, max compression
```

## Comparing `detectools-0.1.2.tar` & `detectools-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.256460 detectools-0.1.2/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1087 2024-03-21 13:04:40.000000 detectools-0.1.2/LICENSE.txt
--rw-r--r--   0 lucas     (1002) lucas     (1002)     3107 2024-04-23 09:25:00.256460 detectools-0.1.2/PKG-INFO
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1637 2024-03-21 11:28:28.000000 detectools-0.1.2/README.md
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      599 2024-04-17 13:45:59.000000 detectools-0.1.2/README_deployment.md
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1442 2024-04-23 09:24:44.000000 detectools-0.1.2/pyproject.toml
--rw-rw-r--   0 lucas     (1002) lucas     (1002)       38 2024-04-23 09:25:00.256460 detectools-0.1.2/setup.cfg
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      145 2024-03-21 13:29:41.000000 detectools-0.1.2/setup.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.252460 detectools-0.1.2/src/
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.252460 detectools-0.1.2/src/detectools/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     2051 2024-04-23 09:14:32.000000 detectools-0.1.2/src/detectools/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     2417 2024-04-17 12:26:22.000000 detectools-0.1.2/src/detectools/augmentation.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    10779 2024-04-18 14:52:14.000000 detectools-0.1.2/src/detectools/dataset.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.256460 detectools-0.1.2/src/detectools/formats/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     3989 2024-03-21 11:28:28.000000 detectools-0.1.2/src/detectools/formats/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    13184 2024-04-19 11:34:07.000000 detectools-0.1.2/src/detectools/formats/base.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     7175 2024-04-23 07:27:53.000000 detectools-0.1.2/src/detectools/formats/detection_format.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     7057 2024-04-23 08:35:56.000000 detectools-0.1.2/src/detectools/formats/mask.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     9748 2024-04-23 07:27:33.000000 detectools-0.1.2/src/detectools/formats/segmentation_format.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     6555 2024-04-22 14:49:17.000000 detectools-0.1.2/src/detectools/inference.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     2209 2024-04-15 10:47:30.000000 detectools-0.1.2/src/detectools/metrics.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.256460 detectools-0.1.2/src/detectools/models/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      330 2024-04-15 10:47:30.000000 detectools-0.1.2/src/detectools/models/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     2641 2024-04-15 10:47:30.000000 detectools-0.1.2/src/detectools/models/base.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    11002 2024-04-17 09:16:04.000000 detectools-0.1.2/src/detectools/models/mask2former.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    10950 2024-04-15 10:47:30.000000 detectools-0.1.2/src/detectools/models/yolo.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    16594 2024-04-16 14:42:36.000000 detectools-0.1.2/src/detectools/models/yolov8_seg.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     8112 2024-04-16 07:53:15.000000 detectools-0.1.2/src/detectools/trainer.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.256460 detectools-0.1.2/src/detectools/utils/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)        0 2024-03-21 13:12:26.000000 detectools-0.1.2/src/detectools/utils/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     3401 2024-04-16 11:03:27.000000 detectools-0.1.2/src/detectools/utils/data_management.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     6207 2024-04-15 10:47:30.000000 detectools-0.1.2/src/detectools/utils/inference.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     2775 2024-04-15 10:47:30.000000 detectools-0.1.2/src/detectools/utils/mask_utils.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    15905 2024-04-16 11:21:48.000000 detectools-0.1.2/src/detectools/utils/metrics.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1202 2024-03-21 11:28:28.000000 detectools-0.1.2/src/detectools/utils/trainer.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     4708 2024-04-23 09:04:07.000000 detectools-0.1.2/src/detectools/utils/visualisation.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-23 09:25:00.256460 detectools-0.1.2/src/detectools.egg-info/
--rw-r--r--   0 lucas     (1002) lucas     (1002)     3107 2024-04-23 09:25:00.000000 detectools-0.1.2/src/detectools.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1016 2024-04-23 09:25:00.000000 detectools-0.1.2/src/detectools.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1002) lucas     (1002)        1 2024-04-23 09:25:00.000000 detectools-0.1.2/src/detectools.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      218 2024-04-23 09:25:00.000000 detectools-0.1.2/src/detectools.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1002) lucas     (1002)       11 2024-04-23 09:25:00.000000 detectools-0.1.2/src/detectools.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 10:29:39.445853 detectools-0.1.3/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1087 2024-03-21 13:04:40.000000 detectools-0.1.3/LICENSE.txt
+-rw-r--r--   0 lucas     (1002) lucas     (1002)     3107 2024-04-29 10:29:39.445853 detectools-0.1.3/PKG-INFO
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1637 2024-03-21 11:28:28.000000 detectools-0.1.3/README.md
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      599 2024-04-17 13:45:59.000000 detectools-0.1.3/README_deployment.md
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1442 2024-04-23 09:24:44.000000 detectools-0.1.3/pyproject.toml
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)       38 2024-04-29 10:29:39.445853 detectools-0.1.3/setup.cfg
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      145 2024-03-21 13:29:41.000000 detectools-0.1.3/setup.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 10:29:39.441853 detectools-0.1.3/src/
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 10:29:39.441853 detectools-0.1.3/src/detectools/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     2051 2024-04-29 10:28:02.000000 detectools-0.1.3/src/detectools/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     2417 2024-04-17 12:26:22.000000 detectools-0.1.3/src/detectools/augmentation.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    10779 2024-04-18 14:52:14.000000 detectools-0.1.3/src/detectools/dataset.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 10:29:39.441853 detectools-0.1.3/src/detectools/formats/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     3989 2024-03-21 11:28:28.000000 detectools-0.1.3/src/detectools/formats/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    13188 2024-04-29 08:39:42.000000 detectools-0.1.3/src/detectools/formats/base.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     7175 2024-04-23 07:27:53.000000 detectools-0.1.3/src/detectools/formats/detection_format.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     7057 2024-04-23 08:35:56.000000 detectools-0.1.3/src/detectools/formats/mask.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     9748 2024-04-23 07:27:33.000000 detectools-0.1.3/src/detectools/formats/segmentation_format.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     6555 2024-04-22 14:49:17.000000 detectools-0.1.3/src/detectools/inference.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     2209 2024-04-15 10:47:30.000000 detectools-0.1.3/src/detectools/metrics.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 10:29:39.445853 detectools-0.1.3/src/detectools/models/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      330 2024-04-15 10:47:30.000000 detectools-0.1.3/src/detectools/models/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     2641 2024-04-15 10:47:30.000000 detectools-0.1.3/src/detectools/models/base.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    11002 2024-04-17 09:16:04.000000 detectools-0.1.3/src/detectools/models/mask2former.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    10950 2024-04-15 10:47:30.000000 detectools-0.1.3/src/detectools/models/yolo.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    16594 2024-04-16 14:42:36.000000 detectools-0.1.3/src/detectools/models/yolov8_seg.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     8112 2024-04-16 07:53:15.000000 detectools-0.1.3/src/detectools/trainer.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 10:29:39.445853 detectools-0.1.3/src/detectools/utils/
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)        0 2024-03-21 13:12:26.000000 detectools-0.1.3/src/detectools/utils/__init__.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     3401 2024-04-16 11:03:27.000000 detectools-0.1.3/src/detectools/utils/data_management.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     6207 2024-04-15 10:47:30.000000 detectools-0.1.3/src/detectools/utils/inference.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     2775 2024-04-15 10:47:30.000000 detectools-0.1.3/src/detectools/utils/mask_utils.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)    16256 2024-04-29 09:04:27.000000 detectools-0.1.3/src/detectools/utils/metrics.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1202 2024-03-21 11:28:28.000000 detectools-0.1.3/src/detectools/utils/trainer.py
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     4708 2024-04-29 09:26:52.000000 detectools-0.1.3/src/detectools/utils/visualisation.py
+drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-04-29 10:29:39.445853 detectools-0.1.3/src/detectools.egg-info/
+-rw-r--r--   0 lucas     (1002) lucas     (1002)     3107 2024-04-29 10:29:39.000000 detectools-0.1.3/src/detectools.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)     1016 2024-04-29 10:29:39.000000 detectools-0.1.3/src/detectools.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)        1 2024-04-29 10:29:39.000000 detectools-0.1.3/src/detectools.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)      218 2024-04-29 10:29:39.000000 detectools-0.1.3/src/detectools.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1002) lucas     (1002)       11 2024-04-29 10:29:39.000000 detectools-0.1.3/src/detectools.egg-info/top_level.txt
```

### Comparing `detectools-0.1.2/LICENSE.txt` & `detectools-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/PKG-INFO` & `detectools-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detectools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Overlay of PyTorch to generalize trainning and inference processes for detection & instance segmentation tasks.
 Author-email: Lucas Bernigaud Samatan <lucas.bernigaud-samatan@inrae.fr>, Jordan Bernigaud Samatan <jordan.bernigaud-samatan@inrae.fr>
 Maintainer-email: Jordan Bernigaud Samatan <jordan.bernigaud-samatan@inrae.fr>
 License: The MIT License (MIT)
         
         Copyright (c) <year> <copyright holders>
```

### Comparing `detectools-0.1.2/README.md` & `detectools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/README_deployment.md` & `detectools-0.1.3/README_deployment.md`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/pyproject.toml` & `detectools-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/__init__.py` & `detectools-0.1.3/src/detectools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Torch prebuild functions to train, evaluate and use models in production."""
 import json
 import os
 import sys
 from pathlib import Path
 from typing import Any, Dict, Literal, Union
 
-__version__ = "0.1.2" # change detectools version here
+__version__ = "0.1.3" # change detectools version here
 
 IMAGE_FOLDER = "images"
 ANNOTATION_FILE = "coco_annotations.json"
 
 COLORS = [
     (0, 102, 204),
     (51, 255, 51),
```

### Comparing `detectools-0.1.2/src/detectools/augmentation.py` & `detectools-0.1.3/src/detectools/augmentation.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/dataset.py` & `detectools-0.1.3/src/detectools/dataset.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/formats/__init__.py` & `detectools-0.1.3/src/detectools/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/formats/base.py` & `detectools-0.1.3/src/detectools/formats/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
             "XYWH",
             "XYXY",
             "CXCYWH",
         ], f"box_format should be one of these [XYWH, XYXY, CXCYWH], got {box_format}."
         converter = ConvertBoundingBoxFormat(box_format)
         boxes = self.get("boxes")
         self.data["boxes"] = converter(boxes)
-        self.format = box_format
+        self.box_format = box_format
 
     def convert_labels(self, convert_labels_dict: Dict[int, int]):
         """Convert labels of Format.
 
         Args:
             convert_dict (Dict[int,int]): Conversion dict for labels.
         """
```

### Comparing `detectools-0.1.2/src/detectools/formats/detection_format.py` & `detectools-0.1.3/src/detectools/formats/detection_format.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/formats/mask.py` & `detectools-0.1.3/src/detectools/formats/mask.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/formats/segmentation_format.py` & `detectools-0.1.3/src/detectools/formats/segmentation_format.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/inference.py` & `detectools-0.1.3/src/detectools/inference.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/metrics.py` & `detectools-0.1.3/src/detectools/metrics.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/models/base.py` & `detectools-0.1.3/src/detectools/models/base.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/models/mask2former.py` & `detectools-0.1.3/src/detectools/models/mask2former.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/models/yolo.py` & `detectools-0.1.3/src/detectools/models/yolo.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/models/yolov8_seg.py` & `detectools-0.1.3/src/detectools/models/yolov8_seg.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/trainer.py` & `detectools-0.1.3/src/detectools/trainer.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/utils/data_management.py` & `detectools-0.1.3/src/detectools/utils/data_management.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/utils/inference.py` & `detectools-0.1.3/src/detectools/utils/inference.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/utils/mask_utils.py` & `detectools-0.1.3/src/detectools/utils/mask_utils.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/utils/metrics.py` & `detectools-0.1.3/src/detectools/utils/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         iou_threshold (float, optional): IoU threshold to discard some matchs with overlapping < to thr. Defaults to 0.5.
 
     Returns:
         Tuple[Tensor, Tensor, Tensor, Tuple[Tensor, Tensor]]: Detection statsitics (TP, FN, FN)
         & prediction and target boxes indexes that match well.
     """
     # set box format to XYXY for torch box iou computation
+    assert prediction.box_format == target.box_format, f"Predictio and taget should have the same box_format, got {prediction.box_format} & {target.box_format}"
+    origin_box_format = prediction.box_format
     prediction.set_boxes_format("XYXY")
     target.set_boxes_format("XYXY")
     # extract boxes
     pred_boxes = prediction.get("boxes")
     target_boxes = target.get("boxes")
     # compute cross matrix of ious
     cross_ious = box_iou(pred_boxes, target_boxes)
@@ -48,14 +50,17 @@
     pred_idxs, target_idxs = torch.where(
         (max_matchs > 0) & (cross_ious > iou_threshold)
     )
     # extract indexes
     pred_idxs = pred_idxs.tolist() if pred_idxs.nelement() > 0 else []
     target_idxs = target_idxs.tolist() if target_idxs.nelement() > 0 else []
     match_idxs = (torch.tensor(pred_idxs).long(), torch.tensor(target_idxs).long())
+    # send back box format to original format
+    prediction.set_boxes_format(origin_box_format)
+    target.set_boxes_format(origin_box_format)
 
     return tp, fp, fn, match_idxs
 
 
 # functionnals metrics
 def f1score(tp, fp, tn, fn):
     return (2 * tp) / (2 * tp + fp + fn)
```

### Comparing `detectools-0.1.2/src/detectools/utils/trainer.py` & `detectools-0.1.3/src/detectools/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools/utils/visualisation.py` & `detectools-0.1.3/src/detectools/utils/visualisation.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.2/src/detectools.egg-info/PKG-INFO` & `detectools-0.1.3/src/detectools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detectools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Overlay of PyTorch to generalize trainning and inference processes for detection & instance segmentation tasks.
 Author-email: Lucas Bernigaud Samatan <lucas.bernigaud-samatan@inrae.fr>, Jordan Bernigaud Samatan <jordan.bernigaud-samatan@inrae.fr>
 Maintainer-email: Jordan Bernigaud Samatan <jordan.bernigaud-samatan@inrae.fr>
 License: The MIT License (MIT)
         
         Copyright (c) <year> <copyright holders>
```

### Comparing `detectools-0.1.2/src/detectools.egg-info/SOURCES.txt` & `detectools-0.1.3/src/detectools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

