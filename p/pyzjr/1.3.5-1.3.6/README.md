# Comparing `tmp/pyzjr-1.3.5.tar.gz` & `tmp/pyzjr-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyzjr-1.3.5.tar", last modified: Sat Apr 20 07:27:26 2024, max compression
+gzip compressed data, was "dist\pyzjr-1.3.6.tar", last modified: Mon Apr 29 07:32:59 2024, max compression
```

## Comparing `pyzjr-1.3.5.tar` & `pyzjr-1.3.6.tar`

### file list

```diff
@@ -1,204 +1,220 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/
--rw-rw-rw-   0        0        0     1075 2023-06-10 05:53:06.000000 pyzjr-1.3.5/LICENSE
--rw-rw-rw-   0        0        0     2931 2024-04-20 07:27:26.000000 pyzjr-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     2124 2024-01-25 07:09:34.000000 pyzjr-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/models_img/
--rw-rw-rw-   0        0        0        0 2024-03-04 11:15:31.000000 pyzjr-1.3.5/models_img/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Math/
--rw-rw-rw-   0        0        0      689 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/Math/Numpy.py
--rw-rw-rw-   0        0        0      212 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/Math/__init__.py
--rw-rw-rw-   0        0        0     3438 2024-02-20 09:48:40.000000 pyzjr-1.3.5/pyzjr/Math/arithmetic.py
--rw-rw-rw-   0        0        0      134 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/Math/constant.py
--rw-rw-rw-   0        0        0     7362 2024-02-19 10:31:56.000000 pyzjr-1.3.5/pyzjr/Math/function.py
--rw-rw-rw-   0        0        0    19620 2024-02-19 09:52:53.000000 pyzjr-1.3.5/pyzjr/Math/point_line.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/Attention/
--rw-rw-rw-   0        0        0     2271 2024-03-04 07:16:29.000000 pyzjr-1.3.5/pyzjr/Models/Attention/A2.py
--rw-rw-rw-   0        0        0     1927 2024-03-09 14:59:27.000000 pyzjr-1.3.5/pyzjr/Models/Attention/AFT.py
--rw-rw-rw-   0        0        0     1911 2024-03-09 15:28:12.000000 pyzjr-1.3.5/pyzjr/Models/Attention/DANet.py
--rw-rw-rw-   0        0        0     5412 2024-03-09 15:10:59.000000 pyzjr-1.3.5/pyzjr/Models/Attention/MobileViT.py
--rw-rw-rw-   0        0        0     3105 2024-03-21 17:03:45.000000 pyzjr-1.3.5/pyzjr/Models/Attention/SE.py
--rw-rw-rw-   0        0        0     1933 2024-03-09 15:18:47.000000 pyzjr-1.3.5/pyzjr/Models/Attention/ViP.py
--rw-rw-rw-   0        0        0     1589 2024-04-20 07:26:32.000000 pyzjr-1.3.5/pyzjr/Models/Attention/__init__.py
--rw-rw-rw-   0        0        0     4795 2024-03-09 14:59:04.000000 pyzjr-1.3.5/pyzjr/Models/Attention/acmix.py
--rw-rw-rw-   0        0        0    12705 2024-03-09 15:00:08.000000 pyzjr-1.3.5/pyzjr/Models/Attention/axial.py
--rw-rw-rw-   0        0        0     3180 2024-03-04 07:32:10.000000 pyzjr-1.3.5/pyzjr/Models/Attention/bam.py
--rw-rw-rw-   0        0        0     3729 2024-03-04 12:35:57.000000 pyzjr-1.3.5/pyzjr/Models/Attention/cbam.py
--rw-rw-rw-   0        0        0     1635 2024-03-09 15:01:57.000000 pyzjr-1.3.5/pyzjr/Models/Attention/coord.py
--rw-rw-rw-   0        0        0     2175 2024-03-04 12:19:45.000000 pyzjr-1.3.5/pyzjr/Models/Attention/cot.py
--rw-rw-rw-   0        0        0     2688 2024-03-09 15:02:25.000000 pyzjr-1.3.5/pyzjr/Models/Attention/crisscross.py
--rw-rw-rw-   0        0        0    26854 2024-03-09 15:22:58.000000 pyzjr-1.3.5/pyzjr/Models/Attention/crossformer.py
--rw-rw-rw-   0        0        0    23025 2024-03-09 15:25:56.000000 pyzjr-1.3.5/pyzjr/Models/Attention/dat.py
--rw-rw-rw-   0        0        0     1340 2024-03-09 15:04:58.000000 pyzjr-1.3.5/pyzjr/Models/Attention/eca.py
--rw-rw-rw-   0        0        0     3752 2024-03-09 15:05:31.000000 pyzjr-1.3.5/pyzjr/Models/Attention/emsa.py
--rw-rw-rw-   0        0        0     1341 2024-03-09 15:06:14.000000 pyzjr-1.3.5/pyzjr/Models/Attention/external.py
--rw-rw-rw-   0        0        0     4161 2024-03-09 15:19:38.000000 pyzjr-1.3.5/pyzjr/Models/Attention/gfnet.py
--rw-rw-rw-   0        0        0     5444 2024-03-09 15:07:26.000000 pyzjr-1.3.5/pyzjr/Models/Attention/halo.py
--rw-rw-rw-   0        0        0    30578 2024-03-09 15:23:53.000000 pyzjr-1.3.5/pyzjr/Models/Attention/moat.py
--rw-rw-rw-   0        0        0     3670 2024-03-09 15:08:27.000000 pyzjr-1.3.5/pyzjr/Models/Attention/muse.py
--rw-rw-rw-   0        0        0     2281 2024-03-09 15:11:27.000000 pyzjr-1.3.5/pyzjr/Models/Attention/outlook.py
--rw-rw-rw-   0        0        0      985 2024-03-09 15:29:37.000000 pyzjr-1.3.5/pyzjr/Models/Attention/parnet.py
--rw-rw-rw-   0        0        0     4087 2024-03-09 15:13:38.000000 pyzjr-1.3.5/pyzjr/Models/Attention/polarized.py
--rw-rw-rw-   0        0        0     2296 2024-03-09 15:11:51.000000 pyzjr-1.3.5/pyzjr/Models/Attention/psa.py
--rw-rw-rw-   0        0        0      930 2024-03-09 14:57:03.000000 pyzjr-1.3.5/pyzjr/Models/Attention/residual.py
--rw-rw-rw-   0        0        0     2355 2024-03-09 14:52:15.000000 pyzjr-1.3.5/pyzjr/Models/Attention/s2.py
--rw-rw-rw-   0        0        0     3084 2024-03-09 15:15:20.000000 pyzjr-1.3.5/pyzjr/Models/Attention/self_att.py
--rw-rw-rw-   0        0        0     1784 2024-03-09 15:14:10.000000 pyzjr-1.3.5/pyzjr/Models/Attention/sge.py
--rw-rw-rw-   0        0        0     2637 2024-03-09 15:16:05.000000 pyzjr-1.3.5/pyzjr/Models/Attention/shuffle.py
--rw-rw-rw-   0        0        0      909 2024-03-09 15:16:39.000000 pyzjr-1.3.5/pyzjr/Models/Attention/simam.py
--rw-rw-rw-   0        0        0     2933 2024-03-09 15:17:26.000000 pyzjr-1.3.5/pyzjr/Models/Attention/simplified_self_att.py
--rw-rw-rw-   0        0        0     1863 2024-03-18 11:12:03.000000 pyzjr-1.3.5/pyzjr/Models/Attention/sk.py
--rw-rw-rw-   0        0        0     2349 2024-03-09 15:18:03.000000 pyzjr-1.3.5/pyzjr/Models/Attention/triplet.py
--rw-rw-rw-   0        0        0     2234 2024-03-04 13:24:57.000000 pyzjr-1.3.5/pyzjr/Models/Attention/ufo.py
--rw-rw-rw-   0        0        0      220 2024-03-16 15:32:39.000000 pyzjr-1.3.5/pyzjr/Models/__init__.py
--rw-rw-rw-   0        0        0     3384 2024-03-21 16:32:55.000000 pyzjr-1.3.5/pyzjr/Models/_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/backbone/
--rw-rw-rw-   0        0        0     5692 2024-03-22 16:07:30.000000 pyzjr-1.3.5/pyzjr/Models/backbone/Darknet.py
--rw-rw-rw-   0        0        0    25919 2024-02-23 14:10:01.000000 pyzjr-1.3.5/pyzjr/Models/backbone/Ghostnet.py
--rw-rw-rw-   0        0        0     1953 2024-03-26 15:38:25.000000 pyzjr-1.3.5/pyzjr/Models/backbone/__init__.py
--rw-rw-rw-   0        0        0     1935 2024-04-01 07:58:53.000000 pyzjr-1.3.5/pyzjr/Models/backbone/alexnet.py
--rw-rw-rw-   0        0        0     7560 2024-02-23 14:18:22.000000 pyzjr-1.3.5/pyzjr/Models/backbone/conv2former.py
--rw-rw-rw-   0        0        0     6278 2024-02-23 14:18:22.000000 pyzjr-1.3.5/pyzjr/Models/backbone/densenet.py
--rw-rw-rw-   0        0        0    12866 2024-04-01 09:42:37.000000 pyzjr-1.3.5/pyzjr/Models/backbone/drn.py
--rw-rw-rw-   0        0        0    17934 2024-04-01 08:53:51.000000 pyzjr-1.3.5/pyzjr/Models/backbone/efficientnet.py
--rw-rw-rw-   0        0        0     7210 2024-04-01 09:54:02.000000 pyzjr-1.3.5/pyzjr/Models/backbone/fasternet.py
--rw-rw-rw-   0        0        0     5623 2024-02-23 14:18:22.000000 pyzjr-1.3.5/pyzjr/Models/backbone/googlenet.py
--rw-rw-rw-   0        0        0     1869 2024-02-04 04:44:18.000000 pyzjr-1.3.5/pyzjr/Models/backbone/lenet.py
--rw-rw-rw-   0        0        0     7048 2024-03-18 16:29:49.000000 pyzjr-1.3.5/pyzjr/Models/backbone/mnasnet.py
--rw-rw-rw-   0        0        0    16395 2024-02-16 16:51:01.000000 pyzjr-1.3.5/pyzjr/Models/backbone/mobilenet.py
--rw-rw-rw-   0        0        0     9972 2024-04-18 15:14:36.000000 pyzjr-1.3.5/pyzjr/Models/backbone/nasnet.py
--rw-rw-rw-   0        0        0     7217 2024-03-18 11:17:15.000000 pyzjr-1.3.5/pyzjr/Models/backbone/regnet.py
--rw-rw-rw-   0        0        0     8910 2024-04-01 09:47:10.000000 pyzjr-1.3.5/pyzjr/Models/backbone/resnet.py
--rw-rw-rw-   0        0        0    11356 2024-03-22 15:56:05.000000 pyzjr-1.3.5/pyzjr/Models/backbone/shufflenet.py
--rw-rw-rw-   0        0        0     4392 2024-03-04 12:30:07.000000 pyzjr-1.3.5/pyzjr/Models/backbone/squeezenet.py
--rw-rw-rw-   0        0        0     3996 2024-02-25 16:22:54.000000 pyzjr-1.3.5/pyzjr/Models/backbone/vgg.py
--rw-rw-rw-   0        0        0     5866 2024-04-01 09:44:12.000000 pyzjr-1.3.5/pyzjr/Models/backbone/xception.py
--rw-rw-rw-   0        0        0     2705 2024-03-22 15:32:04.000000 pyzjr-1.3.5/pyzjr/Models/backbone/zfnet.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/bricks/
--rw-rw-rw-   0        0        0     5577 2024-04-01 09:57:01.000000 pyzjr-1.3.5/pyzjr/Models/bricks/Initer.py
--rw-rw-rw-   0        0        0      426 2024-04-18 15:04:29.000000 pyzjr-1.3.5/pyzjr/Models/bricks/__init__.py
--rw-rw-rw-   0        0        0     1577 2024-03-04 09:07:17.000000 pyzjr-1.3.5/pyzjr/Models/bricks/classfier.py
--rw-rw-rw-   0        0        0    22575 2024-03-04 07:32:10.000000 pyzjr-1.3.5/pyzjr/Models/bricks/comblock.py
--rw-rw-rw-   0        0        0     2646 2024-03-26 15:25:44.000000 pyzjr-1.3.5/pyzjr/Models/bricks/conv_norm_act.py
--rw-rw-rw-   0        0        0     6828 2024-03-04 12:40:27.000000 pyzjr-1.3.5/pyzjr/Models/bricks/drop.py
--rw-rw-rw-   0        0        0     6669 2024-03-06 00:10:20.000000 pyzjr-1.3.5/pyzjr/Models/bricks/mlp.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/conv/
--rw-rw-rw-   0        0        0     1974 2024-04-18 13:35:49.000000 pyzjr-1.3.5/pyzjr/Models/conv/Depthwise_Conv.py
--rw-rw-rw-   0        0        0      508 2024-03-21 15:46:28.000000 pyzjr-1.3.5/pyzjr/Models/conv/Dilated_Conv.py
--rw-rw-rw-   0        0        0     1862 2024-02-29 10:04:41.000000 pyzjr-1.3.5/pyzjr/Models/conv/Partial_Conv.py
--rw-rw-rw-   0        0        0     2660 2024-02-29 10:02:23.000000 pyzjr-1.3.5/pyzjr/Models/conv/Ref_Conv.py
--rw-rw-rw-   0        0        0    11458 2024-02-29 09:11:02.000000 pyzjr-1.3.5/pyzjr/Models/conv/Snake_Conv.py
--rw-rw-rw-   0        0        0      295 2024-03-21 15:46:28.000000 pyzjr-1.3.5/pyzjr/Models/conv/__init__.py
--rw-rw-rw-   0        0        0     3029 2024-04-14 00:39:15.000000 pyzjr-1.3.5/pyzjr/Models/networks.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/sampling/
--rw-rw-rw-   0        0        0      754 2024-04-05 14:24:23.000000 pyzjr-1.3.5/pyzjr/Models/sampling/__init__.py
--rw-rw-rw-   0        0        0     4857 2024-04-05 16:18:30.000000 pyzjr-1.3.5/pyzjr/Models/sampling/adaptivepooling.py
--rw-rw-rw-   0        0        0     1393 2024-01-27 17:10:24.000000 pyzjr-1.3.5/pyzjr/Models/sampling/haarwavelet.py
--rw-rw-rw-   0        0        0     1828 2024-03-04 13:56:06.000000 pyzjr-1.3.5/pyzjr/Models/sampling/medianpooling.py
--rw-rw-rw-   0        0        0     4792 2024-02-26 15:35:21.000000 pyzjr-1.3.5/pyzjr/Models/sampling/standardpooling.py
--rw-rw-rw-   0        0        0      854 2024-03-01 15:33:22.000000 pyzjr-1.3.5/pyzjr/Models/sampling/strideconv.py
--rw-rw-rw-   0        0        0     3692 2024-02-29 15:43:47.000000 pyzjr-1.3.5/pyzjr/Models/sampling/strippooling.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/Models/segmentation/
--rw-rw-rw-   0        0        0       70 2024-02-27 16:31:33.000000 pyzjr-1.3.5/pyzjr/Models/segmentation/__init__.py
--rw-rw-rw-   0        0        0    24988 2024-03-17 06:46:22.000000 pyzjr-1.3.5/pyzjr/Models/segmentation/fcn.py
--rw-rw-rw-   0        0        0     3289 2024-02-29 09:20:12.000000 pyzjr-1.3.5/pyzjr/Models/segmentation/unet.py
--rw-rw-rw-   0        0        0     6378 2024-04-14 00:39:15.000000 pyzjr-1.3.5/pyzjr/PIC.py
--rw-rw-rw-   0        0        0    10349 2024-02-04 05:11:03.000000 pyzjr-1.3.5/pyzjr/Z.py
--rw-rw-rw-   0        0        0      896 2024-04-14 00:39:15.000000 pyzjr-1.3.5/pyzjr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/augmentation/
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/
--rw-rw-rw-   0        0        0    13180 2024-04-13 15:26:35.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/Crack.py
--rw-rw-rw-   0        0        0     8307 2024-02-29 15:56:54.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/_Steger.py
--rw-rw-rw-   0        0        0      366 2024-02-19 10:23:26.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/__init__.py
--rw-rw-rw-   0        0        0     7681 2024-02-18 17:28:31.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/definition.py
--rw-rw-rw-   0        0        0     4827 2024-02-22 16:33:22.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/pixel.py
--rw-rw-rw-   0        0        0     1685 2024-04-13 15:00:07.000000 pyzjr-1.3.5/pyzjr/augmentation/Pixel/utils.py
--rw-rw-rw-   0        0        0      116 2024-04-13 14:32:14.000000 pyzjr-1.3.5/pyzjr/augmentation/__init__.py
--rw-rw-rw-   0        0        0    28643 2024-02-02 16:09:04.000000 pyzjr-1.3.5/pyzjr/augmentation/augments.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/
--rw-rw-rw-   0        0        0      306 2024-02-01 16:36:53.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/__init__.py
--rw-rw-rw-   0        0        0     2192 2024-02-02 16:09:04.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/_utils.py
--rw-rw-rw-   0        0        0     3413 2024-02-28 11:40:46.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/normal.py
--rw-rw-rw-   0        0        0    10459 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/opencv.py
--rw-rw-rw-   0        0        0    40632 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/pillow.py
--rw-rw-rw-   0        0        0     6139 2024-03-21 17:03:45.000000 pyzjr-1.3.5/pyzjr/augmentation/transforms/tvision.py
--rw-rw-rw-   0        0        0     1084 2024-03-04 06:15:09.000000 pyzjr-1.3.5/pyzjr/augmentation/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/core/
--rw-rw-rw-   0        0        0     1105 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/core/__init__.py
--rw-rw-rw-   0        0        0     6991 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/core/__tensor.py
--rw-rw-rw-   0        0        0      680 2023-10-07 12:04:40.000000 pyzjr-1.3.5/pyzjr/core/_utils.py
--rw-rw-rw-   0        0        0     1889 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/core/error.py
--rw-rw-rw-   0        0        0     2692 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/core/general.py
--rw-rw-rw-   0        0        0      669 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/core/helpers.py
--rw-rw-rw-   0        0        0     7254 2023-11-15 11:43:15.000000 pyzjr-1.3.5/pyzjr/core/lr_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/data/
--rw-rw-rw-   0        0        0     1486 2024-03-13 01:39:58.000000 pyzjr-1.3.5/pyzjr/data/Dataloader.py
--rw-rw-rw-   0        0        0     9590 2024-03-08 01:06:58.000000 pyzjr-1.3.5/pyzjr/data/Dataset.py
--rw-rw-rw-   0        0        0    12147 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/data/FM.py
--rw-rw-rw-   0        0        0      215 2024-04-14 15:31:09.000000 pyzjr-1.3.5/pyzjr/data/__init__.py
--rw-rw-rw-   0        0        0     4064 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/data/basedataset.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/data/data_set/
--rw-rw-rw-   0        0        0     9436 2024-03-13 01:39:58.000000 pyzjr-1.3.5/pyzjr/data/data_set/Pascal_voc.py
--rw-rw-rw-   0        0        0        0 2024-02-29 16:00:47.000000 pyzjr-1.3.5/pyzjr/data/data_set/__init__.py
--rw-rw-rw-   0        0        0     1313 2024-03-08 01:30:08.000000 pyzjr-1.3.5/pyzjr/data/data_set/config.py
--rw-rw-rw-   0        0        0    15340 2024-04-13 15:04:54.000000 pyzjr-1.3.5/pyzjr/data/reader.py
--rw-rw-rw-   0        0        0      934 2024-04-14 15:26:14.000000 pyzjr-1.3.5/pyzjr/data/txt_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/devices/
--rw-rw-rw-   0        0        0      498 2024-04-18 15:41:22.000000 pyzjr-1.3.5/pyzjr/devices/__init__.py
--rw-rw-rw-   0        0        0     1572 2024-04-13 15:22:13.000000 pyzjr-1.3.5/pyzjr/devices/get_device.py
--rw-rw-rw-   0        0        0     2888 2024-04-18 15:41:22.000000 pyzjr-1.3.5/pyzjr/devices/measures.py
--rw-rw-rw-   0        0        0     1202 2024-04-13 15:53:39.000000 pyzjr-1.3.5/pyzjr/devices/systeminfo.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/dlearn/
--rw-rw-rw-   0        0        0      949 2024-03-11 15:45:28.000000 pyzjr-1.3.5/pyzjr/dlearn/__init__.py
--rw-rw-rw-   0        0        0     8571 2024-02-17 18:07:27.000000 pyzjr-1.3.5/pyzjr/dlearn/callbacklog.py
--rw-rw-rw-   0        0        0     8379 2024-03-13 01:39:58.000000 pyzjr-1.3.5/pyzjr/dlearn/callbacks.py
--rw-rw-rw-   0        0        0     1051 2024-03-11 15:59:35.000000 pyzjr-1.3.5/pyzjr/dlearn/savemodels.py
--rw-rw-rw-   0        0        0     4801 2024-03-11 15:21:20.000000 pyzjr-1.3.5/pyzjr/dlearn/strategy.py
--rw-rw-rw-   0        0        0     5955 2024-04-13 15:28:23.000000 pyzjr-1.3.5/pyzjr/dlearn/tools.py
--rw-rw-rw-   0        0        0     7360 2024-03-11 16:12:42.000000 pyzjr-1.3.5/pyzjr/dlearn/trainer.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/nn/
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/nn/Metrics/
--rw-rw-rw-   0        0        0      385 2024-04-14 00:39:15.000000 pyzjr-1.3.5/pyzjr/nn/Metrics/__init__.py
--rw-rw-rw-   0        0        0    16237 2024-02-08 15:56:55.000000 pyzjr-1.3.5/pyzjr/nn/Metrics/classification.py
--rw-rw-rw-   0        0        0    11775 2024-03-17 07:10:00.000000 pyzjr-1.3.5/pyzjr/nn/Metrics/semantic.py
--rw-rw-rw-   0        0        0     9459 2024-04-18 15:17:33.000000 pyzjr-1.3.5/pyzjr/nn/Summary.py
--rw-rw-rw-   0        0        0      123 2024-04-18 15:17:33.000000 pyzjr-1.3.5/pyzjr/nn/__init__.py
--rw-rw-rw-   0        0        0    84332 2024-02-22 15:45:34.000000 pyzjr-1.3.5/pyzjr/nn/functional.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/
--rw-rw-rw-   0        0        0     2908 2024-03-04 07:50:15.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/OneHot.py
--rw-rw-rw-   0        0        0      183 2024-03-11 15:59:35.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/__init__.py
--rw-rw-rw-   0        0        0     7193 2024-03-04 07:50:15.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/avgweight.py
--rw-rw-rw-   0        0        0    15225 2024-02-20 09:56:56.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/learnrate.py
--rw-rw-rw-   0        0        0    13059 2024-02-26 16:29:06.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/loss_function.py
--rw-rw-rw-   0        0        0     3779 2024-01-28 10:43:32.000000 pyzjr-1.3.5/pyzjr/nn/torchutils/loss_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/torch3D/
--rw-rw-rw-   0        0        0        0 2024-04-14 00:38:41.000000 pyzjr-1.3.5/pyzjr/torch3D/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/torch3D/networks/
--rw-rw-rw-   0        0        0        0 2024-04-14 00:38:57.000000 pyzjr-1.3.5/pyzjr/torch3D/networks/__init__.py
--rw-rw-rw-   0        0        0       21 2024-04-20 07:26:32.000000 pyzjr-1.3.5/pyzjr/version.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/visualize/
--rw-rw-rw-   0        0        0      410 2024-04-14 15:13:36.000000 pyzjr-1.3.5/pyzjr/visualize/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/visualize/color/
--rw-rw-rw-   0        0        0     1418 2024-04-13 14:47:13.000000 pyzjr-1.3.5/pyzjr/visualize/color/__init__.py
--rw-rw-rw-   0        0        0     4848 2024-04-13 14:43:57.000000 pyzjr-1.3.5/pyzjr/visualize/color/colormap.py
--rw-rw-rw-   0        0        0     3339 2023-11-04 05:34:46.000000 pyzjr-1.3.5/pyzjr/visualize/color/colorspace.py
--rw-rw-rw-   0        0        0     7471 2024-04-13 14:47:13.000000 pyzjr-1.3.5/pyzjr/visualize/color/cvplot.py
--rw-rw-rw-   0        0        0     7937 2024-04-13 15:27:09.000000 pyzjr-1.3.5/pyzjr/visualize/color/findcolor.py
--rw-rw-rw-   0        0        0     1066 2024-02-13 17:07:55.000000 pyzjr-1.3.5/pyzjr/visualize/color/hex.py
--rw-rw-rw-   0        0        0    10985 2024-04-14 00:26:57.000000 pyzjr-1.3.5/pyzjr/visualize/io.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr/visualize/mediapipe/
--rw-rw-rw-   0        0        0     6556 2024-04-14 15:13:36.000000 pyzjr-1.3.5/pyzjr/visualize/mediapipe/HandTrack.py
--rw-rw-rw-   0        0        0      376 2024-01-25 07:15:10.000000 pyzjr-1.3.5/pyzjr/visualize/mediapipe/__init__.py
--rw-rw-rw-   0        0        0      631 2024-02-04 05:11:03.000000 pyzjr-1.3.5/pyzjr/visualize/mediapipe/const.py
--rw-rw-rw-   0        0        0     4327 2024-04-13 15:04:54.000000 pyzjr-1.3.5/pyzjr/visualize/printf.py
--rw-rw-rw-   0        0        0     3367 2024-02-22 15:48:11.000000 pyzjr-1.3.5/pyzjr/visualize/utils.py
--rw-rw-rw-   0        0        0     3796 2024-02-19 09:13:27.000000 pyzjr-1.3.5/pyzjr/visualize/video_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr.egg-info/
--rw-rw-rw-   0        0        0     2931 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5460 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-20 07:27:26.000000 pyzjr-1.3.5/pyzjr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 07:27:26.000000 pyzjr-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     2133 2024-04-20 07:27:04.000000 pyzjr-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/
+-rw-rw-rw-   0        0        0     1075 2023-06-10 05:53:06.000000 pyzjr-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0     2931 2024-04-29 07:32:59.000000 pyzjr-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2124 2024-01-25 07:09:34.000000 pyzjr-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/models_img/
+-rw-rw-rw-   0        0        0        0 2024-03-04 11:15:31.000000 pyzjr-1.3.6/models_img/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Math/
+-rw-rw-rw-   0        0        0      689 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/Math/Numpy.py
+-rw-rw-rw-   0        0        0      212 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/Math/__init__.py
+-rw-rw-rw-   0        0        0     3438 2024-02-20 09:48:40.000000 pyzjr-1.3.6/pyzjr/Math/arithmetic.py
+-rw-rw-rw-   0        0        0      134 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/Math/constant.py
+-rw-rw-rw-   0        0        0     7362 2024-02-19 10:31:56.000000 pyzjr-1.3.6/pyzjr/Math/function.py
+-rw-rw-rw-   0        0        0    19620 2024-02-19 09:52:53.000000 pyzjr-1.3.6/pyzjr/Math/point_line.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/Attention/
+-rw-rw-rw-   0        0        0     2271 2024-03-04 07:16:29.000000 pyzjr-1.3.6/pyzjr/Models/Attention/A2.py
+-rw-rw-rw-   0        0        0     1927 2024-03-09 14:59:27.000000 pyzjr-1.3.6/pyzjr/Models/Attention/AFT.py
+-rw-rw-rw-   0        0        0     1911 2024-03-09 15:28:12.000000 pyzjr-1.3.6/pyzjr/Models/Attention/DANet.py
+-rw-rw-rw-   0        0        0     5412 2024-03-09 15:10:59.000000 pyzjr-1.3.6/pyzjr/Models/Attention/MobileViT.py
+-rw-rw-rw-   0        0        0     3105 2024-03-21 17:03:45.000000 pyzjr-1.3.6/pyzjr/Models/Attention/SE.py
+-rw-rw-rw-   0        0        0     1933 2024-03-09 15:18:47.000000 pyzjr-1.3.6/pyzjr/Models/Attention/ViP.py
+-rw-rw-rw-   0        0        0     1589 2024-04-20 07:26:32.000000 pyzjr-1.3.6/pyzjr/Models/Attention/__init__.py
+-rw-rw-rw-   0        0        0     4795 2024-03-09 14:59:04.000000 pyzjr-1.3.6/pyzjr/Models/Attention/acmix.py
+-rw-rw-rw-   0        0        0    12705 2024-03-09 15:00:08.000000 pyzjr-1.3.6/pyzjr/Models/Attention/axial.py
+-rw-rw-rw-   0        0        0     3180 2024-03-04 07:32:10.000000 pyzjr-1.3.6/pyzjr/Models/Attention/bam.py
+-rw-rw-rw-   0        0        0     3729 2024-03-04 12:35:57.000000 pyzjr-1.3.6/pyzjr/Models/Attention/cbam.py
+-rw-rw-rw-   0        0        0     1635 2024-03-09 15:01:57.000000 pyzjr-1.3.6/pyzjr/Models/Attention/coord.py
+-rw-rw-rw-   0        0        0     2175 2024-03-04 12:19:45.000000 pyzjr-1.3.6/pyzjr/Models/Attention/cot.py
+-rw-rw-rw-   0        0        0     2688 2024-03-09 15:02:25.000000 pyzjr-1.3.6/pyzjr/Models/Attention/crisscross.py
+-rw-rw-rw-   0        0        0    26854 2024-03-09 15:22:58.000000 pyzjr-1.3.6/pyzjr/Models/Attention/crossformer.py
+-rw-rw-rw-   0        0        0    23025 2024-03-09 15:25:56.000000 pyzjr-1.3.6/pyzjr/Models/Attention/dat.py
+-rw-rw-rw-   0        0        0     1340 2024-03-09 15:04:58.000000 pyzjr-1.3.6/pyzjr/Models/Attention/eca.py
+-rw-rw-rw-   0        0        0     3752 2024-03-09 15:05:31.000000 pyzjr-1.3.6/pyzjr/Models/Attention/emsa.py
+-rw-rw-rw-   0        0        0     1341 2024-03-09 15:06:14.000000 pyzjr-1.3.6/pyzjr/Models/Attention/external.py
+-rw-rw-rw-   0        0        0     4161 2024-03-09 15:19:38.000000 pyzjr-1.3.6/pyzjr/Models/Attention/gfnet.py
+-rw-rw-rw-   0        0        0     5444 2024-03-09 15:07:26.000000 pyzjr-1.3.6/pyzjr/Models/Attention/halo.py
+-rw-rw-rw-   0        0        0    30578 2024-03-09 15:23:53.000000 pyzjr-1.3.6/pyzjr/Models/Attention/moat.py
+-rw-rw-rw-   0        0        0     3670 2024-03-09 15:08:27.000000 pyzjr-1.3.6/pyzjr/Models/Attention/muse.py
+-rw-rw-rw-   0        0        0     2281 2024-03-09 15:11:27.000000 pyzjr-1.3.6/pyzjr/Models/Attention/outlook.py
+-rw-rw-rw-   0        0        0      985 2024-03-09 15:29:37.000000 pyzjr-1.3.6/pyzjr/Models/Attention/parnet.py
+-rw-rw-rw-   0        0        0     4087 2024-03-09 15:13:38.000000 pyzjr-1.3.6/pyzjr/Models/Attention/polarized.py
+-rw-rw-rw-   0        0        0     2296 2024-03-09 15:11:51.000000 pyzjr-1.3.6/pyzjr/Models/Attention/psa.py
+-rw-rw-rw-   0        0        0      930 2024-03-09 14:57:03.000000 pyzjr-1.3.6/pyzjr/Models/Attention/residual.py
+-rw-rw-rw-   0        0        0     2355 2024-03-09 14:52:15.000000 pyzjr-1.3.6/pyzjr/Models/Attention/s2.py
+-rw-rw-rw-   0        0        0     3084 2024-03-09 15:15:20.000000 pyzjr-1.3.6/pyzjr/Models/Attention/self_att.py
+-rw-rw-rw-   0        0        0     1784 2024-03-09 15:14:10.000000 pyzjr-1.3.6/pyzjr/Models/Attention/sge.py
+-rw-rw-rw-   0        0        0     2637 2024-03-09 15:16:05.000000 pyzjr-1.3.6/pyzjr/Models/Attention/shuffle.py
+-rw-rw-rw-   0        0        0      909 2024-03-09 15:16:39.000000 pyzjr-1.3.6/pyzjr/Models/Attention/simam.py
+-rw-rw-rw-   0        0        0     2933 2024-03-09 15:17:26.000000 pyzjr-1.3.6/pyzjr/Models/Attention/simplified_self_att.py
+-rw-rw-rw-   0        0        0     1863 2024-03-18 11:12:03.000000 pyzjr-1.3.6/pyzjr/Models/Attention/sk.py
+-rw-rw-rw-   0        0        0     2349 2024-03-09 15:18:03.000000 pyzjr-1.3.6/pyzjr/Models/Attention/triplet.py
+-rw-rw-rw-   0        0        0     2234 2024-03-04 13:24:57.000000 pyzjr-1.3.6/pyzjr/Models/Attention/ufo.py
+-rw-rw-rw-   0        0        0      220 2024-03-16 15:32:39.000000 pyzjr-1.3.6/pyzjr/Models/__init__.py
+-rw-rw-rw-   0        0        0     3384 2024-03-21 16:32:55.000000 pyzjr-1.3.6/pyzjr/Models/_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/backbone/
+-rw-rw-rw-   0        0        0     5692 2024-03-22 16:07:30.000000 pyzjr-1.3.6/pyzjr/Models/backbone/Darknet.py
+-rw-rw-rw-   0        0        0    25919 2024-02-23 14:10:01.000000 pyzjr-1.3.6/pyzjr/Models/backbone/Ghostnet.py
+-rw-rw-rw-   0        0        0     1953 2024-03-26 15:38:25.000000 pyzjr-1.3.6/pyzjr/Models/backbone/__init__.py
+-rw-rw-rw-   0        0        0     1935 2024-04-01 07:58:53.000000 pyzjr-1.3.6/pyzjr/Models/backbone/alexnet.py
+-rw-rw-rw-   0        0        0     7560 2024-02-23 14:18:22.000000 pyzjr-1.3.6/pyzjr/Models/backbone/conv2former.py
+-rw-rw-rw-   0        0        0     6278 2024-02-23 14:18:22.000000 pyzjr-1.3.6/pyzjr/Models/backbone/densenet.py
+-rw-rw-rw-   0        0        0    12866 2024-04-01 09:42:37.000000 pyzjr-1.3.6/pyzjr/Models/backbone/drn.py
+-rw-rw-rw-   0        0        0    17934 2024-04-01 08:53:51.000000 pyzjr-1.3.6/pyzjr/Models/backbone/efficientnet.py
+-rw-rw-rw-   0        0        0     7210 2024-04-01 09:54:02.000000 pyzjr-1.3.6/pyzjr/Models/backbone/fasternet.py
+-rw-rw-rw-   0        0        0     5623 2024-02-23 14:18:22.000000 pyzjr-1.3.6/pyzjr/Models/backbone/googlenet.py
+-rw-rw-rw-   0        0        0     1869 2024-02-04 04:44:18.000000 pyzjr-1.3.6/pyzjr/Models/backbone/lenet.py
+-rw-rw-rw-   0        0        0     7048 2024-03-18 16:29:49.000000 pyzjr-1.3.6/pyzjr/Models/backbone/mnasnet.py
+-rw-rw-rw-   0        0        0    16395 2024-02-16 16:51:01.000000 pyzjr-1.3.6/pyzjr/Models/backbone/mobilenet.py
+-rw-rw-rw-   0        0        0     9972 2024-04-18 15:14:36.000000 pyzjr-1.3.6/pyzjr/Models/backbone/nasnet.py
+-rw-rw-rw-   0        0        0     7217 2024-03-18 11:17:15.000000 pyzjr-1.3.6/pyzjr/Models/backbone/regnet.py
+-rw-rw-rw-   0        0        0     8910 2024-04-01 09:47:10.000000 pyzjr-1.3.6/pyzjr/Models/backbone/resnet.py
+-rw-rw-rw-   0        0        0    11356 2024-03-22 15:56:05.000000 pyzjr-1.3.6/pyzjr/Models/backbone/shufflenet.py
+-rw-rw-rw-   0        0        0     4392 2024-03-04 12:30:07.000000 pyzjr-1.3.6/pyzjr/Models/backbone/squeezenet.py
+-rw-rw-rw-   0        0        0     3996 2024-02-25 16:22:54.000000 pyzjr-1.3.6/pyzjr/Models/backbone/vgg.py
+-rw-rw-rw-   0        0        0     5866 2024-04-01 09:44:12.000000 pyzjr-1.3.6/pyzjr/Models/backbone/xception.py
+-rw-rw-rw-   0        0        0     2705 2024-03-22 15:32:04.000000 pyzjr-1.3.6/pyzjr/Models/backbone/zfnet.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/bricks/
+-rw-rw-rw-   0        0        0     5577 2024-04-01 09:57:01.000000 pyzjr-1.3.6/pyzjr/Models/bricks/Initer.py
+-rw-rw-rw-   0        0        0      426 2024-04-18 15:04:29.000000 pyzjr-1.3.6/pyzjr/Models/bricks/__init__.py
+-rw-rw-rw-   0        0        0     1577 2024-03-04 09:07:17.000000 pyzjr-1.3.6/pyzjr/Models/bricks/classfier.py
+-rw-rw-rw-   0        0        0    22575 2024-03-04 07:32:10.000000 pyzjr-1.3.6/pyzjr/Models/bricks/comblock.py
+-rw-rw-rw-   0        0        0     2646 2024-03-26 15:25:44.000000 pyzjr-1.3.6/pyzjr/Models/bricks/conv_norm_act.py
+-rw-rw-rw-   0        0        0     6828 2024-03-04 12:40:27.000000 pyzjr-1.3.6/pyzjr/Models/bricks/drop.py
+-rw-rw-rw-   0        0        0     6669 2024-03-06 00:10:20.000000 pyzjr-1.3.6/pyzjr/Models/bricks/mlp.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/conv/
+-rw-rw-rw-   0        0        0     1974 2024-04-18 13:35:49.000000 pyzjr-1.3.6/pyzjr/Models/conv/Depthwise_Conv.py
+-rw-rw-rw-   0        0        0      508 2024-03-21 15:46:28.000000 pyzjr-1.3.6/pyzjr/Models/conv/Dilated_Conv.py
+-rw-rw-rw-   0        0        0     1862 2024-02-29 10:04:41.000000 pyzjr-1.3.6/pyzjr/Models/conv/Partial_Conv.py
+-rw-rw-rw-   0        0        0     2660 2024-02-29 10:02:23.000000 pyzjr-1.3.6/pyzjr/Models/conv/Ref_Conv.py
+-rw-rw-rw-   0        0        0    11456 2024-04-28 14:23:02.000000 pyzjr-1.3.6/pyzjr/Models/conv/Snake_Conv.py
+-rw-rw-rw-   0        0        0      295 2024-03-21 15:46:28.000000 pyzjr-1.3.6/pyzjr/Models/conv/__init__.py
+-rw-rw-rw-   0        0        0     3029 2024-04-14 00:39:15.000000 pyzjr-1.3.6/pyzjr/Models/networks.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/sampling/
+-rw-rw-rw-   0        0        0      754 2024-04-05 14:24:23.000000 pyzjr-1.3.6/pyzjr/Models/sampling/__init__.py
+-rw-rw-rw-   0        0        0     4857 2024-04-05 16:18:30.000000 pyzjr-1.3.6/pyzjr/Models/sampling/adaptivepooling.py
+-rw-rw-rw-   0        0        0     1393 2024-01-27 17:10:24.000000 pyzjr-1.3.6/pyzjr/Models/sampling/haarwavelet.py
+-rw-rw-rw-   0        0        0     1828 2024-03-04 13:56:06.000000 pyzjr-1.3.6/pyzjr/Models/sampling/medianpooling.py
+-rw-rw-rw-   0        0        0     4792 2024-02-26 15:35:21.000000 pyzjr-1.3.6/pyzjr/Models/sampling/standardpooling.py
+-rw-rw-rw-   0        0        0      854 2024-03-01 15:33:22.000000 pyzjr-1.3.6/pyzjr/Models/sampling/strideconv.py
+-rw-rw-rw-   0        0        0     3692 2024-02-29 15:43:47.000000 pyzjr-1.3.6/pyzjr/Models/sampling/strippooling.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/Models/segmentation/
+-rw-rw-rw-   0        0        0       70 2024-02-27 16:31:33.000000 pyzjr-1.3.6/pyzjr/Models/segmentation/__init__.py
+-rw-rw-rw-   0        0        0    24988 2024-03-17 06:46:22.000000 pyzjr-1.3.6/pyzjr/Models/segmentation/fcn.py
+-rw-rw-rw-   0        0        0     3289 2024-02-29 09:20:12.000000 pyzjr-1.3.6/pyzjr/Models/segmentation/unet.py
+-rw-rw-rw-   0        0        0     6328 2024-04-20 07:32:10.000000 pyzjr-1.3.6/pyzjr/PIC.py
+-rw-rw-rw-   0        0        0    10349 2024-02-04 05:11:03.000000 pyzjr-1.3.6/pyzjr/Z.py
+-rw-rw-rw-   0        0        0      896 2024-04-14 00:39:15.000000 pyzjr-1.3.6/pyzjr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/augmentation/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/
+-rw-rw-rw-   0        0        0    13180 2024-04-13 15:26:35.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/Crack.py
+-rw-rw-rw-   0        0        0     8307 2024-02-29 15:56:54.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/_Steger.py
+-rw-rw-rw-   0        0        0      366 2024-02-19 10:23:26.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/__init__.py
+-rw-rw-rw-   0        0        0     7681 2024-02-18 17:28:31.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/definition.py
+-rw-rw-rw-   0        0        0     4835 2024-04-29 07:32:55.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/pixel.py
+-rw-rw-rw-   0        0        0     1685 2024-04-13 15:00:07.000000 pyzjr-1.3.6/pyzjr/augmentation/Pixel/utils.py
+-rw-rw-rw-   0        0        0      116 2024-04-13 14:32:14.000000 pyzjr-1.3.6/pyzjr/augmentation/__init__.py
+-rw-rw-rw-   0        0        0    28649 2024-04-25 17:12:47.000000 pyzjr-1.3.6/pyzjr/augmentation/augments.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/
+-rw-rw-rw-   0        0        0      306 2024-02-01 16:36:53.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2192 2024-02-02 16:09:04.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/_utils.py
+-rw-rw-rw-   0        0        0     3413 2024-02-28 11:40:46.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/normal.py
+-rw-rw-rw-   0        0        0    10459 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/opencv.py
+-rw-rw-rw-   0        0        0    40685 2024-04-25 17:14:56.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/pillow.py
+-rw-rw-rw-   0        0        0     6139 2024-03-21 17:03:45.000000 pyzjr-1.3.6/pyzjr/augmentation/transforms/tvision.py
+-rw-rw-rw-   0        0        0     1084 2024-03-04 06:15:09.000000 pyzjr-1.3.6/pyzjr/augmentation/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/core/
+-rw-rw-rw-   0        0        0     1136 2024-04-23 16:30:06.000000 pyzjr-1.3.6/pyzjr/core/__init__.py
+-rw-rw-rw-   0        0        0     6991 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/core/__tensor.py
+-rw-rw-rw-   0        0        0      680 2023-10-07 12:04:40.000000 pyzjr-1.3.6/pyzjr/core/_utils.py
+-rw-rw-rw-   0        0        0      982 2024-04-28 11:13:49.000000 pyzjr-1.3.6/pyzjr/core/decorator.py
+-rw-rw-rw-   0        0        0     2123 2024-04-23 16:46:56.000000 pyzjr-1.3.6/pyzjr/core/error.py
+-rw-rw-rw-   0        0        0     2692 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/core/general.py
+-rw-rw-rw-   0        0        0      671 2024-04-23 16:26:12.000000 pyzjr-1.3.6/pyzjr/core/helpers.py
+-rw-rw-rw-   0        0        0     7254 2023-11-15 11:43:15.000000 pyzjr-1.3.6/pyzjr/core/lr_scheduler.py
+-rw-rw-rw-   0        0        0    15534 2024-04-21 15:07:11.000000 pyzjr-1.3.6/pyzjr/core/utils_pytorch_numpy_unification.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/data/
+-rw-rw-rw-   0        0        0     1486 2024-03-13 01:39:58.000000 pyzjr-1.3.6/pyzjr/data/Dataloader.py
+-rw-rw-rw-   0        0        0     9590 2024-03-08 01:06:58.000000 pyzjr-1.3.6/pyzjr/data/Dataset.py
+-rw-rw-rw-   0        0        0    12147 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/data/FM.py
+-rw-rw-rw-   0        0        0      215 2024-04-14 15:31:09.000000 pyzjr-1.3.6/pyzjr/data/__init__.py
+-rw-rw-rw-   0        0        0     4064 2024-04-14 00:26:57.000000 pyzjr-1.3.6/pyzjr/data/basedataset.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/data/data_set/
+-rw-rw-rw-   0        0        0     9436 2024-03-13 01:39:58.000000 pyzjr-1.3.6/pyzjr/data/data_set/Pascal_voc.py
+-rw-rw-rw-   0        0        0        0 2024-02-29 16:00:47.000000 pyzjr-1.3.6/pyzjr/data/data_set/__init__.py
+-rw-rw-rw-   0        0        0     1313 2024-03-08 01:30:08.000000 pyzjr-1.3.6/pyzjr/data/data_set/config.py
+-rw-rw-rw-   0        0        0    15340 2024-04-13 15:04:54.000000 pyzjr-1.3.6/pyzjr/data/reader.py
+-rw-rw-rw-   0        0        0      934 2024-04-14 15:26:14.000000 pyzjr-1.3.6/pyzjr/data/txt_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/devices/
+-rw-rw-rw-   0        0        0      523 2024-04-27 13:06:29.000000 pyzjr-1.3.6/pyzjr/devices/__init__.py
+-rw-rw-rw-   0        0        0     1572 2024-04-13 15:22:13.000000 pyzjr-1.3.6/pyzjr/devices/get_device.py
+-rw-rw-rw-   0        0        0     3032 2024-04-27 13:06:29.000000 pyzjr-1.3.6/pyzjr/devices/measures.py
+-rw-rw-rw-   0        0        0     1202 2024-04-13 15:53:39.000000 pyzjr-1.3.6/pyzjr/devices/systeminfo.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/dlearn/
+-rw-rw-rw-   0        0        0      949 2024-03-11 15:45:28.000000 pyzjr-1.3.6/pyzjr/dlearn/__init__.py
+-rw-rw-rw-   0        0        0     8571 2024-02-17 18:07:27.000000 pyzjr-1.3.6/pyzjr/dlearn/callbacklog.py
+-rw-rw-rw-   0        0        0     8379 2024-03-13 01:39:58.000000 pyzjr-1.3.6/pyzjr/dlearn/callbacks.py
+-rw-rw-rw-   0        0        0     1051 2024-03-11 15:59:35.000000 pyzjr-1.3.6/pyzjr/dlearn/savemodels.py
+-rw-rw-rw-   0        0        0     5603 2024-04-25 13:21:27.000000 pyzjr-1.3.6/pyzjr/dlearn/strategy.py
+-rw-rw-rw-   0        0        0     5955 2024-04-13 15:28:23.000000 pyzjr-1.3.6/pyzjr/dlearn/tools.py
+-rw-rw-rw-   0        0        0     7356 2024-04-27 09:06:57.000000 pyzjr-1.3.6/pyzjr/dlearn/trainer.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/nn/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/
+-rw-rw-rw-   0        0        0      768 2024-04-28 11:08:26.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/__init__.py
+-rw-rw-rw-   0        0        0    16268 2024-04-28 09:10:34.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/classification.py
+-rw-rw-rw-   0        0        0     3822 2024-04-28 09:10:34.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/indexutils.py
+-rw-rw-rw-   0        0        0     9779 2024-04-28 09:10:34.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/medical_index.py
+-rw-rw-rw-   0        0        0     5837 2024-04-27 18:14:38.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/segment3d.py
+-rw-rw-rw-   0        0        0    11847 2024-04-28 09:10:34.000000 pyzjr-1.3.6/pyzjr/nn/Metrics/semantic.py
+-rw-rw-rw-   0        0        0     9459 2024-04-18 15:17:33.000000 pyzjr-1.3.6/pyzjr/nn/Summary.py
+-rw-rw-rw-   0        0        0      123 2024-04-18 15:17:33.000000 pyzjr-1.3.6/pyzjr/nn/__init__.py
+-rw-rw-rw-   0        0        0    84332 2024-02-22 15:45:34.000000 pyzjr-1.3.6/pyzjr/nn/functional.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/
+-rw-rw-rw-   0        0        0     3262 2024-04-27 18:28:45.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/OneHot.py
+-rw-rw-rw-   0        0        0      835 2024-04-28 10:41:07.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/__init__.py
+-rw-rw-rw-   0        0        0     7197 2024-04-27 18:54:23.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/avgweight.py
+-rw-rw-rw-   0        0        0    15225 2024-02-20 09:56:56.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/learnrate.py
+-rw-rw-rw-   0        0        0    27275 2024-04-28 11:08:26.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/loss_function.py
+-rw-rw-rw-   0        0        0     5217 2024-04-28 10:13:24.000000 pyzjr-1.3.6/pyzjr/nn/torchutils/loss_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/torch3D/
+-rw-rw-rw-   0        0        0       57 2024-04-28 14:21:27.000000 pyzjr-1.3.6/pyzjr/torch3D/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/
+-rw-rw-rw-   0        0        0      266 2024-04-28 14:17:48.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/__init__.py
+-rw-rw-rw-   0        0        0     6344 2024-04-28 12:59:48.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/basic_unet.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/block/
+-rw-rw-rw-   0        0        0    22077 2024-04-28 11:42:36.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/block/DSConv.py
+-rw-rw-rw-   0        0        0       28 2024-04-28 11:44:10.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/block/__init__.py
+-rw-rw-rw-   0        0        0     7862 2024-04-28 12:59:48.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/dscnet.py
+-rw-rw-rw-   0        0        0     5755 2024-04-28 13:34:14.000000 pyzjr-1.3.6/pyzjr/torch3D/networks/vent.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/torch3D/nii/
+-rw-rw-rw-   0        0        0      306 2024-04-28 11:13:49.000000 pyzjr-1.3.6/pyzjr/torch3D/nii/__init__.py
+-rw-rw-rw-   0        0        0     4420 2024-04-27 18:49:10.000000 pyzjr-1.3.6/pyzjr/torch3D/nii/mri.py
+-rw-rw-rw-   0        0        0     4363 2024-04-28 12:59:48.000000 pyzjr-1.3.6/pyzjr/torch3D/nii/nifti_dataset.py
+-rw-rw-rw-   0        0        0     3373 2024-04-28 15:35:45.000000 pyzjr-1.3.6/pyzjr/torch3D/nii/nii_utils.py
+-rw-rw-rw-   0        0        0       21 2024-04-29 07:32:55.000000 pyzjr-1.3.6/pyzjr/version.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/visualize/
+-rw-rw-rw-   0        0        0      410 2024-04-14 15:13:36.000000 pyzjr-1.3.6/pyzjr/visualize/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/visualize/color/
+-rw-rw-rw-   0        0        0     1418 2024-04-13 14:47:13.000000 pyzjr-1.3.6/pyzjr/visualize/color/__init__.py
+-rw-rw-rw-   0        0        0     4848 2024-04-13 14:43:57.000000 pyzjr-1.3.6/pyzjr/visualize/color/colormap.py
+-rw-rw-rw-   0        0        0     3339 2023-11-04 05:34:46.000000 pyzjr-1.3.6/pyzjr/visualize/color/colorspace.py
+-rw-rw-rw-   0        0        0     7471 2024-04-13 14:47:13.000000 pyzjr-1.3.6/pyzjr/visualize/color/cvplot.py
+-rw-rw-rw-   0        0        0     7937 2024-04-13 15:27:09.000000 pyzjr-1.3.6/pyzjr/visualize/color/findcolor.py
+-rw-rw-rw-   0        0        0     1066 2024-02-13 17:07:55.000000 pyzjr-1.3.6/pyzjr/visualize/color/hex.py
+-rw-rw-rw-   0        0        0    10972 2024-04-28 11:08:26.000000 pyzjr-1.3.6/pyzjr/visualize/io.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr/visualize/mediapipe/
+-rw-rw-rw-   0        0        0     6556 2024-04-14 15:13:36.000000 pyzjr-1.3.6/pyzjr/visualize/mediapipe/HandTrack.py
+-rw-rw-rw-   0        0        0      376 2024-01-25 07:15:10.000000 pyzjr-1.3.6/pyzjr/visualize/mediapipe/__init__.py
+-rw-rw-rw-   0        0        0      631 2024-02-04 05:11:03.000000 pyzjr-1.3.6/pyzjr/visualize/mediapipe/const.py
+-rw-rw-rw-   0        0        0     4327 2024-04-13 15:04:54.000000 pyzjr-1.3.6/pyzjr/visualize/printf.py
+-rw-rw-rw-   0        0        0     3367 2024-02-22 15:48:11.000000 pyzjr-1.3.6/pyzjr/visualize/utils.py
+-rw-rw-rw-   0        0        0     3796 2024-02-19 09:13:27.000000 pyzjr-1.3.6/pyzjr/visualize/video_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr.egg-info/
+-rw-rw-rw-   0        0        0     2931 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5988 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-29 07:32:59.000000 pyzjr-1.3.6/pyzjr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 07:32:59.000000 pyzjr-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     2207 2024-04-29 07:32:55.000000 pyzjr-1.3.6/setup.py
```

### Comparing `pyzjr-1.3.5/LICENSE` & `pyzjr-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/PKG-INFO` & `pyzjr-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.3.5
+Version: 1.3.6
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Keywords: python,computer vision,pyzjr,windows
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pyzjr-1.3.5/README.md` & `pyzjr-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Math/Numpy.py` & `pyzjr-1.3.6/pyzjr/Math/Numpy.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Math/arithmetic.py` & `pyzjr-1.3.6/pyzjr/Math/arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Math/function.py` & `pyzjr-1.3.6/pyzjr/Math/function.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Math/point_line.py` & `pyzjr-1.3.6/pyzjr/Math/point_line.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/A2.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/A2.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/AFT.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/AFT.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/DANet.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/DANet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/MobileViT.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/MobileViT.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/SE.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/SE.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/ViP.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/ViP.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/__init__.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/acmix.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/acmix.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/axial.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/axial.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/bam.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/bam.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/cbam.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/cbam.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/coord.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/coord.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/cot.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/cot.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/crisscross.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/crisscross.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/crossformer.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/crossformer.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/dat.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/dat.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/eca.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/eca.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/emsa.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/emsa.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/external.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/external.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/gfnet.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/gfnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/halo.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/halo.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/moat.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/moat.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/muse.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/muse.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/outlook.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/outlook.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/parnet.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/parnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/polarized.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/polarized.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/psa.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/psa.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/residual.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/residual.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/s2.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/s2.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/self_att.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/self_att.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/sge.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/sge.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/shuffle.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/shuffle.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/simam.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/simam.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/simplified_self_att.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/simplified_self_att.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/sk.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/sk.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/triplet.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/triplet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/Attention/ufo.py` & `pyzjr-1.3.6/pyzjr/Models/Attention/ufo.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/_utils.py` & `pyzjr-1.3.6/pyzjr/Models/_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/Darknet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/Darknet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/Ghostnet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/Ghostnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/__init__.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/alexnet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/alexnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/conv2former.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/conv2former.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/densenet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/densenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/drn.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/drn.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/efficientnet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/efficientnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/fasternet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/fasternet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/googlenet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/googlenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/lenet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/lenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/mnasnet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/mnasnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/mobilenet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/mobilenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/nasnet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/nasnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/regnet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/resnet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/shufflenet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/shufflenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/squeezenet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/squeezenet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/vgg.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/vgg.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/xception.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/xception.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/backbone/zfnet.py` & `pyzjr-1.3.6/pyzjr/Models/backbone/zfnet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/bricks/Initer.py` & `pyzjr-1.3.6/pyzjr/Models/bricks/Initer.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/bricks/classfier.py` & `pyzjr-1.3.6/pyzjr/Models/bricks/classfier.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/bricks/comblock.py` & `pyzjr-1.3.6/pyzjr/Models/bricks/comblock.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/bricks/conv_norm_act.py` & `pyzjr-1.3.6/pyzjr/Models/bricks/conv_norm_act.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/bricks/drop.py` & `pyzjr-1.3.6/pyzjr/Models/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/bricks/mlp.py` & `pyzjr-1.3.6/pyzjr/Models/bricks/mlp.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/conv/Depthwise_Conv.py` & `pyzjr-1.3.6/pyzjr/Models/conv/Depthwise_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/conv/Partial_Conv.py` & `pyzjr-1.3.6/pyzjr/Models/conv/Partial_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/conv/Ref_Conv.py` & `pyzjr-1.3.6/pyzjr/Models/conv/Ref_Conv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/conv/Snake_Conv.py` & `pyzjr-1.3.6/pyzjr/Models/conv/Snake_Conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 class DSConv(nn.Module):
     def __init__(self, in_channels=1, out_channels=1, kernel_size=9, extend_scope=1.0,
-                 morph=0, if_offset=True, device="cuda",):
+                 morph=0, if_offset=True, device='cuda' if torch.cuda.is_available() else 'cpu',):
         """
         :param in_channels: 输入通道的数量
         :param out_channels: 输出通道的数量
         :param kernel_size: 内核的大小
         :param extend_scope: 要扩大的范围。此方法的默认值为 1
         :param morph: 卷积核的形态主要沿 x轴（0）和 y轴（1）分为两类
         :param if_offset: 是否需要变形，如果为False，则为标准卷积核。
@@ -261,22 +261,20 @@
                         [2.3, 2.4, 2.5],
                         [2.6, 2.7, 2.8]]],
 
                       [[[3.0, 3.1, 3.2],
                         [3.3, 3.4, 3.5],
                         [3.6, 3.7, 3.8]]]])
 
-    print("输入形状", A.shape)  # torch.Size([4, 1, 3, 3])
+    print("输入形状:", A.shape)  # torch.Size([4, 1, 3, 3])
     conv0 = DSConv(
         in_channels=1,
         out_channels=10,
         kernel_size=15,
         extend_scope=1,
         morph=0,
-        if_offset=True,
-        device="cpu")
+        if_offset=True)
     if torch.cuda.is_available():
         A = A.to(device)
         conv0 = conv0.to(device)
     out = conv0(A)
-    print("输出形状：",out.shape)   # torch.Size([4, 10, 3, 3])
-    # print(out)
+    print("输出形状:", out.shape)  # torch.Size([4, 10, 3, 3])
```

### Comparing `pyzjr-1.3.5/pyzjr/Models/networks.py` & `pyzjr-1.3.6/pyzjr/Models/networks.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/sampling/__init__.py` & `pyzjr-1.3.6/pyzjr/Models/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/sampling/adaptivepooling.py` & `pyzjr-1.3.6/pyzjr/Models/sampling/adaptivepooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/sampling/haarwavelet.py` & `pyzjr-1.3.6/pyzjr/Models/sampling/haarwavelet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/sampling/medianpooling.py` & `pyzjr-1.3.6/pyzjr/Models/sampling/medianpooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/sampling/standardpooling.py` & `pyzjr-1.3.6/pyzjr/Models/sampling/standardpooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/sampling/strideconv.py` & `pyzjr-1.3.6/pyzjr/Models/sampling/strideconv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/sampling/strippooling.py` & `pyzjr-1.3.6/pyzjr/Models/sampling/strippooling.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/segmentation/fcn.py` & `pyzjr-1.3.6/pyzjr/Models/segmentation/fcn.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/Models/segmentation/unet.py` & `pyzjr-1.3.6/pyzjr/Models/segmentation/unet.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/PIC.py` & `pyzjr-1.3.6/pyzjr/PIC.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import cv2
 from pylab import *
-# from pyzjr.augmentation.Color import ColorFind
 import pyzjr.Z as Z
 from pyzjr.Math import *
 from skimage.morphology import disk
 from skimage.filters import rank
 from skimage import measure
 from torchvision import transforms
```

### Comparing `pyzjr-1.3.5/pyzjr/Z.py` & `pyzjr-1.3.6/pyzjr/Z.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/__init__.py` & `pyzjr-1.3.6/pyzjr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/augmentation/Pixel/Crack.py` & `pyzjr-1.3.6/pyzjr/augmentation/Pixel/Crack.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/augmentation/Pixel/_Steger.py` & `pyzjr-1.3.6/pyzjr/augmentation/Pixel/_Steger.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/augmentation/Pixel/definition.py` & `pyzjr-1.3.6/pyzjr/augmentation/Pixel/definition.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/augmentation/Pixel/pixel.py` & `pyzjr-1.3.6/pyzjr/augmentation/Pixel/pixel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import cv2
 import string
 from skimage.morphology import skeletonize
 from skimage.filters import threshold_otsu
 from skimage.color import rgb2gray
-from pyzjr.core import is_gray_image
+from pyzjr.core.general import is_gray_image
 
 __all__=["SkeletonMap", "incircle", "outcircle"]
 
 def SkeletonMap(target):
     """
     获取骨架图的信息
     :param target: 目标图
```

### Comparing `pyzjr-1.3.5/pyzjr/augmentation/Pixel/utils.py` & `pyzjr-1.3.6/pyzjr/augmentation/Pixel/utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/augmentation/augments.py` & `pyzjr-1.3.6/pyzjr/augmentation/augments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 这一部分主要针对于opencv格式的,一般这部分用于传统图像的增强
 """
 import numpy as np
 import cv2
 from math import ceil
 import random
-from pyzjr.core import _check_parameter_is_tuple_2, _check_parameter_is_tuple_and_list_2
+from pyzjr.core.error import _check_parameter_is_tuple_2, _check_parameter_is_tuple_and_list_2
 
 __all__ = ["base_crop1", "base_crop2", "center_crop", "five_crop", "Stitcher_image",\
 
            "Centerzoom", "flip", "horizontal_flip", "vertical_flip", "resize", "adjust_brightness_cv2", "adjust_brightness_numpy",\
 
            "rotate", "adjust_gamma", "pad", "erase", "augment_Hsv","hist_equalize","random_resize_crop","random_crop",\
```

### Comparing `pyzjr-1.3.5/pyzjr/augmentation/transforms/_utils.py` & `pyzjr-1.3.6/pyzjr/augmentation/transforms/_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/augmentation/transforms/normal.py` & `pyzjr-1.3.6/pyzjr/augmentation/transforms/normal.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/augmentation/transforms/opencv.py` & `pyzjr-1.3.6/pyzjr/augmentation/transforms/opencv.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/augmentation/transforms/pillow.py` & `pyzjr-1.3.6/pyzjr/augmentation/transforms/pillow.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 All rights reserved.
 
 This module is based on PIL implemented transformations.
 """
 import torch
 from PIL import Image, ImageOps, ImageEnhance, ImageFilter
 import random
-from pyzjr.core import _check_img_is_plt, is_pil,_check_img_is_ndarray, _check_parameter_is_tuple_and_list_or_single_2, \
-    _check_input_is_tensor, get_image_size, _get_image_num_channels, is_int
+from pyzjr.core.error import _check_img_is_plt, is_pil,_check_img_is_ndarray, _check_parameter_is_tuple_and_list_or_single_2, \
+    _check_input_is_tensor
+from pyzjr.core.general import get_image_size, is_int, get_image_num_channels, is_list_or_tuple
 from ._utils import Images, Compose
 import numpy as np
 
 __all__ = ["PILToTensor",
            "NdarryToPIL",
            "TensorToPIL",
            "MeanStdNormalize",
@@ -818,15 +819,15 @@
         >>> transforms = Compose([Grayscale(), PILToTensor(), TensorToPIL()])
         >>> transformed_image = transforms(image)
     """
     def __init__(self):
         super(Grayscale, self).__init__()
 
     def to_gray(self, img):
-        channels = _get_image_num_channels(img)
+        channels = get_image_num_channels(img)
         if channels == 1:
             img = img.convert('L')
         elif channels == 3:
             img = img.convert('L')
             np_img = np.array(img, dtype=np.uint8)
             np_img = np.dstack([np_img, np_img, np_img])
             img = Image.fromarray(np_img, 'RGB')
```

### Comparing `pyzjr-1.3.5/pyzjr/augmentation/transforms/tvision.py` & `pyzjr-1.3.6/pyzjr/augmentation/transforms/tvision.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/augmentation/utils.py` & `pyzjr-1.3.6/pyzjr/augmentation/utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/core/__init__.py` & `pyzjr-1.3.6/pyzjr/core/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     softmax,
     stack,
     tensor,
     where,
     zeros,
     zeros_like,
 )
+from .decorator import timing
 from .lr_scheduler import _LRScheduler
 from .error import *
 
 from .helpers import (
     _ntuple,
     to_1tuple,
     to_2tuple,
```

### Comparing `pyzjr-1.3.5/pyzjr/core/__tensor.py` & `pyzjr-1.3.6/pyzjr/core/__tensor.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/core/_utils.py` & `pyzjr-1.3.6/pyzjr/core/_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/core/error.py` & `pyzjr-1.3.6/pyzjr/core/error.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,8 +39,14 @@
         raise ValueError(f"{a} should be a list or tuple of two values.")
 
 def _check_parameter_is_tuple_and_list_or_single_2(a):
     if not (isinstance(a, int) or (isinstance(a, (list, tuple)) and len(a) == 2)):
         raise TypeError('Should be a single number or a list/tuple (h, w) of length 2.'
                         'Got {}.'.format(a))
 
+def assert_shape(a, b):
+    assert a.shape == b.shape, "Shape mismatch: {} and {}".format(
+        a.shape, b.shape)
 
+def assert_size(a, b):
+    assert a.size == b.size, "Size mismatch: {} and {}".format(
+        a.size, b.size)
```

### Comparing `pyzjr-1.3.5/pyzjr/core/general.py` & `pyzjr-1.3.6/pyzjr/core/general.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/core/helpers.py` & `pyzjr-1.3.6/pyzjr/core/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,7 +18,8 @@
     if isinstance(value, int):
         return (value, value)
     elif isinstance(value, (list, tuple)):
         if len(value) == 2:
             return value
         else:
             raise ValueError("The input object is of type list or tuple, but the length is not two!")
+
```

### Comparing `pyzjr-1.3.5/pyzjr/core/lr_scheduler.py` & `pyzjr-1.3.6/pyzjr/core/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/data/Dataloader.py` & `pyzjr-1.3.6/pyzjr/data/Dataloader.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/data/Dataset.py` & `pyzjr-1.3.6/pyzjr/data/Dataset.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/data/FM.py` & `pyzjr-1.3.6/pyzjr/data/FM.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/data/basedataset.py` & `pyzjr-1.3.6/pyzjr/data/basedataset.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/data/data_set/Pascal_voc.py` & `pyzjr-1.3.6/pyzjr/data/data_set/Pascal_voc.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/data/data_set/config.py` & `pyzjr-1.3.6/pyzjr/data/data_set/config.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/data/reader.py` & `pyzjr-1.3.6/pyzjr/data/reader.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/data/txt_utils.py` & `pyzjr-1.3.6/pyzjr/data/txt_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/devices/get_device.py` & `pyzjr-1.3.6/pyzjr/devices/get_device.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/devices/measures.py` & `pyzjr-1.3.6/pyzjr/devices/measures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import gc
 import threading
 import time
 import psutil
 import torch
 
-__all__ = ["PeakCPUMemory", "start_measure", "end_measure", "log_measures"]
+__all__ = ["release_gpu_memory", "PeakCPUMemory", "start_measure", "end_measure",
+           "log_measures"]
+
+def release_gpu_memory():
+    gc.collect()
+    if torch.cuda.is_available():
+        torch.cuda.empty_cache()
 
 class PeakCPUMemory:
     def __init__(self):
         self.process = psutil.Process()
         self.peak_monitoring = False
 
     def peak_monitor(self):
```

### Comparing `pyzjr-1.3.5/pyzjr/devices/systeminfo.py` & `pyzjr-1.3.6/pyzjr/devices/systeminfo.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/dlearn/__init__.py` & `pyzjr-1.3.6/pyzjr/dlearn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/dlearn/callbacklog.py` & `pyzjr-1.3.6/pyzjr/dlearn/callbacklog.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/dlearn/callbacks.py` & `pyzjr-1.3.6/pyzjr/dlearn/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/dlearn/savemodels.py` & `pyzjr-1.3.6/pyzjr/dlearn/savemodels.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/dlearn/strategy.py` & `pyzjr-1.3.6/pyzjr/dlearn/strategy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 from PIL import Image
 import torch
 import random
 from thop import clever_format, profile
 from torchsummary import summary
+import warnings
 
 # def mixup(img1, labels, img2, labels2):
 #     # Applies MixUp augmentation https://arxiv.org/pdf/1710.09412.pdf
 #     r = np.random.beta(32.0, 32.0)  # mixup ratio, alpha=beta=32.0
 #     img = (img1 * r + img2 * (1 - r)).astype(np.uint8)
 #     labels = np.concatenate((labels, labels2), 0)
 #     return img, labels
@@ -93,31 +94,45 @@
         new_image = Image.new('RGB', size, (128,128,128))
         new_image.paste(image, ((w-nw)//2, (h-nh)//2))
         return new_image, nw, nh
     else:
         new_image = image.resize((w, h), Image.BICUBIC)
         return new_image
 
-def SeedEvery(seed=11, rank=0):
+def SeedEvery(seed=11, rank=0, use_deterministic_algorithms=None):
     """
     :param seed: 设置基础随机种子
     :param rank: 进程的排名，用于为每个进程设置不同的种子
+    :param use_deterministic_algorithms: 是否使用确定性算法
     """
     combined_seed = seed + rank
     random.seed(combined_seed)
     np.random.seed(combined_seed)
     torch.manual_seed(combined_seed)
     if torch.cuda.is_available():
         import torch.backends.cudnn as cudnn
         import torch.backends.cuda as cuda
         cuda.matmul.allow_tf32 = True
         cudnn.benchmark = True
         torch.cuda.manual_seed(combined_seed)
         torch.cuda.manual_seed_all(combined_seed)
 
+    if torch.backends.flags_frozen():
+        warnings.warn("PyTorch global flag support of backends is disabled, enable it to set global `cudnn` flags.")
+        torch.backends.__allow_nonbracketed_mutation_flag = True
+        
+    if use_deterministic_algorithms:
+        if hasattr(torch, "use_deterministic_algorithms"):
+            torch.use_deterministic_algorithms(True)
+        elif hasattr(torch, "set_deterministic"):
+            torch.set_deterministic(True)
+        else:
+            warnings.warn("If use_deterministic-algorithms=True is set, pytorch version "
+                          "greater than 1.8 may be required to use this feature properly.")
+
 def summarys(input_shape, model):
     """
     打印模型的摘要信息，并计算模型的总浮点运算量和总参数数量
     :param input_shape:
     :param model:要进行计算的模型
     """
     device = "cuda" if torch.cuda.is_available() else "cpu"
```

### Comparing `pyzjr-1.3.5/pyzjr/dlearn/tools.py` & `pyzjr-1.3.6/pyzjr/dlearn/tools.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/dlearn/trainer.py` & `pyzjr-1.3.6/pyzjr/dlearn/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,18 +154,16 @@
     model = SimpleCNN()
     model.to(device)
     loss_function = nn.CrossEntropyLoss()
     optimizer = optim.Adam(model.parameters(), lr=0.001)
     lr_scheduler = StepLR(optimizer, step_size=5, gamma=0.1)
     scaler = GradScaler()
 
-
     Epochs = 10
 
-
     classification_trainer = Classification_train_and_eval(
         net=model,
         train_loader=train_loader,
         val_loader=val_loader,
         epochs=Epochs,
         device=device,
         loss_function=loss_function,
```

### Comparing `pyzjr-1.3.5/pyzjr/nn/Metrics/classification.py` & `pyzjr-1.3.6/pyzjr/nn/Metrics/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,24 @@
 Actual Positive  |        TP          |         FN         |
 Actual Negative  |        FP          |         TN         |
 Time: 2024-01-27
 """
 import numpy as np
 import torch
 
-__all__ = ["accuracy_all_classes", "cls_matrix", "BinaryConfusionMatrix", "MulticlassConfusionMatrix",
-           "ConfusionMatrixs", "ModelIndex", "calculate_metrics", "MultiLabelConfusionMatrix"]
+__all__ = [
+    "accuracy_all_classes",
+    "cls_matrix",
+    "BinaryConfusionMatrix",
+    "MulticlassConfusionMatrix",
+    "ConfusionMatrixs",
+    "ModelIndex",
+    "calculate_metrics",
+    "MultiLabelConfusionMatrix"
+]
 
 def accuracy_all_classes(output, target):
     """
     仅用于所有分类的准确率计算,这里是每个批次的准确率,所以在使用时还要进行itera的累计
     """
     batch_size = target.size(0)
     _, pred = output.max(1)
```

### Comparing `pyzjr-1.3.5/pyzjr/nn/Metrics/semantic.py` & `pyzjr-1.3.6/pyzjr/nn/Metrics/semantic.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,22 @@
 Actual Positive  |        TP          |         FN         |
 Actual Negative  |        FP          |         TN         |
 Time: 2024-01-26
 """
 import torch
 import numpy as np
 
-__all__ = ["Miou", "Recall", "Precision", "F1Score", "DiceCoefficient", "Accuracy",
-           "SegmentationIndex", "AIU"]
+__all__ = ["Miou",
+           "Recall",
+           "Precision",
+           "F1Score",
+           "DiceCoefficient",
+           "Accuracy",
+           "SegmentationIndex",
+           "AIU"]
 
 class Miou(object):
     """
     iou = ( A & B ) / ( A | B )
     """
     def __init__(self, num_classes, ignore=None, threshold=.5, esp=1e-5):
         self.num_classes = num_classes
```

### Comparing `pyzjr-1.3.5/pyzjr/nn/Summary.py` & `pyzjr-1.3.6/pyzjr/nn/Summary.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/nn/functional.py` & `pyzjr-1.3.6/pyzjr/nn/functional.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/nn/torchutils/OneHot.py` & `pyzjr-1.3.6/pyzjr/nn/torchutils/OneHot.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 time 2024-01-11
 """
 import torch
 import numpy as np
 from pyzjr.core.general import is_tensor, is_numpy
 
-__all__ = ["one_hot", "get_one_hot", "get_one_hot_with_torch", "get_one_hot_with_np"]
+__all__ = ["one_hot", "get_one_hot", "get_one_hot_with_torch",
+           "get_one_hot_with_np", "one_hot_3d"]
 
 def one_hot(labels, num_classes=-1):
     """
     将标签转为独热编码, 经过测试与torch.nn.functional里面的函数测试相同
     :param labels: 标签
     :param num_classes: 默认为-1, 表示进行自动计算类别最大的那个
     Examples:
@@ -66,14 +67,27 @@
 
 def get_one_hot(labels, num_classes=-1):
     if is_numpy(labels):
         return get_one_hot_with_np(labels=labels, num_classes=num_classes)
     if is_tensor(labels):
         return get_one_hot_with_torch(labels=labels, num_classes=num_classes)
 
+def one_hot_3d(y, num_classes=None):
+    y = y.astype(np.int64)
+    input_shape = y.shape
+
+    if num_classes is None:
+        num_classes = np.max(y) + 1
+
+    y_reshaped = y.reshape(-1)
+    y_onehot = np.eye(num_classes)[y_reshaped]
+    y_onehot = y_onehot.reshape(*input_shape, num_classes)
+
+    return y_onehot
+
 if __name__=="__main__":
     seg_labels = np.random.randint(0, 3, size=[512, 512])
     seg_labels2 = torch.randint(0, 3, size=[512, 512])
     print(get_one_hot(seg_labels))
     print(get_one_hot(seg_labels).shape)
     print(get_one_hot(seg_labels2))   # torch.Size([512, 512, 3])
     print(get_one_hot(seg_labels2).shape)
```

### Comparing `pyzjr-1.3.5/pyzjr/nn/torchutils/avgweight.py` & `pyzjr-1.3.6/pyzjr/nn/torchutils/avgweight.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 Copyright (c) 2024, Auorui.
 All rights reserved.
 
 Weighted average, reference from <https://pytorch.org/docs/stable/optim.html#putting-it-all-together-ema>
 指数移动平均（EMA）   常见
 随机加权平均（SWA）   https://arxiv.org/abs/1803.05407
 Tanh自适应指数移动EMA算法（T_ADEMA）    Originating from https://kns.cnki.net/kcms2/article/abstract?v=vdPasdvfHvuuN-gB4G4neXcKqbiX3vnPwH2QfVTNb4OQCyQJO2HTgHpa6C3EDWqlnkrcNyjnTtxYjmozsntFZzru-e7vk_X4Fq9NCmtavFoJFkztVbWX1vr5qj9w2djSGdHx0-RWLb0=&uniplatform=NZKPT&flag=copy
+
 https://blog.csdn.net/m0_62919535/article/details/135482009?spm=1001.2014.3001.5501
+
 time 2024-01-09
 """
 import torch
 from copy import deepcopy
 from pyzjr.core.general import is_parallel
 import itertools
 from torch.nn import Module
```

### Comparing `pyzjr-1.3.5/pyzjr/nn/torchutils/learnrate.py` & `pyzjr-1.3.6/pyzjr/nn/torchutils/learnrate.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/visualize/color/__init__.py` & `pyzjr-1.3.6/pyzjr/visualize/color/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/visualize/color/colormap.py` & `pyzjr-1.3.6/pyzjr/visualize/color/colormap.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/visualize/color/colorspace.py` & `pyzjr-1.3.6/pyzjr/visualize/color/colorspace.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/visualize/color/cvplot.py` & `pyzjr-1.3.6/pyzjr/visualize/color/cvplot.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/visualize/color/findcolor.py` & `pyzjr-1.3.6/pyzjr/visualize/color/findcolor.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/visualize/color/hex.py` & `pyzjr-1.3.6/pyzjr/visualize/color/hex.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/visualize/io.py` & `pyzjr-1.3.6/pyzjr/visualize/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 """
 import os
 import cv2
 import imghdr
 import torch
 import numpy as np
 from urllib import request
+
 from matplotlib import pyplot as plt
-from pyzjr.core import is_url
 plt.rcParams['font.sans-serif'] = ['SimHei']
 plt.rcParams['axes.unicode_minus'] = False
 from pathlib import Path
-from pyzjr.core import is_gray_image, is_pil
+from pyzjr.core.general import is_gray_image, is_pil, is_url
 
 __all__ = ["ImagesReader", "imwrite", "imshowplt", "StackedCV2", "StackedImages", "Stackedplt",
            "Stackedtorch", "plot_line", "bar_chart", "scatter_plot", "url2cvImage"]
 
 RGB2BGR  = cv2.COLOR_RGB2BGR
 BGR2RGB  = cv2.COLOR_BGR2RGB
 BGR2GRAY = cv2.COLOR_BGR2GRAY
```

### Comparing `pyzjr-1.3.5/pyzjr/visualize/mediapipe/HandTrack.py` & `pyzjr-1.3.6/pyzjr/visualize/mediapipe/HandTrack.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/visualize/mediapipe/const.py` & `pyzjr-1.3.6/pyzjr/visualize/mediapipe/const.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/visualize/printf.py` & `pyzjr-1.3.6/pyzjr/visualize/printf.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/visualize/utils.py` & `pyzjr-1.3.6/pyzjr/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr/visualize/video_utils.py` & `pyzjr-1.3.6/pyzjr/visualize/video_utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.3.5/pyzjr.egg-info/PKG-INFO` & `pyzjr-1.3.6/pyzjr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.3.5
+Version: 1.3.6
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Keywords: python,computer vision,pyzjr,windows
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pyzjr-1.3.5/pyzjr.egg-info/SOURCES.txt` & `pyzjr-1.3.6/pyzjr.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -119,18 +119,20 @@
 pyzjr/augmentation/transforms/normal.py
 pyzjr/augmentation/transforms/opencv.py
 pyzjr/augmentation/transforms/pillow.py
 pyzjr/augmentation/transforms/tvision.py
 pyzjr/core/__init__.py
 pyzjr/core/__tensor.py
 pyzjr/core/_utils.py
+pyzjr/core/decorator.py
 pyzjr/core/error.py
 pyzjr/core/general.py
 pyzjr/core/helpers.py
 pyzjr/core/lr_scheduler.py
+pyzjr/core/utils_pytorch_numpy_unification.py
 pyzjr/data/Dataloader.py
 pyzjr/data/Dataset.py
 pyzjr/data/FM.py
 pyzjr/data/__init__.py
 pyzjr/data/basedataset.py
 pyzjr/data/dataloader.py
 pyzjr/data/dataset.py
@@ -152,23 +154,37 @@
 pyzjr/dlearn/trainer.py
 pyzjr/math/__init__.py
 pyzjr/nn/Summary.py
 pyzjr/nn/__init__.py
 pyzjr/nn/functional.py
 pyzjr/nn/Metrics/__init__.py
 pyzjr/nn/Metrics/classification.py
+pyzjr/nn/Metrics/indexutils.py
+pyzjr/nn/Metrics/medical_index.py
+pyzjr/nn/Metrics/segment3d.py
 pyzjr/nn/Metrics/semantic.py
 pyzjr/nn/torchutils/OneHot.py
 pyzjr/nn/torchutils/__init__.py
 pyzjr/nn/torchutils/avgweight.py
 pyzjr/nn/torchutils/learnrate.py
 pyzjr/nn/torchutils/loss_function.py
 pyzjr/nn/torchutils/loss_utils.py
 pyzjr/torch3D/__init__.py
 pyzjr/torch3D/networks/__init__.py
+pyzjr/torch3d/__init__.py
+pyzjr/torch3d/networks/__init__.py
+pyzjr/torch3d/networks/basic_unet.py
+pyzjr/torch3d/networks/dscnet.py
+pyzjr/torch3d/networks/vent.py
+pyzjr/torch3d/networks/block/DSConv.py
+pyzjr/torch3d/networks/block/__init__.py
+pyzjr/torch3d/nii/__init__.py
+pyzjr/torch3d/nii/mri.py
+pyzjr/torch3d/nii/nifti_dataset.py
+pyzjr/torch3d/nii/nii_utils.py
 pyzjr/visualize/__init__.py
 pyzjr/visualize/io.py
 pyzjr/visualize/printf.py
 pyzjr/visualize/utils.py
 pyzjr/visualize/video_utils.py
 pyzjr/visualize/color/__init__.py
 pyzjr/visualize/color/colormap.py
```

### Comparing `pyzjr-1.3.5/setup.py` & `pyzjr-1.3.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 - creation time:2022.10
 - pyzjr is the Codebase accumulated by my python programming.
   At present, it is only for my personal use. If you want to
   use it, please contact me. Here are my email and WeChat.
 - WeChat: z15583909992
 - Email: zjricetea@gmail.com
 - Note: Currently still being updated, please refer to the latest version for any changes that may occur
+
+    python setup.py sdist
+    twine upload dist/*
 """
 import codecs
 import os
 from setuptools import setup, find_packages
 
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # from pyzjr.version import __version__
-VERSION = "1.3.5"
+VERSION = "1.3.6"
 DESCRIPTION = ' A computer vision library that supports Win, packaged with patches for visual libraries such as \
                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui) \
                 engineering code experience. '
 LONG_DESCRIPTION = 'pyzjr is a computer vision library that supports Win'
 
 setup(
     name="pyzjr",
@@ -47,14 +50,15 @@
         'torch',
         'pywin32',
         'einops',
         'tensorboard',
         'pytorch_wavelets',
         'opencv-python',
         'torchvision',
+        'nibabel',
     ],
     keywords=['python', 'computer vision', 'pyzjr','windows'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
```

