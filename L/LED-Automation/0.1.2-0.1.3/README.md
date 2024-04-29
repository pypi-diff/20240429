# Comparing `tmp/LED-Automation-0.1.2.tar.gz` & `tmp/LED-Automation-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LED-Automation-0.1.2.tar", last modified: Tue Apr 16 21:11:25 2024, max compression
+gzip compressed data, was "LED-Automation-0.1.3.tar", last modified: Mon Apr 29 15:57:46 2024, max compression
```

## Comparing `LED-Automation-0.1.2.tar` & `LED-Automation-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 21:11:25.189192 LED-Automation-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-04-16 21:11:25.182163 LED-Automation-0.1.2/LEDAutomation/
--rw-rw-rw-   0        0        0     5133 2024-04-15 18:31:44.000000 LED-Automation-0.1.2/LEDAutomation/FtdiInterface.py
--rw-rw-rw-   0        0        0      748 2024-04-15 18:36:39.000000 LED-Automation-0.1.2/LEDAutomation/LedConsole.py
--rw-rw-rw-   0        0        0     6901 2024-04-15 18:31:44.000000 LED-Automation-0.1.2/LEDAutomation/PCA9506.py
--rw-rw-rw-   0        0        0      624 2024-03-04 21:44:33.000000 LED-Automation-0.1.2/LEDAutomation/USBs.py
--rw-rw-rw-   0        0        0        0 2024-04-15 18:32:03.000000 LED-Automation-0.1.2/LEDAutomation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 21:11:25.188184 LED-Automation-0.1.2/LED_Automation.egg-info/
--rw-rw-rw-   0        0        0      760 2024-04-16 21:11:25.000000 LED-Automation-0.1.2/LED_Automation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2024-04-16 21:11:25.000000 LED-Automation-0.1.2/LED_Automation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 21:11:25.000000 LED-Automation-0.1.2/LED_Automation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-16 21:11:25.000000 LED-Automation-0.1.2/LED_Automation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-16 21:11:25.000000 LED-Automation-0.1.2/LED_Automation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      760 2024-04-16 21:11:25.189192 LED-Automation-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      345 2024-04-15 18:31:44.000000 LED-Automation-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-16 21:11:25.190152 LED-Automation-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1042 2024-04-16 21:11:18.000000 LED-Automation-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:57:46.647849 LED-Automation-0.1.3/
+drwxrwxrwx   0        0        0        0 2024-04-29 15:57:46.638849 LED-Automation-0.1.3/LEDAutomation/
+-rw-rw-rw-   0        0        0     5135 2024-04-29 15:49:44.000000 LED-Automation-0.1.3/LEDAutomation/FtdiInterface.py
+-rw-rw-rw-   0        0        0      748 2024-04-15 18:36:39.000000 LED-Automation-0.1.3/LEDAutomation/LedConsole.py
+-rw-rw-rw-   0        0        0     6901 2024-04-15 18:31:44.000000 LED-Automation-0.1.3/LEDAutomation/PCA9506.py
+-rw-rw-rw-   0        0        0      624 2024-03-04 21:44:33.000000 LED-Automation-0.1.3/LEDAutomation/USBs.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 18:32:03.000000 LED-Automation-0.1.3/LEDAutomation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:57:46.645849 LED-Automation-0.1.3/LED_Automation.egg-info/
+-rw-rw-rw-   0        0        0      585 2024-04-29 15:57:46.000000 LED-Automation-0.1.3/LED_Automation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2024-04-29 15:57:46.000000 LED-Automation-0.1.3/LED_Automation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 15:57:46.000000 LED-Automation-0.1.3/LED_Automation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-29 15:57:46.000000 LED-Automation-0.1.3/LED_Automation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-29 15:57:46.000000 LED-Automation-0.1.3/LED_Automation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      585 2024-04-29 15:57:46.646849 LED-Automation-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2024-04-15 18:31:44.000000 LED-Automation-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 15:57:46.647849 LED-Automation-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      856 2024-04-29 15:47:32.000000 LED-Automation-0.1.3/setup.py
```

### Comparing `LED-Automation-0.1.2/LEDAutomation/FtdiInterface.py` & `LED-Automation-0.1.3/LEDAutomation/FtdiInterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pyftdi.i2c as i2c
 from enum import IntFlag
 from typing import List
+import PCA9506 as GPIOExpander
 from PCA9506 import GPIOEnum
 from PCA9506 import ExpanderGPIOAddress
-import PCA9506 as GPIOExpander
+
 # Requires PyFTDI to be installed on the device and the FTDI device to be plugged in
 
 # Scripts in the Scripts folder for finding connected i2C devices
 # py .venv/Scripts/i2cscan.py
 
 
 # Board won't be changing, so having items for the , pinout might change for the console buttons etc, so make sure those are provided via a map or something.
```

### Comparing `LED-Automation-0.1.2/LEDAutomation/LedConsole.py` & `LED-Automation-0.1.3/LEDAutomation/LedConsole.py`

 * *Files identical despite different names*

### Comparing `LED-Automation-0.1.2/LEDAutomation/PCA9506.py` & `LED-Automation-0.1.3/LEDAutomation/PCA9506.py`

 * *Files identical despite different names*

### Comparing `LED-Automation-0.1.2/LEDAutomation/USBs.py` & `LED-Automation-0.1.3/LEDAutomation/USBs.py`

 * *Files identical despite different names*

### Comparing `LED-Automation-0.1.2/LED_Automation.egg-info/PKG-INFO` & `LED-Automation-0.1.3/LED_Automation.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 Metadata-Version: 2.1
 Name: LED-Automation
-Version: 0.1.2
+Version: 0.1.3
 Summary: LED Automation library
-Home-page: https://about.readthedocs.com/?ref=readthedocs.org
-Author: Joshua Parker
-Author-email: Joshua.Parker@johnsonfit.com
-Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 ## Goal of this project
 Create a general purpose library that can be used to automate testing of the LED/PLED Mainboards
```

### Comparing `LED-Automation-0.1.2/PKG-INFO` & `LED-Automation-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 Metadata-Version: 2.1
 Name: LED-Automation
-Version: 0.1.2
+Version: 0.1.3
 Summary: LED Automation library
-Home-page: https://about.readthedocs.com/?ref=readthedocs.org
-Author: Joshua Parker
-Author-email: Joshua.Parker@johnsonfit.com
-Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 ## Goal of this project
 Create a general purpose library that can be used to automate testing of the LED/PLED Mainboards
```

### Comparing `LED-Automation-0.1.2/setup.py` & `LED-Automation-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,23 +11,19 @@
 # Get the long description from the README.md file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="LED-Automation",
-    version="0.1.2",
+    version="0.1.3",
     description="LED Automation library",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://about.readthedocs.com/?ref=readthedocs.org",
-    author="Joshua Parker",
-    author_email="Joshua.Parker@johnsonfit.com",
     classifiers=[
-        "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Operating System :: OS Independent"
     ],
     packages=["LEDAutomation"],
     include_package_data=True,
     install_requires=["numpy"]
 )
```

