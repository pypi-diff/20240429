# Comparing `tmp/pyesorm-0.3.0.tar.gz` & `tmp/pyesorm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyesorm-0.3.0.tar", last modified: Thu Jan 25 12:23:38 2024, max compression
+gzip compressed data, was "pyesorm-0.3.1.tar", last modified: Mon Apr 29 12:27:40 2024, max compression
```

## Comparing `pyesorm-0.3.0.tar` & `pyesorm-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-01-25 12:23:38.543590 pyesorm-0.3.0/
--rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.3.0/LICENSE
--rw-r--r--   0 wallner    (501) staff       (20)    21538 2024-01-25 12:23:38.543361 pyesorm-0.3.0/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)    19908 2024-01-25 10:51:50.000000 pyesorm-0.3.0/README.md
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-01-25 12:23:38.532882 pyesorm-0.3.0/docs/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.3.0/docs/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.3.0/docs/changelog.py
--rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.3.0/docs/conf.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-01-25 12:23:38.537645 pyesorm-0.3.0/esorm/
--rw-r--r--   0 wallner    (501) staff       (20)      638 2023-10-30 16:10:12.000000 pyesorm-0.3.0/esorm/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.3.0/esorm/aggs.py
--rw-r--r--   0 wallner    (501) staff       (20)     2041 2023-10-30 16:10:12.000000 pyesorm-0.3.0/esorm/bulk.py
--rw-r--r--   0 wallner    (501) staff       (20)      470 2023-10-30 16:10:12.000000 pyesorm-0.3.0/esorm/error.py
--rw-r--r--   0 wallner    (501) staff       (20)     1943 2023-10-31 19:12:30.000000 pyesorm-0.3.0/esorm/esorm.py
--rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.3.0/esorm/fastapi.py
--rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.3.0/esorm/fields.py
--rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.3.0/esorm/logger.py
--rw-r--r--   0 wallner    (501) staff       (20)    37204 2024-01-25 08:25:00.000000 pyesorm-0.3.0/esorm/model.py
--rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.3.0/esorm/query.py
--rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.3.0/esorm/response.py
--rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.3.0/esorm/utils.py
--rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.3.0/esorm/watcher.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-01-25 12:23:38.539800 pyesorm-0.3.0/pyesorm.egg-info/
--rw-r--r--   0 wallner    (501) staff       (20)    21538 2024-01-25 12:23:38.000000 pyesorm-0.3.0/pyesorm.egg-info/PKG-INFO
--rw-r--r--   0 wallner    (501) staff       (20)      514 2024-01-25 12:23:38.000000 pyesorm-0.3.0/pyesorm.egg-info/SOURCES.txt
--rw-r--r--   0 wallner    (501) staff       (20)        1 2024-01-25 12:23:38.000000 pyesorm-0.3.0/pyesorm.egg-info/dependency_links.txt
--rw-r--r--   0 wallner    (501) staff       (20)      265 2024-01-25 12:23:38.000000 pyesorm-0.3.0/pyesorm.egg-info/requires.txt
--rw-r--r--   0 wallner    (501) staff       (20)       17 2024-01-25 12:23:38.000000 pyesorm-0.3.0/pyesorm.egg-info/top_level.txt
--rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.3.0/pyproject.toml
--rw-r--r--   0 wallner    (501) staff       (20)     1297 2024-01-25 12:23:38.544243 pyesorm-0.3.0/setup.cfg
--rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.3.0/setup.py
-drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-01-25 12:23:38.540889 pyesorm-0.3.0/tests/
--rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.3.0/tests/__init__.py
--rw-r--r--   0 wallner    (501) staff       (20)     5125 2024-01-25 10:06:17.000000 pyesorm-0.3.0/tests/conftest.py
--rw-r--r--   0 wallner    (501) staff       (20)    20999 2024-01-25 10:47:20.000000 pyesorm-0.3.0/tests/test_esorm.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-04-29 12:27:40.930554 pyesorm-0.3.1/
+-rw-r--r--   0 wallner    (501) staff       (20)    16725 2023-10-30 16:10:12.000000 pyesorm-0.3.1/LICENSE
+-rw-r--r--   0 wallner    (501) staff       (20)    22773 2024-04-29 12:27:40.929481 pyesorm-0.3.1/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)    21136 2024-04-29 12:11:29.000000 pyesorm-0.3.1/README.md
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-04-29 12:27:40.909202 pyesorm-0.3.1/docs/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2024-01-17 15:06:14.000000 pyesorm-0.3.1/docs/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1484 2024-01-17 15:18:18.000000 pyesorm-0.3.1/docs/changelog.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1462 2024-01-17 15:10:11.000000 pyesorm-0.3.1/docs/conf.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-04-29 12:27:40.921892 pyesorm-0.3.1/esorm/
+-rw-r--r--   0 wallner    (501) staff       (20)      666 2024-04-29 11:40:09.000000 pyesorm-0.3.1/esorm/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3132 2024-01-22 17:32:29.000000 pyesorm-0.3.1/esorm/aggs.py
+-rw-r--r--   0 wallner    (501) staff       (20)     2046 2024-04-29 10:57:43.000000 pyesorm-0.3.1/esorm/bulk.py
+-rw-r--r--   0 wallner    (501) staff       (20)      470 2023-10-30 16:10:12.000000 pyesorm-0.3.1/esorm/error.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1943 2023-10-31 19:12:30.000000 pyesorm-0.3.1/esorm/esorm.py
+-rw-r--r--   0 wallner    (501) staff       (20)     3500 2024-01-24 09:39:22.000000 pyesorm-0.3.1/esorm/fastapi.py
+-rw-r--r--   0 wallner    (501) staff       (20)    11640 2023-10-31 19:12:30.000000 pyesorm-0.3.1/esorm/fields.py
+-rw-r--r--   0 wallner    (501) staff       (20)       52 2023-10-30 16:10:12.000000 pyesorm-0.3.1/esorm/logger.py
+-rw-r--r--   0 wallner    (501) staff       (20)    37485 2024-04-29 12:18:45.000000 pyesorm-0.3.1/esorm/model.py
+-rw-r--r--   0 wallner    (501) staff       (20)     9605 2024-01-18 19:16:18.000000 pyesorm-0.3.1/esorm/query.py
+-rw-r--r--   0 wallner    (501) staff       (20)     1315 2024-01-18 19:06:35.000000 pyesorm-0.3.1/esorm/response.py
+-rw-r--r--   0 wallner    (501) staff       (20)      996 2024-01-23 07:15:23.000000 pyesorm-0.3.1/esorm/utils.py
+-rw-r--r--   0 wallner    (501) staff       (20)     5538 2023-10-30 16:10:12.000000 pyesorm-0.3.1/esorm/watcher.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-04-29 12:27:40.927252 pyesorm-0.3.1/pyesorm.egg-info/
+-rw-r--r--   0 wallner    (501) staff       (20)    22773 2024-04-29 12:27:40.000000 pyesorm-0.3.1/pyesorm.egg-info/PKG-INFO
+-rw-r--r--   0 wallner    (501) staff       (20)      514 2024-04-29 12:27:40.000000 pyesorm-0.3.1/pyesorm.egg-info/SOURCES.txt
+-rw-r--r--   0 wallner    (501) staff       (20)        1 2024-04-29 12:27:40.000000 pyesorm-0.3.1/pyesorm.egg-info/dependency_links.txt
+-rw-r--r--   0 wallner    (501) staff       (20)      272 2024-04-29 12:27:40.000000 pyesorm-0.3.1/pyesorm.egg-info/requires.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       17 2024-04-29 12:27:40.000000 pyesorm-0.3.1/pyesorm.egg-info/top_level.txt
+-rw-r--r--   0 wallner    (501) staff       (20)       87 2023-10-31 20:33:56.000000 pyesorm-0.3.1/pyproject.toml
+-rw-r--r--   0 wallner    (501) staff       (20)     1306 2024-04-29 12:27:40.931225 pyesorm-0.3.1/setup.cfg
+-rw-r--r--   0 wallner    (501) staff       (20)       37 2023-10-30 16:10:12.000000 pyesorm-0.3.1/setup.py
+drwxr-xr-x   0 wallner    (501) staff       (20)        0 2024-04-29 12:27:40.926196 pyesorm-0.3.1/tests/
+-rw-r--r--   0 wallner    (501) staff       (20)        0 2023-10-30 16:10:12.000000 pyesorm-0.3.1/tests/__init__.py
+-rw-r--r--   0 wallner    (501) staff       (20)     6472 2024-04-29 11:47:14.000000 pyesorm-0.3.1/tests/conftest.py
+-rw-r--r--   0 wallner    (501) staff       (20)    23736 2024-04-29 11:47:54.000000 pyesorm-0.3.1/tests/test_esorm.py
```

### Comparing `pyesorm-0.3.0/LICENSE` & `pyesorm-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.0/PKG-INFO` & `pyesorm-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
@@ -22,15 +22,15 @@
 License-File: LICENSE
 Requires-Dist: typing-extensions>=4.8.0
 Requires-Dist: elasticsearch<9.0.0,>=8.6.0
 Requires-Dist: aiohttp<4.0.0,>=3.0.0
 Requires-Dist: pydantic>=2.1.0
 Provides-Extra: dev
 Requires-Dist: fastapi; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest==8.0.2; extra == "dev"
 Requires-Dist: pytest-asyncio==0.21.1; extra == "dev"
 Requires-Dist: pytest-spec; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "dev"
 Requires-Dist: sphinx-rtd-dark-mode==1.3.0; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints; extra == "dev"
@@ -52,14 +52,15 @@
     - [Supported ElasticSearch versions](#supported-elasticsearch-versions)
     - [Supported Python versions](#supported-python-versions)
 - [📖 Usage](#usage)
     - [Define a model](#define-a-model)
         - [Python basic types](#python-basic-types)
         - [ESORM field types](#esorm-field-types)
         - [Nested documents](#nested-documents)
+        - [ESBaseModel](#esbasemodel)
         - [Id field](#id-field)
         - [Model Settings](#model-settings)
         - [Describe fields](#describe-fields)
         - [ESModelTimestamp](#esmodeltimestamp)
     - [Connecting to ElasticSearch](#connecting-to-elasticsearch)
         - [Client](#client)
     - [Create index templates](#create-index-templates)
@@ -128,16 +129,19 @@
 
 <a id="usage"></a>
 ## 📖 Usage
 
 <a id="define-a-model"></a>
 ### Define a model
 
-You can use all [Pydantic](https://pydantic-docs.helpmanual.io/usage/models/) model features, because
-`ESModel` is a subclass of `pydantic.BaseModel`.
+You can use all [Pydantic](https://pydantic-docs.helpmanual.io/usage/models/) model features, because `ESModel` is a subclass of `pydantic.BaseModel`.
+(Actually it is a subclass of `ESBaseModel`, see more [below...](#esbasemodel))
+
+`ESModel` extends pydantic `BaseModel` with ElasticSearch specific features. It serializes and deserializes
+documents to and from ElasticSearch types and handle ElasticSearch operations in the background.
 
 <a id="python-basic-types"></a>
 #### Python basic types
 
 ```python
 from esorm import ESModel
 
@@ -190,14 +194,19 @@
 | `long` or `int64`         | `long`       |
 | `float16` or `half_float` | `half_float` |
 | `float32`                 | `float`      |
 | `double`                  | `double`     |
 | `boolean`                 | `boolean`    |
 | `geo_point`               | `geo_point`  |
 
+The `binary` field accepts **base64** encoded strings. However, if you provide `bytes` to it, they 
+will be automatically converted to a **base64** string during serialization. When you retrieve the 
+field, it will always be a **base64** encoded string. You can easily convert it back to bytes using 
+the `bytes()` method: `binary_field.bytes()`.
+
 <a id="nested-documents"></a>
 #### Nested documents
 
 ```python
 from esorm import ESModel
 from esorm.fields import keyword, text, byte
 
@@ -210,14 +219,40 @@
 
 class Post(ESModel):
     title: text
     content: text
     writer: User  # User is a nested document
 ```
 
+
+<a id="esbasemodel"></a>
+#### ESBaseModel
+
+`ESBaseModel` is the base of `ESModel`, also it is useful to use it for nested documents, 
+because by using it will not be included in the ElasticSearch index.
+
+```python
+from esorm import ESModel, ESBaseModel
+from esorm.fields import keyword, text, byte
+
+
+# This way `User` model won't be in the index
+class User(ESBaseModel):  # <---------------
+    name: text
+    email: keyword
+    age: byte = 18
+
+
+class Post(ESModel):
+    title: text
+    content: text
+    writer: User  # User is a nested document
+
+```  
+
 <a id="id-field"></a>
 #### Id field
 
 You can specify id field in [model settings](#model-settings):
 
 ```python
 from esorm import ESModel
```

### Comparing `pyesorm-0.3.0/README.md` & `pyesorm-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     - [Supported ElasticSearch versions](#supported-elasticsearch-versions)
     - [Supported Python versions](#supported-python-versions)
 - [📖 Usage](#usage)
     - [Define a model](#define-a-model)
         - [Python basic types](#python-basic-types)
         - [ESORM field types](#esorm-field-types)
         - [Nested documents](#nested-documents)
+        - [ESBaseModel](#esbasemodel)
         - [Id field](#id-field)
         - [Model Settings](#model-settings)
         - [Describe fields](#describe-fields)
         - [ESModelTimestamp](#esmodeltimestamp)
     - [Connecting to ElasticSearch](#connecting-to-elasticsearch)
         - [Client](#client)
     - [Create index templates](#create-index-templates)
@@ -89,16 +90,19 @@
 
 <a id="usage"></a>
 ## 📖 Usage
 
 <a id="define-a-model"></a>
 ### Define a model
 
-You can use all [Pydantic](https://pydantic-docs.helpmanual.io/usage/models/) model features, because
-`ESModel` is a subclass of `pydantic.BaseModel`.
+You can use all [Pydantic](https://pydantic-docs.helpmanual.io/usage/models/) model features, because `ESModel` is a subclass of `pydantic.BaseModel`.
+(Actually it is a subclass of `ESBaseModel`, see more [below...](#esbasemodel))
+
+`ESModel` extends pydantic `BaseModel` with ElasticSearch specific features. It serializes and deserializes
+documents to and from ElasticSearch types and handle ElasticSearch operations in the background.
 
 <a id="python-basic-types"></a>
 #### Python basic types
 
 ```python
 from esorm import ESModel
 
@@ -151,14 +155,19 @@
 | `long` or `int64`         | `long`       |
 | `float16` or `half_float` | `half_float` |
 | `float32`                 | `float`      |
 | `double`                  | `double`     |
 | `boolean`                 | `boolean`    |
 | `geo_point`               | `geo_point`  |
 
+The `binary` field accepts **base64** encoded strings. However, if you provide `bytes` to it, they 
+will be automatically converted to a **base64** string during serialization. When you retrieve the 
+field, it will always be a **base64** encoded string. You can easily convert it back to bytes using 
+the `bytes()` method: `binary_field.bytes()`.
+
 <a id="nested-documents"></a>
 #### Nested documents
 
 ```python
 from esorm import ESModel
 from esorm.fields import keyword, text, byte
 
@@ -171,14 +180,40 @@
 
 class Post(ESModel):
     title: text
     content: text
     writer: User  # User is a nested document
 ```
 
+
+<a id="esbasemodel"></a>
+#### ESBaseModel
+
+`ESBaseModel` is the base of `ESModel`, also it is useful to use it for nested documents, 
+because by using it will not be included in the ElasticSearch index.
+
+```python
+from esorm import ESModel, ESBaseModel
+from esorm.fields import keyword, text, byte
+
+
+# This way `User` model won't be in the index
+class User(ESBaseModel):  # <---------------
+    name: text
+    email: keyword
+    age: byte = 18
+
+
+class Post(ESModel):
+    title: text
+    content: text
+    writer: User  # User is a nested document
+
+```  
+
 <a id="id-field"></a>
 #### Id field
 
 You can specify id field in [model settings](#model-settings):
 
 ```python
 from esorm import ESModel
```

### Comparing `pyesorm-0.3.0/docs/changelog.py` & `pyesorm-0.3.1/docs/changelog.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.0/docs/conf.py` & `pyesorm-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.0/esorm/aggs.py` & `pyesorm-0.3.1/esorm/aggs.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.0/esorm/bulk.py` & `pyesorm-0.3.1/esorm/bulk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Bulk operation for ElasticSearch
 """
-from datetime import datetime
+from datetime import datetime, UTC
 
 from .model import TModel, ESModelTimestamp
 from .esorm import es
 
 
 class ESBulk:
     """
@@ -47,15 +47,15 @@
             '_id': model.__id__
         }
         routing = model.__routing__
         if routing is not None:
             index['routing'] = routing
 
         if isinstance(model, ESModelTimestamp):
-            document['modified_at'] = datetime.utcnow()
+            document['modified_at'] = datetime.now(UTC)
 
         self._actions.append({'index': index, })
         self._actions.append(document)
 
     async def delete(self, model: TModel):
         """
         Add the model to the bulk for deletion
```

### Comparing `pyesorm-0.3.0/esorm/esorm.py` & `pyesorm-0.3.1/esorm/esorm.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.0/esorm/fastapi.py` & `pyesorm-0.3.1/esorm/fastapi.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.0/esorm/fields.py` & `pyesorm-0.3.1/esorm/fields.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.0/esorm/model.py` & `pyesorm-0.3.1/esorm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,28 +14,31 @@
 from datetime import datetime, date, time
 from functools import wraps
 
 import elasticsearch
 from elasticsearch import NotFoundError as ElasticNotFoundError
 from pydantic import main as pydantic_main
 from pydantic import BaseModel, ConfigDict
-from pydantic.fields import Field, FieldInfo, PrivateAttr
+from pydantic.fields import Field, PrivateAttr
+# noinspection PyProtectedMember
+from pydantic.fields import FieldInfo  # It is just not in __all__ of pydantic.fields, but we strongly need it
 
 from .utils import snake_case, utcnow
 from .aggs import ESAggs, ESAggsResponse
 
 from .error import InvalidResponseError, NotFoundError
 from .esorm import es
 from .query import ESQuery
 from .response import ESResponse
 
 from .logger import logger
 
 __all__ = [
     'TModel',
+    'ESBaseModel',
     'ESModel',
     'ESModelTimestamp',
     'Pagination', 'Sort',
     'setup_mappings',
     'create_index_template',
     'set_default_index_prefix',
     'set_max_lazy_property_concurrency',
@@ -194,15 +197,32 @@
                 if isinstance(attr, property) and hasattr(attr.fget, '__lazy_property__'):
                     # noinspection PyProtectedMember
                     model.ESConfig._lazy_properties[attr_name] = getattr(attr.fget, '__lazy_property__')
 
         return model
 
 
-class ESModel(BaseModel, metaclass=_ESModelMeta):
+class ESBaseModel(BaseModel):
+    """
+    Base class for Elastic
+
+    It is useful for nested models, if you don't need the model in ES mappings
+    """
+
+    model_config = ConfigDict(
+        str_strip_whitespace=True,
+        extra="forbid",
+        populate_by_name=True,
+        arbitrary_types_allowed=True,
+        ser_json_bytes='base64',
+        validate_assignment=True,
+    )
+
+
+class ESModel(ESBaseModel, metaclass=_ESModelMeta):
     """
     ElasticSearch Base Model
     """
 
     _id: Optional[str] = PrivateAttr(None)
     """ The ES id of the document """
 
@@ -225,24 +245,14 @@
 
         lazy_property_max_recursion_depth: int = 1
         """ Maximum recursion depth of lazy properties """
 
         _lazy_properties: Dict[str, Callable[[], Awaitable[Any]]] = {}
         """ Lazy property async function definitions """
 
-    # Pydantic model config
-    model_config = ConfigDict(
-        str_strip_whitespace=True,
-        extra="forbid",
-        populate_by_name=True,
-        arbitrary_types_allowed=True,
-        ser_json_bytes='base64',
-        validate_assignment=True,
-    )
-
     @property
     def __id__(self) -> str:
         """
         The id of the document
 
         This can be overridden to make computed ids
```

### Comparing `pyesorm-0.3.0/esorm/query.py` & `pyesorm-0.3.1/esorm/query.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.0/esorm/response.py` & `pyesorm-0.3.1/esorm/response.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.0/esorm/utils.py` & `pyesorm-0.3.1/esorm/utils.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.0/esorm/watcher.py` & `pyesorm-0.3.1/esorm/watcher.py`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.0/pyesorm.egg-info/PKG-INFO` & `pyesorm-0.3.1/pyesorm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesorm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python ElasticSearch ORM based on Pydantic
 Home-page: https://github.com/wallneradam/esorm
 Author: Adam Wallner
 Author-email: Adam.wallner@gmail.com
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/wallneradam/esorm/issues
 Project-URL: Documentation, https://esorm.readthedocs.io/en/latest/
@@ -22,15 +22,15 @@
 License-File: LICENSE
 Requires-Dist: typing-extensions>=4.8.0
 Requires-Dist: elasticsearch<9.0.0,>=8.6.0
 Requires-Dist: aiohttp<4.0.0,>=3.0.0
 Requires-Dist: pydantic>=2.1.0
 Provides-Extra: dev
 Requires-Dist: fastapi; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest==8.0.2; extra == "dev"
 Requires-Dist: pytest-asyncio==0.21.1; extra == "dev"
 Requires-Dist: pytest-spec; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "dev"
 Requires-Dist: sphinx-rtd-dark-mode==1.3.0; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints; extra == "dev"
@@ -52,14 +52,15 @@
     - [Supported ElasticSearch versions](#supported-elasticsearch-versions)
     - [Supported Python versions](#supported-python-versions)
 - [📖 Usage](#usage)
     - [Define a model](#define-a-model)
         - [Python basic types](#python-basic-types)
         - [ESORM field types](#esorm-field-types)
         - [Nested documents](#nested-documents)
+        - [ESBaseModel](#esbasemodel)
         - [Id field](#id-field)
         - [Model Settings](#model-settings)
         - [Describe fields](#describe-fields)
         - [ESModelTimestamp](#esmodeltimestamp)
     - [Connecting to ElasticSearch](#connecting-to-elasticsearch)
         - [Client](#client)
     - [Create index templates](#create-index-templates)
@@ -128,16 +129,19 @@
 
 <a id="usage"></a>
 ## 📖 Usage
 
 <a id="define-a-model"></a>
 ### Define a model
 
-You can use all [Pydantic](https://pydantic-docs.helpmanual.io/usage/models/) model features, because
-`ESModel` is a subclass of `pydantic.BaseModel`.
+You can use all [Pydantic](https://pydantic-docs.helpmanual.io/usage/models/) model features, because `ESModel` is a subclass of `pydantic.BaseModel`.
+(Actually it is a subclass of `ESBaseModel`, see more [below...](#esbasemodel))
+
+`ESModel` extends pydantic `BaseModel` with ElasticSearch specific features. It serializes and deserializes
+documents to and from ElasticSearch types and handle ElasticSearch operations in the background.
 
 <a id="python-basic-types"></a>
 #### Python basic types
 
 ```python
 from esorm import ESModel
 
@@ -190,14 +194,19 @@
 | `long` or `int64`         | `long`       |
 | `float16` or `half_float` | `half_float` |
 | `float32`                 | `float`      |
 | `double`                  | `double`     |
 | `boolean`                 | `boolean`    |
 | `geo_point`               | `geo_point`  |
 
+The `binary` field accepts **base64** encoded strings. However, if you provide `bytes` to it, they 
+will be automatically converted to a **base64** string during serialization. When you retrieve the 
+field, it will always be a **base64** encoded string. You can easily convert it back to bytes using 
+the `bytes()` method: `binary_field.bytes()`.
+
 <a id="nested-documents"></a>
 #### Nested documents
 
 ```python
 from esorm import ESModel
 from esorm.fields import keyword, text, byte
 
@@ -210,14 +219,40 @@
 
 class Post(ESModel):
     title: text
     content: text
     writer: User  # User is a nested document
 ```
 
+
+<a id="esbasemodel"></a>
+#### ESBaseModel
+
+`ESBaseModel` is the base of `ESModel`, also it is useful to use it for nested documents, 
+because by using it will not be included in the ElasticSearch index.
+
+```python
+from esorm import ESModel, ESBaseModel
+from esorm.fields import keyword, text, byte
+
+
+# This way `User` model won't be in the index
+class User(ESBaseModel):  # <---------------
+    name: text
+    email: keyword
+    age: byte = 18
+
+
+class Post(ESModel):
+    title: text
+    content: text
+    writer: User  # User is a nested document
+
+```  
+
 <a id="id-field"></a>
 #### Id field
 
 You can specify id field in [model settings](#model-settings):
 
 ```python
 from esorm import ESModel
```

### Comparing `pyesorm-0.3.0/pyesorm.egg-info/SOURCES.txt` & `pyesorm-0.3.1/pyesorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyesorm-0.3.0/setup.cfg` & `pyesorm-0.3.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyesorm
-version = 0.3.0
+version = 0.3.1
 author = Adam Wallner
 author_email = Adam.wallner@gmail.com
 description = Python ElasticSearch ORM based on Pydantic
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = ElasticSearch, ORM, Pydantic
 license = MPL-2.0
@@ -30,15 +30,15 @@
 	elasticsearch>=8.6.0, <9.0.0
 	aiohttp>=3.0.0, <4.0.0
 	pydantic>=2.1.0
 
 [options.extras_require]
 dev = 
 	fastapi
-	pytest
+	pytest == 8.0.2
 	pytest-asyncio == 0.21.1
 	pytest-spec
 	pytest-timeout
 	sphinx
 	sphinx-rtd-theme == 1.3.0
 	sphinx-rtd-dark-mode == 1.3.0
 	sphinx-autodoc-typehints
```

### Comparing `pyesorm-0.3.0/tests/conftest.py` & `pyesorm-0.3.1/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import List
+from typing import List, Optional
 
 import sys
 import os
 import asyncio
-import pytest
 import subprocess
 import importlib
 
+import pytest
 import logging
 
 logger = logging.getLogger(__name__)
 disable_loggers = ['elastic_transport.node_pool', 'elastic_transport.transport']
 
 
 #
@@ -23,15 +23,17 @@
 
 
 @pytest.fixture(scope="class")
 def event_loop():
     """
     Use asyncio event loop in class scope
     """
-    return asyncio.get_event_loop()
+    loop = asyncio.get_event_loop()
+    yield loop
+    loop.close()
 
 
 #
 # Fixtures
 #
 
 # noinspection PyProtectedMember
@@ -48,15 +50,15 @@
     yield esorm
     for module_name in list(sys.modules):
         if module_name.startswith('esorm'):
             del sys.modules[module_name]
 
 
 @pytest.fixture(scope="class")  # Test both ES 8.x and 7.x
-async def docker_es(service):
+def docker_es(service):
     compose_file = os.path.join(os.path.dirname(__file__), 'docker-compose.yml')
     res = subprocess.run(['docker', 'compose', '-f', compose_file, 'up', '-d', service], check=True)
     logger.info(f"Started service: {service}")
     assert res.returncode == 0
     yield
     subprocess.run(['docker', 'compose', '-f', compose_file, 'down', service, '-v'], check=True)
     logger.info(f"Stopped service: {service}")
@@ -68,15 +70,14 @@
     """
     ElasticSearch fixture for version 8.x
     """
     es = await esorm.connect(hosts=["http://localhost:9200"], wait=True)
     assert es is not None
     yield es
     await es.close()
-    assert es
 
 
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_python(esorm):
     """
     Model to test python types
@@ -101,16 +102,14 @@
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_es(esorm):
     """
     Model to test ES types
     """
 
-    from datetime import datetime, date, time
-
     class ESFieldModel(esorm.ESModel):
         f_keyword: esorm.fields.keyword
         f_text: esorm.fields.text
         f_binary: esorm.fields.binary
         f_byte: esorm.fields.byte
         f_short: esorm.fields.short
         f_int32: esorm.fields.int32
@@ -121,14 +120,38 @@
         f_geo_point: esorm.fields.geo_point
 
     yield ESFieldModel
 
     del ESFieldModel
 
 
+@pytest.fixture(scope="class")
+def model_es_optional(esorm):
+    """
+    Model to test optional ES types
+    """
+
+    class ESOptionalFieldModel(esorm.ESModel):
+        f_keyword: Optional[esorm.fields.keyword] = None
+        f_text: Optional[esorm.fields.text] = None
+        f_binary: Optional[esorm.fields.binary] = esorm.Field(None, index=False)
+        f_byte: Optional[esorm.fields.byte] = None
+        f_short: Optional[esorm.fields.short] = None
+        f_int32: Optional[esorm.fields.int32] = None
+        f_long: Optional[esorm.fields.long] = None
+        f_float16: Optional[esorm.fields.float16] = None
+        f_float32: Optional[esorm.fields.float32] = None
+        f_double: Optional[esorm.fields.double] = None
+        f_geo_point: Optional[esorm.fields.geo_point] = None
+
+    yield ESOptionalFieldModel
+
+    del ESOptionalFieldModel
+
+
 # noinspection PyUnresolvedReferences
 @pytest.fixture(scope="class")
 def model_timestamp(esorm):
     """
     Model to test timestamp
     """
 
@@ -223,7 +246,28 @@
         @esorm.lazy_property
         async def same_f_strs(self) -> List['LazyPropModel']:
             return await self.search_by_fields({'f_str': self.f_str})
 
     yield LazyPropModel
 
     del LazyPropModel
+
+
+# noinspection PyUnresolvedReferences
+@pytest.fixture(scope="class")
+async def model_nested_binary(esorm):
+    """
+    Model to test nested binary fields
+    """
+    from pydantic import BaseModel
+
+    class BinaryModel(esorm.ESBaseModel):
+        f_binary: Optional[esorm.fields.binary] = esorm.Field(None, index=False)
+
+    class NestedBinaryModel(esorm.ESModel):
+        f_nested: BinaryModel
+
+    await esorm.setup_mappings()
+
+    yield BinaryModel, NestedBinaryModel
+    del BinaryModel
+    del NestedBinaryModel
```

### Comparing `pyesorm-0.3.0/tests/test_esorm.py` & `pyesorm-0.3.1/tests/test_esorm.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,21 @@
     async def test_create_model_with_es_fields(self, es, esorm, model_es):
         """
         Test model with ES fields
         """
         assert model_es is not None
         assert model_es.ESConfig.index == 'esorm-es_field_model'
 
+    async def test_create_model_with_es_optional_fields(self, es, esorm, model_es_optional):
+        """
+        Test model with ES fields
+        """
+        assert model_es_optional is not None
+        assert model_es_optional.ESConfig.index == 'esorm-es_optional_field_model'
+
     async def test_create_timestamp_models(self, es, esorm, model_timestamp):
         """
         Test timestamp models
         """
         assert model_timestamp is not None
         assert model_timestamp.ESConfig.index == 'esorm-timestamp_model'
         assert 'created_at' in model_timestamp.model_fields
@@ -57,16 +64,17 @@
     async def test_create_nested_model(self, es, esorm, model_nested):
         """
         Test nested model
         """
         assert model_nested is not None
         assert model_nested.ESConfig.index == 'esorm-nested_field_model'
 
-    async def test_create_mappings(self, es, esorm, model_python, model_es, model_timestamp,
-                                   model_config, model_with_id, model_nested, model_lazy_prop):
+    async def test_create_mappings(self, es, esorm, model_python, model_es, model_es_optional,
+                                   model_timestamp, model_config, model_with_id, model_nested,
+                                   model_lazy_prop):
         """
         Test create mappings
         """
         await esorm.setup_mappings()
         # Check if index exists
         assert await es.indices.exists(index=model_python.ESConfig.index)
 
@@ -88,14 +96,28 @@
         assert mappings[model_es.ESConfig.index]['mappings']['properties']['f_short']['type'] == 'short'
         assert mappings[model_es.ESConfig.index]['mappings']['properties']['f_int32']['type'] == 'integer'
         assert mappings[model_es.ESConfig.index]['mappings']['properties']['f_long']['type'] == 'long'
         assert mappings[model_es.ESConfig.index]['mappings']['properties']['f_float16']['type'] == 'half_float'
         assert mappings[model_es.ESConfig.index]['mappings']['properties']['f_float32']['type'] == 'float'
         assert mappings[model_es.ESConfig.index]['mappings']['properties']['f_double']['type'] == 'double'
         assert mappings[model_es.ESConfig.index]['mappings']['properties']['f_geo_point']['type'] == 'geo_point'
+        # Check if mappings are correct for ES Optional fields
+        mappings = await es.indices.get_mapping(index=model_es_optional.ESConfig.index)
+        assert mappings[model_es_optional.ESConfig.index]['mappings']['properties']['f_keyword']['type'] == 'keyword'
+        assert mappings[model_es_optional.ESConfig.index]['mappings']['properties']['f_text']['type'] == 'text'
+        assert mappings[model_es_optional.ESConfig.index]['mappings']['properties']['f_binary']['type'] == 'binary'
+        assert mappings[model_es_optional.ESConfig.index]['mappings']['properties']['f_byte']['type'] == 'byte'
+        assert mappings[model_es_optional.ESConfig.index]['mappings']['properties']['f_short']['type'] == 'short'
+        assert mappings[model_es_optional.ESConfig.index]['mappings']['properties']['f_int32']['type'] == 'integer'
+        assert mappings[model_es_optional.ESConfig.index]['mappings']['properties']['f_long']['type'] == 'long'
+        assert mappings[model_es_optional.ESConfig.index]['mappings']['properties']['f_float16']['type'] == 'half_float'
+        assert mappings[model_es_optional.ESConfig.index]['mappings']['properties']['f_float32']['type'] == 'float'
+        assert mappings[model_es_optional.ESConfig.index]['mappings']['properties']['f_double']['type'] == 'double'
+        assert mappings[model_es_optional.ESConfig.index]['mappings']['properties']['f_geo_point'][
+                   'type'] == 'geo_point'
         # Check if mappings are correct for timestamp fields
         mappings = await es.indices.get_mapping(index=model_timestamp.ESConfig.index)
         assert mappings[model_timestamp.ESConfig.index]['mappings']['properties']['created_at']['type'] == 'date'
         assert mappings[model_timestamp.ESConfig.index]['mappings']['properties']['modified_at']['type'] == 'date'
 
         # Check if mappings are correct for model with config
         mappings = await es.indices.get_mapping(index=model_config.ESConfig.index)
@@ -520,7 +542,34 @@
                 }
             }
         }
         doc = await model_config.search_one(query)
         assert doc is not None
         assert doc._id == doc_id == "test3"
         assert doc._routing == "test3__routing__"
+
+    async def test_binary(self, es, esorm, model_es_optional):
+        """
+        Test binary fields
+        """
+        doc = model_es_optional(f_binary=b'\x01\x02\x03\x04')
+        doc_id = await doc.save()
+
+        assert doc_id is not None
+        doc = await model_es_optional.get(doc_id)
+        assert getattr(doc.f_binary, 'bytes') == b'\x01\x02\x03\x04'
+
+        # Modify binary field
+        doc.f_binary = b'\x05\x06\x07\x08'
+        await doc.save()
+        doc = await model_es_optional.get(doc_id)
+        assert getattr(doc.f_binary, 'bytes') == b'\x05\x06\x07\x08'
+
+    async def test_binary_nested(self, es, esorm, model_nested_binary):
+        """
+        Test nested binary fields
+        """
+        binary_model, nested_binary_model = model_nested_binary
+        doc = nested_binary_model(f_nested=binary_model())
+        doc.f_nested.f_binary = b'\x01\x02\x03\x04'
+        doc_id = await doc.save()
+        assert doc_id is not None
```

