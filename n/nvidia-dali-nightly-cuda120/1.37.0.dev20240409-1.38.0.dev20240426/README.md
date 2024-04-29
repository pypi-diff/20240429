# Comparing `tmp/nvidia_dali_nightly_cuda120-1.37.0.dev20240409.tar.gz` & `tmp/nvidia_dali_nightly_cuda120-1.38.0.dev20240426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia_dali_nightly_cuda120-1.37.0.dev20240409.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "nvidia_dali_nightly_cuda120-1.38.0.dev20240426.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvidia_dali_nightly_cuda120-1.37.0.dev20240409.tar` & `nvidia_dali_nightly_cuda120-1.38.0.dev20240426.tar`

### file list

```diff
@@ -1,2 +1,2 @@
 -rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
--rw-r--r--   0        0        0     2451 1993-04-05 07:00:00.000000 PKG-INFO
+-rw-r--r--   0        0        0     2397 1993-04-05 07:00:00.000000 PKG-INFO
```

### PKG-INFO

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda120
-Version: 1.37.0.dev20240409
-Summary: NVIDIA DALI nightly  for CUDA 12.0. Git SHA: fb5786c82c162af3f2120e8ab8cbb8d5d5cdbf12
+Version: 1.38.0.dev20240426
+Summary: NVIDIA DALI nightly  for CUDA 12.0. Git SHA: 15f591232e2d068a76f1658ac7e3ea28b5622822
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -37,16 +37,15 @@
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

