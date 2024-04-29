# Comparing `tmp/deepgpu-2.1.0rc2.tar.gz` & `tmp/deepgpu-2.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepgpu-2.1.0rc2.tar", last modified: Mon Apr 15 03:31:24 2024, max compression
+gzip compressed data, was "deepgpu-2.1.0rc3.tar", last modified: Mon Apr 29 08:43:15 2024, max compression
```

## Comparing `deepgpu-2.1.0rc2.tar` & `deepgpu-2.1.0rc3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:31:24.255031 deepgpu-2.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)       30 2024-03-15 02:47:11.000000 deepgpu-2.1.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      615 2024-04-15 03:31:24.241978 deepgpu-2.1.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      292 2024-04-15 01:48:58.000000 deepgpu-2.1.0rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:31:24.145225 deepgpu-2.1.0rc2/deepgpu/
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-15 02:47:11.000000 deepgpu-2.1.0rc2/deepgpu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:31:24.222051 deepgpu-2.1.0rc2/deepgpu.egg-info/
--rw-r--r--   0 root         (0) root         (0)      615 2024-04-15 03:31:23.000000 deepgpu-2.1.0rc2/deepgpu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      196 2024-04-15 03:31:24.000000 deepgpu-2.1.0rc2/deepgpu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 03:31:23.000000 deepgpu-2.1.0rc2/deepgpu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-15 03:31:23.000000 deepgpu-2.1.0rc2/deepgpu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 03:31:24.257985 deepgpu-2.1.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6624 2024-04-15 02:44:57.000000 deepgpu-2.1.0rc2/setup.py
+drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-29 08:43:15.812187 deepgpu-2.1.0rc3/
+-rw-r--r--   0 du         (502) staff       (20)       30 2023-10-10 07:39:14.000000 deepgpu-2.1.0rc3/MANIFEST.in
+-rw-r--r--   0 du         (502) staff       (20)      615 2024-04-29 08:43:15.811763 deepgpu-2.1.0rc3/PKG-INFO
+-rw-r--r--   0 du         (502) staff       (20)      292 2024-04-26 09:23:15.000000 deepgpu-2.1.0rc3/README.md
+drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-29 08:43:15.810182 deepgpu-2.1.0rc3/deepgpu/
+-rw-r--r--   0 du         (502) staff       (20)       17 2023-10-09 07:10:39.000000 deepgpu-2.1.0rc3/deepgpu/__init__.py
+drwxr-xr-x   0 du         (502) staff       (20)        0 2024-04-29 08:43:15.811410 deepgpu-2.1.0rc3/deepgpu.egg-info/
+-rw-r--r--   0 du         (502) staff       (20)      615 2024-04-29 08:43:15.000000 deepgpu-2.1.0rc3/deepgpu.egg-info/PKG-INFO
+-rw-r--r--   0 du         (502) staff       (20)      196 2024-04-29 08:43:15.000000 deepgpu-2.1.0rc3/deepgpu.egg-info/SOURCES.txt
+-rw-r--r--   0 du         (502) staff       (20)        1 2024-04-29 08:43:15.000000 deepgpu-2.1.0rc3/deepgpu.egg-info/dependency_links.txt
+-rw-r--r--   0 du         (502) staff       (20)        8 2024-04-29 08:43:15.000000 deepgpu-2.1.0rc3/deepgpu.egg-info/top_level.txt
+-rw-r--r--   0 du         (502) staff       (20)       38 2024-04-29 08:43:15.812251 deepgpu-2.1.0rc3/setup.cfg
+-rw-r--r--   0 du         (502) staff       (20)     6789 2024-04-29 08:41:02.000000 deepgpu-2.1.0rc3/setup.py
```

### Comparing `deepgpu-2.1.0rc2/PKG-INFO` & `deepgpu-2.1.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgpu
-Version: 2.1.0rc2
+Version: 2.1.0rc3
 Summary: DEEPGPU is a toolset for AI training acceleration on Alibaba Cloud.
 Home-page: https://www.aliyun.com
 Author: Alibaba Cloud
 License: Copyright (C) Alibaba Group Holding Limited
 Keywords: Distributed,Deep Learning,Communication,NCCL,Pytorch,Tensorflow
 Requires-Python: >=3.8
```

### Comparing `deepgpu-2.1.0rc2/deepgpu.egg-info/PKG-INFO` & `deepgpu-2.1.0rc3/deepgpu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgpu
-Version: 2.1.0rc2
+Version: 2.1.0rc3
 Summary: DEEPGPU is a toolset for AI training acceleration on Alibaba Cloud.
 Home-page: https://www.aliyun.com
 Author: Alibaba Cloud
 License: Copyright (C) Alibaba Group Holding Limited
 Keywords: Distributed,Deep Learning,Communication,NCCL,Pytorch,Tensorflow
 Requires-Python: >=3.8
```

### Comparing `deepgpu-2.1.0rc2/setup.py` & `deepgpu-2.1.0rc3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 import subprocess
 from setuptools.command.install import install
 import os
 
 NAME="deepgpu"
-DEEPGPU_VERSION = "2.1.0rc2"
+DEEPGPU_VERSION = "2.1.0rc3"
 DEEPYTORCH_PKG_VERSION = DEEPGPU_VERSION # same as DEEPGPU version so far
 
 support_os_list = ['ubuntu', 'centos', 'alinux'] # add version later
 support_pytorch_version = ['1.10', '1.11', '1.12', '1.13', '2.0', '2.1']
 support_cuda_version = ['11.1', '11.3', '11.6', '11.7', '11.8', '12.1']
 support_python_version = ['38', '39', '310', '311']
 
@@ -96,15 +96,16 @@
             assert supported == True, \
                 f"{NAME}-{DEEPGPU_VERSION} installed failed for not testing on this os: {os_name} "
         if python_version not in support_python_version:
             supported = False
         if cuda_version not in support_cuda_version:
             supported = False
         if framework_version not in support_pytorch_version:
-            supported = False
+            if framework_version[-2:] != 'a0':
+                supported = False
         assert supported == True, \
             f"{NAME}-{DEEPGPU_VERSION} installed failed for not supporting torch with version: " \
             f"{framework_type}-{framework_version}+cu{cuda_version}-cp{python_version}"
         os.system(f'echo "check deepgpu-version successed!" >> {_temp_log} ')
 
     def run(self):
         # get env
@@ -120,14 +121,17 @@
         framework_version = list(dl.values())[0]
         self.check_deepgpu_version(os_name,
                                    python_version,
                                    cuda_version,
                                    framework_type,
                                    framework_version)
 
+        if framework_version[-2:] == 'a0':
+            framework_version = 'any'
+            cuda_version = 'any'
         # install deepytorch
         pkg = f"{_root_path_deepytorch}" \
             f"deepytorch-{DEEPYTORCH_PKG_VERSION}+{framework_type}{framework_version}" \
             f"cuda{cuda_version}-cp{python_version}-cp{python_version}{py_abi}-" \
             f"linux_x86_64.whl"
         os.system(f'echo "Install: {pkg}" >> {_temp_log}')
         cmd = ["pip3", "install", "--no-cache-dir", "--force-reinstall",
```

