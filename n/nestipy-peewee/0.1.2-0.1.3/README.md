# Comparing `tmp/nestipy_peewee-0.1.2.tar.gz` & `tmp/nestipy_peewee-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_peewee-0.1.2.tar", max compression
+gzip compressed data, was "nestipy_peewee-0.1.3.tar", max compression
```

## Comparing `nestipy_peewee-0.1.2.tar` & `nestipy_peewee-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_peewee-0.1.2/LICENSE
--rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_peewee-0.1.2/README.md
--rw-r--r--   0        0        0      464 2024-04-27 15:56:19.412957 nestipy_peewee-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      185 2024-04-27 07:50:37.316624 nestipy_peewee-0.1.2/src/nestipy_peewee/__init__.py
--rw-r--r--   0        0        0      500 2024-04-27 07:10:46.368156 nestipy_peewee-0.1.2/src/nestipy_peewee/peewee_builder.py
--rw-r--r--   0        0        0      402 2024-04-27 07:49:49.760614 nestipy_peewee-0.1.2/src/nestipy_peewee/peewee_decorator.py
--rw-r--r--   0        0        0       58 2024-04-27 06:47:04.319886 nestipy_peewee-0.1.2/src/nestipy_peewee/peewee_meta.py
--rw-r--r--   0        0        0     2327 2024-04-27 07:50:28.188622 nestipy_peewee-0.1.2/src/nestipy_peewee/peewee_module.py
--rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 nestipy_peewee-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_peewee-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_peewee-0.1.3/README.md
+-rw-r--r--   0        0        0      448 2024-04-29 11:56:24.899734 nestipy_peewee-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      185 2024-04-27 07:50:37.316624 nestipy_peewee-0.1.3/src/nestipy_peewee/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-29 10:45:37.648124 nestipy_peewee-0.1.3/src/nestipy_peewee/peewee_builder.py
+-rw-r--r--   0        0        0      410 2024-04-29 11:05:46.313907 nestipy_peewee-0.1.3/src/nestipy_peewee/peewee_decorator.py
+-rw-r--r--   0        0        0       58 2024-04-27 06:47:04.319886 nestipy_peewee-0.1.3/src/nestipy_peewee/peewee_meta.py
+-rw-r--r--   0        0        0     2327 2024-04-29 11:04:32.938907 nestipy_peewee-0.1.3/src/nestipy_peewee/peewee_module.py
+-rw-r--r--   0        0        0     2375 1970-01-01 00:00:00.000000 nestipy_peewee-0.1.3/PKG-INFO
```

### Comparing `nestipy_peewee-0.1.2/LICENSE` & `nestipy_peewee-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy_peewee-0.1.2/README.md` & `nestipy_peewee-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nestipy_peewee-0.1.2/src/nestipy_peewee/peewee_module.py` & `nestipy_peewee-0.1.3/src/nestipy_peewee/peewee_module.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import inspect
 from dataclasses import asdict
 from typing import Type
-
 from nestipy.common import Module
 from nestipy_dynamic_module import NestipyModule
 from nestipy_ioc import Inject
 from nestipy_metadata import Reflect
 from peewee import Model, Database, SqliteDatabase, MySQLDatabase, PostgresqlDatabase
 
 from .peewee_builder import ConfigurableModuleClass, PEEWEE_DB_CONFIG
@@ -35,15 +34,15 @@
         self._db.create_tables(self._peewee_models)
 
     async def on_shutdown(self):
         if not self._db.is_closed():
             self._db.close()
 
     @classmethod
-    def for_feature(cls, *models: Type):
+    def for_feature(cls, *models: Model):
         for m in models:
             if Reflect.get_metadata(m, PeeweeMetadata.ModelMeta, False) and m not in cls._models:
                 cls._models.append(m)
         return cls
 
     def _setup_model(self):
         db = self._db
```

### Comparing `nestipy_peewee-0.1.2/PKG-INFO` & `nestipy_peewee-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: nestipy-peewee
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: nestipy (>=0.2.0,<0.3.0)
-Requires-Dist: nestipy-dynamic-module (>=0.1.4,<0.2.0)
+Requires-Dist: nestipy (==0.2.7)
 Requires-Dist: peewee (>=3.17.3,<4.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a target="_blank"><img src="https://raw.githubusercontent.com/nestipy/nestipy/release-v1/nestipy.png" width="200" alt="Nestipy Logo" /></a></p>
 <p align="center">
     <a href="https://pypi.org/project/nestipy">
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: nestipy-peewee Version: 0.1.2 Summary: Author:
+Metadata-Version: 2.1 Name: nestipy-peewee Version: 0.1.3 Summary: Author:
 tsiresymila Author-email: tsiresymila@gmail.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: nestipy
-(>=0.2.0,<0.3.0) Requires-Dist: nestipy-dynamic-module (>=0.1.4,<0.2.0)
-Requires-Dist: peewee (>=3.17.3,<4.0.0) Description-Content-Type: text/markdown
+(==0.2.7) Requires-Dist: peewee (>=3.17.3,<4.0.0) Description-Content-Type:
+text/markdown
                                 [Nestipy Logo]
                           _[_V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_L_i_c_e_n_s_e_]
 ## Description
 Nestipy is a Python framework built on top of FastAPI that follows the modular
 architecture of NestJS
 Under the hood, Nestipy makes use of _F_a_s_t_A_P_I, but also provides compatibility
 with a wide range of other libraries, like _B_l_a_c_k_s_h_e_e_p, allowing for easy use of
```

