# Comparing `tmp/wagtail-treemodeladmin-1.9.0.tar.gz` & `tmp/wagtail_treemodeladmin-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-treemodeladmin-1.9.0.tar", last modified: Tue Jan  2 16:58:44 2024, max compression
+gzip compressed data, was "wagtail_treemodeladmin-1.9.1.tar", last modified: Mon Apr 29 12:27:11 2024, max compression
```

## Comparing `wagtail-treemodeladmin-1.9.0.tar` & `wagtail_treemodeladmin-1.9.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:44.361735 wagtail-treemodeladmin-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-01-02 16:58:44.361735 wagtail-treemodeladmin-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 16:58:44.361735 wagtail-treemodeladmin-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:44.357735 wagtail-treemodeladmin-1.9.0/treemodeladmin/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:44.353735 wagtail-treemodeladmin-1.9.0/treemodeladmin/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:44.353735 wagtail-treemodeladmin-1.9.0/treemodeladmin/static/treemodeladmin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:44.357735 wagtail-treemodeladmin-1.9.0/treemodeladmin/static/treemodeladmin/css/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/static/treemodeladmin/css/index.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:44.353735 wagtail-treemodeladmin-1.9.0/treemodeladmin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:44.357735 wagtail-treemodeladmin-1.9.0/treemodeladmin/templates/treemodeladmin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:44.357735 wagtail-treemodeladmin-1.9.0/treemodeladmin/templates/treemodeladmin/includes/
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/templates/treemodeladmin/includes/breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/templates/treemodeladmin/includes/tree_result_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/templates/treemodeladmin/includes/tree_result_row.html
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/templates/treemodeladmin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:44.357735 wagtail-treemodeladmin-1.9.0/treemodeladmin/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/templatetags/treemodeladmin_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:44.357735 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:44.361735 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/treemodeladmintest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/treemodeladmintest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/treemodeladmintest/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:44.361735 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/treemodeladmintest/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/treemodeladmintest/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/treemodeladmintest/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/treemodeladmintest/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/treemodeladmintest/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-01-02 16:58:36.000000 wagtail-treemodeladmin-1.9.0/treemodeladmin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 16:58:44.361735 wagtail-treemodeladmin-1.9.0/wagtail_treemodeladmin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-01-02 16:58:44.000000 wagtail-treemodeladmin-1.9.0/wagtail_treemodeladmin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-01-02 16:58:44.000000 wagtail-treemodeladmin-1.9.0/wagtail_treemodeladmin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 16:58:44.000000 wagtail-treemodeladmin-1.9.0/wagtail_treemodeladmin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-02 16:58:44.000000 wagtail-treemodeladmin-1.9.0/wagtail_treemodeladmin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-02 16:58:44.000000 wagtail-treemodeladmin-1.9.0/wagtail_treemodeladmin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:11.989468 wagtail_treemodeladmin-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-29 12:27:11.989468 wagtail_treemodeladmin-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:27:11.989468 wagtail_treemodeladmin-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:11.981468 wagtail_treemodeladmin-1.9.1/treemodeladmin/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:11.981468 wagtail_treemodeladmin-1.9.1/treemodeladmin/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:11.981468 wagtail_treemodeladmin-1.9.1/treemodeladmin/static/treemodeladmin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:11.981468 wagtail_treemodeladmin-1.9.1/treemodeladmin/static/treemodeladmin/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/static/treemodeladmin/css/index.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:11.981468 wagtail_treemodeladmin-1.9.1/treemodeladmin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:11.981468 wagtail_treemodeladmin-1.9.1/treemodeladmin/templates/treemodeladmin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:11.985468 wagtail_treemodeladmin-1.9.1/treemodeladmin/templates/treemodeladmin/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/templates/treemodeladmin/includes/breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/templates/treemodeladmin/includes/tree_result_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/templates/treemodeladmin/includes/tree_result_row.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/templates/treemodeladmin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:11.985468 wagtail_treemodeladmin-1.9.1/treemodeladmin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/templatetags/treemodeladmin_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:11.985468 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:11.985468 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/treemodeladmintest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/treemodeladmintest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/treemodeladmintest/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:11.985468 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/treemodeladmintest/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/treemodeladmintest/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/treemodeladmintest/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/treemodeladmintest/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/treemodeladmintest/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-04-29 12:27:04.000000 wagtail_treemodeladmin-1.9.1/treemodeladmin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:27:11.985468 wagtail_treemodeladmin-1.9.1/wagtail_treemodeladmin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-29 12:27:11.000000 wagtail_treemodeladmin-1.9.1/wagtail_treemodeladmin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-29 12:27:11.000000 wagtail_treemodeladmin-1.9.1/wagtail_treemodeladmin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:27:11.000000 wagtail_treemodeladmin-1.9.1/wagtail_treemodeladmin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 12:27:11.000000 wagtail_treemodeladmin-1.9.1/wagtail_treemodeladmin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 12:27:11.000000 wagtail_treemodeladmin-1.9.1/wagtail_treemodeladmin.egg-info/top_level.txt
```

### Comparing `wagtail-treemodeladmin-1.9.0/LICENSE` & `wagtail_treemodeladmin-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/PKG-INFO` & `wagtail_treemodeladmin-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-treemodeladmin
-Version: 1.9.0
+Version: 1.9.1
 Summary: TreeModelAdmin for Wagtail
 Author-email: CFPB <tech@cfpb.gov>
 License: CC0
 Project-URL: Homepage, https://github.com/cfpb/wagtail-treemodeladmin
 Project-URL: Bug Reports, https://github.com/cfpb/wagtail-treemodeladmin/issues
 Project-URL: Source, https://github.com/cfpb/wagtail-treemodeladmin
 Classifier: Framework :: Django
@@ -16,15 +16,15 @@
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: wagtail<5.3,>=5.1
+Requires-Dist: wagtail>=5.1
 Requires-Dist: wagtail-modeladmin>=1.0
 Provides-Extra: testing
 Requires-Dist: coverage[toml]; extra == "testing"
 
 # Wagtail-TreeModelAdmin
 
 ![Build Status](https://github.com/cfpb/wagtail-treemodeladmin/workflows/test/badge.svg)
```

### Comparing `wagtail-treemodeladmin-1.9.0/README.md` & `wagtail_treemodeladmin-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/pyproject.toml` & `wagtail_treemodeladmin-1.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "wagtail-treemodeladmin"
-version = "1.9.0"
+version = "1.9.1"
 description = "TreeModelAdmin for Wagtail"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "CC0"}
 authors = [
     {name = "CFPB", email = "tech@cfpb.gov" }
 ]
 dependencies = [
-    "wagtail>=5.1,<5.3",
+    "wagtail>=5.1",
     "wagtail-modeladmin>=1.0",
 ]
 classifiers = [
     "Framework :: Django",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.2",
     "Framework :: Wagtail",
```

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/helpers.py` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/helpers.py`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/options.py` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/options.py`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/templates/treemodeladmin/includes/breadcrumb.html` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/templates/treemodeladmin/includes/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/templates/treemodeladmin/includes/tree_result_list.html` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/templates/treemodeladmin/includes/tree_result_list.html`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/templates/treemodeladmin/includes/tree_result_row.html` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/templates/treemodeladmin/includes/tree_result_row.html`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/templates/treemodeladmin/index.html` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/templates/treemodeladmin/index.html`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/templatetags/treemodeladmin_tags.py` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/templatetags/treemodeladmin_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/settings.py` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/test_options.py` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/test_views.py` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/treemodeladmintest/migrations/0001_initial.py` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/treemodeladmintest/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/treemodeladmintest/models.py` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/treemodeladmintest/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/tests/treemodeladmintest/wagtail_hooks.py` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/tests/treemodeladmintest/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/treemodeladmin/views.py` & `wagtail_treemodeladmin-1.9.1/treemodeladmin/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-treemodeladmin-1.9.0/wagtail_treemodeladmin.egg-info/PKG-INFO` & `wagtail_treemodeladmin-1.9.1/wagtail_treemodeladmin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-treemodeladmin
-Version: 1.9.0
+Version: 1.9.1
 Summary: TreeModelAdmin for Wagtail
 Author-email: CFPB <tech@cfpb.gov>
 License: CC0
 Project-URL: Homepage, https://github.com/cfpb/wagtail-treemodeladmin
 Project-URL: Bug Reports, https://github.com/cfpb/wagtail-treemodeladmin/issues
 Project-URL: Source, https://github.com/cfpb/wagtail-treemodeladmin
 Classifier: Framework :: Django
@@ -16,15 +16,15 @@
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: wagtail<5.3,>=5.1
+Requires-Dist: wagtail>=5.1
 Requires-Dist: wagtail-modeladmin>=1.0
 Provides-Extra: testing
 Requires-Dist: coverage[toml]; extra == "testing"
 
 # Wagtail-TreeModelAdmin
 
 ![Build Status](https://github.com/cfpb/wagtail-treemodeladmin/workflows/test/badge.svg)
```

### Comparing `wagtail-treemodeladmin-1.9.0/wagtail_treemodeladmin.egg-info/SOURCES.txt` & `wagtail_treemodeladmin-1.9.1/wagtail_treemodeladmin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

