# Comparing `tmp/sapit-1.2.0.tar.gz` & `tmp/sapit-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapit-1.2.0.tar", last modified: Mon Apr 29 19:39:41 2024, max compression
+gzip compressed data, was "sapit-1.4.tar", last modified: Mon Apr 29 19:59:11 2024, max compression
```

## Comparing `sapit-1.2.0.tar` & `sapit-1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 19:39:41.078136 sapit-1.2.0/
--rw-rw-rw-   0        0        0     1921 2024-04-29 19:39:41.074139 sapit-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 19:39:41.028166 sapit-1.2.0/sapit/
--rw-rw-rw-   0        0        0       21 2024-04-29 18:37:20.000000 sapit-1.2.0/sapit/__init__.py
--rw-rw-rw-   0        0        0     1264 2024-04-29 19:17:24.000000 sapit-1.2.0/sapit/main.py
-drwxrwxrwx   0        0        0        0 2024-04-29 19:39:41.069149 sapit-1.2.0/sapit.egg-info/
--rw-rw-rw-   0        0        0     1921 2024-04-29 19:39:40.000000 sapit-1.2.0/sapit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-04-29 19:39:40.000000 sapit-1.2.0/sapit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 19:39:40.000000 sapit-1.2.0/sapit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-29 19:39:40.000000 sapit-1.2.0/sapit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-29 19:39:40.000000 sapit-1.2.0/sapit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-29 19:39:40.000000 sapit-1.2.0/sapit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 19:39:41.078136 sapit-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      578 2024-04-29 19:39:12.000000 sapit-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 19:59:11.197240 sapit-1.4/
+-rw-rw-rw-   0        0        0     2494 2024-04-29 19:59:11.191244 sapit-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 19:59:11.132289 sapit-1.4/sapit/
+-rw-rw-rw-   0        0        0      103 2024-04-29 19:48:14.000000 sapit-1.4/sapit/__init__.py
+-rw-rw-rw-   0        0        0     1238 2024-04-29 19:45:34.000000 sapit-1.4/sapit/main.py
+drwxrwxrwx   0        0        0        0 2024-04-29 19:59:11.185248 sapit-1.4/sapit.egg-info/
+-rw-rw-rw-   0        0        0     2494 2024-04-29 19:59:10.000000 sapit-1.4/sapit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-04-29 19:59:11.000000 sapit-1.4/sapit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 19:59:10.000000 sapit-1.4/sapit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-29 19:59:10.000000 sapit-1.4/sapit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-29 19:59:10.000000 sapit-1.4/sapit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-29 19:59:10.000000 sapit-1.4/sapit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 19:59:11.197240 sapit-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      576 2024-04-29 19:41:45.000000 sapit-1.4/setup.py
```

### Comparing `sapit-1.2.0/PKG-INFO` & `sapit-1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapit
-Version: 1.2.0
+Version: 1.4
 Summary: A Text-to-speech module
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pyttsx3==2.90
 Requires-Dist: pydub==0.25.1
 Requires-Dist: ffmpeg==1.4
@@ -48,20 +48,43 @@
 from sapit import say
 
 say ("Hello, World!")
 
 # This will result in the text "Hello, World!" being spoken aloud using the default system text-to-speech engine.
 ```
 
-## Sapit 1.1 (Latest)
+## Sapit 1.2.0
 
-In Sapit 1.1 which is the latest version of Sapit so far you can even specify the voice you want to use It can be male or female
+In Sapit 1.2.0 you can even specify the voice you want to use It can be male or female
 
 ### For Example
 
 ```python
 from sapit import say
 
 say ("Hello, World!", gender = "male") # This will speak in Male voice 
 say ("Hello, World!", gender = "female") # This will speak in Female voice
 say ("Hello, World!")# This will speak in Male voice which is default
 ```
+
+## Sapit 1.4
+
+Sapit 1.4 is the Biggest update so far and In this Update you can eventually save the file without any problem you can name the file
+
+### Example
+
+```python
+from sapit import save
+
+save ("Sapit is the best", 'best.wav')
+
+save ('''This is a very long script
+that can not be done in one line
+and I want to tell you only one thing
+SAPIT IS THE BEST''', 'best.wav')
+```
+
+### Features of Sapit 1.4
+
+â€¢ You can save your Text-to-speech words into an audio file
+â€¢ You can import male or female voice `from sapit import say_male` and `from sapit import say_female`
+â€¢ Bug Fixes
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sapit-1.2.0/sapit.egg-info/PKG-INFO` & `sapit-1.4/sapit.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapit
-Version: 1.2.0
+Version: 1.4
 Summary: A Text-to-speech module
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pyttsx3==2.90
 Requires-Dist: pydub==0.25.1
 Requires-Dist: ffmpeg==1.4
@@ -48,20 +48,43 @@
 from sapit import say
 
 say ("Hello, World!")
 
 # This will result in the text "Hello, World!" being spoken aloud using the default system text-to-speech engine.
 ```
 
-## Sapit 1.1 (Latest)
+## Sapit 1.2.0
 
-In Sapit 1.1 which is the latest version of Sapit so far you can even specify the voice you want to use It can be male or female
+In Sapit 1.2.0 you can even specify the voice you want to use It can be male or female
 
 ### For Example
 
 ```python
 from sapit import say
 
 say ("Hello, World!", gender = "male") # This will speak in Male voice 
 say ("Hello, World!", gender = "female") # This will speak in Female voice
 say ("Hello, World!")# This will speak in Male voice which is default
 ```
+
+## Sapit 1.4
+
+Sapit 1.4 is the Biggest update so far and In this Update you can eventually save the file without any problem you can name the file
+
+### Example
+
+```python
+from sapit import save
+
+save ("Sapit is the best", 'best.wav')
+
+save ('''This is a very long script
+that can not be done in one line
+and I want to tell you only one thing
+SAPIT IS THE BEST''', 'best.wav')
+```
+
+### Features of Sapit 1.4
+
+â€¢ You can save your Text-to-speech words into an audio file
+â€¢ You can import male or female voice `from sapit import say_male` and `from sapit import say_female`
+â€¢ Bug Fixes
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sapit-1.2.0/setup.py` & `sapit-1.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'sapit',
-    version = '1.2.0',
+    version = '1.4',
     description = 'A Text-to-speech module',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     author_email = 'alilodhibusiness@gmail.com',
     author = 'Ali Lodhi',
     packages = ['sapit'],
     install_requires = [
```

