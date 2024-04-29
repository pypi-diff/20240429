# Comparing `tmp/numpy6-0.2.tar.gz` & `tmp/numpy6-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpy6-0.2.tar", last modified: Mon Apr 29 01:32:22 2024, max compression
+gzip compressed data, was "numpy6-0.3.tar", last modified: Mon Apr 29 01:35:05 2024, max compression
```

## Comparing `numpy6-0.2.tar` & `numpy6-0.3.tar`

### file list

```diff
@@ -1,19 +1,29 @@
-drwxr-xr-x   0 sainath   (1000) sainath   (1000)        0 2024-04-29 01:32:22.516370 numpy6-0.2/
--rw-r--r--   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:26:50.000000 numpy6-0.2/LICENSE
--rw-r--r--   0 sainath   (1000) sainath   (1000)       70 2024-04-29 01:32:22.516370 numpy6-0.2/PKG-INFO
--rw-r--r--   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:26:50.000000 numpy6-0.2/README.md
-drwxr-xr-x   0 sainath   (1000) sainath   (1000)        0 2024-04-29 01:32:22.515370 numpy6-0.2/numpy6/
--rw-r--r--   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:46:39.000000 numpy6-0.2/numpy6/__init__.py
--rw-r--r--   0 sainath   (1000) sainath   (1000)     1577 2024-04-29 01:07:07.000000 numpy6-0.2/numpy6/autoencoder.py
--rw-r--r--   0 sainath   (1000) sainath   (1000)     1070 2024-04-29 01:07:07.000000 numpy6-0.2/numpy6/cnn.py
--rw-r--r--   0 sainath   (1000) sainath   (1000)     1149 2024-04-29 01:07:07.000000 numpy6-0.2/numpy6/lstm.py
--rw-r--r--   0 sainath   (1000) sainath   (1000)      562 2024-04-29 01:07:07.000000 numpy6-0.2/numpy6/mcculloch.py
--rw-r--r--   0 sainath   (1000) sainath   (1000)      985 2024-04-29 01:07:07.000000 numpy6-0.2/numpy6/perceptron.py
--rw-r--r--   0 sainath   (1000) sainath   (1000)     1157 2024-04-29 01:07:07.000000 numpy6-0.2/numpy6/rnn.py
-drwxr-xr-x   0 sainath   (1000) sainath   (1000)        0 2024-04-29 01:32:22.515370 numpy6-0.2/numpy6.egg-info/
--rw-r--r--   0 sainath   (1000) sainath   (1000)       70 2024-04-29 01:32:22.000000 numpy6-0.2/numpy6.egg-info/PKG-INFO
--rw-r--r--   0 sainath   (1000) sainath   (1000)      271 2024-04-29 01:32:22.000000 numpy6-0.2/numpy6.egg-info/SOURCES.txt
--rw-r--r--   0 sainath   (1000) sainath   (1000)        1 2024-04-29 01:32:22.000000 numpy6-0.2/numpy6.egg-info/dependency_links.txt
--rw-r--r--   0 sainath   (1000) sainath   (1000)        7 2024-04-29 01:32:22.000000 numpy6-0.2/numpy6.egg-info/top_level.txt
--rw-r--r--   0 sainath   (1000) sainath   (1000)       38 2024-04-29 01:32:22.516370 numpy6-0.2/setup.cfg
--rw-r--r--   0 sainath   (1000) sainath   (1000)      153 2024-04-29 01:32:21.000000 numpy6-0.2/setup.py
+drwxr-xr-x   0 sainath   (1000) sainath   (1000)        0 2024-04-29 01:35:05.899673 numpy6-0.3/
+-rw-r--r--   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:26:50.000000 numpy6-0.3/LICENSE
+-rw-r--r--   0 sainath   (1000) sainath   (1000)       70 2024-04-29 01:35:05.898673 numpy6-0.3/PKG-INFO
+-rw-r--r--   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:26:50.000000 numpy6-0.3/README.md
+drwxr-xr-x   0 sainath   (1000) sainath   (1000)        0 2024-04-29 01:35:05.896673 numpy6-0.3/numpy6/
+-rw-r--r--   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:46:39.000000 numpy6-0.3/numpy6/__init__.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1577 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/autoencoder.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1070 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/cnn.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1149 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/lstm.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)      562 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/mcculloch.py
+drwxr-xr-x   0 sainath   (1000) sainath   (1000)        0 2024-04-29 01:35:05.898673 numpy6-0.3/numpy6/optimization/
+-rw-r--r--   0 sainath   (1000) sainath   (1000)        0 2024-04-29 01:34:49.000000 numpy6-0.3/numpy6/optimization/__init__.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1215 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/optimization/adagradGD.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1510 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/optimization/adamGD.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1261 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/optimization/minibatchGD.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1278 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/optimization/momentumGD.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1351 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/optimization/nesterovGD.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1248 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/optimization/rmsGD.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1278 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/optimization/stocasticGD.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1161 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/optimization/vanilaGD.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)      985 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/perceptron.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1157 2024-04-29 01:07:07.000000 numpy6-0.3/numpy6/rnn.py
+drwxr-xr-x   0 sainath   (1000) sainath   (1000)        0 2024-04-29 01:35:05.898673 numpy6-0.3/numpy6.egg-info/
+-rw-r--r--   0 sainath   (1000) sainath   (1000)       70 2024-04-29 01:35:05.000000 numpy6-0.3/numpy6.egg-info/PKG-INFO
+-rw-r--r--   0 sainath   (1000) sainath   (1000)      565 2024-04-29 01:35:05.000000 numpy6-0.3/numpy6.egg-info/SOURCES.txt
+-rw-r--r--   0 sainath   (1000) sainath   (1000)        1 2024-04-29 01:35:05.000000 numpy6-0.3/numpy6.egg-info/dependency_links.txt
+-rw-r--r--   0 sainath   (1000) sainath   (1000)        7 2024-04-29 01:35:05.000000 numpy6-0.3/numpy6.egg-info/top_level.txt
+-rw-r--r--   0 sainath   (1000) sainath   (1000)       38 2024-04-29 01:35:05.899673 numpy6-0.3/setup.cfg
+-rw-r--r--   0 sainath   (1000) sainath   (1000)      153 2024-04-29 01:35:03.000000 numpy6-0.3/setup.py
```

### Comparing `numpy6-0.2/numpy6/autoencoder.py` & `numpy6-0.3/numpy6/autoencoder.py`

 * *Files identical despite different names*

### Comparing `numpy6-0.2/numpy6/cnn.py` & `numpy6-0.3/numpy6/cnn.py`

 * *Files identical despite different names*

### Comparing `numpy6-0.2/numpy6/lstm.py` & `numpy6-0.3/numpy6/lstm.py`

 * *Files identical despite different names*

### Comparing `numpy6-0.2/numpy6/mcculloch.py` & `numpy6-0.3/numpy6/mcculloch.py`

 * *Files identical despite different names*

### Comparing `numpy6-0.2/numpy6/perceptron.py` & `numpy6-0.3/numpy6/perceptron.py`

 * *Files identical despite different names*

### Comparing `numpy6-0.2/numpy6/rnn.py` & `numpy6-0.3/numpy6/rnn.py`

 * *Files identical despite different names*
