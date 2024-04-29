# Comparing `tmp/drfexts-3.8.4.tar.gz` & `tmp/drfexts-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drfexts-3.8.4.tar", max compression
+gzip compressed data, was "drfexts-3.9.0.tar", max compression
```

## Comparing `drfexts-3.8.4.tar` & `drfexts-3.9.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11347 2022-08-12 03:23:59.731526 drfexts-3.8.4/LICENSE
--rw-r--r--   0        0        0     3514 2022-12-20 09:03:24.666040 drfexts-3.8.4/README.md
--rw-r--r--   0        0        0       22 2024-04-22 08:42:05.860518 drfexts-3.8.4/drfexts/__init__.py
--rw-r--r--   0        0        0      234 2022-08-31 09:46:14.033000 drfexts-3.8.4/drfexts/authentication.py
--rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323137 drfexts-3.8.4/drfexts/choices.py
--rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323301 drfexts-3.8.4/drfexts/constants.py
--rw-r--r--   0        0        0     1028 2024-04-08 07:16:45.990920 drfexts-3.8.4/drfexts/exceptions.py
--rw-r--r--   0        0        0    14673 2024-04-22 08:41:55.352402 drfexts-3.8.4/drfexts/fields.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.033000 drfexts-3.8.4/drfexts/filtersets/__init__.py
--rw-r--r--   0        0        0    18401 2024-03-26 08:39:08.648727 drfexts-3.8.4/drfexts/filtersets/backends.py
--rw-r--r--   0        0        0      964 2024-01-25 08:43:38.750362 drfexts-3.8.4/drfexts/filtersets/fields.py
--rw-r--r--   0        0        0     7878 2024-01-26 07:54:13.385952 drfexts-3.8.4/drfexts/filtersets/filters.py
--rw-r--r--   0        0        0     3155 2024-01-26 07:49:30.950714 drfexts-3.8.4/drfexts/filtersets/widgets.py
--rw-r--r--   0        0        0      534 2024-04-09 09:51:19.663972 drfexts-3.8.4/drfexts/middlewares.py
--rw-r--r--   0        0        0     6800 2022-12-20 09:03:31.324165 drfexts-3.8.4/drfexts/models.py
--rw-r--r--   0        0        0     6304 2023-02-19 06:30:29.180143 drfexts-3.8.4/drfexts/pagination.py
--rw-r--r--   0        0        0     1505 2022-12-20 09:03:24.668996 drfexts-3.8.4/drfexts/paginators.py
--rw-r--r--   0        0        0     4186 2024-01-26 07:54:13.386493 drfexts-3.8.4/drfexts/parsers.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.034000 drfexts-3.8.4/drfexts/permissions.py
--rw-r--r--   0        0        0    10349 2024-01-26 07:54:13.386894 drfexts-3.8.4/drfexts/renderers.py
--rw-r--r--   0        0        0      281 2022-12-20 09:03:24.669838 drfexts-3.8.4/drfexts/routers.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.035000 drfexts-3.8.4/drfexts/serializers/__init__.py
--rw-r--r--   0        0        0    11857 2024-04-22 07:53:44.283450 drfexts-3.8.4/drfexts/serializers/fields.py
--rw-r--r--   0        0        0     4748 2024-04-09 09:51:46.898835 drfexts-3.8.4/drfexts/serializers/mixins.py
--rw-r--r--   0        0        0     4123 2024-03-26 10:39:08.904860 drfexts-3.8.4/drfexts/serializers/serializers.py
--rw-r--r--   0        0        0     1542 2024-01-26 07:54:13.388008 drfexts-3.8.4/drfexts/settings.py
--rw-r--r--   0        0        0     1018 2022-12-20 09:03:24.671352 drfexts-3.8.4/drfexts/storages.py
--rw-r--r--   0        0        0      257 2024-01-26 07:54:13.388379 drfexts-3.8.4/drfexts/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388457 drfexts-3.8.4/drfexts/utils/encoders.py
--rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388512 drfexts-3.8.4/drfexts/utils/log.py
--rw-r--r--   0        0        0      169 2024-01-26 07:54:13.388867 drfexts-3.8.4/drfexts/utils/string.py
--rw-r--r--   0        0        0     3976 2024-04-15 02:12:05.521855 drfexts-3.8.4/drfexts/utils/utils.py
--rw-r--r--   0        0        0     9326 2024-04-01 02:42:55.691495 drfexts-3.8.4/drfexts/viewsets.py
--rw-r--r--   0        0        0     1650 2024-04-22 08:42:05.866574 drfexts-3.8.4/pyproject.toml
--rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 drfexts-3.8.4/PKG-INFO
+-rw-r--r--   0        0        0    11347 2022-08-12 03:23:59.731526 drfexts-3.9.0/LICENSE
+-rw-r--r--   0        0        0     3514 2022-12-20 09:03:24.666040 drfexts-3.9.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-29 07:55:52.260578 drfexts-3.9.0/drfexts/__init__.py
+-rw-r--r--   0        0        0      234 2022-08-31 09:46:14.033000 drfexts-3.9.0/drfexts/authentication.py
+-rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323137 drfexts-3.9.0/drfexts/choices.py
+-rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323301 drfexts-3.9.0/drfexts/constants.py
+-rw-r--r--   0        0        0     1028 2024-04-08 07:16:45.990920 drfexts-3.9.0/drfexts/exceptions.py
+-rw-r--r--   0        0        0    14673 2024-04-29 07:42:01.767486 drfexts-3.9.0/drfexts/fields.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.033000 drfexts-3.9.0/drfexts/filtersets/__init__.py
+-rw-r--r--   0        0        0    18401 2024-04-29 07:42:01.768007 drfexts-3.9.0/drfexts/filtersets/backends.py
+-rw-r--r--   0        0        0      964 2024-01-25 08:43:38.750362 drfexts-3.9.0/drfexts/filtersets/fields.py
+-rw-r--r--   0        0        0     7878 2024-04-29 07:42:01.768377 drfexts-3.9.0/drfexts/filtersets/filters.py
+-rw-r--r--   0        0        0     3155 2024-04-29 07:42:01.768676 drfexts-3.9.0/drfexts/filtersets/widgets.py
+-rw-r--r--   0        0        0      534 2024-04-29 07:42:01.769000 drfexts-3.9.0/drfexts/middlewares.py
+-rw-r--r--   0        0        0     6800 2022-12-20 09:03:31.324165 drfexts-3.9.0/drfexts/models.py
+-rw-r--r--   0        0        0     6304 2023-02-19 06:30:29.180143 drfexts-3.9.0/drfexts/pagination.py
+-rw-r--r--   0        0        0     1505 2022-12-20 09:03:24.668996 drfexts-3.9.0/drfexts/paginators.py
+-rw-r--r--   0        0        0     4186 2024-01-26 07:54:13.386493 drfexts-3.9.0/drfexts/parsers.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.034000 drfexts-3.9.0/drfexts/permissions.py
+-rw-r--r--   0        0        0    10349 2024-01-26 07:54:13.386894 drfexts-3.9.0/drfexts/renderers.py
+-rw-r--r--   0        0        0      281 2022-12-20 09:03:24.669838 drfexts-3.9.0/drfexts/routers.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.035000 drfexts-3.9.0/drfexts/serializers/__init__.py
+-rw-r--r--   0        0        0    11857 2024-04-29 07:42:01.769362 drfexts-3.9.0/drfexts/serializers/fields.py
+-rw-r--r--   0        0        0     4748 2024-04-29 07:42:01.769735 drfexts-3.9.0/drfexts/serializers/mixins.py
+-rw-r--r--   0        0        0     4123 2024-04-29 07:42:01.770156 drfexts-3.9.0/drfexts/serializers/serializers.py
+-rw-r--r--   0        0        0     1542 2024-04-29 07:42:01.771240 drfexts-3.9.0/drfexts/settings.py
+-rw-r--r--   0        0        0     1018 2022-12-20 09:03:24.671352 drfexts-3.9.0/drfexts/storages.py
+-rw-r--r--   0        0        0      257 2024-04-29 07:42:01.771628 drfexts-3.9.0/drfexts/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:42:01.771693 drfexts-3.9.0/drfexts/utils/encoders.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:42:01.771741 drfexts-3.9.0/drfexts/utils/log.py
+-rw-r--r--   0        0        0      169 2024-04-29 07:42:01.772096 drfexts-3.9.0/drfexts/utils/string.py
+-rw-r--r--   0        0        0     3976 2024-04-22 09:55:21.812479 drfexts-3.9.0/drfexts/utils/utils.py
+-rw-r--r--   0        0        0     9459 2024-04-29 07:55:46.019959 drfexts-3.9.0/drfexts/viewsets.py
+-rw-r--r--   0        0        0     1650 2024-04-29 07:55:52.266570 drfexts-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 drfexts-3.9.0/PKG-INFO
```

### Comparing `drfexts-3.8.4/LICENSE` & `drfexts-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/README.md` & `drfexts-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/choices.py` & `drfexts-3.9.0/drfexts/choices.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/constants.py` & `drfexts-3.9.0/drfexts/constants.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/exceptions.py` & `drfexts-3.9.0/drfexts/exceptions.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/fields.py` & `drfexts-3.9.0/drfexts/fields.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/filtersets/backends.py` & `drfexts-3.9.0/drfexts/filtersets/backends.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/filtersets/fields.py` & `drfexts-3.9.0/drfexts/filtersets/fields.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/filtersets/filters.py` & `drfexts-3.9.0/drfexts/filtersets/filters.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/filtersets/widgets.py` & `drfexts-3.9.0/drfexts/filtersets/widgets.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/middlewares.py` & `drfexts-3.9.0/drfexts/middlewares.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/models.py` & `drfexts-3.9.0/drfexts/models.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/pagination.py` & `drfexts-3.9.0/drfexts/pagination.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/paginators.py` & `drfexts-3.9.0/drfexts/paginators.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/parsers.py` & `drfexts-3.9.0/drfexts/parsers.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/renderers.py` & `drfexts-3.9.0/drfexts/renderers.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/serializers/fields.py` & `drfexts-3.9.0/drfexts/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/serializers/mixins.py` & `drfexts-3.9.0/drfexts/serializers/mixins.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/serializers/serializers.py` & `drfexts-3.9.0/drfexts/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/settings.py` & `drfexts-3.9.0/drfexts/settings.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/storages.py` & `drfexts-3.9.0/drfexts/storages.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/utils/utils.py` & `drfexts-3.9.0/drfexts/utils/utils.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.8.4/drfexts/viewsets.py` & `drfexts-3.9.0/drfexts/viewsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from django.utils import timezone
 from rest_framework.fields import ReadOnlyField
 from rest_framework.serializers import ModelSerializer, Serializer
 from rest_framework.viewsets import GenericViewSet
 
 from drfexts.renderers import CustomCSVRenderer, CustomXLSXRenderer
 
+from .filtersets.filters import MultipleSelectFilter
 from .serializers.mixins import ExportSerializerMixin
 
 
 class EagerLoadingMixin:
     function_name = "setup_eager_loading"
 
     def get_queryset(self, *args, **kwargs):
@@ -193,14 +194,15 @@
 class ExportMixin:
     """
     Export data to csv/xlsx file
     """
 
     export_actions = ["list"]
     default_base_filename = "export"
+    filterset_fields_overwrite = {"ids": MultipleSelectFilter(field_name="pk")}
 
     def is_export_action(self) -> bool:
         """
         Return True if the current action is an export action.
         :return:
         """
         if not hasattr(self.request, "accepted_media_type"):
```

### Comparing `drfexts-3.8.4/pyproject.toml` & `drfexts-3.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.commitizen]
-version = "3.8.4"
+version = "3.9.0"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_files = ["pyproject.toml:version", "drfexts/__init__.py"]
 
 [tool.poetry]
 name = "drfexts"
-version = "3.8.4"
+version = "3.9.0"
 package-mode = true
 readme = "README.md"
 description = "Django Restframework Utils"
 authors = ["aiden <allaher@icloud.com>"]
 keywords = ["django", "restframework"]
 homepage = "https://github.com/aiden520/drfexts"
 repository = "https://github.com/aiden520/drfexts"
```

### Comparing `drfexts-3.8.4/PKG-INFO` & `drfexts-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drfexts
-Version: 3.8.4
+Version: 3.9.0
 Summary: Django Restframework Utils
 Home-page: https://github.com/aiden520/drfexts
 License: Apache-2.0
 Keywords: django,restframework
 Author: aiden
 Author-email: allaher@icloud.com
 Requires-Python: >=3.10,<4.0.0
```

