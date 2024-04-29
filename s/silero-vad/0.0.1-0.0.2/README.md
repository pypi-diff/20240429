# Comparing `tmp/silero-vad-0.0.1.tar.gz` & `tmp/silero-vad-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silero-vad-0.0.1.tar", last modified: Mon Apr 29 03:08:17 2024, max compression
+gzip compressed data, was "silero-vad-0.0.2.tar", last modified: Mon Apr 29 03:14:57 2024, max compression
```

## Comparing `silero-vad-0.0.1.tar` & `silero-vad-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:08:17.484533 silero-vad-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-29 03:08:16.000000 silero-vad-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-29 03:08:17.484533 silero-vad-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-29 03:08:16.000000 silero-vad-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 03:08:17.484533 silero-vad-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-29 03:08:16.000000 silero-vad-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:08:17.484533 silero-vad-0.0.1/silero_vad/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-29 03:08:16.000000 silero-vad-0.0.1/silero_vad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-29 03:08:16.000000 silero-vad-0.0.1/silero_vad/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-29 03:08:16.000000 silero-vad-0.0.1/silero_vad/frame_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-29 03:08:16.000000 silero-vad-0.0.1/silero_vad/inference_session.py
--rw-r--r--   0 runner    (1001) docker     (127)  1807522 2024-04-29 03:08:16.000000 silero-vad-0.0.1/silero_vad/silero_vad.onnx
--rw-r--r--   0 runner    (1001) docker     (127)    14289 2024-04-29 03:08:16.000000 silero-vad-0.0.1/silero_vad/silero_vad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-29 03:08:16.000000 silero-vad-0.0.1/silero_vad/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:08:17.484533 silero-vad-0.0.1/silero_vad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-29 03:08:17.000000 silero-vad-0.0.1/silero_vad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-29 03:08:17.000000 silero-vad-0.0.1/silero_vad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:08:17.000000 silero-vad-0.0.1/silero_vad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-29 03:08:17.000000 silero-vad-0.0.1/silero_vad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 03:08:17.000000 silero-vad-0.0.1/silero_vad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 03:08:17.000000 silero-vad-0.0.1/silero_vad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:14:57.033753 silero-vad-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-29 03:14:55.000000 silero-vad-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-29 03:14:55.000000 silero-vad-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-29 03:14:57.033753 silero-vad-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-29 03:14:55.000000 silero-vad-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 03:14:55.000000 silero-vad-0.0.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 03:14:55.000000 silero-vad-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 03:14:57.033753 silero-vad-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-29 03:14:55.000000 silero-vad-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:14:57.033753 silero-vad-0.0.2/silero_vad/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-29 03:14:55.000000 silero-vad-0.0.2/silero_vad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-29 03:14:55.000000 silero-vad-0.0.2/silero_vad/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-29 03:14:55.000000 silero-vad-0.0.2/silero_vad/frame_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-29 03:14:55.000000 silero-vad-0.0.2/silero_vad/inference_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1807522 2024-04-29 03:14:55.000000 silero-vad-0.0.2/silero_vad/silero_vad.onnx
+-rw-r--r--   0 runner    (1001) docker     (127)    14289 2024-04-29 03:14:55.000000 silero-vad-0.0.2/silero_vad/silero_vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-29 03:14:55.000000 silero-vad-0.0.2/silero_vad/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:14:57.033753 silero-vad-0.0.2/silero_vad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-29 03:14:57.000000 silero-vad-0.0.2/silero_vad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-29 03:14:57.000000 silero-vad-0.0.2/silero_vad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:14:57.000000 silero-vad-0.0.2/silero_vad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-29 03:14:57.000000 silero-vad-0.0.2/silero_vad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 03:14:57.000000 silero-vad-0.0.2/silero_vad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 03:14:57.000000 silero-vad-0.0.2/silero_vad.egg-info/top_level.txt
```

### Comparing `silero-vad-0.0.1/LICENSE` & `silero-vad-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.1/PKG-INFO` & `silero-vad-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-vad
-Version: 0.0.1
+Version: 0.0.2
 Summary: Silero VAD
 Home-page: https://github.com/pengzhendong/silero-vad
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -20,16 +20,12 @@
 ### Denoiser
 
 See [RnNoise](https://github.com/werman/noise-suppression-for-voice).
 
 ### Python Usage
 
 ```bash
-$ pip install https://github.com/pengzhendong/silero-vad/archive/refs/heads/master.zip
-$ silero_vad --wav_path audio.wav
-$ python
->>> from silero_vad import SileroVAD
->>> vad = SileroVAD()
->>> vad.get_speech_timestamps("audio.wav")
+$ pip install silero-vad
+$ silero_vad audio.wav
 ```
```

### Comparing `silero-vad-0.0.1/setup.py` & `silero-vad-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.1/silero_vad/__init__.py` & `silero-vad-0.0.2/silero_vad/__init__.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.1/silero_vad/cli.py` & `silero-vad-0.0.2/silero_vad/cli.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.1/silero_vad/frame_queue.py` & `silero-vad-0.0.2/silero_vad/frame_queue.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.1/silero_vad/inference_session.py` & `silero-vad-0.0.2/silero_vad/inference_session.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.1/silero_vad/silero_vad.onnx` & `silero-vad-0.0.2/silero_vad/silero_vad.onnx`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.1/silero_vad/silero_vad.py` & `silero-vad-0.0.2/silero_vad/silero_vad.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.1/silero_vad/utils.py` & `silero-vad-0.0.2/silero_vad/utils.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.1/silero_vad.egg-info/PKG-INFO` & `silero-vad-0.0.2/silero_vad.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-vad
-Version: 0.0.1
+Version: 0.0.2
 Summary: Silero VAD
 Home-page: https://github.com/pengzhendong/silero-vad
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -20,16 +20,12 @@
 ### Denoiser
 
 See [RnNoise](https://github.com/werman/noise-suppression-for-voice).
 
 ### Python Usage
 
 ```bash
-$ pip install https://github.com/pengzhendong/silero-vad/archive/refs/heads/master.zip
-$ silero_vad --wav_path audio.wav
-$ python
->>> from silero_vad import SileroVAD
->>> vad = SileroVAD()
->>> vad.get_speech_timestamps("audio.wav")
+$ pip install silero-vad
+$ silero_vad audio.wav
 ```
```

