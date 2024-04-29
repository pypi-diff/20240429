# Comparing `tmp/beeize-sdk-python-0.1.2.tar.gz` & `tmp/beeize-sdk-python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beeize-sdk-python-0.1.2.tar", last modified: Sat Apr 27 13:01:35 2024, max compression
+gzip compressed data, was "beeize-sdk-python-0.1.3.tar", last modified: Mon Apr 29 14:40:35 2024, max compression
```

## Comparing `beeize-sdk-python-0.1.2.tar` & `beeize-sdk-python-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-27 13:01:35.531160 beeize-sdk-python-0.1.2/
--rw-r--r--   0 zhaoyang   (501) staff       (20)       97 2024-04-27 13:01:35.530885 beeize-sdk-python-0.1.2/PKG-INFO
--rw-r--r--   0 zhaoyang   (501) staff       (20)     6405 2024-04-08 15:33:34.000000 beeize-sdk-python-0.1.2/README.md
--rw-r--r--   0 zhaoyang   (501) staff       (20)       38 2024-04-27 13:01:35.531256 beeize-sdk-python-0.1.2/setup.cfg
--rw-r--r--   0 zhaoyang   (501) staff       (20)      364 2024-04-27 13:00:45.000000 beeize-sdk-python-0.1.2/setup.py
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-27 13:01:35.522448 beeize-sdk-python-0.1.2/src/
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-27 13:01:35.526418 beeize-sdk-python-0.1.2/src/beeize/
--rw-r--r--   0 zhaoyang   (501) staff       (20)       14 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.2/src/beeize/__init__.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     1130 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.2/src/beeize/config.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)      132 2023-12-03 06:12:45.000000 beeize-sdk-python-0.1.2/src/beeize/consts.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     1571 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.2/src/beeize/scraper.py
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-27 13:01:35.529364 beeize-sdk-python-0.1.2/src/beeize/storages/
--rw-r--r--   0 zhaoyang   (501) staff       (20)      176 2024-04-27 11:34:11.000000 beeize-sdk-python-0.1.2/src/beeize/storages/__init__.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     2846 2024-04-27 11:41:19.000000 beeize-sdk-python-0.1.2/src/beeize/storages/dataset.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     6547 2024-04-27 13:00:45.000000 beeize-sdk-python-0.1.2/src/beeize/storages/kv_store.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     5203 2024-04-27 11:41:19.000000 beeize-sdk-python-0.1.2/src/beeize/storages/request_queue.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)        0 2023-11-15 15:27:00.000000 beeize-sdk-python-0.1.2/src/beeize/storages/storage_manager.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     2174 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.2/src/beeize/utils.py
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-27 13:01:35.530516 beeize-sdk-python-0.1.2/src/beeize_sdk_python.egg-info/
--rw-r--r--   0 zhaoyang   (501) staff       (20)       97 2024-04-27 13:01:35.000000 beeize-sdk-python-0.1.2/src/beeize_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 zhaoyang   (501) staff       (20)      476 2024-04-27 13:01:35.000000 beeize-sdk-python-0.1.2/src/beeize_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 zhaoyang   (501) staff       (20)        1 2024-04-27 13:01:35.000000 beeize-sdk-python-0.1.2/src/beeize_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 zhaoyang   (501) staff       (20)        7 2024-04-27 13:01:35.000000 beeize-sdk-python-0.1.2/src/beeize_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-29 14:40:35.187725 beeize-sdk-python-0.1.3/
+-rw-r--r--   0 zhaoyang   (501) staff       (20)       97 2024-04-29 14:40:35.187369 beeize-sdk-python-0.1.3/PKG-INFO
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     6405 2024-04-08 15:33:34.000000 beeize-sdk-python-0.1.3/README.md
+-rw-r--r--   0 zhaoyang   (501) staff       (20)       38 2024-04-29 14:40:35.187834 beeize-sdk-python-0.1.3/setup.cfg
+-rw-r--r--   0 zhaoyang   (501) staff       (20)      364 2024-04-29 14:40:25.000000 beeize-sdk-python-0.1.3/setup.py
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-29 14:40:35.178949 beeize-sdk-python-0.1.3/src/
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-29 14:40:35.182767 beeize-sdk-python-0.1.3/src/beeize/
+-rw-r--r--   0 zhaoyang   (501) staff       (20)       14 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.3/src/beeize/__init__.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     1130 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.3/src/beeize/config.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)      132 2023-12-03 06:12:45.000000 beeize-sdk-python-0.1.3/src/beeize/consts.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     1571 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.3/src/beeize/scraper.py
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-29 14:40:35.185769 beeize-sdk-python-0.1.3/src/beeize/storages/
+-rw-r--r--   0 zhaoyang   (501) staff       (20)      176 2024-04-27 11:34:11.000000 beeize-sdk-python-0.1.3/src/beeize/storages/__init__.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     2846 2024-04-27 11:41:19.000000 beeize-sdk-python-0.1.3/src/beeize/storages/dataset.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     6530 2024-04-29 14:39:49.000000 beeize-sdk-python-0.1.3/src/beeize/storages/kv_store.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     5203 2024-04-27 11:41:19.000000 beeize-sdk-python-0.1.3/src/beeize/storages/request_queue.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)        0 2023-11-15 15:27:00.000000 beeize-sdk-python-0.1.3/src/beeize/storages/storage_manager.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     2174 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.3/src/beeize/utils.py
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-29 14:40:35.186961 beeize-sdk-python-0.1.3/src/beeize_sdk_python.egg-info/
+-rw-r--r--   0 zhaoyang   (501) staff       (20)       97 2024-04-29 14:40:35.000000 beeize-sdk-python-0.1.3/src/beeize_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 zhaoyang   (501) staff       (20)      476 2024-04-29 14:40:35.000000 beeize-sdk-python-0.1.3/src/beeize_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaoyang   (501) staff       (20)        1 2024-04-29 14:40:35.000000 beeize-sdk-python-0.1.3/src/beeize_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaoyang   (501) staff       (20)        7 2024-04-29 14:40:35.000000 beeize-sdk-python-0.1.3/src/beeize_sdk_python.egg-info/top_level.txt
```

### Comparing `beeize-sdk-python-0.1.2/README.md` & `beeize-sdk-python-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `beeize-sdk-python-0.1.2/src/beeize/config.py` & `beeize-sdk-python-0.1.3/src/beeize/config.py`

 * *Files identical despite different names*

### Comparing `beeize-sdk-python-0.1.2/src/beeize/scraper.py` & `beeize-sdk-python-0.1.3/src/beeize/scraper.py`

 * *Files identical despite different names*

### Comparing `beeize-sdk-python-0.1.2/src/beeize/storages/dataset.py` & `beeize-sdk-python-0.1.3/src/beeize/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `beeize-sdk-python-0.1.2/src/beeize/storages/kv_store.py` & `beeize-sdk-python-0.1.3/src/beeize/storages/kv_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         if content_type == 'application/json; charset=utf-8':
             with open(file_path, 'w', encoding='utf-8', errors='ignore') as f:
                 json.dump(value, f, ensure_ascii=False, indent=4)
                 f.flush()
                 os.fsync(f.fileno())
         elif content_type in ['text/plain; charset=utf-8', 'application/octet-stream']:
             mode = 'w' if isinstance(value, str) else 'wb'
-            with open(file_path, mode, encoding='utf-8' if mode == 'w' else None, errors='ignore') as f:
+            with open(file_path, mode, encoding='utf-8' if mode == 'w' else None) as f:
                 f.write(value)
                 f.flush()
                 os.fsync(f.fileno())
 
     @staticmethod
     def _read_data(file_path: str, content_type: str) -> Union[str, bytes, dict, list]:
         if content_type == 'application/json; charset=utf-8':
```

### Comparing `beeize-sdk-python-0.1.2/src/beeize/storages/request_queue.py` & `beeize-sdk-python-0.1.3/src/beeize/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `beeize-sdk-python-0.1.2/src/beeize/utils.py` & `beeize-sdk-python-0.1.3/src/beeize/utils.py`

 * *Files identical despite different names*

