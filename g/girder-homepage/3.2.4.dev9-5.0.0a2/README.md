# Comparing `tmp/girder-homepage-3.2.4.dev9.tar.gz` & `tmp/girder-homepage-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-homepage-3.2.4.dev9.tar", last modified: Mon Apr 29 13:35:07 2024, max compression
+gzip compressed data, was "girder-homepage-5.0.0a2.tar", last modified: Fri Apr 12 16:30:51 2024, max compression
```

## Comparing `girder-homepage-3.2.4.dev9.tar` & `girder-homepage-5.0.0a2.tar`

### file list

```diff
@@ -1,33 +1,26 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:35:07.328144 girder-homepage-3.2.4.dev9/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2024-04-29 13:35:07.328144 girder-homepage-3.2.4.dev9/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:35:07.324144 girder-homepage-3.2.4.dev9/girder_homepage/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/girder_homepage/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       36 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/girder_homepage/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2408 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/girder_homepage/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1695 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/girder_homepage/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:35:07.324144 girder-homepage-3.2.4.dev9/girder_homepage/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/girder_homepage/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      557 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/girder_homepage/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/girder_homepage/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:35:07.324144 girder-homepage-3.2.4.dev9/girder_homepage/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      912 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/girder_homepage/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:35:07.324144 girder-homepage-3.2.4.dev9/girder_homepage/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1472 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/girder_homepage/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:35:07.324144 girder-homepage-3.2.4.dev9/girder_homepage/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6270 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/girder_homepage/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1267 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/girder_homepage/web_client/views/FrontPageView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:35:07.328144 girder-homepage-3.2.4.dev9/girder_homepage.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2024-04-29 13:35:07.000000 girder-homepage-3.2.4.dev9/girder_homepage.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      804 2024-04-29 13:35:07.000000 girder-homepage-3.2.4.dev9/girder_homepage.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-29 13:35:07.000000 girder-homepage-3.2.4.dev9/girder_homepage.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-04-29 13:35:07.000000 girder-homepage-3.2.4.dev9/girder_homepage.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-29 13:35:07.000000 girder-homepage-3.2.4.dev9/girder_homepage.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-29 13:35:07.000000 girder-homepage-3.2.4.dev9/girder_homepage.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-29 13:35:07.000000 girder-homepage-3.2.4.dev9/girder_homepage.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:35:07.328144 girder-homepage-3.2.4.dev9/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6120 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/plugin_tests/homepageSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      700 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/plugin_tests/homepage_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-29 13:35:07.328144 girder-homepage-3.2.4.dev9/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1674 2024-04-29 13:34:16.000000 girder-homepage-3.2.4.dev9/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:51.832654 girder-homepage-5.0.0a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2024-04-12 16:27:18.000000 girder-homepage-5.0.0a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      605 2024-04-12 16:30:51.832654 girder-homepage-5.0.0a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:51.828654 girder-homepage-5.0.0a2/girder_homepage/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      529 2024-04-12 16:27:18.000000 girder-homepage-5.0.0a2/girder_homepage/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       36 2024-04-12 16:27:18.000000 girder-homepage-5.0.0a2/girder_homepage/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2408 2024-04-12 16:27:18.000000 girder-homepage-5.0.0a2/girder_homepage/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1695 2024-04-12 16:27:18.000000 girder-homepage-5.0.0a2/girder_homepage/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:51.828654 girder-homepage-5.0.0a2/girder_homepage/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:51.832654 girder-homepage-5.0.0a2/girder_homepage/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11581 2024-04-12 16:28:21.000000 girder-homepage-5.0.0a2/girder_homepage/web_client/dist/girder-plugin-homepage.umd.cjs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      907 2024-04-12 16:28:21.000000 girder-homepage-5.0.0a2/girder_homepage/web_client/dist/style.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:51.832654 girder-homepage-5.0.0a2/girder_homepage.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      605 2024-04-12 16:30:51.000000 girder-homepage-5.0.0a2/girder_homepage.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      576 2024-04-12 16:30:51.000000 girder-homepage-5.0.0a2/girder_homepage.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:30:51.000000 girder-homepage-5.0.0a2/girder_homepage.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-04-12 16:30:51.000000 girder-homepage-5.0.0a2/girder_homepage.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:30:51.000000 girder-homepage-5.0.0a2/girder_homepage.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:30:51.000000 girder-homepage-5.0.0a2/girder_homepage.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-12 16:30:51.000000 girder-homepage-5.0.0a2/girder_homepage.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-04-12 16:27:18.000000 girder-homepage-5.0.0a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:51.832654 girder-homepage-5.0.0a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder-homepage-5.0.0a2/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      700 2024-04-12 16:27:18.000000 girder-homepage-5.0.0a2/plugin_tests/homepage_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:30:51.832654 girder-homepage-5.0.0a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1674 2024-04-12 16:27:18.000000 girder-homepage-5.0.0a2/setup.py
```

### Comparing `girder-homepage-3.2.4.dev9/PKG-INFO` & `girder-homepage-5.0.0a2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-homepage
-Version: 3.2.4.dev9
+Version: 5.0.0a2
 Summary: Customize the homepage using Markdown.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#homepage
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-homepage-3.2.4.dev9/girder_homepage/rest.py` & `girder-homepage-5.0.0a2/girder_homepage/rest.py`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.2.4.dev9/girder_homepage/settings.py` & `girder-homepage-5.0.0a2/girder_homepage/settings.py`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.2.4.dev9/girder_homepage.egg-info/PKG-INFO` & `girder-homepage-5.0.0a2/girder_homepage.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-homepage
-Version: 3.2.4.dev9
+Version: 5.0.0a2
 Summary: Customize the homepage using Markdown.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#homepage
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-homepage-3.2.4.dev9/plugin_tests/homepage_test.py` & `girder-homepage-5.0.0a2/plugin_tests/homepage_test.py`

 * *Files identical despite different names*

### Comparing `girder-homepage-3.2.4.dev9/setup.py` & `girder-homepage-5.0.0a2/setup.py`

 * *Files identical despite different names*

