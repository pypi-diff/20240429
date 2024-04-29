# Comparing `tmp/trytond_sale_credit_limit-7.0.1.tar.gz` & `tmp/trytond_sale_credit_limit-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_credit_limit-7.0.1.tar", last modified: Mon Jan 15 23:18:38 2024, max compression
+gzip compressed data, was "trytond_sale_credit_limit-7.2.0.tar", last modified: Mon Apr 29 15:47:37 2024, max compression
```

## Comparing `trytond_sale_credit_limit-7.0.1.tar` & `trytond_sale_credit_limit-7.2.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:18:37.995261 trytond_sale_credit_limit-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-10-30 17:06:38.000000 trytond_sale_credit_limit-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1964 2024-01-15 23:18:35.000000 trytond_sale_credit_limit-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-01-15 23:18:35.000000 trytond_sale_credit_limit-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_credit_limit-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_credit_limit-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2778 2024-01-15 23:18:37.995261 trytond_sale_credit_limit-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-10-30 17:06:38.000000 trytond_sale_credit_limit-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-30 17:06:38.000000 trytond_sale_credit_limit-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:18:37.995261 trytond_sale_credit_limit-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-10-30 17:06:38.000000 trytond_sale_credit_limit-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-10-30 17:06:38.000000 trytond_sale_credit_limit-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_credit_limit-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2130 2023-10-30 17:06:38.000000 trytond_sale_credit_limit-7.0.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1682 2024-01-08 10:49:58.000000 trytond_sale_credit_limit-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-01-15 23:18:37.995261 trytond_sale_credit_limit-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4297 2023-10-30 17:06:38.000000 trytond_sale_credit_limit-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:18:37.995261 trytond_sale_credit_limit-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_credit_limit-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5189 2023-10-30 17:06:38.000000 trytond_sale_credit_limit-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_credit_limit-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      118 2023-10-30 17:55:12.000000 trytond_sale_credit_limit-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:18:37.995261 trytond_sale_credit_limit-7.0.1/trytond_sale_credit_limit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2778 2024-01-15 23:18:37.000000 trytond_sale_credit_limit-7.0.1/trytond_sale_credit_limit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      650 2024-01-15 23:18:37.000000 trytond_sale_credit_limit-7.0.1/trytond_sale_credit_limit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-01-15 23:18:37.000000 trytond_sale_credit_limit-7.0.1/trytond_sale_credit_limit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-01-15 23:18:37.000000 trytond_sale_credit_limit-7.0.1/trytond_sale_credit_limit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:05.000000 trytond_sale_credit_limit-7.0.1/trytond_sale_credit_limit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2024-01-15 23:18:37.000000 trytond_sale_credit_limit-7.0.1/trytond_sale_credit_limit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-01-15 23:18:37.000000 trytond_sale_credit_limit-7.0.1/trytond_sale_credit_limit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:37.321487 trytond_sale_credit_limit-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1964 2024-04-29 15:24:57.000000 trytond_sale_credit_limit-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:24:56.000000 trytond_sale_credit_limit-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_credit_limit-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_credit_limit-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2778 2024-04-29 15:47:37.321487 trytond_sale_credit_limit-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-04-15 07:12:15.000000 trytond_sale_credit_limit-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-01-27 09:58:52.000000 trytond_sale_credit_limit-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:37.318154 trytond_sale_credit_limit-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_sale_credit_limit-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-04-15 07:12:15.000000 trytond_sale_credit_limit-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:24.000000 trytond_sale_credit_limit-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2130 2024-03-17 11:01:36.000000 trytond_sale_credit_limit-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1682 2024-04-22 12:14:36.000000 trytond_sale_credit_limit-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:47:37.321487 trytond_sale_credit_limit-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4297 2024-03-17 11:01:36.000000 trytond_sale_credit_limit-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:37.318154 trytond_sale_credit_limit-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_credit_limit-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5189 2024-01-27 09:58:52.000000 trytond_sale_credit_limit-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:24.000000 trytond_sale_credit_limit-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      118 2024-04-29 15:24:52.000000 trytond_sale_credit_limit-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:37.321487 trytond_sale_credit_limit-7.2.0/trytond_sale_credit_limit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2778 2024-04-29 15:47:36.000000 trytond_sale_credit_limit-7.2.0/trytond_sale_credit_limit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      632 2024-04-29 15:47:37.000000 trytond_sale_credit_limit-7.2.0/trytond_sale_credit_limit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:47:36.000000 trytond_sale_credit_limit-7.2.0/trytond_sale_credit_limit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:47:36.000000 trytond_sale_credit_limit-7.2.0/trytond_sale_credit_limit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_sale_credit_limit-7.2.0/trytond_sale_credit_limit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      167 2024-04-29 15:47:36.000000 trytond_sale_credit_limit-7.2.0/trytond_sale_credit_limit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:47:36.000000 trytond_sale_credit_limit-7.2.0/trytond_sale_credit_limit.egg-info/top_level.txt
```

### Comparing `trytond_sale_credit_limit-7.0.1/CHANGELOG` & `trytond_sale_credit_limit-7.2.0/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-01-15
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_sale_credit_limit-7.0.1/COPYRIGHT` & `trytond_sale_credit_limit-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2011-2023 Cédric Krier.
-Copyright (C) 2011-2023 B2CK SPRL.
+Copyright (C) 2011-2024 Cédric Krier.
+Copyright (C) 2011-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_credit_limit-7.0.1/LICENSE` & `trytond_sale_credit_limit-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_credit_limit-7.0.1/PKG-INFO` & `trytond_sale_credit_limit-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_credit_limit
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for sale credit limit
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_credit_limit<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_credit_limit<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Sale Credit Limit
 #################
 
 The sale_credit_limit module adds confirmed sale but not yet invoiced to the
 "Credit Amount" of the Party and check the credit limit of the party when
 confirming a sale.
```

### Comparing `trytond_sale_credit_limit-7.0.1/doc/conf.py` & `trytond_sale_credit_limit-7.2.0/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 base_url = os.environ.get('DOC_BASE_URL')
 if base_url:
     modules_url = base_url + '/modules-{module}/'
     trytond_url = base_url + '/server/'
 else:
     modules_url = (
-        'https://docs.tryton.org/projects/modules-{module}/en/{series}/')
-    trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
+        'https://docs.tryton.org/${series}/modules-{module}/')
+    trytond_url = 'https://docs.tryton.org/${series}/server/'
 
 
 def get_info():
     import configparser
     import subprocess
     import sys
 
@@ -67,22 +67,33 @@
     }
 html_title = info['description']
 master_doc = 'index'
 project = info['name']
 release = version = info['series']
 default_role = 'ref'
 highlight_language = 'none'
+exclude_patterns = ['**/*.inc.rst']
 extensions = [
     'sphinx_copybutton',
     'sphinx.ext.intersphinx',
     ]
 intersphinx_mapping = {
     'trytond': (trytond_url.format(series=version), None),
     }
 intersphinx_mapping.update({
         m: (modules_url.format(
                 module=m.replace('_', '-'), series=version), None)
         for m in info['modules']
         })
 linkcheck_ignore = [r'/.*', r'https://demo.tryton.org/*']
 
+try:
+    with open(os.path.join(
+                os.path.dirname(__file__),
+                'linkcheck_ignore.json'), 'r') as f:
+        import json
+        linkcheck_ignore.extend(json.load(f))
+        del json
+except FileNotFoundError:
+    pass
+
 del get_info, info, base_url, modules_url, trytond_url
```

### Comparing `trytond_sale_credit_limit-7.0.1/party.py` & `trytond_sale_credit_limit-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_credit_limit-7.0.1/sale.py` & `trytond_sale_credit_limit-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_credit_limit-7.0.1/setup.py` & `trytond_sale_credit_limit-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_credit_limit-7.0.1/tests/test_module.py` & `trytond_sale_credit_limit-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_credit_limit-7.0.1/tox.ini` & `trytond_sale_credit_limit-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_credit_limit-7.0.1/trytond_sale_credit_limit.egg-info/PKG-INFO` & `trytond_sale_credit_limit-7.2.0/trytond_sale_credit_limit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-sale-credit-limit
-Version: 7.0.1
+Name: trytond_sale_credit_limit
+Version: 7.2.0
 Summary: Tryton module for sale credit limit
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_credit_limit<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_credit_limit<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Sale Credit Limit
 #################
 
 The sale_credit_limit module adds confirmed sale but not yet invoiced to the
 "Credit Amount" of the Party and check the credit limit of the party when
 confirming a sale.
```

### Comparing `trytond_sale_credit_limit-7.0.1/trytond_sale_credit_limit.egg-info/SOURCES.txt` & `trytond_sale_credit_limit-7.2.0/trytond_sale_credit_limit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 party.py
```

