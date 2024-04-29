# Comparing `tmp/fplab-0.0.2.7.tar.gz` & `tmp/fplab-0.0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fplab-0.0.2.7.tar", last modified: Sat Apr 27 04:35:58 2024, max compression
+gzip compressed data, was "fplab-0.0.2.8.tar", last modified: Mon Apr 29 15:50:42 2024, max compression
```

## Comparing `fplab-0.0.2.7.tar` & `fplab-0.0.2.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:58.091220 fplab-0.0.2.7/
--rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0      523 2024-04-27 04:35:58.091220 fplab-0.0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      862 2024-04-06 15:56:56.000000 fplab-0.0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:57.963977 fplab-0.0.2.7/fplab/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.7/fplab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:57.996099 fplab-0.0.2.7/fplab/enhancement/
--rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.2.7/fplab/enhancement/__init__.py
--rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.2.7/fplab/enhancement/frequency.py
--rw-rw-rw-   0        0        0     4907 2024-04-26 16:08:32.000000 fplab-0.0.2.7/fplab/enhancement/spatial.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:58.012284 fplab-0.0.2.7/fplab/generation/
--rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.2.7/fplab/generation/__init__.py
--rw-rw-rw-   0        0        0     9814 2024-04-27 04:03:12.000000 fplab-0.0.2.7/fplab/generation/distortion.py
--rw-rw-rw-   0        0        0     3304 2024-04-26 16:52:24.000000 fplab-0.0.2.7/fplab/generation/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:58.012284 fplab-0.0.2.7/fplab/intrinsic/
--rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.2.7/fplab/intrinsic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:58.027871 fplab-0.0.2.7/fplab/intrinsic/frequency/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.7/fplab/intrinsic/frequency/__init__.py
--rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.2.7/fplab/intrinsic/frequency/projection.py
--rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.2.7/fplab/intrinsic/frequency/tools.py
--rw-rw-rw-   0        0        0     3116 2024-04-07 04:59:12.000000 fplab-0.0.2.7/fplab/intrinsic/frequency/transform.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:58.027871 fplab-0.0.2.7/fplab/intrinsic/mask/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.7/fplab/intrinsic/mask/__init__.py
--rw-rw-rw-   0        0        0      855 2024-04-06 15:25:34.000000 fplab-0.0.2.7/fplab/intrinsic/mask/mask.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:58.038619 fplab-0.0.2.7/fplab/intrinsic/multiple/
--rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.2.7/fplab/intrinsic/multiple/__init__.py
--rw-rw-rw-   0        0        0     6990 2024-04-07 05:24:47.000000 fplab-0.0.2.7/fplab/intrinsic/multiple/transform.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:58.050610 fplab-0.0.2.7/fplab/intrinsic/orientation/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.7/fplab/intrinsic/orientation/__init__.py
--rw-rw-rw-   0        0        0     6640 2024-04-06 09:18:53.000000 fplab-0.0.2.7/fplab/intrinsic/orientation/gradient.py
--rw-rw-rw-   0        0        0     6215 2024-04-07 04:39:10.000000 fplab-0.0.2.7/fplab/intrinsic/orientation/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:58.058046 fplab-0.0.2.7/fplab/intrinsic/skeleton/
--rw-rw-rw-   0        0        0        0 2024-04-06 15:22:02.000000 fplab-0.0.2.7/fplab/intrinsic/skeleton/__init__.py
--rw-rw-rw-   0        0        0     1752 2024-04-06 16:14:50.000000 fplab-0.0.2.7/fplab/intrinsic/skeleton/skeleton.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:58.060300 fplab-0.0.2.7/fplab/matching/
--rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.2.7/fplab/matching/__init__.py
--rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.2.7/fplab/matching/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:58.068607 fplab-0.0.2.7/fplab/minutiae/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.7/fplab/minutiae/__init__.py
--rw-rw-rw-   0        0        0     6782 2024-04-14 14:52:02.000000 fplab-0.0.2.7/fplab/minutiae/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:58.091220 fplab-0.0.2.7/fplab/tools/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.7/fplab/tools/__init__.py
--rw-rw-rw-   0        0        0    13732 2024-04-06 14:10:17.000000 fplab-0.0.2.7/fplab/tools/array.py
--rw-rw-rw-   0        0        0     5367 2024-04-06 14:01:28.000000 fplab-0.0.2.7/fplab/tools/image.py
--rw-rw-rw-   0        0        0    15076 2024-04-06 09:13:19.000000 fplab-0.0.2.7/fplab/tools/nbis.py
--rw-rw-rw-   0        0        0    15788 2024-04-06 14:10:17.000000 fplab-0.0.2.7/fplab/tools/tensor.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:35:57.990184 fplab-0.0.2.7/fplab.egg-info/
--rw-rw-rw-   0        0        0      523 2024-04-27 04:35:57.000000 fplab-0.0.2.7/fplab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2024-04-27 04:35:57.000000 fplab-0.0.2.7/fplab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 04:35:57.000000 fplab-0.0.2.7/fplab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-27 04:35:57.000000 fplab-0.0.2.7/fplab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 04:35:58.091220 fplab-0.0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      801 2024-04-27 04:33:53.000000 fplab-0.0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.812484 fplab-0.0.2.8/
+-rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.2.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      523 2024-04-29 15:50:42.812484 fplab-0.0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      862 2024-04-06 15:56:56.000000 fplab-0.0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.699061 fplab-0.0.2.8/fplab/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.8/fplab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.722808 fplab-0.0.2.8/fplab/enhancement/
+-rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.2.8/fplab/enhancement/__init__.py
+-rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.2.8/fplab/enhancement/frequency.py
+-rw-rw-rw-   0        0        0     4907 2024-04-26 16:08:32.000000 fplab-0.0.2.8/fplab/enhancement/spatial.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.738553 fplab-0.0.2.8/fplab/generation/
+-rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.2.8/fplab/generation/__init__.py
+-rw-rw-rw-   0        0        0     9898 2024-04-27 05:54:42.000000 fplab-0.0.2.8/fplab/generation/distortion.py
+-rw-rw-rw-   0        0        0     3304 2024-04-26 16:52:24.000000 fplab-0.0.2.8/fplab/generation/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.740886 fplab-0.0.2.8/fplab/intrinsic/
+-rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.2.8/fplab/intrinsic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.757354 fplab-0.0.2.8/fplab/intrinsic/frequency/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.8/fplab/intrinsic/frequency/__init__.py
+-rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.2.8/fplab/intrinsic/frequency/projection.py
+-rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.2.8/fplab/intrinsic/frequency/tools.py
+-rw-rw-rw-   0        0        0     3116 2024-04-07 04:59:12.000000 fplab-0.0.2.8/fplab/intrinsic/frequency/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.759359 fplab-0.0.2.8/fplab/intrinsic/mask/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.8/fplab/intrinsic/mask/__init__.py
+-rw-rw-rw-   0        0        0      855 2024-04-06 15:25:34.000000 fplab-0.0.2.8/fplab/intrinsic/mask/mask.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.766570 fplab-0.0.2.8/fplab/intrinsic/multiple/
+-rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.2.8/fplab/intrinsic/multiple/__init__.py
+-rw-rw-rw-   0        0        0     6990 2024-04-07 05:24:47.000000 fplab-0.0.2.8/fplab/intrinsic/multiple/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.776343 fplab-0.0.2.8/fplab/intrinsic/orientation/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.8/fplab/intrinsic/orientation/__init__.py
+-rw-rw-rw-   0        0        0     6688 2024-04-29 15:36:06.000000 fplab-0.0.2.8/fplab/intrinsic/orientation/gradient.py
+-rw-rw-rw-   0        0        0     6215 2024-04-07 04:39:10.000000 fplab-0.0.2.8/fplab/intrinsic/orientation/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.779218 fplab-0.0.2.8/fplab/intrinsic/skeleton/
+-rw-rw-rw-   0        0        0        0 2024-04-06 15:22:02.000000 fplab-0.0.2.8/fplab/intrinsic/skeleton/__init__.py
+-rw-rw-rw-   0        0        0     1752 2024-04-06 16:14:50.000000 fplab-0.0.2.8/fplab/intrinsic/skeleton/skeleton.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.786148 fplab-0.0.2.8/fplab/matching/
+-rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.2.8/fplab/matching/__init__.py
+-rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.2.8/fplab/matching/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.792484 fplab-0.0.2.8/fplab/minutiae/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.8/fplab/minutiae/__init__.py
+-rw-rw-rw-   0        0        0     6782 2024-04-14 14:52:02.000000 fplab-0.0.2.8/fplab/minutiae/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.812484 fplab-0.0.2.8/fplab/tools/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.8/fplab/tools/__init__.py
+-rw-rw-rw-   0        0        0    13732 2024-04-06 14:10:17.000000 fplab-0.0.2.8/fplab/tools/array.py
+-rw-rw-rw-   0        0        0     5367 2024-04-06 14:01:28.000000 fplab-0.0.2.8/fplab/tools/image.py
+-rw-rw-rw-   0        0        0    15076 2024-04-06 09:13:19.000000 fplab-0.0.2.8/fplab/tools/nbis.py
+-rw-rw-rw-   0        0        0    15788 2024-04-06 14:10:17.000000 fplab-0.0.2.8/fplab/tools/tensor.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:50:42.713117 fplab-0.0.2.8/fplab.egg-info/
+-rw-rw-rw-   0        0        0      523 2024-04-29 15:50:42.000000 fplab-0.0.2.8/fplab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2024-04-29 15:50:42.000000 fplab-0.0.2.8/fplab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 15:50:42.000000 fplab-0.0.2.8/fplab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-29 15:50:42.000000 fplab-0.0.2.8/fplab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 15:50:42.812484 fplab-0.0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      801 2024-04-29 15:39:22.000000 fplab-0.0.2.8/setup.py
```

### Comparing `fplab-0.0.2.7/LICENSE.txt` & `fplab-0.0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/PKG-INFO` & `fplab-0.0.2.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.2.7
+Version: 0.0.2.8
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.2.7/README.md` & `fplab-0.0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/enhancement/frequency.py` & `fplab-0.0.2.8/fplab/enhancement/frequency.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/enhancement/spatial.py` & `fplab-0.0.2.8/fplab/enhancement/spatial.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/generation/distortion.py` & `fplab-0.0.2.8/fplab/generation/distortion.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,25 +154,27 @@
     if display_point_flag:
         display_point(fix_p, old_p, new_p, sp=(h, w), step=round(old_p_dict["pn"]/20))
     ind_h, ind_w = get_index(fix_p, old_p, new_p, sp=(h, w))
     if display_transform_flag:
         display_transform((h, w), index=[ind_h, ind_w])
     if ima.ndim == 2:
         out = map_coordinates(ima, [ind_h, ind_w], mode=pad_md, cval=pad_v)
+        if display_out_flag:
+            IMA(out).show()
     else:
         # 当im是RGB图像时，对每一个通道作相同的处理
         out = np.zeros_like(ima)
         for i in range(ima.shape[2]):
             pv = pad_v
             if pad_md == 'constant':
                 if isinstance(pad_v, (list, tuple, np.ndarray)):
                     pv = pad_v[i]
             out[:, :, i] = map_coordinates(ima[:, :, i], [ind_h, ind_w], mode=pad_md, cval=pv)
-    if display_out_flag:
-        IMA(out).show()
+            if display_out_flag:
+                IMA(out[:, :, i]).show()
     out = type_as(out, im)
     return out
 
 
 def cappelli2001(im, skin_k=3, affine_p=None, region_p=None, pad_md='constant', pad_v=0.,
                  display_transform_flag=False, display_out_flag=False):
     """使用cappelli2001年提出的模型扭曲指纹
```

### Comparing `fplab-0.0.2.7/fplab/generation/tools.py` & `fplab-0.0.2.8/fplab/generation/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/intrinsic/frequency/projection.py` & `fplab-0.0.2.8/fplab/intrinsic/frequency/projection.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/intrinsic/frequency/tools.py` & `fplab-0.0.2.8/fplab/intrinsic/frequency/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/intrinsic/frequency/transform.py` & `fplab-0.0.2.8/fplab/intrinsic/frequency/transform.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/intrinsic/mask/mask.py` & `fplab-0.0.2.8/fplab/intrinsic/mask/mask.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/intrinsic/multiple/transform.py` & `fplab-0.0.2.8/fplab/intrinsic/multiple/transform.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/intrinsic/orientation/gradient.py` & `fplab-0.0.2.8/fplab/intrinsic/orientation/gradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 import torch
 import gc
 from fplab.tools.image import type_as
 from fplab.tools.tensor import imt_pad_blk, imt_cal_grad, imt_sum_average, imt_gaussian, imt_pad_crop
 
 
-def rao1990(im, blk_sz, wd_sz=(5, 5), device=None):
+def rao1990(im, blk_sz, wd_sz=(5, 5), device=None, need_quality=True):
     """使用1990年Rao使用的方法估计指纹方向场。
     im是需要处理的指纹图像。
     blk_sz是估计方向场时的图像块大小，可以为整数或2维向量。
     wd_sz是计算方向场可信度时的窗口大小，可以为整数或2维向量。
     device是数组转化为张量后使用的设备"""
     # 处理输入参数
     if isinstance(blk_sz, int):
@@ -25,29 +25,30 @@
         wsp = wd_sz
     # 估计方向场
     imt = type_as(im, md="t", device=device)
     hg, wg = imt_cal_grad(imt)
     vy = imt_sum_average(2*hg*wg, ksp, kmd="s")
     vx = imt_sum_average(hg*hg-wg*wg, ksp, kmd="s")
     out = 0.5*torch.atan2(vy, vx)
-    # 计算方向场可信度
-    # 原文中使用了绝对值，为了便于使用卷积实现，这里使用了平方
-    cost, sint = torch.cos(out), torch.sin(out)
-    g = hg**2+wg**2
-    g_cos = imt_sum_average(g*cost*cost, wsp, kmd="s")
-    g_sin = imt_sum_average(g*sint*sint, wsp, kmd="s")
-    g_2cs = imt_sum_average(2*g*sint*cost, wsp, kmd="s")
-    sum_g = imt_sum_average(g, wsp, kmd="s")
-    cd = (cost*cost*g_cos+sint*sint*g_sin+cost*sint*g_2cs)/(sum_g+1e-8)
-    out = type_as(out, im)
-    cd = type_as(cd, im)
-    del ksp, wsp, imt, hg, wg, vy, vx
-    del cost, sint, g, g_cos, g_sin, g_2cs, sum_g
-    gc.collect()
-    return out, cd
+    if not need_quality:
+        out = type_as(out, im)
+        return out
+    else:
+        # 计算方向场可信度
+        # 原文中使用了绝对值，为了便于使用卷积实现，这里使用了平方
+        cost, sint = torch.cos(out), torch.sin(out)
+        g = hg**2+wg**2
+        g_cos = imt_sum_average(g*cost*cost, wsp, kmd="s")
+        g_sin = imt_sum_average(g*sint*sint, wsp, kmd="s")
+        g_2cs = imt_sum_average(2*g*sint*cost, wsp, kmd="s")
+        sum_g = imt_sum_average(g, wsp, kmd="s")
+        cd = (cost*cost*g_cos+sint*sint*g_sin+cost*sint*g_2cs)/(sum_g+1e-8)
+        out = type_as(out, im)
+        cd = type_as(cd, im)
+        return out, cd
 
 
 def hong1998(im, blk_sz=(16, 16), wd_sz=(3, 3), device=None):
     """使用1998年HongLin使用的方法估计指纹方向场。
     首先使用1990年Rao的方法估计指纹方向场，然后使用高斯滤波平滑方向场
     im是需要处理的指纹图像。
     blk_sz是估计方向场时的图像块大小，可以为整数或2维向量。
```

### Comparing `fplab-0.0.2.7/fplab/intrinsic/orientation/tools.py` & `fplab-0.0.2.8/fplab/intrinsic/orientation/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/intrinsic/skeleton/skeleton.py` & `fplab-0.0.2.8/fplab/intrinsic/skeleton/skeleton.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/matching/tools.py` & `fplab-0.0.2.8/fplab/matching/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/minutiae/tools.py` & `fplab-0.0.2.8/fplab/minutiae/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/tools/array.py` & `fplab-0.0.2.8/fplab/tools/array.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/tools/image.py` & `fplab-0.0.2.8/fplab/tools/image.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/tools/nbis.py` & `fplab-0.0.2.8/fplab/tools/nbis.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab/tools/tensor.py` & `fplab-0.0.2.8/fplab/tools/tensor.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/fplab.egg-info/PKG-INFO` & `fplab-0.0.2.8/fplab.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.2.7
+Version: 0.0.2.8
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.2.7/fplab.egg-info/SOURCES.txt` & `fplab-0.0.2.8/fplab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.7/setup.py` & `fplab-0.0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2.7'
+VERSION = '0.0.2.8'
 DESCRIPTION = 'Python3 Package for Fingerprint Processing'
 LONG_DESCRIPTION = ('This is a python3 package for fingerprint processing,'
                     ' which can be used for fingerprint enhancement.')
 
 setup(
     name="fplab",
     version=VERSION,
```

