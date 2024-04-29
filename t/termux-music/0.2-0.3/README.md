# Comparing `tmp/termux_music-0.2.tar.gz` & `tmp/termux_music-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termux_music-0.2.tar", last modified: Mon Apr 29 14:32:43 2024, max compression
+gzip compressed data, was "termux_music-0.3.tar", last modified: Mon Apr 29 14:36:58 2024, max compression
```

## Comparing `termux_music-0.2.tar` & `termux_music-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-29 14:32:42.994145 termux_music-0.2/
--rw-------   0 u0_a191  (10191) u0_a191  (10191)    11357 2024-04-29 14:13:34.000000 termux_music-0.2/LICENSE
--rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)     2936 2024-04-29 14:32:42.990812 termux_music-0.2/PKG-INFO
--rw-------   0 u0_a191  (10191) u0_a191  (10191)     2501 2024-04-29 14:13:34.000000 termux_music-0.2/README.rst
--rw-------   0 u0_a191  (10191) u0_a191  (10191)       38 2024-04-29 14:32:42.994145 termux_music-0.2/setup.cfg
--rw-------   0 u0_a191  (10191) u0_a191  (10191)      634 2024-04-29 14:32:14.000000 termux_music-0.2/setup.py
--rwx------   0 u0_a191  (10191) u0_a191  (10191)     1616 2024-04-29 14:32:05.000000 termux_music-0.2/termux-music
-drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-29 14:32:42.990812 termux_music-0.2/termux_music.egg-info/
--rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)     2936 2024-04-29 14:32:42.000000 termux_music-0.2/termux_music.egg-info/PKG-INFO
--rw-------   0 u0_a191  (10191) u0_a191  (10191)      219 2024-04-29 14:32:42.000000 termux_music-0.2/termux_music.egg-info/SOURCES.txt
--rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-29 14:32:42.000000 termux_music-0.2/termux_music.egg-info/dependency_links.txt
--rw-------   0 u0_a191  (10191) u0_a191  (10191)        7 2024-04-29 14:32:42.000000 termux_music-0.2/termux_music.egg-info/requires.txt
--rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-29 14:32:42.000000 termux_music-0.2/termux_music.egg-info/top_level.txt
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-29 14:36:58.208874 termux_music-0.3/
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)    11357 2024-04-29 14:13:34.000000 termux_music-0.3/LICENSE
+-rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)     2936 2024-04-29 14:36:58.205541 termux_music-0.3/PKG-INFO
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)     2501 2024-04-29 14:13:34.000000 termux_music-0.3/README.rst
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)       38 2024-04-29 14:36:58.208874 termux_music-0.3/setup.cfg
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)      634 2024-04-29 14:36:22.000000 termux_music-0.3/setup.py
+-rwx------   0 u0_a191  (10191) u0_a191  (10191)     1667 2024-04-29 14:36:08.000000 termux_music-0.3/termux-music
+drwx------   0 u0_a191  (10191) u0_a191  (10191)        0 2024-04-29 14:36:58.202208 termux_music-0.3/termux_music.egg-info/
+-rw-r--r--   0 u0_a191  (10191) u0_a191  (10191)     2936 2024-04-29 14:36:58.000000 termux_music-0.3/termux_music.egg-info/PKG-INFO
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)      219 2024-04-29 14:36:58.000000 termux_music-0.3/termux_music.egg-info/SOURCES.txt
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-29 14:36:58.000000 termux_music-0.3/termux_music.egg-info/dependency_links.txt
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)        7 2024-04-29 14:36:58.000000 termux_music-0.3/termux_music.egg-info/requires.txt
+-rw-------   0 u0_a191  (10191) u0_a191  (10191)        1 2024-04-29 14:36:58.000000 termux_music-0.3/termux_music.egg-info/top_level.txt
```

### Comparing `termux_music-0.2/LICENSE` & `termux_music-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `termux_music-0.2/PKG-INFO` & `termux_music-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-music
-Version: 0.2
+Version: 0.3
 Summary: Script to Run Music in Termux
 Home-page: https://github.com/androlinuxs/termux-music
 Author: Alexander Krefting
 Author-email: linuxdevalex@outlook.de
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `termux_music-0.2/README.rst` & `termux_music-0.3/README.rst`

 * *Files identical despite different names*

### Comparing `termux_music-0.2/setup.py` & `termux_music-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='termux-music',
-    version='0.2',
+    version='0.3',
     license='Apache License 2.0',
     description='Script to Run Music in Termux',
     long_description=readme(),
     author='Alexander Krefting',
     author_email='linuxdevalex@outlook.de',
     url='https://github.com/androlinuxs/termux-music',
     scripts=['termux-music'],
```

### Comparing `termux_music-0.2/termux-music` & `termux_music-0.3/termux-music`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     try:
         os.makedirs(f"{TERMUX_MUSIC_PATH}/{name}", exist_ok=True)
         os.chdir(f"{TERMUX_MUSIC_PATH}/{name}")
         YouTube(url).streams.filter(only_audio=True).first().download(filename=name)
         for file in os.listdir():
             if '.mp4' in file:
                 os.rename(file, file.replace('.mp4', '.mp3'))
+                os.system(f"mv {name} {name}.mp3")
                 break
     except Exception as e:
         print(f"Fehler: {e}")
         sys.exit(1)
 
 def start_music(name):
     if not name:
```

### Comparing `termux_music-0.2/termux_music.egg-info/PKG-INFO` & `termux_music-0.3/termux_music.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-music
-Version: 0.2
+Version: 0.3
 Summary: Script to Run Music in Termux
 Home-page: https://github.com/androlinuxs/termux-music
 Author: Alexander Krefting
 Author-email: linuxdevalex@outlook.de
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

