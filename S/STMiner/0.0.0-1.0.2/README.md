# Comparing `tmp/STMiner-0.0.0.tar.gz` & `tmp/STMiner-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STMiner-0.0.0.tar", last modified: Mon Apr 29 07:44:47 2024, max compression
+gzip compressed data, was "STMiner-1.0.2.tar", last modified: Mon Apr 29 07:18:34 2024, max compression
```

## Comparing `STMiner-0.0.0.tar` & `STMiner-1.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 07:44:47.665679 STMiner-0.0.0/
--rw-rw-rw-   0        0        0     1088 2023-09-12 02:07:38.000000 STMiner-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     5391 2024-04-29 07:44:47.664680 STMiner-0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 07:44:47.634104 STMiner-0.0.0/STMiner/
-drwxrwxrwx   0        0        0        0 2024-04-29 07:44:47.649111 STMiner-0.0.0/STMiner/Algorithm/
--rw-rw-rw-   0        0        0      665 2024-02-02 08:39:01.000000 STMiner-0.0.0/STMiner/Algorithm/AlgUtils.py
--rw-rw-rw-   0        0        0        0 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/Algorithm/__init__.py
--rw-rw-rw-   0        0        0     2550 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/Algorithm/algorithm.py
--rw-rw-rw-   0        0        0     9040 2024-04-29 02:17:03.000000 STMiner-0.0.0/STMiner/Algorithm/distance.py
--rw-rw-rw-   0        0        0    13090 2023-11-07 08:45:02.000000 STMiner-0.0.0/STMiner/Algorithm/distribution.py
--rw-rw-rw-   0        0        0     1657 2024-04-29 02:17:03.000000 STMiner-0.0.0/STMiner/Algorithm/graph.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:44:47.650110 STMiner-0.0.0/STMiner/CustomApp/
--rw-rw-rw-   0        0        0     6009 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/CustomApp/App.py
--rw-rw-rw-   0        0        0        0 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/CustomApp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:44:47.652110 STMiner-0.0.0/STMiner/IO/
--rw-rw-rw-   0        0        0      350 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/IO/IOUtil.py
--rw-rw-rw-   0        0        0        0 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/IO/__init__.py
--rw-rw-rw-   0        0        0     1176 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/IO/read_h5ad.py
--rw-rw-rw-   0        0        0     6982 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/IO/read_stereo.py
--rw-rw-rw-   0        0        0      645 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/KEGGFinder.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:44:47.653110 STMiner-0.0.0/STMiner/Plot/
--rw-rw-rw-   0        0        0       22 2023-11-23 06:04:11.000000 STMiner-0.0.0/STMiner/Plot/__init__.py
--rw-rw-rw-   0        0        0    13672 2024-03-25 08:43:39.000000 STMiner-0.0.0/STMiner/Plot/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:44:47.655115 STMiner-0.0.0/STMiner/Preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 08:48:53.000000 STMiner-0.0.0/STMiner/Preprocess/__init__.py
--rw-rw-rw-   0        0        0      993 2023-11-05 14:36:29.000000 STMiner-0.0.0/STMiner/Preprocess/filter.py
--rw-rw-rw-   0        0        0      615 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/Preprocess/image.py
--rw-rw-rw-   0        0        0    13564 2024-04-29 02:17:03.000000 STMiner-0.0.0/STMiner/SPFinder.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:44:47.657115 STMiner-0.0.0/STMiner/Simulate/
--rw-rw-rw-   0        0        0     4214 2023-11-07 08:40:55.000000 STMiner-0.0.0/STMiner/Simulate/Simulate.py
--rw-rw-rw-   0        0        0       33 2023-11-23 06:02:42.000000 STMiner-0.0.0/STMiner/Simulate/__init__.py
--rw-rw-rw-   0        0        0     1061 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/Simulate/simUtils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:44:47.658116 STMiner-0.0.0/STMiner/Utils/
--rw-rw-rw-   0        0        0        0 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/Utils/__init__.py
--rw-rw-rw-   0        0        0     5708 2024-02-27 08:49:02.000000 STMiner-0.0.0/STMiner/Utils/utils.py
--rw-rw-rw-   0        0        0       32 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:44:47.663673 STMiner-0.0.0/STMiner/test/
--rw-rw-rw-   0        0        0     6461 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/test/SPFinderTester.py
--rw-rw-rw-   0        0        0        0 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/test/__init__.py
--rw-rw-rw-   0        0        0     1723 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/test/generate_mds_html.py
--rw-rw-rw-   0        0        0     1094 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/test/testUtils.py
--rw-rw-rw-   0        0        0      504 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/test/test_10x_data.py
--rw-rw-rw-   0        0        0     1948 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/test/test_hotspot.py
--rw-rw-rw-   0        0        0     1743 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/test/test_noise.py
--rw-rw-rw-   0        0        0      584 2023-11-05 11:48:31.000000 STMiner-0.0.0/STMiner/test/test_real_data.py
--rw-rw-rw-   0        0        0        0 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/test/test_stero_data.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:44:47.664680 STMiner-0.0.0/STMiner/unittest/
--rw-rw-rw-   0        0        0        0 2023-11-05 09:22:36.000000 STMiner-0.0.0/STMiner/unittest/__init__.py
--rw-rw-rw-   0        0        0       99 2023-11-05 09:22:45.000000 STMiner-0.0.0/STMiner/unittest/test_distribution.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:44:47.646110 STMiner-0.0.0/STMiner.egg-info/
--rw-rw-rw-   0        0        0     5391 2024-04-29 07:44:47.000000 STMiner-0.0.0/STMiner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2024-04-29 07:44:47.000000 STMiner-0.0.0/STMiner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 07:44:47.000000 STMiner-0.0.0/STMiner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      284 2024-04-29 07:44:47.000000 STMiner-0.0.0/STMiner.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-29 07:44:47.000000 STMiner-0.0.0/STMiner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 07:44:47.665679 STMiner-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1592 2024-04-29 07:44:44.000000 STMiner-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:18:34.599448 STMiner-1.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-09-12 02:07:38.000000 STMiner-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      404 2024-04-29 07:18:34.598449 STMiner-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 07:18:34.571894 STMiner-1.0.2/STMiner/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:18:34.583760 STMiner-1.0.2/STMiner/Algorithm/
+-rw-rw-rw-   0        0        0      665 2024-02-02 08:39:01.000000 STMiner-1.0.2/STMiner/Algorithm/AlgUtils.py
+-rw-rw-rw-   0        0        0        0 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/Algorithm/__init__.py
+-rw-rw-rw-   0        0        0     2550 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/Algorithm/algorithm.py
+-rw-rw-rw-   0        0        0     9040 2024-04-29 02:17:03.000000 STMiner-1.0.2/STMiner/Algorithm/distance.py
+-rw-rw-rw-   0        0        0    13090 2023-11-07 08:45:02.000000 STMiner-1.0.2/STMiner/Algorithm/distribution.py
+-rw-rw-rw-   0        0        0     1657 2024-04-29 02:17:03.000000 STMiner-1.0.2/STMiner/Algorithm/graph.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:18:34.585765 STMiner-1.0.2/STMiner/CustomApp/
+-rw-rw-rw-   0        0        0     6009 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/CustomApp/App.py
+-rw-rw-rw-   0        0        0        0 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/CustomApp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:18:34.586792 STMiner-1.0.2/STMiner/IO/
+-rw-rw-rw-   0        0        0      350 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/IO/IOUtil.py
+-rw-rw-rw-   0        0        0        0 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/IO/__init__.py
+-rw-rw-rw-   0        0        0     1176 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/IO/read_h5ad.py
+-rw-rw-rw-   0        0        0     6982 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/IO/read_stereo.py
+-rw-rw-rw-   0        0        0      645 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/KEGGFinder.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:18:34.588176 STMiner-1.0.2/STMiner/Plot/
+-rw-rw-rw-   0        0        0       22 2023-11-23 06:04:11.000000 STMiner-1.0.2/STMiner/Plot/__init__.py
+-rw-rw-rw-   0        0        0    13672 2024-03-25 08:43:39.000000 STMiner-1.0.2/STMiner/Plot/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:18:34.590190 STMiner-1.0.2/STMiner/Preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 08:48:53.000000 STMiner-1.0.2/STMiner/Preprocess/__init__.py
+-rw-rw-rw-   0        0        0      993 2023-11-05 14:36:29.000000 STMiner-1.0.2/STMiner/Preprocess/filter.py
+-rw-rw-rw-   0        0        0      615 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/Preprocess/image.py
+-rw-rw-rw-   0        0        0    13564 2024-04-29 02:17:03.000000 STMiner-1.0.2/STMiner/SPFinder.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:18:34.591489 STMiner-1.0.2/STMiner/Simulate/
+-rw-rw-rw-   0        0        0     4214 2023-11-07 08:40:55.000000 STMiner-1.0.2/STMiner/Simulate/Simulate.py
+-rw-rw-rw-   0        0        0       33 2023-11-23 06:02:42.000000 STMiner-1.0.2/STMiner/Simulate/__init__.py
+-rw-rw-rw-   0        0        0     1061 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/Simulate/simUtils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:18:34.592921 STMiner-1.0.2/STMiner/Utils/
+-rw-rw-rw-   0        0        0        0 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/Utils/__init__.py
+-rw-rw-rw-   0        0        0     5708 2024-02-27 08:49:02.000000 STMiner-1.0.2/STMiner/Utils/utils.py
+-rw-rw-rw-   0        0        0       32 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:18:34.597449 STMiner-1.0.2/STMiner/test/
+-rw-rw-rw-   0        0        0     6461 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/test/SPFinderTester.py
+-rw-rw-rw-   0        0        0        0 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/test/__init__.py
+-rw-rw-rw-   0        0        0     1723 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/test/generate_mds_html.py
+-rw-rw-rw-   0        0        0     1094 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/test/testUtils.py
+-rw-rw-rw-   0        0        0      504 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/test/test_10x_data.py
+-rw-rw-rw-   0        0        0     1948 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/test/test_hotspot.py
+-rw-rw-rw-   0        0        0     1743 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/test/test_noise.py
+-rw-rw-rw-   0        0        0      584 2023-11-05 11:48:31.000000 STMiner-1.0.2/STMiner/test/test_real_data.py
+-rw-rw-rw-   0        0        0        0 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/test/test_stero_data.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:18:34.598449 STMiner-1.0.2/STMiner/unittest/
+-rw-rw-rw-   0        0        0        0 2023-11-05 09:22:36.000000 STMiner-1.0.2/STMiner/unittest/__init__.py
+-rw-rw-rw-   0        0        0       99 2023-11-05 09:22:45.000000 STMiner-1.0.2/STMiner/unittest/test_distribution.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:18:34.581651 STMiner-1.0.2/STMiner.egg-info/
+-rw-rw-rw-   0        0        0      404 2024-04-29 07:18:34.000000 STMiner-1.0.2/STMiner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1165 2024-04-29 07:18:34.000000 STMiner-1.0.2/STMiner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 07:18:34.000000 STMiner-1.0.2/STMiner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      284 2024-04-29 07:18:34.000000 STMiner-1.0.2/STMiner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-29 07:18:34.000000 STMiner-1.0.2/STMiner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 07:18:34.599448 STMiner-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1312 2024-04-29 07:18:24.000000 STMiner-1.0.2/setup.py
```

### Comparing `STMiner-0.0.0/LICENSE` & `STMiner-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/Algorithm/AlgUtils.py` & `STMiner-1.0.2/STMiner/Algorithm/AlgUtils.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/Algorithm/algorithm.py` & `STMiner-1.0.2/STMiner/Algorithm/algorithm.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/Algorithm/distance.py` & `STMiner-1.0.2/STMiner/Algorithm/distance.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/Algorithm/distribution.py` & `STMiner-1.0.2/STMiner/Algorithm/distribution.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/Algorithm/graph.py` & `STMiner-1.0.2/STMiner/Algorithm/graph.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/CustomApp/App.py` & `STMiner-1.0.2/STMiner/CustomApp/App.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/IO/read_h5ad.py` & `STMiner-1.0.2/STMiner/IO/read_h5ad.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/IO/read_stereo.py` & `STMiner-1.0.2/STMiner/IO/read_stereo.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/KEGGFinder.py` & `STMiner-1.0.2/STMiner/KEGGFinder.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/Plot/plot.py` & `STMiner-1.0.2/STMiner/Plot/plot.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/Preprocess/filter.py` & `STMiner-1.0.2/STMiner/Preprocess/filter.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/Preprocess/image.py` & `STMiner-1.0.2/STMiner/Preprocess/image.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/SPFinder.py` & `STMiner-1.0.2/STMiner/SPFinder.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/Simulate/Simulate.py` & `STMiner-1.0.2/STMiner/Simulate/Simulate.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/Simulate/simUtils.py` & `STMiner-1.0.2/STMiner/Simulate/simUtils.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/Utils/utils.py` & `STMiner-1.0.2/STMiner/Utils/utils.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/test/SPFinderTester.py` & `STMiner-1.0.2/STMiner/test/SPFinderTester.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/test/generate_mds_html.py` & `STMiner-1.0.2/STMiner/test/generate_mds_html.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/test/testUtils.py` & `STMiner-1.0.2/STMiner/test/testUtils.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/test/test_hotspot.py` & `STMiner-1.0.2/STMiner/test/test_hotspot.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/test/test_noise.py` & `STMiner-1.0.2/STMiner/test/test_noise.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner/test/test_real_data.py` & `STMiner-1.0.2/STMiner/test/test_real_data.py`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/STMiner.egg-info/SOURCES.txt` & `STMiner-1.0.2/STMiner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `STMiner-0.0.0/setup.py` & `STMiner-1.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 from setuptools import setup, find_packages
-from os import path
-
-
-this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
 
 setup(
     name='STMiner',
-    version='0.0.0',
+    version='1.0.2',
     author='Peisen Sun',
     url='https://github.com/PSSUN/STMiner',
     license='MIT License',
     description='Python package for spatial transcriptomics data analysis',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
     author_email='sunpeisen@stu.xjtu.edu.cn',
     packages=find_packages(),
     platforms=['Linux', 'Mac', 'Windows'],
     keywords=['STMiner',
               'bioinformatics',
               'GMM',
               'hellinger distance',
```

