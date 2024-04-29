# Comparing `tmp/dvtag-0.7.1.tar.gz` & `tmp/dvtag-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvtag-0.7.1.tar", last modified: Sun Apr 28 15:09:05 2024, max compression
+gzip compressed data, was "dvtag-0.7.2.tar", last modified: Mon Apr 29 01:21:32 2024, max compression
```

## Comparing `dvtag-0.7.1.tar` & `dvtag-0.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:09:05.880869 dvtag-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-28 15:08:52.000000 dvtag-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-28 15:09:05.880869 dvtag-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-28 15:08:52.000000 dvtag-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:09:05.880869 dvtag-0.7.1/dvtag/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-28 15:08:52.000000 dvtag-0.7.1/dvtag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-28 15:08:52.000000 dvtag-0.7.1/dvtag/doujinvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-28 15:08:52.000000 dvtag-0.7.1/dvtag/dvtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-28 15:08:52.000000 dvtag-0.7.1/dvtag/scrape.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-28 15:08:52.000000 dvtag-0.7.1/dvtag/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:09:05.880869 dvtag-0.7.1/dvtag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-28 15:09:05.000000 dvtag-0.7.1/dvtag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-28 15:09:05.000000 dvtag-0.7.1/dvtag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:09:05.000000 dvtag-0.7.1/dvtag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-28 15:09:05.000000 dvtag-0.7.1/dvtag.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-28 15:09:05.000000 dvtag-0.7.1/dvtag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 15:09:05.000000 dvtag-0.7.1/dvtag.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-28 15:08:52.000000 dvtag-0.7.1/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-28 15:09:05.880869 dvtag-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:08:52.000000 dvtag-0.7.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-28 15:08:52.000000 dvtag-0.7.1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:21:32.619966 dvtag-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-29 01:21:20.000000 dvtag-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-29 01:21:32.619966 dvtag-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-29 01:21:20.000000 dvtag-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:21:32.619966 dvtag-0.7.2/dvtag/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 01:21:20.000000 dvtag-0.7.2/dvtag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-29 01:21:20.000000 dvtag-0.7.2/dvtag/doujinvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-29 01:21:20.000000 dvtag-0.7.2/dvtag/dvtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-29 01:21:20.000000 dvtag-0.7.2/dvtag/scrape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-29 01:21:20.000000 dvtag-0.7.2/dvtag/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:21:32.619966 dvtag-0.7.2/dvtag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-29 01:21:32.000000 dvtag-0.7.2/dvtag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-29 01:21:32.000000 dvtag-0.7.2/dvtag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 01:21:32.000000 dvtag-0.7.2/dvtag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 01:21:32.000000 dvtag-0.7.2/dvtag.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-29 01:21:32.000000 dvtag-0.7.2/dvtag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 01:21:32.000000 dvtag-0.7.2/dvtag.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-29 01:21:20.000000 dvtag-0.7.2/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-29 01:21:32.623966 dvtag-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 01:21:20.000000 dvtag-0.7.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-29 01:21:20.000000 dvtag-0.7.2/utils.py
```

### Comparing `dvtag-0.7.1/LICENSE` & `dvtag-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvtag-0.7.1/PKG-INFO` & `dvtag-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvtag
-Version: 0.7.1
+Version: 0.7.2
 Summary: A tool for tagging your doujin voice library.
 Home-page: https://github.com/nobekanai/dvtag
 Author: Nobe Kanai
 Author-email: nobekanai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dvtag-0.7.1/README.md` & `dvtag-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `dvtag-0.7.1/dvtag/dvtag.py` & `dvtag-0.7.2/dvtag/dvtag.py`

 * *Files identical despite different names*

### Comparing `dvtag-0.7.1/dvtag/scrape.py` & `dvtag-0.7.2/dvtag/scrape.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import re
 from html import unescape
+from urllib.parse import urljoin
 
 from .doujinvoice import DoujinVoice
 from .utils import create_request_session
 
 session = create_request_session()
 
 __all__ = ["scrape", "ParsingError"]
@@ -32,15 +33,15 @@
     if m := re.search(r'data-product-name="(.+)"\s*data-maker-name="(.+)"', html):
         name = m.group(1)
         circle = m.group(2)
     else:
         raise ParsingError(f"no work name found", workno)
 
     if m := re.search(r"\"og:image\"[\s\S]*?content=\"(.+?)\"", html):
-        image_url = m.group(1)
+        image_url = urljoin("https://www.dlsite.com", m.group(1))
     else:
         raise ParsingError(f"no cover image url found", workno)
 
     seiyus: list[str] = []
     if m := re.search(r"<th>声優</th>[\s\S]*?<td>[\s\S]*?(<a[\s\S]*?>[\s\S]*?)</td>", html):
         seiyu_list_html = m.group(1)
         for seiyu_html in re.finditer(r"<a[\s\S]*?>(.+?)<", seiyu_list_html):
```

### Comparing `dvtag-0.7.1/dvtag/utils.py` & `dvtag-0.7.2/dvtag/utils.py`

 * *Files identical despite different names*

### Comparing `dvtag-0.7.1/dvtag.egg-info/PKG-INFO` & `dvtag-0.7.2/dvtag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvtag
-Version: 0.7.1
+Version: 0.7.2
 Summary: A tool for tagging your doujin voice library.
 Home-page: https://github.com/nobekanai/dvtag
 Author: Nobe Kanai
 Author-email: nobekanai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dvtag-0.7.1/main.py` & `dvtag-0.7.2/main.py`

 * *Files identical despite different names*

### Comparing `dvtag-0.7.1/setup.cfg` & `dvtag-0.7.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dvtag
-version = 0.7.1
+version = 0.7.2
 author = Nobe Kanai
 author_email = nobekanai@gmail.com
 description = A tool for tagging your doujin voice library.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nobekanai/dvtag
 classifiers =
```

### Comparing `dvtag-0.7.1/utils.py` & `dvtag-0.7.2/utils.py`

 * *Files identical despite different names*

