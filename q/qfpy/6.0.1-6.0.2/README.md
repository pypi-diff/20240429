# Comparing `tmp/qfpy-6.0.1.tar.gz` & `tmp/qfpy-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfpy-6.0.1.tar", last modified: Sun Apr 21 04:51:04 2024, max compression
+gzip compressed data, was "qfpy-6.0.2.tar", last modified: Mon Apr 29 16:56:09 2024, max compression
```

## Comparing `qfpy-6.0.1.tar` & `qfpy-6.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 04:51:04.182348 qfpy-6.0.1/
--rw-rw-rw-   0        0        0      159 2024-04-21 04:51:04.180400 qfpy-6.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-21 04:50:53.000000 qfpy-6.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-21 04:51:04.182348 qfpy-6.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-21 04:51:04.154474 qfpy-6.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-21 04:51:04.169136 qfpy-6.0.1/src/qfpy/
--rw-rw-rw-   0        0        0       29 2024-03-06 16:44:46.000000 qfpy-6.0.1/src/qfpy/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-21 04:50:44.000000 qfpy-6.0.1/src/qfpy/character.py
--rw-rw-rw-   0        0        0     1393 2024-03-27 09:56:39.000000 qfpy-6.0.1/src/qfpy/exif.py
--rw-rw-rw-   0        0        0     3124 2024-04-21 04:46:11.000000 qfpy-6.0.1/src/qfpy/ffmpeg.py
--rw-rw-rw-   0        0        0      611 2024-04-21 04:47:36.000000 qfpy-6.0.1/src/qfpy/folder.py
--rw-rw-rw-   0        0        0      845 2024-03-23 10:23:45.000000 qfpy-6.0.1/src/qfpy/function.py
--rw-rw-rw-   0        0        0      804 2024-03-23 10:20:43.000000 qfpy-6.0.1/src/qfpy/process.py
-drwxrwxrwx   0        0        0        0 2024-04-21 04:51:04.178439 qfpy-6.0.1/src/qfpy.egg-info/
--rw-rw-rw-   0        0        0      159 2024-04-21 04:51:04.000000 qfpy-6.0.1/src/qfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-04-21 04:51:04.000000 qfpy-6.0.1/src/qfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 04:51:04.000000 qfpy-6.0.1/src/qfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-21 04:51:04.000000 qfpy-6.0.1/src/qfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 16:56:09.856638 qfpy-6.0.2/
+-rw-rw-rw-   0        0        0      159 2024-04-29 16:56:09.853712 qfpy-6.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-29 16:55:56.000000 qfpy-6.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 16:56:09.856638 qfpy-6.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 16:56:09.827781 qfpy-6.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 16:56:09.843403 qfpy-6.0.2/src/qfpy/
+-rw-rw-rw-   0        0        0       70 2024-04-29 16:54:46.000000 qfpy-6.0.2/src/qfpy/__init__.py
+-rw-rw-rw-   0        0        0      210 2024-04-29 16:48:36.000000 qfpy-6.0.2/src/qfpy/character.py
+-rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-6.0.2/src/qfpy/exif.py
+-rw-rw-rw-   0        0        0     3067 2024-04-29 16:52:59.000000 qfpy-6.0.2/src/qfpy/ffmpeg.py
+-rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-6.0.2/src/qfpy/folder.py
+-rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-6.0.2/src/qfpy/function.py
+-rw-rw-rw-   0        0        0      854 2024-04-29 16:55:44.000000 qfpy-6.0.2/src/qfpy/process.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:56:09.852735 qfpy-6.0.2/src/qfpy.egg-info/
+-rw-rw-rw-   0        0        0      159 2024-04-29 16:56:09.000000 qfpy-6.0.2/src/qfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-04-29 16:56:09.000000 qfpy-6.0.2/src/qfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 16:56:09.000000 qfpy-6.0.2/src/qfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-29 16:56:09.000000 qfpy-6.0.2/src/qfpy.egg-info/top_level.txt
```

### Comparing `qfpy-6.0.1/src/qfpy/exif.py` & `qfpy-6.0.2/src/qfpy/exif.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""
+def get_exif(file_path: str | Path) -> dict
+
+def ch_tag(file_path: str | Path, tag: str, value: str)
+"""
+
 import json
 import subprocess as sp
 from pathlib import Path
 
 COMMENT = "Comment"
 
 
@@ -41,8 +47,9 @@
     cmd = ["exiftool", f"-{tag}={value}", file_path, "-overwrite_original"]
     # 执行命令，并捕获输出
     sp.run(cmd, capture_output=True)
 
 
 
 if __name__ == "__main__":
+    "das".lower()
     pass
```

### Comparing `qfpy-6.0.1/src/qfpy/ffmpeg.py` & `qfpy-6.0.2/src/qfpy/ffmpeg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
-函数
+def concat_video(files: list[str], output_file: str)
 
-concat_video：合并视频
-is_hevc：是否为HEVC编码
-is_not_hevc：是否为非HEVC编码
-———————————
+def is_hevc(file: Path) -> bool
 
-类 FFprobe
+def is_not_hevc(file: Path) -> bool
 
-    duration：获取视频时长
+class FFprobe
+    def duration
 
-    codec：获取视频编码
-
-    size：获取视频大小
+    def codec_name
+    
+    def size
 """
 
 import json
 import subprocess as sp
 from pathlib import Path
 
 from moviepy.editor import VideoFileClip, concatenate_videoclips
```

### Comparing `qfpy-6.0.1/src/qfpy/folder.py` & `qfpy-6.0.2/src/qfpy/folder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+"""
+def count_suffix(folder: str) -> Counter
+"""
+
 from collections import Counter
 from pathlib import Path
 
 
 def count_suffix(folder: str) -> Counter:
     """
     统计文件夹中所有文件后缀
     :param file_path: 文件路径
     :return: 字典
     """
     suffix_counter = Counter()
     try:
         for file in Path(folder).rglob("*"):
-            if file.is_dir(): continue
-            if file.is_symlink(): continue # 忽略符号链接
+            if file.is_dir():
+                continue
+            if file.is_symlink():
+                continue  # 忽略符号链接
             suffix_counter[file.suffix.lower()] += 1
     except FileNotFoundError:
         pass
     return suffix_counter
 
 
 if __name__ == "__main__":
```

### Comparing `qfpy-6.0.1/src/qfpy/function.py` & `qfpy-6.0.2/src/qfpy/function.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-map_funcs：map 多个函数
+map_funcs(funcs: list[Callable], iterable: Iterable) -> Iterable
 """
 from typing import Callable, Iterable
 
 
 def map_funcs(funcs: list[Callable], iterable: Iterable) -> Iterable:
     """
     对给定的可迭代对象应用多个函数。
```

### Comparing `qfpy-6.0.1/src/qfpy/process.py` & `qfpy-6.0.2/src/qfpy/process.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+def exist(process_name: str) -> bool
+"""
+
 import psutil
 
 
 def exist(process_name: str) -> bool:
     """
     检查指定的进程是否在运行
```

