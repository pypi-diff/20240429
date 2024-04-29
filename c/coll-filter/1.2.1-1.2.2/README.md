# Comparing `tmp/coll-filter-1.2.1.tar.gz` & `tmp/coll-filter-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coll-filter-1.2.1.tar", last modified: Sun Apr 28 11:35:43 2024, max compression
+gzip compressed data, was "coll-filter-1.2.2.tar", last modified: Sun Apr 28 11:37:41 2024, max compression
```

## Comparing `coll-filter-1.2.1.tar` & `coll-filter-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-28 11:35:43.864221 coll-filter-1.2.1/
--rw-r--r--   0 summy      (501) staff       (20)      946 2024-04-28 11:35:43.863610 coll-filter-1.2.1/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      591 2024-04-28 11:30:28.000000 coll-filter-1.2.1/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-28 11:35:43.857457 coll-filter-1.2.1/cf/
--rw-r--r--   0 summy      (501) staff       (20)     6680 2024-04-28 11:16:57.000000 coll-filter-1.2.1/cf/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     9727 2024-04-28 11:25:00.000000 coll-filter-1.2.1/cf/base.py
--rw-r--r--   0 summy      (501) staff       (20)     5143 2024-04-28 10:05:34.000000 coll-filter-1.2.1/cf/pooling.py
--rw-r--r--   0 summy      (501) staff       (20)      867 2023-11-27 02:09:24.000000 coll-filter-1.2.1/cf/utils.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-28 11:35:43.861660 coll-filter-1.2.1/coll_filter.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      946 2024-04-28 11:35:43.000000 coll-filter-1.2.1/coll_filter.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      258 2024-04-28 11:35:43.000000 coll-filter-1.2.1/coll_filter.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-28 11:35:43.000000 coll-filter-1.2.1/coll_filter.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-28 11:32:15.000000 coll-filter-1.2.1/coll_filter.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        3 2024-04-28 11:35:43.000000 coll-filter-1.2.1/coll_filter.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-28 11:35:43.864472 coll-filter-1.2.1/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      846 2024-04-28 11:31:06.000000 coll-filter-1.2.1/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-28 11:35:43.862588 coll-filter-1.2.1/test/
--rw-r--r--   0 summy      (501) staff       (20)      277 2024-01-05 03:59:08.000000 coll-filter-1.2.1/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-28 11:37:41.374529 coll-filter-1.2.2/
+-rw-r--r--   0 summy      (501) staff       (20)      956 2024-04-28 11:37:41.373755 coll-filter-1.2.2/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      601 2024-04-28 11:37:37.000000 coll-filter-1.2.2/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-28 11:37:41.367150 coll-filter-1.2.2/cf/
+-rw-r--r--   0 summy      (501) staff       (20)     6680 2024-04-28 11:16:57.000000 coll-filter-1.2.2/cf/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     9727 2024-04-28 11:25:00.000000 coll-filter-1.2.2/cf/base.py
+-rw-r--r--   0 summy      (501) staff       (20)     5143 2024-04-28 10:05:34.000000 coll-filter-1.2.2/cf/pooling.py
+-rw-r--r--   0 summy      (501) staff       (20)      867 2023-11-27 02:09:24.000000 coll-filter-1.2.2/cf/utils.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-28 11:37:41.371737 coll-filter-1.2.2/coll_filter.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      956 2024-04-28 11:37:41.000000 coll-filter-1.2.2/coll_filter.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      258 2024-04-28 11:37:41.000000 coll-filter-1.2.2/coll_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-28 11:37:41.000000 coll-filter-1.2.2/coll_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-28 11:32:15.000000 coll-filter-1.2.2/coll_filter.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        3 2024-04-28 11:37:41.000000 coll-filter-1.2.2/coll_filter.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-28 11:37:41.374799 coll-filter-1.2.2/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      846 2024-04-28 11:37:37.000000 coll-filter-1.2.2/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-28 11:37:41.372631 coll-filter-1.2.2/test/
+-rw-r--r--   0 summy      (501) staff       (20)      277 2024-01-05 03:59:08.000000 coll-filter-1.2.2/test/test.py
```

### Comparing `coll-filter-1.2.1/PKG-INFO` & `coll-filter-1.2.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coll-filter
-Version: 1.2.1
+Version: 1.2.2
 Summary: Collaborative Filtering with multi-process parallelism.
 Home-page: https://gitee.com/summry/myai
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: Collaborative Filtering,recommend
 Platform: UNKNOWN
@@ -12,21 +12,21 @@
 Description-Content-Type: text/markdown
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from cf import CollFilter
+    from cf import CollFilter
 
-   if __name__ == '__main__':
-       data = read_data(train_path)
-       data = pre_process(data)  # return [(user_id: Any, item_id: Any, float),]
-       cf = CollFilter(data)
-       ucf = cf.user_cf()  # return {user_id: [(item_id, score),],}
-       icf = cf.item_cf()  # return {user_id: [(item_id, score),],}
-       recommends = cf.recommends(user_ids, recall_num=5) # return {user_id: [(item_id, score),],}
-       recommend = cf.recommend(user_id, recall_num=5) # return [(item_id, score),]
-       cf.release()
+    if __name__ == '__main__':
+        data = read_data(train_path)
+        data = pre_process(data)  # return [(user_id: Any, item_id: Any, float),]
+        cf = CollFilter(data)
+        ucf = cf.user_cf()  # return {user_id: [(item_id, score),],}
+        icf = cf.item_cf()  # return {user_id: [(item_id, score),],}
+        recommends = cf.recommends(user_ids, recall_num=5) # return {user_id: [(item_id, score),],}
+        recommend = cf.recommend(user_id, recall_num=5) # return [(item_id, score),]
+        cf.release()
```

### Comparing `coll-filter-1.2.1/README.rst` & `coll-filter-1.2.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from cf import CollFilter
+    from cf import CollFilter
 
-   if __name__ == '__main__':
-       data = read_data(train_path)
-       data = pre_process(data)  # return [(user_id: Any, item_id: Any, float),]
-       cf = CollFilter(data)
-       ucf = cf.user_cf()  # return {user_id: [(item_id, score),],}
-       icf = cf.item_cf()  # return {user_id: [(item_id, score),],}
-       recommends = cf.recommends(user_ids, recall_num=5) # return {user_id: [(item_id, score),],}
-       recommend = cf.recommend(user_id, recall_num=5) # return [(item_id, score),]
-       cf.release()
+    if __name__ == '__main__':
+        data = read_data(train_path)
+        data = pre_process(data)  # return [(user_id: Any, item_id: Any, float),]
+        cf = CollFilter(data)
+        ucf = cf.user_cf()  # return {user_id: [(item_id, score),],}
+        icf = cf.item_cf()  # return {user_id: [(item_id, score),],}
+        recommends = cf.recommends(user_ids, recall_num=5) # return {user_id: [(item_id, score),],}
+        recommend = cf.recommend(user_id, recall_num=5) # return [(item_id, score),]
+        cf.release()
```

### Comparing `coll-filter-1.2.1/cf/__init__.py` & `coll-filter-1.2.2/cf/__init__.py`

 * *Files identical despite different names*

### Comparing `coll-filter-1.2.1/cf/base.py` & `coll-filter-1.2.2/cf/base.py`

 * *Files identical despite different names*

### Comparing `coll-filter-1.2.1/cf/pooling.py` & `coll-filter-1.2.2/cf/pooling.py`

 * *Files identical despite different names*

### Comparing `coll-filter-1.2.1/cf/utils.py` & `coll-filter-1.2.2/cf/utils.py`

 * *Files identical despite different names*

### Comparing `coll-filter-1.2.1/coll_filter.egg-info/PKG-INFO` & `coll-filter-1.2.2/coll_filter.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coll-filter
-Version: 1.2.1
+Version: 1.2.2
 Summary: Collaborative Filtering with multi-process parallelism.
 Home-page: https://gitee.com/summry/myai
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: Collaborative Filtering,recommend
 Platform: UNKNOWN
@@ -12,21 +12,21 @@
 Description-Content-Type: text/markdown
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from cf import CollFilter
+    from cf import CollFilter
 
-   if __name__ == '__main__':
-       data = read_data(train_path)
-       data = pre_process(data)  # return [(user_id: Any, item_id: Any, float),]
-       cf = CollFilter(data)
-       ucf = cf.user_cf()  # return {user_id: [(item_id, score),],}
-       icf = cf.item_cf()  # return {user_id: [(item_id, score),],}
-       recommends = cf.recommends(user_ids, recall_num=5) # return {user_id: [(item_id, score),],}
-       recommend = cf.recommend(user_id, recall_num=5) # return [(item_id, score),]
-       cf.release()
+    if __name__ == '__main__':
+        data = read_data(train_path)
+        data = pre_process(data)  # return [(user_id: Any, item_id: Any, float),]
+        cf = CollFilter(data)
+        ucf = cf.user_cf()  # return {user_id: [(item_id, score),],}
+        icf = cf.item_cf()  # return {user_id: [(item_id, score),],}
+        recommends = cf.recommends(user_ids, recall_num=5) # return {user_id: [(item_id, score),],}
+        recommend = cf.recommend(user_id, recall_num=5) # return [(item_id, score),]
+        cf.release()
```

### Comparing `coll-filter-1.2.1/setup.py` & `coll-filter-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='coll-filter',
     packages=['cf'],
     description="Collaborative Filtering with multi-process parallelism.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.1',
+    version='1.2.2',
     url='https://gitee.com/summry/myai',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['Collaborative Filtering', 'recommend'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

