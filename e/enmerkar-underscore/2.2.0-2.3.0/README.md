# Comparing `tmp/enmerkar-underscore-2.2.0.tar.gz` & `tmp/enmerkar_underscore-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enmerkar-underscore-2.2.0.tar", last modified: Thu Aug  3 11:04:02 2023, max compression
+gzip compressed data, was "enmerkar_underscore-2.3.0.tar", last modified: Mon Apr 29 18:22:52 2024, max compression
```

## Comparing `enmerkar-underscore-2.2.0.tar` & `enmerkar_underscore-2.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.478622 enmerkar-underscore-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-08-03 11:04:02.478622 enmerkar-underscore-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.474622 enmerkar-underscore-2.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     6777 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8609 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6466 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.474622 enmerkar-underscore-2.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-08-03 11:04:02.478622 enmerkar-underscore-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5710 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.474622 enmerkar-underscore-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.474622 enmerkar-underscore-2.2.0/src/enmerkar_underscore/
--rw-r--r--   0 runner    (1001) docker     (122)     3218 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.478622 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-08-03 11:04:02.000000 enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:04:02.478622 enmerkar-underscore-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2006 2023-08-03 11:03:57.000000 enmerkar-underscore-2.2.0/tests/test_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:22:52.152658 enmerkar_underscore-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-29 18:22:52.152658 enmerkar_underscore-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:22:52.152658 enmerkar_underscore-2.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:22:52.152658 enmerkar_underscore-2.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-29 18:22:52.156658 enmerkar_underscore-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:22:52.148658 enmerkar_underscore-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:22:52.152658 enmerkar_underscore-2.3.0/src/enmerkar_underscore/
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/src/enmerkar_underscore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:22:52.152658 enmerkar_underscore-2.3.0/src/enmerkar_underscore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-29 18:22:52.000000 enmerkar_underscore-2.3.0/src/enmerkar_underscore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-29 18:22:52.000000 enmerkar_underscore-2.3.0/src/enmerkar_underscore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:22:52.000000 enmerkar_underscore-2.3.0/src/enmerkar_underscore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 18:22:52.000000 enmerkar_underscore-2.3.0/src/enmerkar_underscore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:22:52.000000 enmerkar_underscore-2.3.0/src/enmerkar_underscore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 18:22:52.000000 enmerkar_underscore-2.3.0/src/enmerkar_underscore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-29 18:22:52.000000 enmerkar_underscore-2.3.0/src/enmerkar_underscore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:22:52.152658 enmerkar_underscore-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-29 18:22:44.000000 enmerkar_underscore-2.3.0/tests/test_extract.py
```

### Comparing `enmerkar-underscore-2.2.0/CONTRIBUTING.rst` & `enmerkar_underscore-2.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.2.0/HISTORY.rst` & `enmerkar_underscore-2.3.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.2.0/LICENSE` & `enmerkar_underscore-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.2.0/PKG-INFO` & `enmerkar_underscore-2.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: enmerkar-underscore
-Version: 2.2.0
+Version: 2.3.0
 Summary: Implements a underscore extractor for django-babel.
 Home-page: https://github.com/openedx/enmerkar-underscore
 Author: edX
 Author-email: oscm@edx.org
 License: BSD
 Keywords: enmerkar-underscore
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
+Requires-Dist: babel>=1.3
+Requires-Dist: django
+Requires-Dist: enmerkar==0.7.1
 
 =================================
 Django Babel Underscore Extractor
 =================================
 
 .. image:: https://badge.fury.io/py/django-babel-underscore.png
     :target: http://badge.fury.io/py/django-babel-underscore
```

### Comparing `enmerkar-underscore-2.2.0/README.rst` & `enmerkar_underscore-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.2.0/docs/Makefile` & `enmerkar_underscore-2.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.2.0/docs/conf.py` & `enmerkar_underscore-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.2.0/docs/index.rst` & `enmerkar_underscore-2.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.2.0/docs/make.bat` & `enmerkar_underscore-2.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.2.0/requirements/constraints.txt` & `enmerkar_underscore-2.3.0/requirements/constraints.txt`

 * *Files 23% similar despite different names*

```diff
@@ -6,7 +6,11 @@
 # When pinning something here, please provide an explanation of why.  Ideally,
 # link to other information that will help people in the future to remove the
 # pin when possible.  Writing an issue against the offending project and
 # linking to it here is good.
 
 # Common constraints for edx repos
 -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+
+
+# Temporary to Support the python 3.11 Upgrade
+backports.zoneinfo;python_version<"3.9"  # Newer versions have zoneinfo available in the standard library
```

### Comparing `enmerkar-underscore-2.2.0/setup.py` & `enmerkar_underscore-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,13 @@
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',        
-        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.2',
     ],
 )
```

### Comparing `enmerkar-underscore-2.2.0/src/enmerkar_underscore/__init__.py` & `enmerkar_underscore-2.3.0/src/enmerkar_underscore/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import django
-
 from django.template.base import Lexer
 
 if django.VERSION[:2] >= (2, 1):
     from django.template.base import TokenType
     TOKEN_TEXT = TokenType.TEXT
 else:  # django < 2.1
     from django.template.base import TOKEN_TEXT
 
 from django.utils.encoding import force_str
 from enmerkar.extract import extract_django
-from markey import underscore
-from markey.tools import TokenStream
-from markey.machine import tokenize, parse_arguments
 
+from .vendor.markey import underscore
+from .vendor.markey.machine import parse_arguments, tokenize
+from .vendor.markey.tools import TokenStream
 
-__version__ = '2.2.0'
+__version__ = '2.3.0'
 
 def extract(fileobj, keywords, comment_tags, options):
     """Extracts translation messages from underscore template files.
 
     This method does also extract django templates. If a template does not
     contain any django translation tags we always fallback to underscore extraction.
```

### Comparing `enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/PKG-INFO` & `enmerkar_underscore-2.3.0/src/enmerkar_underscore.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: enmerkar-underscore
-Version: 2.2.0
+Version: 2.3.0
 Summary: Implements a underscore extractor for django-babel.
 Home-page: https://github.com/openedx/enmerkar-underscore
 Author: edX
 Author-email: oscm@edx.org
 License: BSD
 Keywords: enmerkar-underscore
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
+Requires-Dist: babel>=1.3
+Requires-Dist: django
+Requires-Dist: enmerkar==0.7.1
 
 =================================
 Django Babel Underscore Extractor
 =================================
 
 .. image:: https://badge.fury.io/py/django-babel-underscore.png
     :target: http://badge.fury.io/py/django-babel-underscore
```

### Comparing `enmerkar-underscore-2.2.0/src/enmerkar_underscore.egg-info/SOURCES.txt` & `enmerkar_underscore-2.3.0/src/enmerkar_underscore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.2.0/tests/__init__.py` & `enmerkar_underscore-2.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `enmerkar-underscore-2.2.0/tests/test_extract.py` & `enmerkar_underscore-2.3.0/tests/test_extract.py`

 * *Files identical despite different names*

