# Comparing `tmp/proteus-7.0.1.tar.gz` & `tmp/proteus-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus-7.0.1.tar", last modified: Mon Jan  1 12:05:37 2024, max compression
+gzip compressed data, was "proteus-7.2.0.tar", last modified: Mon Apr 29 15:55:08 2024, max compression
```

## Comparing `proteus-7.0.1.tar` & `proteus-7.2.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:05:37.020959 proteus-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      179 2023-10-30 17:06:38.000000 proteus-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     4573 2024-01-01 12:05:34.000000 proteus-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      694 2024-01-01 12:05:34.000000 proteus-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    42788 2023-10-30 17:06:38.000000 proteus-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)       81 2023-10-30 17:06:38.000000 proteus-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     5777 2024-01-01 12:05:37.020959 proteus-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4178 2023-10-30 17:06:39.000000 proteus-7.0.1/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:05:37.014293 proteus-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2256 2023-10-30 17:06:39.000000 proteus-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4178 2023-10-30 17:06:39.000000 proteus-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 proteus-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:39.000000 proteus-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:05:37.017626 proteus-7.0.1/proteus/
--rw-r--r--   0 ced       (1000) ced       (1000)    49431 2023-12-27 10:39:54.000000 proteus-7.0.1/proteus/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13340 2023-10-30 17:06:38.000000 proteus-7.0.1/proteus/config.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22081 2023-10-30 17:06:38.000000 proteus-7.0.1/proteus/pyson.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:05:37.017626 proteus-7.0.1/proteus/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-10-30 17:06:39.000000 proteus-7.0.1/proteus/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-10-30 17:06:39.000000 proteus-7.0.1/proteus/tests/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1484 2023-10-30 17:06:39.000000 proteus-7.0.1/proteus/tests/test_config.py
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2023-10-30 17:06:38.000000 proteus-7.0.1/proteus/tests/test_context.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12536 2023-10-30 17:06:39.000000 proteus-7.0.1/proteus/tests/test_model.py
--rw-r--r--   0 ced       (1000) ced       (1000)      800 2023-10-30 17:06:39.000000 proteus-7.0.1/proteus/tests/test_readme.py
--rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-10-30 17:06:38.000000 proteus-7.0.1/proteus/tests/test_report.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2150 2023-10-30 17:06:39.000000 proteus-7.0.1/proteus/tests/test_wizard.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-01 12:05:37.017626 proteus-7.0.1/proteus.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     5777 2024-01-01 12:05:36.000000 proteus-7.0.1/proteus.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      612 2024-01-01 12:05:36.000000 proteus-7.0.1/proteus.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-01-01 12:05:36.000000 proteus-7.0.1/proteus.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      106 2024-01-01 12:05:36.000000 proteus-7.0.1/proteus.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-01-01 12:05:36.000000 proteus-7.0.1/proteus.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:28.000000 proteus-7.0.1/proteus.egg-info/zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-01-01 12:05:37.020959 proteus-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2988 2023-10-30 17:06:39.000000 proteus-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-10-30 17:06:39.000000 proteus-7.0.1/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:08.353024 proteus-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4616 2024-04-29 15:30:47.000000 proteus-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      694 2024-04-29 15:30:47.000000 proteus-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    42788 2023-01-16 14:00:21.000000 proteus-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)       81 2023-04-15 07:12:15.000000 proteus-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     5799 2024-04-29 15:55:08.353024 proteus-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     4178 2023-04-15 07:12:15.000000 proteus-7.2.0/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:08.349691 proteus-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2223 2024-04-27 16:30:39.000000 proteus-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4178 2023-04-15 07:12:15.000000 proteus-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 proteus-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-02-04 18:51:27.000000 proteus-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:08.349691 proteus-7.2.0/proteus/
+-rw-r--r--   0 ced       (1000) ced       (1000)    49431 2024-04-29 15:30:43.000000 proteus-7.2.0/proteus/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13493 2024-04-27 16:30:39.000000 proteus-7.2.0/proteus/config.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22081 2024-02-04 18:51:27.000000 proteus-7.2.0/proteus/pyson.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:08.353024 proteus-7.2.0/proteus/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 proteus-7.2.0/proteus/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 proteus-7.2.0/proteus/tests/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1484 2023-04-15 07:12:15.000000 proteus-7.2.0/proteus/tests/test_config.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      564 2023-01-16 14:00:21.000000 proteus-7.2.0/proteus/tests/test_context.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12463 2024-04-27 16:30:39.000000 proteus-7.2.0/proteus/tests/test_model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      817 2024-04-22 12:14:37.000000 proteus-7.2.0/proteus/tests/test_readme.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      793 2023-04-15 07:12:15.000000 proteus-7.2.0/proteus/tests/test_report.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2150 2023-04-15 07:12:15.000000 proteus-7.2.0/proteus/tests/test_wizard.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:08.353024 proteus-7.2.0/proteus.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5799 2024-04-29 15:55:07.000000 proteus-7.2.0/proteus.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      594 2024-04-29 15:55:08.000000 proteus-7.2.0/proteus.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:55:07.000000 proteus-7.2.0/proteus.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      106 2024-04-29 15:55:07.000000 proteus-7.2.0/proteus.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:55:07.000000 proteus-7.2.0/proteus.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 proteus-7.2.0/proteus.egg-info/zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:55:08.353024 proteus-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3010 2024-04-27 16:30:39.000000 proteus-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2024-03-17 11:01:36.000000 proteus-7.2.0/tox.ini
```

### Comparing `proteus-7.0.1/CHANGELOG` & `proteus-7.2.0/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
-Version 7.0.1 - 2024-01-01
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
-
+* Add skip warning on trytond configuration
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 * Support PYSON comparison of timedelta
 * Support encoding timedelta into PYSON TimeDelta
```

### Comparing `proteus-7.0.1/COPYRIGHT` & `proteus-7.2.0/COPYRIGHT`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2010-2023 Cédric Krier.
-Copyright (C) 2010-2023 B2CK SPRL.
+Copyright (C) 2010-2024 Cédric Krier.
+Copyright (C) 2010-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `proteus-7.0.1/LICENSE` & `proteus-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proteus-7.0.1/PKG-INFO` & `proteus-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: proteus
-Version: 7.0.1
+Version: 7.2.0
 Summary: Library to access Tryton server as a client
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: LGPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/
+Project-URL: Documentation, https://docs.tryton.org/latest/client-library/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton library cli
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
@@ -30,18 +30,18 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: defusedxml
 Requires-Dist: python-dateutil
 Provides-Extra: trytond
-Requires-Dist: trytond<7.1,>=7.0; extra == "trytond"
+Requires-Dist: trytond<7.3,>=7.2; extra == "trytond"
 Provides-Extra: test
-Requires-Dist: trytond<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_party<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_party<7.3,>=7.2; extra == "test"
 
 =======================
 Tryton Scripting Client
 =======================
 
 A library to access Tryton's models like a client.
```

### Comparing `proteus-7.0.1/README.rst` & `proteus-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `proteus-7.0.1/doc/conf.py` & `proteus-7.2.0/doc/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import os
 
 base_url = os.environ.get('DOC_BASE_URL')
 if base_url:
     modules_url = base_url + '/modules-{module}/'
     trytond_url = base_url + '/server/'
 else:
-    modules_url = (
-        'https://docs.tryton.org/projects/modules-{module}/en/{series}/')
-    trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
+    modules_url = 'https://docs.tryton.org/${series}/modules-{module}/'
+    trytond_url = 'https://docs.tryton.org/${series}/server/'
 
 
 def get_info():
     import subprocess
     import sys
 
     module_dir = os.path.dirname(os.path.dirname(__file__))
```

### Comparing `proteus-7.0.1/doc/index.rst` & `proteus-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `proteus-7.0.1/proteus/__init__.py` & `proteus-7.2.0/proteus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import datetime
 import functools
 import threading
 from decimal import Decimal
 
 import proteus.config
 
-__version__ = "7.0.1"
+__version__ = "7.2.0"
 __all__ = ['Model', 'Wizard', 'Report']
 
 _MODELS = threading.local()
 
 
 class _EvalEnvironment(dict):
     'Dictionary for evaluation'
```

### Comparing `proteus-7.0.1/proteus/config.py` & `proteus-7.2.0/proteus/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,16 @@
             with Transaction().start(self._config.database_name,
                     self._config.user, readonly=rpc.readonly,
                     **extras) as transaction:
                 try:
                     (c_args, c_kwargs,
                         transaction.context, transaction.timestamp) \
                             = rpc.convert(self._object, *args, **kwargs)
+                    if self._config.skip_warning:
+                        transaction.context['_skip_warnings'] = True
                     meth = getattr(self._object, self._name)
                     if (rpc.instantiate is None
                             or not is_instance_method(
                                 self._object, self._name)):
                         result = rpc.result(meth(*c_args, **c_kwargs))
                     else:
                         assert rpc.instantiate == 0
@@ -272,14 +274,15 @@
             uri = urllib.parse.urlparse(database)
             database_name = uri.path.strip('/')
         if not database_name:
             database_name = os.environ['DB_NAME']
         self.database_name = database_name
         self._user = user
         self.config_file = config_file
+        self.skip_warning = False
 
         Pool.start()
         self.pool = Pool(database_name)
         self.pool.init()
 
         with Transaction().start(self.database_name, 0) as transaction:
             User = self.pool.get('res.user')
```

### Comparing `proteus-7.0.1/proteus/pyson.py` & `proteus-7.2.0/proteus/pyson.py`

 * *Files identical despite different names*

### Comparing `proteus-7.0.1/proteus/tests/test_config.py` & `proteus-7.2.0/proteus/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `proteus-7.0.1/proteus/tests/test_context.py` & `proteus-7.2.0/proteus/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `proteus-7.0.1/proteus/tests/test_model.py` & `proteus-7.2.0/proteus/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,17 +192,16 @@
     def test_save_one2many(self):
         Group = Model.get('res.group')
         group = Group()
         group.name = 'Test save one2many'
         group.save()
 
         ModelAccess = Model.get('ir.model.access')
-        Model_ = Model.get('ir.model')
         model_access = ModelAccess()
-        model_access.model = Model_.find([('model', '=', 'res.group')])[0]
+        model_access.model = 'res.group'
         model_access.perm_read = True
         model_access.perm_write = True
         model_access.perm_create = True
         model_access.perm_delete = True
 
         group.model_access.append(model_access)
         group.save()
```

### Comparing `proteus-7.0.1/proteus/tests/test_readme.py` & `proteus-7.2.0/proteus/tests/test_readme.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,7 +16,8 @@
         tests.addTest(doctest.DocTestSuite(mod))
     if os.path.isfile(readme):
         tests.addTest(doctest.DocFileSuite(
                 readme, module_relative=False,
                 setUp=doctest_setup, tearDown=doctest_teardown,
                 encoding='utf-8',
                 optionflags=doctest.REPORT_ONLY_FIRST_FAILURE))
+    return tests
```

### Comparing `proteus-7.0.1/proteus/tests/test_report.py` & `proteus-7.2.0/proteus/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `proteus-7.0.1/proteus/tests/test_wizard.py` & `proteus-7.2.0/proteus/tests/test_wizard.py`

 * *Files identical despite different names*

### Comparing `proteus-7.0.1/proteus.egg-info/PKG-INFO` & `proteus-7.2.0/proteus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: proteus
-Version: 7.0.1
+Version: 7.2.0
 Summary: Library to access Tryton server as a client
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: LGPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/
+Project-URL: Documentation, https://docs.tryton.org/latest/client-library/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton library cli
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
@@ -30,18 +30,18 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: defusedxml
 Requires-Dist: python-dateutil
 Provides-Extra: trytond
-Requires-Dist: trytond<7.1,>=7.0; extra == "trytond"
+Requires-Dist: trytond<7.3,>=7.2; extra == "trytond"
 Provides-Extra: test
-Requires-Dist: trytond<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_party<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_party<7.3,>=7.2; extra == "test"
 
 =======================
 Tryton Scripting Client
 =======================
 
 A library to access Tryton's models like a client.
```

### Comparing `proteus-7.0.1/proteus.egg-info/SOURCES.txt` & `proteus-7.2.0/proteus.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
 tox.ini
```

### Comparing `proteus-7.0.1/setup.py` & `proteus-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     long_description=readme(),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/',
+        "Documentation": 'https://docs.tryton.org/latest/client-library/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton library cli',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

