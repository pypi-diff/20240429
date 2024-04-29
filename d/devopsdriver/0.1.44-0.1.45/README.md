# Comparing `tmp/devopsdriver-0.1.44.tar.gz` & `tmp/devopsdriver-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopsdriver-0.1.44.tar", last modified: Wed Apr 10 14:55:50 2024, max compression
+gzip compressed data, was "devopsdriver-0.1.45.tar", last modified: Mon Apr 29 03:22:42 2024, max compression
```

## Comparing `devopsdriver-0.1.44.tar` & `devopsdriver-0.1.45.tar`

### file list

```diff
@@ -1,51 +1,57 @@
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 14:55:50.055486 devopsdriver-0.1.44/
--rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.44/LICENSE
--rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-10 14:55:50.055254 devopsdriver-0.1.44/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)     8101 2024-04-10 14:54:35.000000 devopsdriver-0.1.44/README.md
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 14:55:50.050401 devopsdriver-0.1.44/devopsdriver/
--rw-r--r--   0 marcp      (501) staff       (20)      216 2024-04-10 14:55:27.000000 devopsdriver-0.1.44/devopsdriver/__init__.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 14:55:50.051788 devopsdriver-0.1.44/devopsdriver/azdo/
--rw-r--r--   0 marcp      (501) staff       (20)      431 2024-04-10 06:48:39.000000 devopsdriver-0.1.44/devopsdriver/azdo/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)      843 2024-04-10 14:24:30.000000 devopsdriver-0.1.44/devopsdriver/azdo/azureobject.py
--rw-r--r--   0 marcp      (501) staff       (20)     2926 2024-04-10 14:53:52.000000 devopsdriver-0.1.44/devopsdriver/azdo/clients.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 14:55:50.052399 devopsdriver-0.1.44/devopsdriver/azdo/pipeline/
--rw-r--r--   0 marcp      (501) staff       (20)      332 2024-04-10 13:43:08.000000 devopsdriver-0.1.44/devopsdriver/azdo/pipeline/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)      672 2024-04-10 06:48:39.000000 devopsdriver-0.1.44/devopsdriver/azdo/pipeline/client.py
--rw-r--r--   0 marcp      (501) staff       (20)      667 2024-04-10 06:48:39.000000 devopsdriver-0.1.44/devopsdriver/azdo/pipeline/log.py
--rw-r--r--   0 marcp      (501) staff       (20)      918 2024-04-10 06:48:39.000000 devopsdriver-0.1.44/devopsdriver/azdo/pipeline/pipeline.py
--rw-r--r--   0 marcp      (501) staff       (20)     1195 2024-04-10 13:36:56.000000 devopsdriver-0.1.44/devopsdriver/azdo/pipeline/run.py
--rw-r--r--   0 marcp      (501) staff       (20)     3777 2024-04-07 15:39:41.000000 devopsdriver-0.1.44/devopsdriver/azdo/timestamp.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 14:55:50.052756 devopsdriver-0.1.44/devopsdriver/azdo/workitem/
--rw-r--r--   0 marcp      (501) staff       (20)       29 2024-04-06 20:27:22.000000 devopsdriver-0.1.44/devopsdriver/azdo/workitem/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)     2986 2024-04-10 13:37:32.000000 devopsdriver-0.1.44/devopsdriver/azdo/workitem/client.py
--rw-r--r--   0 marcp      (501) staff       (20)     8771 2024-04-08 22:35:57.000000 devopsdriver-0.1.44/devopsdriver/azdo/workitem/wiql.py
--rw-r--r--   0 marcp      (501) staff       (20)     1477 2024-04-10 14:27:03.000000 devopsdriver-0.1.44/devopsdriver/dataobject.py
--rw-r--r--   0 marcp      (501) staff       (20)     1227 2024-04-06 22:13:48.000000 devopsdriver-0.1.44/devopsdriver/manage_settings.py
--rw-r--r--   0 marcp      (501) staff       (20)     3002 2024-04-06 20:27:22.000000 devopsdriver-0.1.44/devopsdriver/sendmail.py
--rw-r--r--   0 marcp      (501) staff       (20)    12276 2024-04-06 22:13:48.000000 devopsdriver-0.1.44/devopsdriver/settings.py
--rw-r--r--   0 marcp      (501) staff       (20)     1077 2024-04-06 21:50:31.000000 devopsdriver-0.1.44/devopsdriver/template.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 14:55:50.053057 devopsdriver-0.1.44/devopsdriver/templates/
--rw-r--r--   0 marcp      (501) staff       (20)      483 2024-04-06 22:13:48.000000 devopsdriver-0.1.44/devopsdriver/templates/manage_settings.txt.mako
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 14:55:50.054818 devopsdriver-0.1.44/devopsdriver.egg-info/
--rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-10 14:55:50.000000 devopsdriver-0.1.44/devopsdriver.egg-info/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)     1256 2024-04-10 14:55:50.000000 devopsdriver-0.1.44/devopsdriver.egg-info/SOURCES.txt
--rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-10 14:55:50.000000 devopsdriver-0.1.44/devopsdriver.egg-info/dependency_links.txt
--rw-r--r--   0 marcp      (501) staff       (20)       63 2024-04-10 14:55:50.000000 devopsdriver-0.1.44/devopsdriver.egg-info/entry_points.txt
--rw-r--r--   0 marcp      (501) staff       (20)      163 2024-04-10 14:55:50.000000 devopsdriver-0.1.44/devopsdriver.egg-info/requires.txt
--rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-10 14:55:50.000000 devopsdriver-0.1.44/devopsdriver.egg-info/top_level.txt
--rw-r--r--   0 marcp      (501) staff       (20)     1669 2024-04-08 16:56:00.000000 devopsdriver-0.1.44/pyproject.toml
--rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-10 14:55:50.055529 devopsdriver-0.1.44/setup.cfg
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-10 14:55:50.054654 devopsdriver-0.1.44/tests/
--rw-r--r--   0 marcp      (501) staff       (20)     4787 2024-04-10 06:48:39.000000 devopsdriver-0.1.44/tests/test_azure_azureobject.py
--rw-r--r--   0 marcp      (501) staff       (20)     6213 2024-04-10 14:53:52.000000 devopsdriver-0.1.44/tests/test_azure_clients.py
--rw-r--r--   0 marcp      (501) staff       (20)     1097 2024-04-10 06:48:39.000000 devopsdriver-0.1.44/tests/test_azure_pipeline.py
--rw-r--r--   0 marcp      (501) staff       (20)      888 2024-04-10 06:48:39.000000 devopsdriver-0.1.44/tests/test_azure_pipeline_client.py
--rw-r--r--   0 marcp      (501) staff       (20)     1711 2024-04-10 13:36:55.000000 devopsdriver-0.1.44/tests/test_azure_pipeline_run.py
--rw-r--r--   0 marcp      (501) staff       (20)     9588 2024-04-10 05:10:33.000000 devopsdriver-0.1.44/tests/test_azure_timestamp.py
--rw-r--r--   0 marcp      (501) staff       (20)     1744 2024-04-10 13:37:30.000000 devopsdriver-0.1.44/tests/test_azure_workitem_client.py
--rw-r--r--   0 marcp      (501) staff       (20)     2881 2024-04-08 22:35:57.000000 devopsdriver-0.1.44/tests/test_azure_workitem_wiql.py
--rw-r--r--   0 marcp      (501) staff       (20)      830 2024-04-10 05:10:33.000000 devopsdriver-0.1.44/tests/test_dataobject.py
--rw-r--r--   0 marcp      (501) staff       (20)     2624 2024-04-06 22:13:48.000000 devopsdriver-0.1.44/tests/test_manage_settings.py
--rw-r--r--   0 marcp      (501) staff       (20)     4466 2024-04-06 20:27:22.000000 devopsdriver-0.1.44/tests/test_sendmail.py
--rw-r--r--   0 marcp      (501) staff       (20)    10203 2024-04-06 22:13:48.000000 devopsdriver-0.1.44/tests/test_settings.py
--rw-r--r--   0 marcp      (501) staff       (20)      886 2024-04-06 20:14:20.000000 devopsdriver-0.1.44/tests/test_template.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-29 03:22:42.177107 devopsdriver-0.1.45/
+-rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.45/LICENSE
+-rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-29 03:22:42.176879 devopsdriver-0.1.45/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)     8101 2024-04-29 03:22:09.000000 devopsdriver-0.1.45/README.md
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-29 03:22:42.172016 devopsdriver-0.1.45/devopsdriver/
+-rw-r--r--   0 marcp      (501) staff       (20)      216 2024-04-29 03:21:58.000000 devopsdriver-0.1.45/devopsdriver/__init__.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-29 03:22:42.173204 devopsdriver-0.1.45/devopsdriver/azdo/
+-rw-r--r--   0 marcp      (501) staff       (20)      431 2024-04-10 06:48:39.000000 devopsdriver-0.1.45/devopsdriver/azdo/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)      843 2024-04-25 00:22:36.000000 devopsdriver-0.1.45/devopsdriver/azdo/azureobject.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-29 03:22:42.173529 devopsdriver-0.1.45/devopsdriver/azdo/builds/
+-rw-r--r--   0 marcp      (501) staff       (20)        0 2024-04-29 03:21:14.000000 devopsdriver-0.1.45/devopsdriver/azdo/builds/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2284 2024-04-29 03:21:14.000000 devopsdriver-0.1.45/devopsdriver/azdo/builds/build.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1875 2024-04-29 03:21:14.000000 devopsdriver-0.1.45/devopsdriver/azdo/builds/client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2982 2024-04-29 03:21:14.000000 devopsdriver-0.1.45/devopsdriver/azdo/clients.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-29 03:22:42.174129 devopsdriver-0.1.45/devopsdriver/azdo/pipeline/
+-rw-r--r--   0 marcp      (501) staff       (20)      332 2024-04-10 13:43:08.000000 devopsdriver-0.1.45/devopsdriver/azdo/pipeline/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)      672 2024-04-10 06:48:39.000000 devopsdriver-0.1.45/devopsdriver/azdo/pipeline/client.py
+-rw-r--r--   0 marcp      (501) staff       (20)      667 2024-04-10 06:48:39.000000 devopsdriver-0.1.45/devopsdriver/azdo/pipeline/log.py
+-rw-r--r--   0 marcp      (501) staff       (20)      918 2024-04-10 06:48:39.000000 devopsdriver-0.1.45/devopsdriver/azdo/pipeline/pipeline.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1195 2024-04-10 13:36:56.000000 devopsdriver-0.1.45/devopsdriver/azdo/pipeline/run.py
+-rw-r--r--   0 marcp      (501) staff       (20)     3777 2024-04-07 15:39:41.000000 devopsdriver-0.1.45/devopsdriver/azdo/timestamp.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-29 03:22:42.174487 devopsdriver-0.1.45/devopsdriver/azdo/workitem/
+-rw-r--r--   0 marcp      (501) staff       (20)       29 2024-04-06 20:27:22.000000 devopsdriver-0.1.45/devopsdriver/azdo/workitem/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2986 2024-04-10 13:37:32.000000 devopsdriver-0.1.45/devopsdriver/azdo/workitem/client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     8771 2024-04-08 22:35:57.000000 devopsdriver-0.1.45/devopsdriver/azdo/workitem/wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1649 2024-04-29 03:21:14.000000 devopsdriver-0.1.45/devopsdriver/dataobject.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1227 2024-04-06 22:13:48.000000 devopsdriver-0.1.45/devopsdriver/manage_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     3002 2024-04-06 20:27:22.000000 devopsdriver-0.1.45/devopsdriver/sendmail.py
+-rw-r--r--   0 marcp      (501) staff       (20)    12276 2024-04-06 22:13:48.000000 devopsdriver-0.1.45/devopsdriver/settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1077 2024-04-06 21:50:31.000000 devopsdriver-0.1.45/devopsdriver/template.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-29 03:22:42.174609 devopsdriver-0.1.45/devopsdriver/templates/
+-rw-r--r--   0 marcp      (501) staff       (20)      483 2024-04-06 22:13:48.000000 devopsdriver-0.1.45/devopsdriver/templates/manage_settings.txt.mako
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-29 03:22:42.176453 devopsdriver-0.1.45/devopsdriver.egg-info/
+-rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-29 03:22:42.000000 devopsdriver-0.1.45/devopsdriver.egg-info/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)     1421 2024-04-29 03:22:42.000000 devopsdriver-0.1.45/devopsdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-29 03:22:42.000000 devopsdriver-0.1.45/devopsdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       63 2024-04-29 03:22:42.000000 devopsdriver-0.1.45/devopsdriver.egg-info/entry_points.txt
+-rw-r--r--   0 marcp      (501) staff       (20)      163 2024-04-29 03:22:42.000000 devopsdriver-0.1.45/devopsdriver.egg-info/requires.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-29 03:22:42.000000 devopsdriver-0.1.45/devopsdriver.egg-info/top_level.txt
+-rw-r--r--   0 marcp      (501) staff       (20)     1669 2024-04-29 03:21:14.000000 devopsdriver-0.1.45/pyproject.toml
+-rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-29 03:22:42.177147 devopsdriver-0.1.45/setup.cfg
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-29 03:22:42.176307 devopsdriver-0.1.45/tests/
+-rw-r--r--   0 marcp      (501) staff       (20)     4787 2024-04-10 06:48:39.000000 devopsdriver-0.1.45/tests/test_azure_azureobject.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2385 2024-04-29 03:21:14.000000 devopsdriver-0.1.45/tests/test_azure_build.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1585 2024-04-29 03:21:14.000000 devopsdriver-0.1.45/tests/test_azure_build_client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     6213 2024-04-10 14:53:52.000000 devopsdriver-0.1.45/tests/test_azure_clients.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1097 2024-04-10 06:48:39.000000 devopsdriver-0.1.45/tests/test_azure_pipeline.py
+-rw-r--r--   0 marcp      (501) staff       (20)      888 2024-04-10 06:48:39.000000 devopsdriver-0.1.45/tests/test_azure_pipeline_client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1711 2024-04-10 13:36:55.000000 devopsdriver-0.1.45/tests/test_azure_pipeline_run.py
+-rw-r--r--   0 marcp      (501) staff       (20)     9588 2024-04-10 05:10:33.000000 devopsdriver-0.1.45/tests/test_azure_timestamp.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1744 2024-04-10 13:37:30.000000 devopsdriver-0.1.45/tests/test_azure_workitem_client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2881 2024-04-08 22:35:57.000000 devopsdriver-0.1.45/tests/test_azure_workitem_wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)      830 2024-04-10 05:10:33.000000 devopsdriver-0.1.45/tests/test_dataobject.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2624 2024-04-06 22:13:48.000000 devopsdriver-0.1.45/tests/test_manage_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     4466 2024-04-06 20:27:22.000000 devopsdriver-0.1.45/tests/test_sendmail.py
+-rw-r--r--   0 marcp      (501) staff       (20)    10203 2024-04-06 22:13:48.000000 devopsdriver-0.1.45/tests/test_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)      886 2024-04-06 20:14:20.000000 devopsdriver-0.1.45/tests/test_template.py
```

### Comparing `devopsdriver-0.1.44/LICENSE` & `devopsdriver-0.1.45/LICENSE`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/PKG-INFO` & `devopsdriver-0.1.45/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.44
+Version: 0.1.45
 Summary: DevOps tools
 Author-email: Marc Page <marcallenpage@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -36,35 +36,35 @@
 Keywords: azure,devops,jira,confluence,email,pipelines,tools
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: keyring==25.1.0
-Requires-Dist: setuptools==69.2.0
+Requires-Dist: setuptools==69.5.1
 Requires-Dist: azure-devops==7.1.0b4
-Requires-Dist: Mako==1.3.2
+Requires-Dist: Mako==1.3.3
 Provides-Extra: dev
 Requires-Dist: black>=24.3.0; extra == "dev"
 Requires-Dist: pylint>=3.1.0; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest>=8.1.1; extra == "test"
 Requires-Dist: coverage>=7.4.4; extra == "test"
 Provides-Extra: doc
 
 ![status sheild](https://img.shields.io/static/v1?label=status&message=beta&color=blue&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.44&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.44/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.45&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.45/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
```

### Comparing `devopsdriver-0.1.44/README.md` & `devopsdriver-0.1.45/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![status sheild](https://img.shields.io/static/v1?label=status&message=beta&color=blue&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.44&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.44/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.45&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.45/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
```

### Comparing `devopsdriver-0.1.44/devopsdriver/azdo/azureobject.py` & `devopsdriver-0.1.45/devopsdriver/azdo/azureobject.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/devopsdriver/azdo/clients.py` & `devopsdriver-0.1.45/devopsdriver/azdo/clients.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from azure.devops.connection import Connection as AzureConnection
 from msrest.authentication import BasicAuthentication as MSBasicAuthentication
 
 from devopsdriver.settings import Settings
 from devopsdriver.azdo.workitem.client import Client as WIClient
 from devopsdriver.azdo.pipeline.client import Client as PLClient
+from devopsdriver.azdo.builds.client import Client as BClient
 
 
 # for testing
 CONNECTION = AzureConnection
 AUTHENTICATION = MSBasicAuthentication
 
 
@@ -56,15 +57,15 @@
         unsupported_clients = set(clients) - set(client_calls)
         assert not unsupported_clients, f"{unsupported_clients} not supported"
         self.workitem = WIClient(Azure.__client("workitem", clients, client_calls))
         self.pipeline = PLClient(Azure.__client("pipeline", clients, client_calls))
         self.core = Azure._Client(Azure.__client("core", clients, client_calls))
         self.task = Azure._Client(Azure.__client("task", clients, client_calls))
         self.git = Azure._Client(Azure.__client("git", clients, client_calls))
-        self.build = Azure._Client(Azure.__client("build", clients, client_calls))
+        self.build = BClient(Azure.__client("build", clients, client_calls))
         self.identity = Azure._Client(Azure.__client("identity", clients, client_calls))
 
     @staticmethod
     def __client(name: str, clients: dict, calls: dict) -> any:
         if clients and not clients.get(name, False):
             return None
```

### Comparing `devopsdriver-0.1.44/devopsdriver/azdo/pipeline/client.py` & `devopsdriver-0.1.45/devopsdriver/azdo/pipeline/client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/devopsdriver/azdo/pipeline/log.py` & `devopsdriver-0.1.45/devopsdriver/azdo/pipeline/log.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/devopsdriver/azdo/pipeline/pipeline.py` & `devopsdriver-0.1.45/devopsdriver/azdo/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/devopsdriver/azdo/pipeline/run.py` & `devopsdriver-0.1.45/devopsdriver/azdo/pipeline/run.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/devopsdriver/azdo/timestamp.py` & `devopsdriver-0.1.45/devopsdriver/azdo/timestamp.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/devopsdriver/azdo/workitem/client.py` & `devopsdriver-0.1.45/devopsdriver/azdo/workitem/client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/devopsdriver/azdo/workitem/wiql.py` & `devopsdriver-0.1.45/devopsdriver/azdo/workitem/wiql.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/devopsdriver/dataobject.py` & `devopsdriver-0.1.45/devopsdriver/dataobject.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 #!/usr/bin/env python3
 
 """ Data Objects """
 
 
+from json import dumps
+
+
 class DataObject:  # pylint: disable=too-few-public-methods
     """dict like object with fuzzy field matching"""
 
     def __init__(self, data: dict):
         self.data = data
 
     def _matches_field(self, name: str, field: str) -> bool:
@@ -42,14 +45,20 @@
             return self._parse_value(data[found[0]])
 
         return None
 
     def __getattr__(self, name: str) -> any:
         return self._get_field(name, self.data)
 
+    def __str__(self) -> str:
+        return dumps(self.data, indent=2)
+
+    def __repr__(self) -> str:
+        return dumps(self.data, indent=2)
+
     class _Dict(dict):
         def __init__(self, dataobject, data: dict):
             self.dataobject = dataobject
             super().__init__(data)
 
         def __getattr__(self, name: str) -> any:
             return self.dataobject._get_field(name, self)
```

### Comparing `devopsdriver-0.1.44/devopsdriver/manage_settings.py` & `devopsdriver-0.1.45/devopsdriver/manage_settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/devopsdriver/sendmail.py` & `devopsdriver-0.1.45/devopsdriver/sendmail.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/devopsdriver/settings.py` & `devopsdriver-0.1.45/devopsdriver/settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/devopsdriver/template.py` & `devopsdriver-0.1.45/devopsdriver/template.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/devopsdriver.egg-info/PKG-INFO` & `devopsdriver-0.1.45/devopsdriver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.44
+Version: 0.1.45
 Summary: DevOps tools
 Author-email: Marc Page <marcallenpage@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -36,35 +36,35 @@
 Keywords: azure,devops,jira,confluence,email,pipelines,tools
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: keyring==25.1.0
-Requires-Dist: setuptools==69.2.0
+Requires-Dist: setuptools==69.5.1
 Requires-Dist: azure-devops==7.1.0b4
-Requires-Dist: Mako==1.3.2
+Requires-Dist: Mako==1.3.3
 Provides-Extra: dev
 Requires-Dist: black>=24.3.0; extra == "dev"
 Requires-Dist: pylint>=3.1.0; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest>=8.1.1; extra == "test"
 Requires-Dist: coverage>=7.4.4; extra == "test"
 Provides-Extra: doc
 
 ![status sheild](https://img.shields.io/static/v1?label=status&message=beta&color=blue&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.44&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.44/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.45&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.45/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
```

### Comparing `devopsdriver-0.1.44/devopsdriver.egg-info/SOURCES.txt` & `devopsdriver-0.1.45/devopsdriver.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -13,24 +13,29 @@
 devopsdriver.egg-info/entry_points.txt
 devopsdriver.egg-info/requires.txt
 devopsdriver.egg-info/top_level.txt
 devopsdriver/azdo/__init__.py
 devopsdriver/azdo/azureobject.py
 devopsdriver/azdo/clients.py
 devopsdriver/azdo/timestamp.py
+devopsdriver/azdo/builds/__init__.py
+devopsdriver/azdo/builds/build.py
+devopsdriver/azdo/builds/client.py
 devopsdriver/azdo/pipeline/__init__.py
 devopsdriver/azdo/pipeline/client.py
 devopsdriver/azdo/pipeline/log.py
 devopsdriver/azdo/pipeline/pipeline.py
 devopsdriver/azdo/pipeline/run.py
 devopsdriver/azdo/workitem/__init__.py
 devopsdriver/azdo/workitem/client.py
 devopsdriver/azdo/workitem/wiql.py
 devopsdriver/templates/manage_settings.txt.mako
 tests/test_azure_azureobject.py
+tests/test_azure_build.py
+tests/test_azure_build_client.py
 tests/test_azure_clients.py
 tests/test_azure_pipeline.py
 tests/test_azure_pipeline_client.py
 tests/test_azure_pipeline_run.py
 tests/test_azure_timestamp.py
 tests/test_azure_workitem_client.py
 tests/test_azure_workitem_wiql.py
```

### Comparing `devopsdriver-0.1.44/pyproject.toml` & `devopsdriver-0.1.45/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 readme = "README.md"
 license = {file = "LICENSE"}
 dynamic = ["version"]
 requires-python = ">= 3.10"
 dependencies = [
   "PyYAML==6.0.1",
   "keyring==25.1.0",
-  "setuptools==69.2.0",  # neded for azure-devops to use 7.1 API
+  "setuptools==69.5.1",  # neded for azure-devops to use 7.1 API
   "azure-devops==7.1.0b4",
-  "Mako==1.3.2",
+  "Mako==1.3.3",
 ]
 keywords = ["azure", "devops", "jira", "confluence", "email", "pipelines", "tools"]
 classifiers=[
     "Development Status :: 1 - Planning",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: The Unlicense (Unlicense)",
-    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.10",
     "Topic :: Utilities",
     "Topic :: Software Development",
 ]
 authors = [
   {name = "Marc Page", email = "marcallenpage@gmail.com"},
 ]
```

### Comparing `devopsdriver-0.1.44/tests/test_azure_azureobject.py` & `devopsdriver-0.1.45/tests/test_azure_azureobject.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/tests/test_azure_clients.py` & `devopsdriver-0.1.45/tests/test_azure_clients.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/tests/test_azure_pipeline.py` & `devopsdriver-0.1.45/tests/test_azure_pipeline.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/tests/test_azure_pipeline_client.py` & `devopsdriver-0.1.45/tests/test_azure_pipeline_client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/tests/test_azure_pipeline_run.py` & `devopsdriver-0.1.45/tests/test_azure_pipeline_run.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/tests/test_azure_timestamp.py` & `devopsdriver-0.1.45/tests/test_azure_timestamp.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/tests/test_azure_workitem_client.py` & `devopsdriver-0.1.45/tests/test_azure_workitem_client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/tests/test_azure_workitem_wiql.py` & `devopsdriver-0.1.45/tests/test_azure_workitem_wiql.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/tests/test_dataobject.py` & `devopsdriver-0.1.45/tests/test_dataobject.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/tests/test_manage_settings.py` & `devopsdriver-0.1.45/tests/test_manage_settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/tests/test_sendmail.py` & `devopsdriver-0.1.45/tests/test_sendmail.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/tests/test_settings.py` & `devopsdriver-0.1.45/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.44/tests/test_template.py` & `devopsdriver-0.1.45/tests/test_template.py`

 * *Files identical despite different names*

