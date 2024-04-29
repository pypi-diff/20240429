# Comparing `tmp/trytond_stock_supply_forecast-7.0.0.tar.gz` & `tmp/trytond_stock_supply_forecast-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_supply_forecast-7.0.0.tar", last modified: Mon Oct 30 17:44:30 2023, max compression
+gzip compressed data, was "trytond_stock_supply_forecast-7.2.0.tar", last modified: Mon Apr 29 15:53:31 2024, max compression
```

## Comparing `trytond_stock_supply_forecast-7.0.0.tar` & `trytond_stock_supply_forecast-7.2.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:30.339630 trytond_stock_supply_forecast-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-10-22 17:23:28.000000 trytond_stock_supply_forecast-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2175 2023-10-30 17:15:52.000000 trytond_stock_supply_forecast-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:15:51.000000 trytond_stock_supply_forecast-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_supply_forecast-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2669 2023-10-30 17:44:30.339630 trytond_stock_supply_forecast-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      150 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:30.336297 trytond_stock_supply_forecast-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2023-10-22 17:23:28.000000 trytond_stock_supply_forecast-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      150 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:28.000000 trytond_stock_supply_forecast-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:44:30.339630 trytond_stock_supply_forecast-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4464 2023-10-27 17:38:49.000000 trytond_stock_supply_forecast-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.0.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:30.336297 trytond_stock_supply_forecast-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2897 2023-06-10 11:39:56.000000 trytond_stock_supply_forecast-7.0.0/tests/scenario_stock_supply_forecast.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_supply_forecast-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       75 2023-10-30 17:15:48.000000 trytond_stock_supply_forecast-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:30.339630 trytond_stock_supply_forecast-7.0.0/trytond_stock_supply_forecast.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2669 2023-10-30 17:44:29.000000 trytond_stock_supply_forecast-7.0.0/trytond_stock_supply_forecast.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      792 2023-10-30 17:44:30.000000 trytond_stock_supply_forecast-7.0.0/trytond_stock_supply_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:44:29.000000 trytond_stock_supply_forecast-7.0.0/trytond_stock_supply_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-10-30 17:44:29.000000 trytond_stock_supply_forecast-7.0.0/trytond_stock_supply_forecast.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_stock_supply_forecast-7.0.0/trytond_stock_supply_forecast.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      108 2023-10-30 17:44:29.000000 trytond_stock_supply_forecast-7.0.0/trytond_stock_supply_forecast.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:44:29.000000 trytond_stock_supply_forecast-7.0.0/trytond_stock_supply_forecast.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:31.828882 trytond_stock_supply_forecast-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2276 2024-04-29 15:29:30.000000 trytond_stock_supply_forecast-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:29:30.000000 trytond_stock_supply_forecast-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_supply_forecast-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2669 2024-04-29 15:53:31.828882 trytond_stock_supply_forecast-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      150 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:31.825549 trytond_stock_supply_forecast-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-27 16:30:39.000000 trytond_stock_supply_forecast-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      150 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:37.000000 trytond_stock_supply_forecast-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:53:31.828882 trytond_stock_supply_forecast-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4464 2024-03-17 11:01:36.000000 trytond_stock_supply_forecast-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:31.825549 trytond_stock_supply_forecast-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2886 2024-04-22 12:14:37.000000 trytond_stock_supply_forecast-7.2.0/tests/scenario_stock_supply_forecast.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:37.000000 trytond_stock_supply_forecast-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       75 2024-04-29 15:29:26.000000 trytond_stock_supply_forecast-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:31.825549 trytond_stock_supply_forecast-7.2.0/trytond_stock_supply_forecast.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2669 2024-04-29 15:53:31.000000 trytond_stock_supply_forecast-7.2.0/trytond_stock_supply_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      774 2024-04-29 15:53:31.000000 trytond_stock_supply_forecast-7.2.0/trytond_stock_supply_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:53:31.000000 trytond_stock_supply_forecast-7.2.0/trytond_stock_supply_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:53:31.000000 trytond_stock_supply_forecast-7.2.0/trytond_stock_supply_forecast.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_stock_supply_forecast-7.2.0/trytond_stock_supply_forecast.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      108 2024-04-29 15:53:31.000000 trytond_stock_supply_forecast-7.2.0/trytond_stock_supply_forecast.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:53:31.000000 trytond_stock_supply_forecast-7.2.0/trytond_stock_supply_forecast.egg-info/top_level.txt
```

### Comparing `trytond_stock_supply_forecast-7.0.0/CHANGELOG` & `trytond_stock_supply_forecast-7.2.0/CHANGELOG`

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

### Comparing `trytond_stock_supply_forecast-7.0.0/COPYRIGHT` & `trytond_stock_supply_forecast-7.2.0/COPYRIGHT`

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

### Comparing `trytond_stock_supply_forecast-7.0.0/LICENSE` & `trytond_stock_supply_forecast-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_forecast-7.0.0/PKG-INFO` & `trytond_stock_supply_forecast-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_supply_forecast
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add forecast to supply computation
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
@@ -48,18 +48,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_stock_supply<7.1,>=7.0
-Requires-Dist: trytond_stock_forecast<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_stock_supply<7.3,>=7.2
+Requires-Dist: trytond_stock_forecast<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Stock Supply Forecast Module
 ############################
 
 The stock supply forecast module takes forecast into account to compute
 purchase requests.
```

### Comparing `trytond_stock_supply_forecast-7.0.0/doc/conf.py` & `trytond_stock_supply_forecast-7.2.0/doc/conf.py`

 * *Files 3% similar despite different names*

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

### Comparing `trytond_stock_supply_forecast-7.0.0/setup.py` & `trytond_stock_supply_forecast-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_forecast-7.0.0/stock.py` & `trytond_stock_supply_forecast-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_forecast-7.0.0/tests/scenario_stock_supply_forecast.rst` & `trytond_stock_supply_forecast-7.2.0/tests/scenario_stock_supply_forecast.rst`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Stock Supply Forecast Scenario
 ==============================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import (create_chart,
-    ...     get_accounts)
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+
     >>> today = dt.date.today()
     >>> yesterday = today - dt.timedelta(days=1)
     >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock_supply_forecast')
@@ -90,11 +90,10 @@
 
 There is a draft purchase request after confirming the forecast::
 
     >>> forecast.click('confirm')
     >>> create_pr = Wizard('stock.supply')
     >>> create_pr.execute('create_')
     >>> pr, = PurchaseRequest.find([('state', '=', 'draft')])
-    >>> pr.product == product
-    True
+    >>> assertEqual(pr.product, product)
     >>> pr.quantity
     10.0
```

### Comparing `trytond_stock_supply_forecast-7.0.0/tox.ini` & `trytond_stock_supply_forecast-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_forecast-7.0.0/trytond_stock_supply_forecast.egg-info/PKG-INFO` & `trytond_stock_supply_forecast-7.2.0/trytond_stock_supply_forecast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-stock-supply-forecast
-Version: 7.0.0
+Name: trytond_stock_supply_forecast
+Version: 7.2.0
 Summary: Tryton module to add forecast to supply computation
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
@@ -48,18 +48,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_stock_supply<7.1,>=7.0
-Requires-Dist: trytond_stock_forecast<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_stock_supply<7.3,>=7.2
+Requires-Dist: trytond_stock_forecast<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Stock Supply Forecast Module
 ############################
 
 The stock supply forecast module takes forecast into account to compute
 purchase requests.
```

### Comparing `trytond_stock_supply_forecast-7.0.0/trytond_stock_supply_forecast.egg-info/SOURCES.txt` & `trytond_stock_supply_forecast-7.2.0/trytond_stock_supply_forecast.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 setup.py
```

