# Comparing `tmp/twettletwattletwattle-0.0.1.tar.gz` & `tmp/twettletwattletwattle-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twettletwattletwattle-0.0.1.tar", last modified: Tue Oct 17 16:41:55 2023, max compression
+gzip compressed data, was "twettletwattletwattle-1.0.0.tar", last modified: Mon Apr 29 19:49:49 2024, max compression
```

## Comparing `twettletwattletwattle-0.0.1.tar` & `twettletwattletwattle-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zazzz      (501) staff       (20)        0 2023-10-17 16:41:55.706286 twettletwattletwattle-0.0.1/
--rw-r--r--   0 zazzz      (501) staff       (20)    35149 2023-10-17 16:30:58.000000 twettletwattletwattle-0.0.1/LICENSE
--rw-r--r--   0 zazzz      (501) staff       (20)       81 2023-10-17 16:38:57.000000 twettletwattletwattle-0.0.1/MANIFEST.in
--rw-r--r--   0 zazzz      (501) staff       (20)      441 2023-10-17 16:41:55.706046 twettletwattletwattle-0.0.1/PKG-INFO
--rw-r--r--   0 zazzz      (501) staff       (20)       23 2023-10-17 16:32:41.000000 twettletwattletwattle-0.0.1/README.md
--rw-r--r--   0 zazzz      (501) staff       (20)      103 2023-10-17 16:30:58.000000 twettletwattletwattle-0.0.1/pyproject.toml
--rw-r--r--   0 zazzz      (501) staff       (20)       38 2023-10-17 16:41:55.706333 twettletwattletwattle-0.0.1/setup.cfg
--rw-r--r--   0 zazzz      (501) staff       (20)      755 2023-10-17 16:41:49.000000 twettletwattletwattle-0.0.1/setup.py
-drwxr-xr-x   0 zazzz      (501) staff       (20)        0 2023-10-17 16:41:55.703359 twettletwattletwattle-0.0.1/twettletwattletwattle/
--rw-r--r--   0 zazzz      (501) staff       (20)     6148 2023-10-17 16:36:51.000000 twettletwattletwattle-0.0.1/twettletwattletwattle/.DS_Store
-drwxr-xr-x   0 zazzz      (501) staff       (20)        0 2023-10-17 16:41:55.705253 twettletwattletwattle-0.0.1/twettletwattletwattle/src/
--rw-r--r--   0 zazzz      (501) staff       (20)        1 2023-10-17 16:30:58.000000 twettletwattletwattle-0.0.1/twettletwattletwattle/src/__init__.py
--rw-r--r--   0 zazzz      (501) staff       (20)       92 2023-10-17 16:34:13.000000 twettletwattletwattle-0.0.1/twettletwattletwattle/src/__main__.py
--rw-rw-r--   0 zazzz      (501) staff       (20)  1355264 2022-09-19 20:44:40.000000 twettletwattletwattle-0.0.1/twettletwattletwattle/src/mimikatz.exe
--rw-r--r--   0 zazzz      (501) staff       (20)  1206166 2023-10-17 16:35:42.000000 twettletwattletwattle-0.0.1/twettletwattletwattle/src/mimikatz_trunk.zip
--rw-rw-r--   0 zazzz      (501) staff       (20)    37376 2022-09-19 20:44:02.000000 twettletwattletwattle-0.0.1/twettletwattletwattle/src/mimilib.dll
-drwxr-xr-x   0 zazzz      (501) staff       (20)        0 2023-10-17 16:41:55.705782 twettletwattletwattle-0.0.1/twettletwattletwattle/src/twettletwattletwattle.egg-info/
--rw-r--r--   0 zazzz      (501) staff       (20)      441 2023-10-17 16:41:55.000000 twettletwattletwattle-0.0.1/twettletwattletwattle/src/twettletwattletwattle.egg-info/PKG-INFO
--rw-r--r--   0 zazzz      (501) staff       (20)      567 2023-10-17 16:41:55.000000 twettletwattletwattle-0.0.1/twettletwattletwattle/src/twettletwattletwattle.egg-info/SOURCES.txt
--rw-r--r--   0 zazzz      (501) staff       (20)        1 2023-10-17 16:41:55.000000 twettletwattletwattle-0.0.1/twettletwattletwattle/src/twettletwattletwattle.egg-info/dependency_links.txt
--rw-r--r--   0 zazzz      (501) staff       (20)        1 2023-10-17 16:41:55.000000 twettletwattletwattle-0.0.1/twettletwattletwattle/src/twettletwattletwattle.egg-info/top_level.txt
+drwxr-xr-x   0 zazzz      (501) staff       (20)        0 2024-04-29 19:49:49.199257 twettletwattletwattle-1.0.0/
+-rw-r--r--   0 zazzz      (501) staff       (20)    35149 2023-10-17 16:30:58.000000 twettletwattletwattle-1.0.0/LICENSE
+-rw-r--r--   0 zazzz      (501) staff       (20)       81 2023-10-17 16:38:57.000000 twettletwattletwattle-1.0.0/MANIFEST.in
+-rw-r--r--   0 zazzz      (501) staff       (20)      441 2024-04-29 19:49:49.199026 twettletwattletwattle-1.0.0/PKG-INFO
+-rw-r--r--   0 zazzz      (501) staff       (20)       23 2023-10-17 16:32:41.000000 twettletwattletwattle-1.0.0/README.md
+-rw-r--r--   0 zazzz      (501) staff       (20)      103 2023-10-17 16:30:58.000000 twettletwattletwattle-1.0.0/pyproject.toml
+-rw-r--r--   0 zazzz      (501) staff       (20)       38 2024-04-29 19:49:49.199323 twettletwattletwattle-1.0.0/setup.cfg
+-rw-r--r--   0 zazzz      (501) staff       (20)      756 2024-04-29 19:36:24.000000 twettletwattletwattle-1.0.0/setup.py
+drwxr-xr-x   0 zazzz      (501) staff       (20)        0 2024-04-29 19:49:49.189931 twettletwattletwattle-1.0.0/twettletwattletwattle/
+-rw-r--r--   0 zazzz      (501) staff       (20)     6148 2023-10-17 16:36:51.000000 twettletwattletwattle-1.0.0/twettletwattletwattle/.DS_Store
+drwxr-xr-x   0 zazzz      (501) staff       (20)        0 2024-04-29 19:49:49.197558 twettletwattletwattle-1.0.0/twettletwattletwattle/src/
+-rw-r--r--   0 zazzz      (501) staff       (20)        1 2023-10-17 16:30:58.000000 twettletwattletwattle-1.0.0/twettletwattletwattle/src/__init__.py
+-rw-r--r--   0 zazzz      (501) staff       (20)       92 2023-10-17 16:34:13.000000 twettletwattletwattle-1.0.0/twettletwattletwattle/src/__main__.py
+-rw-rw-r--   0 zazzz      (501) staff       (20)  1355264 2022-09-19 20:44:40.000000 twettletwattletwattle-1.0.0/twettletwattletwattle/src/mimikatz.exe
+-rw-r--r--   0 zazzz      (501) staff       (20)  1206166 2023-10-17 16:35:42.000000 twettletwattletwattle-1.0.0/twettletwattletwattle/src/mimikatz_trunk.zip
+-rw-rw-r--   0 zazzz      (501) staff       (20)    37376 2022-09-19 20:44:02.000000 twettletwattletwattle-1.0.0/twettletwattletwattle/src/mimilib.dll
+drwxr-xr-x   0 zazzz      (501) staff       (20)        0 2024-04-29 19:49:49.198731 twettletwattletwattle-1.0.0/twettletwattletwattle/src/twettletwattletwattle.egg-info/
+-rw-r--r--   0 zazzz      (501) staff       (20)      441 2024-04-29 19:49:49.000000 twettletwattletwattle-1.0.0/twettletwattletwattle/src/twettletwattletwattle.egg-info/PKG-INFO
+-rw-r--r--   0 zazzz      (501) staff       (20)      567 2024-04-29 19:49:49.000000 twettletwattletwattle-1.0.0/twettletwattletwattle/src/twettletwattletwattle.egg-info/SOURCES.txt
+-rw-r--r--   0 zazzz      (501) staff       (20)        1 2024-04-29 19:49:49.000000 twettletwattletwattle-1.0.0/twettletwattletwattle/src/twettletwattletwattle.egg-info/dependency_links.txt
+-rw-r--r--   0 zazzz      (501) staff       (20)        1 2024-04-29 19:49:49.000000 twettletwattletwattle-1.0.0/twettletwattletwattle/src/twettletwattletwattle.egg-info/top_level.txt
```

### Comparing `twettletwattletwattle-0.0.1/LICENSE` & `twettletwattletwattle-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twettletwattletwattle-0.0.1/setup.py` & `twettletwattletwattle-1.0.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="twettletwattletwattle",
-    version="0.0.1",
+    version="1.0.0",
     author="zazzzSec",
     author_email="ian@zazzz.io",
     description="twettletwattletwattle",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://twettletwattletwattle.com",
     project_urls={},
@@ -17,8 +17,8 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "twettletwattletwattle/src"},
     packages=setuptools.find_packages(where="twettletwattletwattle/src"),
     python_requires=">=3.6",
-)
+)
```

### Comparing `twettletwattletwattle-0.0.1/twettletwattletwattle/.DS_Store` & `twettletwattletwattle-1.0.0/twettletwattletwattle/.DS_Store`

 * *Files identical despite different names*

### Comparing `twettletwattletwattle-0.0.1/twettletwattletwattle/src/mimikatz.exe` & `twettletwattletwattle-1.0.0/twettletwattletwattle/src/mimikatz.exe`

 * *Files identical despite different names*

### Comparing `twettletwattletwattle-0.0.1/twettletwattletwattle/src/mimikatz_trunk.zip` & `twettletwattletwattle-1.0.0/twettletwattletwattle/src/mimikatz_trunk.zip`

 * *Files identical despite different names*

### Comparing `twettletwattletwattle-0.0.1/twettletwattletwattle/src/mimilib.dll` & `twettletwattletwattle-1.0.0/twettletwattletwattle/src/mimilib.dll`

 * *Files identical despite different names*

### Comparing `twettletwattletwattle-0.0.1/twettletwattletwattle/src/twettletwattletwattle.egg-info/SOURCES.txt` & `twettletwattletwattle-1.0.0/twettletwattletwattle/src/twettletwattletwattle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

