# Comparing `tmp/sapit-1.0.0.tar.gz` & `tmp/sapit-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapit-1.0.0.tar", last modified: Mon Apr 29 18:44:27 2024, max compression
+gzip compressed data, was "sapit-1.2.0.tar", last modified: Mon Apr 29 19:39:41 2024, max compression
```

## Comparing `sapit-1.0.0.tar` & `sapit-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 18:44:27.495913 sapit-1.0.0/
--rw-rw-rw-   0        0        0     1337 2024-04-29 18:44:27.491915 sapit-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 18:44:27.438945 sapit-1.0.0/sapit/
--rw-rw-rw-   0        0        0       21 2024-04-29 18:37:20.000000 sapit-1.0.0/sapit/__init__.py
--rw-rw-rw-   0        0        0     1250 2024-04-29 18:37:36.000000 sapit-1.0.0/sapit/main.py
-drwxrwxrwx   0        0        0        0 2024-04-29 18:44:27.483928 sapit-1.0.0/sapit.egg-info/
--rw-rw-rw-   0        0        0     1337 2024-04-29 18:44:27.000000 sapit-1.0.0/sapit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-04-29 18:44:27.000000 sapit-1.0.0/sapit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 18:44:27.000000 sapit-1.0.0/sapit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-29 18:44:27.000000 sapit-1.0.0/sapit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-29 18:44:27.000000 sapit-1.0.0/sapit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-29 18:44:27.000000 sapit-1.0.0/sapit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 18:44:27.497912 sapit-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      578 2024-04-29 18:43:57.000000 sapit-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 19:39:41.078136 sapit-1.2.0/
+-rw-rw-rw-   0        0        0     1921 2024-04-29 19:39:41.074139 sapit-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 19:39:41.028166 sapit-1.2.0/sapit/
+-rw-rw-rw-   0        0        0       21 2024-04-29 18:37:20.000000 sapit-1.2.0/sapit/__init__.py
+-rw-rw-rw-   0        0        0     1264 2024-04-29 19:17:24.000000 sapit-1.2.0/sapit/main.py
+drwxrwxrwx   0        0        0        0 2024-04-29 19:39:41.069149 sapit-1.2.0/sapit.egg-info/
+-rw-rw-rw-   0        0        0     1921 2024-04-29 19:39:40.000000 sapit-1.2.0/sapit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-04-29 19:39:40.000000 sapit-1.2.0/sapit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 19:39:40.000000 sapit-1.2.0/sapit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-29 19:39:40.000000 sapit-1.2.0/sapit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-29 19:39:40.000000 sapit-1.2.0/sapit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-29 19:39:40.000000 sapit-1.2.0/sapit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 19:39:41.078136 sapit-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      578 2024-04-29 19:39:12.000000 sapit-1.2.0/setup.py
```

### Comparing `sapit-1.0.0/PKG-INFO` & `sapit-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: sapit
-Version: 1.0.0
+Version: 1.2.0
 Summary: A Text-to-speech module
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pyttsx3==2.90
 Requires-Dist: pydub==0.25.1
 Requires-Dist: ffmpeg==1.4
 
 # Sapit - Python Text-to-Speech Module
 
 Sapit is a Python module that enables users to utilize a text-to-speech function similar to the "say" command on macOS. With Sapit, you can easily convert text into speech in your Python scripts or projects.
 
-# Founder
 
-Sapit was created by "ALI LODHI" He is from Pakistan, Ali lodhi is well experienced python programmer who loves writing python code. The Idea of Sapit came when he was making a Desktop Assistant for his personal use and he had to write a lot of code so that's why to ease of use he created sapit. 
 
 ## Installation
 
 You can install Sapit using pip:
 
 ```bash
 pip install sapit
@@ -30,11 +28,40 @@
 Using Sapit is simple. Just import the `say` function from the `sapit` module and call it with the text you want to convert into speech:
 
 ```python
 from sapit import say
 
 say("Hello, World!")
 ```
+# Founder
+
+Sapit was created by "ALI LODHI" He is from Pakistan, Ali lodhi is well experienced python programmer who loves writing python code. The Idea of Sapit came when he was making a Desktop Assistant for his personal use and he had to write a lot of code so that's why to ease of use he created sapit. 
+
+# Versions
 
-This will result in the text "Hello, World!" being spoken aloud using the default system text-to-speech engine.
+## Sapit 1.0
+
+In Sapit 1.0 you can use `say` function to speak something with the default voice of your Computer
+
+### Example
+
+```python
+from sapit import say
 
-Feel free to adjust any part of the readme to better fit your needs!
+say ("Hello, World!")
+
+# This will result in the text "Hello, World!" being spoken aloud using the default system text-to-speech engine.
+```
+
+## Sapit 1.1 (Latest)
+
+In Sapit 1.1 which is the latest version of Sapit so far you can even specify the voice you want to use It can be male or female
+
+### For Example
+
+```python
+from sapit import say
+
+say ("Hello, World!", gender = "male") # This will speak in Male voice 
+say ("Hello, World!", gender = "female") # This will speak in Female voice
+say ("Hello, World!")# This will speak in Male voice which is default
+```
```

### Comparing `sapit-1.0.0/sapit.egg-info/PKG-INFO` & `sapit-1.2.0/sapit.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: sapit
-Version: 1.0.0
+Version: 1.2.0
 Summary: A Text-to-speech module
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pyttsx3==2.90
 Requires-Dist: pydub==0.25.1
 Requires-Dist: ffmpeg==1.4
 
 # Sapit - Python Text-to-Speech Module
 
 Sapit is a Python module that enables users to utilize a text-to-speech function similar to the "say" command on macOS. With Sapit, you can easily convert text into speech in your Python scripts or projects.
 
-# Founder
 
-Sapit was created by "ALI LODHI" He is from Pakistan, Ali lodhi is well experienced python programmer who loves writing python code. The Idea of Sapit came when he was making a Desktop Assistant for his personal use and he had to write a lot of code so that's why to ease of use he created sapit. 
 
 ## Installation
 
 You can install Sapit using pip:
 
 ```bash
 pip install sapit
@@ -30,11 +28,40 @@
 Using Sapit is simple. Just import the `say` function from the `sapit` module and call it with the text you want to convert into speech:
 
 ```python
 from sapit import say
 
 say("Hello, World!")
 ```
+# Founder
+
+Sapit was created by "ALI LODHI" He is from Pakistan, Ali lodhi is well experienced python programmer who loves writing python code. The Idea of Sapit came when he was making a Desktop Assistant for his personal use and he had to write a lot of code so that's why to ease of use he created sapit. 
+
+# Versions
 
-This will result in the text "Hello, World!" being spoken aloud using the default system text-to-speech engine.
+## Sapit 1.0
+
+In Sapit 1.0 you can use `say` function to speak something with the default voice of your Computer
+
+### Example
+
+```python
+from sapit import say
 
-Feel free to adjust any part of the readme to better fit your needs!
+say ("Hello, World!")
+
+# This will result in the text "Hello, World!" being spoken aloud using the default system text-to-speech engine.
+```
+
+## Sapit 1.1 (Latest)
+
+In Sapit 1.1 which is the latest version of Sapit so far you can even specify the voice you want to use It can be male or female
+
+### For Example
+
+```python
+from sapit import say
+
+say ("Hello, World!", gender = "male") # This will speak in Male voice 
+say ("Hello, World!", gender = "female") # This will speak in Female voice
+say ("Hello, World!")# This will speak in Male voice which is default
+```
```

### Comparing `sapit-1.0.0/setup.py` & `sapit-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'sapit',
-    version = '1.0.0',
+    version = '1.2.0',
     description = 'A Text-to-speech module',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     author_email = 'alilodhibusiness@gmail.com',
     author = 'Ali Lodhi',
     packages = ['sapit'],
     install_requires = [
```

