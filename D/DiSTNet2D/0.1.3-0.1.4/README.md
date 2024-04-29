# Comparing `tmp/DiSTNet2D-0.1.3.tar.gz` & `tmp/distnet2d-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DiSTNet2D-0.1.3.tar", last modified: Fri Apr 12 16:02:09 2024, max compression
+gzip compressed data, was "distnet2d-0.1.4.tar", last modified: Mon Apr 29 15:52:10 2024, max compression
```

## Comparing `DiSTNet2D-0.1.3.tar` & `distnet2d-0.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:02:09.776208 DiSTNet2D-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:02:09.776208 DiSTNet2D-0.1.3/DiSTNet2D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-12 16:02:09.000000 DiSTNet2D-0.1.3/DiSTNet2D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-12 16:02:09.000000 DiSTNet2D-0.1.3/DiSTNet2D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:02:09.000000 DiSTNet2D-0.1.3/DiSTNet2D.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 16:02:09.000000 DiSTNet2D-0.1.3/DiSTNet2D.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 16:02:09.000000 DiSTNet2D-0.1.3/DiSTNet2D.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-12 16:02:09.776208 DiSTNet2D-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:02:09.772208 DiSTNet2D-0.1.3/distnet_2d/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:02:09.772208 DiSTNet2D-0.1.3/distnet_2d/data/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34930 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/data/dydx_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/data/medoid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/data/swim1d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:02:09.772208 DiSTNet2D-0.1.3/distnet_2d/model/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/model/architectures.py
--rw-r--r--   0 runner    (1001) docker     (127)    37619 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/model/distnet_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/model/distnet_2d_seg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/model/gradient_accumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    25269 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/model/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/model/spatial_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:02:09.776208 DiSTNet2D-0.1.3/distnet_2d/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/utils/agc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/utils/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/utils/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/distnet_2d/utils/objectwise_computation_tf.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:02:09.776208 DiSTNet2D-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-12 16:02:06.000000 DiSTNet2D-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:52:10.694016 distnet2d-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:52:10.694016 distnet2d-0.1.4/DiSTNet2D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-29 15:52:10.000000 distnet2d-0.1.4/DiSTNet2D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-29 15:52:10.000000 distnet2d-0.1.4/DiSTNet2D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:52:10.000000 distnet2d-0.1.4/DiSTNet2D.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 15:52:10.000000 distnet2d-0.1.4/DiSTNet2D.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 15:52:10.000000 distnet2d-0.1.4/DiSTNet2D.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 15:52:06.000000 distnet2d-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-29 15:52:10.694016 distnet2d-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-29 15:52:06.000000 distnet2d-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:52:10.690016 distnet2d-0.1.4/distnet_2d/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:52:10.690016 distnet2d-0.1.4/distnet_2d/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34930 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/data/dydx_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/data/medoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/data/swim1d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:52:10.690016 distnet2d-0.1.4/distnet_2d/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37691 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/distnet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/distnet_2d_seg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/gradient_accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25438 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/spatial_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:52:10.694016 distnet2d-0.1.4/distnet_2d/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/agc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/objectwise_computation_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:52:10.694016 distnet2d-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-29 15:52:06.000000 distnet2d-0.1.4/setup.py
```

### Comparing `DiSTNet2D-0.1.3/DiSTNet2D.egg-info/PKG-INFO` & `distnet2d-0.1.4/DiSTNet2D.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DiSTNet2D
-Version: 0.1.3
+Version: 0.1.4
 Summary: tensorflow/keras implementation of DiSTNet 2D
 Home-page: https://github.com/jeanollion/distnet2d
-Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.3/distnet2d-0.1.3.tar.gz
+Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.4/distnet2d-0.1.4.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Segmentation,Tracking,Cell,Tensorflow,Keras
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
@@ -18,15 +18,15 @@
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: tensorflow>=2.7.1
 Requires-Dist: edt>=2.0.2
 Requires-Dist: scikit-fmm
 Requires-Dist: numba
-Requires-Dist: dataset_iterator>=0.4.0
+Requires-Dist: dataset_iterator>=0.4.2
 Requires-Dist: elasticdeform>=0.4.7
 
 # DistNet2D: Leveraging long-range temporal information for efficient segmentation and tracking
 
 This repository contains python code for training the neural network.
 
 [Link to preprint](https://arxiv.org/abs/2310.19641)
```

### Comparing `DiSTNet2D-0.1.3/DiSTNet2D.egg-info/SOURCES.txt` & `distnet2d-0.1.4/DiSTNet2D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DiSTNet2D-0.1.3/LICENSE.txt` & `distnet2d-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DiSTNet2D-0.1.3/PKG-INFO` & `distnet2d-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DiSTNet2D
-Version: 0.1.3
+Version: 0.1.4
 Summary: tensorflow/keras implementation of DiSTNet 2D
 Home-page: https://github.com/jeanollion/distnet2d
-Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.3/distnet2d-0.1.3.tar.gz
+Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.4/distnet2d-0.1.4.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Segmentation,Tracking,Cell,Tensorflow,Keras
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
@@ -18,15 +18,15 @@
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: tensorflow>=2.7.1
 Requires-Dist: edt>=2.0.2
 Requires-Dist: scikit-fmm
 Requires-Dist: numba
-Requires-Dist: dataset_iterator>=0.4.0
+Requires-Dist: dataset_iterator>=0.4.2
 Requires-Dist: elasticdeform>=0.4.7
 
 # DistNet2D: Leveraging long-range temporal information for efficient segmentation and tracking
 
 This repository contains python code for training the neural network.
 
 [Link to preprint](https://arxiv.org/abs/2310.19641)
```

### Comparing `DiSTNet2D-0.1.3/README.md` & `distnet2d-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `DiSTNet2D-0.1.3/distnet_2d/data/dydx_iterator.py` & `distnet2d-0.1.4/distnet_2d/data/dydx_iterator.py`

 * *Files identical despite different names*

### Comparing `DiSTNet2D-0.1.3/distnet_2d/data/swim1d.py` & `distnet2d-0.1.4/distnet_2d/data/swim1d.py`

 * *Files identical despite different names*

### Comparing `DiSTNet2D-0.1.3/distnet_2d/model/distnet_2d.py` & `distnet2d-0.1.4/distnet_2d/model/distnet_2d.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import tensorflow as tf
-from .layers import Combine, ResConv2D, Conv2DBNDrop, Conv2DTransposeBNDrop, WSConv2D, BatchToChannel, SplitBatch, ChannelToBatch, NConvToBatch2D, SelectFeature
+from .layers import ker_size_to_string, Combine, ResConv2D, Conv2DBNDrop, Conv2DTransposeBNDrop, WSConv2D, BatchToChannel, SplitBatch, ChannelToBatch, NConvToBatch2D, SelectFeature
 import numpy as np
 from .spatial_attention import SpatialAttention2D
 from ..utils.helpers import ensure_multiplicity, flatten_list
 from ..utils.losses import weighted_loss_by_category, balanced_category_loss, PseudoHuber
 from ..utils.agc import adaptive_clip_grad
 from .gradient_accumulator import GradientAccumulator
 import time
@@ -475,22 +475,22 @@
             combine = Combine(name = name, filters=filters, kernel_size = combine_kernel_size, l2_reg=l2_reg, weight_scaled=skip_combine_mode.lower()=="wsconv")
         else:
             combine = None
         op = op.lower().replace("_", "")
         if op == "res1d" or op=="resconv1d":
             raise NotImplementedError("ResConv1D are not implemented")
         elif op == "res2d" or op=="resconv2d":
-            convs = [ResConv2D(kernel_size=conv_kernel_size, activation=activation_out if i==n_conv-1 else activation, weight_scaled=weight_scaled, batch_norm=batch_norm, dropout_rate=dropout_rate, l2_reg=l2_reg, weighted_sum=weighted_sum, name=f"{name}/ResConv2D_{i}_{conv_kernel_size}x{conv_kernel_size}") for i in range(n_conv)]
+            convs = [ResConv2D(kernel_size=conv_kernel_size, activation=activation_out if i==n_conv-1 else activation, weight_scaled=weight_scaled, batch_norm=batch_norm, dropout_rate=dropout_rate, l2_reg=l2_reg, weighted_sum=weighted_sum, name=f"{name}/ResConv2D_{i}_{ker_size_to_string(conv_kernel_size)}") for i in range(n_conv)]
         else:
             if weight_scaled:
-                convs = [WSConv2D(filters=filters_out if i==n_conv-1 else filters, kernel_size=conv_kernel_size, padding='same', activation=activation_out if i==n_conv-1 else activation, dropout_rate=dropout_rate, name=f"{name}/Conv_{i}_{conv_kernel_size}x{conv_kernel_size}") for i in range(n_conv)]
+                convs = [WSConv2D(filters=filters_out if i==n_conv-1 else filters, kernel_size=conv_kernel_size, padding='same', activation=activation_out if i==n_conv-1 else activation, dropout_rate=dropout_rate, name=f"{name}/Conv_{i}_{ker_size_to_string(conv_kernel_size)}") for i in range(n_conv)]
             elif batch_norm or dropout_rate>0:
-                convs = [Conv2DBNDrop(filters=filters_out if i==n_conv-1 else filters, kernel_size=conv_kernel_size, activation=activation_out if i==n_conv-1 else activation, batch_norm=batch_norm, dropout_rate=dropout_rate, l2_reg=l2_reg, name=f"{name}/Conv_{i}_{conv_kernel_size}x{conv_kernel_size}") for i in range(n_conv)]
+                convs = [Conv2DBNDrop(filters=filters_out if i==n_conv-1 else filters, kernel_size=conv_kernel_size, activation=activation_out if i==n_conv-1 else activation, batch_norm=batch_norm, dropout_rate=dropout_rate, l2_reg=l2_reg, name=f"{name}/Conv_{i}_{ker_size_to_string(conv_kernel_size)}") for i in range(n_conv)]
             else:
-                convs = [tf.keras.layers.Conv2D(filters=filters_out if i==n_conv-1 else filters, kernel_size=conv_kernel_size, padding='same', activation=activation_out if i==n_conv-1 else activation, kernel_regularizer=tf.keras.regularizers.l2(l2_reg) if l2_reg>0 else None, name=f"{name}/Conv_{i}_{conv_kernel_size}x{conv_kernel_size}") for i in range(n_conv)]
+                convs = [tf.keras.layers.Conv2D(filters=filters_out if i==n_conv-1 else filters, kernel_size=conv_kernel_size, padding='same', activation=activation_out if i==n_conv-1 else activation, kernel_regularizer=tf.keras.regularizers.l2(l2_reg) if l2_reg>0 else None, name=f"{name}/Conv_{i}_{ker_size_to_string(conv_kernel_size)}") for i in range(n_conv)]
         f = tf.cast(factor, tf.float32)
         def op(input):
             down, res = input
             up = up_op(down)
             if res is not None:
                 if combine is not None:
                     up = combine([up, res])
@@ -523,26 +523,26 @@
             kernel_size = size_factor
         if parent_name is not None and len(parent_name)>0:
             name = f"{parent_name}/{name}"
         if mode=="tconv":
             if weight_scaled:
                 raise NotImplementedError("Weight scaled transpose conv is not implemented")
             elif batch_norm or dropout_rate>0:
-                upsample = Conv2DTransposeBNDrop(filters=filters, kernel_size=kernel_size, strides=size_factor, activation=activation, batch_norm=batch_norm, dropout_rate=dropout_rate, l2_reg=l2_reg, name=f"{name}/tConv{kernel_size}x{kernel_size}")
+                upsample = Conv2DTransposeBNDrop(filters=filters, kernel_size=kernel_size, strides=size_factor, activation=activation, batch_norm=batch_norm, dropout_rate=dropout_rate, l2_reg=l2_reg, name=f"{name}/tConv{ker_size_to_string(kernel_size)}")
             else:
                 kernel_regularizer=tf.keras.regularizers.l2(l2_reg) if l2_reg>0 else None
-                upsample = tf.keras.layers.Conv2DTranspose(filters, kernel_size=kernel_size, strides=size_factor, padding='same', activation=activation, use_bias=use_bias, kernel_regularizer=kernel_regularizer, name=f"{name}/tConv{kernel_size}x{kernel_size}")
+                upsample = tf.keras.layers.Conv2DTranspose(filters, kernel_size=kernel_size, strides=size_factor, padding='same', activation=activation, use_bias=use_bias, kernel_regularizer=kernel_regularizer, name=f"{name}/tConv{ker_size_to_string(kernel_size)}")
             conv=None
         else:
             interpolation = "nearest" if mode=="up_nn" else 'bilinear'
             upsample = tf.keras.layers.UpSampling2D(size=size_factor, interpolation=interpolation, name = f"{name}/Upsample{size_factor}x{size_factor}_{interpolation}")
             if batch_norm:
-                conv = Conv2DBNDrop(filters=filters, kernel_size=kernel_size, strides=1, batch_norm=batch_norm, dropout_rate=dropout_rate, l2_reg=l2_reg, name=f"{name}/Conv{kernel_size}x{kernel_size}", activation=activation )
+                conv = Conv2DBNDrop(filters=filters, kernel_size=kernel_size, strides=1, batch_norm=batch_norm, dropout_rate=dropout_rate, l2_reg=l2_reg, name=f"{name}/Conv{ker_size_to_string(kernel_size)}", activation=activation )
             else:
-                conv = tf.keras.layers.Conv2D(filters=filters, kernel_size=kernel_size, strides=1, padding='same', name=f"{name}/Conv{kernel_size}x{kernel_size}", use_bias=use_bias, activation=activation, kernel_regularizer=tf.keras.regularizers.l2(l2_reg) if l2_reg>0 else None )
+                conv = tf.keras.layers.Conv2D(filters=filters, kernel_size=kernel_size, strides=1, padding='same', name=f"{name}/Conv{ker_size_to_string(kernel_size)}", use_bias=use_bias, activation=activation, kernel_regularizer=tf.keras.regularizers.l2(l2_reg) if l2_reg>0 else None )
         def op(input):
             x = upsample(input)
             if conv is not None:
                 x = conv(x)
             return x
         return op
 
@@ -599,23 +599,23 @@
     return sequence, down, total_contraction, residual_filters, out_filters
 
 def parse_params(filters:int = 0, kernel_size:int = 3, op:str = "conv", dilation:int=1, activation="relu", downscale:int=1, dropout_rate:float=0, weight_scaled:bool=False, batch_norm:bool=False, weighted_sum:bool=False, l2_reg:float=0, split_conv:bool = False, num_attention_heads:int=1, name:str=""):
     op = op.lower().replace("_", "")
     if op =="res1d" or op=="resconv1d":
         raise NotImplementedError("ResConv1D is not implmeneted")
     elif op =="res2d" or op == "resconv2d":
-        return ResConv2D(kernel_size=kernel_size, dilation=dilation, activation=activation, dropout_rate=dropout_rate, weight_scaled=weight_scaled, batch_norm=batch_norm, weighted_sum=weighted_sum, l2_reg=l2_reg, split_conv=split_conv, name=f"{name}/ResConv2D{kernel_size}x{kernel_size}")
+        return ResConv2D(kernel_size=kernel_size, dilation=dilation, activation=activation, dropout_rate=dropout_rate, weight_scaled=weight_scaled, batch_norm=batch_norm, weighted_sum=weighted_sum, l2_reg=l2_reg, split_conv=split_conv, name=f"{name}/ResConv2D{ker_size_to_string(kernel_size)}")
     assert filters > 0 , "filters must be > 0"
     if op=="selfattention" or op=="sa":
         self_attention_op = SpatialAttention2D(num_heads=num_attention_heads, positional_encoding="2D", dropout=dropout_rate, l2_reg=l2_reg, name=f"{name}/SelfAttention")
         self_attention_skip_op = Combine(filters=filters, l2_reg=l2_reg, name=f"{name}/SelfAttentionSkip")
         def op(x):
             sa = self_attention_op([x, x])
             return self_attention_skip_op([x, sa])
         return op
     if weight_scaled: # no l2_reg
-        return WSConv2D(filters=filters, kernel_size=kernel_size, strides = downscale, dilation_rate = dilation, activation=activation, dropout_rate=dropout_rate, padding='same', name=f"{name}/Conv{kernel_size}x{kernel_size}")
+        return WSConv2D(filters=filters, kernel_size=kernel_size, strides = downscale, dilation_rate = dilation, activation=activation, dropout_rate=dropout_rate, padding='same', name=f"{name}/Conv{ker_size_to_string(kernel_size)}")
     elif batch_norm or dropout_rate>0:
-        return Conv2DBNDrop(filters=filters, kernel_size=kernel_size, strides = downscale, dilation = dilation, activation=activation, dropout_rate=dropout_rate, batch_norm=batch_norm, l2_reg=l2_reg, name=f"{name}/Conv{kernel_size}x{kernel_size}")
+        return Conv2DBNDrop(filters=filters, kernel_size=kernel_size, strides = downscale, dilation = dilation, activation=activation, dropout_rate=dropout_rate, batch_norm=batch_norm, l2_reg=l2_reg, name=f"{name}/Conv{ker_size_to_string(kernel_size)}")
     else:
         kernel_regularizer=tf.keras.regularizers.l2(l2_reg) if l2_reg>0 else None
-        return tf.keras.layers.Conv2D(filters=filters, kernel_size=kernel_size, strides = downscale, dilation_rate = dilation, padding='same', activation=activation, kernel_regularizer=kernel_regularizer, name=f"{name}/Conv{kernel_size}x{kernel_size}")
+        return tf.keras.layers.Conv2D(filters=filters, kernel_size=kernel_size, strides = downscale, dilation_rate = dilation, padding='same', activation=activation, kernel_regularizer=kernel_regularizer, name=f"{name}/Conv{ker_size_to_string(kernel_size)}")
```

### Comparing `DiSTNet2D-0.1.3/distnet_2d/model/distnet_2d_seg.py` & `distnet2d-0.1.4/distnet_2d/model/distnet_2d_seg.py`

 * *Files identical despite different names*

### Comparing `DiSTNet2D-0.1.3/distnet_2d/model/gradient_accumulator.py` & `distnet2d-0.1.4/distnet_2d/model/gradient_accumulator.py`

 * *Files identical despite different names*

### Comparing `DiSTNet2D-0.1.3/distnet_2d/model/layers.py` & `distnet2d-0.1.4/distnet_2d/model/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,25 +289,25 @@
         input_channels = int(input_shape[-1])
         conv_fun = WSConv2D if self.weight_scaled else (SplitConv2D if self.split_conv else tf.keras.layers.Conv2D)
         self.conv1 = conv_fun(
             filters=input_channels,
             kernel_size=self.kernel_size,
             strides=1,
             padding='same',
-            name=f"{self.name}/1_{self.kernel_size}x{self.kernel_size}",
+            name=f"{self.name}/1_{ker_size_to_string(self.kernel_size)}",
             activation="linear",
             #kernel_regularizer=tf.keras.regularizers.l2(self.l2_reg) if self.l2_reg>0 else None
         )
         self.conv2 = conv_fun(
             filters=input_channels,
             kernel_size=self.kernel_size,
             dilation_rate = self.dilation,
             strides=1,
             padding='same',
-            name=f"{self.name}/2_{self.kernel_size}x{self.kernel_size}",
+            name=f"{self.name}/2_{ker_size_to_string(self.kernel_size)}",
             activation="linear",
             #kernel_regularizer=tf.keras.regularizers.l2(self.l2_reg) if self.l2_reg>0 else None
         )
         self.gamma = get_gamma(self.activation) if self.weight_scaled else 1.
         self.activation_layer = tf.keras.activations.get(self.activation)
         if self.dropout_rate>0:
             self.drop = tf.keras.layers.SpatialDropout2D(self.dropout_rate)
@@ -364,15 +364,15 @@
     def build(self, input_shape):
         self.conv = tf.keras.layers.Conv2D(
             filters=self.filters,
             kernel_size=self.kernel_size,
             dilation_rate = self.dilation,
             strides=self.strides,
             padding='same',
-            name=f"{self.name}/{self.kernel_size}",
+            name=f"{self.name}/Conv",
             activation="linear",
             kernel_regularizer=tf.keras.regularizers.l2(self.l2_reg) if self.l2_reg>0 else None
         )
         self.activation_layer = tf.keras.activations.get(self.activation)
         if self.dropout_rate>0:
             self.drop = tf.keras.layers.SpatialDropout2D(self.dropout_rate)
         if self.batch_norm:
@@ -417,15 +417,15 @@
         self.conv = tf.keras.layers.Conv2DTranspose(
             filters=self.filters,
             kernel_size=self.kernel_size,
             strides=self.strides,
             padding='same',
             activation="linear",
             kernel_regularizer=tf.keras.regularizers.l2(self.l2_reg) if self.l2_reg>0 else None,
-            name=f"{self.name}/tConv{self.kernel_size}x{self.kernel_size}",
+            name=f"{self.name}/tConv{ker_size_to_string(self.kernel_size)}",
         )
         self.activation_layer = tf.keras.activations.get(self.activation)
         if self.dropout_rate>0:
             self.drop = tf.keras.layers.SpatialDropout2D(self.dropout_rate, name=f"{self.name}/Dropout")
         if self.batch_norm:
             #self.bn = MockBatchNormalization(name = f"{self.name}/MockBatchNormalization")
             self.bn = tf.keras.layers.BatchNormalization(name = f"{self.name}/BatchNormalization")
@@ -478,15 +478,15 @@
             dilation_rate = self.dilation,
             strides=self.strides,
             padding=self.padding,
             name=name,
             activation="linear",
             kernel_regularizer=self.kernel_regularizer
         )
-        self.convs = [conv_fun(f"{self.name}/{self.kernel_size}_{i}") for i in range(3)]
+        self.convs = [conv_fun(f"{self.name}/Conv_{i}") for i in range(3)]
         self.activation_layer = tf.keras.activations.get(self.activation)
         if self.dropout_rate>0:
             self.drop = tf.keras.layers.SpatialDropout2D(self.dropout_rate)
         if self.batch_norm:
             self.bn = tf.keras.layers.BatchNormalization()
         super().build(input_shape)
 
@@ -607,7 +607,12 @@
 
     def call(self, inputs):
         weights = self.weight[tf.newaxis, tf.newaxis, tf.newaxis]
         if not self.per_channel:
             weights = weights[tf.newaxis]
         mul = tf.math.multiply(tf.stack(inputs, axis = -1), weights)
         return tf.math.reduce_sum(mul, axis=-1, keepdims = False)
+
+def ker_size_to_string(ker_size, dims=2):
+    if not isinstance(ker_size, (list, tuple)):
+        ker_size = ensure_multiplicity(dims, ker_size)
+    return 'x'.join([str(k) for k in ker_size])
```

### Comparing `DiSTNet2D-0.1.3/distnet_2d/model/spatial_attention.py` & `distnet2d-0.1.4/distnet_2d/model/spatial_attention.py`

 * *Files identical despite different names*

### Comparing `DiSTNet2D-0.1.3/distnet_2d/utils/agc.py` & `distnet2d-0.1.4/distnet_2d/utils/agc.py`

 * *Files identical despite different names*

### Comparing `DiSTNet2D-0.1.3/distnet_2d/utils/callbacks.py` & `distnet2d-0.1.4/distnet_2d/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `DiSTNet2D-0.1.3/distnet_2d/utils/helpers.py` & `distnet2d-0.1.4/distnet_2d/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `DiSTNet2D-0.1.3/distnet_2d/utils/losses.py` & `distnet2d-0.1.4/distnet_2d/utils/losses.py`

 * *Files identical despite different names*

### Comparing `DiSTNet2D-0.1.3/distnet_2d/utils/lovasz_loss.py` & `distnet2d-0.1.4/distnet_2d/utils/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `DiSTNet2D-0.1.3/distnet_2d/utils/objectwise_computation_tf.py` & `distnet2d-0.1.4/distnet_2d/utils/objectwise_computation_tf.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 # assumes iterator in return_central_only= True (thus framewindow = 1 and next = true)
 def get_metrics_fun(spatial_dims, center_scale:float, max_objects_number:int=0, reduce:bool=True):
     spatial_dims = ensure_multiplicity(2, spatial_dims)
     scale = tf.cast(center_scale, tf.float32)
     coord_distance_fun = _coord_distance_fun()
     spa_wmean_fun = _get_spatial_wmean_by_object_fun(*spatial_dims)
+    spa_max_fun = _get_soft_argmax_2d_by_object_fun(*spatial_dims)
     mean_fun = _get_mean_by_object_fun()
     mean_fun_lm = _get_mean_by_object_fun(nan=-1)
     def fun(args):
         edm, gdcm, dY, dX, lm, true_edm, true_dY, true_dX, true_lm, labels, prev_labels, true_center_ob = args
         labels = tf.transpose(labels, perm=[2, 0, 1]) # T, Y, X
         gdcm = tf.transpose(gdcm, perm=[2, 0, 1])
         edm = tf.transpose(edm, perm=[2, 0, 1])
@@ -36,15 +37,15 @@
         edm_IoU = 0.5 * (edm_IoU + contour_IoU)
 
         #mask = tf.where(labels > 0, one, zero)
         #edm_L2 = tf.math.divide_no_nan(tf.math.reduce_sum(mask * (edm - true_edm) ** 2), tf.cast(tf.reduce_sum(sizes), edm.dtype))
 
         # CENTER  compute center coordinates per objects: spatial mean of predicted gaussian function of GDCM
         center_values = tf.math.exp(-tf.math.square(tf.math.divide(gdcm, scale)))
-        center_coord = _objectwise_compute(center_values, [0], spa_wmean_fun, labels, ids, sizes) # (N, 2)
+        center_coord = _objectwise_compute(center_values, [0], spa_max_fun, labels, ids, sizes) # (N, 2)
         #print(f"center: {tf.concat([true_center_ob[0], center_coord[0]], -1).numpy()}")
         center_l2 = coord_distance_fun(true_center_ob, center_coord)
         center_l2 = tf.cond(tf.math.is_nan(center_l2), lambda: tf.cast(0, center_l2.dtype), lambda: center_l2)
 
         # motion: l2 of pred vs true center coordinates
         dYX = tf.stack([dY, dX], -1) # Y, X, T, 2
         dYX = tf.transpose(dYX, perm=[2, 0, 1, 3]) # T, Y, X, 2
@@ -108,21 +109,40 @@
             wsum = tf.stack([wsum_y, wsum_x]) # (2)
             sum = tf.reduce_sum(data_masked, keepdims = False)
             #sum = tf.stop_gradient(sum)
             return tf.math.divide(wsum, sum) # when no values should return nan # (2)
         return tf.cond(tf.math.equal(size, 0), lambda:tf.stack([nan, nan]), non_null)
     return apply
 
+def _get_soft_argmax_2d_by_object_fun(Y, X, beta=1e2):
+    Y, X = tf.meshgrid(tf.range(Y, dtype=tf.float32), tf.range(X, dtype=tf.float32), indexing='ij')
+    nan = tf.cast(float('NaN'), tf.float32)
+    def sam(data, mask, size): # (Y, X)
+        def non_null():
+            shape = tf.shape(data)
+            data_masked = tf.math.multiply_no_nan(data, mask)
+            data_masked = tf.reshape(data_masked, (-1,)) # (X * Y,)
+            data_masked = tf.nn.softmax(data_masked * beta, axis = 0)
+            data_masked = tf.reshape(data_masked, shape) # (X, Y)
+            argmax_y = tf.reduce_sum(data_masked * Y, axis=[0, 1], keepdims=False) # (1,)
+            argmax_x = tf.reduce_sum(data_masked * X, axis=[0, 1], keepdims=False) # (1,)
+            argmax = tf.stack([argmax_y, argmax_x], -1) # (2,)
+            sum = tf.reduce_sum(data_masked, keepdims=False)
+            # sum = tf.stop_gradient(sum)
+            return tf.math.divide(argmax, sum)  # when no values should return nan # (2)
+        return tf.cond(tf.math.equal(size, 0), lambda:tf.stack([nan, nan]), non_null) # when no values should return nan
+    return sam
+
 def _get_mean_by_object_fun(nan=float('NaN')):
     nan = tf.cast(nan, tf.float32)
     def fun(data, mask, size): # (Y, X, C)
         mask = tf.expand_dims(mask, -1)
-        nan_tensor = tf.repeat(nan, repeats=tf.shape(data)[-1])
+        null = lambda: tf.repeat(nan, repeats=tf.shape(data)[-1])
         non_null = lambda: tf.math.divide(tf.reduce_sum(tf.math.multiply_no_nan(data, mask), axis=[0, 1], keepdims=False), tf.cast(size, tf.float32))
-        return tf.cond(tf.math.equal(size, 0), lambda:nan_tensor, non_null)
+        return tf.cond(tf.math.equal(size, 0), null, non_null)
     return fun
 
 def _objectwise_compute(data, channels, fun, labels, ids, sizes, label_channels=None): # [(tensor, range, fun)], (T, Y, X), (T, N), (T, N)
     if label_channels is None:
         label_channels = channels
     else:
         assert len(label_channels) == len(channels), "label_channels and channels must have same length"
@@ -130,15 +150,15 @@
         dc, lc = args
         return _objectwise_compute_channel(data[dc], fun, labels[lc], ids[lc], sizes[lc])
     return tf.map_fn(treat_im, (tf.convert_to_tensor(channels), tf.convert_to_tensor(label_channels)), fn_output_signature=data.dtype)
 
 def _objectwise_compute_channel(data, fun, labels, ids, sizes): # tensor, fun, (Y, X), (N), ( N)
     def treat_ob(args):
         id, size = args
-        mask = tf.cond(tf.math.equal(id, 0), lambda:0., lambda:tf.cast(tf.math.equal(labels, id), tf.float32))
+        mask = tf.cond(tf.math.equal(id, 0), lambda:tf.zeros_like(labels, dtype=tf.float32), lambda:tf.cast(tf.math.equal(labels, id), tf.float32))
         return fun(data, mask, size)
     return tf.map_fn(treat_ob, (ids, sizes), fn_output_signature=data.dtype)
 
 def _coord_distance_fun():
     def loss(true, pred): # (C, N, 2)
         no_na_mask = tf.stop_gradient(tf.cast(tf.math.logical_not(tf.math.logical_or(tf.math.is_nan(true[...,:1]), tf.math.is_nan(pred[...,:1]))), tf.float32)) # non-empty objects # (C, N, 1)
         n_obj = tf.reduce_sum(no_na_mask[...,0], axis=-1, keepdims=False) # (C)
@@ -177,15 +197,15 @@
             kernel = np.tile(kernel,rep) # (Y, X, C, O, 2)
     return kernel
 
 def _IoU(true, pred, tolerance:bool=False):
     true_inter = _dilate_mask(true) if tolerance else true
     intersection = tf.math.count_nonzero(tf.math.logical_and(true_inter, pred))
     union = tf.math.count_nonzero(tf.math.logical_or(true, pred))
-    return tf.math.divide_no_nan(tf.cast(intersection, tf.float32), tf.cast(union, tf.float32))
+    return tf.cond(tf.math.equal(union, tf.cast(0, union.dtype)), lambda: tf.cast(1., tf.float32), lambda: tf.math.divide(tf.cast(intersection, tf.float32), tf.cast(union, tf.float32)))
 
 def _dilate_mask(maskYX):
     maskYX = tf.cast(maskYX, tf.float16)
     mean_kernel = [[1./9, 1./9, 1./9], [1./9, 1./9, 1./9], [1./9, 1./9, 1./9]]
     conv = _convolve(maskYX, tf.cast(mean_kernel, tf.float16))
     return tf.math.greater(conv, tf.cast(0., tf.float16))
```

### Comparing `DiSTNet2D-0.1.3/setup.py` & `distnet2d-0.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="DiSTNet2D",
-    version="0.1.3",
+    version="0.1.4",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="tensorflow/keras implementation of DiSTNet 2D",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/distnet2d",
-    download_url='https://github.com/jeanollion/distnet2d/releases/download/v0.1.3/distnet2d-0.1.3.tar.gz',
+    download_url='https://github.com/jeanollion/distnet2d/releases/download/v0.1.4/distnet2d-0.1.4.tar.gz',
     packages=setuptools.find_packages(),
     keywords=['Segmentation', 'Tracking', 'Cell', 'Tensorflow', 'Keras'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Programming Language :: Python :: 3',
     ],
     python_requires='>=3',
-    install_requires=['numpy', 'scipy', 'tensorflow>=2.7.1', 'edt>=2.0.2', 'scikit-fmm', 'numba', 'dataset_iterator>=0.4.0', 'elasticdeform>=0.4.7']
+    install_requires=['numpy', 'scipy', 'tensorflow>=2.7.1', 'edt>=2.0.2', 'scikit-fmm', 'numba', 'dataset_iterator>=0.4.2', 'elasticdeform>=0.4.7']
 )
```

