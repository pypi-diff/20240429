# Comparing `tmp/pyjvcprojector-1.0.8.tar.gz` & `tmp/pyjvcprojector-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjvcprojector-1.0.8.tar", last modified: Wed Jan 17 14:22:23 2024, max compression
+gzip compressed data, was "pyjvcprojector-1.0.9.tar", last modified: Wed Jan 17 15:55:46 2024, max compression
```

## Comparing `pyjvcprojector-1.0.8.tar` & `pyjvcprojector-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-01-17 14:22:23.758680 pyjvcprojector-1.0.8/
--rw-r--r--   0 steve      (501) staff       (20)     1069 2022-12-20 20:10:52.000000 pyjvcprojector-1.0.8/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)     2701 2024-01-17 14:22:23.758806 pyjvcprojector-1.0.8/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     2101 2022-12-30 15:06:44.000000 pyjvcprojector-1.0.8/README.md
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-01-17 14:22:23.756916 pyjvcprojector-1.0.8/jvcprojector/
--rw-r--r--   0 steve      (501) staff       (20)      275 2024-01-17 14:09:11.000000 pyjvcprojector-1.0.8/jvcprojector/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)    11297 2023-01-01 19:31:59.000000 pyjvcprojector-1.0.8/jvcprojector/command.py
--rw-r--r--   0 steve      (501) staff       (20)     2818 2023-01-01 19:32:35.000000 pyjvcprojector-1.0.8/jvcprojector/connection.py
--rw-r--r--   0 steve      (501) staff       (20)     1024 2024-01-17 14:09:11.000000 pyjvcprojector-1.0.8/jvcprojector/const.py
--rw-r--r--   0 steve      (501) staff       (20)     6628 2023-01-01 19:34:32.000000 pyjvcprojector-1.0.8/jvcprojector/device.py
--rw-r--r--   0 steve      (501) staff       (20)      377 2022-12-27 23:57:50.000000 pyjvcprojector-1.0.8/jvcprojector/error.py
--rw-r--r--   0 steve      (501) staff       (20)     5206 2023-01-01 21:15:47.000000 pyjvcprojector-1.0.8/jvcprojector/projector.py
--rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-27 23:51:41.000000 pyjvcprojector-1.0.8/jvcprojector/py.typed
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-01-17 14:22:23.758360 pyjvcprojector-1.0.8/pyjvcprojector.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)     2701 2024-01-17 14:22:23.000000 pyjvcprojector-1.0.8/pyjvcprojector.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      431 2024-01-17 14:22:23.000000 pyjvcprojector-1.0.8/pyjvcprojector.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2024-01-17 14:22:23.000000 pyjvcprojector-1.0.8/pyjvcprojector.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       17 2024-01-17 14:22:23.000000 pyjvcprojector-1.0.8/pyjvcprojector.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       13 2024-01-17 14:22:23.000000 pyjvcprojector-1.0.8/pyjvcprojector.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)     1380 2022-12-29 00:50:02.000000 pyjvcprojector-1.0.8/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)      851 2024-01-17 14:22:23.759743 pyjvcprojector-1.0.8/setup.cfg
--rw-r--r--   0 steve      (501) staff       (20)       37 2022-12-20 20:10:24.000000 pyjvcprojector-1.0.8/setup.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-01-17 15:55:46.974743 pyjvcprojector-1.0.9/
+-rw-r--r--   0 steve      (501) staff       (20)     1069 2022-12-20 20:10:52.000000 pyjvcprojector-1.0.9/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)     2701 2024-01-17 15:55:46.975327 pyjvcprojector-1.0.9/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     2101 2022-12-30 15:06:44.000000 pyjvcprojector-1.0.9/README.md
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-01-17 15:55:46.967642 pyjvcprojector-1.0.9/jvcprojector/
+-rw-r--r--   0 steve      (501) staff       (20)      275 2024-01-17 15:53:32.000000 pyjvcprojector-1.0.9/jvcprojector/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)    11297 2023-01-01 19:31:59.000000 pyjvcprojector-1.0.9/jvcprojector/command.py
+-rw-r--r--   0 steve      (501) staff       (20)     2818 2023-01-01 19:32:35.000000 pyjvcprojector-1.0.9/jvcprojector/connection.py
+-rw-r--r--   0 steve      (501) staff       (20)     1322 2024-01-17 15:55:04.000000 pyjvcprojector-1.0.9/jvcprojector/const.py
+-rw-r--r--   0 steve      (501) staff       (20)     6628 2023-01-01 19:34:32.000000 pyjvcprojector-1.0.9/jvcprojector/device.py
+-rw-r--r--   0 steve      (501) staff       (20)      377 2022-12-27 23:57:50.000000 pyjvcprojector-1.0.9/jvcprojector/error.py
+-rw-r--r--   0 steve      (501) staff       (20)     5206 2023-01-01 21:15:47.000000 pyjvcprojector-1.0.9/jvcprojector/projector.py
+-rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-27 23:51:41.000000 pyjvcprojector-1.0.9/jvcprojector/py.typed
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-01-17 15:55:46.974381 pyjvcprojector-1.0.9/pyjvcprojector.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)     2701 2024-01-17 15:55:46.000000 pyjvcprojector-1.0.9/pyjvcprojector.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      431 2024-01-17 15:55:46.000000 pyjvcprojector-1.0.9/pyjvcprojector.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2024-01-17 15:55:46.000000 pyjvcprojector-1.0.9/pyjvcprojector.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       17 2024-01-17 15:55:46.000000 pyjvcprojector-1.0.9/pyjvcprojector.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       13 2024-01-17 15:55:46.000000 pyjvcprojector-1.0.9/pyjvcprojector.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)     1380 2022-12-29 00:50:02.000000 pyjvcprojector-1.0.9/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)      851 2024-01-17 15:55:46.976437 pyjvcprojector-1.0.9/setup.cfg
+-rw-r--r--   0 steve      (501) staff       (20)       37 2022-12-20 20:10:24.000000 pyjvcprojector-1.0.9/setup.py
```

### Comparing `pyjvcprojector-1.0.8/LICENSE` & `pyjvcprojector-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjvcprojector-1.0.8/PKG-INFO` & `pyjvcprojector-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvcprojector
-Version: 1.0.8
+Version: 1.0.9
 Summary: "A python library for controlling a JVC Projector over a network connection."
 Home-page: https://github.com/SteveEasley/pyjvcprojector
 Author: Steve Easley
 Author-email: tardis74@yahoo.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyjvcprojector-1.0.8/README.md` & `pyjvcprojector-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyjvcprojector-1.0.8/jvcprojector/command.py` & `pyjvcprojector-1.0.9/jvcprojector/command.py`

 * *Files identical despite different names*

### Comparing `pyjvcprojector-1.0.8/jvcprojector/connection.py` & `pyjvcprojector-1.0.9/jvcprojector/connection.py`

 * *Files identical despite different names*

### Comparing `pyjvcprojector-1.0.8/jvcprojector/const.py` & `pyjvcprojector-1.0.9/jvcprojector/const.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,10 +32,20 @@
 REMOTE_ADVANCED_MENU: Final = "7373"
 REMOTE_PICTURE_MODE: Final = "73F4"
 REMOTE_COLOR_PROFILE: Final = "7388"
 REMOTE_LENS_CONTROL: Final = "7330"
 REMOTE_SETTING_MEMORY: Final = "73D4"
 REMOTE_GAMMA_SETTINGS: Final = "73F5"
 REMOTE_CMD: Final = "738A"
-REMOTE_MEM_MODE1: Final = "738A"
-REMOTE_MEM_MODE2: Final = "738A"
-REMOTE_MEM_MODE3: Final = "738A"
+REMOTE_MODE_1: Final = "73D8"
+REMOTE_MODE_2: Final = "73D9"
+REMOTE_MODE_3: Final = "73DA"
+REMOTE_HDMI_1: Final = "7370"
+REMOTE_HDMI_2: Final = "7371"
+REMOTE_LENS_AP: Final = "7320"
+REMOTE_ANAMO: Final = "73C5"
+REMOTE_GAMMA: Final = "7375"
+REMOTE_COLOR_TEMP: Final = "7376"
+REMOTE_3D_FORMAT: Final = "73D6"
+REMOTE_PIC_ADJ: Final = "7372"
+REMOTE_NATURAL: Final = "736A"
+REMOTE_CINEMA: Final = "7368"
```

### Comparing `pyjvcprojector-1.0.8/jvcprojector/device.py` & `pyjvcprojector-1.0.9/jvcprojector/device.py`

 * *Files identical despite different names*

### Comparing `pyjvcprojector-1.0.8/jvcprojector/projector.py` & `pyjvcprojector-1.0.9/jvcprojector/projector.py`

 * *Files identical despite different names*

### Comparing `pyjvcprojector-1.0.8/pyjvcprojector.egg-info/PKG-INFO` & `pyjvcprojector-1.0.9/pyjvcprojector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvcprojector
-Version: 1.0.8
+Version: 1.0.9
 Summary: "A python library for controlling a JVC Projector over a network connection."
 Home-page: https://github.com/SteveEasley/pyjvcprojector
 Author: Steve Easley
 Author-email: tardis74@yahoo.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyjvcprojector-1.0.8/pyproject.toml` & `pyjvcprojector-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjvcprojector-1.0.8/setup.cfg` & `pyjvcprojector-1.0.9/setup.cfg`

 * *Files identical despite different names*

