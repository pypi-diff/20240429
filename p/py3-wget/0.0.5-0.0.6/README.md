# Comparing `tmp/py3_wget-0.0.5.tar.gz` & `tmp/py3_wget-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3_wget-0.0.5.tar", last modified: Thu Apr 25 16:10:02 2024, max compression
+gzip compressed data, was "py3_wget-0.0.6.tar", last modified: Mon Apr 29 14:11:54 2024, max compression
```

## Comparing `py3_wget-0.0.5.tar` & `py3_wget-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-25 16:10:02.507089 py3_wget-0.0.5/
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-25 14:41:05.000000 py3_wget-0.0.5/LICENSE
--rw-r--r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-25 16:10:02.507089 py3_wget-0.0.5/PKG-INFO
--rw-rw-r--   0 gaber     (1000) gaber     (1000)      452 2024-04-25 16:03:04.000000 py3_wget-0.0.5/README.md
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-25 16:10:02.507089 py3_wget-0.0.5/py3_wget/
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       32 2024-04-25 14:41:05.000000 py3_wget-0.0.5/py3_wget/__init__.py
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     2476 2024-04-25 16:07:21.000000 py3_wget-0.0.5/py3_wget/main.py
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-25 16:10:02.507089 py3_wget-0.0.5/py3_wget.egg-info/
--rw-r--r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-25 16:10:02.000000 py3_wget-0.0.5/py3_wget.egg-info/PKG-INFO
--rw-rw-r--   0 gaber     (1000) gaber     (1000)      255 2024-04-25 16:10:02.000000 py3_wget-0.0.5/py3_wget.egg-info/SOURCES.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)        1 2024-04-25 16:10:02.000000 py3_wget-0.0.5/py3_wget.egg-info/dependency_links.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       14 2024-04-25 16:10:02.000000 py3_wget-0.0.5/py3_wget.egg-info/requires.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       15 2024-04-25 16:10:02.000000 py3_wget-0.0.5/py3_wget.egg-info/top_level.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       38 2024-04-25 16:10:02.507089 py3_wget-0.0.5/setup.cfg
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     1022 2024-04-25 16:08:48.000000 py3_wget-0.0.5/setup.py
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-25 16:10:02.507089 py3_wget-0.0.5/tests/
--rw-rw-r--   0 gaber     (1000) gaber     (1000)        0 2024-04-25 16:02:23.000000 py3_wget-0.0.5/tests/__init__.py
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     1619 2024-04-25 16:08:26.000000 py3_wget-0.0.5/tests/test.py
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-29 14:11:54.143618 py3_wget-0.0.6/
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-29 14:09:48.000000 py3_wget-0.0.6/LICENSE
+-rw-r--r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-29 14:11:54.143618 py3_wget-0.0.6/PKG-INFO
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)      452 2024-04-29 14:09:48.000000 py3_wget-0.0.6/README.md
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-29 14:11:54.139618 py3_wget-0.0.6/py3_wget/
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       32 2024-04-29 14:09:48.000000 py3_wget-0.0.6/py3_wget/__init__.py
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     2494 2024-04-29 14:10:30.000000 py3_wget-0.0.6/py3_wget/main.py
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-29 14:11:54.143618 py3_wget-0.0.6/py3_wget.egg-info/
+-rw-r--r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-29 14:11:54.000000 py3_wget-0.0.6/py3_wget.egg-info/PKG-INFO
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)      255 2024-04-29 14:11:54.000000 py3_wget-0.0.6/py3_wget.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)        1 2024-04-29 14:11:54.000000 py3_wget-0.0.6/py3_wget.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       14 2024-04-29 14:11:54.000000 py3_wget-0.0.6/py3_wget.egg-info/requires.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       15 2024-04-29 14:11:54.000000 py3_wget-0.0.6/py3_wget.egg-info/top_level.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       38 2024-04-29 14:11:54.143618 py3_wget-0.0.6/setup.cfg
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     1022 2024-04-29 14:11:44.000000 py3_wget-0.0.6/setup.py
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-29 14:11:54.143618 py3_wget-0.0.6/tests/
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)        0 2024-04-29 14:09:48.000000 py3_wget-0.0.6/tests/__init__.py
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     1619 2024-04-29 14:09:48.000000 py3_wget-0.0.6/tests/test.py
```

### Comparing `py3_wget-0.0.5/LICENSE` & `py3_wget-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py3_wget-0.0.5/PKG-INFO` & `py3_wget-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3_wget
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple tool to download files with python, supporting a progress bar
 Author: Gabriele Berton
 Author-email: <berton.gabri@gmail.com>
 Keywords: python,download,progress bar
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py3_wget-0.0.5/py3_wget/main.py` & `py3_wget-0.0.6/py3_wget/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             partial_filename = f"{output_filename}.part"
             if os.path.exists(output_path):
                 print(f"File {output_path} already exists, I won't download it again")
                 return
             
             total_size = int(req.headers.get('content-length', 0))  # Total size in bytes
             
-            tqdm_bar = tqdm(total=total_size, desc=os.path.basename(output_path), unit='iB', unit_scale=True)
+            tqdm_bar = tqdm(total=total_size, desc=os.path.basename(output_path), unit='B', unit_scale=True, unit_divisor=1024)
             with open(partial_filename, 'wb') as file:
                 for data in req.iter_content(block_size_bytes):
                     tqdm_bar.update(len(data))
                     file.write(data)
             tqdm_bar.close()
             if total_size != 0 and tqdm_bar.n != total_size:
                 print(tqdm_bar.n)
```

### Comparing `py3_wget-0.0.5/py3_wget.egg-info/PKG-INFO` & `py3_wget-0.0.6/py3_wget.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3-wget
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple tool to download files with python, supporting a progress bar
 Author: Gabriele Berton
 Author-email: <berton.gabri@gmail.com>
 Keywords: python,download,progress bar
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py3_wget-0.0.5/setup.py` & `py3_wget-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'A simple tool to download files with python, supporting a progress bar'
 
 # Setting up
 setup(
     name="py3_wget",
     version=VERSION,
     author="Gabriele Berton",
```

### Comparing `py3_wget-0.0.5/tests/test.py` & `py3_wget-0.0.6/tests/test.py`

 * *Files identical despite different names*

