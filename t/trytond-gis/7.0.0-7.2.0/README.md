# Comparing `tmp/trytond_gis-7.0.0.tar.gz` & `tmp/trytond_gis-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_gis-7.0.0.tar", last modified: Mon Oct 30 17:46:25 2023, max compression
+gzip compressed data, was "trytond_gis-7.2.0.tar", last modified: Mon Apr 29 15:55:34 2024, max compression
```

## Comparing `trytond_gis-7.0.0.tar` & `trytond_gis-7.2.0.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:46:25.673514 trytond_gis-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      187 2023-10-07 15:40:36.000000 trytond_gis-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1559 2023-10-30 17:17:23.000000 trytond_gis-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      723 2023-10-30 17:17:23.000000 trytond_gis-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_gis-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)       81 2023-04-15 07:12:15.000000 trytond_gis-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     1369 2023-10-30 17:46:25.670180 trytond_gis-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      179 2023-04-15 07:12:16.000000 trytond_gis-7.0.0/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:46:25.666847 trytond_gis-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2319 2023-10-07 15:40:36.000000 trytond_gis-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      179 2023-04-15 07:12:16.000000 trytond_gis-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_gis-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-07 15:40:36.000000 trytond_gis-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:46:25.673514 trytond_gis-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2788 2023-10-27 17:38:49.000000 trytond_gis-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      463 2023-10-27 17:38:49.000000 trytond_gis-7.0.0/tox.ini
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:46:25.670180 trytond_gis-7.0.0/trytond_gis/
--rw-r--r--   0 ced       (1000) ced       (1000)      557 2023-10-30 17:17:18.000000 trytond_gis-7.0.0/trytond_gis/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-01-16 14:00:21.000000 trytond_gis-7.0.0/trytond_gis/const.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2323 2023-08-13 15:26:13.000000 trytond_gis-7.0.0/trytond_gis/fields.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:46:25.670180 trytond_gis-7.0.0/trytond_gis/postgis/
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-15 07:12:16.000000 trytond_gis-7.0.0/trytond_gis/postgis/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2187 2023-04-15 07:12:16.000000 trytond_gis-7.0.0/trytond_gis/postgis/database.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2924 2023-04-15 07:12:16.000000 trytond_gis-7.0.0/trytond_gis/postgis/table.py
--rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-01-16 14:00:21.000000 trytond_gis-7.0.0/trytond_gis/sql.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:46:25.670180 trytond_gis-7.0.0/trytond_gis/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:15.000000 trytond_gis-7.0.0/trytond_gis/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-01-16 14:00:21.000000 trytond_gis-7.0.0/trytond_gis/tests/gis.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3330 2023-10-27 17:38:49.000000 trytond_gis-7.0.0/trytond_gis/tests/test_fields.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:46:25.670180 trytond_gis-7.0.0/trytond_gis.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     1369 2023-10-30 17:46:25.000000 trytond_gis-7.0.0/trytond_gis.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      666 2023-10-30 17:46:25.000000 trytond_gis-7.0.0/trytond_gis.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:46:25.000000 trytond_gis-7.0.0/trytond_gis.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      108 2023-10-30 17:46:25.000000 trytond_gis-7.0.0/trytond_gis.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond_gis-7.0.0/trytond_gis.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       42 2023-10-30 17:46:25.000000 trytond_gis-7.0.0/trytond_gis.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       12 2023-10-30 17:46:25.000000 trytond_gis-7.0.0/trytond_gis.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:34.305679 trytond_gis-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1660 2024-04-29 15:31:04.000000 trytond_gis-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      723 2024-04-29 15:31:04.000000 trytond_gis-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_gis-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)       81 2023-04-15 07:12:15.000000 trytond_gis-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     1368 2024-04-29 15:55:34.305679 trytond_gis-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      179 2023-04-15 07:12:16.000000 trytond_gis-7.2.0/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:34.305679 trytond_gis-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2286 2024-04-27 16:30:39.000000 trytond_gis-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      179 2023-04-15 07:12:16.000000 trytond_gis-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_gis-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-02-04 18:51:27.000000 trytond_gis-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:55:34.305679 trytond_gis-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     2787 2024-04-27 16:30:39.000000 trytond_gis-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      463 2024-03-17 11:01:36.000000 trytond_gis-7.2.0/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:34.305679 trytond_gis-7.2.0/trytond_gis/
+-rw-r--r--   0 ced       (1000) ced       (1000)      557 2024-04-29 15:31:00.000000 trytond_gis-7.2.0/trytond_gis/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-01-16 14:00:21.000000 trytond_gis-7.2.0/trytond_gis/const.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2323 2024-01-27 09:58:52.000000 trytond_gis-7.2.0/trytond_gis/fields.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:34.305679 trytond_gis-7.2.0/trytond_gis/postgis/
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2024-04-22 12:01:28.000000 trytond_gis-7.2.0/trytond_gis/postgis/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2292 2024-04-22 12:01:28.000000 trytond_gis-7.2.0/trytond_gis/postgis/database.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2924 2023-04-15 07:12:16.000000 trytond_gis-7.2.0/trytond_gis/postgis/table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      285 2023-01-16 14:00:21.000000 trytond_gis-7.2.0/trytond_gis/sql.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:34.305679 trytond_gis-7.2.0/trytond_gis/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:15.000000 trytond_gis-7.2.0/trytond_gis/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-01-16 14:00:21.000000 trytond_gis-7.2.0/trytond_gis/tests/gis.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3330 2024-03-17 11:01:36.000000 trytond_gis-7.2.0/trytond_gis/tests/test_fields.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:34.305679 trytond_gis-7.2.0/trytond_gis.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1368 2024-04-29 15:55:33.000000 trytond_gis-7.2.0/trytond_gis.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      648 2024-04-29 15:55:34.000000 trytond_gis-7.2.0/trytond_gis.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:55:33.000000 trytond_gis-7.2.0/trytond_gis.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      108 2024-04-29 15:55:33.000000 trytond_gis-7.2.0/trytond_gis.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond_gis-7.2.0/trytond_gis.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       42 2024-04-29 15:55:33.000000 trytond_gis-7.2.0/trytond_gis.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       12 2024-04-29 15:55:33.000000 trytond_gis-7.2.0/trytond_gis.egg-info/top_level.txt
```

### Comparing `trytond_gis-7.0.0/CHANGELOG` & `trytond_gis-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.2.0 - 2024-04-29
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 
 Version 6.8.0 - 2023-05-01
 --------------------------
```

### Comparing `trytond_gis-7.0.0/COPYRIGHT` & `trytond_gis-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (c) 2017-2023 B2CK.
-Copyright (c) 2017-2023 Cédric Krier.
+Copyright (c) 2017-2024 B2CK.
+Copyright (c) 2017-2024 Cédric Krier.
 Copyright (c) 2017-2023 Nicolas Évrard.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_gis-7.0.0/LICENSE` & `trytond_gis-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_gis-7.0.0/PKG-INFO` & `trytond_gis-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_gis
-Version: 7.0.0
+Version: 7.2.0
 Summary: Adds Geographic Information System support to trytond
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/backend-gis
+Project-URL: Documentation, https://docs.tryton.org/latest/backend-gis/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton GIS
 Platform: any
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: geomet
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Requires-Dist: psycopg2>=2.0.14
 
 Tryton GIS backend
 ==================
 
 It adds GIS__ support to Tryton.
```

### Comparing `trytond_gis-7.0.0/doc/conf.py` & `trytond_gis-7.2.0/doc/conf.py`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_gis-7.0.0/setup.py` & `trytond_gis-7.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     long_description=readme(),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/projects/backend-gis',
+        "Documentation": 'https://docs.tryton.org/latest/backend-gis/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton GIS',
     packages=find_packages(),
     classifiers=[
         'Framework :: Tryton',
```

### Comparing `trytond_gis-7.0.0/trytond_gis/__init__.py` & `trytond_gis-7.2.0/trytond_gis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is part of trytond_gis.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from trytond.config import config
 
 from .const import WGS_84
 
-__version__ = "7.0.0"
+__version__ = "7.2.0"
 
 
 class _GeoJSON(dict):
 
     def __init__(self, *args, **kwargs):
         super(_GeoJSON, self).__init__(*args, **kwargs)
         if 'meta' not in self:
```

### Comparing `trytond_gis-7.0.0/trytond_gis/fields.py` & `trytond_gis-7.2.0/trytond_gis/fields.py`

 * *Files identical despite different names*

### Comparing `trytond_gis-7.0.0/trytond_gis/postgis/database.py` & `trytond_gis-7.2.0/trytond_gis/postgis/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,16 +33,19 @@
     @classmethod
     def _connection_params(cls, name):
         params = super()._connection_params(name)
         uri = parse_uri(params['dsn'])
         params['dsn'] = uri._replace(scheme='postgresql').geturl()
         return params
 
-    def get_connection(self, autocommit=False, readonly=False):
-        conn = super(Database, self).get_connection(autocommit, readonly)
+    def get_connection(
+            self, autocommit=False, readonly=False, statement_timeout=None):
+        conn = super().get_connection(
+            autocommit=autocommit, readonly=readonly,
+            statement_timeout=statement_timeout)
 
         if self._GIS_OIDS is None:
             cursor = conn.cursor()
             cursor.execute(
                 "SELECT 1 FROM pg_extension WHERE extname='postgis'")
             if cursor.fetchone():
                 cursor.execute('SELECT NULL::geometry, NULL::geography')
```

### Comparing `trytond_gis-7.0.0/trytond_gis/postgis/table.py` & `trytond_gis-7.2.0/trytond_gis/postgis/table.py`

 * *Files identical despite different names*

### Comparing `trytond_gis-7.0.0/trytond_gis/tests/test_fields.py` & `trytond_gis-7.2.0/trytond_gis/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `trytond_gis-7.0.0/trytond_gis.egg-info/PKG-INFO` & `trytond_gis-7.2.0/trytond_gis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-gis
-Version: 7.0.0
+Name: trytond_gis
+Version: 7.2.0
 Summary: Adds Geographic Information System support to trytond
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/backend-gis
+Project-URL: Documentation, https://docs.tryton.org/latest/backend-gis/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton GIS
 Platform: any
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: geomet
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond<7.3,>=7.2
 Requires-Dist: psycopg2>=2.0.14
 
 Tryton GIS backend
 ==================
 
 It adds GIS__ support to Tryton.
```

### Comparing `trytond_gis-7.0.0/trytond_gis.egg-info/SOURCES.txt` & `trytond_gis-7.2.0/trytond_gis.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

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

