# Comparing `tmp/ld_msgs-0.2.tar.gz` & `tmp/ld_msgs-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ld_msgs-0.2.tar", last modified: Fri Apr 26 15:45:24 2024, max compression
+gzip compressed data, was "ld_msgs-0.3.tar", last modified: Mon Apr 29 12:33:46 2024, max compression
```

## Comparing `ld_msgs-0.2.tar` & `ld_msgs-0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 15:45:24.830000 ld_msgs-0.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      625 2024-04-26 15:45:24.824000 ld_msgs-0.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       99 2024-04-26 15:45:17.000000 ld_msgs-0.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 15:45:24.080000 ld_msgs-0.2/ld_msgs.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      625 2024-04-26 15:45:23.000000 ld_msgs-0.2/ld_msgs.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2024-04-26 15:45:23.000000 ld_msgs-0.2/ld_msgs.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-26 15:45:23.000000 ld_msgs-0.2/ld_msgs.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       41 2024-04-26 15:45:23.000000 ld_msgs-0.2/ld_msgs.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-04-26 15:45:23.000000 ld_msgs-0.2/ld_msgs.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-26 15:45:24.805000 ld_msgs-0.2/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1071 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22329 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_image_tagging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10493 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_2d_bbox.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14195 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_2d_bbox_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16461 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_2d_instance_segmentation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4835 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_2d_polyline.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9544 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_2d_polyline_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26612 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_2dobject.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29664 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_2dobject_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36941 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_annotation_comment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21483 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_annotation_comment_item.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39518 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_annotation_comment_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7518 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_can.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7514 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_can2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27850 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_data_msg.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16722 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_ego_motion.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24385 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_face.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10533 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_gps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9283 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_image.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15051 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_imu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17608 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_imu_gps.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22494 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_imugps_can.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    49544 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_mesh.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48580 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_mesh_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33434 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_mobileye_lane.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11909 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_mobileye_traffic_sign.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48881 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_object.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    51330 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_object_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4123 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_packet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9033 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_road_feature_facility.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14093 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_road_feature_feature.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7894 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_road_feature_lane.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29628 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_road_feature_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6998 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_rt_matrix.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7047 2024-04-26 12:08:33.000000 ld_msgs-0.2/msg/_ld_sensor_location.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-26 15:45:24.834000 ld_msgs-0.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      809 2024-04-26 15:45:10.000000 ld_msgs-0.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 12:33:46.697000 ld_msgs-0.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      625 2024-04-29 12:33:46.690000 ld_msgs-0.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       99 2024-04-29 12:32:58.000000 ld_msgs-0.3/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 12:33:45.928000 ld_msgs-0.3/ld_msgs.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      625 2024-04-29 12:33:45.000000 ld_msgs-0.3/ld_msgs.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2024-04-29 12:33:45.000000 ld_msgs-0.3/ld_msgs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-29 12:33:45.000000 ld_msgs-0.3/ld_msgs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2024-04-29 12:33:45.000000 ld_msgs-0.3/ld_msgs.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-04-29 12:33:45.000000 ld_msgs-0.3/ld_msgs.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 12:33:46.669000 ld_msgs-0.3/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1071 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22329 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_image_tagging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10493 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_2d_bbox.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14195 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_2d_bbox_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16461 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_2d_instance_segmentation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4835 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_2d_polyline.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9544 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_2d_polyline_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26612 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_2dobject.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29664 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_2dobject_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36941 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_annotation_comment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21483 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_annotation_comment_item.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39518 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_annotation_comment_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7518 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_can.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7514 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_can2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27850 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_data_msg.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16722 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_ego_motion.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24385 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_face.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10533 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_gps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9283 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_image.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15051 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_imu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17608 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_imu_gps.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22494 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_imugps_can.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    49544 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_mesh.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48580 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_mesh_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33434 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_mobileye_lane.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11909 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_mobileye_traffic_sign.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48881 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_object.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    51330 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_object_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4123 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_packet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9033 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_road_feature_facility.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14093 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_road_feature_feature.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7894 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_road_feature_lane.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29628 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_road_feature_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6998 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_rt_matrix.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7047 2024-04-26 12:08:33.000000 ld_msgs-0.3/msg/_ld_sensor_location.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-29 12:33:46.703000 ld_msgs-0.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      815 2024-04-29 12:32:53.000000 ld_msgs-0.3/setup.py
```

### Comparing `ld_msgs-0.2/PKG-INFO` & `ld_msgs-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ld_msgs
-Version: 0.2
+Version: 0.3
 Summary: ld_msg lib for python
 Home-page: 
 Author: shuo shen
 Author-email: shuo.shen@liangdao.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,9 +15,9 @@
 Description-Content-Type: text/markdown
 
 This is for the LD LDE_Online Project generated.
 
 
 Download method:
 ```
-pip install ld-msgs=0.2
+pip install ld-msgs=0.3
 ```
```

### Comparing `ld_msgs-0.2/ld_msgs.egg-info/PKG-INFO` & `ld_msgs-0.3/ld_msgs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ld-msgs
-Version: 0.2
+Version: 0.3
 Summary: ld_msg lib for python
 Home-page: 
 Author: shuo shen
 Author-email: shuo.shen@liangdao.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,9 +15,9 @@
 Description-Content-Type: text/markdown
 
 This is for the LD LDE_Online Project generated.
 
 
 Download method:
 ```
-pip install ld-msgs=0.2
+pip install ld-msgs=0.3
 ```
```

### Comparing `ld_msgs-0.2/ld_msgs.egg-info/SOURCES.txt` & `ld_msgs-0.3/ld_msgs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/__init__.py` & `ld_msgs-0.3/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_image_tagging.py` & `ld_msgs-0.3/msg/_image_tagging.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_2d_bbox.py` & `ld_msgs-0.3/msg/_ld_2d_bbox.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_2d_bbox_list.py` & `ld_msgs-0.3/msg/_ld_2d_bbox_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_2d_instance_segmentation.py` & `ld_msgs-0.3/msg/_ld_2d_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_2d_polyline.py` & `ld_msgs-0.3/msg/_ld_2d_polyline.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_2d_polyline_list.py` & `ld_msgs-0.3/msg/_ld_2d_polyline_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_2dobject.py` & `ld_msgs-0.3/msg/_ld_2dobject.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_2dobject_list.py` & `ld_msgs-0.3/msg/_ld_2dobject_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_annotation_comment.py` & `ld_msgs-0.3/msg/_ld_annotation_comment.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_annotation_comment_item.py` & `ld_msgs-0.3/msg/_ld_annotation_comment_item.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_annotation_comment_list.py` & `ld_msgs-0.3/msg/_ld_annotation_comment_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_can.py` & `ld_msgs-0.3/msg/_ld_can.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_can2.py` & `ld_msgs-0.3/msg/_ld_can2.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_data_msg.py` & `ld_msgs-0.3/msg/_ld_data_msg.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_ego_motion.py` & `ld_msgs-0.3/msg/_ld_ego_motion.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_face.py` & `ld_msgs-0.3/msg/_ld_face.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_gps.py` & `ld_msgs-0.3/msg/_ld_gps.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_image.py` & `ld_msgs-0.3/msg/_ld_image.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_imu.py` & `ld_msgs-0.3/msg/_ld_imu.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_imu_gps.py` & `ld_msgs-0.3/msg/_ld_imu_gps.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_imugps_can.py` & `ld_msgs-0.3/msg/_ld_imugps_can.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_mesh.py` & `ld_msgs-0.3/msg/_ld_mesh.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_mesh_list.py` & `ld_msgs-0.3/msg/_ld_mesh_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_mobileye_lane.py` & `ld_msgs-0.3/msg/_ld_mobileye_lane.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_mobileye_traffic_sign.py` & `ld_msgs-0.3/msg/_ld_mobileye_traffic_sign.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_object.py` & `ld_msgs-0.3/msg/_ld_object.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_object_list.py` & `ld_msgs-0.3/msg/_ld_object_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_packet.py` & `ld_msgs-0.3/msg/_ld_packet.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_road_feature_facility.py` & `ld_msgs-0.3/msg/_ld_road_feature_facility.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_road_feature_feature.py` & `ld_msgs-0.3/msg/_ld_road_feature_feature.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_road_feature_lane.py` & `ld_msgs-0.3/msg/_ld_road_feature_lane.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_road_feature_list.py` & `ld_msgs-0.3/msg/_ld_road_feature_list.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_rt_matrix.py` & `ld_msgs-0.3/msg/_ld_rt_matrix.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/msg/_ld_sensor_location.py` & `ld_msgs-0.3/msg/_ld_sensor_location.py`

 * *Files identical despite different names*

### Comparing `ld_msgs-0.2/setup.py` & `ld_msgs-0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ld_msgs',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     description='ld_msg lib for python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='shuo shen',
     author_email='shuo.shen@liangdao.de',
     url='',
     install_requires=[
-        'geometry_msgs',
-        'std_msgs',
-        'sensor_msgs',
+        # 'geometry_msgs',
+        # 'std_msgs',
+        # 'sensor_msgs',
         'genpy'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

