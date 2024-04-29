# Comparing `tmp/simpleproxymanager-0.1.0.tar.gz` & `tmp/simpleproxymanager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleproxymanager-0.1.0.tar", last modified: Thu Apr 25 22:53:13 2024, max compression
+gzip compressed data, was "simpleproxymanager-0.1.2.tar", last modified: Mon Apr 29 16:42:30 2024, max compression
```

## Comparing `simpleproxymanager-0.1.0.tar` & `simpleproxymanager-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ale       (1000) ale       (1000)        0 2024-04-25 22:53:13.848663 simpleproxymanager-0.1.0/
--rw-r--r--   0 ale       (1000) ale       (1000)    35149 2024-04-25 21:36:14.000000 simpleproxymanager-0.1.0/LICENSE.md
--rw-r--r--   0 ale       (1000) ale       (1000)    43308 2024-04-25 22:53:13.847663 simpleproxymanager-0.1.0/PKG-INFO
--rw-r--r--   0 ale       (1000) ale       (1000)     1977 2024-04-25 21:46:59.000000 simpleproxymanager-0.1.0/README.md
--rw-r--r--   0 ale       (1000) ale       (1000)      887 2024-04-25 21:36:14.000000 simpleproxymanager-0.1.0/pyproject.toml
--rw-r--r--   0 ale       (1000) ale       (1000)       38 2024-04-25 22:53:13.848663 simpleproxymanager-0.1.0/setup.cfg
-drwxr-xr-x   0 ale       (1000) ale       (1000)        0 2024-04-25 22:53:13.846663 simpleproxymanager-0.1.0/src/
-drwxr-xr-x   0 ale       (1000) ale       (1000)        0 2024-04-25 22:53:13.846663 simpleproxymanager-0.1.0/src/SimpleProxyManager/
--rw-r--r--   0 ale       (1000) ale       (1000)     6505 2024-04-25 21:36:14.000000 simpleproxymanager-0.1.0/src/SimpleProxyManager/SimpleProxyManager.py
--rw-r--r--   0 ale       (1000) ale       (1000)       21 2024-04-25 21:36:14.000000 simpleproxymanager-0.1.0/src/SimpleProxyManager/__init__.py
-drwxr-xr-x   0 ale       (1000) ale       (1000)        0 2024-04-25 22:53:13.847663 simpleproxymanager-0.1.0/src/SimpleProxyManager.egg-info/
--rw-r--r--   0 ale       (1000) ale       (1000)    43308 2024-04-25 22:53:13.000000 simpleproxymanager-0.1.0/src/SimpleProxyManager.egg-info/PKG-INFO
--rw-r--r--   0 ale       (1000) ale       (1000)      344 2024-04-25 22:53:13.000000 simpleproxymanager-0.1.0/src/SimpleProxyManager.egg-info/SOURCES.txt
--rw-r--r--   0 ale       (1000) ale       (1000)        1 2024-04-25 22:53:13.000000 simpleproxymanager-0.1.0/src/SimpleProxyManager.egg-info/dependency_links.txt
--rw-r--r--   0 ale       (1000) ale       (1000)       86 2024-04-25 22:53:13.000000 simpleproxymanager-0.1.0/src/SimpleProxyManager.egg-info/requires.txt
--rw-r--r--   0 ale       (1000) ale       (1000)       19 2024-04-25 22:53:13.000000 simpleproxymanager-0.1.0/src/SimpleProxyManager.egg-info/top_level.txt
+drwxr-xr-x   0 ale       (1000) ale       (1000)        0 2024-04-29 16:42:30.821495 simpleproxymanager-0.1.2/
+-rw-r--r--   0 ale       (1000) ale       (1000)    35149 2024-04-25 21:36:14.000000 simpleproxymanager-0.1.2/LICENSE.md
+-rw-r--r--   0 ale       (1000) ale       (1000)    43675 2024-04-29 16:42:30.820495 simpleproxymanager-0.1.2/PKG-INFO
+-rw-r--r--   0 ale       (1000) ale       (1000)     2344 2024-04-29 16:22:36.000000 simpleproxymanager-0.1.2/README.md
+-rw-r--r--   0 ale       (1000) ale       (1000)      970 2024-04-29 16:39:44.000000 simpleproxymanager-0.1.2/pyproject.toml
+-rw-r--r--   0 ale       (1000) ale       (1000)       38 2024-04-29 16:42:30.821495 simpleproxymanager-0.1.2/setup.cfg
+drwxr-xr-x   0 ale       (1000) ale       (1000)        0 2024-04-29 16:42:30.817495 simpleproxymanager-0.1.2/src/
+drwxr-xr-x   0 ale       (1000) ale       (1000)        0 2024-04-29 16:42:30.819495 simpleproxymanager-0.1.2/src/SimpleProxyManager/
+-rw-r--r--   0 ale       (1000) ale       (1000)     6500 2024-04-29 16:22:36.000000 simpleproxymanager-0.1.2/src/SimpleProxyManager/SimpleProxyManager.py
+-rw-r--r--   0 ale       (1000) ale       (1000)       67 2024-04-29 16:22:36.000000 simpleproxymanager-0.1.2/src/SimpleProxyManager/__init__.py
+drwxr-xr-x   0 ale       (1000) ale       (1000)        0 2024-04-29 16:42:30.820495 simpleproxymanager-0.1.2/src/SimpleProxyManager.egg-info/
+-rw-r--r--   0 ale       (1000) ale       (1000)    43675 2024-04-29 16:42:30.000000 simpleproxymanager-0.1.2/src/SimpleProxyManager.egg-info/PKG-INFO
+-rw-r--r--   0 ale       (1000) ale       (1000)      344 2024-04-29 16:42:30.000000 simpleproxymanager-0.1.2/src/SimpleProxyManager.egg-info/SOURCES.txt
+-rw-r--r--   0 ale       (1000) ale       (1000)        1 2024-04-29 16:42:30.000000 simpleproxymanager-0.1.2/src/SimpleProxyManager.egg-info/dependency_links.txt
+-rw-r--r--   0 ale       (1000) ale       (1000)       86 2024-04-29 16:42:30.000000 simpleproxymanager-0.1.2/src/SimpleProxyManager.egg-info/requires.txt
+-rw-r--r--   0 ale       (1000) ale       (1000)       19 2024-04-29 16:42:30.000000 simpleproxymanager-0.1.2/src/SimpleProxyManager.egg-info/top_level.txt
```

### Comparing `simpleproxymanager-0.1.0/LICENSE.md` & `simpleproxymanager-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `simpleproxymanager-0.1.0/PKG-INFO` & `simpleproxymanager-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleProxyManager
-Version: 0.1.0
+Version: 0.1.2
 Summary: Simple Python multithreaded proxy manager, focused on scrapes
 Author-email: "Alessandro G. Magnasco" <amagnasco@gradcenter.cuny.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -693,14 +693,15 @@
 Requires-Dist: requests>=2.31.0
 Requires-Dist: urllib3>=2.2.1
 
 # SimpleProxyManager
 Python multithreaded proxy manager, focused on scrapes
 
 This project lives at https://github.com/amagnasco/SimpleProxyManager. Feel free to submit an issue or improvements!
+Releases: https://pypi.org/project/SimpleProxyManager/
 
 Warning: if using on macOS, don't use this if also using os.fork() due to dependency urllib.request
 
 For an example implementation, check out dev/example.py.
 
 Major dependencies: requests, urllib3.
 
@@ -724,18 +725,26 @@
 
 ## Version History
 This project uses semantic versioning. 
 - ### to-do:
     - improve usage docs
     - improve error handling
     - add test cases
-    - add i18n
     - improve HTTP status code handling
     - differentiate input proxy list by http/https
-    - publish to pypi
     - add a "reset queues to all" method
     - improve manual exit handling
-    - publish github package
     - abstract proxy assigner method from req
     - improve input and type checking
+- ### 0.2.0 (in development):
+    - add i18n
+    - consolidate load conf into one dict/json
+    - improve input and type checking
+    - improve exit condition when 0 proxies available
+- ### 0.1.2:
+    - handle HTTPErrors into general exceptions
+    - simplify class name and init for cleaner import
+    - updated example
+- ### 0.1.1:
+	- added GitHub > PyPi publication workflow
 - ### 0.1.0:
     - First release! Functional enough to share, but some logs might still be in Spanish while I sort out the i18n.
```

### Comparing `simpleproxymanager-0.1.0/README.md` & `simpleproxymanager-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SimpleProxyManager
 Python multithreaded proxy manager, focused on scrapes
 
 This project lives at https://github.com/amagnasco/SimpleProxyManager. Feel free to submit an issue or improvements!
+Releases: https://pypi.org/project/SimpleProxyManager/
 
 Warning: if using on macOS, don't use this if also using os.fork() due to dependency urllib.request
 
 For an example implementation, check out dev/example.py.
 
 Major dependencies: requests, urllib3.
 
@@ -29,18 +30,26 @@
 
 ## Version History
 This project uses semantic versioning. 
 - ### to-do:
     - improve usage docs
     - improve error handling
     - add test cases
-    - add i18n
     - improve HTTP status code handling
     - differentiate input proxy list by http/https
-    - publish to pypi
     - add a "reset queues to all" method
     - improve manual exit handling
-    - publish github package
     - abstract proxy assigner method from req
     - improve input and type checking
+- ### 0.2.0 (in development):
+    - add i18n
+    - consolidate load conf into one dict/json
+    - improve input and type checking
+    - improve exit condition when 0 proxies available
+- ### 0.1.2:
+    - handle HTTPErrors into general exceptions
+    - simplify class name and init for cleaner import
+    - updated example
+- ### 0.1.1:
+	- added GitHub > PyPi publication workflow
 - ### 0.1.0:
     - First release! Functional enough to share, but some logs might still be in Spanish while I sort out the i18n.
```

### Comparing `simpleproxymanager-0.1.0/pyproject.toml` & `simpleproxymanager-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SimpleProxyManager"
-version = "0.1.0"
+dynamic = ["version"]
 description = "Simple Python multithreaded proxy manager, focused on scrapes"
 readme = "README.md"
 authors = [{ name = "Alessandro G. Magnasco", email = "amagnasco@gradcenter.cuny.edu"}]
 license = { file = "LICENSE.md"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
@@ -22,8 +22,11 @@
     "idna>=3.7",
     "requests>=2.31.0",
     "urllib3>=2.2.1"
     ]
 requires-python = ">=3.12"
 
 [project.urls]
-Homepage = "https://github.com/amagnasco/SimpleProxyManager"
+Homepage = "https://github.com/amagnasco/SimpleProxyManager"
+
+[tool.setuptools.dynamic]
+version = {attr = "SimpleProxyManager.__version__"}
```

### Comparing `simpleproxymanager-0.1.0/src/SimpleProxyManager/SimpleProxyManager.py` & `simpleproxymanager-0.1.2/src/SimpleProxyManager/SimpleProxyManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 ### SimpleProxyManager.py
 # by Alessandro G. Magnasco 2024
-# licenced under Creative Commons CC-BY-SA 4.0
+# licenced under GNU GPL
 # https://github.com/amagnasco/SimpleProxyManager
+# https://pypi.org/project/SimpleProxyManager/
 
 # concurrency
 import threading
 import queue
 # HTTP
 import urllib.request
 from urllib.parse import urlparse
 # time management
 import random
 import time
 
-class SimpleProxyManager:
+class ProxyManager:
     def __init__(self, threads, wait, headers, test):
-        self.f = "SimpleProxyManager"
+        self.f = "ProxyManager"
         # conf
         self.threads = threads
         self.wait = wait
         self.headers = headers
         self.test = test
         # proxies
         self.all = queue.Queue()
@@ -163,16 +164,16 @@
                 # wait before requesting
                 time.sleep(random.randint(self.wait['min'], self.wait['max']))
 
                 try:
                     # getter
                     res = self.get(p, uri)
                     #print('status is: ' + str(res.status))
-                except HTTPError as err:
-                    raise Exception(fn + " error: HTTP response was " + str(err.reason))
+                except Exception as err:
+                    raise Exception(fn + " error: trace: " + str(err))
                 else:
                     return {"success": True, "data": res}
 
             raise Exception(fn + " error: no hay proxies disponibles!")
         except Exception as err:
             return {"success": False, "error": err}
```

### Comparing `simpleproxymanager-0.1.0/src/SimpleProxyManager.egg-info/PKG-INFO` & `simpleproxymanager-0.1.2/src/SimpleProxyManager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleProxyManager
-Version: 0.1.0
+Version: 0.1.2
 Summary: Simple Python multithreaded proxy manager, focused on scrapes
 Author-email: "Alessandro G. Magnasco" <amagnasco@gradcenter.cuny.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -693,14 +693,15 @@
 Requires-Dist: requests>=2.31.0
 Requires-Dist: urllib3>=2.2.1
 
 # SimpleProxyManager
 Python multithreaded proxy manager, focused on scrapes
 
 This project lives at https://github.com/amagnasco/SimpleProxyManager. Feel free to submit an issue or improvements!
+Releases: https://pypi.org/project/SimpleProxyManager/
 
 Warning: if using on macOS, don't use this if also using os.fork() due to dependency urllib.request
 
 For an example implementation, check out dev/example.py.
 
 Major dependencies: requests, urllib3.
 
@@ -724,18 +725,26 @@
 
 ## Version History
 This project uses semantic versioning. 
 - ### to-do:
     - improve usage docs
     - improve error handling
     - add test cases
-    - add i18n
     - improve HTTP status code handling
     - differentiate input proxy list by http/https
-    - publish to pypi
     - add a "reset queues to all" method
     - improve manual exit handling
-    - publish github package
     - abstract proxy assigner method from req
     - improve input and type checking
+- ### 0.2.0 (in development):
+    - add i18n
+    - consolidate load conf into one dict/json
+    - improve input and type checking
+    - improve exit condition when 0 proxies available
+- ### 0.1.2:
+    - handle HTTPErrors into general exceptions
+    - simplify class name and init for cleaner import
+    - updated example
+- ### 0.1.1:
+	- added GitHub > PyPi publication workflow
 - ### 0.1.0:
     - First release! Functional enough to share, but some logs might still be in Spanish while I sort out the i18n.
```

