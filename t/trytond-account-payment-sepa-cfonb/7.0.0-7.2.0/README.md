# Comparing `tmp/trytond_account_payment_sepa_cfonb-7.0.0.tar.gz` & `tmp/trytond_account_payment_sepa_cfonb-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_sepa_cfonb-7.0.0.tar", last modified: Mon Oct 30 17:23:34 2023, max compression
+gzip compressed data, was "trytond_account_payment_sepa_cfonb-7.2.0.tar", last modified: Mon Apr 29 15:35:09 2024, max compression
```

## Comparing `trytond_account_payment_sepa_cfonb-7.0.0.tar` & `trytond_account_payment_sepa_cfonb-7.2.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:34.500307 trytond_account_payment_sepa_cfonb-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-10-22 17:22:54.000000 trytond_account_payment_sepa_cfonb-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1608 2023-10-30 17:02:48.000000 trytond_account_payment_sepa_cfonb-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:02:47.000000 trytond_account_payment_sepa_cfonb-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment_sepa_cfonb-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2794 2023-10-30 17:23:34.500307 trytond_account_payment_sepa_cfonb-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:20.000000 trytond_account_payment_sepa_cfonb-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:34.500307 trytond_account_payment_sepa_cfonb-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2827 2023-10-22 17:22:54.000000 trytond_account_payment_sepa_cfonb-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:20.000000 trytond_account_payment_sepa_cfonb-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:54.000000 trytond_account_payment_sepa_cfonb-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1709 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.0.0/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:23:34.500307 trytond_account_payment_sepa_cfonb-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4550 2023-10-27 17:38:49.000000 trytond_account_payment_sepa_cfonb-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:34.496974 trytond_account_payment_sepa_cfonb-7.0.0/template/
--rw-r--r--   0 ced       (1000) ced       (1000)     2627 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.0.0/template/base-cfonb.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4052 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.0.0/template/pain.001.001.03-cfonb.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4729 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.0.0/template/pain.008.001.02-cfonb.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:34.500307 trytond_account_payment_sepa_cfonb-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      952 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_payment_sepa_cfonb-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      108 2023-10-30 17:02:44.000000 trytond_account_payment_sepa_cfonb-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:23:34.500307 trytond_account_payment_sepa_cfonb-7.0.0/trytond_account_payment_sepa_cfonb.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2794 2023-10-30 17:23:34.000000 trytond_account_payment_sepa_cfonb-7.0.0/trytond_account_payment_sepa_cfonb.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      893 2023-10-30 17:23:34.000000 trytond_account_payment_sepa_cfonb-7.0.0/trytond_account_payment_sepa_cfonb.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:23:34.000000 trytond_account_payment_sepa_cfonb-7.0.0/trytond_account_payment_sepa_cfonb.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:23:34.000000 trytond_account_payment_sepa_cfonb-7.0.0/trytond_account_payment_sepa_cfonb.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_account_payment_sepa_cfonb-7.0.0/trytond_account_payment_sepa_cfonb.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-10-30 17:23:34.000000 trytond_account_payment_sepa_cfonb-7.0.0/trytond_account_payment_sepa_cfonb.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:23:34.000000 trytond_account_payment_sepa_cfonb-7.0.0/trytond_account_payment_sepa_cfonb.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:09.417715 trytond_account_payment_sepa_cfonb-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1709 2024-04-29 15:15:24.000000 trytond_account_payment_sepa_cfonb-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:15:23.000000 trytond_account_payment_sepa_cfonb-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment_sepa_cfonb-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2794 2024-04-29 15:35:09.417715 trytond_account_payment_sepa_cfonb-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:20.000000 trytond_account_payment_sepa_cfonb-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:09.417715 trytond_account_payment_sepa_cfonb-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-27 16:30:39.000000 trytond_account_payment_sepa_cfonb-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:20.000000 trytond_account_payment_sepa_cfonb-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:57.000000 trytond_account_payment_sepa_cfonb-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1709 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.2.0/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:35:09.417715 trytond_account_payment_sepa_cfonb-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4550 2024-03-17 11:01:36.000000 trytond_account_payment_sepa_cfonb-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:09.417715 trytond_account_payment_sepa_cfonb-7.2.0/template/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2627 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.2.0/template/base-cfonb.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4052 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.2.0/template/pain.001.001.03-cfonb.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4729 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.2.0/template/pain.008.001.02-cfonb.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:09.417715 trytond_account_payment_sepa_cfonb-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      952 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:57.000000 trytond_account_payment_sepa_cfonb-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      108 2024-04-29 15:15:19.000000 trytond_account_payment_sepa_cfonb-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:09.417715 trytond_account_payment_sepa_cfonb-7.2.0/trytond_account_payment_sepa_cfonb.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2794 2024-04-29 15:35:08.000000 trytond_account_payment_sepa_cfonb-7.2.0/trytond_account_payment_sepa_cfonb.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      875 2024-04-29 15:35:09.000000 trytond_account_payment_sepa_cfonb-7.2.0/trytond_account_payment_sepa_cfonb.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:35:08.000000 trytond_account_payment_sepa_cfonb-7.2.0/trytond_account_payment_sepa_cfonb.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-29 15:35:08.000000 trytond_account_payment_sepa_cfonb-7.2.0/trytond_account_payment_sepa_cfonb.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_account_payment_sepa_cfonb-7.2.0/trytond_account_payment_sepa_cfonb.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-04-29 15:35:08.000000 trytond_account_payment_sepa_cfonb-7.2.0/trytond_account_payment_sepa_cfonb.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:35:08.000000 trytond_account_payment_sepa_cfonb-7.2.0/trytond_account_payment_sepa_cfonb.egg-info/top_level.txt
```

### Comparing `trytond_account_payment_sepa_cfonb-7.0.0/CHANGELOG` & `trytond_account_payment_sepa_cfonb-7.2.0/CHANGELOG`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_account_payment_sepa_cfonb-7.0.0/LICENSE` & `trytond_account_payment_sepa_cfonb-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-7.0.0/PKG-INFO` & `trytond_account_payment_sepa_cfonb-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_sepa_cfonb
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for CFONB SEPA payment
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
@@ -50,19 +50,19 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Genshi
 Requires-Dist: lxml
-Requires-Dist: trytond_account_payment<7.1,>=7.0
-Requires-Dist: trytond_account_payment_sepa<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_bank<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_payment<7.3,>=7.2
+Requires-Dist: trytond_account_payment_sepa<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_bank<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Account Payment SEPA CFONB Module
 #################################
 
 The account_payment_sepa_cfonb module adds CFONB flavors to SEPA messages.
```

### Comparing `trytond_account_payment_sepa_cfonb-7.0.0/doc/conf.py` & `trytond_account_payment_sepa_cfonb-7.2.0/doc/conf.py`

 * *Files 10% similar despite different names*

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

### Comparing `trytond_account_payment_sepa_cfonb-7.0.0/payment.py` & `trytond_account_payment_sepa_cfonb-7.2.0/payment.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-7.0.0/setup.py` & `trytond_account_payment_sepa_cfonb-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-7.0.0/template/base-cfonb.xml` & `trytond_account_payment_sepa_cfonb-7.2.0/template/base-cfonb.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-7.0.0/template/pain.001.001.03-cfonb.xml` & `trytond_account_payment_sepa_cfonb-7.2.0/template/pain.001.001.03-cfonb.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-7.0.0/template/pain.008.001.02-cfonb.xml` & `trytond_account_payment_sepa_cfonb-7.2.0/template/pain.008.001.02-cfonb.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-7.0.0/tests/test_module.py` & `trytond_account_payment_sepa_cfonb-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-7.0.0/tox.ini` & `trytond_account_payment_sepa_cfonb-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-7.0.0/trytond_account_payment_sepa_cfonb.egg-info/PKG-INFO` & `trytond_account_payment_sepa_cfonb-7.2.0/trytond_account_payment_sepa_cfonb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-payment-sepa-cfonb
-Version: 7.0.0
+Name: trytond_account_payment_sepa_cfonb
+Version: 7.2.0
 Summary: Tryton module for CFONB SEPA payment
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
@@ -50,19 +50,19 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Genshi
 Requires-Dist: lxml
-Requires-Dist: trytond_account_payment<7.1,>=7.0
-Requires-Dist: trytond_account_payment_sepa<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_bank<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_payment<7.3,>=7.2
+Requires-Dist: trytond_account_payment_sepa<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_bank<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Account Payment SEPA CFONB Module
 #################################
 
 The account_payment_sepa_cfonb module adds CFONB flavors to SEPA messages.
```

### Comparing `trytond_account_payment_sepa_cfonb-7.0.0/trytond_account_payment_sepa_cfonb.egg-info/SOURCES.txt` & `trytond_account_payment_sepa_cfonb-7.2.0/trytond_account_payment_sepa_cfonb.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 payment.py
```

