# Comparing `tmp/djeasyview-1.0.7.tar.gz` & `tmp/djeasyview-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djeasyview-1.0.7.tar", last modified: Wed Mar 20 07:09:15 2024, max compression
+gzip compressed data, was "djeasyview-1.0.8.tar", last modified: Mon Apr 29 06:40:33 2024, max compression
```

## Comparing `djeasyview-1.0.7.tar` & `djeasyview-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-03-20 07:09:15.602767 djeasyview-1.0.7/
--rw-r--r--   0 anand      (501) staff       (20)       64 2024-03-04 08:32:53.000000 djeasyview-1.0.7/MANIFEST.in
--rw-r--r--   0 anand      (501) staff       (20)     2382 2024-03-20 07:09:15.602842 djeasyview-1.0.7/PKG-INFO
--rw-r--r--   0 anand      (501) staff       (20)     1979 2024-03-20 07:06:50.000000 djeasyview-1.0.7/README.md
-drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-03-20 07:09:15.602017 djeasyview-1.0.7/djeasyview/
--rw-r--r--   0 anand      (501) staff       (20)        0 2024-03-04 08:28:49.000000 djeasyview-1.0.7/djeasyview/__init__.py
--rw-r--r--   0 anand      (501) staff       (20)     3155 2024-03-20 07:05:23.000000 djeasyview-1.0.7/djeasyview/response.py
--rw-r--r--   0 anand      (501) staff       (20)     5524 2024-03-20 06:54:51.000000 djeasyview-1.0.7/djeasyview/views.py
-drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-03-20 07:09:15.602656 djeasyview-1.0.7/djeasyview.egg-info/
--rw-r--r--   0 anand      (501) staff       (20)     2382 2024-03-20 07:09:15.000000 djeasyview-1.0.7/djeasyview.egg-info/PKG-INFO
--rw-r--r--   0 anand      (501) staff       (20)      300 2024-03-20 07:09:15.000000 djeasyview-1.0.7/djeasyview.egg-info/SOURCES.txt
--rw-r--r--   0 anand      (501) staff       (20)        1 2024-03-20 07:09:15.000000 djeasyview-1.0.7/djeasyview.egg-info/dependency_links.txt
--rw-r--r--   0 anand      (501) staff       (20)       27 2024-03-20 07:09:15.000000 djeasyview-1.0.7/djeasyview.egg-info/requires.txt
--rw-r--r--   0 anand      (501) staff       (20)       11 2024-03-20 07:09:15.000000 djeasyview-1.0.7/djeasyview.egg-info/top_level.txt
--rw-r--r--   0 anand      (501) staff       (20)      101 2024-02-29 17:49:48.000000 djeasyview-1.0.7/pyproject.toml
--rw-r--r--   0 anand      (501) staff       (20)      394 2024-03-20 07:09:15.603051 djeasyview-1.0.7/setup.cfg
--rw-r--r--   0 anand      (501) staff       (20)      467 2024-03-20 07:07:39.000000 djeasyview-1.0.7/setup.py
+drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-04-29 06:40:33.684150 djeasyview-1.0.8/
+-rw-r--r--   0 anand      (501) staff       (20)       64 2024-03-04 08:32:53.000000 djeasyview-1.0.8/MANIFEST.in
+-rw-r--r--   0 anand      (501) staff       (20)     2542 2024-04-29 06:40:33.684206 djeasyview-1.0.8/PKG-INFO
+-rw-r--r--   0 anand      (501) staff       (20)     2139 2024-03-20 07:13:01.000000 djeasyview-1.0.8/README.md
+drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-04-29 06:40:33.683274 djeasyview-1.0.8/djeasyview/
+-rw-r--r--   0 anand      (501) staff       (20)        0 2024-03-04 08:28:49.000000 djeasyview-1.0.8/djeasyview/__init__.py
+-rw-r--r--   0 anand      (501) staff       (20)     3155 2024-03-20 07:05:23.000000 djeasyview-1.0.8/djeasyview/response.py
+-rw-r--r--   0 anand      (501) staff       (20)     5621 2024-04-29 06:38:40.000000 djeasyview-1.0.8/djeasyview/views.py
+drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-04-29 06:40:33.684030 djeasyview-1.0.8/djeasyview.egg-info/
+-rw-r--r--   0 anand      (501) staff       (20)     2542 2024-04-29 06:40:33.000000 djeasyview-1.0.8/djeasyview.egg-info/PKG-INFO
+-rw-r--r--   0 anand      (501) staff       (20)      300 2024-04-29 06:40:33.000000 djeasyview-1.0.8/djeasyview.egg-info/SOURCES.txt
+-rw-r--r--   0 anand      (501) staff       (20)        1 2024-04-29 06:40:33.000000 djeasyview-1.0.8/djeasyview.egg-info/dependency_links.txt
+-rw-r--r--   0 anand      (501) staff       (20)       27 2024-04-29 06:40:33.000000 djeasyview-1.0.8/djeasyview.egg-info/requires.txt
+-rw-r--r--   0 anand      (501) staff       (20)       11 2024-04-29 06:40:33.000000 djeasyview-1.0.8/djeasyview.egg-info/top_level.txt
+-rw-r--r--   0 anand      (501) staff       (20)      101 2024-02-29 17:49:48.000000 djeasyview-1.0.8/pyproject.toml
+-rw-r--r--   0 anand      (501) staff       (20)      394 2024-04-29 06:40:33.684414 djeasyview-1.0.8/setup.cfg
+-rw-r--r--   0 anand      (501) staff       (20)      467 2024-04-29 06:40:27.000000 djeasyview-1.0.8/setup.py
```

### Comparing `djeasyview-1.0.7/PKG-INFO` & `djeasyview-1.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djeasyview
-Version: 1.0.7
+Version: 1.0.8
 Author: Anand Raj
 Author-email: anand98.ar@gmail.com
 License: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
@@ -37,14 +37,16 @@
 
 class YourView(DjeasyListCreateView):
     model = YourModel
     list_serializer_class = YourModelSerializer
     create_serializer_class = YourModelSerializer
     serializer_class = YourModelSerializer
     queryset = YourModel
+    select_related = ['key1' , 'key2']
+    prefetch_related = ['key1' , 'key2']
     permission_classes = [IsAuthenticated]
     enable_cache = True
     cache_duration = 60
 ```
 
 ### GET , PUT , PATCH , DELETE api's
 
@@ -58,14 +60,16 @@
 
 class YourView(DjeasyRetrieveUpdateApiView):
     model = YourModel
     list_serializer_class = YourModelSerializer
     create_serializer_class = YourModelSerializer
     serializer_class = YourModelSerializer
     queryset = YourModel
+    select_related = ['key1' , 'key2']
+    prefetch_related = ['key1' , 'key2']
     permission_classes = [IsAuthenticated]
     enable_cache = True
     cache_duration = 60
 ```
```

### Comparing `djeasyview-1.0.7/README.md` & `djeasyview-1.0.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
 class YourView(DjeasyListCreateView):
     model = YourModel
     list_serializer_class = YourModelSerializer
     create_serializer_class = YourModelSerializer
     serializer_class = YourModelSerializer
     queryset = YourModel
+    select_related = ['key1' , 'key2']
+    prefetch_related = ['key1' , 'key2']
     permission_classes = [IsAuthenticated]
     enable_cache = True
     cache_duration = 60
 ```
 
 ### GET , PUT , PATCH , DELETE api's
 
@@ -45,14 +47,16 @@
 
 class YourView(DjeasyRetrieveUpdateApiView):
     model = YourModel
     list_serializer_class = YourModelSerializer
     create_serializer_class = YourModelSerializer
     serializer_class = YourModelSerializer
     queryset = YourModel
+    select_related = ['key1' , 'key2']
+    prefetch_related = ['key1' , 'key2']
     permission_classes = [IsAuthenticated]
     enable_cache = True
     cache_duration = 60
 ```
```

### Comparing `djeasyview-1.0.7/djeasyview/response.py` & `djeasyview-1.0.8/djeasyview/response.py`

 * *Files identical despite different names*

### Comparing `djeasyview-1.0.7/djeasyview/views.py` & `djeasyview-1.0.8/djeasyview/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     model: Type[Model]
     context: Optional[Dict[str, any]] = None
     serializer_save: Optional[Dict[str, any]] = None
     select_related: Optional[List[str]] = None
     prefetch_related: Optional[List[str]] = None
     enable_cache: Optional[bool] = False
     cache_duration: Optional[int] = None
+    order_by: Optional[List[str]] = None
 
     def __init__(self) -> None:
         if self.enable_cache and not self.cache_duration:
             raise ImproperlyConfigured(
                 "if enable cache is set to True you must define the cache duration , example 60 * 60 "
             )
 
@@ -50,15 +51,15 @@
 
     def get_queryset(self) -> Model:
         queryset = super().get_queryset()
         if self.select_related:
             queryset = queryset.select_related(*self.select_related)
         if self.prefetch_related:
             queryset = queryset.prefetch_related(*self.prefetch_related)
-        return queryset
+        return queryset.order_by(*self.order_by) if self.order_by else queryset
 
     def get_list_serializer(self, instance: Model) -> BaseSerializer:
         return (
             self.list_serializer_class(instance, context=self.context, many=True)
             if self.context
             else self.list_serializer_class(instance, many=True)
         )
```

### Comparing `djeasyview-1.0.7/djeasyview.egg-info/PKG-INFO` & `djeasyview-1.0.8/djeasyview.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djeasyview
-Version: 1.0.7
+Version: 1.0.8
 Author: Anand Raj
 Author-email: anand98.ar@gmail.com
 License: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
@@ -37,14 +37,16 @@
 
 class YourView(DjeasyListCreateView):
     model = YourModel
     list_serializer_class = YourModelSerializer
     create_serializer_class = YourModelSerializer
     serializer_class = YourModelSerializer
     queryset = YourModel
+    select_related = ['key1' , 'key2']
+    prefetch_related = ['key1' , 'key2']
     permission_classes = [IsAuthenticated]
     enable_cache = True
     cache_duration = 60
 ```
 
 ### GET , PUT , PATCH , DELETE api's
 
@@ -58,14 +60,16 @@
 
 class YourView(DjeasyRetrieveUpdateApiView):
     model = YourModel
     list_serializer_class = YourModelSerializer
     create_serializer_class = YourModelSerializer
     serializer_class = YourModelSerializer
     queryset = YourModel
+    select_related = ['key1' , 'key2']
+    prefetch_related = ['key1' , 'key2']
     permission_classes = [IsAuthenticated]
     enable_cache = True
     cache_duration = 60
 ```
```

