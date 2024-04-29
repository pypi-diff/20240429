# Comparing `tmp/deepgpu-2.1.0rc3.tar.gz` & `tmp/deepgpu-2.1.0rc3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepgpu-2.1.0rc3.tar", last modified: Mon Apr 29 08:43:15 2024, max compression
+gzip compressed data, was "deepgpu-2.1.0rc3.post1.tar", last modified: Mon Apr 29 09:08:41 2024, max compression
```

## Comparing `deepgpu-2.1.0rc3.tar` & `deepgpu-2.1.0rc3.post1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-29 08:43:15.812187 deepgpu-2.1.0rc3/
--rw-r--r--   0 du         (502) staff       (20)       30 2023-10-10 07:39:14.000000 deepgpu-2.1.0rc3/MANIFEST.in
--rw-r--r--   0 du         (502) staff       (20)      615 2024-04-29 08:43:15.811763 deepgpu-2.1.0rc3/PKG-INFO
--rw-r--r--   0 du         (502) staff       (20)      292 2024-04-26 09:23:15.000000 deepgpu-2.1.0rc3/README.md
-drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-29 08:43:15.810182 deepgpu-2.1.0rc3/deepgpu/
--rw-r--r--   0 du         (502) staff       (20)       17 2023-10-09 07:10:39.000000 deepgpu-2.1.0rc3/deepgpu/__init__.py
-drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-29 08:43:15.811410 deepgpu-2.1.0rc3/deepgpu.egg-info/
--rw-r--r--   0 du         (502) staff       (20)      615 2024-04-29 08:43:15.000000 deepgpu-2.1.0rc3/deepgpu.egg-info/PKG-INFO
--rw-r--r--   0 du         (502) staff       (20)      196 2024-04-29 08:43:15.000000 deepgpu-2.1.0rc3/deepgpu.egg-info/SOURCES.txt
--rw-r--r--   0 du         (502) staff       (20)        1 2024-04-29 08:43:15.000000 deepgpu-2.1.0rc3/deepgpu.egg-info/dependency_links.txt
--rw-r--r--   0 du         (502) staff       (20)        8 2024-04-29 08:43:15.000000 deepgpu-2.1.0rc3/deepgpu.egg-info/top_level.txt
--rw-r--r--   0 du         (502) staff       (20)       38 2024-04-29 08:43:15.812251 deepgpu-2.1.0rc3/setup.cfg
--rw-r--r--   0 du         (502) staff       (20)     6789 2024-04-29 08:41:02.000000 deepgpu-2.1.0rc3/setup.py
+drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-29 09:08:41.852810 deepgpu-2.1.0rc3.post1/
+-rw-r--r--   0 du         (502) staff       (20)       30 2023-10-10 07:39:14.000000 deepgpu-2.1.0rc3.post1/MANIFEST.in
+-rw-r--r--   0 du         (502) staff       (20)      621 2024-04-29 09:08:41.851981 deepgpu-2.1.0rc3.post1/PKG-INFO
+-rw-r--r--   0 du         (502) staff       (20)      292 2024-04-26 09:23:15.000000 deepgpu-2.1.0rc3.post1/README.md
+drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-29 09:08:41.850448 deepgpu-2.1.0rc3.post1/deepgpu/
+-rw-r--r--   0 du         (502) staff       (20)       17 2023-10-09 07:10:39.000000 deepgpu-2.1.0rc3.post1/deepgpu/__init__.py
+drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-29 09:08:41.851634 deepgpu-2.1.0rc3.post1/deepgpu.egg-info/
+-rw-r--r--   0 du         (502) staff       (20)      621 2024-04-29 09:08:41.000000 deepgpu-2.1.0rc3.post1/deepgpu.egg-info/PKG-INFO
+-rw-r--r--   0 du         (502) staff       (20)      196 2024-04-29 09:08:41.000000 deepgpu-2.1.0rc3.post1/deepgpu.egg-info/SOURCES.txt
+-rw-r--r--   0 du         (502) staff       (20)        1 2024-04-29 09:08:41.000000 deepgpu-2.1.0rc3.post1/deepgpu.egg-info/dependency_links.txt
+-rw-r--r--   0 du         (502) staff       (20)        8 2024-04-29 09:08:41.000000 deepgpu-2.1.0rc3.post1/deepgpu.egg-info/top_level.txt
+-rw-r--r--   0 du         (502) staff       (20)       38 2024-04-29 09:08:41.852889 deepgpu-2.1.0rc3.post1/setup.cfg
+-rw-r--r--   0 du         (502) staff       (20)     6831 2024-04-29 09:08:27.000000 deepgpu-2.1.0rc3.post1/setup.py
```

### Comparing `deepgpu-2.1.0rc3/setup.py` & `deepgpu-2.1.0rc3.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import subprocess
 from setuptools.command.install import install
 import os
 
 NAME="deepgpu"
 DEEPGPU_VERSION = "2.1.0rc3"
 DEEPYTORCH_PKG_VERSION = DEEPGPU_VERSION # same as DEEPGPU version so far
-
+DEEPGPU_VERSION = "2.1.0rc3.post1"
 support_os_list = ['ubuntu', 'centos', 'alinux'] # add version later
 support_pytorch_version = ['1.10', '1.11', '1.12', '1.13', '2.0', '2.1']
-support_cuda_version = ['11.1', '11.3', '11.6', '11.7', '11.8', '12.1']
+support_cuda_version = ['11.1', '11.3', '11.6', '11.7', '11.8', '12.1', '12.3']
 support_python_version = ['38', '39', '310', '311']
 
 _root_path_deepgpu = "https://mirrors.aliyun.com/deepgpu/"
 _root_path_deepytorch = f"{_root_path_deepgpu}/deepytorch/{DEEPYTORCH_PKG_VERSION}/"
 _temp_path = f"{os.environ['HOME']}/.deepgpu/"
 _temp_log = f"{_temp_path}/log"
```

