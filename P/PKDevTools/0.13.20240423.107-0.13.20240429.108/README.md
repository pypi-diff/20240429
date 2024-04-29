# Comparing `tmp/PKDevTools-0.13.20240423.107.tar.gz` & `tmp/PKDevTools-0.13.20240429.108.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240423.107.tar", last modified: Tue Apr 23 18:43:33 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240429.108.tar", last modified: Mon Apr 29 11:41:41 2024, max compression
```

## Comparing `PKDevTools-0.13.20240423.107.tar` & `PKDevTools-0.13.20240429.108.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:43:33.240993 PKDevTools-0.13.20240423.107/
--rw-rw-rw-   0        0        0     1086 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-23 18:43:33.225363 PKDevTools-0.13.20240423.107/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:43:33.240993 PKDevTools-0.13.20240423.107/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5178 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6380 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2534 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    13778 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     5081 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/PKJoinableQueue.py
--rw-rw-rw-   0        0        0    10832 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     2004 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-23 18:43:28.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16136 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     7430 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:43:33.225363 PKDevTools-0.13.20240423.107/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5204 2024-04-23 18:43:33.000000 PKDevTools-0.13.20240423.107/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1122 2024-04-23 18:43:33.000000 PKDevTools-0.13.20240423.107/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:43:33.000000 PKDevTools-0.13.20240423.107/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-04-23 18:43:33.000000 PKDevTools-0.13.20240423.107/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 18:43:26.000000 PKDevTools-0.13.20240423.107/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-04-23 18:43:33.000000 PKDevTools-0.13.20240423.107/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-23 18:43:33.000000 PKDevTools-0.13.20240423.107/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5204 2024-04-23 18:43:33.240993 PKDevTools-0.13.20240423.107/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/README.md
--rw-rw-rw-   0        0        0       86 2024-04-23 18:43:33.240993 PKDevTools-0.13.20240423.107/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-04-23 18:42:09.000000 PKDevTools-0.13.20240423.107/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:41:41.536074 PKDevTools-0.13.20240429.108/
+-rw-rw-rw-   0        0        0     1086 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-29 11:41:41.520458 PKDevTools-0.13.20240429.108/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:41:41.536074 PKDevTools-0.13.20240429.108/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5178 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6380 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2534 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    14378 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     5081 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/PKJoinableQueue.py
+-rw-rw-rw-   0        0        0    10832 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     2004 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-29 11:41:36.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16136 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     7430 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:41:41.520458 PKDevTools-0.13.20240429.108/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-04-29 11:41:41.000000 PKDevTools-0.13.20240429.108/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1122 2024-04-29 11:41:41.000000 PKDevTools-0.13.20240429.108/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 11:41:41.000000 PKDevTools-0.13.20240429.108/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-04-29 11:41:41.000000 PKDevTools-0.13.20240429.108/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-29 11:41:34.000000 PKDevTools-0.13.20240429.108/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      176 2024-04-29 11:41:41.000000 PKDevTools-0.13.20240429.108/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-29 11:41:41.000000 PKDevTools-0.13.20240429.108/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5204 2024-04-29 11:41:41.536074 PKDevTools-0.13.20240429.108/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-29 11:41:41.536074 PKDevTools-0.13.20240429.108/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-04-29 11:40:40.000000 PKDevTools-0.13.20240429.108/setup.py
```

### Comparing `PKDevTools-0.13.20240423.107/LICENSE` & `PKDevTools-0.13.20240429.108/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/__init__.py` & `PKDevTools-0.13.20240429.108/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/PKDateUtilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 
 """
+import os
+import json
 import calendar
 import numpy as np
 import pytz
 import pandas as pd
 import datetime
 import requests
 from datetime import timezone
@@ -152,17 +154,26 @@
         if simulate:
             return curr.replace(year=year if year is not None else curr.year,
                                 month=month if month is not None else curr.month,
                                 day=day if day is not None else curr.day,
                                 hour=hour if hour is not None else curr.hour,
                                 minute=minute if minute is not None else curr.minute,)
         else:
+            if "simulation" in os.environ.keys():
+                simulatedEnvs = json.loads(os.environ["simulation"])
+                if "currentDateTime" in simulatedEnvs.keys():
+                    dttime = datetime.datetime.strptime(simulatedEnvs["currentDateTime"], "%Y-%m-%d %H:%M:%S").replace(tzinfo=curr.tzinfo)
+                    return dttime
             return curr
 
     def isTradingTime():
+        if "simulation" in os.environ.keys():
+            simulatedEnvs = json.loads(os.environ["simulation"])
+            if "isTrading" in simulatedEnvs.keys():
+                return simulatedEnvs["isTrading"]
         curr = PKDateUtilities.currentDateTime()
         openTime = curr.replace(hour=9, minute=15)
         closeTime = curr.replace(hour=15, minute=30)
         return (openTime <= curr <= closeTime) and PKDateUtilities.isTradingWeekday()
 
     def isTradingWeekday(checkDate=None):
         if checkDate is None:
```

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/PKJoinableQueue.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/PKJoinableQueue.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240429.108/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240429.108/PKDevTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240423.107
+Version: 0.13.20240429.108
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240423.107.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240429.108.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240423.107/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240429.108/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/PKG-INFO` & `PKDevTools-0.13.20240429.108/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240423.107
+Version: 0.13.20240429.108
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240423.107.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240429.108.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240423.107/README.md` & `PKDevTools-0.13.20240429.108/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.107/setup.py` & `PKDevTools-0.13.20240429.108/setup.py`

 * *Files identical despite different names*

