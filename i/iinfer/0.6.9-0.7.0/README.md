# Comparing `tmp/iinfer-0.6.9.tar.gz` & `tmp/iinfer-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iinfer-0.6.9.tar", last modified: Mon Apr 15 12:38:00 2024, max compression
+gzip compressed data, was "iinfer-0.7.0.tar", last modified: Mon Apr 29 11:29:40 2024, max compression
```

## Comparing `iinfer-0.6.9.tar` & `iinfer-0.7.0.tar`

### file list

```diff
@@ -1,192 +1,191 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.944293 iinfer-0.6.9/
--rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.6.9/LICENSE
--rw-rw-rw-   0        0        0     5553 2024-04-15 12:38:00.942295 iinfer-0.6.9/PKG-INFO
--rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.6.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.874571 iinfer-0.6.9/iinfer/
--rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/__init__.py
--rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.942578 iinfer-0.6.9/iinfer/app/
--rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.6.9/iinfer/app/__init__.py
--rw-rw-rw-   0        0        0    44638 2024-04-14 02:06:22.000000 iinfer-0.6.9/iinfer/app/app.py
--rw-rw-rw-   0        0        0    31308 2024-04-14 08:44:28.000000 iinfer-0.6.9/iinfer/app/client.py
--rw-rw-rw-   0        0        0    12382 2024-04-13 10:46:15.000000 iinfer-0.6.9/iinfer/app/common.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.962579 iinfer-0.6.9/iinfer/app/commons/
--rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.6.9/iinfer/app/commons/convert.py
--rw-rw-rw-   0        0        0     7466 2024-03-30 02:49:07.000000 iinfer-0.6.9/iinfer/app/commons/module.py
--rw-rw-rw-   0        0        0    57143 2024-04-15 11:48:19.000000 iinfer-0.6.9/iinfer/app/gui.py
--rw-rw-rw-   0        0        0     5247 2024-04-11 12:30:41.000000 iinfer-0.6.9/iinfer/app/injection.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.019585 iinfer-0.6.9/iinfer/app/injections/
--rw-rw-rw-   0        0        0     2023 2024-04-11 11:13:52.000000 iinfer-0.6.9/iinfer/app/injections/after_cls_jadge_injection.py
--rw-rw-rw-   0        0        0     4500 2024-04-06 14:50:20.000000 iinfer-0.6.9/iinfer/app/injections/after_csv_injection.py
--rw-rw-rw-   0        0        0     6515 2024-04-07 06:56:33.000000 iinfer-0.6.9/iinfer/app/injections/after_det_filter_injection.py
--rw-rw-rw-   0        0        0     8540 2024-04-07 07:16:07.000000 iinfer-0.6.9/iinfer/app/injections/after_det_jadge_injection.py
--rw-rw-rw-   0        0        0     4790 2024-04-07 00:11:59.000000 iinfer-0.6.9/iinfer/app/injections/after_http_injection.py
--rw-rw-rw-   0        0        0     9077 2024-04-11 13:28:27.000000 iinfer-0.6.9/iinfer/app/injections/after_seg_bbox_injection.py
--rw-rw-rw-   0        0        0     8688 2024-04-11 13:41:09.000000 iinfer-0.6.9/iinfer/app/injections/after_seg_filter_injection.py
--rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.6.9/iinfer/app/injections/before_grayimg_injection.py
--rw-rw-rw-   0        0        0    14447 2024-03-23 14:43:05.000000 iinfer-0.6.9/iinfer/app/install.py
--rw-rw-rw-   0        0        0     4811 2024-03-10 08:54:06.000000 iinfer-0.6.9/iinfer/app/postprocess.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.089592 iinfer-0.6.9/iinfer/app/postprocesses/
--rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/app/postprocesses/cls_jadge.py
--rw-rw-rw-   0        0        0     2393 2024-04-06 14:52:31.000000 iinfer-0.6.9/iinfer/app/postprocesses/csv.py
--rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.6.9/iinfer/app/postprocesses/det_clip.py
--rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.6.9/iinfer/app/postprocesses/det_face_store.py
--rw-rw-rw-   0        0        0     4444 2024-04-11 13:48:21.000000 iinfer-0.6.9/iinfer/app/postprocesses/det_filter.py
--rw-rw-rw-   0        0        0     5201 2024-04-07 07:20:08.000000 iinfer-0.6.9/iinfer/app/postprocesses/det_jadge.py
--rw-rw-rw-   0        0        0     3813 2024-04-07 00:25:09.000000 iinfer-0.6.9/iinfer/app/postprocesses/httpreq.py
--rw-rw-rw-   0        0        0     4369 2024-04-11 13:06:06.000000 iinfer-0.6.9/iinfer/app/postprocesses/seg_bbox.py
--rw-rw-rw-   0        0        0     4252 2024-04-11 12:27:14.000000 iinfer-0.6.9/iinfer/app/postprocesses/seg_filter.py
--rw-rw-rw-   0        0        0     6077 2024-02-24 13:15:38.000000 iinfer-0.6.9/iinfer/app/predict.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.147601 iinfer-0.6.9/iinfer/app/predicts/
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/app/predicts/__init__.py
--rw-rw-rw-   0        0        0     7618 2024-03-30 02:49:18.000000 iinfer-0.6.9/iinfer/app/predicts/insightface_det.py
--rw-rw-rw-   0        0        0     4134 2024-03-30 02:49:30.000000 iinfer-0.6.9/iinfer/app/predicts/mmdet_det_YoloX.py
--rw-rw-rw-   0        0        0      384 2024-03-30 02:49:24.000000 iinfer-0.6.9/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     4712 2024-03-30 02:49:40.000000 iinfer-0.6.9/iinfer/app/predicts/mmpretrain_cls_swin.py
--rw-rw-rw-   0        0        0      418 2024-03-30 02:49:36.000000 iinfer-0.6.9/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
--rw-rw-rw-   0        0        0    10366 2024-03-30 02:49:45.000000 iinfer-0.6.9/iinfer/app/predicts/mmrotate_det_ReDet.py
--rw-rw-rw-   0        0        0     5712 2024-04-05 13:16:32.000000 iinfer-0.6.9/iinfer/app/predicts/mmseg_seg_PSPNet.py
--rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.6.9/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
--rw-rw-rw-   0        0        0     4647 2024-03-30 02:50:02.000000 iinfer-0.6.9/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
--rw-rw-rw-   0        0        0     5301 2024-03-30 02:50:07.000000 iinfer-0.6.9/iinfer/app/predicts/onnx_det_TinyYoloV3.py
--rw-rw-rw-   0        0        0     5509 2024-03-30 02:50:11.000000 iinfer-0.6.9/iinfer/app/predicts/onnx_det_YoloV3.py
--rw-rw-rw-   0        0        0     9843 2024-03-30 02:50:23.000000 iinfer-0.6.9/iinfer/app/predicts/onnx_det_YoloX.py
--rw-rw-rw-   0        0        0     2887 2024-03-30 02:50:17.000000 iinfer-0.6.9/iinfer/app/predicts/onnx_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/app/redis.py
--rw-rw-rw-   0        0        0    49856 2024-04-15 12:16:57.000000 iinfer-0.6.9/iinfer/app/server.py
--rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/config.yml
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.165604 iinfer-0.6.9/iinfer/datasets/
--rw-rw-rw-   0        0        0      684 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/datasets/label_coco.txt
--rw-rw-rw-   0        0        0      153 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/datasets/label_voc.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.195605 iinfer-0.6.9/iinfer/docker/
--rw-rw-rw-   0        0        0      813 2024-03-11 12:27:01.000000 iinfer-0.6.9/iinfer/docker/Dockerfile
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/docker/__init__.py
--rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/docker/build.sh
--rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/docker/docker-compose.yml
-drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.773558 iinfer-0.6.9/iinfer/extensions/
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.244649 iinfer-0.6.9/iinfer/extensions/injection/
--rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.6.9/iinfer/extensions/injection/after_cls_jadge_injection.json
--rw-rw-rw-   0        0        0       99 2024-04-11 14:24:51.000000 iinfer-0.6.9/iinfer/extensions/injection/after_csv_injection.json
--rw-rw-rw-   0        0        0      129 2024-04-07 04:03:58.000000 iinfer-0.6.9/iinfer/extensions/injection/after_det_filter_injection.json
--rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.6.9/iinfer/extensions/injection/after_det_jadge_injection.json
--rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.6.9/iinfer/extensions/injection/after_http_injection.json
--rw-rw-rw-   0        0        0      107 2024-04-07 03:43:59.000000 iinfer-0.6.9/iinfer/extensions/injection/after_seg_bbox_injection.json
--rw-rw-rw-   0        0        0      115 2024-04-07 03:42:37.000000 iinfer-0.6.9/iinfer/extensions/injection/after_seg_filter_injection.json
--rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.6.9/iinfer/extensions/injection/before_gray_injection.json
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.623016 iinfer-0.6.9/iinfer/licenses/
--rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
--rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
--rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
--rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
--rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
--rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
--rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
--rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
--rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
--rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
--rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
--rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
--rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
--rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
--rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
--rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
--rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
--rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
--rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
--rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
--rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
--rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
--rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
--rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
--rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
--rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
--rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
--rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
--rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
--rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/files.txt
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/logconf_client.yml
--rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/logconf_gui.yml
--rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/logconf_install.yml
--rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/logconf_postprocess.yml
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/logconf_redis.yml
--rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/logconf_server.yml
--rw-rw-rw-   0        0        0     1010 2024-04-15 11:45:35.000000 iinfer-0.6.9/iinfer/version.py
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.628022 iinfer-0.6.9/iinfer/web/
-drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.807561 iinfer-0.6.9/iinfer/web/assets/
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.667266 iinfer-0.6.9/iinfer/web/assets/bootstrap/
--rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
--rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
--rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
--rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.736272 iinfer-0.6.9/iinfer/web/assets/iinfer/
--rw-rw-rw-   0        0        0     5664 2024-04-12 12:02:38.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/filer_modal.js
--rw-rw-rw-   0        0        0    16712 2024-04-12 12:00:35.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/list_cmd.js
--rw-rw-rw-   0        0        0     6560 2024-04-12 12:12:27.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/list_pipe.js
--rw-rw-rw-   0        0        0     4447 2024-04-12 12:12:53.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/main.js
--rw-rw-rw-   0        0        0      439 2024-04-12 12:08:33.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/open_capture.js
--rw-rw-rw-   0        0        0      459 2024-04-12 12:07:28.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/open_output_json.js
--rw-rw-rw-   0        0        0      122 2024-03-03 02:33:47.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/svfiler.css
--rw-rw-rw-   0        0        0    24743 2024-04-15 12:24:01.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/svfiler.js
--rw-rw-rw-   0        0        0     1079 2024-04-12 12:06:23.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/view_raw.js
--rw-rw-rw-   0        0        0     4543 2024-04-12 12:04:28.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/view_result.js
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.739270 iinfer-0.6.9/iinfer/web/assets/jquery/
--rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery/jquery.min.3.2.0.js
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.744273 iinfer-0.6.9/iinfer/web/assets/jquery-resizable/
--rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.795280 iinfer-0.6.9/iinfer/web/assets/jquery-ui/
--rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/AUTHORS.txt
--rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.866286 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/
--rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
--rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
--rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
--rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
--rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.min.css
--rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.min.js
--rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
--rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
--rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/package.json
-drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.806563 iinfer-0.6.9/iinfer/web/assets/lightbox2/
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.872286 iinfer-0.6.9/iinfer/web/assets/lightbox2/css/
--rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/lightbox2/css/lightbox.min.css
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.903292 iinfer-0.6.9/iinfer/web/assets/lightbox2/images/
--rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/lightbox2/images/close.png
--rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/lightbox2/images/loading.gif
--rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/lightbox2/images/next.png
--rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/lightbox2/images/prev.png
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.907292 iinfer-0.6.9/iinfer/web/assets/lightbox2/js/
--rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/lightbox2/js/lightbox.min.js
-drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.808561 iinfer-0.6.9/iinfer/web/assets/tree-menu/
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.911289 iinfer-0.6.9/iinfer/web/assets/tree-menu/css/
--rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/tree-menu/css/tree-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.936295 iinfer-0.6.9/iinfer/web/assets/tree-menu/image/
--rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/tree-menu/image/file.png
--rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/tree-menu/image/folder-close.png
--rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/tree-menu/image/folder-open.png
-drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.940295 iinfer-0.6.9/iinfer/web/assets/tree-menu/js/
--rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/tree-menu/js/tree-menu.js
--rw-rw-rw-   0        0        0    30911 2024-04-13 04:36:58.000000 iinfer-0.6.9/iinfer/web/main.html
-drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.894571 iinfer-0.6.9/iinfer.egg-info/
--rw-rw-rw-   0        0        0     5553 2024-04-15 12:37:59.000000 iinfer-0.6.9/iinfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7259 2024-04-15 12:37:59.000000 iinfer-0.6.9/iinfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 12:37:59.000000 iinfer-0.6.9/iinfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-15 12:37:59.000000 iinfer-0.6.9/iinfer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-04-15 12:37:59.000000 iinfer-0.6.9/iinfer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-15 12:37:59.000000 iinfer-0.6.9/iinfer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 12:38:00.944293 iinfer-0.6.9/setup.cfg
--rw-rw-rw-   0        0        0     2185 2024-04-06 23:22:57.000000 iinfer-0.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.516207 iinfer-0.7.0/
+-rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     5553 2024-04-29 11:29:40.514207 iinfer-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.843204 iinfer-0.7.0/iinfer/
+-rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/__init__.py
+-rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.893203 iinfer-0.7.0/iinfer/app/
+-rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.7.0/iinfer/app/__init__.py
+-rw-rw-rw-   0        0        0    49119 2024-04-28 12:19:10.000000 iinfer-0.7.0/iinfer/app/app.py
+-rw-rw-rw-   0        0        0    33060 2024-04-28 13:16:47.000000 iinfer-0.7.0/iinfer/app/client.py
+-rw-rw-rw-   0        0        0    13214 2024-04-28 13:45:06.000000 iinfer-0.7.0/iinfer/app/common.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.902202 iinfer-0.7.0/iinfer/app/commons/
+-rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.7.0/iinfer/app/commons/convert.py
+-rw-rw-rw-   0        0        0     7466 2024-03-30 02:49:07.000000 iinfer-0.7.0/iinfer/app/commons/module.py
+-rw-rw-rw-   0        0        0     3508 2024-04-28 01:45:44.000000 iinfer-0.7.0/iinfer/app/gui.py
+-rw-rw-rw-   0        0        0     5247 2024-04-11 12:30:41.000000 iinfer-0.7.0/iinfer/app/injection.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.939203 iinfer-0.7.0/iinfer/app/injections/
+-rw-rw-rw-   0        0        0     2023 2024-04-11 11:13:52.000000 iinfer-0.7.0/iinfer/app/injections/after_cls_jadge_injection.py
+-rw-rw-rw-   0        0        0     4500 2024-04-06 14:50:20.000000 iinfer-0.7.0/iinfer/app/injections/after_csv_injection.py
+-rw-rw-rw-   0        0        0     6515 2024-04-07 06:56:33.000000 iinfer-0.7.0/iinfer/app/injections/after_det_filter_injection.py
+-rw-rw-rw-   0        0        0     8540 2024-04-07 07:16:07.000000 iinfer-0.7.0/iinfer/app/injections/after_det_jadge_injection.py
+-rw-rw-rw-   0        0        0     4790 2024-04-07 00:11:59.000000 iinfer-0.7.0/iinfer/app/injections/after_http_injection.py
+-rw-rw-rw-   0        0        0     9077 2024-04-11 13:28:27.000000 iinfer-0.7.0/iinfer/app/injections/after_seg_bbox_injection.py
+-rw-rw-rw-   0        0        0     8688 2024-04-11 13:41:09.000000 iinfer-0.7.0/iinfer/app/injections/after_seg_filter_injection.py
+-rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.7.0/iinfer/app/injections/before_grayimg_injection.py
+-rw-rw-rw-   0        0        0    14447 2024-03-23 14:43:05.000000 iinfer-0.7.0/iinfer/app/install.py
+-rw-rw-rw-   0        0        0     4811 2024-03-10 08:54:06.000000 iinfer-0.7.0/iinfer/app/postprocess.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.984207 iinfer-0.7.0/iinfer/app/postprocesses/
+-rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/app/postprocesses/cls_jadge.py
+-rw-rw-rw-   0        0        0     2393 2024-04-06 14:52:31.000000 iinfer-0.7.0/iinfer/app/postprocesses/csv.py
+-rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.7.0/iinfer/app/postprocesses/det_clip.py
+-rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.7.0/iinfer/app/postprocesses/det_face_store.py
+-rw-rw-rw-   0        0        0     4444 2024-04-11 13:48:21.000000 iinfer-0.7.0/iinfer/app/postprocesses/det_filter.py
+-rw-rw-rw-   0        0        0     5201 2024-04-07 07:20:08.000000 iinfer-0.7.0/iinfer/app/postprocesses/det_jadge.py
+-rw-rw-rw-   0        0        0     3813 2024-04-07 00:25:09.000000 iinfer-0.7.0/iinfer/app/postprocesses/httpreq.py
+-rw-rw-rw-   0        0        0     4369 2024-04-11 13:06:06.000000 iinfer-0.7.0/iinfer/app/postprocesses/seg_bbox.py
+-rw-rw-rw-   0        0        0     4252 2024-04-11 12:27:14.000000 iinfer-0.7.0/iinfer/app/postprocesses/seg_filter.py
+-rw-rw-rw-   0        0        0     6077 2024-02-24 13:15:38.000000 iinfer-0.7.0/iinfer/app/predict.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.024206 iinfer-0.7.0/iinfer/app/predicts/
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/app/predicts/__init__.py
+-rw-rw-rw-   0        0        0     7618 2024-03-30 02:49:18.000000 iinfer-0.7.0/iinfer/app/predicts/insightface_det.py
+-rw-rw-rw-   0        0        0     4134 2024-03-30 02:49:30.000000 iinfer-0.7.0/iinfer/app/predicts/mmdet_det_YoloX.py
+-rw-rw-rw-   0        0        0      384 2024-03-30 02:49:24.000000 iinfer-0.7.0/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     4712 2024-03-30 02:49:40.000000 iinfer-0.7.0/iinfer/app/predicts/mmpretrain_cls_swin.py
+-rw-rw-rw-   0        0        0      418 2024-03-30 02:49:36.000000 iinfer-0.7.0/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
+-rw-rw-rw-   0        0        0    10366 2024-03-30 02:49:45.000000 iinfer-0.7.0/iinfer/app/predicts/mmrotate_det_ReDet.py
+-rw-rw-rw-   0        0        0     5712 2024-04-05 13:16:32.000000 iinfer-0.7.0/iinfer/app/predicts/mmseg_seg_PSPNet.py
+-rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.7.0/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
+-rw-rw-rw-   0        0        0     4647 2024-03-30 02:50:02.000000 iinfer-0.7.0/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
+-rw-rw-rw-   0        0        0     5301 2024-03-30 02:50:07.000000 iinfer-0.7.0/iinfer/app/predicts/onnx_det_TinyYoloV3.py
+-rw-rw-rw-   0        0        0     5509 2024-03-30 02:50:11.000000 iinfer-0.7.0/iinfer/app/predicts/onnx_det_YoloV3.py
+-rw-rw-rw-   0        0        0     9843 2024-03-30 02:50:23.000000 iinfer-0.7.0/iinfer/app/predicts/onnx_det_YoloX.py
+-rw-rw-rw-   0        0        0     2887 2024-03-30 02:50:17.000000 iinfer-0.7.0/iinfer/app/predicts/onnx_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/app/redis.py
+-rw-rw-rw-   0        0        0    51249 2024-04-29 07:04:17.000000 iinfer-0.7.0/iinfer/app/server.py
+-rw-rw-rw-   0        0        0    76790 2024-04-29 10:40:51.000000 iinfer-0.7.0/iinfer/app/web.py
+-rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/config.yml
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.041204 iinfer-0.7.0/iinfer/docker/
+-rw-rw-rw-   0        0        0      813 2024-03-11 12:27:01.000000 iinfer-0.7.0/iinfer/docker/Dockerfile
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/docker/__init__.py
+-rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/docker/build.sh
+-rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/docker/docker-compose.yml
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.787210 iinfer-0.7.0/iinfer/extensions/
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.080206 iinfer-0.7.0/iinfer/extensions/injection/
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.0/iinfer/extensions/injection/after_cls_jadge_injection.json
+-rw-rw-rw-   0        0        0       99 2024-04-11 14:24:51.000000 iinfer-0.7.0/iinfer/extensions/injection/after_csv_injection.json
+-rw-rw-rw-   0        0        0      129 2024-04-07 04:03:58.000000 iinfer-0.7.0/iinfer/extensions/injection/after_det_filter_injection.json
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.0/iinfer/extensions/injection/after_det_jadge_injection.json
+-rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.7.0/iinfer/extensions/injection/after_http_injection.json
+-rw-rw-rw-   0        0        0      107 2024-04-07 03:43:59.000000 iinfer-0.7.0/iinfer/extensions/injection/after_seg_bbox_injection.json
+-rw-rw-rw-   0        0        0      115 2024-04-07 03:42:37.000000 iinfer-0.7.0/iinfer/extensions/injection/after_seg_filter_injection.json
+-rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.7.0/iinfer/extensions/injection/before_gray_injection.json
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.341204 iinfer-0.7.0/iinfer/licenses/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
+-rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
+-rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
+-rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
+-rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
+-rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
+-rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
+-rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
+-rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
+-rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
+-rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
+-rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
+-rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
+-rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
+-rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
+-rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
+-rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
+-rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
+-rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
+-rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
+-rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.7.0/iinfer/licenses/files.txt
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/logconf_client.yml
+-rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/logconf_gui.yml
+-rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/logconf_install.yml
+-rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/logconf_postprocess.yml
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/logconf_redis.yml
+-rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/logconf_server.yml
+-rw-rw-rw-   0        0        0      630 2024-04-25 10:56:07.000000 iinfer-0.7.0/iinfer/logconf_web.yml
+-rw-rw-rw-   0        0        0     1010 2024-04-29 10:52:21.000000 iinfer-0.7.0/iinfer/version.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.344207 iinfer-0.7.0/iinfer/web/
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.793205 iinfer-0.7.0/iinfer/web/assets/
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.366204 iinfer-0.7.0/iinfer/web/assets/bootstrap/
+-rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
+-rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
+-rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
+-rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.397205 iinfer-0.7.0/iinfer/web/assets/iinfer/
+-rw-rw-rw-   0        0        0     5664 2024-04-23 14:00:17.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/filer_modal.js
+-rw-rw-rw-   0        0        0    16723 2024-04-28 01:44:14.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/list_cmd.js
+-rw-rw-rw-   0        0        0     6675 2024-04-28 01:46:33.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/list_pipe.js
+-rw-rw-rw-   0        0        0     5581 2024-04-23 14:04:49.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/main.js
+-rw-rw-rw-   0        0        0      439 2024-04-23 14:05:01.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/open_capture.js
+-rw-rw-rw-   0        0        0      459 2024-04-23 14:05:10.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/open_output_json.js
+-rw-rw-rw-   0        0        0      127 2024-04-18 14:57:44.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/svfiler.css
+-rw-rw-rw-   0        0        0    24976 2024-04-23 14:07:35.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/svfiler.js
+-rw-rw-rw-   0        0        0     1246 2024-04-23 14:07:58.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/view_raw.js
+-rw-rw-rw-   0        0        0     4543 2024-04-23 14:08:58.000000 iinfer-0.7.0/iinfer/web/assets/iinfer/view_result.js
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.401205 iinfer-0.7.0/iinfer/web/assets/jquery/
+-rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery/jquery.min.3.2.0.js
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.404204 iinfer-0.7.0/iinfer/web/assets/jquery-resizable/
+-rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.442206 iinfer-0.7.0/iinfer/web/assets/jquery-ui/
+-rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.473201 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/
+-rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
+-rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
+-rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
+-rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
+-rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.min.css
+-rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.min.js
+-rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
+-rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
+-rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/jquery-ui/package.json
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.793205 iinfer-0.7.0/iinfer/web/assets/lightbox2/
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.476203 iinfer-0.7.0/iinfer/web/assets/lightbox2/css/
+-rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/lightbox2/css/lightbox.min.css
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.490207 iinfer-0.7.0/iinfer/web/assets/lightbox2/images/
+-rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/lightbox2/images/close.png
+-rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/lightbox2/images/loading.gif
+-rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/lightbox2/images/next.png
+-rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/lightbox2/images/prev.png
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.493205 iinfer-0.7.0/iinfer/web/assets/lightbox2/js/
+-rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/lightbox2/js/lightbox.min.js
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.795208 iinfer-0.7.0/iinfer/web/assets/tree-menu/
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.496205 iinfer-0.7.0/iinfer/web/assets/tree-menu/css/
+-rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/tree-menu/css/tree-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.508205 iinfer-0.7.0/iinfer/web/assets/tree-menu/image/
+-rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/tree-menu/image/file.png
+-rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/tree-menu/image/folder-close.png
+-rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/tree-menu/image/folder-open.png
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:40.512207 iinfer-0.7.0/iinfer/web/assets/tree-menu/js/
+-rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.7.0/iinfer/web/assets/tree-menu/js/tree-menu.js
+-rw-rw-rw-   0        0        0    31056 2024-04-21 10:24:46.000000 iinfer-0.7.0/iinfer/web/gui.html
+drwxrwxrwx   0        0        0        0 2024-04-29 11:29:39.858204 iinfer-0.7.0/iinfer.egg-info/
+-rw-rw-rw-   0        0        0     5553 2024-04-29 11:29:39.000000 iinfer-0.7.0/iinfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7238 2024-04-29 11:29:39.000000 iinfer-0.7.0/iinfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 11:29:39.000000 iinfer-0.7.0/iinfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 11:29:39.000000 iinfer-0.7.0/iinfer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-04-29 11:29:39.000000 iinfer-0.7.0/iinfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-29 11:29:39.000000 iinfer-0.7.0/iinfer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 11:29:40.516207 iinfer-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     2185 2024-04-06 23:22:57.000000 iinfer-0.7.0/setup.py
```

### Comparing `iinfer-0.6.9/LICENSE` & `iinfer-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/PKG-INFO` & `iinfer-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.6.9
+Version: 0.7.0
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.6.9/README.md` & `iinfer-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/app.py` & `iinfer-0.7.0/iinfer/app/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,712 +1,748 @@
 from iinfer import version
-from iinfer.app import common, client, gui, install, postprocess, redis, server
+from iinfer.app import common, client, gui, install, postprocess, redis, server, web
 from iinfer.app.postprocesses import cls_jadge, csv, det_clip, det_face_store, det_filter, det_jadge, httpreq, seg_bbox, seg_filter
 from pathlib import Path
 import argparse
 import argcomplete
 import cv2
 import os
 import sys
 import time
 
 
 def main(args_list:list=None):
-    return _main(args_list)[0]
+    app = IinferApp()
+    return app.main(args_list)[0]
 
-def _main(args_list:list=None):
-    """
-    コマンドライン引数を処理し、サーバーまたはクライアントを起動し、コマンドを実行する。
-    """
-    parser = argparse.ArgumentParser(prog='iinfer', description='This application generates modules to set up the application system.')
-    parser.add_argument('--version', help='show version infomation.', action='store_true')
-    parser.add_argument('--host', help='Setting the redis server host.', default=os.environ.get('REDIS_HOST', 'localhost'))
-    parser.add_argument('--port', help='Setting the redis server port.', type=int, default=int(os.environ.get('REDIS_PORT', '6379')))
-    parser.add_argument('--password', help='Setting the redis server password.', default=os.environ.get('REDIS_PASSWORD', 'password'))
-    parser.add_argument('--svname', help='Setting the service name of server.', type=str, default='server')
-    parser.add_argument('-u', '--useopt', help=f'Use options file.')
-    parser.add_argument('-s', '--saveopt', help=f'save options file. with --useopt option.', action='store_true')
-    parser.add_argument('-f', '--format', help='Setting the cmd format.', action='store_true')
-    parser.add_argument('-m', '--mode', help='Setting the boot mode.', choices=['redis', 'install', 'server', 'client', 'postprocess', 'gui'])
-    parser.add_argument('--data', help='Setting the data directory.', default=common.HOME_DIR / ".iinfer")
-    parser.add_argument('-n', '--name', help='Setting the cmd name.')
-    parser.add_argument('--timeout', help='Setting the cmd timeout.', type=int, default=60)
-    parser.add_argument('-c', '--cmd', help='Setting the cmd type.',
-                        choices=['redis', 'server', 'onnx', 'mmdet', 'mmseg', 'mmcls', 'mmpretrain', 'insightface', # install mode
-                                 'docker_run', 'docker_stop', # redis mode
-                                 'start', 'stop', # server or client or gui mode
-                                 'list' , # server mode
-                                 'deploy', 'deploy_list', 'undeploy', 'predict', 'predict_type_list', 'capture', # client mode
-                                 'file_list', 'file_mkdir', 'file_rmdir', 'file_download', 'file_upload', 'file_remove', # client mode
-                                 'cls_jadge', 'csv', 'det_clip', 'det_face_store', 'det_filter', 'det_jadge', 'httpreq', 'seg_bbox', 'seg_filter', # postprocess mode
-                                ])
-    parser.add_argument('-T','--use_track', help='Setting the multi object tracking enable for Object Detection.', action='store_true')
-    parser.add_argument('--model_img_width', help='Setting the cmd deploy model_img_width.', type=int)
-    parser.add_argument('--model_img_height', help='Setting the cmd deploy model_img_height.', type=int)
-    parser.add_argument('--model_file', help='Setting the cmd deploy model_file file.')
-    parser.add_argument('--model_conf_file', help='Setting the cmd deploy model_conf_file file.', action='append')
-    parser.add_argument('--predict_type', help='Setting the cmd deploy predict_type. If Custom, custom_predict_py must be specified.',
-                        choices=['Custom'] + list(common.BASE_MODELS.keys()))
-    parser.add_argument('--custom_predict_py', help='Setting the cmd deploy custom_predict.py file.')
-    parser.add_argument('--label_file', help='Setting the cmd deploy label_txt file.')
-    parser.add_argument('--color_file', help='Setting the cmd deploy color_txt file.')
-    parser.add_argument('--before_injection_type', help='Setting the cmd deploy before_injection_type.', action='append',
-                        choices=list(common.BASE_BREFORE_INJECTIONS.keys()))
-    parser.add_argument('--before_injection_conf', help='Setting the cmd deploy before_injection_conf file.')
-    parser.add_argument('--before_injection_py', help='Setting the cmd deploy before_injection_py file.', action='append')
-    parser.add_argument('--after_injection_type', help='Setting the cmd deploy after_injection_type file.', action='append',
-                        choices=list(common.BASE_AFTER_INJECTIONS.keys()))
-    parser.add_argument('--after_injection_conf', help='Setting the cmd deploy after_injection_conf file.')
-    parser.add_argument('--after_injection_py', help='Setting the cmd deploy after_injection_py file.', action='append')
-    parser.add_argument('--overwrite', help='Setting the cmd deploy overwrite save.', action='store_true')
-
-    parser.add_argument('--model_provider', help='Setting the cmd start model_provider.',
-                        choices=['CPUExecutionProvider','CUDAExecutionProvider','TensorrtExecutionProvider'], default='CPUExecutionProvider')
-    parser.add_argument('--gpuid', help='Setting the cmd start gpuid.', type=int, default=None)
-    parser.add_argument('-i', '--input_file', help='Setting the cmd input file.', default=None)
-    parser.add_argument('--output_image', help='Setting the cmd output image file.', default=None)
-    parser.add_argument('-o', '--output_json', help='Setting the cmd output json file.', default=None)
-    parser.add_argument('-a', '--output_json_append', help='Setting append the cmd output json file.', action='store_true')
-    parser.add_argument('-P', '--output_preview', help='Setting the output preview.', action='store_true')
-    parser.add_argument('--stdin', help='Setting the cmd stdin.', action='store_true')
-    parser.add_argument('--nodraw', help='Setting the cmd predict nodraw.', action='store_true')
-    parser.add_argument('--image_type', help='Setting the cmd predict image type.', choices=['bmp', 'png', 'jpeg', 'capture', 'output_json'], default='jpeg')
-    parser.add_argument('--wsl_name', help='WSL distribution name.')
-    parser.add_argument('--wsl_user', help='WSL distribution user.')
-    parser.add_argument('-d', '--capture_device', help='Setting the capture input device. device id, video file, rtsp url.', default='0')
-    parser.add_argument('--capture_frame_width', help='Setting the capture input frame width.', type=int, default=None)
-    parser.add_argument('--capture_frame_height', help='Setting the capture input frame height.', type=int, default=None)
-    parser.add_argument('--capture_fps', help='Setting the capture input fps.', type=int, default=1000)
-    parser.add_argument('--capture_count', help='Setting the capture count.', type=int, default=-1)
-
-    parser.add_argument('--svpath', help='Setting the server file path.', type=str, default='/')
-    parser.add_argument('--download_file', help='Setting the download file path.', type=str, default=None)
-    parser.add_argument('--upload_file', help='Setting the upload file path.', type=str, default=None)
-
-    parser.add_argument('--fileup_name', help='Setting the param name of file upload.', type=str, default='file')
-    parser.add_argument('--img_connectstr', help='Setting the postprocess img_connectstr.', type=str, default=None)
-    parser.add_argument('--json_connectstr', help='Setting the postprocess json_connectstr.', type=str, default=None)
-    parser.add_argument('--text_connectstr', help='Setting the postprocess text_connectstr.', type=str, default=None)
-
-    parser.add_argument('--out_headers', help='Setting the csv cmd out_headers in postprocess.', type=str, action='append')
-    parser.add_argument('--noheader', help='Setting the csv cmd noheader in postprocess.', action='store_true')
-    parser.add_argument('--output_csv', help='Setting the output_csv in postprocess.', type=str, default=None)
-
-    parser.add_argument('--clip_margin', help='Setting the postprocess clip_margin.', type=int, default=0)
-
-    parser.add_argument('--score_th', help='Setting the postprocess score_th.', type=float, default=0.0)
-    parser.add_argument('--width_th', help='Setting the postprocess width_th.', type=int, default=0)
-    parser.add_argument('--height_th', help='Setting the postprocess height_th.', type=int, default=0)
-    parser.add_argument('--classes', help='Setting the postprocess classes.', type=int, action='append')
-    parser.add_argument('--labels', help='Setting the postprocess labels.', type=str, action='append')
-    parser.add_argument('--ok_score_th', help='Setting the postprocess ok_score_th.', type=float, default=None)
-    parser.add_argument('--ok_classes', help='Setting the postprocess ok_classes.', type=int, action='append')
-    parser.add_argument('--ok_labels', help='Setting the postprocess ok_labels.', type=str, action='append')
-    parser.add_argument('--ng_score_th', help='Setting the postprocess ng_score_th.', type=float, default=None)
-    parser.add_argument('--ng_classes', help='Setting the postprocess ng_classes.', type=int, action='append')
-    parser.add_argument('--ng_labels', help='Setting the postprocess ng_labels.', type=str, action='append')
-    parser.add_argument('--ext_score_th', help='Setting the postprocess ext_score_th.', type=float, default=None)
-    parser.add_argument('--ext_classes', help='Setting the postprocess ext_classes.', type=int, action='append')
-    parser.add_argument('--ext_labels', help='Setting the postprocess ext_labels.', type=str, action='append')
-    parser.add_argument('--face_threshold', help='Setting the postprocess face_threshold.', type=float, default=0.0)
-
-    parser.add_argument('--del_segments', help='Setting the postprocess del_segments.', action='store_true')
-    parser.add_argument('--nodraw_bbox', help='Setting the postprocess nodraw_bbox.', action='store_true')
-    parser.add_argument('--nodraw_rbbox', help='Setting the postprocess nodraw_rbbox.', action='store_true')
-    parser.add_argument('--logits_th', help='Setting the postprocess logits_th.', type=float, default=0.0)
-    parser.add_argument('--del_logits', help='Setting the postprocess del_logits.', action='store_true')
-
-    parser.add_argument('--install_iinfer', help='Setting the install server install_iinfer.', type=str, default='iinfer')
-    parser.add_argument('--install_onnx', help='Setting the install server install_onnx.', action='store_true')
-    parser.add_argument('--install_mmdet', help='Setting the install server install_mmdet.', action='store_true')
-    parser.add_argument('--install_mmseg', help='Setting the install server install_mmseg.', action='store_true')
-    parser.add_argument('--install_mmcls', help='Setting the install server install_mmcls.', action='store_true')
-    parser.add_argument('--install_mmpretrain', help='Setting the install server install_mmpretrain.', action='store_true')
-    parser.add_argument('--install_insightface', help='Setting the install server install_insightface.', action='store_true')
-    parser.add_argument('--install_tag', help='Setting the install server install_tag.', type=str, default=None)
-    parser.add_argument('--install_use_gpu', help='Setting the install use gpu.', action='store_true')
-
-    argcomplete.autocomplete(parser)
-    if args_list is not None:
-        args = parser.parse_args(args=args_list)
-    else:
-        args = parser.parse_args()
-    args_dict = vars(args)
-    opt = common.loadopt(args.useopt)
-    host = common.getopt(opt, 'host', preval=args_dict, withset=True)
-    port = common.getopt(opt, 'port', preval=args_dict, withset=True)
-    password = common.getopt(opt, 'password', preval=args_dict, withset=True)
-    svname = common.getopt(opt, 'svname', preval=args_dict, withset=True)
-    format = common.getopt(opt, 'format', preval=args_dict, withset=True)
-    mode = common.getopt(opt, 'mode', preval=args_dict, withset=True)
-    data = common.getopt(opt, 'data', preval=args_dict, withset=True)
-    timeout = common.getopt(opt, 'timeout', preval=args_dict, withset=True)
-    name = common.getopt(opt, 'name', preval=args_dict, withset=True)
-    cmd = common.getopt(opt, 'cmd', preval=args_dict, withset=True)
-    model_img_width = common.getopt(opt, 'model_img_width', preval=args_dict, withset=True)
-    model_img_height = common.getopt(opt, 'model_img_height', preval=args_dict, withset=True)
-    model_file = common.getopt(opt, 'model_file', preval=args_dict, withset=True)
-    model_conf_file = common.getopt(opt, 'model_conf_file', preval=args_dict, withset=True)
-    predict_type = common.getopt(opt, 'predict_type', preval=args_dict, withset=True)
-    custom_predict_py = common.getopt(opt, 'custom_predict_py', preval=args_dict, withset=True)
-    label_file = common.getopt(opt, 'label_file', preval=args_dict, withset=True)
-    color_file = common.getopt(opt, 'color_file', preval=args_dict, withset=True)
-    before_injection_conf = common.getopt(opt, 'before_injection_conf', preval=args_dict, withset=True)
-    before_injection_type = common.getopt(opt, 'before_injection_type', preval=args_dict, withset=True)
-    before_injection_py = common.getopt(opt, 'before_injection_py', preval=args_dict, withset=True)
-    after_injection_conf = common.getopt(opt, 'after_injection_conf', preval=args_dict, withset=True)
-    after_injection_type = common.getopt(opt, 'after_injection_type', preval=args_dict, withset=True)
-    after_injection_py = common.getopt(opt, 'after_injection_py', preval=args_dict, withset=True)
-    overwrite = common.getopt(opt, 'overwrite', preval=args_dict, withset=True)
-
-    model_provider = common.getopt(opt, 'model_provider', preval=args_dict, withset=True)
-    gpuid = common.getopt(opt, 'gpuid', preval=args_dict, withset=True)
-    input_file = common.getopt(opt, 'input_file', preval=args_dict, withset=True)
-    output_image = common.getopt(opt, 'output_image', preval=args_dict, withset=True)
-    output_json = common.getopt(opt, 'output_json', preval=args_dict, withset=True)
-    output_json_append = common.getopt(opt, 'output_json_append', preval=args_dict, withset=True)
-    output_preview = common.getopt(opt, 'output_preview', preval=args_dict, withset=True)
-    stdin = common.getopt(opt, 'stdin', preval=args_dict, withset=True)
-    nodraw = common.getopt(opt, 'nodraw', preval=args_dict, withset=True)
-    image_type = common.getopt(opt, 'image_type', preval=args_dict, withset=True)
-    use_track = common.getopt(opt, 'use_track', preval=args_dict, withset=True)
-
-    wsl_name = common.getopt(opt, 'wsl_name', preval=args_dict, withset=True)
-    wsl_user = common.getopt(opt, 'wsl_user', preval=args_dict, withset=True)
-
-    capture_device = common.getopt(opt, 'capture_device', preval=args_dict, withset=True)
-    capture_frame_width = common.getopt(opt, 'capture_frame_width', preval=args_dict, withset=True)
-    capture_frame_height = common.getopt(opt, 'capture_frame_height', preval=args_dict, withset=True)
-    capture_fps = common.getopt(opt, 'capture_fps', preval=args_dict, withset=True)
-    capture_count = common.getopt(opt, 'capture_count', preval=args_dict, withset=True)
-
-    svpath = common.getopt(opt, 'svpath', preval=args_dict, withset=True)
-    download_file = common.getopt(opt, 'download_file', preval=args_dict, withset=True)
-    upload_file = common.getopt(opt, 'upload_file', preval=args_dict, withset=True)
-
-    json_connectstr = common.getopt(opt, 'json_connectstr', preval=args_dict, withset=True)
-    img_connectstr = common.getopt(opt, 'img_connectstr', preval=args_dict, withset=True)
-    text_connectstr = common.getopt(opt, 'text_connectstr', preval=args_dict, withset=True)
-    fileup_name = common.getopt(opt, 'fileup_name', preval=args_dict, withset=True)
-
-    out_headers = common.getopt(opt, 'out_headers', preval=args_dict, withset=True)
-    noheader = common.getopt(opt, 'noheader', preval=args_dict, withset=True)
-    output_csv = common.getopt(opt, 'output_csv', preval=args_dict, withset=True)
-
-    clip_margin = common.getopt(opt, 'clip_margin', preval=args_dict, withset=True)
-
-    score_th = common.getopt(opt, 'score_th', preval=args_dict, withset=True)
-    width_th = common.getopt(opt, 'width_th', preval=args_dict, withset=True)
-    height_th = common.getopt(opt, 'height_th', preval=args_dict, withset=True)
-    classes = common.getopt(opt, 'classes', preval=args_dict, withset=True)
-    labels = common.getopt(opt, 'labels', preval=args_dict, withset=True)
-
-    ok_score_th = common.getopt(opt, 'ok_score_th', preval=args_dict, withset=True)
-    ok_classes = common.getopt(opt, 'ok_classes', preval=args_dict, withset=True)
-    ok_labels = common.getopt(opt, 'ok_labels', preval=args_dict, withset=True)
-    ng_score_th = common.getopt(opt, 'ng_score_th', preval=args_dict, withset=True)
-    ng_classes = common.getopt(opt, 'ng_classes', preval=args_dict, withset=True)
-    ng_labels = common.getopt(opt, 'ng_labels', preval=args_dict, withset=True)
-    ext_score_th = common.getopt(opt, 'ext_score_th', preval=args_dict, withset=True)
-    ext_classes = common.getopt(opt, 'ext_classes', preval=args_dict, withset=True)
-    ext_labels = common.getopt(opt, 'ext_labels', preval=args_dict, withset=True)
-    face_threshold = common.getopt(opt, 'face_threshold', preval=args_dict, withset=True)
-
-    del_segments = common.getopt(opt, 'del_segments', preval=args_dict, withset=True)
-    nodraw_bbox = common.getopt(opt, 'nodraw_bbox', preval=args_dict, withset=True)
-    nodraw_rbbox = common.getopt(opt, 'nodraw_rbbox', preval=args_dict, withset=True)
-    logits_th = common.getopt(opt, 'logits_th', preval=args_dict, withset=True)
-    del_logits = common.getopt(opt, 'del_logits', preval=args_dict, withset=True)
-
-    install_iinfer = common.getopt(opt, 'install_iinfer', preval=args_dict, withset=True)
-    install_onnx = common.getopt(opt, 'install_onnx', preval=args_dict, withset=True)
-    install_mmdet = common.getopt(opt, 'install_mmdet', preval=args_dict, withset=True)
-    install_mmseg = common.getopt(opt, 'install_mmseg', preval=args_dict, withset=True)
-    install_mmcls = common.getopt(opt, 'install_mmcls', preval=args_dict, withset=True)
-    install_mmpretrain = common.getopt(opt, 'install_mmpretrain', preval=args_dict, withset=True)
-    install_insightface = common.getopt(opt, 'install_insightface', preval=args_dict, withset=True)
-    install_tag = common.getopt(opt, 'install_tag', preval=args_dict, withset=True)
-    install_use_gpu = common.getopt(opt, 'install_use_gpu', preval=args_dict, withset=True)
-
-    tm = time.time()
-    ret = {"success":f"Start command. {args}"}
-
-    if args.saveopt:
-        if args.useopt is None:
-            msg = {"warn":f"Please specify the --useopt option."}
-            common.print_format(msg, format, tm, output_json, output_json_append)
-            return 1, msg
-        common.saveopt(opt, args.useopt)
-        ret = {"success":f"Save options file. {args.useopt}"}
+class IinferApp:
+    def main(self, args_list:list=None, file_dict:dict=dict()):
+        """
+        コマンドライン引数を処理し、サーバーまたはクライアントを起動し、コマンドを実行する。
+        """
+        parser = argparse.ArgumentParser(prog='iinfer', description='This application generates modules to set up the application system.')
+        parser.add_argument('--version', help='show version infomation.', action='store_true')
+        parser.add_argument('--host', help='Setting the redis server host.', default=os.environ.get('REDIS_HOST', 'localhost'))
+        parser.add_argument('--port', help='Setting the redis server port.', type=int, default=int(os.environ.get('REDIS_PORT', '6379')))
+        parser.add_argument('--password', help='Setting the redis server password.', default=os.environ.get('REDIS_PASSWORD', 'password'))
+        parser.add_argument('--svname', help='Setting the service name of server.', type=str, default='server')
+        parser.add_argument('-u', '--useopt', help=f'Use options file.')
+        parser.add_argument('-s', '--saveopt', help=f'save options file. with --useopt option.', action='store_true')
+        parser.add_argument('-f', '--format', help='Setting the cmd format.', action='store_true')
+        parser.add_argument('-m', '--mode', help='Setting the boot mode.', choices=['redis', 'install', 'server', 'client', 'postprocess', 'gui', 'web'])
+        parser.add_argument('--data', help='Setting the data directory.', default=common.HOME_DIR / ".iinfer")
+        parser.add_argument('-n', '--name', help='Setting the cmd name.')
+        parser.add_argument('--timeout', help='Setting the cmd timeout.', type=int, default=60)
+        parser.add_argument('-c', '--cmd', help='Setting the cmd type.',
+                            choices=['redis', 'server', 'onnx', 'mmdet', 'mmseg', 'mmcls', 'mmpretrain', 'insightface', # install mode
+                                    'docker_run', 'docker_stop', # redis mode
+                                    'start', 'stop', # server or client or gui mode or web mode
+                                    'list' , # server mode
+                                    'deploy', 'deploy_list', 'undeploy', 'predict', 'predict_type_list', 'capture', # client mode
+                                    'file_list', 'file_mkdir', 'file_rmdir', 'file_download', 'file_upload', 'file_remove', # client mode
+                                    'cls_jadge', 'csv', 'det_clip', 'det_face_store', 'det_filter', 'det_jadge', 'httpreq', 'seg_bbox', 'seg_filter', # postprocess mode
+                                    ])
+        parser.add_argument('-T','--use_track', help='Setting the multi object tracking enable for Object Detection.', action='store_true')
+        parser.add_argument('--model_img_width', help='Setting the cmd deploy model_img_width.', type=int)
+        parser.add_argument('--model_img_height', help='Setting the cmd deploy model_img_height.', type=int)
+        parser.add_argument('--model_file', help='Setting the cmd deploy model_file file.')
+        parser.add_argument('--model_conf_file', help='Setting the cmd deploy model_conf_file file.', action='append')
+        parser.add_argument('--predict_type', help='Setting the cmd deploy predict_type. If Custom, custom_predict_py must be specified.',
+                            choices=['Custom'] + list(common.BASE_MODELS.keys()))
+        parser.add_argument('--custom_predict_py', help='Setting the cmd deploy custom_predict.py file.')
+        parser.add_argument('--label_file', help='Setting the cmd deploy label_txt file.')
+        parser.add_argument('--color_file', help='Setting the cmd deploy color_txt file.')
+        parser.add_argument('--before_injection_type', help='Setting the cmd deploy before_injection_type.', action='append',
+                            choices=list(common.BASE_BREFORE_INJECTIONS.keys()))
+        parser.add_argument('--before_injection_conf', help='Setting the cmd deploy before_injection_conf file.')
+        parser.add_argument('--before_injection_py', help='Setting the cmd deploy before_injection_py file.', action='append')
+        parser.add_argument('--after_injection_type', help='Setting the cmd deploy after_injection_type file.', action='append',
+                            choices=list(common.BASE_AFTER_INJECTIONS.keys()))
+        parser.add_argument('--after_injection_conf', help='Setting the cmd deploy after_injection_conf file.')
+        parser.add_argument('--after_injection_py', help='Setting the cmd deploy after_injection_py file.', action='append')
+        parser.add_argument('--overwrite', help='Setting the cmd deploy overwrite save.', action='store_true')
+
+        parser.add_argument('--model_provider', help='Setting the cmd start model_provider.',
+                            choices=['CPUExecutionProvider','CUDAExecutionProvider','TensorrtExecutionProvider'], default='CPUExecutionProvider')
+        parser.add_argument('--gpuid', help='Setting the cmd start gpuid.', type=int, default=None)
+        parser.add_argument('-i', '--input_file', help='Setting the cmd input file.', default=None)
+        parser.add_argument('--output_image', help='Setting the cmd output image file.', default=None)
+        parser.add_argument('-o', '--output_json', help='Setting the cmd output json file.', default=None)
+        parser.add_argument('-a', '--output_json_append', help='Setting append the cmd output json file.', action='store_true')
+        parser.add_argument('-P', '--output_preview', help='Setting the output preview.', action='store_true')
+        parser.add_argument('--stdin', help='Setting the cmd stdin.', action='store_true')
+        parser.add_argument('--nodraw', help='Setting the cmd predict nodraw.', action='store_true')
+        parser.add_argument('--image_type', help='Setting the cmd predict image type.', choices=['bmp', 'png', 'jpeg', 'capture', 'output_json'], default='jpeg')
+        parser.add_argument('--wsl_name', help='WSL distribution name.')
+        parser.add_argument('--wsl_user', help='WSL distribution user.')
+        parser.add_argument('-d', '--capture_device', help='Setting the capture input device. device id, video file, rtsp url.', default='0')
+        parser.add_argument('--capture_frame_width', help='Setting the capture input frame width.', type=int, default=None)
+        parser.add_argument('--capture_frame_height', help='Setting the capture input frame height.', type=int, default=None)
+        parser.add_argument('--capture_fps', help='Setting the capture input fps.', type=int, default=1000)
+        parser.add_argument('--capture_count', help='Setting the capture count.', type=int, default=-1)
+
+        parser.add_argument('--svpath', help='Setting the server file path.', type=str, default='/')
+        parser.add_argument('--download_file', help='Setting the download file path.', type=str, default=None)
+        parser.add_argument('--upload_file', help='Setting the upload file path.', type=str, default=None)
+
+        parser.add_argument('--fileup_name', help='Setting the param name of file upload.', type=str, default='file')
+        parser.add_argument('--img_connectstr', help='Setting the postprocess img_connectstr.', type=str, default=None)
+        parser.add_argument('--json_connectstr', help='Setting the postprocess json_connectstr.', type=str, default=None)
+        parser.add_argument('--text_connectstr', help='Setting the postprocess text_connectstr.', type=str, default=None)
+
+        parser.add_argument('--out_headers', help='Setting the csv cmd out_headers in postprocess.', type=str, action='append')
+        parser.add_argument('--noheader', help='Setting the csv cmd noheader in postprocess.', action='store_true')
+        parser.add_argument('--output_csv', help='Setting the output_csv in postprocess.', type=str, default=None)
+
+        parser.add_argument('--clip_margin', help='Setting the postprocess clip_margin.', type=int, default=0)
+
+        parser.add_argument('--score_th', help='Setting the postprocess score_th.', type=float, default=0.0)
+        parser.add_argument('--width_th', help='Setting the postprocess width_th.', type=int, default=0)
+        parser.add_argument('--height_th', help='Setting the postprocess height_th.', type=int, default=0)
+        parser.add_argument('--classes', help='Setting the postprocess classes.', type=int, action='append')
+        parser.add_argument('--labels', help='Setting the postprocess labels.', type=str, action='append')
+        parser.add_argument('--ok_score_th', help='Setting the postprocess ok_score_th.', type=float, default=None)
+        parser.add_argument('--ok_classes', help='Setting the postprocess ok_classes.', type=int, action='append')
+        parser.add_argument('--ok_labels', help='Setting the postprocess ok_labels.', type=str, action='append')
+        parser.add_argument('--ng_score_th', help='Setting the postprocess ng_score_th.', type=float, default=None)
+        parser.add_argument('--ng_classes', help='Setting the postprocess ng_classes.', type=int, action='append')
+        parser.add_argument('--ng_labels', help='Setting the postprocess ng_labels.', type=str, action='append')
+        parser.add_argument('--ext_score_th', help='Setting the postprocess ext_score_th.', type=float, default=None)
+        parser.add_argument('--ext_classes', help='Setting the postprocess ext_classes.', type=int, action='append')
+        parser.add_argument('--ext_labels', help='Setting the postprocess ext_labels.', type=str, action='append')
+        parser.add_argument('--face_threshold', help='Setting the postprocess face_threshold.', type=float, default=0.0)
+
+        parser.add_argument('--del_segments', help='Setting the postprocess del_segments.', action='store_true')
+        parser.add_argument('--nodraw_bbox', help='Setting the postprocess nodraw_bbox.', action='store_true')
+        parser.add_argument('--nodraw_rbbox', help='Setting the postprocess nodraw_rbbox.', action='store_true')
+        parser.add_argument('--logits_th', help='Setting the postprocess logits_th.', type=float, default=0.0)
+        parser.add_argument('--del_logits', help='Setting the postprocess del_logits.', action='store_true')
+
+        parser.add_argument('--install_iinfer', help='Setting the install server install_iinfer.', type=str, default='iinfer')
+        parser.add_argument('--install_onnx', help='Setting the install server install_onnx.', action='store_true')
+        parser.add_argument('--install_mmdet', help='Setting the install server install_mmdet.', action='store_true')
+        parser.add_argument('--install_mmseg', help='Setting the install server install_mmseg.', action='store_true')
+        parser.add_argument('--install_mmcls', help='Setting the install server install_mmcls.', action='store_true')
+        parser.add_argument('--install_mmpretrain', help='Setting the install server install_mmpretrain.', action='store_true')
+        parser.add_argument('--install_insightface', help='Setting the install server install_insightface.', action='store_true')
+        parser.add_argument('--install_tag', help='Setting the install server install_tag.', type=str, default=None)
+        parser.add_argument('--install_use_gpu', help='Setting the install use gpu.', action='store_true')
+
+        parser.add_argument('--allow_host', help='Setting the web mode allow_host.', type=str, default='0.0.0.0')
+        parser.add_argument('--listen_port', help='Setting the web mode listen_port.', type=int, default=8081)
+
+        argcomplete.autocomplete(parser)
+        if args_list is not None:
+            args = parser.parse_args(args=args_list)
+        else:
+            args = parser.parse_args()
+        args_dict = vars(args)
+        for key, val in file_dict.items():
+            args_dict[key] = val
+
+        opt = common.loadopt(args.useopt)
+        host = common.getopt(opt, 'host', preval=args_dict, withset=True)
+        port = common.getopt(opt, 'port', preval=args_dict, withset=True)
+        password = common.getopt(opt, 'password', preval=args_dict, withset=True)
+        svname = common.getopt(opt, 'svname', preval=args_dict, withset=True)
+        format = common.getopt(opt, 'format', preval=args_dict, withset=True)
+        mode = common.getopt(opt, 'mode', preval=args_dict, withset=True)
+        data = common.getopt(opt, 'data', preval=args_dict, withset=True)
+        timeout = common.getopt(opt, 'timeout', preval=args_dict, withset=True)
+        name = common.getopt(opt, 'name', preval=args_dict, withset=True)
+        cmd = common.getopt(opt, 'cmd', preval=args_dict, withset=True)
+        model_img_width = common.getopt(opt, 'model_img_width', preval=args_dict, withset=True)
+        model_img_height = common.getopt(opt, 'model_img_height', preval=args_dict, withset=True)
+        model_file = common.getopt(opt, 'model_file', preval=args_dict, withset=True)
+        model_conf_file = common.getopt(opt, 'model_conf_file', preval=args_dict, withset=True)
+        predict_type = common.getopt(opt, 'predict_type', preval=args_dict, withset=True)
+        custom_predict_py = common.getopt(opt, 'custom_predict_py', preval=args_dict, withset=True)
+        label_file = common.getopt(opt, 'label_file', preval=args_dict, withset=True)
+        color_file = common.getopt(opt, 'color_file', preval=args_dict, withset=True)
+        before_injection_conf = common.getopt(opt, 'before_injection_conf', preval=args_dict, withset=True)
+        before_injection_type = common.getopt(opt, 'before_injection_type', preval=args_dict, withset=True)
+        before_injection_py = common.getopt(opt, 'before_injection_py', preval=args_dict, withset=True)
+        after_injection_conf = common.getopt(opt, 'after_injection_conf', preval=args_dict, withset=True)
+        after_injection_type = common.getopt(opt, 'after_injection_type', preval=args_dict, withset=True)
+        after_injection_py = common.getopt(opt, 'after_injection_py', preval=args_dict, withset=True)
+        overwrite = common.getopt(opt, 'overwrite', preval=args_dict, withset=True)
+
+        model_provider = common.getopt(opt, 'model_provider', preval=args_dict, withset=True)
+        gpuid = common.getopt(opt, 'gpuid', preval=args_dict, withset=True)
+        input_file = common.getopt(opt, 'input_file', preval=args_dict, withset=True)
+        output_image = common.getopt(opt, 'output_image', preval=args_dict, withset=True)
+        output_json = common.getopt(opt, 'output_json', preval=args_dict, withset=True)
+        output_json_append = common.getopt(opt, 'output_json_append', preval=args_dict, withset=True)
+        output_preview = common.getopt(opt, 'output_preview', preval=args_dict, withset=True)
+        stdin = common.getopt(opt, 'stdin', preval=args_dict, withset=True)
+        nodraw = common.getopt(opt, 'nodraw', preval=args_dict, withset=True)
+        image_type = common.getopt(opt, 'image_type', preval=args_dict, withset=True)
+        use_track = common.getopt(opt, 'use_track', preval=args_dict, withset=True)
+
+        wsl_name = common.getopt(opt, 'wsl_name', preval=args_dict, withset=True)
+        wsl_user = common.getopt(opt, 'wsl_user', preval=args_dict, withset=True)
+
+        capture_device = common.getopt(opt, 'capture_device', preval=args_dict, withset=True)
+        capture_frame_width = common.getopt(opt, 'capture_frame_width', preval=args_dict, withset=True)
+        capture_frame_height = common.getopt(opt, 'capture_frame_height', preval=args_dict, withset=True)
+        capture_fps = common.getopt(opt, 'capture_fps', preval=args_dict, withset=True)
+        capture_count = common.getopt(opt, 'capture_count', preval=args_dict, withset=True)
+
+        svpath = common.getopt(opt, 'svpath', preval=args_dict, withset=True)
+        download_file = common.getopt(opt, 'download_file', preval=args_dict, withset=True)
+        upload_file = common.getopt(opt, 'upload_file', preval=args_dict, withset=True)
+
+        json_connectstr = common.getopt(opt, 'json_connectstr', preval=args_dict, withset=True)
+        img_connectstr = common.getopt(opt, 'img_connectstr', preval=args_dict, withset=True)
+        text_connectstr = common.getopt(opt, 'text_connectstr', preval=args_dict, withset=True)
+        fileup_name = common.getopt(opt, 'fileup_name', preval=args_dict, withset=True)
+
+        out_headers = common.getopt(opt, 'out_headers', preval=args_dict, withset=True)
+        noheader = common.getopt(opt, 'noheader', preval=args_dict, withset=True)
+        output_csv = common.getopt(opt, 'output_csv', preval=args_dict, withset=True)
+
+        clip_margin = common.getopt(opt, 'clip_margin', preval=args_dict, withset=True)
+
+        score_th = common.getopt(opt, 'score_th', preval=args_dict, withset=True)
+        width_th = common.getopt(opt, 'width_th', preval=args_dict, withset=True)
+        height_th = common.getopt(opt, 'height_th', preval=args_dict, withset=True)
+        classes = common.getopt(opt, 'classes', preval=args_dict, withset=True)
+        labels = common.getopt(opt, 'labels', preval=args_dict, withset=True)
+
+        ok_score_th = common.getopt(opt, 'ok_score_th', preval=args_dict, withset=True)
+        ok_classes = common.getopt(opt, 'ok_classes', preval=args_dict, withset=True)
+        ok_labels = common.getopt(opt, 'ok_labels', preval=args_dict, withset=True)
+        ng_score_th = common.getopt(opt, 'ng_score_th', preval=args_dict, withset=True)
+        ng_classes = common.getopt(opt, 'ng_classes', preval=args_dict, withset=True)
+        ng_labels = common.getopt(opt, 'ng_labels', preval=args_dict, withset=True)
+        ext_score_th = common.getopt(opt, 'ext_score_th', preval=args_dict, withset=True)
+        ext_classes = common.getopt(opt, 'ext_classes', preval=args_dict, withset=True)
+        ext_labels = common.getopt(opt, 'ext_labels', preval=args_dict, withset=True)
+        face_threshold = common.getopt(opt, 'face_threshold', preval=args_dict, withset=True)
+
+        del_segments = common.getopt(opt, 'del_segments', preval=args_dict, withset=True)
+        nodraw_bbox = common.getopt(opt, 'nodraw_bbox', preval=args_dict, withset=True)
+        nodraw_rbbox = common.getopt(opt, 'nodraw_rbbox', preval=args_dict, withset=True)
+        logits_th = common.getopt(opt, 'logits_th', preval=args_dict, withset=True)
+        del_logits = common.getopt(opt, 'del_logits', preval=args_dict, withset=True)
+
+        install_iinfer = common.getopt(opt, 'install_iinfer', preval=args_dict, withset=True)
+        install_onnx = common.getopt(opt, 'install_onnx', preval=args_dict, withset=True)
+        install_mmdet = common.getopt(opt, 'install_mmdet', preval=args_dict, withset=True)
+        install_mmseg = common.getopt(opt, 'install_mmseg', preval=args_dict, withset=True)
+        install_mmcls = common.getopt(opt, 'install_mmcls', preval=args_dict, withset=True)
+        install_mmpretrain = common.getopt(opt, 'install_mmpretrain', preval=args_dict, withset=True)
+        install_insightface = common.getopt(opt, 'install_insightface', preval=args_dict, withset=True)
+        install_tag = common.getopt(opt, 'install_tag', preval=args_dict, withset=True)
+        install_use_gpu = common.getopt(opt, 'install_use_gpu', preval=args_dict, withset=True)
+
+        allow_host = common.getopt(opt, 'allow_host', preval=args_dict, withset=True)
+        listen_port = common.getopt(opt, 'listen_port', preval=args_dict, withset=True)
+
+        tm = time.time()
+        ret = {"success":f"Start command. {args}"}
+
+        if args.saveopt:
+            if args.useopt is None:
+                msg = {"warn":f"Please specify the --useopt option."}
+                common.print_format(msg, format, tm, output_json, output_json_append)
+                return 1, msg
+            common.saveopt(opt, args.useopt)
+            ret = {"success":f"Save options file. {args.useopt}"}
 
-    if args.version:
-        common.print_format(version.__description__, False, tm, None, False)
-        return 0, version.__description__
-    elif mode == 'server':
-        logger, _ = common.load_config(mode)
-        if cmd == 'start':
-            if data is None:
-                msg = {"warn":f"Please specify the --data option."}
+        if args.version:
+            common.print_format(version.__description__, False, tm, None, False)
+            return 0, version.__description__
+        elif mode == 'server':
+            logger, _ = common.load_config(mode)
+            if cmd == 'start':
+                if data is None:
+                    msg = {"warn":f"Please specify the --data option."}
+                    common.print_format(msg, format, tm, output_json, output_json_append)
+                    return 1, msg
+                if svname is None:
+                    msg = {"warn":f"Please specify the --svname option."}
+                    common.print_format(msg, format, tm, output_json, output_json_append)
+                    return 1, msg
+                self.sv = server.Server(Path(data), logger, redis_host=host, redis_port=port, redis_password=password, svname=svname)
+                self.sv.start_server()
+            elif cmd == 'stop':
+                if svname is None:
+                    msg = {"warn":f"Please specify the --svname option."}
+                    common.print_format(msg, format, tm, output_json, output_json_append)
+                    return 1, msg
+                cl = client.Client(logger, redis_host=host, redis_port=port, redis_password=password, svname=svname)
+                ret = cl.stop_server(timeout=timeout)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+            elif cmd == 'list':
+                self.sv = server.Server(Path(data), logger, redis_host=host, redis_port=port, redis_password=password, svname='server') # list取得なのでデフォルトのsvnameを指定
+                ret = self.sv.list_server()
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+            else:
+                msg = {"warn":f"Unkown command."}
                 common.print_format(msg, format, tm, output_json, output_json_append)
                 return 1, msg
-            if svname is None:
-                msg = {"warn":f"Please specify the --svname option."}
+
+        elif mode == 'gui':
+            logger, _ = common.load_config(mode)
+            if cmd == 'start':
+                if data is None:
+                    msg = {"warn":f"Please specify the --data option."}
+                    common.print_format(msg, format, tm, output_json, output_json_append)
+                    return 1, msg
+                self.web = gui.Gui(logger, Path(data))
+                self.web.start()
+                msg = {"success":"eel web complate."}
+                common.print_format(msg, format, tm, output_json, output_json_append)
+                return 0, msg
+            else:
+                msg = {"warn":f"Unkown command."}
+                common.print_format(msg, format, tm, output_json, output_json_append)
+                return 1, msg
+
+        elif mode == 'web':
+            logger, _ = common.load_config(mode)
+            if cmd == 'start':
+                if data is None:
+                    msg = {"warn":f"Please specify the --data option."}
+                    common.print_format(msg, format, tm, output_json, output_json_append)
+                    return 1, msg
+                self.web = web.Web(logger, Path(data))
+                self.web.start(allow_host, listen_port)
+                msg = {"success":"web complate."}
+                common.print_format(msg, format, tm, output_json, output_json_append)
+                return 0, msg
+            elif cmd == 'stop':
+                self.web = web.Web(logger, Path(data))
+                self.web.stop()
+                msg = {"success":"web complate."}
+                common.print_format(msg, format, tm, output_json, output_json_append)
+                return 0, msg
+            else:
+                msg = {"warn":f"Unkown command."}
                 common.print_format(msg, format, tm, output_json, output_json_append)
                 return 1, msg
-            sv = server.Server(Path(data), logger, redis_host=host, redis_port=port, redis_password=password, svname=svname)
-            sv.start_server()
-        elif cmd == 'stop':
+            
+        elif mode == 'client':
+            logger, _ = common.load_config(mode)
             if svname is None:
                 msg = {"warn":f"Please specify the --svname option."}
                 common.print_format(msg, format, tm, output_json, output_json_append)
                 return 1, msg
-            cl = client.Client(logger, redis_host=host, redis_port=port, redis_password=password, svname=svname)
-            ret = cl.stop_server(timeout=timeout)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-        elif cmd == 'list':
-            sv = server.Server(Path(data), logger, redis_host=host, redis_port=port, redis_password=password, svname='server') # list取得なのでデフォルトのsvnameを指定
-            ret = sv.list_server()
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-        else:
-            msg = {"warn":f"Unkown command."}
-            common.print_format(msg, format, tm, output_json, output_json_append)
-            return 1, msg
+            self.cl = client.Client(logger, redis_host=host, redis_port=port, redis_password=password, svname=svname)
+            if cmd == 'deploy':
+                model_file = Path(model_file) if model_file is not None else None
+                if model_conf_file is not None:
+                    model_conf_file = [Path(f) for f in model_conf_file if f is not None and f != '']
+                if before_injection_py is not None:
+                    before_injection_py = [Path(f) for f in before_injection_py if f is not None and f != '']
+                if after_injection_py is not None:
+                    after_injection_py = [Path(f) for f in after_injection_py if f is not None and f != '']
+                custom_predict_py = Path(custom_predict_py) if custom_predict_py is not None else None
+                label_file = Path(label_file) if label_file is not None else None
+                color_file = Path(color_file) if color_file is not None else None
+                before_injection_conf = Path(before_injection_conf) if before_injection_conf is not None else None
+                after_injection_conf = Path(after_injection_conf) if after_injection_conf is not None else None
+                ret = self.cl.deploy(name, model_img_width, model_img_height, model_file, model_conf_file, predict_type,
+                                custom_predict_py, label_file=label_file, color_file=color_file,
+                                before_injection_conf=before_injection_conf, before_injection_type=before_injection_type, before_injection_py=before_injection_py,
+                                after_injection_conf=after_injection_conf, after_injection_type=after_injection_type, after_injection_py=after_injection_py,
+                                overwrite=overwrite, timeout=timeout)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'deploy_list':
+                ret = self.cl.deploy_list(timeout=timeout)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'undeploy':
+                ret = self.cl.undeploy(name, timeout=timeout)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'start':
+                ret = self.cl.start(name, model_provider=model_provider, use_track=use_track, gpuid=gpuid, timeout=timeout)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'stop':
+                ret = self.cl.stop(name, timeout=timeout)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'predict':
+                try:
+                    if input_file is not None:
+                        ret = self.cl.predict(name, image_file=input_file, image_type=image_type,
+                                                output_image_file=output_image, output_preview=output_preview,
+                                                nodraw=nodraw, timeout=timeout)
+                        if type(ret) is list:
+                            for r in ret:
+                                common.print_format(r, format, tm, output_json, output_json_append)
+                                tm = time.time()
+                                output_json_append = True
+                        else:
+                            common.print_format(ret, format, tm, output_json, output_json_append)
+                    elif stdin:
+                        if image_type is None:
+                            msg = {"warn":f"Please specify the --image_type option."}
+                            common.print_format(msg, format, tm, output_json, output_json_append)
+                            return 1, msg
+                        if image_type == 'capture':
+                            for line in sys.stdin:
+                                ret = self.cl.predict(name, image=line, image_type=image_type, output_image_file=output_image, output_preview=output_preview, nodraw=nodraw, timeout=timeout)
+                                common.print_format(ret, format, tm, output_json, output_json_append)
+                                tm = time.time()
+                                output_json_append = True
+                        else:
+                            ret = self.cl.predict(name, image=sys.stdin.buffer.read(), image_type=image_type, output_image_file=output_image, output_preview=output_preview, nodraw=nodraw, timeout=timeout)
+                            common.print_format(ret, format, tm, output_json, output_json_append)
+                            tm = time.time()
+                    else:
+                        msg = {"warn":f"Image file or stdin is empty."}
+                        common.print_format(msg, format, tm, output_json, output_json_append)
+                        return 1, msg
+                finally:
+                    try:
+                        cv2.destroyWindow('preview')
+                    except:
+                        pass
+
+            elif cmd == 'file_list':
+                ret = self.cl.file_list(svpath, timeout=timeout)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+            
+            elif cmd == 'file_mkdir':
+                ret = self.cl.file_mkdir(svpath, timeout=timeout)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+            
+            elif cmd == 'file_rmdir':
+                ret = self.cl.file_rmdir(svpath, timeout=timeout)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+            
+            elif cmd == 'file_download':
+                download_file = Path(download_file) if download_file is not None else None
+                ret = self.cl.file_download(svpath, download_file, timeout=timeout)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+            
+            elif cmd == 'file_upload':
+                upload_file = Path(upload_file) if upload_file is not None else None
+                ret = self.cl.file_upload(svpath, upload_file, timeout=timeout)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'file_remove':
+                ret = self.cl.file_remove(svpath, timeout=timeout)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'predict_type_list':
+                type_list = [dict(predict_type=key, site=val['site'], image_width=val['image_width'], image_height=val['image_height'],
+                                required_model_conf=val['required_model_conf'], required_model_weight=val['required_model_weight']) for key,val in common.BASE_MODELS.items()]
+                type_list.append(dict(predict_type='Custom', site='Custom', image_width=None, image_height=None))
+                ret = type_list
+                common.print_format(ret, format, tm, output_json, output_json_append)
+
+            elif cmd == 'capture':
+                count = 0
+                append = False
+                try:
+                    for t,b64,h,w,c,fn in self.cl.capture(capture_device=capture_device, image_type=image_type,
+                                        capture_frame_width=capture_frame_width, capture_frame_height=capture_frame_height, capture_fps=capture_fps,
+                                        output_preview=output_preview):
+                        ret = f"{t},"+b64+f",{h},{w},{c},{fn}"
+                        if output_csv is not None:
+                            with open(output_csv, 'a' if append else 'w', encoding="utf-8") as f:
+                                print(ret, file=f)
+                                append = True
+                        else: common.print_format(ret, False, tm, None, False)
+                        tm = time.time()
+                        count += 1
+                        if capture_count > 0 and count >= capture_count:
+                            break
+                finally:
+                    try:
+                        cv2.destroyWindow('preview')
+                    except:
+                        pass
 
-    elif mode == 'gui':
-        logger, _ = common.load_config(mode)
-        if cmd == 'start':
-            if data is None:
-                msg = {"warn":f"Please specify the --data option."}
+            else:
+                msg = {"warn":f"Unkown command."}
                 common.print_format(msg, format, tm, output_json, output_json_append)
                 return 1, msg
-            web = gui.Web(logger, Path(data))
-            web.start()
-            msg = {"success":"eel web complate."}
-            common.print_format(msg, format, tm, output_json, output_json_append)
-            return 0, msg
-        else:
-            msg = {"warn":f"Unkown command."}
-            common.print_format(msg, format, tm, output_json, output_json_append)
-            return 1, msg
 
-    elif mode == 'client':
-        logger, _ = common.load_config(mode)
-        if svname is None:
-            msg = {"warn":f"Please specify the --svname option."}
-            common.print_format(msg, format, tm, output_json, output_json_append)
-            return 1, msg
-        cl = client.Client(logger, redis_host=host, redis_port=port, redis_password=password, svname=svname)
-        if cmd == 'deploy':
-            model_file = Path(model_file) if model_file is not None else None
-            if model_conf_file is not None:
-                model_conf_file = [Path(f) for f in model_conf_file if f is not None and f != '']
-            if before_injection_py is not None:
-                before_injection_py = [Path(f) for f in before_injection_py if f is not None and f != '']
-            if after_injection_py is not None:
-                after_injection_py = [Path(f) for f in after_injection_py if f is not None and f != '']
-            custom_predict_py = Path(custom_predict_py) if custom_predict_py is not None else None
-            label_file = Path(label_file) if label_file is not None else None
-            color_file = Path(color_file) if color_file is not None else None
-            before_injection_conf = Path(before_injection_conf) if before_injection_conf is not None else None
-            after_injection_conf = Path(after_injection_conf) if after_injection_conf is not None else None
-            ret = cl.deploy(name, model_img_width, model_img_height, model_file, model_conf_file, predict_type,
-                            custom_predict_py, label_file=label_file, color_file=color_file,
-                            before_injection_conf=before_injection_conf, before_injection_type=before_injection_type, before_injection_py=before_injection_py,
-                            after_injection_conf=after_injection_conf, after_injection_type=after_injection_type, after_injection_py=after_injection_py,
-                            overwrite=overwrite, timeout=timeout)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-
-        elif cmd == 'deploy_list':
-            ret = cl.deploy_list(timeout=timeout)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-
-        elif cmd == 'undeploy':
-            ret = cl.undeploy(name, timeout=timeout)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-
-        elif cmd == 'start':
-            ret = cl.start(name, model_provider=model_provider, use_track=use_track, gpuid=gpuid, timeout=timeout)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-
-        elif cmd == 'stop':
-            ret = cl.stop(name, timeout=timeout)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
+        elif mode == 'postprocess':
+            logger, _ = common.load_config(mode)
+            def _to_proc(f, proc:postprocess.Postprocess, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, output_json, output_json_append, output_csv=None):
+                try:
+                    for line in f:
+                        line = line.rstrip()
+                        if line == "":
+                            continue
+                        try:
+                            json_session, img_session, text_session = proc.create_session(json_connectstr, img_connectstr, text_connectstr)
+                            ret = proc.postprocess(json_session, img_session, text_session, line, timeout=timeout)
+                            if output_csv is not None:
+                                with open(output_csv, 'a' if output_json_append else 'w', encoding="utf-8") as f:
+                                    txt = common.print_format(ret, format, tm, output_json, output_json_append, stdout=False)
+                                    print(txt.strip(), file=f)
+                            else: common.print_format(ret, format, tm, output_json, output_json_append)
+                        except Exception as e:
+                            msg = {"warn":f"Invalid input. {e}"}
+                            common.print_format(msg, format, tm, output_json, output_json_append)
+                            ret = msg
+                        tm = time.time()
+                        output_json_append = True
+                    return ret
+                finally:
+                    try:
+                        cv2.destroyWindow('preview')
+                    except:
+                        pass
 
-        elif cmd == 'predict':
-            try:
+            def _exec_proc(input_file, stdin, proc:postprocess.Postprocess, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, output_json, output_json_append, output_csv=None):
                 if input_file is not None:
-                    ret = cl.predict(name, image_file=Path(input_file), image_type=image_type, output_image_file=output_image, output_preview=output_preview, nodraw=nodraw, timeout=timeout)
-                    if type(ret) is list:
-                        for r in ret:
-                            common.print_format(r, format, tm, output_json, output_json_append)
-                            tm = time.time()
-                            output_json_append = True
-                    else:
-                        common.print_format(ret, format, tm, output_json, output_json_append)
+                    with open(input_file, 'r', encoding="UTF-8") as f:
+                        ret = _to_proc(f.readlines(), proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append, output_csv=output_csv)
                 elif stdin:
-                    if image_type is None:
-                        msg = {"warn":f"Please specify the --image_type option."}
-                        common.print_format(msg, format, tm, output_json, output_json_append)
-                        return 1, msg
-                    if image_type == 'capture':
-                        for line in sys.stdin:
-                            ret = cl.predict(name, image=line, image_type=image_type, output_image_file=output_image, output_preview=output_preview, nodraw=nodraw, timeout=timeout)
-                            common.print_format(ret, format, tm, output_json, output_json_append)
-                            tm = time.time()
-                            output_json_append = True
-                    else:
-                        ret = cl.predict(name, image=sys.stdin.buffer.read(), image_type=image_type, output_image_file=output_image, output_preview=output_preview, nodraw=nodraw, timeout=timeout)
-                        common.print_format(ret, format, tm, output_json, output_json_append)
-                        tm = time.time()
+                    ret = _to_proc(sys.stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append, output_csv=output_csv)
                 else:
                     msg = {"warn":f"Image file or stdin is empty."}
                     common.print_format(msg, format, tm, output_json, output_json_append)
                     return 1, msg
-            finally:
+                return 0, ret
+
+            if cmd == 'cls_jadge':
                 try:
-                    cv2.destroyWindow('preview')
-                except:
-                    pass
-
-        elif cmd == 'file_list':
-            ret = cl.file_list(svpath, timeout=timeout)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-        
-        elif cmd == 'file_mkdir':
-            ret = cl.file_mkdir(svpath, timeout=timeout)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-        
-        elif cmd == 'file_rmdir':
-            ret = cl.file_rmdir(svpath, timeout=timeout)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-        
-        elif cmd == 'file_download':
-            download_file = Path(download_file) if download_file is not None else None
-            ret = cl.file_download(svpath, download_file, timeout=timeout)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-        
-        elif cmd == 'file_upload':
-            upload_file = Path(upload_file) if upload_file is not None else None
-            ret = cl.file_upload(svpath, upload_file, timeout=timeout)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-
-        elif cmd == 'file_remove':
-            ret = cl.file_remove(svpath, timeout=timeout)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-
-        elif cmd == 'predict_type_list':
-            type_list = [dict(predict_type=key, site=val['site'], image_width=val['image_width'], image_height=val['image_height'],
-                              required_model_conf=val['required_model_conf'], required_model_weight=val['required_model_weight']) for key,val in common.BASE_MODELS.items()]
-            type_list.append(dict(predict_type='Custom', site='Custom', image_width=None, image_height=None))
-            ret = type_list
-            common.print_format(ret, format, tm, output_json, output_json_append)
-
-        elif cmd == 'capture':
-            count = 0
-            append = False
-            try:
-                for t,b64,h,w,c,fn in cl.capture(capture_device=capture_device, image_type=image_type,
-                                    capture_frame_width=capture_frame_width, capture_frame_height=capture_frame_height, capture_fps=capture_fps,
-                                    output_preview=output_preview):
-                    ret = f"{t},"+b64+f",{h},{w},{c},{fn}"
-                    if output_csv is not None:
-                        with open(output_csv, 'a' if append else 'w', encoding="utf-8") as f:
-                            print(ret, file=f)
-                            append = True
-                    else: common.print_format(ret, False, tm, None, False)
-                    tm = time.time()
-                    count += 1
-                    if capture_count > 0 and count >= capture_count:
-                        break
-            finally:
-                try:
-                    cv2.destroyWindow('preview')
-                except:
-                    pass
+                    proc = cls_jadge.ClaJadge(logger, ok_score_th=ok_score_th, ok_classes=ok_classes, ok_labels=ok_labels,
+                                            ng_score_th=ng_score_th, ng_classes=ng_classes, ng_labels=ng_labels,
+                                            ext_score_th=ext_score_th, ext_classes=ext_classes, ext_labels=ext_labels,
+                                            nodraw=nodraw, output_preview=output_preview)
+                except Exception as e:
+                    common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
+                    return 1, msg
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+                if code != 0:
+                    return code, ret
 
-        else:
-            msg = {"warn":f"Unkown command."}
-            common.print_format(msg, format, tm, output_json, output_json_append)
-            return 1, msg
+            elif cmd == 'csv':
+                try:
+                    proc = csv.Csv(logger, out_headers=out_headers, noheader=noheader)
+                except Exception as e:
+                    common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
+                    return 1, msg
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, None, False, output_csv=output_csv)
+                if code != 0:
+                    return code, ret
 
-    elif mode == 'postprocess':
-        logger, _ = common.load_config(mode)
-        def _to_proc(f, proc:postprocess.Postprocess, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, output_json, output_json_append, output_csv=None):
-            try:
-                for line in f:
-                    line = line.rstrip()
-                    if line == "":
-                        continue
-                    try:
-                        json_session, img_session, text_session = proc.create_session(json_connectstr, img_connectstr, text_connectstr)
-                        ret = proc.postprocess(json_session, img_session, text_session, line, timeout=timeout)
-                        if output_csv is not None:
-                            with open(output_csv, 'a' if output_json_append else 'w', encoding="utf-8") as f:
-                                txt = common.print_format(ret, format, tm, output_json, output_json_append, stdout=False)
-                                print(txt.strip(), file=f)
-                        else: common.print_format(ret, format, tm, output_json, output_json_append)
-                    except Exception as e:
-                        msg = {"warn":f"Invalid input. {e}"}
-                        common.print_format(msg, format, tm, output_json, output_json_append)
-                        ret = msg
-                    tm = time.time()
-                    output_json_append = True
-                return ret
-            finally:
-                try:
-                    cv2.destroyWindow('preview')
-                except:
-                    pass
-
-        def _exec_proc(input_file, stdin, proc:postprocess.Postprocess, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, output_json, output_json_append, output_csv=None):
-            if input_file is not None:
-                with open(input_file, 'r', encoding="UTF-8") as f:
-                    ret = _to_proc(f.readlines(), proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append, output_csv=output_csv)
-            elif stdin:
-                ret = _to_proc(sys.stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append, output_csv=output_csv)
-            else:
-                msg = {"warn":f"Image file or stdin is empty."}
-                common.print_format(msg, format, tm, output_json, output_json_append)
-                return 1, msg
-            return 0, ret
+            elif cmd == 'det_clip':
+                try:
+                    proc = det_clip.DetClip(logger, image_type=image_type, clip_margin=clip_margin)
+                except Exception as e:
+                    common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
+                    return 1, msg
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, None, False, output_csv=output_csv)
+                if code != 0:
+                    return code, ret
 
-        if cmd == 'cls_jadge':
-            try:
-                proc = cls_jadge.ClaJadge(logger, ok_score_th=ok_score_th, ok_classes=ok_classes, ok_labels=ok_labels,
-                                        ng_score_th=ng_score_th, ng_classes=ng_classes, ng_labels=ng_labels,
-                                        ext_score_th=ext_score_th, ext_classes=ext_classes, ext_labels=ext_labels,
-                                        nodraw=nodraw, output_preview=output_preview)
-            except Exception as e:
-                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
-                return 1, msg
-            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
-            if code != 0:
-                return code, ret
-
-        elif cmd == 'csv':
-            try:
-                proc = csv.Csv(logger, out_headers=out_headers, noheader=noheader)
-            except Exception as e:
-                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
-                return 1, msg
-            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, None, False, output_csv=output_csv)
-            if code != 0:
-                return code, ret
-
-        elif cmd == 'det_clip':
-            try:
-                proc = det_clip.DetClip(logger, image_type=image_type, clip_margin=clip_margin)
-            except Exception as e:
-                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
-                return 1, msg
-            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, None, False, output_csv=output_csv)
-            if code != 0:
-                return code, ret
-
-        elif cmd == 'det_face_store':
-            try:
-                proc = det_face_store.DetFaceStore(logger, face_threshold=face_threshold, image_type=image_type, clip_margin=clip_margin)
-            except Exception as e:
-                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
-                return 1, msg
-            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, output_json, output_json_append)
-            if code != 0:
-                return code, ret
-
-        elif cmd == 'det_filter':
-            try:
-                proc = det_filter.DetFilter(logger, score_th=score_th, width_th=width_th, height_th=height_th, classes=classes, labels=labels, nodraw=nodraw, output_preview=output_preview)
-            except Exception as e:
-                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
-                return 1, msg
-            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
-            if code != 0:
-                return code, ret
-
-        elif cmd == 'det_jadge':
-            try:
-                proc = det_jadge.DetJadge(logger, ok_score_th=ok_score_th, ok_classes=ok_classes, ok_labels=ok_labels,
-                                        ng_score_th=ng_score_th, ng_classes=ng_classes, ng_labels=ng_labels,
-                                        ext_score_th=ext_score_th, ext_classes=ext_classes, ext_labels=ext_labels,
-                                        nodraw=nodraw, output_preview=output_preview)
-            except Exception as e:
-                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
-                return 1, msg
-            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
-            if code != 0:
-                return code, ret
-
-        elif cmd == 'httpreq':
-            try:
-                proc = httpreq.Httpreq(logger, fileup_name=fileup_name)
-            except Exception as e:
-                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
-                return 1, msg
-            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, None, False)
-            if code != 0:
-                return code, ret
-
-        elif cmd == 'seg_bbox':
-            try:
-                proc = seg_bbox.SegBBox(logger, del_segments=del_segments, nodraw=nodraw, nodraw_bbox=nodraw_bbox, nodraw_rbbox=nodraw_rbbox,
-                                        output_preview=output_preview)
-            except Exception as e:
-                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
-                return 1, msg
-            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
-            if code != 0:
-                return code, ret
-
-        elif cmd == 'seg_filter':
-            try:
-                proc = seg_filter.SegFilter(logger, logits_th=logits_th, classes=classes, labels=labels, nodraw=nodraw, del_logits=del_logits)
-            except Exception as e:
-                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
-                return 1, msg
-            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
-            if code != 0:
-                return code, ret
+            elif cmd == 'det_face_store':
+                try:
+                    proc = det_face_store.DetFaceStore(logger, face_threshold=face_threshold, image_type=image_type, clip_margin=clip_margin)
+                except Exception as e:
+                    common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
+                    return 1, msg
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, output_json, output_json_append)
+                if code != 0:
+                    return code, ret
 
-        else:
-            msg = {"warn":f"Unkown command."}
-            common.print_format(msg, format, tm, output_json, output_json_append)
-            return 1, msg
+            elif cmd == 'det_filter':
+                try:
+                    proc = det_filter.DetFilter(logger, score_th=score_th, width_th=width_th, height_th=height_th, classes=classes, labels=labels, nodraw=nodraw, output_preview=output_preview)
+                except Exception as e:
+                    common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
+                    return 1, msg
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+                if code != 0:
+                    return code, ret
 
-    elif mode == 'redis':
-        logger, _ = common.load_config(mode)
-        rd = redis.Redis(logger=logger, wsl_name=wsl_name, wsl_user=wsl_user)
-        if cmd == 'docker_run':
-            ret = rd.docker_run(port, password)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-
-        elif cmd == 'docker_stop':
-            ret = rd.docker_stop()
-            common.print_format(ret, format, tm, output_json, output_json_append)
+            elif cmd == 'det_jadge':
+                try:
+                    proc = det_jadge.DetJadge(logger, ok_score_th=ok_score_th, ok_classes=ok_classes, ok_labels=ok_labels,
+                                            ng_score_th=ng_score_th, ng_classes=ng_classes, ng_labels=ng_labels,
+                                            ext_score_th=ext_score_th, ext_classes=ext_classes, ext_labels=ext_labels,
+                                            nodraw=nodraw, output_preview=output_preview)
+                except Exception as e:
+                    common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
+                    return 1, msg
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+                if code != 0:
+                    return code, ret
 
-        else:
-            msg = {"warn":f"Unkown command."}
-            common.print_format(msg, format, tm, output_json, output_json_append)
-            return 1, msg
+            elif cmd == 'httpreq':
+                try:
+                    proc = httpreq.Httpreq(logger, fileup_name=fileup_name)
+                except Exception as e:
+                    common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
+                    return 1, msg
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, None, False)
+                if code != 0:
+                    return code, ret
 
-    elif mode == 'install':
-        logger, _ = common.load_config(mode)
-        inst = install.Install(logger=logger)
-        if cmd == 'redis':
-            ret = inst.redis()
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-
-        elif cmd == 'server':
-            install_set = not (install_onnx or install_mmdet or install_mmseg or install_mmcls or install_mmpretrain or install_insightface)
-            onnx = install_set
-            mmdet = install_set
-            mmseg = install_set
-            mmcls = False
-            mmpretrain = install_set
-            insightface = install_set
-            onnx = install_onnx if install_onnx else onnx
-            mmdet = install_mmdet if install_mmdet else mmdet
-            mmseg = install_mmseg if install_mmseg else mmseg
-            mmcls = install_mmcls if install_mmcls else mmcls
-            mmpretrain = install_mmpretrain if install_mmpretrain else mmpretrain
-            insightface = install_insightface if install_insightface else insightface
-            if data is None:
-                msg = {"warn":f"Please specify the --data option."}
-                common.print_format(msg, format, tm, output_json, output_json_append)
-                return 1, msg
-            ret = inst.server(Path(data), install_iinfer, install_onnx=onnx,
-                              install_mmdet=mmdet, install_mmseg=mmseg, install_mmcls=mmcls, install_mmpretrain=mmpretrain,
-                              install_insightface=insightface, install_tag=install_tag, install_use_gpu=install_use_gpu)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-
-        elif cmd == 'onnx':
-            ret = inst.onnx(install_use_gpu=install_use_gpu)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-
-        elif cmd == 'mmdet':
-            if data is None:
-                msg = {"warn":f"Please specify the --data option."}
-                common.print_format(msg, format, tm, output_json, output_json_append)
-                return 1, msg
-            ret = inst.mmdet(Path(data), install_use_gpu=install_use_gpu)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-
-        elif cmd == 'mmseg':
-            if data is None:
-                msg = {"warn":f"Please specify the --data option."}
+            elif cmd == 'seg_bbox':
+                try:
+                    proc = seg_bbox.SegBBox(logger, del_segments=del_segments, nodraw=nodraw, nodraw_bbox=nodraw_bbox, nodraw_rbbox=nodraw_rbbox,
+                                            output_preview=output_preview)
+                except Exception as e:
+                    common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
+                    return 1, msg
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+                if code != 0:
+                    return code, ret
+
+            elif cmd == 'seg_filter':
+                try:
+                    proc = seg_filter.SegFilter(logger, logits_th=logits_th, classes=classes, labels=labels, nodraw=nodraw, del_logits=del_logits)
+                except Exception as e:
+                    common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
+                    return 1, msg
+                code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+                if code != 0:
+                    return code, ret
+
+            else:
+                msg = {"warn":f"Unkown command."}
                 common.print_format(msg, format, tm, output_json, output_json_append)
                 return 1, msg
-            ret = inst.mmseg(Path(data), install_use_gpu=install_use_gpu)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-
-        elif cmd == 'mmcls':
-            ret = inst.mmcls(Path(data), install_use_gpu=install_use_gpu)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-
-        elif cmd == 'mmpretrain':
-            if data is None:
-                msg = {"warn":f"Please specify the --data option."}
+
+        elif mode == 'redis':
+            logger, _ = common.load_config(mode)
+            rd = redis.Redis(logger=logger, wsl_name=wsl_name, wsl_user=wsl_user)
+            if cmd == 'docker_run':
+                ret = rd.docker_run(port, password)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+
+            elif cmd == 'docker_stop':
+                ret = rd.docker_stop()
+                common.print_format(ret, format, tm, output_json, output_json_append)
+
+            else:
+                msg = {"warn":f"Unkown command."}
                 common.print_format(msg, format, tm, output_json, output_json_append)
                 return 1, msg
-            ret = inst.mmpretrain(Path(data), install_use_gpu=install_use_gpu)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
-
-        elif cmd == 'insightface':
-            if data is None:
-                msg = {"warn":f"Please specify the --data option."}
+
+        elif mode == 'install':
+            logger, _ = common.load_config(mode)
+            self.inst = install.Install(logger=logger)
+            if cmd == 'redis':
+                ret = self.inst.redis()
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'server':
+                install_set = not (install_onnx or install_mmdet or install_mmseg or install_mmcls or install_mmpretrain or install_insightface)
+                onnx = install_set
+                mmdet = install_set
+                mmseg = install_set
+                mmcls = False
+                mmpretrain = install_set
+                insightface = install_set
+                onnx = install_onnx if install_onnx else onnx
+                mmdet = install_mmdet if install_mmdet else mmdet
+                mmseg = install_mmseg if install_mmseg else mmseg
+                mmcls = install_mmcls if install_mmcls else mmcls
+                mmpretrain = install_mmpretrain if install_mmpretrain else mmpretrain
+                insightface = install_insightface if install_insightface else insightface
+                if data is None:
+                    msg = {"warn":f"Please specify the --data option."}
+                    common.print_format(msg, format, tm, output_json, output_json_append)
+                    return 1, msg
+                ret = self.inst.server(Path(data), install_iinfer, install_onnx=onnx,
+                                install_mmdet=mmdet, install_mmseg=mmseg, install_mmcls=mmcls, install_mmpretrain=mmpretrain,
+                                install_insightface=insightface, install_tag=install_tag, install_use_gpu=install_use_gpu)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'onnx':
+                ret = self.inst.onnx(install_use_gpu=install_use_gpu)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'mmdet':
+                if data is None:
+                    msg = {"warn":f"Please specify the --data option."}
+                    common.print_format(msg, format, tm, output_json, output_json_append)
+                    return 1, msg
+                ret = self.inst.mmdet(Path(data), install_use_gpu=install_use_gpu)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'mmseg':
+                if data is None:
+                    msg = {"warn":f"Please specify the --data option."}
+                    common.print_format(msg, format, tm, output_json, output_json_append)
+                    return 1, msg
+                ret = self.inst.mmseg(Path(data), install_use_gpu=install_use_gpu)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'mmcls':
+                ret = self.inst.mmcls(Path(data), install_use_gpu=install_use_gpu)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'mmpretrain':
+                if data is None:
+                    msg = {"warn":f"Please specify the --data option."}
+                    common.print_format(msg, format, tm, output_json, output_json_append)
+                    return 1, msg
+                ret = self.inst.mmpretrain(Path(data), install_use_gpu=install_use_gpu)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            elif cmd == 'insightface':
+                if data is None:
+                    msg = {"warn":f"Please specify the --data option."}
+                    common.print_format(msg, format, tm, output_json, output_json_append)
+                    return 1, msg
+                ret = self.inst.insightface(Path(data), install_use_gpu=install_use_gpu)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
+
+            else:
+                msg = {"warn":f"Unkown command."}
                 common.print_format(msg, format, tm, output_json, output_json_append)
                 return 1, msg
-            ret = inst.insightface(Path(data), install_use_gpu=install_use_gpu)
-            common.print_format(ret, format, tm, output_json, output_json_append)
-            if 'success' not in ret:
-                return 1, ret
 
         else:
-            msg = {"warn":f"Unkown command."}
+            msg = {"warn":f"Unkown mode."}
             common.print_format(msg, format, tm, output_json, output_json_append)
             return 1, msg
 
-    else:
-        msg = {"warn":f"Unkown mode."}
-        common.print_format(msg, format, tm, output_json, output_json_append)
-        return 1, msg
-
-    return 0, ret
+        return 0, ret
```

### Comparing `iinfer-0.6.9/iinfer/app/client.py` & `iinfer-0.7.0/iinfer/app/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         self.redis_port = redis_port
         self.password = redis_password
         if svname is None or svname == "":
             raise Exception("svname is empty.")
         self.svname = f"sv-{svname}"
         self.hbname = f"hb-{svname}"
         self.redis_cli = redis.Redis(host=self.redis_host, port=self.redis_port, db=0, password=redis_password)
+        self.is_running = False
 
     def __exit__(self, a, b, c):
         pass
 
     def check_server(self):
         """
         Redisサーバーにpingを送信し、応答があるか確認する
@@ -63,16 +64,29 @@
         Returns:
             dict: Redisサーバーからの応答
         """
         try:
             self.check_server()
             reskey = common.random_string()
             self.redis_cli.rpush(key, f"{cmd} {reskey} {' '.join([str(p) for p in params])}")
-            res = self.redis_cli.blpop([reskey], timeout=timeout)
-            return self._response(reskey, res)
+            self.is_running = True
+            stime = time.time()
+            while self.is_running:
+                ctime = time.time()
+                if ctime - stime > timeout:
+                    raise Exception(f"Response timed out.")
+                res = self.redis_cli.blpop([reskey], timeout=1)
+                if res is None or len(res) <= 0:
+                    time.sleep(1)
+                    continue
+                return self._response(reskey, res)
+            raise KeyboardInterrupt(f"Stop command.")
+        except KeyboardInterrupt as e:
+            self.logger.error(f"Stop command. cmd={cmd}, params={params}", exc_info=True)
+            return {"error": f"Stop command. cmd={cmd}, params={params}"}
         except Exception as e:
             self.logger.error(f"fail to execute command. cmd={cmd}, params={params}, msg={e}", exc_info=True)
             return {"error": f"fail to execute command. cmd={cmd}, params={params}, msg={e}"}
 
     def _response(self, reskey:str, res_msg:List[str]):
         """
         Redisサーバーからの応答を解析する
@@ -308,22 +322,22 @@
         return res_json
 
 
     def stop_server(self, timeout:int = 60):
         res_json = self._proc(self.svname, 'stop_server', [], timeout=timeout)
         return res_json
 
-    def predict(self, name:str, image = None, image_file:Path = None, image_file_enable:bool=True, image_type:str = 'jpeg', output_image_file:Path = None, output_preview:bool=False, nodraw:bool=False, timeout:int = 60):
+    def predict(self, name:str, image = None, image_file = None, image_file_enable:bool=True, image_type:str = 'jpeg', output_image_file:Path = None, output_preview:bool=False, nodraw:bool=False, timeout:int = 60):
         """
         画像をRedisサーバーに送信し、推論結果を取得する
 
         Args:
             name (str): モデル名
             image (np.ndarray | bytes, optional): 画像データ. Defaults to None. np.ndarray型の場合はデコードしない(RGBであること).
-            image_file (Path, optional): 画像ファイルのパス. Defaults to None.
+            image_file (str|file-like object, optional): 画像ファイルのパス. Defaults to None.
             image_file_enable (bool, optional): 画像ファイルを使用するかどうか. Defaults to True. image_fileがNoneでなく、このパラメーターがTrueの場合はimage_fileを使用する.
             image_type (str, optional): 画像の形式. Defaults to 'jpeg'.
             output_image_file (Path, optional): 予測結果の画像ファイルのパス. Defaults to None.
             output_preview (bool, optional): 予測結果の画像をプレビューするかどうか. Defaults to False.
             nodraw (bool, optional): 描画フラグ. Defaults to False.
             timeout (int, optional): タイムアウト時間. Defaults to 60.
 
@@ -337,24 +351,33 @@
             self.logger.error(f"name is empty.")
             return {"error": f"name is empty."}
         if image is None and image_file is None:
             self.logger.error(f"image and image_file is empty.")
             return {"error": f"image and image_file is empty."}
         npy_b64 = None
         if image_file is not None and image_file_enable:
-            if not image_file.exists():
-                self.logger.error(f"Not found image_file. {image_file}.")
-                return {"error": f"Not found image_file. {image_file}."}
+            if type(image_file) == str:
+                if not Path(image_file).exists():
+                    self.logger.error(f"Not found image_file. {image_file}.")
+                    return {"error": f"Not found image_file. {image_file}."}
             if image_type == 'jpeg' or image_type == 'png' or image_type == 'bmp':
-                with open(image_file, "rb") as f:
+                f = None
+                try:
+                    f = image_file if type(image_file) is not str else open(image_file, "rb")
                     img_npy = convert.imgfile2npy(f)
+                finally:
+                    if f is not None: f.close()
             elif image_type == 'capture':
-                with open(image_file, "r", encoding='utf-8') as f:
+                f = None
+                try:
+                    f = image_file if type(image_file) is not str else open(image_file, "r", encoding='utf-8')
                     res_list = []
                     for line in f:
+                        if type(line) is bytes:
+                            line = line.decode('utf-8').strip()
                         capture_data = line.split(',')
                         t = capture_data[0]
                         img = capture_data[1]
                         h = int(capture_data[2])
                         w = int(capture_data[3])
                         c = int(capture_data[4])
                         fn = Path(capture_data[5].strip())
@@ -365,16 +388,20 @@
                         res_json = self.predict(name, image=img_npy, image_file=fn, image_file_enable=False, output_image_file=output_image_file, output_preview=output_preview, nodraw=nodraw, timeout=timeout)
                         res_list.append(res_json)
                     if len(res_list) <= 0:
                         return {"warn": f"capture file is no data."}
                     elif len(res_list) == 1:
                         return res_list[0]
                     return res_list
+                finally:
+                    if f is not None: f.close()
             elif image_type == 'output_json':
-                with open(image_file, "r", encoding='utf-8') as f:
+                f = None
+                try:
+                    f = image_file if type(image_file) is not str else open(image_file, "r", encoding='utf-8')
                     res_list = []
                     for line in f:
                         res_json = json.loads(line)
                         if not ("output_image" in res_json and "output_image_shape" in res_json and "output_image_name" in res_json):
                             self.logger.warn(f"image_file data is invalid. Not found output_image or output_image_shape or output_image_name key.")
                             continue
                         img_npy = convert.b64str2npy(res_json["output_image"], shape=res_json["output_image_shape"])
@@ -382,62 +409,68 @@
                                                 output_image_file=output_image_file, output_preview=output_preview, nodraw=nodraw, timeout=timeout)
                         res_list.append(res_json)
                     if len(res_list) <= 0:
                         return {"warn": f"output_json file is no data."}
                     elif len(res_list) == 1:
                         return res_list[0]
                     return res_list
+                finally:
+                    if f is not None: f.close()
             else:
                 self.logger.error(f"image_type is invalid. {image_type}.")
                 return {"error": f"image_type is invalid. {image_type}."}
         else:
             if type(image) == np.ndarray:
                 img_npy = image
-                if image_file is None: image_file = Path(f'{datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")}.capture')
+                if image_file is None: image_file = f'{datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")}.capture'
                 image_file_enable = False
             elif image_type == 'capture':
                 capture_data = image.split(',')
                 #self.logger.info(f"capture_data={capture_data[1:]}")
                 t = capture_data[0]
                 img = capture_data[1]
                 h = int(capture_data[2])
                 w = int(capture_data[3])
                 c = int(capture_data[4])
-                if image_file is None: image_file = Path(capture_data[5])
+                if image_file is None: image_file = capture_data[5]
                 image_file_enable = False
                 if t == 'capture':
                     img_npy = convert.b64str2npy(img, shape=(h, w, c) if c > 0 else (h, w))
                 else:
                     img_npy = convert.imgbytes2npy(convert.b64str2bytes(img))
             elif image_type == 'output_json':
                 res_json = json.loads(image)
                 if not ("output_image" in res_json and "output_image_shape" in res_json and "output_image_name" in res_json):
                     self.logger.error(f"image_file data is invalid. Not found output_image or output_image_shape or output_image_name key.")
                     return {"error": f"image_file data is invalid. Not found output_image or output_image_shape or output_image_name key."}
                 img_npy = convert.b64str2npy(res_json["output_image"], shape=res_json["output_image_shape"])
-                if image_file is None: image_file = Path(res_json["output_image_name"])
+                if image_file is None: image_file = res_json["output_image_name"]
                 image_file_enable = False
             elif image_type == 'jpeg' or image_type == 'png' or image_type == 'bmp':
                 img_npy = convert.imgbytes2npy(image)
-                if image_file is None: image_file = Path(f'{datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")}.{image_type}')
+                if image_file is None: image_file = f'{datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")}.{image_type}'
                 image_file_enable = False
             else:
                 self.logger.error(f"image_type is invalid. {image_type}.")
                 return {"error": f"image_type is invalid. {image_type}."}
 
         npy_b64 = convert.npy2b64str(img_npy)
         #img_npy2 = np.frombuffer(base64.b64decode(npy_b64), dtype='uint8').reshape(img_npy.shape)
 
-        res_json = self._proc(self.svname, 'predict', [name, npy_b64, str(nodraw), str(img_npy.shape[0]), str(img_npy.shape[1]), str(img_npy.shape[2] if len(img_npy.shape) > 2 else '-1'), image_file.name], timeout=timeout)
+        res_json = self._proc(self.svname, 'predict',
+                              [name, npy_b64, str(nodraw), str(img_npy.shape[0]), str(img_npy.shape[1]),
+                               str(img_npy.shape[2] if len(img_npy.shape) > 2 else '-1'), image_file], timeout=timeout)
         if "output_image" in res_json and "output_image_shape" in res_json:
             #byteio = BytesIO(base64.b64decode(res_json["output_image"]))
             #img_npy = np.load(byteio)
             img_npy = convert.b64str2npy(res_json["output_image"], res_json["output_image_shape"])
             if output_image_file is not None:
-                convert.npy2imgfile(img_npy, output_image_file=output_image_file, image_type=image_type)
+                exp = Path(output_image_file).suffix
+                exp = exp[1:] if exp[0] == '.' else exp
+                convert.npy2imgfile(img_npy, output_image_file=output_image_file, image_type=exp)
             if output_preview:
                 # RGB画像をBGR画像に変換
                 try:
                     cv2.imshow('preview', convert.bgr2rgb(img_npy))
                     cv2.waitKey(1)
                 except KeyboardInterrupt:
                     pass
@@ -569,19 +602,22 @@
             cap.set(cv2.CAP_PROP_FRAME_WIDTH, capture_frame_width)
         if capture_frame_height is not None:
             cap.set(cv2.CAP_PROP_FRAME_HEIGHT, capture_frame_height)
         if capture_fps is not None:
             cap.set(cv2.CAP_PROP_FPS, capture_fps)
         try:
             interval = float(1 / capture_fps)
-            while True:
+            self.is_running = True
+            while self.is_running:
                 start = time.perf_counter()
                 ret, frame = cap.read()
                 output_image_name = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")
                 if ret:
+                    if capture_frame_width is not None and capture_frame_height is not None:
+                        frame = cv2.resize(frame, (capture_frame_width, capture_frame_height), interpolation=cv2.INTER_NEAREST)
                     img_npy = convert.bgr2rgb(frame)
                     if output_preview:
                         # RGB画像をBGR画像に変換
                         cv2.imshow('preview', convert.bgr2rgb(img_npy))
                         cv2.waitKey(1)
                     img_b64 = None
                     if image_type == 'capture' or image_type is None:
```

### Comparing `iinfer-0.6.9/iinfer/app/common.py` & `iinfer-0.7.0/iinfer/app/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 import json
 import numpy as np
 import os
 import platform
 import random
 import shutil
 import string
+import re
 import requests
 import subprocess
+import tempfile
 import time
 import yaml
 
 APP_ID = 'iinfer'
 HOME_DIR = Path(os.path.expanduser("~"))
 
 def load_config(mode:str) -> Tuple[logging.Logger, dict]:
@@ -50,14 +52,16 @@
         return int(o)
     if isinstance(o, np.int32):
         return int(o)
     if isinstance(o, np.intc):
         return int(o)
     if isinstance(o, Path):
         return str(o)
+    if isinstance(o, tempfile._TemporaryFileWrapper):
+        return str(o)
     if isinstance(o, datetime.datetime):
         return o.strftime('%Y-%m-%dT%H:%M:%S')
     raise TypeError(f"Type {type(o)} not serializable")
 
 def saveopt(opt:dict, opt_path:Path) -> None:
     """
     コマンドラインオプションをJSON形式でファイルに保存します。
@@ -114,14 +118,38 @@
     if key in opt:
         return opt[key]
     else:
         if withset:
             opt[key] = defval
         return defval
 
+def safe_fname(fname:str) -> str:
+    """
+    ファイル名に使えない文字を置換します。
+
+    Args:
+        fname (str): ファイル名
+
+    Returns:
+        str: 置換後のファイル名
+    """
+    return re.sub('[\s:\\\\/,\.\?\#\$\%\^\&\!\@\*\~\|\<\>\(\)\{\}\[\]\'\"\`]', '_',str(fname))
+
+def check_fname(fname:str) -> bool:
+    """
+    ファイル名に使えない文字が含まれているかどうかをチェックします。
+
+    Args:
+        fname (str): ファイル名
+
+    Returns:
+        bool: Trueの場合は使えない文字が含まれている
+    """
+    return re.search('[\s:\\\\/,\.\?\#\$\%\^\&\!\@\*\~\|\<\>\(\)\{\}\[\]\'\"\`]',str(fname)) is not None
+
 def mkdirs(dir_path:Path):
     """
     ディレクトリを中間パスも含めて作成します。
 
     Args:
         dir_path (Path): 作成するディレクトリのパス
```

### Comparing `iinfer-0.6.9/iinfer/app/commons/convert.py` & `iinfer-0.7.0/iinfer/app/commons/convert.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/commons/module.py` & `iinfer-0.7.0/iinfer/app/commons/module.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/injection.py` & `iinfer-0.7.0/iinfer/app/injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/injections/after_cls_jadge_injection.py` & `iinfer-0.7.0/iinfer/app/injections/after_cls_jadge_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/injections/after_csv_injection.py` & `iinfer-0.7.0/iinfer/app/injections/after_csv_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/injections/after_det_filter_injection.py` & `iinfer-0.7.0/iinfer/app/injections/after_det_filter_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/injections/after_det_jadge_injection.py` & `iinfer-0.7.0/iinfer/app/injections/after_det_jadge_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/injections/after_http_injection.py` & `iinfer-0.7.0/iinfer/app/injections/after_http_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/injections/after_seg_bbox_injection.py` & `iinfer-0.7.0/iinfer/app/injections/after_seg_bbox_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/injections/after_seg_filter_injection.py` & `iinfer-0.7.0/iinfer/app/injections/after_seg_filter_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/injections/before_grayimg_injection.py` & `iinfer-0.7.0/iinfer/app/injections/before_grayimg_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/install.py` & `iinfer-0.7.0/iinfer/app/install.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/postprocess.py` & `iinfer-0.7.0/iinfer/app/postprocess.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/postprocesses/cls_jadge.py` & `iinfer-0.7.0/iinfer/app/postprocesses/cls_jadge.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/postprocesses/csv.py` & `iinfer-0.7.0/iinfer/app/postprocesses/csv.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/postprocesses/det_clip.py` & `iinfer-0.7.0/iinfer/app/postprocesses/det_clip.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/postprocesses/det_face_store.py` & `iinfer-0.7.0/iinfer/app/postprocesses/det_face_store.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/postprocesses/det_filter.py` & `iinfer-0.7.0/iinfer/app/postprocesses/det_filter.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/postprocesses/det_jadge.py` & `iinfer-0.7.0/iinfer/app/postprocesses/det_jadge.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/postprocesses/httpreq.py` & `iinfer-0.7.0/iinfer/app/postprocesses/httpreq.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/postprocesses/seg_bbox.py` & `iinfer-0.7.0/iinfer/app/postprocesses/seg_bbox.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/postprocesses/seg_filter.py` & `iinfer-0.7.0/iinfer/app/postprocesses/seg_filter.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/predict.py` & `iinfer-0.7.0/iinfer/app/predict.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/predicts/insightface_det.py` & `iinfer-0.7.0/iinfer/app/predicts/insightface_det.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/predicts/mmdet_det_YoloX.py` & `iinfer-0.7.0/iinfer/app/predicts/mmdet_det_YoloX.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/predicts/mmpretrain_cls_swin.py` & `iinfer-0.7.0/iinfer/app/predicts/mmpretrain_cls_swin.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/predicts/mmrotate_det_ReDet.py` & `iinfer-0.7.0/iinfer/app/predicts/mmrotate_det_ReDet.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/predicts/mmseg_seg_PSPNet.py` & `iinfer-0.7.0/iinfer/app/predicts/mmseg_seg_PSPNet.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py` & `iinfer-0.7.0/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/predicts/onnx_det_TinyYoloV3.py` & `iinfer-0.7.0/iinfer/app/predicts/onnx_det_TinyYoloV3.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/predicts/onnx_det_YoloV3.py` & `iinfer-0.7.0/iinfer/app/predicts/onnx_det_YoloV3.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/predicts/onnx_det_YoloX.py` & `iinfer-0.7.0/iinfer/app/predicts/onnx_det_YoloX.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/predicts/onnx_det_YoloX_Lite.py` & `iinfer-0.7.0/iinfer/app/predicts/onnx_det_YoloX_Lite.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/redis.py` & `iinfer-0.7.0/iinfer/app/redis.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/app/server.py` & `iinfer-0.7.0/iinfer/app/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from iinfer.app.commons import convert, module
 from typing import List, Dict, Any, Tuple
 import base64
 import datetime
 import logging
 import json
 import numpy as np
-import re
 import redis
 import shutil
 import time
 
 
 class Server(object):
     RESP_SCCESS:int = 0
@@ -381,15 +380,15 @@
                 self.responce(reskey, {"warn": f"{name}_file is not None but {name}_bin is None."})
                 return False, files
             if files is None and datas is not None:
                 self.logger.warn(f"{name}_file is None but {name}_bin is not None.")
                 self.responce(reskey, {"warn": f"{name}_file is None but {name}_bin is not None."})
                 return False, files
             if files is not None:
-                files = [deploy_dir / cf for cf in files]
+                files = [deploy_dir / cf for cf in files if cf is not None and cf != '']
                 for i, cf in enumerate(files):
                     with open(cf, "wb") as f:
                         f.write(datas[i])
                         self.logger.info(f"Save {cf} to {str(deploy_dir)}")
             return True, files
         ret, model_conf_file = _save_m('model_conf', model_conf_file, model_conf_bin)
         if not ret: return self.RESP_WARN
@@ -714,53 +713,73 @@
             self.logger.warn(f"{name} has not yet started a session.")
             self.responce(reskey, {"warn": f"{name} has not yet started a session."})
             return self.RESP_WARN
         if nodraw is None:
             nodraw = False
         session = self.sessions[name]
         try:
+            predict_process_start = time.perf_counter()
             # 前処理を実行
             if session['before_injections'] is not None:
                 injections:List[injection.BeforeInjection] = session['before_injections']
                 for inject in injections:
                     image = inject.action(reskey, name, image, session)
+            before_injections_end = time.perf_counter()
             # 推論を実行
             predict_obj:predict.Predict = session['predict_obj']
             outputs, output_image = predict_obj.predict(session['session'], session['model_img_width'], session['model_img_height'], image,
                                                         labels=session['labels'], colors=session['colors'], nodraw=nodraw)
             outputs['image_name'] = output_image_name
+            predict_end = time.perf_counter()
             if session['tracker'] is not None:
                 if 'output_boxes' in outputs and 'output_scores' in outputs and 'output_classes' in outputs:
                     detections = [Detection(box, score, cls) for box, score, cls in zip(outputs['output_boxes'], outputs['output_scores'], outputs['output_classes'])]
                     session['tracker'].step(detections=detections)
                     tracks = session['tracker'].active_tracks()
                     outputs['output_tracks'] = [t.id for t in tracks]
                     if image is not None:
                         image = common.draw_boxes(image, outputs['output_boxes'], outputs['output_scores'], outputs['output_classes'], ids=outputs['output_tracks'])
+            tracker_end = time.perf_counter()
 
             def _after_injection(reskey:str, name:str, output:dict, output_image:Image.Image, session:dict):
                 if session['after_injections'] is not None:
                     injections:List[injection.AfterInjection] = session['after_injections']
                     for inject in injections:
                         output, output_image = inject.action(reskey, name, output, output_image, session)
                 return output, output_image
 
+            def _set_perftime(output, predict_process_start, before_injections_end, predict_end, tracker_end, after_injections_end, predict_process_end):
+                performance = f"before={(before_injections_end-predict_process_start):.3f}s" \
+                              f", predict={(predict_end-before_injections_end):.3f}s" \
+                              f", track={(tracker_end-predict_end):.3f}s" \
+                              f", after={(after_injections_end-tracker_end):.3f}s" \
+                              f", process={(predict_process_end-predict_process_start):.3f}s"
+                if 'success' in output:
+                    output['success']['performance'] = performance
+
             if output_image is not None:
                 output = dict(success=outputs, output_image_name=output_image_name)
                 # 後処理を実行
                 output, output_image = _after_injection(reskey, name, output, output_image, session)
+                after_injections_end = time.perf_counter()
                 output_image_npy = convert.img2npy(output_image)
                 output_image_b64 = convert.npy2b64str(output_image_npy)
+                predict_process_end = time.perf_counter()
                 output['output_image'] = output_image_b64
                 output['output_image_shape'] = output_image_npy.shape
+                _set_perftime(output, predict_process_start, before_injections_end, predict_end,
+                             tracker_end, after_injections_end, predict_process_end)
                 self.responce(reskey, output)
                 return self.RESP_SCCESS
             output = dict(success=outputs)
             # 後処理を実行
-            output, output_image = _after_injection(reskey, name, output, None, session)
+            output, _ = _after_injection(reskey, name, output, None, session)
+            after_injections_end = predict_process_end = time.perf_counter()
+            _set_perftime(output, predict_process_start, before_injections_end, predict_end,
+                            tracker_end, after_injections_end, predict_process_end)
             self.responce(reskey, output)
             return self.RESP_SCCESS
         except Exception as e:
             self.logger.warn(f"Failed to run inference: {e}", exc_info=True)
             self.responce(reskey, {"warn": f"Failed to run inference: {e}"})
             return self.RESP_WARN
 
@@ -811,16 +830,14 @@
 
         Returns:
             int: レスポンスコード
         """
         chk, _ = self._file_exists(reskey, current_path)
         if not chk: return self.RESP_WARN
         
-        def _mk_key(path):
-            return re.sub('[\s:\\\\/,\.#$%^&!@*\(\)\{\}\[\]\'\"\`]', '_',str(path))
         def _ts2str(ts):
             return datetime.datetime.fromtimestamp(ts)
 
         current_path = f'/{current_path}' if not current_path.startswith('/') else current_path
         current_path_parts = current_path.split("/")
         current_path_parts = current_path_parts[1:] if current_path=='/' else current_path_parts
         path_tree = {}
@@ -828,22 +845,22 @@
         for i, cpart in enumerate(current_path_parts):
             cpath = '/'.join(current_path_parts[1:i+1])
             file_list:Path = self.data_dir / cpath
             children = dict()
             for f in file_list.iterdir():
                 parts = str(f)[data_dir_len:].replace("\\","/").split("/")
                 path = "/".join(parts[:i+2])
-                key = _mk_key(path)
+                key = common.safe_fname(path)
                 if key in children:
                     continue
                 children[key] = dict(name=f.name, is_dir=f.is_dir(), path=path, size=f.stat().st_size , last=_ts2str(f.stat().st_mtime))
 
             tpath = '/'.join(current_path_parts[:i+1])
             tpath = '/' if tpath=='' else tpath
-            tpath_key = _mk_key(tpath)
+            tpath_key = common.safe_fname(tpath)
             cpart = '/' if cpart=='' else cpart
             path_tree[tpath_key] = dict(name=cpart, is_dir=True, path=tpath, children=children, size=0, last="")
 
         self.responce(reskey, {"success": path_tree})
         return self.RESP_SCCESS
 
     def file_mkdir(self, reskey:str, current_path:str):
```

### Comparing `iinfer-0.6.9/iinfer/docker/Dockerfile` & `iinfer-0.7.0/iinfer/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt` & `iinfer-0.7.0/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/licenses/files.txt` & `iinfer-0.7.0/iinfer/licenses/files.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/logconf_client.yml` & `iinfer-0.7.0/iinfer/logconf_client.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/logconf_gui.yml` & `iinfer-0.7.0/iinfer/logconf_gui.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/logconf_install.yml` & `iinfer-0.7.0/iinfer/logconf_install.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/logconf_postprocess.yml` & `iinfer-0.7.0/iinfer/logconf_postprocess.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/logconf_redis.yml` & `iinfer-0.7.0/iinfer/logconf_redis.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/logconf_server.yml` & `iinfer-0.7.0/iinfer/logconf_server.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/version.py` & `iinfer-0.7.0/iinfer/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
 
-dt_now = datetime.datetime(2024, 4, 15)
+dt_now = datetime.datetime(2024, 4, 29)
 __title__ = 'iinfer (Image Inference Application)'
-__version__ = '0.6.9'
+__version__ = '0.7.0'
 __copyright__ = f'Copyright © 2023-{dt_now.strftime("%Y")} hamacom2004jp'
 __pypiurl__ = 'https://pypi.org/project/iinfer/'
 __srcurl__ = 'https://github.com/hamacom2004jp/iinfer'
 __docurl__ = 'https://hamacom2004jp.github.io/iinfer/index.html'
 __description__ = f'{__title__} {__version__}\n' + \
                   f'{__copyright__}\n' + \
                   f'Web Site: PyPi <{__pypiurl__}>\n' + \
```

### Comparing `iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js` & `iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js` & `iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css` & `iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css` & `iinfer-0.7.0/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/iinfer/filer_modal.js` & `iinfer-0.7.0/iinfer/web/assets/iinfer/filer_modal.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,101 +1,101 @@
 // ファイラーモーダル
 filer_modal_func = async (target_id, modal_title, current_path, call_back_func) => {
-    filer_modal = $(`#filer_modal`);
-    filer_modal.find(`.modal-title`).text(modal_title);
-    filer_modal.find(`.modal-body`).html(`<ul class="tree-menu overflow-auto border col-4"></ul><div class="file-list overflow-auto col-8"></div>`);
-    filer_modal.find(`.tree-menu`).css(`height`, `calc(100vh - 180px)`);
-    filer_modal.find(`.file-list`).css(`height`, `calc(100vh - 180px)`);
-    //filer_modal.find(`.tree-menu`).resizable({ghost:true});
-    filer_modal.find(`.filer_address_bot`).off(`click`).on('click', async () => {
-        current_path = filer_modal.find(`.filer_address`).val();
+    filer_modal = $('#filer_modal');
+    filer_modal.find('.modal-title').text(modal_title);
+    filer_modal.find('.modal-body').html('<ul class="tree-menu overflow-auto border col-4"></ul><div class="file-list overflow-auto col-8"></div>');
+    filer_modal.find('.tree-menu').css('height', 'calc(100vh - 180px)');
+    filer_modal.find('.file-list').css('height', 'calc(100vh - 180px)');
+    //filer_modal.find('.tree-menu').resizable({ghost:true});
+    filer_modal.find('.filer_address_bot').off('click').on('click', async () => {
+        current_path = filer_modal.find('.filer_address').val();
         key = current_path.replace(/[\s\:\\\/\,\.\#\$\%\^\&\!\@\*\(\)\{\}\[\]\'\"\`]/g, `_`);
         current_node = $(`#${key}`);
         if (current_node.length <= 0) {
             alert(`invalid path:${key}`);
             return;
         }
-        await reload_tree(target_id, filer_modal.find(`.tree-menu`), current_path, filer_modal.find(`.file-list`));
+        await reload_tree(target_id, filer_modal.find('.tree-menu'), current_path, filer_modal.find('.file-list'));
     });
 
     reload_tree = async (target_id, current_node, current_path, file_list_elem) => {
         //dict(name=part, is_dir=path.is_dir(), path=str(path), children=children)
         py_list_tree = await eel.list_tree(current_path)();
-        current_node.html(``);
+        current_node.html('');
         $.each(py_list_tree, (key, node) => {
-            if (!node[`is_dir`]) return;
+            if (!node['is_dir']) return;
             li_elem = $(`#${key}`);
             if (li_elem.length > 0) {
                 li_elem.html(`<a href="#" class="folder-open">${node['name']}</a>`);
             } else {
                 li_elem = $(`<li id="${key}"><a href="#" class="folder-open">${node['name']}</a></li>`);
                 current_node.append(li_elem);
             }
             mk_func = (target_id, current_node, current_path) => {
                 // 左側ペインのフォルダを選択した時の処理
                 return () => reload_tree(target_id, current_node, current_path);
             }
-            li_elem.find(`a`).off(`click`).on('click', mk_func(target_id, current_node, node[`path`]));
-            if (node[`children`]) {
-                ul_elem = $(`<ul/>`);
+            li_elem.find('a').off('click').on('click', mk_func(target_id, current_node, node['path']));
+            if (node['children']) {
+                ul_elem = $('<ul/>');
                 li_elem.append(ul_elem);
-                $.each(node[`children`], (k, n) => {
-                    if (!n[`is_dir`]) return;
+                $.each(node['children'], (k, n) => {
+                    if (!n['is_dir']) return;
                     li = $(`<li id="${k}"><a href="#" class="folder-close">${n['name']}</a></li>`);
-                    li.find(`a`).click(mk_func(target_id, ul_elem, n[`path`]));
+                    li.find('a').click(mk_func(target_id, ul_elem, n['path']));
                     ul_elem.append(li);
                 });
             }
         });
         py_list_tree_keys = Object.keys(py_list_tree);
         if (py_list_tree_keys.length > 0) {
             node = py_list_tree[py_list_tree_keys[py_list_tree_keys.length - 1]];
-            table = $(`<table class="table table-bordered table-hover table-sm"></table>`);
-            filer_modal.find(`.file-list`).html(``);
-            filer_modal.find(`.file-list`).append(table);
-            table_head = $(`<thead class="table-dark bg-dark"></thead>`);
-            table_head.append($(`<tr><th scope="col">-</th><th scope="col">name</th><th scope="col">size</th><th scope="col">last</th></tr>`));
+            table = $('<table class="table table-bordered table-hover table-sm"></table>');
+            filer_modal.find('.file-list').html('');
+            filer_modal.find('.file-list').append(table);
+            table_head = $('<thead class="table-dark bg-dark"></thead>');
+            table_head.append($('<tr><th scope="col">-</th><th scope="col">name</th><th scope="col">size</th><th scope="col">last</th></tr>'));
             table.append(table_head);
-            table_body = $(`<tbody></tbody>`);
+            table_body = $('<tbody></tbody>');
             table.append(table_body);
-            filer_modal.find(`.filer_address`).val(node[`path`]);
-            if (node[`children`]) {
+            filer_modal.find('.filer_address').val(node['path']);
+            if (node['children']) {
                 mk_func = (target_id, current_node, current_path) => {
                     // 右側ペインのフォルダを選択した時の処理
                     return () => reload_tree(target_id, current_node, current_path);
                 }
-                $.each(node[`children`], (k, n) => {
-                    if (!n[`is_dir`]) return;
-                    tr_elem = $(`<tr/>`);
+                $.each(node['children'], (k, n) => {
+                    if (!n['is_dir']) return;
+                    tr_elem = $('<tr/>');
                     table_body.append(tr_elem);
                     td = $(`<td><a href="#" class="folder-close">${n['name']}</a></td>`);
-                    td.find(`a`).click(mk_func(target_id, $(`#${k}`), n[`path`]));
-                    tr_elem.append($(`<td><img src="/assets/tree-menu/image/folder-close.png"></td>`));
+                    td.find('a').click(mk_func(target_id, $(`#${k}`), n['path']));
+                    tr_elem.append($('<td><img src="/assets/tree-menu/image/folder-close.png"></td>'));
                     tr_elem.append(td);
                     tr_elem.append($(`<td>${n['size']}</td>`));
                     tr_elem.append($(`<td>${n['last']}</td>`));
                 });
                 mk_func = (target_id, current_node, current_path) => {
                     // 右側ペインのファイルを選択した時の処理
                     return () => {
                         $(`[id="${target_id}"]`).val(current_path);
-                        filer_modal.modal(`hide`);
+                        filer_modal.modal('hide');
                         if (call_back_func) call_back_func(current_path);
                     }
                 }
-                $.each(node[`children`], (k, n) => {
-                    if (n[`is_dir`]) return;
-                    tr_elem = $(`<tr/>`);
+                $.each(node['children'], (k, n) => {
+                    if (n['is_dir']) return;
+                    tr_elem = $('<tr/>');
                     table_body.append(tr_elem);
                     td = $(`<td><a href="#" class="folder-close">${n['name']}</a></td>`);
-                    td.find(`a`).click(mk_func(target_id, $(`#${k}`), n[`path`]));
-                    tr_elem.append($(`<td><img src="/assets/tree-menu/image/file.png"></td>`));
+                    td.find('a').click(mk_func(target_id, $(`#${k}`), n['path']));
+                    tr_elem.append($('<td><img src="/assets/tree-menu/image/file.png"></td>'));
                     tr_elem.append(td);
                     tr_elem.append($(`<td>${n['size']}</td>`));
                     tr_elem.append($(`<td>${n['last']}</td>`));
                 });
             }
         }
     }
-    await reload_tree(target_id, filer_modal.find(`.tree-menu`), current_path, filer_modal.find(`.file-list`));
-    filer_modal.modal(`show`);
+    await reload_tree(target_id, filer_modal.find('.tree-menu'), current_path, filer_modal.find('.file-list'));
+    filer_modal.modal('show');
 };
```

### Comparing `iinfer-0.6.9/iinfer/web/assets/iinfer/list_pipe.js` & `iinfer-0.7.0/iinfer/web/assets/iinfer/list_pipe.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,142 +1,141 @@
 // 保存済みパイプラインファイル一覧の取得
 list_pipe_func = async () => {
-    $(`#pipe_items`).html(``);
-    kwd = $(`#pipe_kwd`).val();
-    py_list_pipe = await eel.list_pipe(kwd ? `*${kwd}*` : `*`)();
+    $('#pipe_items').html('');
+    kwd = $('#pipe_kwd').val();
+    py_list_pipe = await eel.list_pipe(kwd ? `*${kwd}*` : '*')();
     $.each(py_list_pipe, (i, row) => {
-        elem = $($(`#pipe_template`).html());
-        elem.find(`.pipe_title`).text(row[`title`]);
-        elem.find(`.pipe_desc`).text(row[`description`]);
-        $(`#pipe_items`).append(elem);
+        elem = $($('#pipe_template').html());
+        elem.find('.pipe_title').text(row['title']);
+        elem.find('.pipe_desc').text(row['description']);
+        $('#pipe_items').append(elem);
     });
-    $(`#pipe_items`).append($($(`#pipe_add`).html()));
+    $('#pipe_items').append($($('#pipe_add').html()));
 }
 list_pipe_func_then = () => {
     // パイプラインカードクリック時の処理（モーダルダイアログを開く）
     pipe_card_func = async (e) => {
-        pipe_modal = $(`#pipe_modal`);
-        pipe_modal.find(`.is-invalid, .is-valid`).removeClass(`is-invalid`).removeClass(`is-valid`);
-        row_content = pipe_modal.find(`.row_content`);
-        row_content.html(``);
-        modal_title = $(e.currentTarget).find(`.pipe_title`).text();
+        pipe_modal = $('#pipe_modal');
+        pipe_modal.find('.is-invalid, .is-valid').removeClass('is-invalid').removeClass('is-valid');
+        row_content = pipe_modal.find('.row_content');
+        row_content.html('');
+        modal_title = $(e.currentTarget).find('.pipe_title').text();
         cmd_select_template_func = (add_buton, py_list_cmd) => {
-            cmd_select_template = $(pipe_modal.find(`.cmd_select_template`).html());
-            row_content = pipe_modal.find(`.row_content`);
-            if (row_content.find(`.cmd_select_item`).length > 0) {
-                add_buton.parents(`.cmd_select_item`).after(cmd_select_template);
+            cmd_select_template = $(pipe_modal.find('.cmd_select_template').html());
+            row_content = pipe_modal.find('.row_content');
+            if (row_content.find('.cmd_select_item').length > 0) {
+                add_buton.parents('.cmd_select_item').after(cmd_select_template);
             } else {
                 row_content.append(cmd_select_template);
-                cmd_select_template.find(`[name="pipe_cmd"]`).attr(`required`, true);
-                cmd_select_template.find(`.del_buton`).hide();
+                cmd_select_template.find('[name="pipe_cmd"]').attr('required', true);
+                cmd_select_template.find('.del_buton').hide();
             }
-            pipe_cmd_select = cmd_select_template.find(`[name="pipe_cmd"]`);
-            pipe_cmd_select.append(`<option></option>`);
+            pipe_cmd_select = cmd_select_template.find('[name="pipe_cmd"]');
+            pipe_cmd_select.append('<option></option>');
             $.each(py_list_cmd, (i, cmd) => {
-                option = $(`<option></option>`);
+                option = $('<option></option>');
                 pipe_cmd_select.append(option);
-                option.attr(`value`, cmd[`title`]);
+                option.attr('value', cmd['title']);
                 option.text(`${cmd['title']}(mode=${cmd['mode']}, cmd=${cmd['cmd']})`);
             });
-            cmd_select_template.find(`.add_buton`).click((e) => {
+            cmd_select_template.find('.add_buton').click((e) => {
                 cmd_select_template_func($(e.currentTarget), py_list_cmd);
             });
-            cmd_select_template.find(`.del_buton`).click((e) => {
-                $(e.currentTarget).parents(`.cmd_select_item`).remove();
+            cmd_select_template.find('.del_buton').click((e) => {
+                $(e.currentTarget).parents('.cmd_select_item').remove();
             });
             return cmd_select_template;
         }
-        if (modal_title != ``) {
+        if (modal_title != '') {
             // パイプラインファイルの読み込み
             py_list_cmd = await eel.list_cmd(null)();
-            cmd_select = cmd_select_template_func(pipe_modal.find(`.add_buton`), py_list_cmd)
+            cmd_select = cmd_select_template_func(pipe_modal.find('.add_buton'), py_list_cmd)
             py_load_pipe = await eel.load_pipe(modal_title)();
             $.each(py_load_pipe, (key, val) => {
-                if (typeof val === `boolean`) {
+                if (typeof val === 'boolean') {
                     val = val.toString();
                 }
                 // フォームに値をセット
                 if (Array.isArray(val)) {
                     $.each(val, (i, v) => {
-                        e = pipe_modal.find(`[name="${key}"]`).parent().find(`.add_buton`)[i];
+                        e = pipe_modal.find(`[name="${key}"]`).parent().find('.add_buton')[i];
                         $(e).click();
                     });
                     pipe_modal.find(`[name="${key}"]`).each((i, e) => {
-                        $(e).val(val[i]);
+                        if (val[i] && val[i] != "" || i == 0) $(e).val(val[i]);
+                        else $(e).parent().find('.del_buton').click();
                     });
                 } else {
                     pipe_modal.find(`[name="${key}"]`).val(val);
                 }
             });
-            $(`#cmd_del`).show();
-            pipe_modal.find(`[name="title"]`).attr(`readonly`, true);
+            $('#cmd_del').show();
+            pipe_modal.find('[name="title"]').attr('readonly', true);
         } else {
             // 新規パイプラインファイルの作成
-            modal_title = `New Pipeline`;
-            $(`#cmd_del`).hide();
-            pipe_modal.find(`[name="title"]`).val(``);
-            pipe_modal.find(`[name="title"]`).attr(`readonly`, false);
-            pipe_modal.find(`[name="description"]`).val(``);
+            modal_title = 'New Pipeline';
+            $('#cmd_del').hide();
+            pipe_modal.find('[name="title"]').val('');
+            pipe_modal.find('[name="title"]').attr('readonly', false);
+            pipe_modal.find('[name="description"]').val('');
             py_list_cmd = await eel.list_cmd(null)();
-            cmd_select = cmd_select_template_func(pipe_modal.find(`.add_buton`), py_list_cmd)
+            cmd_select = cmd_select_template_func(pipe_modal.find('.add_buton'), py_list_cmd)
         }
-        pipe_modal.find(`.modal-title`).text(`Pipeline : ${modal_title}`);
-        pipe_modal.modal(`show`);
+        pipe_modal.find('.modal-title').text(`Pipeline : ${modal_title}`);
+        pipe_modal.modal('show');
     }
-    $(`.pipe_card`).off(`click`).on('click', pipe_card_func);
+    $('.pipe_card').off('click').on('click', pipe_card_func);
     // パイプラインファイルの保存
-    $(`#pipe_save`).off(`click`).on('click', async () => {
-        pipe_modal = $(`#pipe_modal`);
+    $('#pipe_save').off('click').on('click', async () => {
+        pipe_modal = $('#pipe_modal');
         var [title, opt] = get_param(pipe_modal);
-        if (pipe_modal.find(`.row_content, .row_content_common`).find(`.is-invalid`).length > 0) {
+        if (pipe_modal.find('.row_content, .row_content_common').find('.is-invalid').length > 0) {
             return;
         }
-        $(`#loading`).removeClass(`d-none`);
-        await eel.save_pipe(title, opt)();
+        $('#loading').removeClass('d-none');
+        result = await eel.save_pipe(title, opt)();
         await list_pipe_func();
-        $(`.pipe_card`).off(`click`).on('click', pipe_card_func);
-        window.alert(`save success.`);
-        $(`#loading`).addClass(`d-none`);
+        $('.pipe_card').off('click').on('click', pipe_card_func);
+        if (result['success']) alert(result['success']);
+        else if (result['warn']) alert(result['warn']);
+        $('#loading').addClass('d-none');
     });
     // パイプラインファイルの削除
-    $(`#pipe_del`).off(`click`).on('click', async () => {
-        pipe_modal = $(`#pipe_modal`);
-        var title = pipe_modal.find(`[name="title"]`).val();
-        $(`#loading`).removeClass(`d-none`);
+    $('#pipe_del').off('click').on('click', async () => {
+        pipe_modal = $('#pipe_modal');
+        var title = pipe_modal.find('[name="title"]').val();
+        $('#loading').removeClass('d-none');
         if (window.confirm(`delete "${title}"?`)) {
             await eel.del_pipe(title)();
-            pipe_modal.modal(`hide`);
+            pipe_modal.modal('hide');
             await list_pipe_func();
-            $(`.pipe_card`).off(`click`).on('click', pipe_card_func);
+            $('.pipe_card').off('click').on('click', pipe_card_func);
         }
-        $(`#loading`).addClass(`d-none`);
+        $('#loading').addClass('d-none');
     });
     // パイプラインファイルの実行
-    $(`#pipe_exec`).off(`click`).on('click', async () => {
-        pipe_modal = $(`#pipe_modal`);
+    $('#pipe_exec').off('click').on('click', async () => {
+        pipe_modal = $('#pipe_modal');
         var [title, opt] = get_param(pipe_modal);
-        if (pipe_modal.find(`.row_content`).find(`.is-invalid`).length > 0) {
+        if (pipe_modal.find('.row_content').find('.is-invalid').length > 0) {
             return;
         }
-        $(`#loading`).removeClass(`d-none`);
+        $('#loading').removeClass('d-none');
         // コマンドの実行
-        eel.exec_pipe(title, opt)().then((result) => {
-            pipe_modal.modal(`hide`);
-            view_result_func(title, result);
-            $(`#loading`).addClass(`d-none`);
-        });
+        $('#loading').find('.bbforce').addClass('pipe_executed');
+        eel.exec_pipe(title, opt)().then((result) => {});
     });
     // RAW表示の実行
-    $(`#pipe_raw`).off(`click`).on('click', async () => {
-        pipe_modal = $(`#pipe_modal`);
+    $('#pipe_raw').off('click').on('click', async () => {
+        pipe_modal = $('#pipe_modal');
         var [title, opt] = get_param(pipe_modal);
-        if (pipe_modal.find(`.row_content`).find(`.is-invalid`).length > 0) {
+        if (pipe_modal.find('.row_content').find('.is-invalid').length > 0) {
             return;
         }
-        $(`#loading`).removeClass(`d-none`);
+        $('#loading').removeClass('d-none');
         // コマンドの実行
         eel.raw_pipe(title, opt)().then((result) => {
             view_raw_func(title, result);
-            $(`#loading`).addClass(`d-none`);
+            $('#loading').addClass('d-none');
         });
     });
 };
```

### Comparing `iinfer-0.6.9/iinfer/web/assets/iinfer/main.js` & `iinfer-0.7.0/iinfer/web/assets/iinfer/main.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,111 +1,138 @@
 change_dark_mode = (dark_mode) => {
-    html = $(`html`);
-    if (dark_mode) html.attr(`data-bs-theme`, `dark`);
-    else if (html.attr(`data-bs-theme`) == `dark`) html.removeAttr(`data-bs-theme`);
-    else html.attr(`data-bs-theme`, `dark`);
+    html = $('html');
+    if (dark_mode) html.attr('data-bs-theme', 'dark');
+    else if (html.attr('data-bs-theme') == 'dark') html.removeAttr('data-bs-theme');
+    else html.attr('data-bs-theme', 'dark');
 }
 $(() => {
     // ダークモード対応
-    change_dark_mode(window.matchMedia(`(prefers-color-scheme: dark)`).matches);
+    change_dark_mode(window.matchMedia('(prefers-color-scheme: dark)').matches);
     // copyright情報取得
     copyright_func = async () => {
         copyright = await eel.copyright()();
-        $(`.copyright`).text(copyright);
+        $('.copyright').text(copyright);
     };
     copyright_func();
     // コマンド一覧の取得と表示
     list_cmd_func().then(list_cmd_func_then);
     // コマンド一覧の検索
-    $('#cmd_kwd').off(`change`).on(`change`, (e) => list_cmd_func().then(list_cmd_func_then));
+    $('#cmd_kwd').off('change').on('change', (e) => list_cmd_func().then(list_cmd_func_then));
     // パイプライン一覧の取得と表示
     list_pipe_func().then(list_pipe_func_then);
     // パイプライン一覧の検索
-    $('#pipe_kwd').off(`change`).on(`change`, (e) => list_pipe_func().then(list_pipe_func_then));
+    $('#pipe_kwd').off('change').on('change', (e) => list_pipe_func().then(list_pipe_func_then));
 
-    $(`#versions_modal`).on(`shown.bs.modal	`, () => {
+    $('#versions_modal').on('shown.bs.modal	', () => {
         // iinferのバージョン情報取得
         versions_iinfer_func = async () => {
             versions_iinfer = await eel.versions_iinfer()();
-            $(`#versions_iinfer`).html(``);
+            $('#versions_iinfer').html('');
             $.each(versions_iinfer, (i, v) => {
-                v = v.replace(/<([^>]+)>/g, `<a href="$1" target="_blank">$1</a>`);
-                div = $(`<div class="d-block"></div>`);
-                $(`#versions_iinfer`).append(div);
+                v = v.replace(/<([^>]+)>/g, '<a href="$1" target="_blank">$1</a>');
+                div = $('<div class="d-block"></div>');
+                $('#versions_iinfer').append(div);
                 if (i == 0) {
-                    div.addClass(`m-3`);
+                    div.addClass('m-3');
                     div.append(`<h4>${v}</h4>`);
                 } else {
-                    div.addClass(`ms-5 me-5`);
+                    div.addClass('ms-5 me-5');
                     div.append(`<h6>${v}</h6>`);
                 }
             });
         };
         versions_iinfer_func();
         // usedのバージョン情報取得
         versions_used_func = async () => {
             versions_used = await eel.versions_used()();
-            $(`#versions_used`).html(``);
-            div = $(`<div class="overflow-auto" style="height:calc(100vh - 260px);"></div>`);
-            table = $(`<table class="table table-bordered table-hover table-sm"></table>`);
-            table_head = $(`<thead class="table-dark bg-dark"></thead>`);
-            table_body = $(`<tbody></tbody>`);
+            $('#versions_used').html('');
+            div = $('<div class="overflow-auto" style="height:calc(100vh - 260px);"></div>');
+            table = $('<table class="table table-bordered table-hover table-sm"></table>');
+            table_head = $('<thead class="table-dark bg-dark"></thead>');
+            table_body = $('<tbody></tbody>');
             table.append(table_head);
             table.append(table_body);
             div.append(table);
-            $(`#versions_used`).append(div);
+            $('#versions_used').append(div);
             $.each(versions_used, (i, row) => {
-                tr = $(`<tr></tr>`);
+                tr = $('<tr></tr>');
                 $.each(row, (j, cel) => {
-                    td = $(`<td></td>`).text(cel);
+                    td = $('<td></td>').text(cel);
                     tr.append(td);
                 });
                 if (i == 0) table_head.append(tr);
                 else table_body.append(tr);
             });
         };
         versions_used_func();
     })
 
     // modal setting
-    $(`.modal-dialog`).draggable({
-        cursor: "move",
-        cancel: ".modal-body"
-    });
-    $(`#filer_modal .modal-dialog`).draggable({
-        cursor: "move",
-        cancel: ".modal-body, .filer_address"
-    });
-    $(`.btn_window_stack`).off(`click`).on('click', () => {
-        $(`.btn_window_stack`).css(`margin-left`, `0px`).hide();
-        $(`.btn_window`).css(`margin-left`, `auto`).show();
-        $(`.btn_window_stack`).parents(`.modal-dialog`).removeClass(`modal-fullscreen`);
-    });
-    $(`.btn_window`).off(`click`).on('click', () => {
-        $(`.btn_window_stack`).css(`margin-left`, `auto`).show();
-        $(`.btn_window`).css(`margin-left`, `0px`).hide();
-        $(`.btn_window_stack`).parents(`.modal-dialog`).addClass(`modal-fullscreen`);
+    $('.modal-dialog').draggable({
+        cursor: 'move',
+        cancel: '.modal-body'
+    });
+    $('#filer_modal .modal-dialog').draggable({
+        cursor: 'move',
+        cancel: '.modal-body, .filer_address'
+    });
+    $('.btn_window_stack').off('click').on('click', () => {
+        $('.btn_window_stack').css('margin-left', '0px').hide();
+        $('.btn_window').css('margin-left', 'auto').show();
+        $('.btn_window_stack').parents('.modal-dialog').removeClass('modal-fullscreen');
+    });
+    $('.btn_window').off('click').on('click', () => {
+        $('.btn_window_stack').css('margin-left', 'auto').show();
+        $('.btn_window').css('margin-left', '0px').hide();
+        $('.btn_window_stack').parents('.modal-dialog').addClass('modal-fullscreen');
+    });
+    $('.btn_window_stack').css('margin-left', '0px').hide();
+    $('.btn_window').css('margin-left', 'auto').show();
+    $('.bbforce').off('click').on('click', async () => {
+        if ($('#loading').find('.bbforce').hasClass('pipe_executed') &&
+            window.confirm('パイプラインでこのアクションを実行すると、guiモード自体が停止します。実行しますか？')) {
+            await eel.bbforce_cmd()();
+            $('#loading').addClass('d-none');
+            window.close();
+        } else if (!$('#loading').find('.bbforce').hasClass('pipe_executed')) {
+            await eel.bbforce_cmd()();
+            $('#loading').addClass('d-none');
+        }
     });
-    $(`.btn_window_stack`).css(`margin-left`, `0px`).hide();
-    $(`.btn_window`).css(`margin-left`, `auto`).show();
 
     // disable F5 and Ctrl+R
-    $(document).on(`keydown`, (e) => {
+    $(document).on('keydown', (e) => {
         if ((e.which || e.keyCode) == 116) {
             return false;
         } else if ((e.which || e.keyCode) == 82 && e.ctrlKey) {
             return false;
         }
     });
-    $(window).on("beforeunload", () => {
+    /*$(window).on('beforeunload', () => {
         event.preventDefault();
-        event.returnValue = `Check`;
-    });
+        event.returnValue = 'Check';
+    });*/
     eel.expose(js_console_modal_log_func);
 
     function js_console_modal_log_func(line) {
-        elem = $(`#console_modal_log`);
+        elem = $('#console_modal_log');
         text = elem.val() + line;
         elem.val(text);
         elem.get(0).setSelectionRange(text.length - 1, text.length - 1);
     };
+    eel.expose(js_return_cmd_exec_func);
+
+    function js_return_cmd_exec_func(title, result) {
+        cmd_modal = $('#cmd_modal');
+        cmd_modal.modal('hide');
+        view_result_func(title, result);
+        $('#loading').addClass('d-none');
+    }
+    eel.expose(js_return_pipe_exec_func);
+
+    function js_return_pipe_exec_func(title, result) {
+        pipe_modal = $('#pipe_modal');
+        pipe_modal.modal('hide');
+        view_result_func(title, result);
+        $('#loading').addClass('d-none');
+    }
 });
```

### Comparing `iinfer-0.6.9/iinfer/web/assets/iinfer/svfiler.js` & `iinfer-0.7.0/iinfer/web/assets/iinfer/svfiler.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,80 +1,80 @@
 const filer = (svpath) => {
-    const modal = $("#svfiler_modal").length ? $("#svfiler_modal") : $(
-        `<div id="svfiler_modal" class="modal" tabindex="-1">` +
-        `<div class="modal-dialog modal-lg">` +
-        `<div id="result_form" class="modal-content novalidate">` +
-        `<div class="modal-header">` +
-        `<div class="input-group p-1">` +
-        `<button class="btn btn-outline-secondary dropdown-toggle filer_server_bot" type="button" data-bs-toggle="dropdown" aria-expanded="false">Server</button>` +
-        `<ul class="dropdown-menu filer_server"><li class="mb-3 p-3">` +
-        `<div class="col-12">` +
-        `<div class="input-group">` +
-        `<label class="input-group-text text-decoration-underline"><span class="text-danger">*</span>host</label>` +
-        `<input name="filer_host" type="text" class="form-control filer_host" param_data_type="str" param_data_multi="false" required>` +
-        `</div>` +
-        `</div>` +
-        `<div class="col-12">` +
-        `<div class="input-group">` +
-        `<label class="input-group-text text-decoration-underline"><span class="text-danger">*</span>port</label>` +
-        `<input name="filer_port" type="text" class="form-control filer_port" param_data_type="int" param_data_multi="false" required>` +
-        `</div>` +
-        `</div>` +
-        `<div class="col-12">` +
-        `<div class="input-group">` +
-        `<label class="input-group-text text-decoration-underline"><span class="text-danger">*</span>password</label>` +
-        `<input name="filer_password" type="text" class="form-control filer_password" param_data_type="str" param_data_multi="false" required>` +
-        `<input name="filer_svname" type="hidden" class="filer_svname">` +
-        `</div>` +
-        `</div>` +
-        `</li><li><hr class="dropdown-divider"></li></ul>` +
-        `<input type="text" class="form-control filer_address" aria-describedby="button-addon2">` +
-        `<button class="btn btn-outline-secondary filer_address_bot" type="button" id="button-addon2">` +
-        `<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-right-circle" viewBox="0 0 16 16">` +
-        `<path fill-rule="evenodd" d="M1 8a7 7 0 1 0 14 0A7 7 0 0 0 1 8zm15 0A8 8 0 1 1 0 8a8 8 0 0 1 16 0zM4.5 7.5a.5.5 0 0 0 0 1h5.793l-2.147 2.146a.5.5 0 0 0 .708.708l3-3a.5.5 0 0 0 0-.708l-3-3a.5.5 0 1 0-.708.708L10.293 7.5H4.5z"/>` +
-        `</svg>` +
-        `</button>` +
-        `</div>` +
-        `<button type="button" class="btn btn_window_stack">` +
-        `<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-window-stack" viewBox="0 0 16 16">` +
-        `<path d="M4.5 6a.5.5 0 1 0 0-1 .5.5 0 0 0 0 1ZM6 6a.5.5 0 1 0 0-1 .5.5 0 0 0 0 1Zm2-.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0Z"/>` +
-        `<path d="M12 1a2 2 0 0 1 2 2 2 2 0 0 1 2 2v8a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2 2 2 0 0 1-2-2V3a2 2 0 0 1 2-2h10ZM2 12V5a2 2 0 0 1 2-2h9a1 1 0 0 0-1-1H2a1 1 0 0 0-1 1v8a1 1 0 0 0 1 1Zm1-4v5a1 1 0 0 0 1 1h10a1 1 0 0 0 1-1V8H3Zm12-1V5a1 1 0 0 0-1-1H4a1 1 0 0 0-1 1v2h12Z"/>` +
-        `</svg>` +
-        `</button>` +
-        `<button type="button" class="btn btn_window">` +
-        `<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-window" viewBox="0 0 16 16">` +
-        `<path d="M2.5 4a.5.5 0 1 0 0-1 .5.5 0 0 0 0 1zm2-.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0zm1 .5a.5.5 0 1 0 0-1 .5.5 0 0 0 0 1z"/>` +
-        `<path d="M2 1a2 2 0 0 0-2 2v10a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V3a2 2 0 0 0-2-2H2zm13 2v2H1V3a1 1 0 0 1 1-1h12a1 1 0 0 1 1 1zM2 14a1 1 0 0 1-1-1V6h14v7a1 1 0 0 1-1 1H2z"/>` +
-        `</svg>` +
-        `</button>` +
-        `<button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close" style="margin-left: 0px;"></button>` +
-        `</div>` +
-        `<div class="modal-body row">` +
-        `<ul class="tree-menu tree_ul overflow-auto border col-4" style="height:calc(100vh - 240px)"></ul>` +
-        `<div class="file-list drop-area overflow-auto col-8 p-1" style="height:calc(100vh - 240px)"></div>` +
-        `<div class="progress p-0 d-none" role="progressbar" aria-valuenow="0" aria-valuemin="0" aria-valuemax="100">` +
-        `<div class="progress-bar progress-bar-striped progress-bar-animated bg-success" style="width: 0%"></div>` +
-        `</div>` +
-        `<a class="filer_download d-none" href="#">.</a>` +
-        `</div>` +
-        `<div class="modal-footer">` +
-        `<button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>` +
-        `</div>` +
-        `</div>` +
-        `</div>` +
-        `</div>`
+    const modal = $('#svfiler_modal').length ? $('#svfiler_modal') : $(
+        '<div id="svfiler_modal" class="modal" tabindex="-1">' +
+        '<div class="modal-dialog modal-lg">' +
+        '<div id="result_form" class="modal-content novalidate">' +
+        '<div class="modal-header">' +
+        '<div class="input-group p-1">' +
+        '<button class="btn btn-outline-secondary dropdown-toggle filer_server_bot" type="button" data-bs-toggle="dropdown" aria-expanded="false">Server</button>' +
+        '<ul class="dropdown-menu filer_server"><li class="mb-3 p-3">' +
+        '<div class="col-12">' +
+        '<div class="input-group">' +
+        '<label class="input-group-text text-decoration-underline"><span class="text-danger">*</span>host</label>' +
+        '<input name="filer_host" type="text" class="form-control filer_host" param_data_type="str" param_data_multi="false" required>' +
+        '</div>' +
+        '</div>' +
+        '<div class="col-12">' +
+        '<div class="input-group">' +
+        '<label class="input-group-text text-decoration-underline"><span class="text-danger">*</span>port</label>' +
+        '<input name="filer_port" type="text" class="form-control filer_port" param_data_type="int" param_data_multi="false" required>' +
+        '</div>' +
+        '</div>' +
+        '<div class="col-12">' +
+        '<div class="input-group">' +
+        '<label class="input-group-text text-decoration-underline"><span class="text-danger">*</span>password</label>' +
+        '<input name="filer_password" type="text" class="form-control filer_password" param_data_type="str" param_data_multi="false" required>' +
+        '<input name="filer_svname" type="hidden" class="filer_svname">' +
+        '</div>' +
+        '</div>' +
+        '</li><li><hr class="dropdown-divider"></li></ul>' +
+        '<input type="text" class="form-control filer_address" aria-describedby="button-addon2">' +
+        '<button class="btn btn-outline-secondary filer_address_bot" type="button" id="button-addon2">' +
+        '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-right-circle" viewBox="0 0 16 16">' +
+        '<path fill-rule="evenodd" d="M1 8a7 7 0 1 0 14 0A7 7 0 0 0 1 8zm15 0A8 8 0 1 1 0 8a8 8 0 0 1 16 0zM4.5 7.5a.5.5 0 0 0 0 1h5.793l-2.147 2.146a.5.5 0 0 0 .708.708l3-3a.5.5 0 0 0 0-.708l-3-3a.5.5 0 1 0-.708.708L10.293 7.5H4.5z"/>' +
+        '</svg>' +
+        '</button>' +
+        '</div>' +
+        '<button type="button" class="btn btn_window_stack">' +
+        '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-window-stack" viewBox="0 0 16 16">' +
+        '<path d="M4.5 6a.5.5 0 1 0 0-1 .5.5 0 0 0 0 1ZM6 6a.5.5 0 1 0 0-1 .5.5 0 0 0 0 1Zm2-.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0Z"/>' +
+        '<path d="M12 1a2 2 0 0 1 2 2 2 2 0 0 1 2 2v8a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2 2 2 0 0 1-2-2V3a2 2 0 0 1 2-2h10ZM2 12V5a2 2 0 0 1 2-2h9a1 1 0 0 0-1-1H2a1 1 0 0 0-1 1v8a1 1 0 0 0 1 1Zm1-4v5a1 1 0 0 0 1 1h10a1 1 0 0 0 1-1V8H3Zm12-1V5a1 1 0 0 0-1-1H4a1 1 0 0 0-1 1v2h12Z"/>' +
+        '</svg>' +
+        '</button>' +
+        '<button type="button" class="btn btn_window">' +
+        '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-window" viewBox="0 0 16 16">' +
+        '<path d="M2.5 4a.5.5 0 1 0 0-1 .5.5 0 0 0 0 1zm2-.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0zm1 .5a.5.5 0 1 0 0-1 .5.5 0 0 0 0 1z"/>' +
+        '<path d="M2 1a2 2 0 0 0-2 2v10a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V3a2 2 0 0 0-2-2H2zm13 2v2H1V3a1 1 0 0 1 1-1h12a1 1 0 0 1 1 1zM2 14a1 1 0 0 1-1-1V6h14v7a1 1 0 0 1-1 1H2z"/>' +
+        '</svg>' +
+        '</button>' +
+        '<button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close" style="margin-left: 0px;"></button>' +
+        '</div>' +
+        '<div class="modal-body row">' +
+        '<ul class="tree-menu tree_ul overflow-auto border col-4" style="height:calc(100vh - 240px)"></ul>' +
+        '<div class="file-list drop-area overflow-auto col-8 p-1" style="height:calc(100vh - 240px)"></div>' +
+        '<div class="progress p-0 d-none" role="progressbar" aria-valuenow="0" aria-valuemin="0" aria-valuemax="100">' +
+        '<div class="progress-bar progress-bar-striped progress-bar-animated bg-success" style="width: 0%"></div>' +
+        '</div>' +
+        '<a class="filer_download d-none" href="#">.</a>' +
+        '</div>' +
+        '<div class="modal-footer">' +
+        '<button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>' +
+        '</div>' +
+        '</div>' +
+        '</div>' +
+        '</div>'
     );
-    const loading = $("#loading").length ? $("#loading") : $(
-        `<div id="loading" class="position-absolute top-0 start-0 w-100 h-100 d-none" style="background:rgba(0, 0, 0, 0.3);z-index:10000;">` +
-        `<div class="text-center position-absolute top-50 start-50 w-100 translate-middle">` +
-        `<div class="spinner-border text-light" role="status">` +
-        `<span class="sr-only"></span>` +
-        `</div>` +
-        `</div>` +
-        `</div>`
+    const loading = $('#loading').length ? $('#loading') : $(
+        '<div id="loading" class="position-absolute top-0 start-0 w-100 h-100 d-none" style="background:rgba(0, 0, 0, 0.3);z-index:10000;">' +
+        '<div class="text-center position-absolute top-50 start-50 w-100 translate-middle">' +
+        '<div class="spinner-border text-light" role="status">' +
+        '<span class="sr-only"></span>' +
+        '</div>' +
+        '</div>' +
+        '</div>'
     );
     const show_loading = () => {
         loading.removeClass('d-none');
     }
     const hide_loading = () => {
         loading.addClass('d-none');
         modal.find('.progress').addClass('d-none');
@@ -102,21 +102,22 @@
         const res = target !== null ? Math.floor((size / target) * 100) / 100 : size
         return `${res} ${unit}`
     };
     // ツリー表示 ================================================================
     const tree = (svpath, current_ul_elem) => {
         show_loading();
         opt = get_server_opt();
-        opt["mode"] = "client";
-        opt["cmd"] = "file_list";
-        opt["svpath"] = svpath;
-        eel.exec_cmd("file_list", opt)().then(async res => {
+        opt['mode'] = 'client';
+        opt['cmd'] = 'file_list';
+        opt['capture_stdout'] = true;
+        opt['svpath'] = svpath;
+        eel.exec_cmd('file_list', opt, true)().then(async res => {
             current_ul_elem.html('');
-            if (res["warn"]) {
-                alert(res["warn"]);
+            if (res['warn']) {
+                alert(res['warn']);
                 hide_loading();
                 return;
             }
             list_tree = res[0]['success'];
             hide_loading();
             // 左側ペイン
             Object.keys(list_tree).map((key) => {
@@ -134,33 +135,33 @@
                 current_li_elem.append(current_a_elem);
                 mk_func = (_p, _e) => {
                     return () => {
                         tree(_p, _e);
                         event.stopPropagation();
                     }
                 }
-                current_a_elem.off("click").on("click", mk_func(node['path'], current_ul_elem));
+                current_a_elem.off('click').on('click', mk_func(node['path'], current_ul_elem));
                 Object.keys(children).map((k, i) => {
                     n = children[k];
                     if (!n['is_dir']) return;
-                    ul_elem = $(`<ul class="tree_ul"/>`).append(`<li id="${k}" data_path="${n['path']}"><a href="#" class="folder-close">${n['name']}</a></li>`);
+                    ul_elem = $('<ul class="tree_ul"/>').append(`<li id="${k}" data_path="${n['path']}"><a href="#" class="folder-close">${n['name']}</a></li>`);
                     current_li_elem.append(ul_elem);
-                    modal.find(`#${k}`).off("click");
-                    modal.find(`#${k}`).on("click", mk_func(n['path'], current_ul_elem));
+                    modal.find(`#${k}`).off('click');
+                    modal.find(`#${k}`).on('click', mk_func(n['path'], current_ul_elem));
                 });
             });
             // 右側ペイン
             list_tree_keys = Object.keys(list_tree);
             if (list_tree_keys.length > 0) {
                 node = list_tree[list_tree_keys[list_tree_keys.length - 1]];
-                modal.find(".filer_address").val(node['path']);
-                table = $(`<table class="table table-bordered table-hover table-sm">` +
-                    `<thead class="table-dark bg-dark"><tr><th scope="col">-</th><th scope="col">name</th><th scope="col">size</th><th scope="col">last</th></tr></thead>` +
-                    `</table>`);
-                table_body = $(`<tbody></tbody>`);
+                modal.find('.filer_address').val(node['path']);
+                table = $('<table class="table table-bordered table-hover table-sm">' +
+                    '<thead class="table-dark bg-dark"><tr><th scope="col">-</th><th scope="col">name</th><th scope="col">size</th><th scope="col">last</th></tr></thead>' +
+                    '</table>');
+                table_body = $('<tbody></tbody>');
                 modal.find('.file-list').html('');
                 modal.find('.file-list').append(table);
                 table.append(table_body);
                 children = node['children'];
                 if (children) {
                     // ツリー表示関数の生成
                     mk_tree = (_p, _e) => {
@@ -169,25 +170,26 @@
                     // 削除関数の生成
                     mk_delete = (_p, _e, is_dir) => {
                         return () => {
                             if (confirm(`「${_p}」を削除しますか？${is_dir?"\n【注意】ディレクトリの場合は中身も削除されます。":""}`)) {
                                 remote = is_dir ? 'file_rmdir' : 'file_remove';
                                 show_loading();
                                 opt = get_server_opt();
-                                opt["mode"] = "client";
-                                opt["cmd"] = remote;
-                                opt["svpath"] = _p;
-                                eel.exec_cmd(remote, opt)().then(async res => {
-                                    if (res["warn"]) {
-                                        alert(res["warn"]);
+                                opt['mode'] = 'client';
+                                opt['cmd'] = remote;
+                                opt['capture_stdout'] = true;
+                                opt['svpath'] = _p;
+                                eel.exec_cmd(remote, opt, true)().then(async res => {
+                                    if (res['warn']) {
+                                        alert(res['warn']);
                                         hide_loading();
                                         return;
                                     }
                                     hide_loading();
-                                    tree(res[0]["success"]["path"], _e);
+                                    tree(res[0]['success']['path'], _e);
                                 }).then(() => {
                                     hide_loading();
                                 }, (error) => {
                                     console.log(error);
                                     hide_loading();
                                 });
                             }
@@ -203,20 +205,21 @@
                         return blob;
                     }
                     // ダウンロード関数の生成
                     mk_download = (_p) => {
                         return () => {
                             show_loading();
                             opt = get_server_opt();
-                            opt["mode"] = "client";
-                            opt["cmd"] = "file_download";
-                            opt["svpath"] = _p;
-                            eel.exec_cmd("file_download", opt)().then(async res => {
-                                if (res["warn"]) {
-                                    alert(res["warn"]);
+                            opt['mode'] = 'client';
+                            opt['cmd'] = 'file_download';
+                            opt['capture_stdout'] = true;
+                            opt['svpath'] = _p;
+                            eel.exec_cmd('file_download', opt, true)().then(async res => {
+                                if (res['warn']) {
+                                    alert(res['warn']);
                                     hide_loading();
                                     return;
                                 }
                                 blob = mk_blob(res[0]['success']['data']);
                                 link = modal.find('.filer_download');
                                 link.attr('download', res[0]['success']['name']);
                                 link.get(0).href = window.URL.createObjectURL(blob);
@@ -230,68 +233,69 @@
                             });
                         }
                     };
                     // フォルダ作成関数の生成
                     mk_mkdir = (_p, _e, is_dir) => {
                         return () => {
                             _p = _p.substring(0, _p.lastIndexOf('/') + 1);
-                            prompt_text = prompt("Enter a new folder name.");
+                            prompt_text = prompt('Enter a new folder name.');
                             if (prompt_text) {
                                 show_loading();
                                 opt = get_server_opt();
-                                opt["mode"] = "client";
-                                opt["cmd"] = "file_mkdir";
-                                opt["svpath"] = `${_p}/${prompt_text}`;
-                                eel.exec_cmd("file_mkdir", opt)().then(async res => {
-                                    if (res["warn"]) {
-                                        alert(res["warn"]);
+                                opt['mode'] = 'client';
+                                opt['cmd'] = 'file_mkdir';
+                                opt['capture_stdout'] = true;
+                                opt['svpath'] = `${_p}/${prompt_text}`;
+                                eel.exec_cmd('file_mkdir', opt, true)().then(async res => {
+                                    if (res['warn']) {
+                                        alert(res['warn']);
                                         hide_loading();
                                         return;
                                     }
                                     hide_loading();
-                                    tree(res[0]["success"]["path"], _e);
+                                    tree(res[0]['success']['path'], _e);
                                 }).then(() => {
                                     hide_loading();
                                 }, (error) => {
                                     console.log(error);
                                     hide_loading();
                                 });
                             }
                         }
                     };
                     // ファイルリストの生成
                     mk_tr = (_p, _e, is_dir) => {
                         png = is_dir ? 'folder-close.png' : 'file.png';
-                        dt = is_dir ? '-' : new Date(n['last']).toLocaleDateString("ja-JP", {
-                            year: "numeric",
-                            month: "2-digit",
-                            day: "2-digit",
-                            hour: "2-digit",
-                            minute: "2-digit",
-                            second: "2-digit"
+                        dt = is_dir ? '-' : new Date(n['last']).toLocaleDateString('ja-JP', {
+                            year: 'numeric',
+                            month: '2-digit',
+                            day: '2-digit',
+                            hour: '2-digit',
+                            minute: '2-digit',
+                            second: '2-digit'
                         });
-                        tr = $(`<tr>` +
+                        tr = $('<tr>' +
                             `<td><img src="/assets/tree-menu/image/${png}"></td>` +
-                            `<td>` +
-                            `<div class="droudown">` +
+                            '<td>' +
+                            '<div class="droudown">' +
                             `<a class="dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">${n['name']}</a>` +
-                            `<ul class="dropdown-menu"/>` +
-                            `</div>` +
-                            `</td>` +
+                            '<ul class="dropdown-menu"/>' +
+                            '</div>' +
+                            '</td>' +
                             `<td class="text-end">${calc_size(n['size'])}</td>` +
                             `<td class="text-end">${dt}</td>` +
-                            `</tr>`);
+                            '</tr>');
                         if (is_dir) {
-                            tr.find('.dropdown-menu').append(`<li><a class="dropdown-item open" href="#">Open</a></li>`);
-                            tr.find('.dropdown-menu').append(`<li><a class="dropdown-item mkdir" href="#">Create Folder</a></li>`);
-                            tr.find('.dropdown-menu').append(`<li><a class="dropdown-item delete" href="#">Delete</a></li>`);
+                            tr.find('.dropdown-menu').append('<li><a class="dropdown-item open" href="#">Open</a></li>');
+                            tr.find('.dropdown-menu').append('<li><a class="dropdown-item mkdir" href="#">Create Folder</a></li>');
+                            tr.find('.dropdown-menu').append('<li><a class="dropdown-item delete" href="#">Delete</a></li>');
                         } else {
-                            tr.find('.dropdown-menu').append(`<li><a class="dropdown-item download" href="#">Download</a></li>`);
-                            tr.find('.dropdown-menu').append(`<li><a class="dropdown-item mkdir" href="#">Create Folder</a></li>`);
-                            tr.find('.dropdown-menu').append(`<li><a class="dropdown-item delete" href="#">Delete</a></li>`);
+                            tr.find('.dropdown-menu').append('<li><a class="dropdown-item download" href="#">Download</a></li>');
+                            tr.find('.dropdown-menu').append('<li><a class="dropdown-item mkdir" href="#">Create Folder</a></li>');
+                            tr.find('.dropdown-menu').append('<li><a class="dropdown-item delete" href="#">Delete</a></li>');
                         }
                         tr.find('.open').off('click').on('click', mk_tree(_p, _e));
                         tr.find('.delete').off('click').on('click', mk_delete(_p, _e, is_dir));
                         tr.find('.mkdir').off('click').on('click', mk_mkdir(_p, _e, is_dir));
                         tr.find('.download').off('click').on('click', mk_download(_p));
                         return tr;
                     };
@@ -353,26 +357,27 @@
     }
     const load_server_list = () => {
         show_loading();
         modal.find('.filer_svnames').remove();
         opt = get_server_opt();
         opt['mode'] = 'server';
         opt['cmd'] = 'list';
+        opt["capture_stdout"] = true;
         delete opt['svname'];
-        eel.exec_cmd("server_list", opt)().then(async res => {
+        eel.exec_cmd("server_list", opt, true)().then(async res => {
             if (res["warn"]) {
                 alert(res["warn"]);
                 hide_loading();
                 return;
             }
-            if (res.length <= 0 || !res[0][`success`]) {
+            if (res.length <= 0 || !res[0]['success']) {
                 hide_loading();
                 return;
             }
-            res[0][`success`].forEach(elem => {
+            res[0]['success'].forEach(elem => {
                 a_elem = $(`<a class="dropdown-item" href="#" data-host="${opt['host']}" data-port="${opt['port']}" data-password="${opt['password']}" data-svname="${elem['svname']}">${elem['svname']} ( ${opt['host']}:${opt['port']} )</a>`);
                 mk_func = (elem) => {
                     return () => {
                         modal.find('.filer_host').val(elem.attr('data-host'));
                         modal.find('.filer_port').val(elem.attr('data-port'));
                         modal.find('.filer_password').val(elem.attr('data-password'));
                         modal.find('.filer_svname').val(elem.attr('data-svname'));
@@ -380,15 +385,15 @@
                         localStorage.setItem('filer_port', elem.attr('data-port'));
                         localStorage.setItem('filer_password', elem.attr('data-password'));
                         localStorage.setItem('filer_svname', elem.attr('data-svname'));
                         tree("/", modal.find('.tree-menu'))
                     }
                 };
                 a_elem.off("click").on("click", mk_func(a_elem));
-                li_elem = $(`<li class="filer_svnames"></li>`).append(a_elem);
+                li_elem = $('<li class="filer_svnames"></li>').append(a_elem);
                 modal.find('.filer_server').append(li_elem);
             });
             modal.find('.filer_server').find('.dropdown-item:first').click();
         }).then(() => {
             hide_loading();
         }, (error) => {
             console.log(error);
@@ -415,16 +420,16 @@
                 maxwidth = prog_elem.css('width');
                 maxwidth = parseInt(maxwidth.replace('px', ''));
                 left = bar_elem.css('left');
                 if (!left || left == 'auto') left = 0;
                 else left = parseInt(left.replace('px', ''));
                 if (left > maxwidth) left = -200;
                 left += 2;
-                bar_elem.css('width', `200px`).css('position', 'relative').css('left', `${left}px`);
-                bar_elem.text(`Server processing...`);
+                bar_elem.css('width', '200px').css('position', 'relative').css('left', `${left}px`);
+                bar_elem.text('Server processing...');
                 var progress_handle = setTimeout(() => {
                     if (!loading.is('.d-none')) progress(_min, _max, _now, _text, _show, _cycle);
                 }, 20);
             }
         }
         // https://qiita.com/KokiSakano/items/a122bc0a1a368c697643
         const files = [];
```

### Comparing `iinfer-0.6.9/iinfer/web/assets/iinfer/view_raw.js` & `iinfer-0.7.0/iinfer/web/assets/iinfer/view_raw.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,27 +1,31 @@
 // RAW結果をモーダルダイアログに表示
 view_raw_func = (title, result) => {
-    result_modal = $(`#result_modal`);
-    result_modal.find(`.modal-title`).text(title);
-    result_modal.find(`.modal-body`).html(``);
-    table = $(`<table class="table table-bordered table-hover table-sm"></table>`);
-    table_head = $(`<thead class="table-dark bg-dark"></thead>`);
-    table_body = $(`<tbody></tbody>`);
+    result_modal = $('#result_modal');
+    result_modal.find('.modal-title').text(title);
+    result_modal.find('.modal-body').html('');
+    table = $('<table class="table table-bordered table-hover table-sm"></table>');
+    table_head = $('<thead class="table-dark bg-dark"></thead>');
+    table_body = $('<tbody></tbody>');
     table.append(table_head);
     table.append(table_body);
-    result_modal.find(`.modal-body`).append(table);
+    result_modal.find('.modal-body').append(table);
     // list型の結果をテーブルに変換
     list2table = (data, table_head, table_body) => {
         $.each(data, (i, row) => {
-            tr = $(`<tr></tr>`);
-            $.each(row, (key, val) => {
-                if (i == 0) {
-                    table_head.append($(`<th scope="col">${key}</th>`));
-                }
-                tr.append($(`<td>${val}</td>`));
-            });
+            tr = $('<tr></tr>');
+            if (typeof row === 'string') {
+                tr.append($(`<td>${row}</td>`));
+            } else {
+                $.each(row, (key, val) => {
+                    if (i == 0) {
+                        table_head.append($(`<th scope="col">${key}</th>`));
+                    }
+                    tr.append($(`<td>${val}</td>`));
+                });
+            }
             table_body.append(tr);
         });
     }
     list2table(result, table_head, table_body);
-    result_modal.modal(`show`);
+    result_modal.modal('show');
 }
```

### Comparing `iinfer-0.6.9/iinfer/web/assets/iinfer/view_result.js` & `iinfer-0.7.0/iinfer/web/assets/iinfer/view_result.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,95 +1,95 @@
 // 実行結果をモーダルダイアログに表示
 view_result_func = (title, result) => {
-    result_modal = $(`#result_modal`);
-    result_modal.find(`.modal-title`).text(title);
-    result_modal.find(`.modal-body`).html(``);
+    result_modal = $('#result_modal');
+    result_modal.find('.modal-title').text(title);
+    result_modal.find('.modal-body').html('');
     mk_table_func = () => {
-        table = $(`<table class="table table-bordered table-hover table-sm"></table>`);
-        table_head = $(`<thead class="table-dark bg-dark"></thead>`);
-        table_body = $(`<tbody></tbody>`);
+        table = $('<table class="table table-bordered table-hover table-sm"></table>');
+        table_head = $('<thead class="table-dark bg-dark"></thead>');
+        table_body = $('<tbody></tbody>');
         table.append(table_head);
         table.append(table_body);
         return table;
     }
-    result_modal.find(`.modal-body`).append(mk_table_func());
+    result_modal.find('.modal-body').append(mk_table_func());
     // list型の結果をテーブルに変換
     list2table = (data, table_head, table_body) => {
         $.each(data, (i, row) => {
-            if (row[`success`] && typeof row[`success`] == "object" && !Array.isArray(row[`success`])) {
-                dict2table(row[`success`], i == 0 ? table_head : null, table_body, row[`output_image`]);
+            if (row['success'] && typeof row['success'] == "object" && !Array.isArray(row['success'])) {
+                dict2table(row['success'], i == 0 ? table_head : null, table_body, row['output_image']);
                 return;
             }
-            if (typeof row == `string` || row instanceof String) {
-                tr = $(`<tr></tr>`);
+            if (typeof row == 'string' || row instanceof String) {
+                tr = $('<tr></tr>');
                 table_body.append(tr);
                 tr.append($(`<td>${row}</td>`));
                 return;
             }
-            tr = $(`<tr></tr>`);
+            tr = $('<tr></tr>');
             table_body.append(tr);
             $.each(row, (key, val) => {
                 if (i == 0) {
                     table_head.append($(`<th scope="col">${key}</th>`));
                 }
-                if (val && val[`success`] && Array.isArray(val[`success`])) {
+                if (val && val['success'] && Array.isArray(val['success'])) {
                     tbl = mk_table_func()
-                    td = $(`<td></td>`);
+                    td = $('<td></td>');
                     td.append(tbl);
                     tr.append(td);
-                    list2table(val[`success`], tbl.find(`thead`), tbl.find(`tbody`));
-                } else if (val && val[`success`] && typeof val[`success`] == "object") {
+                    list2table(val['success'], tbl.find('thead'), tbl.find('tbody'));
+                } else if (val && val['success'] && typeof val['success'] == "object") {
                     tbl = mk_table_func()
-                    td = $(`<td></td>`);
+                    td = $('<td></td>');
                     td.append(tbl);
                     tr.append(td);
-                    dict2table(val[`success`], tbl.find(`thead`), tbl.find(`tbody`));
+                    dict2table(val['success'], tbl.find('thead'), tbl.find('tbody'));
                 } else if (val && Array.isArray(val) && val.length > 0 && typeof val[0] == "object") {
                     tbl = mk_table_func()
-                    td = $(`<td></td>`);
+                    td = $('<td></td>');
                     td.append(tbl);
                     tr.append(td);
-                    list2table(val, tbl.find(`thead`), tbl.find(`tbody`));
+                    list2table(val, tbl.find('thead'), tbl.find('tbody'));
                 } else {
                     tr.append($(`<td>${val}</td>`));
                 }
             });
         });
     }
     // dict型の結果をテーブルに変換
     dict2table = (data, table_head, table_body, output_image) => {
-        tr = $(`<tr></tr>`);
+        tr = $('<tr></tr>');
         if (output_image) {
-            if (table_head) table_head.append($(`<th scope="col">output_image</th>`));
-            img = $(`<img class="img-thumbnail">`).attr(`src`, `data:image/png;base64,${output_image}`);
-            img.css(`width`, `100px`).css(`height`, `auto`);
+            if (table_head) table_head.append($('<th scope="col">output_image</th>'));
+            img = $('<img class="img-thumbnail">').attr('src', `data:image/png;base64,${output_image}`);
+            img.css('width', '100px').css('height', 'auto');
             anchor = $(`<a href="data:image/jpeg;base64,${output_image}" data-lightbox="output_image"></a>`).append(img);
-            tr.append($(`<td></td>`).append(anchor));
+            tr.append($('<td></td>').append(anchor));
         }
         $.each(data, (key, val) => {
             if (table_head) table_head.append($(`<th scope="col">${key}</th>`));
-            if (key != `warn` && val) {
+            if (key != 'warn' && val) {
                 if (typeof value === 'object' || Array.isArray(val)) {
                     val = JSON.stringify(val);
                 }
-                if ((typeof val === `string` || val instanceof String) && val.length > 150) {
+                if ((typeof val === 'string' || val instanceof String) && val.length > 150) {
                     val = `${val.substring(0, 150)}...`;
                 }
             }
             tr.append($(`<td>${val}</td>`));
         });
         table_body.append(tr);
     }
     // 結果をテーブルに変換
-    if (result[`success`] && Array.isArray(result[`success`])) {
-        list2table(result[`success`], table_head, table_body);
-    } else if (result[`success`] && typeof result[`success`] == "object") {
-        dict2table(result[`success`], table_head, table_body, result[`output_image`]);
+    if (result['success'] && Array.isArray(result['success'])) {
+        list2table(result['success'], table_head, table_body);
+    } else if (result['success'] && typeof result['success'] == "object") {
+        dict2table(result['success'], table_head, table_body, result['output_image']);
     } else if (Array.isArray(result)) {
         list2table(result, table_head, table_body);
     } else if (typeof result === "string" || result instanceof String) {
-        $(`#result_modal`).find(`.modal-body`).html(result);
+        $('#result_modal').find('.modal-body').html(result);
     } else {
         dict2table(result, table_head, table_body);
     }
-    result_modal.modal(`show`);
+    result_modal.modal('show');
 }
```

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery/jquery.min.3.2.0.js` & `iinfer-0.7.0/iinfer/web/assets/jquery/jquery.min.3.2.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js` & `iinfer-0.7.0/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-ui/AUTHORS.txt` & `iinfer-0.7.0/iinfer/web/assets/jquery-ui/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-ui/LICENSE.txt` & `iinfer-0.7.0/iinfer/web/assets/jquery-ui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png` & `iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png` & `iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png` & `iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png` & `iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png` & `iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png` & `iinfer-0.7.0/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.min.css` & `iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.min.js` & `iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css` & `iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css` & `iinfer-0.7.0/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/jquery-ui/package.json` & `iinfer-0.7.0/iinfer/web/assets/jquery-ui/package.json`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/lightbox2/css/lightbox.min.css` & `iinfer-0.7.0/iinfer/web/assets/lightbox2/css/lightbox.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/lightbox2/images/loading.gif` & `iinfer-0.7.0/iinfer/web/assets/lightbox2/images/loading.gif`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/lightbox2/images/next.png` & `iinfer-0.7.0/iinfer/web/assets/lightbox2/images/next.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/lightbox2/images/prev.png` & `iinfer-0.7.0/iinfer/web/assets/lightbox2/images/prev.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/lightbox2/js/lightbox.min.js` & `iinfer-0.7.0/iinfer/web/assets/lightbox2/js/lightbox.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/tree-menu/css/tree-menu.css` & `iinfer-0.7.0/iinfer/web/assets/tree-menu/css/tree-menu.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/assets/tree-menu/js/tree-menu.js` & `iinfer-0.7.0/iinfer/web/assets/tree-menu/js/tree-menu.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.9/iinfer/web/main.html` & `iinfer-0.7.0/iinfer/web/gui.html`

 * *Files 1% similar despite different names*

```diff
@@ -424,14 +424,17 @@
     </div>
     <!-- ローディングマスク -->
     <div id="loading" class="position-absolute top-0 start-0 w-100 h-100 d-none" style="background:rgba(0, 0, 0, 0.3);z-index:10000;">
         <div class="text-center position-absolute top-50 start-50 w-100 translate-middle">
             <div class="spinner-border text-light" role="status">
                 <span class="sr-only"></span>
             </div>
+            <div>
+                <button type="button" class="btn btn-outline-danger mt-3 bbforce">Back by force</button>
+            </div>
         </div>
     </div>
     <!-- フッター -->
     <footer class="bg-dark fixed-bottom text-center text-white p-2 copyright"></footer>
 </body>
 <link rel="stylesheet" href="assets/bootstrap/bootstrap.min.5.3.0.css">
 <link rel="stylesheet" href="assets/lightbox2/css/lightbox.min.css">
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_tznvgklr_/tmpqnex39jp_TarContainer/0/182.html", line 84, column 73: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_tznvgklr_/tmpqnex39jp_TarContainer/0/182.html", line 112, column 73: Levels of opening and closing headings don't match*

```diff
@@ -35,7 +35,8 @@
 Clear Close
 **** VVeerrssiioonnss ****
     * iinfer
     * Used software
 versions_iinfer
 versions_used
 Close
+Back by force
```

### Comparing `iinfer-0.6.9/iinfer.egg-info/PKG-INFO` & `iinfer-0.7.0/iinfer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.6.9
+Version: 0.7.0
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.6.9/iinfer.egg-info/SOURCES.txt` & `iinfer-0.7.0/iinfer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 iinfer/config.yml
 iinfer/logconf_client.yml
 iinfer/logconf_gui.yml
 iinfer/logconf_install.yml
 iinfer/logconf_postprocess.yml
 iinfer/logconf_redis.yml
 iinfer/logconf_server.yml
+iinfer/logconf_web.yml
 iinfer/version.py
 iinfer.egg-info/PKG-INFO
 iinfer.egg-info/SOURCES.txt
 iinfer.egg-info/dependency_links.txt
 iinfer.egg-info/entry_points.txt
 iinfer.egg-info/requires.txt
 iinfer.egg-info/top_level.txt
@@ -24,14 +25,15 @@
 iinfer/app/gui.py
 iinfer/app/injection.py
 iinfer/app/install.py
 iinfer/app/postprocess.py
 iinfer/app/predict.py
 iinfer/app/redis.py
 iinfer/app/server.py
+iinfer/app/web.py
 iinfer/app/commons/convert.py
 iinfer/app/commons/module.py
 iinfer/app/injections/after_cls_jadge_injection.py
 iinfer/app/injections/after_csv_injection.py
 iinfer/app/injections/after_det_filter_injection.py
 iinfer/app/injections/after_det_jadge_injection.py
 iinfer/app/injections/after_http_injection.py
@@ -57,16 +59,14 @@
 iinfer/app/predicts/mmseg_seg_PSPNet.py
 iinfer/app/predicts/mmseg_seg_SwinUpernet.py
 iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
 iinfer/app/predicts/onnx_det_TinyYoloV3.py
 iinfer/app/predicts/onnx_det_YoloV3.py
 iinfer/app/predicts/onnx_det_YoloX.py
 iinfer/app/predicts/onnx_det_YoloX_Lite.py
-iinfer/datasets/label_coco.txt
-iinfer/datasets/label_voc.txt
 iinfer/docker/Dockerfile
 iinfer/docker/__init__.py
 iinfer/docker/build.sh
 iinfer/docker/docker-compose.yml
 iinfer/extensions/injection/after_cls_jadge_injection.json
 iinfer/extensions/injection/after_csv_injection.json
 iinfer/extensions/injection/after_det_filter_injection.json
@@ -114,15 +114,15 @@
 iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
 iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
 iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
 iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
 iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
 iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
 iinfer/licenses/files.txt
-iinfer/web/main.html
+iinfer/web/gui.html
 iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
 iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
 iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
 iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
 iinfer/web/assets/iinfer/filer_modal.js
 iinfer/web/assets/iinfer/list_cmd.js
 iinfer/web/assets/iinfer/list_pipe.js
```

### Comparing `iinfer-0.6.9/setup.py` & `iinfer-0.7.0/setup.py`

 * *Files identical despite different names*

