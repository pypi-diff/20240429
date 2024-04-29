# Comparing `tmp/csulb_dataset-0.1.4.tar.gz` & `tmp/csulb_dataset-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csulb_dataset-0.1.4.tar", last modified: Mon Apr 29 21:47:55 2024, max compression
+gzip compressed data, was "csulb_dataset-0.1.5.tar", last modified: Mon Apr 29 21:54:37 2024, max compression
```

## Comparing `csulb_dataset-0.1.4.tar` & `csulb_dataset-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 guru       (501) staff       (20)        0 2024-04-29 21:47:55.927303 csulb_dataset-0.1.4/
--rw-r--r--   0 guru       (501) staff       (20)      256 2024-04-29 21:47:55.927173 csulb_dataset-0.1.4/PKG-INFO
--rw-r--r--   0 guru       (501) staff       (20)       16 2024-04-29 20:09:04.000000 csulb_dataset-0.1.4/README.md
-drwxr-xr-x   0 guru       (501) staff       (20)        0 2024-04-29 21:47:55.926433 csulb_dataset-0.1.4/csulb_dataset.egg-info/
--rw-r--r--   0 guru       (501) staff       (20)      256 2024-04-29 21:47:55.000000 csulb_dataset-0.1.4/csulb_dataset.egg-info/PKG-INFO
--rw-r--r--   0 guru       (501) staff       (20)      260 2024-04-29 21:47:55.000000 csulb_dataset-0.1.4/csulb_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 guru       (501) staff       (20)        1 2024-04-29 21:47:55.000000 csulb_dataset-0.1.4/csulb_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 guru       (501) staff       (20)        7 2024-04-29 21:47:55.000000 csulb_dataset-0.1.4/csulb_dataset.egg-info/requires.txt
--rw-r--r--   0 guru       (501) staff       (20)       19 2024-04-29 21:47:55.000000 csulb_dataset-0.1.4/csulb_dataset.egg-info/top_level.txt
-drwxr-xr-x   0 guru       (501) staff       (20)        0 2024-04-29 21:47:55.926872 csulb_dataset-0.1.4/csulb_mock_dataset/
--rw-r--r--   0 guru       (501) staff       (20)       28 2024-04-29 21:16:45.000000 csulb_dataset-0.1.4/csulb_mock_dataset/__init__.py
--rw-r--r--   0 guru       (501) staff       (20)      270 2024-04-29 21:19:26.000000 csulb_dataset-0.1.4/csulb_mock_dataset/data.py
--rw-r--r--   0 guru       (501) staff       (20)       38 2024-04-29 21:47:55.927355 csulb_dataset-0.1.4/setup.cfg
--rw-r--r--   0 guru       (501) staff       (20)      629 2024-04-29 21:47:48.000000 csulb_dataset-0.1.4/setup.py
+drwxr-xr-x   0 guru       (501) staff       (20)        0 2024-04-29 21:54:37.449241 csulb_dataset-0.1.5/
+-rw-r--r--   0 guru       (501) staff       (20)      256 2024-04-29 21:54:37.449145 csulb_dataset-0.1.5/PKG-INFO
+-rw-r--r--   0 guru       (501) staff       (20)       16 2024-04-29 20:09:04.000000 csulb_dataset-0.1.5/README.md
+drwxr-xr-x   0 guru       (501) staff       (20)        0 2024-04-29 21:54:37.448577 csulb_dataset-0.1.5/csulb_dataset.egg-info/
+-rw-r--r--   0 guru       (501) staff       (20)      256 2024-04-29 21:54:37.000000 csulb_dataset-0.1.5/csulb_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 guru       (501) staff       (20)      260 2024-04-29 21:54:37.000000 csulb_dataset-0.1.5/csulb_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 guru       (501) staff       (20)        1 2024-04-29 21:54:37.000000 csulb_dataset-0.1.5/csulb_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 guru       (501) staff       (20)        7 2024-04-29 21:54:37.000000 csulb_dataset-0.1.5/csulb_dataset.egg-info/requires.txt
+-rw-r--r--   0 guru       (501) staff       (20)       19 2024-04-29 21:54:37.000000 csulb_dataset-0.1.5/csulb_dataset.egg-info/top_level.txt
+drwxr-xr-x   0 guru       (501) staff       (20)        0 2024-04-29 21:54:37.448904 csulb_dataset-0.1.5/csulb_mock_dataset/
+-rw-r--r--   0 guru       (501) staff       (20)       28 2024-04-29 21:16:45.000000 csulb_dataset-0.1.5/csulb_mock_dataset/__init__.py
+-rw-r--r--   0 guru       (501) staff       (20)      268 2024-04-29 21:54:21.000000 csulb_dataset-0.1.5/csulb_mock_dataset/data.py
+-rw-r--r--   0 guru       (501) staff       (20)       38 2024-04-29 21:54:37.449276 csulb_dataset-0.1.5/setup.cfg
+-rw-r--r--   0 guru       (501) staff       (20)      629 2024-04-29 21:54:33.000000 csulb_dataset-0.1.5/setup.py
```

### Comparing `csulb_dataset-0.1.4/setup.py` & `csulb_dataset-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='csulb_dataset',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     include_package_data=True,
     package_data={
         '': ['data/*.csv'],  # Ensure this matches the path to your CSV files
     },
     install_requires=[
         'pandas',  # Ensure pandas is installed with your package
```

