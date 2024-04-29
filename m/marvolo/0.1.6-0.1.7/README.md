# Comparing `tmp/marvolo-0.1.6.tar.gz` & `tmp/marvolo-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marvolo-0.1.6.tar", last modified: Mon Feb 26 06:17:05 2024, max compression
+gzip compressed data, was "marvolo-0.1.7.tar", last modified: Mon Apr 29 07:00:52 2024, max compression
```

## Comparing `marvolo-0.1.6.tar` & `marvolo-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 06:17:05.338223 marvolo-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-26 06:17:05.334223 marvolo-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-26 06:17:04.000000 marvolo-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 06:17:05.334223 marvolo-0.1.6/marvolo/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-26 06:17:04.000000 marvolo-0.1.6/marvolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-02-26 06:17:04.000000 marvolo-0.1.6/marvolo/cv.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-26 06:17:04.000000 marvolo-0.1.6/marvolo/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-02-26 06:17:04.000000 marvolo-0.1.6/marvolo/my_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-26 06:17:04.000000 marvolo-0.1.6/marvolo/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 06:17:05.334223 marvolo-0.1.6/marvolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-26 06:17:05.000000 marvolo-0.1.6/marvolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-26 06:17:05.000000 marvolo-0.1.6/marvolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 06:17:05.000000 marvolo-0.1.6/marvolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-26 06:17:05.000000 marvolo-0.1.6/marvolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-26 06:17:05.000000 marvolo-0.1.6/marvolo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 06:17:05.338223 marvolo-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-26 06:17:04.000000 marvolo-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:00:52.523375 marvolo-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-29 07:00:52.523375 marvolo-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 07:00:52.000000 marvolo-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:00:52.523375 marvolo-0.1.7/marvolo/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-29 07:00:52.000000 marvolo-0.1.7/marvolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-29 07:00:52.000000 marvolo-0.1.7/marvolo/cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-29 07:00:52.000000 marvolo-0.1.7/marvolo/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-29 07:00:52.000000 marvolo-0.1.7/marvolo/my_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-29 07:00:52.000000 marvolo-0.1.7/marvolo/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:00:52.523375 marvolo-0.1.7/marvolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-29 07:00:52.000000 marvolo-0.1.7/marvolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-29 07:00:52.000000 marvolo-0.1.7/marvolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:00:52.000000 marvolo-0.1.7/marvolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 07:00:52.000000 marvolo-0.1.7/marvolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 07:00:52.000000 marvolo-0.1.7/marvolo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:00:52.523375 marvolo-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-29 07:00:52.000000 marvolo-0.1.7/setup.py
```

### Comparing `marvolo-0.1.6/marvolo/cv.py` & `marvolo-0.1.7/marvolo/cv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,63 @@
 import os
 import re
+
 import imageio
 import numpy as np
 
+
 def _natural_sort_key(s):
     """
     Key function for natural sorting.
     """
-    return [int(text) if text.isdigit() else text.lower() for text in re.split('([0-9]+)', s)]
+    return [int(text) if text.isdigit() else text.lower() for text in re.split("([0-9]+)", s)]
+
 
-def video_to_image(video_path, image_folder, type = 'png', stride = 1, clear = True):
+def video_to_image(video_path, image_folder, type="png", stride=1, clear=True):
     video = imageio.get_reader(video_path)
 
-    os.makedirs(image_folder, exist_ok = True)
+    os.makedirs(image_folder, exist_ok=True)
 
     if clear:
-        os.system(f'rm -rf {image_folder}')
-        os.makedirs(image_folder, exist_ok = True)
+        os.system(f"rm -rf {image_folder}")
+        os.makedirs(image_folder, exist_ok=True)
 
     for frame_number, frame_data in enumerate(video):
         if frame_number % stride != 0:
             continue
-        imageio.imwrite(os.path.join(image_folder, f'{frame_number}.{type}'), frame_data)
-    
-    print(f'Total {frame_number + 1} frames, saved {(frame_number + 1) // stride} frames')
+        imageio.imwrite(os.path.join(image_folder, f"{frame_number}.{type}"), frame_data)
+
+    print(f"Total {frame_number + 1} frames, saved {(frame_number + 1) // stride} frames")
+
 
-def video_to_array(video_path, stride = 1):
-    '''
+def video_to_array(video_path, stride=1):
+    """
     Return a numpy array, shape as B * H * W * C
-    '''
+    """
     video = imageio.get_reader(video_path)
-    
+
     images = []
     for frame_number, frame_data in enumerate(video):
         if frame_number % stride != 0:
             continue
         images.append(frame_data)
-    
+
     # TODO support for tensor
     return np.array(images)
 
-def image_to_video(video_name, image_path = None, images = None, fps = 30, stride = 1):
+
+def image_to_video(video_name, image_path=None, images=None, fps=30, stride=1):
     if images is None:
         files = os.listdir(image_path)
-        files = sorted([f for f in files if f.endswith(('.png', '.jpg', '.jpeg'))], key=_natural_sort_key)
+        files = sorted([f for f in files if f.endswith((".png", ".jpg", ".jpeg"))], key=_natural_sort_key)
         images = []
         for image_file in files:
             image_path = os.path.join(image_path, image_file)
             images.append(imageio.imread(image_path))
 
         images = images[::stride]
 
-    out = imageio.get_writer(video_name, fps = fps)
+    out = imageio.get_writer(video_name, fps=fps)
 
     for img in images:
         out.append_data(img)
     out.close()
```

### Comparing `marvolo-0.1.6/marvolo/ffmpeg.py` & `marvolo-0.1.7/marvolo/ffmpeg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import os
 
+
 def resize(video, output, height, width):
     height = int(height)
     width = int(width)
-    command = f"ffmpeg -i {video} -vf \"scale={height}:{width}\" {output} -y"
+    command = f'ffmpeg -i {video} -vf "scale={height}:{width}" {output} -y'
     os.system(command)
 
-def cat_same_size(video1, video2, output, overlay = 0):
+
+def cat_same_size(video1, video2, output, overlay=0):
     overlay = int(overlay)
-    command = f"ffmpeg -i {video1} -i {video2} -filter_complex \"[0:v]pad=iw*2:ih*1[a];[a][1:v]overlay=w+{overlay}\" {output} -y"
+    command = f'ffmpeg -i {video1} -i {video2} -filter_complex "[0:v]pad=iw*2:ih*1[a];[a][1:v]overlay=w+{overlay}" {output} -y'
     os.system(command)
 
+
 def change_fps(video, output, new_fps):
     new_fps = int(new_fps)
     command = f"ffmpeg -i {video} -r {new_fps} {output} -y"
     os.system(command)
 
+
 def split_video(video, output, length):
     command = f"ffmpeg -i {video} -ss 00:00:00 -to {length} {output} -y"
     os.system(command)
 
-if __name__ == '__main__':
-    split_video('./a.mp4', './b.mp4', 2)
+
+if __name__ == "__main__":
+    split_video("./a.mp4", "./b.mp4", 2)
```

### Comparing `marvolo-0.1.6/setup.py` & `marvolo-0.1.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Copyright (C) 2023 Haitao Zhou. All rights reserved.
 from setuptools import setup
 
 setup(
-    name='marvolo',
-    version='v0.1.6',
-    description='Some useful tools about CV develeped by Marvolo',
-    platforms=['all'],
-    author='Marvolo',
-    author_email='18377221@buaa.edu.cn',
-    python_requires='>=3.6',
-    url='',
-    install_requires=['opencv-python','imageio', 'colorlog', 'numpy'],
-    license='MIT',
-        classifiers=[
+    name="marvolo",
+    version="v0.1.7",
+    description="Some useful tools about CV develeped by Marvolo",
+    platforms=["all"],
+    author="Marvolo",
+    author_email="18377221@buaa.edu.cn",
+    python_requires=">=3.6",
+    url="",
+    install_requires=["opencv-python", "imageio", "colorlog", "numpy", "imageio[ffmpeg]"],
+    license="MIT",
+    classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

