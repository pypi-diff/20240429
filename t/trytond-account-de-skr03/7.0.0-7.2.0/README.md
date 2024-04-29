# Comparing `tmp/trytond_account_de_skr03-7.0.0.tar.gz` & `tmp/trytond_account_de_skr03-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_de_skr03-7.0.0.tar", last modified: Mon Oct 30 17:19:01 2023, max compression
+gzip compressed data, was "trytond_account_de_skr03-7.2.0.tar", last modified: Mon Apr 29 15:32:21 2024, max compression
```

## Comparing `trytond_account_de_skr03-7.0.0.tar` & `trytond_account_de_skr03-7.2.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:01.789006 trytond_account_de_skr03-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-22 17:22:48.000000 trytond_account_de_skr03-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2616 2023-10-30 17:01:09.000000 trytond_account_de_skr03-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      762 2023-10-30 17:01:09.000000 trytond_account_de_skr03-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35146 2023-01-16 14:00:20.000000 trytond_account_de_skr03-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_de_skr03-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     1729 2023-10-30 17:19:01.789006 trytond_account_de_skr03-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      106 2023-04-15 07:12:14.000000 trytond_account_de_skr03-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_account_de_skr03-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1720 2023-04-15 07:12:15.000000 trytond_account_de_skr03-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)   392382 2023-04-15 07:12:15.000000 trytond_account_de_skr03-7.0.0/account_de.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:01.785673 trytond_account_de_skr03-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2817 2023-10-22 17:22:48.000000 trytond_account_de_skr03-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      106 2023-04-15 07:12:14.000000 trytond_account_de_skr03-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:48.000000 trytond_account_de_skr03-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:19:01.789006 trytond_account_de_skr03-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     3526 2023-10-27 17:38:49.000000 trytond_account_de_skr03-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    85941 2023-04-15 07:12:14.000000 trytond_account_de_skr03-7.0.0/tax_de.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:01.785673 trytond_account_de_skr03-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_de_skr03-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_account_de_skr03-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_de_skr03-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       83 2023-10-30 17:01:06.000000 trytond_account_de_skr03-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:19:01.789006 trytond_account_de_skr03-7.0.0/trytond_account_de_skr03.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     1729 2023-10-30 17:19:01.000000 trytond_account_de_skr03-7.0.0/trytond_account_de_skr03.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      685 2023-10-30 17:19:01.000000 trytond_account_de_skr03-7.0.0/trytond_account_de_skr03.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:19:01.000000 trytond_account_de_skr03-7.0.0/trytond_account_de_skr03.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-10-30 17:19:01.000000 trytond_account_de_skr03-7.0.0/trytond_account_de_skr03.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_account_de_skr03-7.0.0/trytond_account_de_skr03.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       44 2023-10-30 17:19:01.000000 trytond_account_de_skr03-7.0.0/trytond_account_de_skr03.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:19:01.000000 trytond_account_de_skr03-7.0.0/trytond_account_de_skr03.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:21.155449 trytond_account_de_skr03-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2717 2024-04-29 15:13:12.000000 trytond_account_de_skr03-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      762 2024-04-29 15:13:12.000000 trytond_account_de_skr03-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35146 2023-01-16 14:00:20.000000 trytond_account_de_skr03-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_de_skr03-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     1729 2024-04-29 15:32:21.155449 trytond_account_de_skr03-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      106 2023-04-15 07:12:14.000000 trytond_account_de_skr03-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_account_de_skr03-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1720 2023-04-15 07:12:15.000000 trytond_account_de_skr03-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   392382 2023-04-15 07:12:15.000000 trytond_account_de_skr03-7.2.0/account_de.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:21.152115 trytond_account_de_skr03-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_account_de_skr03-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      106 2023-04-15 07:12:14.000000 trytond_account_de_skr03-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:51.000000 trytond_account_de_skr03-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:32:21.155449 trytond_account_de_skr03-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3526 2024-03-17 11:01:36.000000 trytond_account_de_skr03-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    85941 2023-04-15 07:12:14.000000 trytond_account_de_skr03-7.2.0/tax_de.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:21.152115 trytond_account_de_skr03-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_de_skr03-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_account_de_skr03-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:51.000000 trytond_account_de_skr03-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       83 2024-04-29 15:13:08.000000 trytond_account_de_skr03-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:21.152115 trytond_account_de_skr03-7.2.0/trytond_account_de_skr03.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1729 2024-04-29 15:32:20.000000 trytond_account_de_skr03-7.2.0/trytond_account_de_skr03.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      667 2024-04-29 15:32:21.000000 trytond_account_de_skr03-7.2.0/trytond_account_de_skr03.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:32:20.000000 trytond_account_de_skr03-7.2.0/trytond_account_de_skr03.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:32:20.000000 trytond_account_de_skr03-7.2.0/trytond_account_de_skr03.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_account_de_skr03-7.2.0/trytond_account_de_skr03.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       44 2024-04-29 15:32:20.000000 trytond_account_de_skr03-7.2.0/trytond_account_de_skr03.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:32:20.000000 trytond_account_de_skr03-7.2.0/trytond_account_de_skr03.egg-info/top_level.txt
```

### Comparing `trytond_account_de_skr03-7.0.0/CHANGELOG` & `trytond_account_de_skr03-7.2.0/CHANGELOG`

 * *Files 9% similar despite different names*

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

### Comparing `trytond_account_de_skr03-7.0.0/COPYRIGHT` & `trytond_account_de_skr03-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_de_skr03-7.0.0/LICENSE` & `trytond_account_de_skr03-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_de_skr03-7.0.0/PKG-INFO` & `trytond_account_de_skr03-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_de_skr03
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module with German chart of accounts SKR03
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
@@ -29,14 +29,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 German Account Module
 #####################
 
 The German account module define the SKR03 chart of account.
```

### Comparing `trytond_account_de_skr03-7.0.0/account.py` & `trytond_account_de_skr03-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_de_skr03-7.0.0/account_de.xml` & `trytond_account_de_skr03-7.2.0/account_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_de_skr03-7.0.0/doc/conf.py` & `trytond_account_de_skr03-7.2.0/doc/conf.py`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_account_de_skr03-7.0.0/setup.py` & `trytond_account_de_skr03-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_de_skr03-7.0.0/tax_de.xml` & `trytond_account_de_skr03-7.2.0/tax_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_de_skr03-7.0.0/tox.ini` & `trytond_account_de_skr03-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_de_skr03-7.0.0/trytond_account_de_skr03.egg-info/PKG-INFO` & `trytond_account_de_skr03-7.2.0/trytond_account_de_skr03.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-de-skr03
-Version: 7.0.0
+Name: trytond_account_de_skr03
+Version: 7.2.0
 Summary: Tryton module with German chart of accounts SKR03
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
@@ -29,14 +29,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 German Account Module
 #####################
 
 The German account module define the SKR03 chart of account.
```

### Comparing `trytond_account_de_skr03-7.0.0/trytond_account_de_skr03.egg-info/SOURCES.txt` & `trytond_account_de_skr03-7.2.0/trytond_account_de_skr03.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 account.py
```

