# Comparing `tmp/numpy6-0.1.tar.gz` & `tmp/numpy6-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpy6-0.1.tar", last modified: Sun Apr 28 19:56:09 2024, max compression
+gzip compressed data, was "numpy6-0.2.tar", last modified: Mon Apr 29 01:32:22 2024, max compression
```

## Comparing `numpy6-0.1.tar` & `numpy6-0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:56:09.003222 numpy6-0.1/
--rw-r--r--   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:26:50.000000 numpy6-0.1/LICENSE
--rw-r--r--   0 sainath   (1000) sainath   (1000)       70 2024-04-28 19:56:09.003222 numpy6-0.1/PKG-INFO
--rw-r--r--   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:26:50.000000 numpy6-0.1/README.md
-drwxr-xr-x   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:56:09.002222 numpy6-0.1/numpy6/
--rw-r--r--   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:46:39.000000 numpy6-0.1/numpy6/__init__.py
--rw-r--r--   0 sainath   (1000) sainath   (1000)     1070 2024-04-28 19:31:36.000000 numpy6-0.1/numpy6/cnn.py
--rw-r--r--   0 sainath   (1000) sainath   (1000)      562 2024-04-28 19:31:36.000000 numpy6-0.1/numpy6/mcculloch.py
--rw-r--r--   0 sainath   (1000) sainath   (1000)      985 2024-04-28 19:31:36.000000 numpy6-0.1/numpy6/perceptron.py
-drwxr-xr-x   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:56:09.003222 numpy6-0.1/numpy6.egg-info/
--rw-r--r--   0 sainath   (1000) sainath   (1000)       70 2024-04-28 19:56:08.000000 numpy6-0.1/numpy6.egg-info/PKG-INFO
--rw-r--r--   0 sainath   (1000) sainath   (1000)      220 2024-04-28 19:56:08.000000 numpy6-0.1/numpy6.egg-info/SOURCES.txt
--rw-r--r--   0 sainath   (1000) sainath   (1000)        1 2024-04-28 19:56:08.000000 numpy6-0.1/numpy6.egg-info/dependency_links.txt
--rw-r--r--   0 sainath   (1000) sainath   (1000)        7 2024-04-28 19:56:08.000000 numpy6-0.1/numpy6.egg-info/top_level.txt
--rw-r--r--   0 sainath   (1000) sainath   (1000)       38 2024-04-28 19:56:09.003222 numpy6-0.1/setup.cfg
--rw-r--r--   0 sainath   (1000) sainath   (1000)      153 2024-04-28 19:56:06.000000 numpy6-0.1/setup.py
+drwxr-xr-x   0 sainath   (1000) sainath   (1000)        0 2024-04-29 01:32:22.516370 numpy6-0.2/
+-rw-r--r--   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:26:50.000000 numpy6-0.2/LICENSE
+-rw-r--r--   0 sainath   (1000) sainath   (1000)       70 2024-04-29 01:32:22.516370 numpy6-0.2/PKG-INFO
+-rw-r--r--   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:26:50.000000 numpy6-0.2/README.md
+drwxr-xr-x   0 sainath   (1000) sainath   (1000)        0 2024-04-29 01:32:22.515370 numpy6-0.2/numpy6/
+-rw-r--r--   0 sainath   (1000) sainath   (1000)        0 2024-04-28 19:46:39.000000 numpy6-0.2/numpy6/__init__.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1577 2024-04-29 01:07:07.000000 numpy6-0.2/numpy6/autoencoder.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1070 2024-04-29 01:07:07.000000 numpy6-0.2/numpy6/cnn.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1149 2024-04-29 01:07:07.000000 numpy6-0.2/numpy6/lstm.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)      562 2024-04-29 01:07:07.000000 numpy6-0.2/numpy6/mcculloch.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)      985 2024-04-29 01:07:07.000000 numpy6-0.2/numpy6/perceptron.py
+-rw-r--r--   0 sainath   (1000) sainath   (1000)     1157 2024-04-29 01:07:07.000000 numpy6-0.2/numpy6/rnn.py
+drwxr-xr-x   0 sainath   (1000) sainath   (1000)        0 2024-04-29 01:32:22.515370 numpy6-0.2/numpy6.egg-info/
+-rw-r--r--   0 sainath   (1000) sainath   (1000)       70 2024-04-29 01:32:22.000000 numpy6-0.2/numpy6.egg-info/PKG-INFO
+-rw-r--r--   0 sainath   (1000) sainath   (1000)      271 2024-04-29 01:32:22.000000 numpy6-0.2/numpy6.egg-info/SOURCES.txt
+-rw-r--r--   0 sainath   (1000) sainath   (1000)        1 2024-04-29 01:32:22.000000 numpy6-0.2/numpy6.egg-info/dependency_links.txt
+-rw-r--r--   0 sainath   (1000) sainath   (1000)        7 2024-04-29 01:32:22.000000 numpy6-0.2/numpy6.egg-info/top_level.txt
+-rw-r--r--   0 sainath   (1000) sainath   (1000)       38 2024-04-29 01:32:22.516370 numpy6-0.2/setup.cfg
+-rw-r--r--   0 sainath   (1000) sainath   (1000)      153 2024-04-29 01:32:21.000000 numpy6-0.2/setup.py
```

### Comparing `numpy6-0.1/numpy6/cnn.py` & `numpy6-0.2/numpy6/cnn.py`

 * *Files identical despite different names*

### Comparing `numpy6-0.1/numpy6/mcculloch.py` & `numpy6-0.2/numpy6/mcculloch.py`

 * *Files identical despite different names*

### Comparing `numpy6-0.1/numpy6/perceptron.py` & `numpy6-0.2/numpy6/perceptron.py`

 * *Files identical despite different names*

