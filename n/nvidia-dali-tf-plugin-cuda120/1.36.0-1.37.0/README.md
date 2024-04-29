# Comparing `tmp/nvidia_dali_tf_plugin_cuda120-1.36.0.tar.gz` & `tmp/nvidia_dali_tf_plugin_cuda120-1.37.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia_dali_tf_plugin_cuda120-1.36.0.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "nvidia_dali_tf_plugin_cuda120-1.37.0.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvidia_dali_tf_plugin_cuda120-1.36.0.tar` & `nvidia_dali_tf_plugin_cuda120-1.37.0.tar`

### file list

```diff
@@ -1,2 +1,2 @@
 -rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
--rw-r--r--   0        0        0     2446 1993-04-05 07:00:00.000000 PKG-INFO
+-rw-r--r--   0        0        0     2374 1993-04-05 07:00:00.000000 PKG-INFO
```

### PKG-INFO

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-cuda120
-Version: 1.36.0
-Summary: NVIDIA DALI  TensorFlow plugin for CUDA 12.0. Git SHA: e2ae685702638e3f8fae8091344f0f7ea045a1f9
+Version: 1.37.0
+Summary: NVIDIA DALI  TensorFlow plugin for CUDA 12.0. Git SHA: 1bc7fc20b0ff373a3320eca0c7f4860feb4a3bd2
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <3.13
 Description-Content-Type: text/x-rst
@@ -36,18 +35,17 @@
 are handled transparently for the user.
 
 In addition, the deep learning frameworks have multiple data pre-processing implementations,
 resulting in challenges such as portability of training and inference workflows, and code
 maintainability. Data processing pipelines implemented using DALI are portable because they
 can easily be retargeted to TensorFlow, PyTorch, MXNet and PaddlePaddle.
 
-For more details please check the |release-doc|_.
+For more details please check the
+`latest DALI Documentation <https://docs.nvidia.com/deeplearning/dali/user-guide/docs/index.html>`_.
 
 .. image:: https://raw.githubusercontent.com/NVIDIA/DALI/main/dali.png
     :width: 800
     :align: center
     :alt: DALI Diagram
 
-.. |release-doc| replace:: latest DALI Documentation
-.. _release-doc: https://docs.nvidia.com/deeplearning/dali/user-guide/docs/index.html
```

