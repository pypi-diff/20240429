# Comparing `tmp/termux_music-0.3.tar.gz` & `tmp/termux_music-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termux_music-0.3.tar", last modified: Mon Apr 29 14:36:58 2024, max compression
+gzip compressed data, was "termux_music-0.4.tar", last modified: Mon Apr 29 14:40:46 2024, max compression
```

## Comparing `termux_music-0.3.tar` & `termux_music-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-29 14:36:58.208874 termux_music-0.3/
--rw-------   0 u0_a191  (10191) u0_a191  (10191)    11357 2024-04-29 14:13:34.000000 termux_music-0.3/LICENSE
--rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)     2936 2024-04-29 14:36:58.205541 termux_music-0.3/PKG-INFO
--rw-------   0 u0_a191  (10191) u0_a191  (10191)     2501 2024-04-29 14:13:34.000000 termux_music-0.3/README.rst
--rw-------   0 u0_a191  (10191) u0_a191  (10191)       38 2024-04-29 14:36:58.208874 termux_music-0.3/setup.cfg
--rw-------   0 u0_a191  (10191) u0_a191  (10191)      634 2024-04-29 14:36:22.000000 termux_music-0.3/setup.py
--rwx------   0 u0_a191  (10191) u0_a191  (10191)     1667 2024-04-29 14:36:08.000000 termux_music-0.3/termux-music
-drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-29 14:36:58.202208 termux_music-0.3/termux_music.egg-info/
--rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)     2936 2024-04-29 14:36:58.000000 termux_music-0.3/termux_music.egg-info/PKG-INFO
--rw-------   0 u0_a191  (10191) u0_a191  (10191)      219 2024-04-29 14:36:58.000000 termux_music-0.3/termux_music.egg-info/SOURCES.txt
--rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-29 14:36:58.000000 termux_music-0.3/termux_music.egg-info/dependency_links.txt
--rw-------   0 u0_a191  (10191) u0_a191  (10191)        7 2024-04-29 14:36:58.000000 termux_music-0.3/termux_music.egg-info/requires.txt
--rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-29 14:36:58.000000 termux_music-0.3/termux_music.egg-info/top_level.txt
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-29 14:40:46.330476 termux_music-0.4/
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)    11357 2024-04-29 14:13:34.000000 termux_music-0.4/LICENSE
+-rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)     2936 2024-04-29 14:40:46.330476 termux_music-0.4/PKG-INFO
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)     2501 2024-04-29 14:13:34.000000 termux_music-0.4/README.rst
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)       38 2024-04-29 14:40:46.330476 termux_music-0.4/setup.cfg
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)      634 2024-04-29 14:40:29.000000 termux_music-0.4/setup.py
+-rwx------   0 u0_a191  (10191) u0_a191  (10191)     1663 2024-04-29 14:39:56.000000 termux_music-0.4/termux-music
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-29 14:40:46.327142 termux_music-0.4/termux_music.egg-info/
+-rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)     2936 2024-04-29 14:40:46.000000 termux_music-0.4/termux_music.egg-info/PKG-INFO
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)      219 2024-04-29 14:40:46.000000 termux_music-0.4/termux_music.egg-info/SOURCES.txt
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-29 14:40:46.000000 termux_music-0.4/termux_music.egg-info/dependency_links.txt
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)        7 2024-04-29 14:40:46.000000 termux_music-0.4/termux_music.egg-info/requires.txt
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-29 14:40:46.000000 termux_music-0.4/termux_music.egg-info/top_level.txt
```

### Comparing `termux_music-0.3/LICENSE` & `termux_music-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `termux_music-0.3/PKG-INFO` & `termux_music-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-music
-Version: 0.3
+Version: 0.4
 Summary: Script to Run Music in Termux
 Home-page: https://github.com/androlinuxs/termux-music
 Author: Alexander Krefting
 Author-email: linuxdevalex@outlook.de
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `termux_music-0.3/README.rst` & `termux_music-0.4/README.rst`

 * *Files identical despite different names*

### Comparing `termux_music-0.3/setup.py` & `termux_music-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='termux-music',
-    version='0.3',
+    version='0.4',
     license='Apache License 2.0',
     description='Script to Run Music in Termux',
     long_description=readme(),
     author='Alexander Krefting',
     author_email='linuxdevalex@outlook.de',
     url='https://github.com/androlinuxs/termux-music',
     scripts=['termux-music'],
```

### Comparing `termux_music-0.3/termux-music` & `termux_music-0.4/termux-music`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def start_music(name):
     if not name:
         print("Bitte gib einen Namen an.")
         sys.exit(1)
 
     try:
-        os.system(f"termux-media-player play {TERMUX_MUSIC_PATH}/{name}/{name}.mp3")
+        os.system(f"termux-media-player play {TERMUX_MUSIC_PATH}/{name}/{name}")
     except Exception as e:
         print(f"Fehler: {e}")
         sys.exit(1)
 
 if __name__ == "__main__":
     CMD = sys.argv[1]
```

### Comparing `termux_music-0.3/termux_music.egg-info/PKG-INFO` & `termux_music-0.4/termux_music.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-music
-Version: 0.3
+Version: 0.4
 Summary: Script to Run Music in Termux
 Home-page: https://github.com/androlinuxs/termux-music
 Author: Alexander Krefting
 Author-email: linuxdevalex@outlook.de
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

