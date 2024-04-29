# Comparing `tmp/cuda-mock-0.1.7.tar.gz` & `tmp/cuda-mock-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cuda-mock-0.1.7.tar", last modified: Sat Apr 27 10:19:23 2024, max compression
+gzip compressed data, was "dist/cuda-mock-0.1.8.tar", last modified: Mon Apr 29 12:50:34 2024, max compression
```

## Comparing `cuda-mock-0.1.7.tar` & `cuda-mock-0.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/
--rw-r--r--   0 root         (0) root         (0)     1495 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3919 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/include/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/GlobalVarMgr.h
--rw-r--r--   0 root         (0) root         (0)     3118 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/backtrace.h
--rw-r--r--   0 root         (0) root         (0)     1505 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/cuda_mock.h
--rw-r--r--   0 root         (0) root         (0)     3205 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/env_util.h
--rw-r--r--   0 root         (0) root         (0)    13039 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/hook.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/include/logger/
--rw-r--r--   0 root         (0) root         (0)     1899 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/logger/StringRef.h
--rw-r--r--   0 root         (0) root         (0)    16271 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/logger/logger.h
--rw-r--r--   0 root         (0) root         (0)      658 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/logger/logger_stl.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/include/profile/
--rw-r--r--   0 root         (0) root         (0)     1603 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/profile/Timer.h
--rw-r--r--   0 root         (0) root         (0)    24151 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/support.h
--rw-r--r--   0 root         (0) root         (0)      340 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/xpu_mock.h
--rw-r--r--   0 root         (0) root         (0)      350 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2516 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/cuda_mock/
--rw-r--r--   0 root         (0) root         (0)      254 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/src/cuda_mock/__init__.py
--rw-r--r--   0 root         (0) root         (0)      216 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/src/cuda_mock/ctypes_helper.py
--rw-r--r--   0 root         (0) root         (0)     8620 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/src/cuda_mock/cuda_mock_impl.py
--rw-r--r--   0 root         (0) root         (0)     2701 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/src/cuda_mock/dynamic_obj.py
--rw-r--r--   0 root         (0) root         (0)    19425 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/src/cuda_mock/gpu_validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/cuda_mock.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/cuda_mock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      624 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/cuda_mock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/cuda_mock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 10:11:30.000000 cuda-mock-0.1.7/src/cuda_mock.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/cuda_mock.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/
+-rw-r--r--   0 root         (0) root         (0)     1495 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3919 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/include/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/GlobalVarMgr.h
+-rw-r--r--   0 root         (0) root         (0)     3118 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/backtrace.h
+-rw-r--r--   0 root         (0) root         (0)     1505 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/cuda_mock.h
+-rw-r--r--   0 root         (0) root         (0)     3205 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/env_util.h
+-rw-r--r--   0 root         (0) root         (0)    13039 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/hook.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/include/logger/
+-rw-r--r--   0 root         (0) root         (0)     1899 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/logger/StringRef.h
+-rw-r--r--   0 root         (0) root         (0)    16271 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/logger/logger.h
+-rw-r--r--   0 root         (0) root         (0)      658 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/logger/logger_stl.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/include/profile/
+-rw-r--r--   0 root         (0) root         (0)     1603 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/profile/Timer.h
+-rw-r--r--   0 root         (0) root         (0)    24151 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/support.h
+-rw-r--r--   0 root         (0) root         (0)      340 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/xpu_mock.h
+-rw-r--r--   0 root         (0) root         (0)      350 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/cuda_mock/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/src/cuda_mock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      216 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/src/cuda_mock/ctypes_helper.py
+-rw-r--r--   0 root         (0) root         (0)     8620 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/src/cuda_mock/cuda_mock_impl.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/src/cuda_mock/dynamic_obj.py
+-rw-r--r--   0 root         (0) root         (0)    19425 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/src/cuda_mock/gpu_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/cuda_mock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/cuda_mock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      624 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/cuda_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/cuda_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 12:42:35.000000 cuda-mock-0.1.8/src/cuda_mock.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/cuda_mock.egg-info/top_level.txt
```

### Comparing `cuda-mock-0.1.7/LICENSE` & `cuda-mock-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/PKG-INFO` & `cuda-mock-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuda-mock
-Version: 0.1.7
+Version: 0.1.8
 Summary: mock cuda runtime api
 Home-page: https://github.com/lipracer/torch-cuda-mock
 Author: lipracer
 Author-email: lipracer <lipracer@gmail.com>
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cuda-mock-0.1.7/README.md` & `cuda-mock-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/include/GlobalVarMgr.h` & `cuda-mock-0.1.8/include/GlobalVarMgr.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/include/backtrace.h` & `cuda-mock-0.1.8/include/backtrace.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/include/cuda_mock.h` & `cuda-mock-0.1.8/include/cuda_mock.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/include/env_util.h` & `cuda-mock-0.1.8/include/env_util.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/include/hook.h` & `cuda-mock-0.1.8/include/hook.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/include/logger/StringRef.h` & `cuda-mock-0.1.8/include/logger/StringRef.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/include/logger/logger.h` & `cuda-mock-0.1.8/include/logger/logger.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/include/logger/logger_stl.h` & `cuda-mock-0.1.8/include/logger/logger_stl.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/include/profile/Timer.h` & `cuda-mock-0.1.8/include/profile/Timer.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/include/support.h` & `cuda-mock-0.1.8/include/support.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/setup.py` & `cuda-mock-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         subprocess.check_call(['cmake', f'{script_dir}'] + cmake_args + ninja_args, cwd=build_dir)
         subprocess.check_call(['cmake', '--build', '.'], cwd=build_dir)
         subprocess.check_call([f'{install_cmd}', 'install'], cwd=build_dir)
 
 setup(
     name="cuda-mock",
-    version="0.1.7",
+    version="0.1.8",
     author="lipracer",
     author_email="lipracer@gmail.com",
     description="a tools hook some api call at runtime",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
 
     url="https://github.com/lipracer/torch-cuda-mock",
```

### Comparing `cuda-mock-0.1.7/src/cuda_mock/cuda_mock_impl.py` & `cuda-mock-0.1.8/src/cuda_mock/cuda_mock_impl.py`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/src/cuda_mock/dynamic_obj.py` & `cuda-mock-0.1.8/src/cuda_mock/dynamic_obj.py`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/src/cuda_mock/gpu_validation.py` & `cuda-mock-0.1.8/src/cuda_mock/gpu_validation.py`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.7/src/cuda_mock.egg-info/PKG-INFO` & `cuda-mock-0.1.8/src/cuda_mock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuda-mock
-Version: 0.1.7
+Version: 0.1.8
 Summary: mock cuda runtime api
 Home-page: https://github.com/lipracer/torch-cuda-mock
 Author: lipracer
 Author-email: lipracer <lipracer@gmail.com>
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cuda-mock-0.1.7/src/cuda_mock.egg-info/SOURCES.txt` & `cuda-mock-0.1.8/src/cuda_mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

