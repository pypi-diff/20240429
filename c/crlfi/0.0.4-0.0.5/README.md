# Comparing `tmp/crlfi-0.0.4.tar.gz` & `tmp/crlfi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crlfi-0.0.4.tar", last modified: Tue Apr 23 10:31:36 2024, max compression
+gzip compressed data, was "crlfi-0.0.5.tar", last modified: Mon Apr 29 16:41:23 2024, max compression
```

## Comparing `crlfi-0.0.4.tar` & `crlfi-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 10:31:36.651025 crlfi-0.0.4/
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1074 2024-04-23 05:50:39.000000 crlfi-0.0.4/LICENSE
--rw-r--r--   0 karthikeyan   (501) staff       (20)     4752 2024-04-23 10:31:36.650846 crlfi-0.0.4/PKG-INFO
--rw-r--r--   0 karthikeyan   (501) staff       (20)     4299 2024-04-23 10:27:02.000000 crlfi-0.0.4/README.md
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 10:31:36.646198 crlfi-0.0.4/crlfi.egg-info/
--rw-r--r--   0 karthikeyan   (501) staff       (20)     4752 2024-04-23 10:31:36.000000 crlfi-0.0.4/crlfi.egg-info/PKG-INFO
--rw-r--r--   0 karthikeyan   (501) staff       (20)      454 2024-04-23 10:31:36.000000 crlfi-0.0.4/crlfi.egg-info/SOURCES.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)        1 2024-04-23 10:31:36.000000 crlfi-0.0.4/crlfi.egg-info/dependency_links.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)       40 2024-04-23 10:31:36.000000 crlfi-0.0.4/crlfi.egg-info/entry_points.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)       23 2024-04-23 10:31:36.000000 crlfi-0.0.4/crlfi.egg-info/requires.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)        4 2024-04-23 10:31:36.000000 crlfi-0.0.4/crlfi.egg-info/top_level.txt
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 10:31:36.646928 crlfi-0.0.4/cve/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-23 05:42:44.000000 crlfi-0.0.4/cve/__init__.py
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 10:31:36.648678 crlfi-0.0.4/cve/includes/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-01-04 13:26:47.000000 crlfi-0.0.4/cve/includes/__init__.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      629 2024-04-23 06:03:03.000000 crlfi-0.0.4/cve/includes/bot.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      456 2024-04-23 06:03:12.000000 crlfi-0.0.4/cve/includes/filereader.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     2248 2024-04-23 06:03:29.000000 crlfi-0.0.4/cve/includes/scan.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      267 2024-04-21 11:46:48.000000 crlfi-0.0.4/cve/includes/writefile.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1724 2024-04-23 06:02:23.000000 crlfi-0.0.4/cve/main.py
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 10:31:36.650385 crlfi-0.0.4/cve/utils/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-01-04 13:25:36.000000 crlfi-0.0.4/cve/utils/__init__.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1946 2024-04-23 06:02:44.000000 crlfi-0.0.4/cve/utils/configure.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      796 2024-04-23 08:50:24.000000 crlfi-0.0.4/cve/utils/const.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1697 2024-04-21 12:43:27.000000 crlfi-0.0.4/cve/utils/helpers.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      227 2024-02-12 08:19:58.000000 crlfi-0.0.4/cve/utils/status.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)       38 2024-04-23 10:31:36.651099 crlfi-0.0.4/setup.cfg
--rw-r--r--   0 karthikeyan   (501) staff       (20)      978 2024-04-23 10:31:09.000000 crlfi-0.0.4/setup.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:41:23.191813 crlfi-0.0.5/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1074 2024-04-29 16:39:36.000000 crlfi-0.0.5/LICENSE
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     4752 2024-04-29 16:41:23.191637 crlfi-0.0.5/PKG-INFO
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     4299 2024-04-29 16:39:36.000000 crlfi-0.0.5/README.md
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:41:23.185231 crlfi-0.0.5/crlfi/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/__init__.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:41:23.189848 crlfi-0.0.5/crlfi/includes/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/includes/__init__.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      633 2024-04-29 16:40:08.000000 crlfi-0.0.5/crlfi/includes/bot.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      458 2024-04-29 16:40:08.000000 crlfi-0.0.5/crlfi/includes/filereader.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     2256 2024-04-29 16:40:08.000000 crlfi-0.0.5/crlfi/includes/scan.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      267 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/includes/writefile.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1736 2024-04-29 16:40:08.000000 crlfi-0.0.5/crlfi/main.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:41:23.191315 crlfi-0.0.5/crlfi/utils/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/utils/__init__.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1948 2024-04-29 16:40:08.000000 crlfi-0.0.5/crlfi/utils/configure.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      662 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/utils/const.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1697 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/utils/helpers.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      227 2024-04-29 16:39:36.000000 crlfi-0.0.5/crlfi/utils/status.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-29 16:41:23.188189 crlfi-0.0.5/crlfi.egg-info/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     4752 2024-04-29 16:41:23.000000 crlfi-0.0.5/crlfi.egg-info/PKG-INFO
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      478 2024-04-29 16:41:23.000000 crlfi-0.0.5/crlfi.egg-info/SOURCES.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        1 2024-04-29 16:41:23.000000 crlfi-0.0.5/crlfi.egg-info/dependency_links.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       42 2024-04-29 16:41:23.000000 crlfi-0.0.5/crlfi.egg-info/entry_points.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       23 2024-04-29 16:41:23.000000 crlfi-0.0.5/crlfi.egg-info/requires.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        6 2024-04-29 16:41:23.000000 crlfi-0.0.5/crlfi.egg-info/top_level.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       38 2024-04-29 16:41:23.191873 crlfi-0.0.5/setup.cfg
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      980 2024-04-29 16:41:19.000000 crlfi-0.0.5/setup.py
```

### Comparing `crlfi-0.0.4/LICENSE` & `crlfi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.4/PKG-INFO` & `crlfi-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crlfi
-Version: 0.0.4
+Version: 0.0.5
 Author: @cappriciosec
 Author-email: <contact@cappriciosec.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crlfi Version: 0.0.4 Author: @cappriciosec Author-
+Metadata-Version: 2.1 Name: crlfi Version: 0.0.5 Author: @cappriciosec Author-
 email:
 cappriciosec.com> Classifier: Development Status :: 1 - Planning Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
 Content-Type: text/markdown License-File: LICENSE
                                     [logo]
```

### Comparing `crlfi-0.0.4/README.md` & `crlfi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.4/crlfi.egg-info/PKG-INFO` & `crlfi-0.0.5/crlfi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crlfi
-Version: 0.0.4
+Version: 0.0.5
 Author: @cappriciosec
 Author-email: <contact@cappriciosec.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crlfi Version: 0.0.4 Author: @cappriciosec Author-
+Metadata-Version: 2.1 Name: crlfi Version: 0.0.5 Author: @cappriciosec Author-
 email:
 cappriciosec.com> Classifier: Development Status :: 1 - Planning Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
 Content-Type: text/markdown License-File: LICENSE
                                     [logo]
```

### Comparing `crlfi-0.0.4/cve/includes/bot.py` & `crlfi-0.0.5/crlfi/includes/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
  * crlfi
  * crlfi Bug scanner for WebPentesters and Bugbounty Hunters
  *
  * @Developed By Cappricio Securities <https://cappriciosec.com>
  */
 """
 import requests
-from cve.utils import const
-from cve.utils import configure
+from crlfi.utils import const
+from crlfi.utils import configure
 
 
 def sendmessage(vul):
 
     data = {"Tname": "crlfi", "chatid": configure.get_chatid(), "data": vul,
             "Blog": const.Data.blog, "bugname": const.Data.bugname, "Priority": "Low"}
```

### Comparing `crlfi-0.0.4/cve/includes/scan.py` & `crlfi-0.0.5/crlfi/includes/scan.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,21 @@
  * crlfi
  * crlfi Bug scanner for WebPentesters and Bugbounty Hunters
  *
  * @Developed By Cappricio Securities <https://cappriciosec.com>
  */
  
 """
-from cve.includes import bot
-from cve.utils import configure
+from crlfi.includes import bot
+from crlfi.utils import configure
 import requests
 from urllib3.exceptions import InsecureRequestWarning
 from urllib.parse import quote
-from cve.includes import writefile
-from cve.utils import const
+from crlfi.includes import writefile
+from crlfi.utils import const
 requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 
 
 
 def cvescan(url, output):
     try:
         with requests.Session() as session:
```

### Comparing `crlfi-0.0.4/cve/main.py` & `crlfi-0.0.5/crlfi/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,20 +6,20 @@
  *
  * @Developed By Cappricio Securities <https://cappriciosec.com>
  */
 
 
 """
 import click
-from cve.utils import helpers
-from cve.includes import scan
-from cve.includes import filereader
-from cve.utils import configure
-from cve.utils import const
-from cve.utils import status
+from crlfi.utils import helpers
+from crlfi.includes import scan
+from crlfi.includes import filereader
+from crlfi.utils import configure
+from crlfi.utils import const
+from crlfi.utils import status
 import webbrowser
 import os
 
 
 def helpbanner(ctx, params, value):
     if value:
         helpers.display_help()
```

### Comparing `crlfi-0.0.4/cve/utils/configure.py` & `crlfi-0.0.5/crlfi/utils/configure.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
  * @Developed By Cappricio Securities <https://cappriciosec.com>
  */
 
 
 """
 import os
 import yaml
-from cve.utils import const
+from crlfi.utils import const
 
 
 def new_chatid(chatid):
     yaml_file_path = os.path.expanduser(
         const.Data.config_path)
     folder_path = os.path.dirname(yaml_file_path)
     os.makedirs(folder_path, exist_ok=True)
```

### Comparing `crlfi-0.0.4/cve/utils/const.py` & `crlfi-0.0.5/crlfi/utils/const.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,15 @@
  */
 
 
 """
 
 
 class Data:
-    blog = 'https://blogs.cappriciosec.com/blog/138/Cappricio%20Securities%20Discovers%20CRLF%20Injection%20Vulnerability%20in%20Popular%20Website,%20Responsible%20Disclosure%20Earns%20Bounty'
+    blog = 'https://blogs.cappriciosec.com/blog/137/crlfi'
     api = 'https://api.cappriciosec.com/Telegram/cappriciosecbot.php'
     config_path = '~/.config/cappriciosec-tools/cappriciosec.yaml'
     payloadurl = 'https://raw.githubusercontent.com/Cappricio-Securities/PayloadAllTheThings/main/crlfi.txt'
     bugname = 'CRLF Injection'
 
 
 class Colors:
```

### Comparing `crlfi-0.0.4/cve/utils/helpers.py` & `crlfi-0.0.5/crlfi/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.4/setup.py` & `crlfi-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'A Tool to find an Easy Bounty - crlfi'
 LONG_DESCRIPTION = 'This is a tool used by several security researchers to find Carriage Return Line Feed Injection Bug'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
@@ -12,15 +12,15 @@
     version=VERSION,
     author="@cappriciosec",
     author_email="<contact@cappriciosec.com>",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': [
-            'crlfi = cve.main:main',
+            'crlfi = crlfi.main:main',
         ],
     },
     install_requires=['urllib3', 'requests', 'click'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

