# Comparing `tmp/mongodb_orm-0.0.122.tar.gz` & `tmp/mongodb_orm-0.0.123.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_orm-0.0.122.tar", last modified: Fri Apr 26 10:47:00 2024, max compression
+gzip compressed data, was "mongodb_orm-0.0.123.tar", last modified: Mon Apr 29 09:46:49 2024, max compression
```

## Comparing `mongodb_orm-0.0.122.tar` & `mongodb_orm-0.0.123.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.931899 mongodb_orm-0.0.122/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-26 10:47:00.931144 mongodb_orm-0.0.122/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.0.122/README.md
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.909714 mongodb_orm-0.0.122/mongodb_orm/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.0.122/mongodb_orm/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.0.122/mongodb_orm/apps.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.914124 mongodb_orm-0.0.122/mongodb_orm/custom_urls/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.0.122/mongodb_orm/custom_urls/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1530 2024-04-23 15:22:07.000000 mongodb_orm-0.0.122/mongodb_orm/custom_urls/bread_urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.915401 mongodb_orm-0.0.122/mongodb_orm/decorators/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.122/mongodb_orm/decorators/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-04-04 10:34:42.000000 mongodb_orm-0.0.122/mongodb_orm/decorators/chained.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.916750 mongodb_orm-0.0.122/mongodb_orm/exceptions/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.122/mongodb_orm/exceptions/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.0.122/mongodb_orm/exceptions/syntax_exceptions.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.919392 mongodb_orm-0.0.122/mongodb_orm/interfaces/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.0.122/mongodb_orm/interfaces/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2494 2024-04-26 10:36:48.000000 mongodb_orm-0.0.122/mongodb_orm/interfaces/base_mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7557 2024-04-26 10:46:45.000000 mongodb_orm-0.0.122/mongodb_orm/interfaces/mongodb_model.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      824 2024-04-26 10:40:10.000000 mongodb_orm-0.0.122/mongodb_orm/interfaces/mongodb_model_events.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.920182 mongodb_orm-0.0.122/mongodb_orm/management/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.122/mongodb_orm/management/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.921167 mongodb_orm-0.0.122/mongodb_orm/management/commands/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.122/mongodb_orm/management/commands/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.0.122/mongodb_orm/management/commands/update_schema.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.921988 mongodb_orm-0.0.122/mongodb_orm/models/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.122/mongodb_orm/models/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.922964 mongodb_orm-0.0.122/mongodb_orm/singletons/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.122/mongodb_orm/singletons/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.0.122/mongodb_orm/singletons/mongodb_singleton_client.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.927076 mongodb_orm-0.0.122/mongodb_orm/types/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.0.122/mongodb_orm/types/Relation.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.122/mongodb_orm/types/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.0.122/mongodb_orm/types/index.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-04-04 10:34:44.000000 mongodb_orm-0.0.122/mongodb_orm/types/logger_object.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      453 2024-04-04 10:34:44.000000 mongodb_orm-0.0.122/mongodb_orm/types/model_schema.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.0.122/mongodb_orm/types/options.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      148 2024-04-23 14:22:14.000000 mongodb_orm-0.0.122/mongodb_orm/urls.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.928170 mongodb_orm-0.0.122/mongodb_orm/utils/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.0.122/mongodb_orm/utils/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1163 2024-04-26 10:44:00.000000 mongodb_orm-0.0.122/mongodb_orm/utils/helpers.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.929444 mongodb_orm-0.0.122/mongodb_orm/views/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.122/mongodb_orm/views/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3901 2024-04-23 14:28:47.000000 mongodb_orm-0.0.122/mongodb_orm/views/mongodb_api_model_view.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-26 10:47:00.930316 mongodb_orm-0.0.122/mongodb_orm.egg-info/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-26 10:47:00.000000 mongodb_orm-0.0.122/mongodb_orm.egg-info/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1208 2024-04-26 10:47:00.000000 mongodb_orm-0.0.122/mongodb_orm.egg-info/SOURCES.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-04-26 10:47:00.000000 mongodb_orm-0.0.122/mongodb_orm.egg-info/dependency_links.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-04-26 10:47:00.000000 mongodb_orm-0.0.122/mongodb_orm.egg-info/requires.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-04-26 10:47:00.000000 mongodb_orm-0.0.122/mongodb_orm.egg-info/top_level.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-04-26 10:47:00.932057 mongodb_orm-0.0.122/setup.cfg
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-04-26 10:46:45.000000 mongodb_orm-0.0.122/setup.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.703145 mongodb_orm-0.0.123/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-29 09:46:49.702183 mongodb_orm-0.0.123/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.0.123/README.md
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.678435 mongodb_orm-0.0.123/mongodb_orm/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.0.123/mongodb_orm/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.0.123/mongodb_orm/apps.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.683198 mongodb_orm-0.0.123/mongodb_orm/custom_urls/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.0.123/mongodb_orm/custom_urls/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1530 2024-04-23 15:22:07.000000 mongodb_orm-0.0.123/mongodb_orm/custom_urls/bread_urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.684587 mongodb_orm-0.0.123/mongodb_orm/decorators/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.123/mongodb_orm/decorators/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-04-04 10:34:42.000000 mongodb_orm-0.0.123/mongodb_orm/decorators/chained.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.685949 mongodb_orm-0.0.123/mongodb_orm/exceptions/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.123/mongodb_orm/exceptions/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.0.123/mongodb_orm/exceptions/syntax_exceptions.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.688948 mongodb_orm-0.0.123/mongodb_orm/interfaces/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.0.123/mongodb_orm/interfaces/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2494 2024-04-26 10:36:48.000000 mongodb_orm-0.0.123/mongodb_orm/interfaces/base_mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7557 2024-04-26 10:46:45.000000 mongodb_orm-0.0.123/mongodb_orm/interfaces/mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      801 2024-04-29 09:28:59.000000 mongodb_orm-0.0.123/mongodb_orm/interfaces/mongodb_model_events.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.689696 mongodb_orm-0.0.123/mongodb_orm/management/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.123/mongodb_orm/management/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.690595 mongodb_orm-0.0.123/mongodb_orm/management/commands/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.123/mongodb_orm/management/commands/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.0.123/mongodb_orm/management/commands/update_schema.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.691426 mongodb_orm-0.0.123/mongodb_orm/models/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.123/mongodb_orm/models/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.692582 mongodb_orm-0.0.123/mongodb_orm/singletons/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.123/mongodb_orm/singletons/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.0.123/mongodb_orm/singletons/mongodb_singleton_client.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.697065 mongodb_orm-0.0.123/mongodb_orm/types/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.0.123/mongodb_orm/types/Relation.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.123/mongodb_orm/types/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.0.123/mongodb_orm/types/index.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-04-04 10:34:44.000000 mongodb_orm-0.0.123/mongodb_orm/types/logger_object.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      453 2024-04-04 10:34:44.000000 mongodb_orm-0.0.123/mongodb_orm/types/model_schema.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.0.123/mongodb_orm/types/options.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      148 2024-04-23 14:22:14.000000 mongodb_orm-0.0.123/mongodb_orm/urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.698260 mongodb_orm-0.0.123/mongodb_orm/utils/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.0.123/mongodb_orm/utils/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1163 2024-04-26 10:44:00.000000 mongodb_orm-0.0.123/mongodb_orm/utils/helpers.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.700103 mongodb_orm-0.0.123/mongodb_orm/views/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.123/mongodb_orm/views/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3901 2024-04-23 14:28:47.000000 mongodb_orm-0.0.123/mongodb_orm/views/mongodb_api_model_view.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-29 09:46:49.701049 mongodb_orm-0.0.123/mongodb_orm.egg-info/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-04-29 09:46:49.000000 mongodb_orm-0.0.123/mongodb_orm.egg-info/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1208 2024-04-29 09:46:49.000000 mongodb_orm-0.0.123/mongodb_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-04-29 09:46:49.000000 mongodb_orm-0.0.123/mongodb_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-04-29 09:46:49.000000 mongodb_orm-0.0.123/mongodb_orm.egg-info/requires.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-04-29 09:46:49.000000 mongodb_orm-0.0.123/mongodb_orm.egg-info/top_level.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-04-29 09:46:49.703374 mongodb_orm-0.0.123/setup.cfg
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-04-29 09:43:11.000000 mongodb_orm-0.0.123/setup.py
```

### Comparing `mongodb_orm-0.0.122/README.md` & `mongodb_orm-0.0.123/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.122/mongodb_orm/custom_urls/bread_urls.py` & `mongodb_orm-0.0.123/mongodb_orm/custom_urls/bread_urls.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.122/mongodb_orm/interfaces/base_mongodb_model.py` & `mongodb_orm-0.0.123/mongodb_orm/interfaces/base_mongodb_model.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.122/mongodb_orm/interfaces/mongodb_model.py` & `mongodb_orm-0.0.123/mongodb_orm/interfaces/mongodb_model.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.122/mongodb_orm/interfaces/mongodb_model_events.py` & `mongodb_orm-0.0.123/mongodb_orm/interfaces/mongodb_model_events.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     def __new__(cls, *args, **kwargs):
         if cls is MongoDBModelEvents:
             raise TypeError(f"only children of '{cls.__name__}' may be instantiated")
         return object.__new__(cls)
 
     def on_save(self, record: dict) -> None:
         # Callback Event when new record added
-        print('works')
         pass
 
     def on_update(self, old_record: dict, new_record: dict) -> None:
         # Callback Event when a record get updated
         pass
 
     def on_partial_update(self, to_update_record: dict, new_record: dict) -> None:
```

### Comparing `mongodb_orm-0.0.122/mongodb_orm/management/commands/update_schema.py` & `mongodb_orm-0.0.123/mongodb_orm/management/commands/update_schema.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.122/mongodb_orm/utils/helpers.py` & `mongodb_orm-0.0.123/mongodb_orm/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.122/mongodb_orm/views/mongodb_api_model_view.py` & `mongodb_orm-0.0.123/mongodb_orm/views/mongodb_api_model_view.py`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.122/mongodb_orm.egg-info/SOURCES.txt` & `mongodb_orm-0.0.123/mongodb_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongodb_orm-0.0.122/setup.py` & `mongodb_orm-0.0.123/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 # Fix and optimise the library installation
 setup(
     name="mongodb_orm",
-    version="0.0.122",
+    version="0.0.123",
     author="Khai",
     author_email="sarraj.khaireddine@gmail.com",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     description="mongodb ORM for django framework",
     long_description="mongodb ORM for django framework",
```

