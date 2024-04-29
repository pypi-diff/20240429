# Comparing `tmp/simple_disk_queue-0.0.1.tar.gz` & `tmp/simple_disk_queue-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_disk_queue-0.0.1.tar", last modified: Thu Nov  9 01:11:22 2023, max compression
+gzip compressed data, was "simple_disk_queue-0.0.2.tar", last modified: Mon Apr 29 21:13:03 2024, max compression
```

## Comparing `simple_disk_queue-0.0.1.tar` & `simple_disk_queue-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 zhenlin4 (1132177) zhenlin4 (1132177)        0 2023-11-09 01:11:22.071527 simple_disk_queue-0.0.1/
--rw-r--r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      900 2023-11-09 01:11:22.071527 simple_disk_queue-0.0.1/PKG-INFO
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      439 2023-11-09 01:08:22.000000 simple_disk_queue-0.0.1/README.md
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)       38 2023-11-09 01:11:22.071527 simple_disk_queue-0.0.1/setup.cfg
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1115 2023-11-08 03:38:06.000000 simple_disk_queue-0.0.1/setup.py
-drwxrwxr-x   0 zhenlin4 (1132177) zhenlin4 (1132177)        0 2023-11-09 01:11:22.069527 simple_disk_queue-0.0.1/simple_disk_queue/
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      244 2023-11-09 00:54:44.000000 simple_disk_queue-0.0.1/simple_disk_queue/__init__.py
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1481 2023-11-09 01:08:37.000000 simple_disk_queue-0.0.1/simple_disk_queue/_utils.py
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      422 2023-11-08 04:51:55.000000 simple_disk_queue-0.0.1/simple_disk_queue/config.py
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     3109 2023-11-09 00:56:35.000000 simple_disk_queue-0.0.1/simple_disk_queue/disk_queue.py
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      736 2023-11-09 00:56:47.000000 simple_disk_queue-0.0.1/simple_disk_queue/rw_lock.py
-drwxrwxr-x   0 zhenlin4 (1132177) zhenlin4 (1132177)        0 2023-11-09 01:11:22.071527 simple_disk_queue-0.0.1/simple_disk_queue.egg-info/
--rw-r--r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      900 2023-11-09 01:11:22.000000 simple_disk_queue-0.0.1/simple_disk_queue.egg-info/PKG-INFO
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      369 2023-11-09 01:11:22.000000 simple_disk_queue-0.0.1/simple_disk_queue.egg-info/SOURCES.txt
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)        1 2023-11-09 01:11:22.000000 simple_disk_queue-0.0.1/simple_disk_queue.egg-info/dependency_links.txt
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)       16 2023-11-09 01:11:22.000000 simple_disk_queue-0.0.1/simple_disk_queue.egg-info/requires.txt
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)       18 2023-11-09 01:11:22.000000 simple_disk_queue-0.0.1/simple_disk_queue.egg-info/top_level.txt
+drwxrwxr-x   0 zhenlin4 (1132177) zhenlin4 (1132177)        0 2024-04-29 21:13:03.758756 simple_disk_queue-0.0.2/
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1051 2024-04-29 21:13:03.756756 simple_disk_queue-0.0.2/PKG-INFO
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      439 2024-04-29 21:12:11.000000 simple_disk_queue-0.0.2/README.md
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)       38 2024-04-29 21:13:03.759756 simple_disk_queue-0.0.2/setup.cfg
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1115 2024-04-29 21:12:11.000000 simple_disk_queue-0.0.2/setup.py
+drwxrwxr-x   0 zhenlin4 (1132177) zhenlin4 (1132177)        0 2024-04-29 21:13:03.728756 simple_disk_queue-0.0.2/simple_disk_queue/
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      303 2024-04-29 21:12:11.000000 simple_disk_queue-0.0.2/simple_disk_queue/__init__.py
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1897 2024-04-29 21:12:11.000000 simple_disk_queue-0.0.2/simple_disk_queue/_utils.py
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      422 2024-02-20 23:58:23.000000 simple_disk_queue-0.0.2/simple_disk_queue/config.py
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     6107 2024-04-29 21:12:12.000000 simple_disk_queue-0.0.2/simple_disk_queue/disk_queue.py
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      962 2024-04-29 21:12:12.000000 simple_disk_queue-0.0.2/simple_disk_queue/rw_lock.py
+drwxrwxr-x   0 zhenlin4 (1132177) zhenlin4 (1132177)        0 2024-04-29 21:13:03.752756 simple_disk_queue-0.0.2/simple_disk_queue.egg-info/
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1051 2024-04-29 21:13:03.000000 simple_disk_queue-0.0.2/simple_disk_queue.egg-info/PKG-INFO
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      369 2024-04-29 21:13:03.000000 simple_disk_queue-0.0.2/simple_disk_queue.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)        1 2024-04-29 21:13:03.000000 simple_disk_queue-0.0.2/simple_disk_queue.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)       16 2024-04-29 21:13:03.000000 simple_disk_queue-0.0.2/simple_disk_queue.egg-info/requires.txt
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)       18 2024-04-29 21:13:03.000000 simple_disk_queue-0.0.2/simple_disk_queue.egg-info/top_level.txt
```

### Comparing `simple_disk_queue-0.0.1/PKG-INFO` & `simple_disk_queue-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: simple_disk_queue
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create a disk-based queue
 Home-page: https://github.com/zlin7/python-simple_disk_queue
 Author: Zhen Lin
 Author-email: zhenlin4@illinois.edu
 License: MIT
+Description: 
+        # Installation
+        
+        `pip install .` or `pip install simple-disk-queue`
+        
+        **By default, a folder called `.cache/simple_disk_queue` is created under your home directory, and will be used to store queues.**
+        If you want to change it, see "Global Settings" below.
+        
+        # Quick Start
+        
+        An example can be found in `examples/test.py`.
+        We can first call `init_queue()` to initialize the jobs, and then run `sdq.DiskQueue.run('test')` in different processes.
+        
+        
+        
+        
+        ## 0.0.1
+        ==================
+        
+        1. Core functionality: Add jobs to a queue and run jobs from a queue.
 Keywords: Job Scheduler,Disk-based Queue,Disk Queue Scheduler
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: filelock>=3.9.0
-
-
-# Installation
-
-`pip install .` or `pip install simple-disk-queue`
-
-**By default, a folder called `.cache/simple_disk_queue` is created under your home directory, and will be used to store queues.**
-If you want to change it, see "Global Settings" below.
-
-# Quick Start
-
-An example can be found in `examples/test.py`.
-We can first call `init_queue()` to initialize the jobs, and then run `sdq.DiskQueue.run('test')` in different processes.
-
-
-
-
-## 0.0.1
-==================
-
-1. Core functionality: Add jobs to a queue and run jobs from a queue.
```

### Comparing `simple_disk_queue-0.0.1/setup.py` & `simple_disk_queue-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md', encoding='utf-8') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='simple_disk_queue',
-    version='0.0.1',
+    version='0.0.2',
     description='Create a disk-based queue',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Zhen Lin',
     author_email='zhenlin4@illinois.edu',
```

### Comparing `simple_disk_queue-0.0.1/simple_disk_queue.egg-info/PKG-INFO` & `simple_disk_queue-0.0.2/simple_disk_queue.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: simple-disk-queue
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create a disk-based queue
 Home-page: https://github.com/zlin7/python-simple_disk_queue
 Author: Zhen Lin
 Author-email: zhenlin4@illinois.edu
 License: MIT
+Description: 
+        # Installation
+        
+        `pip install .` or `pip install simple-disk-queue`
+        
+        **By default, a folder called `.cache/simple_disk_queue` is created under your home directory, and will be used to store queues.**
+        If you want to change it, see "Global Settings" below.
+        
+        # Quick Start
+        
+        An example can be found in `examples/test.py`.
+        We can first call `init_queue()` to initialize the jobs, and then run `sdq.DiskQueue.run('test')` in different processes.
+        
+        
+        
+        
+        ## 0.0.1
+        ==================
+        
+        1. Core functionality: Add jobs to a queue and run jobs from a queue.
 Keywords: Job Scheduler,Disk-based Queue,Disk Queue Scheduler
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: filelock>=3.9.0
-
-
-# Installation
-
-`pip install .` or `pip install simple-disk-queue`
-
-**By default, a folder called `.cache/simple_disk_queue` is created under your home directory, and will be used to store queues.**
-If you want to change it, see "Global Settings" below.
-
-# Quick Start
-
-An example can be found in `examples/test.py`.
-We can first call `init_queue()` to initialize the jobs, and then run `sdq.DiskQueue.run('test')` in different processes.
-
-
-
-
-## 0.0.1
-==================
-
-1. Core functionality: Add jobs to a queue and run jobs from a queue.
```

