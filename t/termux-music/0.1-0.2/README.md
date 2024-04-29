# Comparing `tmp/termux_music-0.1.tar.gz` & `tmp/termux_music-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termux_music-0.1.tar", last modified: Mon Apr 29 14:21:56 2024, max compression
+gzip compressed data, was "termux_music-0.2.tar", last modified: Mon Apr 29 14:32:43 2024, max compression
```

## Comparing `termux_music-0.1.tar` & `termux_music-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-29 14:21:56.642386 termux_music-0.1/
--rw-------   0 u0_a191  (10191) u0_a191  (10191)    11357 2024-04-29 14:13:34.000000 termux_music-0.1/LICENSE
--rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)     2936 2024-04-29 14:21:56.642386 termux_music-0.1/PKG-INFO
--rw-------   0 u0_a191  (10191) u0_a191  (10191)     2501 2024-04-29 14:13:34.000000 termux_music-0.1/README.rst
--rw-------   0 u0_a191  (10191) u0_a191  (10191)       38 2024-04-29 14:21:56.642386 termux_music-0.1/setup.cfg
--rw-------   0 u0_a191  (10191) u0_a191  (10191)      634 2024-04-29 14:17:44.000000 termux_music-0.1/setup.py
--rwx------   0 u0_a191  (10191) u0_a191  (10191)     1501 2024-04-29 14:12:31.000000 termux_music-0.1/termux-music
-drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-29 14:21:56.639053 termux_music-0.1/termux_music.egg-info/
--rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)     2936 2024-04-29 14:21:56.000000 termux_music-0.1/termux_music.egg-info/PKG-INFO
--rw-------   0 u0_a191  (10191) u0_a191  (10191)      219 2024-04-29 14:21:56.000000 termux_music-0.1/termux_music.egg-info/SOURCES.txt
--rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-29 14:21:56.000000 termux_music-0.1/termux_music.egg-info/dependency_links.txt
--rw-------   0 u0_a191  (10191) u0_a191  (10191)        7 2024-04-29 14:21:56.000000 termux_music-0.1/termux_music.egg-info/requires.txt
--rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-29 14:21:56.000000 termux_music-0.1/termux_music.egg-info/top_level.txt
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-29 14:32:42.994145 termux_music-0.2/
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)    11357 2024-04-29 14:13:34.000000 termux_music-0.2/LICENSE
+-rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)     2936 2024-04-29 14:32:42.990812 termux_music-0.2/PKG-INFO
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)     2501 2024-04-29 14:13:34.000000 termux_music-0.2/README.rst
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)       38 2024-04-29 14:32:42.994145 termux_music-0.2/setup.cfg
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)      634 2024-04-29 14:32:14.000000 termux_music-0.2/setup.py
+-rwx------   0 u0_a191  (10191) u0_a191  (10191)     1616 2024-04-29 14:32:05.000000 termux_music-0.2/termux-music
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-29 14:32:42.990812 termux_music-0.2/termux_music.egg-info/
+-rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)     2936 2024-04-29 14:32:42.000000 termux_music-0.2/termux_music.egg-info/PKG-INFO
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)      219 2024-04-29 14:32:42.000000 termux_music-0.2/termux_music.egg-info/SOURCES.txt
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-29 14:32:42.000000 termux_music-0.2/termux_music.egg-info/dependency_links.txt
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)        7 2024-04-29 14:32:42.000000 termux_music-0.2/termux_music.egg-info/requires.txt
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-29 14:32:42.000000 termux_music-0.2/termux_music.egg-info/top_level.txt
```

### Comparing `termux_music-0.1/LICENSE` & `termux_music-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `termux_music-0.1/PKG-INFO` & `termux_music-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-music
-Version: 0.1
+Version: 0.2
 Summary: Script to Run Music in Termux
 Home-page: https://github.com/androlinuxs/termux-music
 Author: Alexander Krefting
 Author-email: linuxdevalex@outlook.de
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `termux_music-0.1/README.rst` & `termux_music-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `termux_music-0.1/setup.py` & `termux_music-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='termux-music',
-    version='0.1',
+    version='0.2',
     license='Apache License 2.0',
     description='Script to Run Music in Termux',
     long_description=readme(),
     author='Alexander Krefting',
     author_email='linuxdevalex@outlook.de',
     url='https://github.com/androlinuxs/termux-music',
     scripts=['termux-music'],
```

### Comparing `termux_music-0.1/termux-music` & `termux_music-0.2/termux-music`

 * *Files 15% similar despite different names*

```diff
@@ -4,35 +4,38 @@
 import sys
 from pytube import YouTube
 
 TERMUX_MUSIC_PATH = "/data/data/com.termux/files/usr/lib/termux-music"
 
 def download_music(url, name):
     if not url or not name:
-        print("Please provide a URL and a name.")
+        print("Bitte gib eine URL und einen Namen an.")
         sys.exit(1)
 
     try:
         os.makedirs(f"{TERMUX_MUSIC_PATH}/{name}", exist_ok=True)
         os.chdir(f"{TERMUX_MUSIC_PATH}/{name}")
         YouTube(url).streams.filter(only_audio=True).first().download(filename=name)
-        os.rename(f"{name}.mp4", f"{name}.mp3")
+        for file in os.listdir():
+            if '.mp4' in file:
+                os.rename(file, file.replace('.mp4', '.mp3'))
+                break
     except Exception as e:
-        print(f"Error: {e}")
+        print(f"Fehler: {e}")
         sys.exit(1)
 
 def start_music(name):
     if not name:
-        print("Please provide a name.")
+        print("Bitte gib einen Namen an.")
         sys.exit(1)
 
     try:
         os.system(f"termux-media-player play {TERMUX_MUSIC_PATH}/{name}/{name}.mp3")
     except Exception as e:
-        print(f"Error: {e}")
+        print(f"Fehler: {e}")
         sys.exit(1)
 
 if __name__ == "__main__":
     CMD = sys.argv[1]
 
     if CMD in ["--download", "-d", "download"]:
         download_music(*sys.argv[2:])
@@ -41,9 +44,9 @@
     elif CMD in ["--stop", "-st", "stop"]:
         os.system("termux-media-player stop")
     elif CMD in ["--play", "-pl", "play"]:
         os.system("termux-media-player play")
     elif CMD in ["--pause", "-pa", "pause"]:
         os.system("termux-media-player pause")
     else:
-        print("Available options: --download, --start, --stop, --play, --pause")
+        print("Verfügbare Optionen: --download, --start, --stop, --play, --pause")
         sys.exit(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `termux_music-0.1/termux_music.egg-info/PKG-INFO` & `termux_music-0.2/termux_music.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-music
-Version: 0.1
+Version: 0.2
 Summary: Script to Run Music in Termux
 Home-page: https://github.com/androlinuxs/termux-music
 Author: Alexander Krefting
 Author-email: linuxdevalex@outlook.de
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

