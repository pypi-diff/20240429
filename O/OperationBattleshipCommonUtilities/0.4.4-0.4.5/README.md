# Comparing `tmp/operationbattleshipcommonutilities-0.4.4.tar.gz` & `tmp/operationbattleshipcommonutilities-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operationbattleshipcommonutilities-0.4.4.tar", last modified: Tue Apr 23 05:31:30 2024, max compression
+gzip compressed data, was "operationbattleshipcommonutilities-0.4.5.tar", last modified: Mon Apr 29 00:43:48 2024, max compression
```

## Comparing `operationbattleshipcommonutilities-0.4.4.tar` & `operationbattleshipcommonutilities-0.4.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 05:31:30.601817 operationbattleshipcommonutilities-0.4.4/
--rw-rw-rw-   0        0        0    11558 2024-03-23 16:54:02.000000 operationbattleshipcommonutilities-0.4.4/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-23 05:31:30.597822 operationbattleshipcommonutilities-0.4.4/OperationBattleshipCommonUtilities.egg-info/
--rw-rw-rw-   0        0        0     3177 2024-04-23 05:31:30.000000 operationbattleshipcommonutilities-0.4.4/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1182 2024-04-23 05:31:30.000000 operationbattleshipcommonutilities-0.4.4/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 05:31:30.000000 operationbattleshipcommonutilities-0.4.4/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-23 05:31:30.000000 operationbattleshipcommonutilities-0.4.4/OperationBattleshipCommonUtilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2024-04-23 05:31:30.000000 operationbattleshipcommonutilities-0.4.4/OperationBattleshipCommonUtilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3177 2024-04-23 05:31:30.598819 operationbattleshipcommonutilities-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     2571 2024-03-08 06:05:09.000000 operationbattleshipcommonutilities-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 05:31:30.595818 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/
--rw-rw-rw-   0        0        0     4577 2024-03-24 01:03:06.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/ApifyJobsCaller.py
--rw-rw-rw-   0        0        0     2601 2024-04-01 21:52:27.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/CandidateRequirementsDao.py
--rw-rw-rw-   0        0        0     6556 2024-04-23 05:23:30.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/CompanyDao.py
--rw-rw-rw-   0        0        0     3143 2024-04-01 21:48:50.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/FailureLogger.py
--rw-rw-rw-   0        0        0     1513 2024-04-01 23:24:18.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/GenaricDatabaseDao.py
--rw-rw-rw-   0        0        0     2219 2024-04-01 21:47:52.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/GeographyHelper.py
--rw-rw-rw-   0        0        0     3365 2024-04-01 21:47:37.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/JobKeyWordsDao.py
--rw-rw-rw-   0        0        0    18787 2024-04-23 03:16:06.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/JobPostingDao.py
--rw-rw-rw-   0        0        0     1706 2024-04-01 21:39:48.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/JobResponsibilitiesDao.py
--rw-rw-rw-   0        0        0     2848 2024-04-01 21:39:04.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/JobSkillsDao.py
--rw-rw-rw-   0        0        0     1830 2024-02-17 14:46:22.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
--rw-rw-rw-   0        0        0      613 2024-03-12 04:49:56.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/NomicAICaller.py
--rw-rw-rw-   0        0        0     1087 2024-02-15 03:50:23.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/OpenAICaller.py
--rw-rw-rw-   0        0        0     3332 2024-04-23 05:20:23.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/PineConeDatabaseCaller.py
--rw-rw-rw-   0        0        0        0 2024-01-26 02:28:14.000000 operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-23 05:31:30.602823 operationbattleshipcommonutilities-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      734 2024-04-23 05:24:14.000000 operationbattleshipcommonutilities-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 00:43:48.019741 operationbattleshipcommonutilities-0.4.5/
+-rw-rw-rw-   0        0        0    11558 2024-03-23 16:54:02.000000 operationbattleshipcommonutilities-0.4.5/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-29 00:43:48.010781 operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/
+-rw-rw-rw-   0        0        0     3177 2024-04-29 00:43:47.000000 operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1182 2024-04-29 00:43:47.000000 operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 00:43:47.000000 operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-29 00:43:47.000000 operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2024-04-29 00:43:47.000000 operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3177 2024-04-29 00:43:48.013732 operationbattleshipcommonutilities-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2571 2024-03-08 06:05:09.000000 operationbattleshipcommonutilities-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 00:43:47.967735 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/
+-rw-rw-rw-   0        0        0     4577 2024-03-24 01:03:06.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/ApifyJobsCaller.py
+-rw-rw-rw-   0        0        0     2601 2024-04-01 21:52:27.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/CandidateRequirementsDao.py
+-rw-rw-rw-   0        0        0     6556 2024-04-23 05:23:30.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/CompanyDao.py
+-rw-rw-rw-   0        0        0     3143 2024-04-01 21:48:50.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/FailureLogger.py
+-rw-rw-rw-   0        0        0     1513 2024-04-01 23:24:18.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/GenaricDatabaseDao.py
+-rw-rw-rw-   0        0        0     2219 2024-04-01 21:47:52.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/GeographyHelper.py
+-rw-rw-rw-   0        0        0     3365 2024-04-01 21:47:37.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobKeyWordsDao.py
+-rw-rw-rw-   0        0        0     4132 2024-04-28 16:36:13.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobPostingDao.py
+-rw-rw-rw-   0        0        0     1706 2024-04-01 21:39:48.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobResponsibilitiesDao.py
+-rw-rw-rw-   0        0        0     2848 2024-04-01 21:39:04.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobSkillsDao.py
+-rw-rw-rw-   0        0        0     1830 2024-02-17 14:46:22.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
+-rw-rw-rw-   0        0        0      613 2024-03-12 04:49:56.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/NomicAICaller.py
+-rw-rw-rw-   0        0        0     1087 2024-02-15 03:50:23.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/OpenAICaller.py
+-rw-rw-rw-   0        0        0     3332 2024-04-23 05:20:23.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/PineConeDatabaseCaller.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 02:28:14.000000 operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-29 00:43:48.019741 operationbattleshipcommonutilities-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      734 2024-04-29 00:38:03.000000 operationbattleshipcommonutilities-0.4.5/setup.py
```

### Comparing `operationbattleshipcommonutilities-0.4.4/LICENSE` & `operationbattleshipcommonutilities-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/OperationBattleshipCommonUtilities.egg-info/PKG-INFO` & `operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OperationBattleshipCommonUtilities
-Version: 0.4.4
+Version: 0.4.5
 Summary: Classes and Utilities that are shared in the Operation Battleship Application
 Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
 Author: Matthew Caraway
 Author-email: matthew@CarawayLabs.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `operationbattleshipcommonutilities-0.4.4/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt` & `operationbattleshipcommonutilities-0.4.5/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/PKG-INFO` & `operationbattleshipcommonutilities-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OperationBattleshipCommonUtilities
-Version: 0.4.4
+Version: 0.4.5
 Summary: Classes and Utilities that are shared in the Operation Battleship Application
 Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
 Author: Matthew Caraway
 Author-email: matthew@CarawayLabs.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `operationbattleshipcommonutilities-0.4.4/README.md` & `operationbattleshipcommonutilities-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/ApifyJobsCaller.py` & `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/ApifyJobsCaller.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/CandidateRequirementsDao.py` & `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/CandidateRequirementsDao.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/CompanyDao.py` & `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/CompanyDao.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/FailureLogger.py` & `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/FailureLogger.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/GenaricDatabaseDao.py` & `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/GenaricDatabaseDao.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/GeographyHelper.py` & `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/GeographyHelper.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/JobKeyWordsDao.py` & `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobKeyWordsDao.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/JobResponsibilitiesDao.py` & `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobResponsibilitiesDao.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/JobSkillsDao.py` & `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobSkillsDao.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/JobTitleCategoryClassifier.py` & `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/JobTitleCategoryClassifier.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/NomicAICaller.py` & `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/NomicAICaller.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/OpenAICaller.py` & `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/OpenAICaller.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/operation_battleship_common_utilities/PineConeDatabaseCaller.py` & `operationbattleshipcommonutilities-0.4.5/operation_battleship_common_utilities/PineConeDatabaseCaller.py`

 * *Files identical despite different names*

### Comparing `operationbattleshipcommonutilities-0.4.4/setup.py` & `operationbattleshipcommonutilities-0.4.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='OperationBattleshipCommonUtilities',
-    version='0.4.4',
+    version='0.4.5',
     packages=find_packages(),
     license='Apache-2.0 license',
     description='Classes and Utilities that are shared in the Operation Battleship Application',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Matthew Caraway',
     author_email='matthew@CarawayLabs.com',
```

