# Comparing `tmp/cammello-0.0.1.tar.gz` & `tmp/cammello-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cammello-0.0.1.tar", last modified: Fri Jun  9 22:02:22 2023, max compression
+gzip compressed data, was "cammello-0.0.2.tar", last modified: Mon Apr 29 19:02:41 2024, max compression
```

## Comparing `cammello-0.0.1.tar` & `cammello-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-09 22:02:22.425253 cammello-0.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1073 2023-06-09 22:00:50.000000 cammello-0.0.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1094 2023-06-09 22:02:22.425253 cammello-0.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      654 2023-06-09 21:55:11.000000 cammello-0.0.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-09 22:02:22.421253 cammello-0.0.1/cammello/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      280 2023-06-09 21:59:19.000000 cammello-0.0.1/cammello/__about__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2023-06-09 21:46:53.000000 cammello-0.0.1/cammello/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      221 2023-06-09 21:49:54.000000 cammello-0.0.1/cammello/cammello.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-09 22:02:22.425253 cammello-0.0.1/cammello/res/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17814 2023-06-09 21:56:32.000000 cammello-0.0.1/cammello/res/616532.png
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-09 22:02:22.425253 cammello-0.0.1/cammello.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1094 2023-06-09 22:02:22.000000 cammello-0.0.1/cammello.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      242 2023-06-09 22:02:22.000000 cammello-0.0.1/cammello.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-09 22:02:22.000000 cammello-0.0.1/cammello.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-06-09 22:02:22.000000 cammello-0.0.1/cammello.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-09 22:02:22.425253 cammello-0.0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      838 2023-06-09 22:02:05.000000 cammello-0.0.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-29 19:02:41.246324 cammello-0.0.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1073 2024-04-29 18:55:15.000000 cammello-0.0.2/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     1023 2024-04-29 19:02:41.246324 cammello-0.0.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      590 2024-04-29 18:55:15.000000 cammello-0.0.2/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-29 19:02:41.246324 cammello-0.0.2/cammello/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      194 2024-04-29 18:59:02.000000 cammello-0.0.2/cammello/__about__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       32 2024-04-29 18:59:50.000000 cammello-0.0.2/cammello/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2024-04-29 18:55:15.000000 cammello-0.0.2/cammello/cammello.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-29 19:02:41.246324 cammello-0.0.2/cammello/res/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17814 2024-04-29 18:55:15.000000 cammello-0.0.2/cammello/res/cammello.png
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-29 19:02:41.246324 cammello-0.0.2/cammello.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     1023 2024-04-29 19:02:41.000000 cammello-0.0.2/cammello.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      244 2024-04-29 19:02:41.000000 cammello-0.0.2/cammello.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-29 19:02:41.000000 cammello-0.0.2/cammello.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2024-04-29 19:02:41.000000 cammello-0.0.2/cammello.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-29 19:02:41.246324 cammello-0.0.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      838 2024-04-29 18:55:15.000000 cammello-0.0.2/setup.py
```

### Comparing `cammello-0.0.1/LICENSE` & `cammello-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cammello-0.0.1/PKG-INFO` & `cammello-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cammello
-Version: 0.0.1
-Summary: A singing Cammello.
+Version: 0.0.2
+Summary: Un cammello.
 Home-page: https://github.com/LucaMingarelli/cammello
 Author: Luca Mingarelli
 Author-email: lucamingarelli@me.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Cammello <img src="https://raw.githubusercontent.com/LucaMingarelli/cammello/master/cammello/res/cammello.png"  width="80">
+# Cammello <img src="/cammello/res/cammello.png"  width="80">
 
 [![version](https://img.shields.io/badge/version-0.0.1-success.svg)](#)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cammello.svg)](https://pypi.org/project/cammello/)
 [![License](https://img.shields.io/pypi/l/cammello.svg)](https://github.com/LucaMingarelli/cammello/blob/master/LICENSE.txt)
 
 [//]: # ([![Downloads]&#40;https://static.pepy.tech/personalized-badge/cammello?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads&#41;]&#40;https://pepy.tech/project/cammello&#41;)
```

### Comparing `cammello-0.0.1/README.md` & `cammello-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-# Cammello <img src="https://raw.githubusercontent.com/LucaMingarelli/cammello/master/cammello/res/cammello.png"  width="80">
+# Cammello <img src="/cammello/res/cammello.png"  width="80">
 
 [![version](https://img.shields.io/badge/version-0.0.1-success.svg)](#)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cammello.svg)](https://pypi.org/project/cammello/)
 [![License](https://img.shields.io/pypi/l/cammello.svg)](https://github.com/LucaMingarelli/cammello/blob/master/LICENSE.txt)
 
 [//]: # ([![Downloads]&#40;https://static.pepy.tech/personalized-badge/cammello?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads&#41;]&#40;https://pepy.tech/project/cammello&#41;)
```

### Comparing `cammello-0.0.1/cammello/res/616532.png` & `cammello-0.0.2/cammello/res/cammello.png`

 * *Files identical despite different names*

### Comparing `cammello-0.0.1/cammello.egg-info/PKG-INFO` & `cammello-0.0.2/cammello.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cammello
-Version: 0.0.1
-Summary: A singing Cammello.
+Version: 0.0.2
+Summary: Un cammello.
 Home-page: https://github.com/LucaMingarelli/cammello
 Author: Luca Mingarelli
 Author-email: lucamingarelli@me.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Cammello <img src="https://raw.githubusercontent.com/LucaMingarelli/cammello/master/cammello/res/cammello.png"  width="80">
+# Cammello <img src="/cammello/res/cammello.png"  width="80">
 
 [![version](https://img.shields.io/badge/version-0.0.1-success.svg)](#)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cammello.svg)](https://pypi.org/project/cammello/)
 [![License](https://img.shields.io/pypi/l/cammello.svg)](https://github.com/LucaMingarelli/cammello/blob/master/LICENSE.txt)
 
 [//]: # ([![Downloads]&#40;https://static.pepy.tech/personalized-badge/cammello?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads&#41;]&#40;https://pepy.tech/project/cammello&#41;)
```

### Comparing `cammello-0.0.1/setup.py` & `cammello-0.0.2/setup.py`

 * *Files identical despite different names*

