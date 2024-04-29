# Comparing `tmp/pyzjr-1.3.6.tar.gz` & `tmp/pyzjr-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyzjr-1.3.6.tar", last modified: Mon Apr 29 07:32:59 2024, max compression
+gzip compressed data, was "dist\pyzjr-1.3.7.tar", last modified: Mon Apr 29 07:56:56 2024, max compression
```

## Comparing `pyzjr-1.3.6.tar` & `pyzjr-1.3.7.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/
--rw-rw-rw-   0        0        0     1075 2023-06-10 05:53:06.000000 pyzjr-1.3.6/LICENSE
--rw-rw-rw-   0        0        0     2931 2024-04-29 07:32:59.000000 pyzjr-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     2124 2024-01-25 07:09:34.000000 pyzjr-1.3.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/models_img/
--rw-rw-rw-   0        0        0        0 2024-03-04 11:15:31.000000 pyzjr-1.3.6/models_img/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Math/
--rw-rw-rw-   0        0        0      689 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/Math/Numpy.py
--rw-rw-rw-   0        0        0      212 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/Math/__init__.py
--rw-rw-rw-   0        0        0     3438 2024-02-20 09:48:40.000000 pyzjr-1.3.6/pyzjr/Math/arithmetic.py
--rw-rw-rw-   0        0        0      134 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/Math/constant.py
--rw-rw-rw-   0        0        0     7362 2024-02-19 10:31:56.000000 pyzjr-1.3.6/pyzjr/Math/function.py
--rw-rw-rw-   0        0        0    19620 2024-02-19 09:52:53.000000 pyzjr-1.3.6/pyzjr/Math/point_line.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/Attention/
--rw-rw-rw-   0        0        0     2271 2024-03-04 07:16:29.000000 pyzjr-1.3.6/pyzjr/Models/Attention/A2.py
--rw-rw-rw-   0        0        0     1927 2024-03-09 14:59:27.000000 pyzjr-1.3.6/pyzjr/Models/Attention/AFT.py
--rw-rw-rw-   0        0        0     1911 2024-03-09 15:28:12.000000 pyzjr-1.3.6/pyzjr/Models/Attention/DANet.py
--rw-rw-rw-   0        0        0     5412 2024-03-09 15:10:59.000000 pyzjr-1.3.6/pyzjr/Models/Attention/MobileViT.py
--rw-rw-rw-   0        0        0     3105 2024-03-21 17:03:45.000000 pyzjr-1.3.6/pyzjr/Models/Attention/SE.py
--rw-rw-rw-   0        0        0     1933 2024-03-09 15:18:47.000000 pyzjr-1.3.6/pyzjr/Models/Attention/ViP.py
--rw-rw-rw-   0        0        0     1589 2024-04-20 07:26:32.000000 pyzjr-1.3.6/pyzjr/Models/Attention/__init__.py
--rw-rw-rw-   0        0        0     4795 2024-03-09 14:59:04.000000 pyzjr-1.3.6/pyzjr/Models/Attention/acmix.py
--rw-rw-rw-   0        0        0    12705 2024-03-09 15:00:08.000000 pyzjr-1.3.6/pyzjr/Models/Attention/axial.py
--rw-rw-rw-   0        0        0     3180 2024-03-04 07:32:10.000000 pyzjr-1.3.6/pyzjr/Models/Attention/bam.py
--rw-rw-rw-   0        0        0     3729 2024-03-04 12:35:57.000000 pyzjr-1.3.6/pyzjr/Models/Attention/cbam.py
--rw-rw-rw-   0        0        0     1635 2024-03-09 15:01:57.000000 pyzjr-1.3.6/pyzjr/Models/Attention/coord.py
--rw-rw-rw-   0        0        0     2175 2024-03-04 12:19:45.000000 pyzjr-1.3.6/pyzjr/Models/Attention/cot.py
--rw-rw-rw-   0        0        0     2688 2024-03-09 15:02:25.000000 pyzjr-1.3.6/pyzjr/Models/Attention/crisscross.py
--rw-rw-rw-   0        0        0    26854 2024-03-09 15:22:58.000000 pyzjr-1.3.6/pyzjr/Models/Attention/crossformer.py
--rw-rw-rw-   0        0        0    23025 2024-03-09 15:25:56.000000 pyzjr-1.3.6/pyzjr/Models/Attention/dat.py
--rw-rw-rw-   0        0        0     1340 2024-03-09 15:04:58.000000 pyzjr-1.3.6/pyzjr/Models/Attention/eca.py
--rw-rw-rw-   0        0        0     3752 2024-03-09 15:05:31.000000 pyzjr-1.3.6/pyzjr/Models/Attention/emsa.py
--rw-rw-rw-   0        0        0     1341 2024-03-09 15:06:14.000000 pyzjr-1.3.6/pyzjr/Models/Attention/external.py
--rw-rw-rw-   0        0        0     4161 2024-03-09 15:19:38.000000 pyzjr-1.3.6/pyzjr/Models/Attention/gfnet.py
--rw-rw-rw-   0        0        0     5444 2024-03-09 15:07:26.000000 pyzjr-1.3.6/pyzjr/Models/Attention/halo.py
--rw-rw-rw-   0        0        0    30578 2024-03-09 15:23:53.000000 pyzjr-1.3.6/pyzjr/Models/Attention/moat.py
--rw-rw-rw-   0        0        0     3670 2024-03-09 15:08:27.000000 pyzjr-1.3.6/pyzjr/Models/Attention/muse.py
--rw-rw-rw-   0        0        0     2281 2024-03-09 15:11:27.000000 pyzjr-1.3.6/pyzjr/Models/Attention/outlook.py
--rw-rw-rw-   0        0        0      985 2024-03-09 15:29:37.000000 pyzjr-1.3.6/pyzjr/Models/Attention/parnet.py
--rw-rw-rw-   0        0        0     4087 2024-03-09 15:13:38.000000 pyzjr-1.3.6/pyzjr/Models/Attention/polarized.py
--rw-rw-rw-   0        0        0     2296 2024-03-09 15:11:51.000000 pyzjr-1.3.6/pyzjr/Models/Attention/psa.py
--rw-rw-rw-   0        0        0      930 2024-03-09 14:57:03.000000 pyzjr-1.3.6/pyzjr/Models/Attention/residual.py
--rw-rw-rw-   0        0        0     2355 2024-03-09 14:52:15.000000 pyzjr-1.3.6/pyzjr/Models/Attention/s2.py
--rw-rw-rw-   0        0        0     3084 2024-03-09 15:15:20.000000 pyzjr-1.3.6/pyzjr/Models/Attention/self_att.py
--rw-rw-rw-   0        0        0     1784 2024-03-09 15:14:10.000000 pyzjr-1.3.6/pyzjr/Models/Attention/sge.py
--rw-rw-rw-   0        0        0     2637 2024-03-09 15:16:05.000000 pyzjr-1.3.6/pyzjr/Models/Attention/shuffle.py
--rw-rw-rw-   0        0        0      909 2024-03-09 15:16:39.000000 pyzjr-1.3.6/pyzjr/Models/Attention/simam.py
--rw-rw-rw-   0        0        0     2933 2024-03-09 15:17:26.000000 pyzjr-1.3.6/pyzjr/Models/Attention/simplified_self_att.py
--rw-rw-rw-   0        0        0     1863 2024-03-18 11:12:03.000000 pyzjr-1.3.6/pyzjr/Models/Attention/sk.py
--rw-rw-rw-   0        0        0     2349 2024-03-09 15:18:03.000000 pyzjr-1.3.6/pyzjr/Models/Attention/triplet.py
--rw-rw-rw-   0        0        0     2234 2024-03-04 13:24:57.000000 pyzjr-1.3.6/pyzjr/Models/Attention/ufo.py
--rw-rw-rw-   0        0        0      220 2024-03-16 15:32:39.000000 pyzjr-1.3.6/pyzjr/Models/__init__.py
--rw-rw-rw-   0        0        0     3384 2024-03-21 16:32:55.000000 pyzjr-1.3.6/pyzjr/Models/_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/backbone/
--rw-rw-rw-   0        0        0     5692 2024-03-22 16:07:30.000000 pyzjr-1.3.6/pyzjr/Models/backbone/Darknet.py
--rw-rw-rw-   0        0        0    25919 2024-02-23 14:10:01.000000 pyzjr-1.3.6/pyzjr/Models/backbone/Ghostnet.py
--rw-rw-rw-   0        0        0     1953 2024-03-26 15:38:25.000000 pyzjr-1.3.6/pyzjr/Models/backbone/__init__.py
--rw-rw-rw-   0        0        0     1935 2024-04-01 07:58:53.000000 pyzjr-1.3.6/pyzjr/Models/backbone/alexnet.py
--rw-rw-rw-   0        0        0     7560 2024-02-23 14:18:22.000000 pyzjr-1.3.6/pyzjr/Models/backbone/conv2former.py
--rw-rw-rw-   0        0        0     6278 2024-02-23 14:18:22.000000 pyzjr-1.3.6/pyzjr/Models/backbone/densenet.py
--rw-rw-rw-   0        0        0    12866 2024-04-01 09:42:37.000000 pyzjr-1.3.6/pyzjr/Models/backbone/drn.py
--rw-rw-rw-   0        0        0    17934 2024-04-01 08:53:51.000000 pyzjr-1.3.6/pyzjr/Models/backbone/efficientnet.py
--rw-rw-rw-   0        0        0     7210 2024-04-01 09:54:02.000000 pyzjr-1.3.6/pyzjr/Models/backbone/fasternet.py
--rw-rw-rw-   0        0        0     5623 2024-02-23 14:18:22.000000 pyzjr-1.3.6/pyzjr/Models/backbone/googlenet.py
--rw-rw-rw-   0        0        0     1869 2024-02-04 04:44:18.000000 pyzjr-1.3.6/pyzjr/Models/backbone/lenet.py
--rw-rw-rw-   0        0        0     7048 2024-03-18 16:29:49.000000 pyzjr-1.3.6/pyzjr/Models/backbone/mnasnet.py
--rw-rw-rw-   0        0        0    16395 2024-02-16 16:51:01.000000 pyzjr-1.3.6/pyzjr/Models/backbone/mobilenet.py
--rw-rw-rw-   0        0        0     9972 2024-04-18 15:14:36.000000 pyzjr-1.3.6/pyzjr/Models/backbone/nasnet.py
--rw-rw-rw-   0        0        0     7217 2024-03-18 11:17:15.000000 pyzjr-1.3.6/pyzjr/Models/backbone/regnet.py
--rw-rw-rw-   0        0        0     8910 2024-04-01 09:47:10.000000 pyzjr-1.3.6/pyzjr/Models/backbone/resnet.py
--rw-rw-rw-   0        0        0    11356 2024-03-22 15:56:05.000000 pyzjr-1.3.6/pyzjr/Models/backbone/shufflenet.py
--rw-rw-rw-   0        0        0     4392 2024-03-04 12:30:07.000000 pyzjr-1.3.6/pyzjr/Models/backbone/squeezenet.py
--rw-rw-rw-   0        0        0     3996 2024-02-25 16:22:54.000000 pyzjr-1.3.6/pyzjr/Models/backbone/vgg.py
--rw-rw-rw-   0        0        0     5866 2024-04-01 09:44:12.000000 pyzjr-1.3.6/pyzjr/Models/backbone/xception.py
--rw-rw-rw-   0        0        0     2705 2024-03-22 15:32:04.000000 pyzjr-1.3.6/pyzjr/Models/backbone/zfnet.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/bricks/
--rw-rw-rw-   0        0        0     5577 2024-04-01 09:57:01.000000 pyzjr-1.3.6/pyzjr/Models/bricks/Initer.py
--rw-rw-rw-   0        0        0      426 2024-04-18 15:04:29.000000 pyzjr-1.3.6/pyzjr/Models/bricks/__init__.py
--rw-rw-rw-   0        0        0     1577 2024-03-04 09:07:17.000000 pyzjr-1.3.6/pyzjr/Models/bricks/classfier.py
--rw-rw-rw-   0        0        0    22575 2024-03-04 07:32:10.000000 pyzjr-1.3.6/pyzjr/Models/bricks/comblock.py
--rw-rw-rw-   0        0        0     2646 2024-03-26 15:25:44.000000 pyzjr-1.3.6/pyzjr/Models/bricks/conv_norm_act.py
--rw-rw-rw-   0        0        0     6828 2024-03-04 12:40:27.000000 pyzjr-1.3.6/pyzjr/Models/bricks/drop.py
--rw-rw-rw-   0        0        0     6669 2024-03-06 00:10:20.000000 pyzjr-1.3.6/pyzjr/Models/bricks/mlp.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/conv/
--rw-rw-rw-   0        0        0     1974 2024-04-18 13:35:49.000000 pyzjr-1.3.6/pyzjr/Models/conv/Depthwise_Conv.py
--rw-rw-rw-   0        0        0      508 2024-03-21 15:46:28.000000 pyzjr-1.3.6/pyzjr/Models/conv/Dilated_Conv.py
--rw-rw-rw-   0        0        0     1862 2024-02-29 10:04:41.000000 pyzjr-1.3.6/pyzjr/Models/conv/Partial_Conv.py
--rw-rw-rw-   0        0        0     2660 2024-02-29 10:02:23.000000 pyzjr-1.3.6/pyzjr/Models/conv/Ref_Conv.py
--rw-rw-rw-   0        0        0    11456 2024-04-28 14:23:02.000000 pyzjr-1.3.6/pyzjr/Models/conv/Snake_Conv.py
--rw-rw-rw-   0        0        0      295 2024-03-21 15:46:28.000000 pyzjr-1.3.6/pyzjr/Models/conv/__init__.py
--rw-rw-rw-   0        0        0     3029 2024-04-14 00:39:15.000000 pyzjr-1.3.6/pyzjr/Models/networks.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/sampling/
--rw-rw-rw-   0        0        0      754 2024-04-05 14:24:23.000000 pyzjr-1.3.6/pyzjr/Models/sampling/__init__.py
--rw-rw-rw-   0        0        0     4857 2024-04-05 16:18:30.000000 pyzjr-1.3.6/pyzjr/Models/sampling/adaptivepooling.py
--rw-rw-rw-   0        0        0     1393 2024-01-27 17:10:24.000000 pyzjr-1.3.6/pyzjr/Models/sampling/haarwavelet.py
--rw-rw-rw-   0        0        0     1828 2024-03-04 13:56:06.000000 pyzjr-1.3.6/pyzjr/Models/sampling/medianpooling.py
--rw-rw-rw-   0        0        0     4792 2024-02-26 15:35:21.000000 pyzjr-1.3.6/pyzjr/Models/sampling/standardpooling.py
--rw-rw-rw-   0        0        0      854 2024-03-01 15:33:22.000000 pyzjr-1.3.6/pyzjr/Models/sampling/strideconv.py
--rw-rw-rw-   0        0        0     3692 2024-02-29 15:43:47.000000 pyzjr-1.3.6/pyzjr/Models/sampling/strippooling.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/segmentation/
--rw-rw-rw-   0        0        0       70 2024-02-27 16:31:33.000000 pyzjr-1.3.6/pyzjr/Models/segmentation/__init__.py
--rw-rw-rw-   0        0        0    24988 2024-03-17 06:46:22.000000 pyzjr-1.3.6/pyzjr/Models/segmentation/fcn.py
--rw-rw-rw-   0        0        0     3289 2024-02-29 09:20:12.000000 pyzjr-1.3.6/pyzjr/Models/segmentation/unet.py
--rw-rw-rw-   0        0        0     6328 2024-04-20 07:32:10.000000 pyzjr-1.3.6/pyzjr/PIC.py
--rw-rw-rw-   0        0        0    10349 2024-02-04 05:11:03.000000 pyzjr-1.3.6/pyzjr/Z.py
--rw-rw-rw-   0        0        0      896 2024-04-14 00:39:15.000000 pyzjr-1.3.6/pyzjr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/augmentation/
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/
--rw-rw-rw-   0        0        0    13180 2024-04-13 15:26:35.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/Crack.py
--rw-rw-rw-   0        0        0     8307 2024-02-29 15:56:54.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/_Steger.py
--rw-rw-rw-   0        0        0      366 2024-02-19 10:23:26.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/__init__.py
--rw-rw-rw-   0        0        0     7681 2024-02-18 17:28:31.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/definition.py
--rw-rw-rw-   0        0        0     4835 2024-04-29 07:32:55.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/pixel.py
--rw-rw-rw-   0        0        0     1685 2024-04-13 15:00:07.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/utils.py
--rw-rw-rw-   0        0        0      116 2024-04-13 14:32:14.000000 pyzjr-1.3.6/pyzjr/augmentation/__init__.py
--rw-rw-rw-   0        0        0    28649 2024-04-25 17:12:47.000000 pyzjr-1.3.6/pyzjr/augmentation/augments.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/
--rw-rw-rw-   0        0        0      306 2024-02-01 16:36:53.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/__init__.py
--rw-rw-rw-   0        0        0     2192 2024-02-02 16:09:04.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/_utils.py
--rw-rw-rw-   0        0        0     3413 2024-02-28 11:40:46.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/normal.py
--rw-rw-rw-   0        0        0    10459 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/opencv.py
--rw-rw-rw-   0        0        0    40685 2024-04-25 17:14:56.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/pillow.py
--rw-rw-rw-   0        0        0     6139 2024-03-21 17:03:45.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/tvision.py
--rw-rw-rw-   0        0        0     1084 2024-03-04 06:15:09.000000 pyzjr-1.3.6/pyzjr/augmentation/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/core/
--rw-rw-rw-   0        0        0     1136 2024-04-23 16:30:06.000000 pyzjr-1.3.6/pyzjr/core/__init__.py
--rw-rw-rw-   0        0        0     6991 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/core/__tensor.py
--rw-rw-rw-   0        0        0      680 2023-10-07 12:04:40.000000 pyzjr-1.3.6/pyzjr/core/_utils.py
--rw-rw-rw-   0        0        0      982 2024-04-28 11:13:49.000000 pyzjr-1.3.6/pyzjr/core/decorator.py
--rw-rw-rw-   0        0        0     2123 2024-04-23 16:46:56.000000 pyzjr-1.3.6/pyzjr/core/error.py
--rw-rw-rw-   0        0        0     2692 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/core/general.py
--rw-rw-rw-   0        0        0      671 2024-04-23 16:26:12.000000 pyzjr-1.3.6/pyzjr/core/helpers.py
--rw-rw-rw-   0        0        0     7254 2023-11-15 11:43:15.000000 pyzjr-1.3.6/pyzjr/core/lr_scheduler.py
--rw-rw-rw-   0        0        0    15534 2024-04-21 15:07:11.000000 pyzjr-1.3.6/pyzjr/core/utils_pytorch_numpy_unification.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/data/
--rw-rw-rw-   0        0        0     1486 2024-03-13 01:39:58.000000 pyzjr-1.3.6/pyzjr/data/Dataloader.py
--rw-rw-rw-   0        0        0     9590 2024-03-08 01:06:58.000000 pyzjr-1.3.6/pyzjr/data/Dataset.py
--rw-rw-rw-   0        0        0    12147 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/data/FM.py
--rw-rw-rw-   0        0        0      215 2024-04-14 15:31:09.000000 pyzjr-1.3.6/pyzjr/data/__init__.py
--rw-rw-rw-   0        0        0     4064 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/data/basedataset.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/data/data_set/
--rw-rw-rw-   0        0        0     9436 2024-03-13 01:39:58.000000 pyzjr-1.3.6/pyzjr/data/data_set/Pascal_voc.py
--rw-rw-rw-   0        0        0        0 2024-02-29 16:00:47.000000 pyzjr-1.3.6/pyzjr/data/data_set/__init__.py
--rw-rw-rw-   0        0        0     1313 2024-03-08 01:30:08.000000 pyzjr-1.3.6/pyzjr/data/data_set/config.py
--rw-rw-rw-   0        0        0    15340 2024-04-13 15:04:54.000000 pyzjr-1.3.6/pyzjr/data/reader.py
--rw-rw-rw-   0        0        0      934 2024-04-14 15:26:14.000000 pyzjr-1.3.6/pyzjr/data/txt_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/devices/
--rw-rw-rw-   0        0        0      523 2024-04-27 13:06:29.000000 pyzjr-1.3.6/pyzjr/devices/__init__.py
--rw-rw-rw-   0        0        0     1572 2024-04-13 15:22:13.000000 pyzjr-1.3.6/pyzjr/devices/get_device.py
--rw-rw-rw-   0        0        0     3032 2024-04-27 13:06:29.000000 pyzjr-1.3.6/pyzjr/devices/measures.py
--rw-rw-rw-   0        0        0     1202 2024-04-13 15:53:39.000000 pyzjr-1.3.6/pyzjr/devices/systeminfo.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/dlearn/
--rw-rw-rw-   0        0        0      949 2024-03-11 15:45:28.000000 pyzjr-1.3.6/pyzjr/dlearn/__init__.py
--rw-rw-rw-   0        0        0     8571 2024-02-17 18:07:27.000000 pyzjr-1.3.6/pyzjr/dlearn/callbacklog.py
--rw-rw-rw-   0        0        0     8379 2024-03-13 01:39:58.000000 pyzjr-1.3.6/pyzjr/dlearn/callbacks.py
--rw-rw-rw-   0        0        0     1051 2024-03-11 15:59:35.000000 pyzjr-1.3.6/pyzjr/dlearn/savemodels.py
--rw-rw-rw-   0        0        0     5603 2024-04-25 13:21:27.000000 pyzjr-1.3.6/pyzjr/dlearn/strategy.py
--rw-rw-rw-   0        0        0     5955 2024-04-13 15:28:23.000000 pyzjr-1.3.6/pyzjr/dlearn/tools.py
--rw-rw-rw-   0        0        0     7356 2024-04-27 09:06:57.000000 pyzjr-1.3.6/pyzjr/dlearn/trainer.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/nn/
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/
--rw-rw-rw-   0        0        0      768 2024-04-28 11:08:26.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/__init__.py
--rw-rw-rw-   0        0        0    16268 2024-04-28 09:10:34.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/classification.py
--rw-rw-rw-   0        0        0     3822 2024-04-28 09:10:34.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/indexutils.py
--rw-rw-rw-   0        0        0     9779 2024-04-28 09:10:34.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/medical_index.py
--rw-rw-rw-   0        0        0     5837 2024-04-27 18:14:38.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/segment3d.py
--rw-rw-rw-   0        0        0    11847 2024-04-28 09:10:34.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/semantic.py
--rw-rw-rw-   0        0        0     9459 2024-04-18 15:17:33.000000 pyzjr-1.3.6/pyzjr/nn/Summary.py
--rw-rw-rw-   0        0        0      123 2024-04-18 15:17:33.000000 pyzjr-1.3.6/pyzjr/nn/__init__.py
--rw-rw-rw-   0        0        0    84332 2024-02-22 15:45:34.000000 pyzjr-1.3.6/pyzjr/nn/functional.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/
--rw-rw-rw-   0        0        0     3262 2024-04-27 18:28:45.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/OneHot.py
--rw-rw-rw-   0        0        0      835 2024-04-28 10:41:07.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/__init__.py
--rw-rw-rw-   0        0        0     7197 2024-04-27 18:54:23.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/avgweight.py
--rw-rw-rw-   0        0        0    15225 2024-02-20 09:56:56.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/learnrate.py
--rw-rw-rw-   0        0        0    27275 2024-04-28 11:08:26.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/loss_function.py
--rw-rw-rw-   0        0        0     5217 2024-04-28 10:13:24.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/loss_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/torch3D/
--rw-rw-rw-   0        0        0       57 2024-04-28 14:21:27.000000 pyzjr-1.3.6/pyzjr/torch3D/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/
--rw-rw-rw-   0        0        0      266 2024-04-28 14:17:48.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/__init__.py
--rw-rw-rw-   0        0        0     6344 2024-04-28 12:59:48.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/basic_unet.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/block/
--rw-rw-rw-   0        0        0    22077 2024-04-28 11:42:36.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/block/DSConv.py
--rw-rw-rw-   0        0        0       28 2024-04-28 11:44:10.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/block/__init__.py
--rw-rw-rw-   0        0        0     7862 2024-04-28 12:59:48.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/dscnet.py
--rw-rw-rw-   0        0        0     5755 2024-04-28 13:34:14.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/vent.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/torch3D/nii/
--rw-rw-rw-   0        0        0      306 2024-04-28 11:13:49.000000 pyzjr-1.3.6/pyzjr/torch3D/nii/__init__.py
--rw-rw-rw-   0        0        0     4420 2024-04-27 18:49:10.000000 pyzjr-1.3.6/pyzjr/torch3D/nii/mri.py
--rw-rw-rw-   0        0        0     4363 2024-04-28 12:59:48.000000 pyzjr-1.3.6/pyzjr/torch3D/nii/nifti_dataset.py
--rw-rw-rw-   0        0        0     3373 2024-04-28 15:35:45.000000 pyzjr-1.3.6/pyzjr/torch3D/nii/nii_utils.py
--rw-rw-rw-   0        0        0       21 2024-04-29 07:32:55.000000 pyzjr-1.3.6/pyzjr/version.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/visualize/
--rw-rw-rw-   0        0        0      410 2024-04-14 15:13:36.000000 pyzjr-1.3.6/pyzjr/visualize/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/visualize/color/
--rw-rw-rw-   0        0        0     1418 2024-04-13 14:47:13.000000 pyzjr-1.3.6/pyzjr/visualize/color/__init__.py
--rw-rw-rw-   0        0        0     4848 2024-04-13 14:43:57.000000 pyzjr-1.3.6/pyzjr/visualize/color/colormap.py
--rw-rw-rw-   0        0        0     3339 2023-11-04 05:34:46.000000 pyzjr-1.3.6/pyzjr/visualize/color/colorspace.py
--rw-rw-rw-   0        0        0     7471 2024-04-13 14:47:13.000000 pyzjr-1.3.6/pyzjr/visualize/color/cvplot.py
--rw-rw-rw-   0        0        0     7937 2024-04-13 15:27:09.000000 pyzjr-1.3.6/pyzjr/visualize/color/findcolor.py
--rw-rw-rw-   0        0        0     1066 2024-02-13 17:07:55.000000 pyzjr-1.3.6/pyzjr/visualize/color/hex.py
--rw-rw-rw-   0        0        0    10972 2024-04-28 11:08:26.000000 pyzjr-1.3.6/pyzjr/visualize/io.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/visualize/mediapipe/
--rw-rw-rw-   0        0        0     6556 2024-04-14 15:13:36.000000 pyzjr-1.3.6/pyzjr/visualize/mediapipe/HandTrack.py
--rw-rw-rw-   0        0        0      376 2024-01-25 07:15:10.000000 pyzjr-1.3.6/pyzjr/visualize/mediapipe/__init__.py
--rw-rw-rw-   0        0        0      631 2024-02-04 05:11:03.000000 pyzjr-1.3.6/pyzjr/visualize/mediapipe/const.py
--rw-rw-rw-   0        0        0     4327 2024-04-13 15:04:54.000000 pyzjr-1.3.6/pyzjr/visualize/printf.py
--rw-rw-rw-   0        0        0     3367 2024-02-22 15:48:11.000000 pyzjr-1.3.6/pyzjr/visualize/utils.py
--rw-rw-rw-   0        0        0     3796 2024-02-19 09:13:27.000000 pyzjr-1.3.6/pyzjr/visualize/video_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr.egg-info/
--rw-rw-rw-   0        0        0     2931 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5988 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 07:32:59.000000 pyzjr-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     2207 2024-04-29 07:32:55.000000 pyzjr-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/
+-rw-rw-rw-   0        0        0     1075 2023-06-10 05:53:06.000000 pyzjr-1.3.7/LICENSE
+-rw-rw-rw-   0        0        0     2931 2024-04-29 07:56:56.000000 pyzjr-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2124 2024-01-25 07:09:34.000000 pyzjr-1.3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/models_img/
+-rw-rw-rw-   0        0        0        0 2024-03-04 11:15:31.000000 pyzjr-1.3.7/models_img/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/Math/
+-rw-rw-rw-   0        0        0      689 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Math/Numpy.py
+-rw-rw-rw-   0        0        0      212 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Math/__init__.py
+-rw-rw-rw-   0        0        0     3438 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Math/arithmetic.py
+-rw-rw-rw-   0        0        0      134 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Math/constant.py
+-rw-rw-rw-   0        0        0     7362 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Math/function.py
+-rw-rw-rw-   0        0        0    19620 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Math/point_line.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/Models/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/Models/Attention/
+-rw-rw-rw-   0        0        0     2271 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/A2.py
+-rw-rw-rw-   0        0        0     1927 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/AFT.py
+-rw-rw-rw-   0        0        0     1911 2024-04-29 07:40:57.000000 pyzjr-1.3.7/pyzjr/Models/Attention/DANet.py
+-rw-rw-rw-   0        0        0     5412 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/MobileViT.py
+-rw-rw-rw-   0        0        0     3105 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/SE.py
+-rw-rw-rw-   0        0        0     1933 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/ViP.py
+-rw-rw-rw-   0        0        0     1589 2024-04-29 07:40:19.000000 pyzjr-1.3.7/pyzjr/Models/Attention/__init__.py
+-rw-rw-rw-   0        0        0     4795 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/acmix.py
+-rw-rw-rw-   0        0        0    12705 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/axial.py
+-rw-rw-rw-   0        0        0     3180 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/bam.py
+-rw-rw-rw-   0        0        0     3729 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/cbam.py
+-rw-rw-rw-   0        0        0     1635 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/coord.py
+-rw-rw-rw-   0        0        0     2175 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/cot.py
+-rw-rw-rw-   0        0        0     2688 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/crisscross.py
+-rw-rw-rw-   0        0        0    26854 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/crossformer.py
+-rw-rw-rw-   0        0        0    23025 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/dat.py
+-rw-rw-rw-   0        0        0     1340 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/eca.py
+-rw-rw-rw-   0        0        0     3752 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/emsa.py
+-rw-rw-rw-   0        0        0     1341 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/external.py
+-rw-rw-rw-   0        0        0     4161 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/gfnet.py
+-rw-rw-rw-   0        0        0     5444 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/halo.py
+-rw-rw-rw-   0        0        0    30578 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/moat.py
+-rw-rw-rw-   0        0        0     3670 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/muse.py
+-rw-rw-rw-   0        0        0     2281 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/outlook.py
+-rw-rw-rw-   0        0        0      985 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/parnet.py
+-rw-rw-rw-   0        0        0     4087 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/polarized.py
+-rw-rw-rw-   0        0        0     2296 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/psa.py
+-rw-rw-rw-   0        0        0      930 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/residual.py
+-rw-rw-rw-   0        0        0     2355 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/s2.py
+-rw-rw-rw-   0        0        0     3084 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/self_att.py
+-rw-rw-rw-   0        0        0     1784 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/sge.py
+-rw-rw-rw-   0        0        0     2637 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/shuffle.py
+-rw-rw-rw-   0        0        0      909 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/simam.py
+-rw-rw-rw-   0        0        0     2933 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/simplified_self_att.py
+-rw-rw-rw-   0        0        0     1863 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/sk.py
+-rw-rw-rw-   0        0        0     2349 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/triplet.py
+-rw-rw-rw-   0        0        0     2234 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/Attention/ufo.py
+-rw-rw-rw-   0        0        0      220 2024-04-29 07:38:52.000000 pyzjr-1.3.7/pyzjr/Models/__init__.py
+-rw-rw-rw-   0        0        0     3384 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/Models/backbone/
+-rw-rw-rw-   0        0        0     5692 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/Darknet.py
+-rw-rw-rw-   0        0        0    25919 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/Ghostnet.py
+-rw-rw-rw-   0        0        0     1953 2024-04-29 07:42:05.000000 pyzjr-1.3.7/pyzjr/Models/backbone/__init__.py
+-rw-rw-rw-   0        0        0     1935 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/alexnet.py
+-rw-rw-rw-   0        0        0     7560 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/conv2former.py
+-rw-rw-rw-   0        0        0     6278 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/densenet.py
+-rw-rw-rw-   0        0        0    12866 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/drn.py
+-rw-rw-rw-   0        0        0    17934 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/efficientnet.py
+-rw-rw-rw-   0        0        0     7210 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/fasternet.py
+-rw-rw-rw-   0        0        0     5623 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/googlenet.py
+-rw-rw-rw-   0        0        0     1869 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/lenet.py
+-rw-rw-rw-   0        0        0     7048 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/mnasnet.py
+-rw-rw-rw-   0        0        0    16395 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/mobilenet.py
+-rw-rw-rw-   0        0        0     9972 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/nasnet.py
+-rw-rw-rw-   0        0        0     7217 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/regnet.py
+-rw-rw-rw-   0        0        0     8910 2024-04-29 07:41:16.000000 pyzjr-1.3.7/pyzjr/Models/backbone/resnet.py
+-rw-rw-rw-   0        0        0    11356 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/shufflenet.py
+-rw-rw-rw-   0        0        0     4392 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/squeezenet.py
+-rw-rw-rw-   0        0        0     3996 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/vgg.py
+-rw-rw-rw-   0        0        0     5866 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/xception.py
+-rw-rw-rw-   0        0        0     2705 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/backbone/zfnet.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/Models/bricks/
+-rw-rw-rw-   0        0        0     5577 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/bricks/Initer.py
+-rw-rw-rw-   0        0        0      426 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/bricks/__init__.py
+-rw-rw-rw-   0        0        0     1577 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/bricks/classfier.py
+-rw-rw-rw-   0        0        0    22575 2024-04-29 07:40:36.000000 pyzjr-1.3.7/pyzjr/Models/bricks/comblock.py
+-rw-rw-rw-   0        0        0     2646 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/bricks/conv_norm_act.py
+-rw-rw-rw-   0        0        0     6828 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/bricks/drop.py
+-rw-rw-rw-   0        0        0     6669 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/bricks/mlp.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/Models/conv/
+-rw-rw-rw-   0        0        0     1974 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/conv/Depthwise_Conv.py
+-rw-rw-rw-   0        0        0      508 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/conv/Dilated_Conv.py
+-rw-rw-rw-   0        0        0     1862 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/conv/Partial_Conv.py
+-rw-rw-rw-   0        0        0     2660 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/conv/Ref_Conv.py
+-rw-rw-rw-   0        0        0    11456 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/conv/Snake_Conv.py
+-rw-rw-rw-   0        0        0      295 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/conv/__init__.py
+-rw-rw-rw-   0        0        0     3029 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/networks.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/Models/sampling/
+-rw-rw-rw-   0        0        0      754 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/sampling/__init__.py
+-rw-rw-rw-   0        0        0     4857 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/sampling/adaptivepooling.py
+-rw-rw-rw-   0        0        0     1393 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/sampling/haarwavelet.py
+-rw-rw-rw-   0        0        0     1828 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/sampling/medianpooling.py
+-rw-rw-rw-   0        0        0     4792 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/sampling/standardpooling.py
+-rw-rw-rw-   0        0        0      854 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/sampling/strideconv.py
+-rw-rw-rw-   0        0        0     3692 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/sampling/strippooling.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/Models/segmentation/
+-rw-rw-rw-   0        0        0       70 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/segmentation/__init__.py
+-rw-rw-rw-   0        0        0    24988 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/segmentation/fcn.py
+-rw-rw-rw-   0        0        0     3289 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Models/segmentation/unet.py
+-rw-rw-rw-   0        0        0     6328 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/PIC.py
+-rw-rw-rw-   0        0        0    10349 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/Z.py
+-rw-rw-rw-   0        0        0      896 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/augmentation/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/augmentation/Pixel/
+-rw-rw-rw-   0        0        0    13180 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/Pixel/Crack.py
+-rw-rw-rw-   0        0        0     8307 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/Pixel/_Steger.py
+-rw-rw-rw-   0        0        0      366 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/Pixel/__init__.py
+-rw-rw-rw-   0        0        0     7681 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/Pixel/definition.py
+-rw-rw-rw-   0        0        0     4835 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/Pixel/pixel.py
+-rw-rw-rw-   0        0        0     1685 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/Pixel/utils.py
+-rw-rw-rw-   0        0        0      116 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/__init__.py
+-rw-rw-rw-   0        0        0    28649 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/augments.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/augmentation/transforms/
+-rw-rw-rw-   0        0        0      306 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2192 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/transforms/_utils.py
+-rw-rw-rw-   0        0        0     3413 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/transforms/normal.py
+-rw-rw-rw-   0        0        0    10459 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/transforms/opencv.py
+-rw-rw-rw-   0        0        0    40685 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/transforms/pillow.py
+-rw-rw-rw-   0        0        0     6139 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/transforms/tvision.py
+-rw-rw-rw-   0        0        0     1084 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/augmentation/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/core/
+-rw-rw-rw-   0        0        0     1136 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/core/__init__.py
+-rw-rw-rw-   0        0        0     6991 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/core/__tensor.py
+-rw-rw-rw-   0        0        0      680 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/core/_utils.py
+-rw-rw-rw-   0        0        0      982 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/core/decorator.py
+-rw-rw-rw-   0        0        0     2123 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/core/error.py
+-rw-rw-rw-   0        0        0     2692 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/core/general.py
+-rw-rw-rw-   0        0        0      671 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/core/helpers.py
+-rw-rw-rw-   0        0        0     7254 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/core/lr_scheduler.py
+-rw-rw-rw-   0        0        0    15534 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/core/utils_pytorch_numpy_unification.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/data/
+-rw-rw-rw-   0        0        0     1486 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/data/Dataloader.py
+-rw-rw-rw-   0        0        0     9590 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/data/Dataset.py
+-rw-rw-rw-   0        0        0    12147 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/data/FM.py
+-rw-rw-rw-   0        0        0      215 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/data/__init__.py
+-rw-rw-rw-   0        0        0     4064 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/data/basedataset.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/data/data_set/
+-rw-rw-rw-   0        0        0     9436 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/data/data_set/Pascal_voc.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/data/data_set/__init__.py
+-rw-rw-rw-   0        0        0     1313 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/data/data_set/config.py
+-rw-rw-rw-   0        0        0    15340 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/data/reader.py
+-rw-rw-rw-   0        0        0      934 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/data/txt_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/devices/
+-rw-rw-rw-   0        0        0      523 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/devices/__init__.py
+-rw-rw-rw-   0        0        0     1572 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/devices/get_device.py
+-rw-rw-rw-   0        0        0     3032 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/devices/measures.py
+-rw-rw-rw-   0        0        0     1202 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/devices/systeminfo.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/dlearn/
+-rw-rw-rw-   0        0        0      949 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/dlearn/__init__.py
+-rw-rw-rw-   0        0        0     8571 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/dlearn/callbacklog.py
+-rw-rw-rw-   0        0        0     8379 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/dlearn/callbacks.py
+-rw-rw-rw-   0        0        0     1051 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/dlearn/savemodels.py
+-rw-rw-rw-   0        0        0     5603 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/dlearn/strategy.py
+-rw-rw-rw-   0        0        0     5955 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/dlearn/tools.py
+-rw-rw-rw-   0        0        0     7356 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/dlearn/trainer.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/nn/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/nn/Metrics/
+-rw-rw-rw-   0        0        0      768 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/Metrics/__init__.py
+-rw-rw-rw-   0        0        0    16268 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/Metrics/classification.py
+-rw-rw-rw-   0        0        0     3822 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/Metrics/indexutils.py
+-rw-rw-rw-   0        0        0     9779 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/Metrics/medical_index.py
+-rw-rw-rw-   0        0        0     5837 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/Metrics/segment3d.py
+-rw-rw-rw-   0        0        0    11847 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/Metrics/semantic.py
+-rw-rw-rw-   0        0        0     9459 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/Summary.py
+-rw-rw-rw-   0        0        0      123 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/__init__.py
+-rw-rw-rw-   0        0        0    84332 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/functional.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/nn/torchutils/
+-rw-rw-rw-   0        0        0     3262 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/torchutils/OneHot.py
+-rw-rw-rw-   0        0        0      835 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/torchutils/__init__.py
+-rw-rw-rw-   0        0        0     7197 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/torchutils/avgweight.py
+-rw-rw-rw-   0        0        0    15225 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/torchutils/learnrate.py
+-rw-rw-rw-   0        0        0    27275 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/torchutils/loss_function.py
+-rw-rw-rw-   0        0        0     5217 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/nn/torchutils/loss_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/torch3D/
+-rw-rw-rw-   0        0        0       57 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/torch3D/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/torch3D/networks/
+-rw-rw-rw-   0        0        0      266 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/torch3D/networks/__init__.py
+-rw-rw-rw-   0        0        0     6344 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/torch3D/networks/basic_unet.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/torch3D/networks/block/
+-rw-rw-rw-   0        0        0    22077 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/torch3D/networks/block/DSConv.py
+-rw-rw-rw-   0        0        0       28 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/torch3D/networks/block/__init__.py
+-rw-rw-rw-   0        0        0     7862 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/torch3D/networks/dscnet.py
+-rw-rw-rw-   0        0        0     5755 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/torch3D/networks/vent.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/torch3D/nii/
+-rw-rw-rw-   0        0        0      306 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/torch3D/nii/__init__.py
+-rw-rw-rw-   0        0        0     4420 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/torch3D/nii/mri.py
+-rw-rw-rw-   0        0        0     4363 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/torch3D/nii/nifti_dataset.py
+-rw-rw-rw-   0        0        0     3373 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/torch3D/nii/nii_utils.py
+-rw-rw-rw-   0        0        0       21 2024-04-29 07:56:40.000000 pyzjr-1.3.7/pyzjr/version.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/visualize/
+-rw-rw-rw-   0        0        0      410 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/visualize/color/
+-rw-rw-rw-   0        0        0     1418 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/color/__init__.py
+-rw-rw-rw-   0        0        0     4848 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/color/colormap.py
+-rw-rw-rw-   0        0        0     3339 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/color/colorspace.py
+-rw-rw-rw-   0        0        0     7471 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/color/cvplot.py
+-rw-rw-rw-   0        0        0     7937 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/color/findcolor.py
+-rw-rw-rw-   0        0        0     1066 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/color/hex.py
+-rw-rw-rw-   0        0        0    10972 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/io.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr/visualize/mediapipe/
+-rw-rw-rw-   0        0        0     6556 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/mediapipe/HandTrack.py
+-rw-rw-rw-   0        0        0      376 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/mediapipe/__init__.py
+-rw-rw-rw-   0        0        0      631 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/mediapipe/const.py
+-rw-rw-rw-   0        0        0     4327 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/printf.py
+-rw-rw-rw-   0        0        0     3367 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/utils.py
+-rw-rw-rw-   0        0        0     3796 2024-04-29 07:37:02.000000 pyzjr-1.3.7/pyzjr/visualize/video_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr.egg-info/
+-rw-rw-rw-   0        0        0     2931 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7154 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-29 07:56:56.000000 pyzjr-1.3.7/pyzjr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 07:56:56.000000 pyzjr-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     2207 2024-04-29 07:56:40.000000 pyzjr-1.3.7/setup.py
```

### Comparing `pyzjr-1.3.6/LICENSE` & `pyzjr-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/PKG-INFO` & `pyzjr-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.3.6
+Version: 1.3.7
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Keywords: python,computer vision,pyzjr,windows
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pyzjr-1.3.6/README.md` & `pyzjr-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Math/Numpy.py` & `pyzjr-1.3.7/pyzjr/Math/Numpy.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Math/arithmetic.py` & `pyzjr-1.3.7/pyzjr/Math/arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Math/function.py` & `pyzjr-1.3.7/pyzjr/Math/function.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Math/point_line.py` & `pyzjr-1.3.7/pyzjr/Math/point_line.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/A2.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/A2.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/AFT.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/AFT.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/DANet.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/DANet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import torch
 from torch import nn
-from pyzjr.Models.attention.self_att import ScaledDotProductAttention
-from pyzjr.Models.attention.simplified_self_att import SimplifiedScaledDotProductAttention
+from pyzjr.Models.Attention.self_att import ScaledDotProductAttention
+from pyzjr.Models.Attention.simplified_self_att import SimplifiedScaledDotProductAttention
 
 class PositionAttentionModule(nn.Module):
 
     def __init__(self,d_model=512,kernel_size=3, H=7, W=7):
         super().__init__()
         self.cnn=nn.Conv2d(d_model,d_model,kernel_size=kernel_size,padding=(kernel_size-1)//2)
         self.pa=ScaledDotProductAttention(d_model,d_k=d_model,d_v=d_model,h=1)
```

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/MobileViT.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/MobileViT.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/SE.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/SE.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/ViP.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/ViP.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/__init__.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .A2 import DoubleAttention
 from .bam import BAMAttention
 from .cbam import CBAMAttention, LightCBAMAttention
-from .se import SEAttention, EffectiveSEAttention, SqueezeExcitation
+from .SE import SEAttention, EffectiveSEAttention, SqueezeExcitation
 from .ufo import UFOAttention
 from .cot import CoTAttention
 
 # __all__ = ["BAMAttention", "SEAttention", "SqueezeExcitation", "EffectiveSEAttention",
 #            "CBAMAttention", "LightCBAMAttention", "DoubleAttention", "UFOAttention",
 #            "CoTAttention"]
```

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/acmix.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/acmix.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/axial.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/axial.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/bam.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/bam.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/cbam.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/cbam.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/coord.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/coord.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/cot.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/cot.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/crisscross.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/crisscross.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/crossformer.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/crossformer.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/dat.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/dat.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/eca.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/eca.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/emsa.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/emsa.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/external.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/external.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/gfnet.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/gfnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/halo.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/halo.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/moat.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/moat.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/muse.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/muse.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/outlook.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/outlook.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/parnet.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/parnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/polarized.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/polarized.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/psa.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/psa.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/residual.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/residual.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/s2.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/s2.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/self_att.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/self_att.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/sge.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/sge.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/shuffle.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/shuffle.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/simam.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/simam.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/simplified_self_att.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/simplified_self_att.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/sk.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/sk.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/triplet.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/triplet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/Attention/ufo.py` & `pyzjr-1.3.7/pyzjr/Models/Attention/ufo.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/_utils.py` & `pyzjr-1.3.7/pyzjr/Models/_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/Darknet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/Darknet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/Ghostnet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/Ghostnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/__init__.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 # 2010s
 from .alexnet import AlexNet
 from .zfnet import ZFNet
 from .vgg import VGG, vgg11_bn, vgg13_bn, vgg16_bn, vgg19_bn
 from .googlenet import GoogLeNet
 from .resnet import ResNet, resnet18, resnet34, resnet50, resnet101, resnet152
 from .squeezenet import SqueezeNet, squeezenet1_0, squeezenet1_1
-from .darknet import darknet19, darknet53
+from .Darknet import darknet19, darknet53
 from .mobilenet import MobileNetV1, MobileNetV2, MobileNetV3, MobileNetV3_Large, MobileNetV3_Small
 from .densenet import DenseNet, densenet121, densenet161, densenet169, densenet201
 from .mnasnet import MNASNet, mnasnet0_5, mnasnet0_75, mnasnet1_0, mnasnet1_3
 from .shufflenet import ShuffleNetV1, ShuffleNetV2, shufflenet_v1_g1, shufflenet_v1_g2, \
     shufflenet_v1_g3, shufflenet_v1_g4, shufflenet_v1_g8, shufflenet_v2_x0_5, shufflenet_v2_x1_0, \
     shufflenet_v2_x1_5, shufflenet_v2_x2_0
 from .xception import Xception
 from .drn import DRN, DRN_A, drn_a_50, drn_c_26, drn_c_42, drn_c_58, drn_d_22, drn_d_24, drn_d_38, \
     drn_d_40, drn_d_54, drn_d_56, drn_d_105, drn_d_107
 
 # 2020s
 from .conv2former import Conv2Former_n, Conv2Former_t, Conv2Former_s, Conv2Former_l, Conv2Former_b
-from .ghostnet import GhostNet, GGhostRegNet, ghostnetv1, ghostnetv2, g_ghost_regnetx_002, \
+from .Ghostnet import GhostNet, GGhostRegNet, ghostnetv1, ghostnetv2, g_ghost_regnetx_002, \
     g_ghost_regnetx_004, g_ghost_regnetx_006, g_ghost_regnetx_008, g_ghost_regnetx_016, \
     g_ghost_regnetx_032, g_ghost_regnetx_040, g_ghost_regnetx_064, g_ghost_regnetx_080, \
     g_ghost_regnetx_120, g_ghost_regnetx_160, g_ghost_regnetx_320
 from .regnet import regnetx_002, regnetx_004, regnetx_006, regnetx_008, regnetx_016, regnetx_032,\
     regnetx_040, regnetx_064, regnetx_080, regnetx_120, regnetx_160, regnetx_320
 from .fasternet import fasternet_t0, fasternet_t1, fasternet_t2, fasternet_s, \
     fasternet_m, fasternet_l
```

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/alexnet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/alexnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/conv2former.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/conv2former.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/densenet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/densenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/drn.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/drn.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/efficientnet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/efficientnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/fasternet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/fasternet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/googlenet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/googlenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/lenet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/lenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/mnasnet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/mnasnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/mobilenet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/mobilenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/nasnet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/nasnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/regnet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/resnet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/resnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 resnet18, resnet34, resnet50, resnet101, resnet152
 (Optional addition of SE module)
 
 Blog records: https://blog.csdn.net/m0_62919535/article/details/132384303
 """
 import torch
 import torch.nn as nn
-from pyzjr.Models.attention import SEAttention
+from pyzjr.Models.Attention import SEAttention
 from pyzjr.Models.bricks import ConvBnReLU, ConvBn
 
 __all__ = ["ResNet", 'resnet18', 'resnet34', 'resnet50', 'resnet101', 'resnet152']
 
 def conv3x3(in_channels, out_channels, stride=1, groups=1, dilation=1):
     """3x3 convolution with padding:捕捉局部特征和空间相关性，学习更复杂的特征和抽象表示"""
     return nn.Conv2d(in_channels, out_channels, kernel_size=3, stride=stride,
```

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/shufflenet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/shufflenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/squeezenet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/squeezenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/vgg.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/vgg.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/xception.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/xception.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/backbone/zfnet.py` & `pyzjr-1.3.7/pyzjr/Models/backbone/zfnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/bricks/Initer.py` & `pyzjr-1.3.7/pyzjr/Models/bricks/Initer.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/bricks/classfier.py` & `pyzjr-1.3.7/pyzjr/Models/bricks/classfier.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/bricks/comblock.py` & `pyzjr-1.3.7/pyzjr/Models/bricks/comblock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Time: 2024-01-28 0:59
 """
 import torch
 import math
 import torch.nn as nn
 import torch.nn.functional as F
-from pyzjr.Models.attention import BAMAttention, SEAttention
+from pyzjr.Models.Attention import BAMAttention, SEAttention
 
 def conv3x3(in_channels, out_channels, stride=1, groups=1, dilation=1):
     """3x3 convolution with padding:捕捉局部特征和空间相关性，学习更复杂的特征和抽象表示"""
     return nn.Conv2d(in_channels, out_channels, kernel_size=3, stride=stride,
                      padding=dilation, groups=groups, bias=False, dilation=dilation)
 
 def conv1x1(in_channels, out_channels, stride=1):
```

### Comparing `pyzjr-1.3.6/pyzjr/Models/bricks/conv_norm_act.py` & `pyzjr-1.3.7/pyzjr/Models/bricks/conv_norm_act.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/bricks/drop.py` & `pyzjr-1.3.7/pyzjr/Models/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/bricks/mlp.py` & `pyzjr-1.3.7/pyzjr/Models/bricks/mlp.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/conv/Depthwise_Conv.py` & `pyzjr-1.3.7/pyzjr/Models/conv/Depthwise_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/conv/Partial_Conv.py` & `pyzjr-1.3.7/pyzjr/Models/conv/Partial_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/conv/Ref_Conv.py` & `pyzjr-1.3.7/pyzjr/Models/conv/Ref_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/conv/Snake_Conv.py` & `pyzjr-1.3.7/pyzjr/Models/conv/Snake_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/networks.py` & `pyzjr-1.3.7/pyzjr/Models/networks.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/sampling/__init__.py` & `pyzjr-1.3.7/pyzjr/Models/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/sampling/adaptivepooling.py` & `pyzjr-1.3.7/pyzjr/Models/sampling/adaptivepooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/sampling/haarwavelet.py` & `pyzjr-1.3.7/pyzjr/Models/sampling/haarwavelet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/sampling/medianpooling.py` & `pyzjr-1.3.7/pyzjr/Models/sampling/medianpooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/sampling/standardpooling.py` & `pyzjr-1.3.7/pyzjr/Models/sampling/standardpooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/sampling/strideconv.py` & `pyzjr-1.3.7/pyzjr/Models/sampling/strideconv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/sampling/strippooling.py` & `pyzjr-1.3.7/pyzjr/Models/sampling/strippooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/segmentation/fcn.py` & `pyzjr-1.3.7/pyzjr/Models/segmentation/fcn.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Models/segmentation/unet.py` & `pyzjr-1.3.7/pyzjr/Models/segmentation/unet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/PIC.py` & `pyzjr-1.3.7/pyzjr/PIC.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/Z.py` & `pyzjr-1.3.7/pyzjr/Z.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/__init__.py` & `pyzjr-1.3.7/pyzjr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/augmentation/Pixel/Crack.py` & `pyzjr-1.3.7/pyzjr/augmentation/Pixel/Crack.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/augmentation/Pixel/_Steger.py` & `pyzjr-1.3.7/pyzjr/augmentation/Pixel/_Steger.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/augmentation/Pixel/definition.py` & `pyzjr-1.3.7/pyzjr/augmentation/Pixel/definition.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/augmentation/Pixel/pixel.py` & `pyzjr-1.3.7/pyzjr/augmentation/Pixel/pixel.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/augmentation/Pixel/utils.py` & `pyzjr-1.3.7/pyzjr/augmentation/Pixel/utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/augmentation/augments.py` & `pyzjr-1.3.7/pyzjr/augmentation/augments.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/augmentation/transforms/_utils.py` & `pyzjr-1.3.7/pyzjr/augmentation/transforms/_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/augmentation/transforms/normal.py` & `pyzjr-1.3.7/pyzjr/augmentation/transforms/normal.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/augmentation/transforms/opencv.py` & `pyzjr-1.3.7/pyzjr/augmentation/transforms/opencv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/augmentation/transforms/pillow.py` & `pyzjr-1.3.7/pyzjr/augmentation/transforms/pillow.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/augmentation/transforms/tvision.py` & `pyzjr-1.3.7/pyzjr/augmentation/transforms/tvision.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/augmentation/utils.py` & `pyzjr-1.3.7/pyzjr/augmentation/utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/core/__init__.py` & `pyzjr-1.3.7/pyzjr/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/core/__tensor.py` & `pyzjr-1.3.7/pyzjr/core/__tensor.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/core/_utils.py` & `pyzjr-1.3.7/pyzjr/core/_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/core/decorator.py` & `pyzjr-1.3.7/pyzjr/core/decorator.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/core/error.py` & `pyzjr-1.3.7/pyzjr/core/error.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/core/general.py` & `pyzjr-1.3.7/pyzjr/core/general.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/core/helpers.py` & `pyzjr-1.3.7/pyzjr/core/helpers.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/core/lr_scheduler.py` & `pyzjr-1.3.7/pyzjr/core/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/core/utils_pytorch_numpy_unification.py` & `pyzjr-1.3.7/pyzjr/core/utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/data/Dataloader.py` & `pyzjr-1.3.7/pyzjr/data/Dataloader.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/data/Dataset.py` & `pyzjr-1.3.7/pyzjr/data/Dataset.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/data/FM.py` & `pyzjr-1.3.7/pyzjr/data/FM.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/data/basedataset.py` & `pyzjr-1.3.7/pyzjr/data/basedataset.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/data/data_set/Pascal_voc.py` & `pyzjr-1.3.7/pyzjr/data/data_set/Pascal_voc.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/data/data_set/config.py` & `pyzjr-1.3.7/pyzjr/data/data_set/config.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/data/reader.py` & `pyzjr-1.3.7/pyzjr/data/reader.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/data/txt_utils.py` & `pyzjr-1.3.7/pyzjr/data/txt_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/devices/__init__.py` & `pyzjr-1.3.7/pyzjr/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/devices/get_device.py` & `pyzjr-1.3.7/pyzjr/devices/get_device.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/devices/measures.py` & `pyzjr-1.3.7/pyzjr/devices/measures.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/devices/systeminfo.py` & `pyzjr-1.3.7/pyzjr/devices/systeminfo.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/dlearn/__init__.py` & `pyzjr-1.3.7/pyzjr/dlearn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/dlearn/callbacklog.py` & `pyzjr-1.3.7/pyzjr/dlearn/callbacklog.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/dlearn/callbacks.py` & `pyzjr-1.3.7/pyzjr/dlearn/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/dlearn/savemodels.py` & `pyzjr-1.3.7/pyzjr/dlearn/savemodels.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/dlearn/strategy.py` & `pyzjr-1.3.7/pyzjr/dlearn/strategy.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/dlearn/tools.py` & `pyzjr-1.3.7/pyzjr/dlearn/tools.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/dlearn/trainer.py` & `pyzjr-1.3.7/pyzjr/dlearn/trainer.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/Metrics/__init__.py` & `pyzjr-1.3.7/pyzjr/nn/Metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/Metrics/classification.py` & `pyzjr-1.3.7/pyzjr/nn/Metrics/classification.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/Metrics/indexutils.py` & `pyzjr-1.3.7/pyzjr/nn/Metrics/indexutils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/Metrics/medical_index.py` & `pyzjr-1.3.7/pyzjr/nn/Metrics/medical_index.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/Metrics/segment3d.py` & `pyzjr-1.3.7/pyzjr/nn/Metrics/segment3d.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/Metrics/semantic.py` & `pyzjr-1.3.7/pyzjr/nn/Metrics/semantic.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/Summary.py` & `pyzjr-1.3.7/pyzjr/nn/Summary.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/functional.py` & `pyzjr-1.3.7/pyzjr/nn/functional.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/torchutils/OneHot.py` & `pyzjr-1.3.7/pyzjr/nn/torchutils/OneHot.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/torchutils/__init__.py` & `pyzjr-1.3.7/pyzjr/nn/torchutils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/torchutils/avgweight.py` & `pyzjr-1.3.7/pyzjr/nn/torchutils/avgweight.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/torchutils/learnrate.py` & `pyzjr-1.3.7/pyzjr/nn/torchutils/learnrate.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/torchutils/loss_function.py` & `pyzjr-1.3.7/pyzjr/nn/torchutils/loss_function.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/nn/torchutils/loss_utils.py` & `pyzjr-1.3.7/pyzjr/nn/torchutils/loss_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/torch3D/networks/basic_unet.py` & `pyzjr-1.3.7/pyzjr/torch3D/networks/basic_unet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/torch3D/networks/block/DSConv.py` & `pyzjr-1.3.7/pyzjr/torch3D/networks/block/DSConv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/torch3D/networks/dscnet.py` & `pyzjr-1.3.7/pyzjr/torch3D/networks/dscnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/torch3D/networks/vent.py` & `pyzjr-1.3.7/pyzjr/torch3D/networks/vent.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/torch3D/nii/mri.py` & `pyzjr-1.3.7/pyzjr/torch3D/nii/mri.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/torch3D/nii/nifti_dataset.py` & `pyzjr-1.3.7/pyzjr/torch3D/nii/nifti_dataset.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/torch3D/nii/nii_utils.py` & `pyzjr-1.3.7/pyzjr/torch3D/nii/nii_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/visualize/color/__init__.py` & `pyzjr-1.3.7/pyzjr/visualize/color/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/visualize/color/colormap.py` & `pyzjr-1.3.7/pyzjr/visualize/color/colormap.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/visualize/color/colorspace.py` & `pyzjr-1.3.7/pyzjr/visualize/color/colorspace.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/visualize/color/cvplot.py` & `pyzjr-1.3.7/pyzjr/visualize/color/cvplot.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/visualize/color/findcolor.py` & `pyzjr-1.3.7/pyzjr/visualize/color/findcolor.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/visualize/color/hex.py` & `pyzjr-1.3.7/pyzjr/visualize/color/hex.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/visualize/io.py` & `pyzjr-1.3.7/pyzjr/visualize/io.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/visualize/mediapipe/HandTrack.py` & `pyzjr-1.3.7/pyzjr/visualize/mediapipe/HandTrack.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/visualize/mediapipe/const.py` & `pyzjr-1.3.7/pyzjr/visualize/mediapipe/const.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/visualize/printf.py` & `pyzjr-1.3.7/pyzjr/visualize/printf.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/visualize/utils.py` & `pyzjr-1.3.7/pyzjr/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr/visualize/video_utils.py` & `pyzjr-1.3.7/pyzjr/visualize/video_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.6/pyzjr.egg-info/PKG-INFO` & `pyzjr-1.3.7/pyzjr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.3.6
+Version: 1.3.7
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Keywords: python,computer vision,pyzjr,windows
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pyzjr-1.3.6/setup.py` & `pyzjr-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # from pyzjr.version import __version__
-VERSION = "1.3.6"
+VERSION = "1.3.7"
 DESCRIPTION = ' A computer vision library that supports Win, packaged with patches for visual libraries such as \
                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui) \
                 engineering code experience. '
 LONG_DESCRIPTION = 'pyzjr is a computer vision library that supports Win'
 
 setup(
     name="pyzjr",
```

