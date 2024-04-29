# Comparing `tmp/dataextractoroeg-0.3.5.tar.gz` & `tmp/dataextractoroeg-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.3.5.tar", last modified: Mon Apr 29 12:48:23 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.3.6.tar", last modified: Mon Apr 29 12:53:59 2024, max compression
```

## Comparing `dataextractoroeg-0.3.5.tar` & `dataextractoroeg-0.3.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 12:48:23.006582 dataextractoroeg-0.3.5/
--rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.3.5/.gitignore
-drwxrwxrwx   0        0        0        0 2024-04-29 12:48:23.000611 dataextractoroeg-0.3.5/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     3046 2024-04-29 12:48:22.000000 dataextractoroeg-0.3.5/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2024-04-29 12:48:22.000000 dataextractoroeg-0.3.5/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 12:48:22.000000 dataextractoroeg-0.3.5/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-29 12:48:22.000000 dataextractoroeg-0.3.5/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-29 12:48:22.000000 dataextractoroeg-0.3.5/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 12:48:22.000000 dataextractoroeg-0.3.5/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.3.5/LICENSE.txt
--rw-rw-rw-   0        0        0     3046 2024-04-29 12:48:23.003044 dataextractoroeg-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 12:48:22.976251 dataextractoroeg-0.3.5/doiExtractor/
-drwxrwxrwx   0        0        0        0 2024-04-29 12:48:22.984650 dataextractoroeg-0.3.5/doiExtractor/ExistingPapers/
--rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.3.5/doiExtractor/ExistingPapers/Papers.csv
--rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.3.5/doiExtractor/ExistingPapers/name_doi_papers.csv
-drwxrwxrwx   0        0        0        0 2024-04-29 12:48:22.994550 dataextractoroeg-0.3.5/doiExtractor/Outputs/
--rw-rw-rw-   0        0        0    14166 2024-04-26 10:27:22.000000 dataextractoroeg-0.3.5/doiExtractor/Outputs/dois.txt
--rw-rw-rw-   0        0        0    77928 2024-04-25 14:42:00.000000 dataextractoroeg-0.3.5/doiExtractor/Outputs/results.csv
--rw-rw-rw-   0        0        0   123715 2024-04-29 12:01:52.000000 dataextractoroeg-0.3.5/doiExtractor/Outputs/results.json
--rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.3.5/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     8046 2024-04-29 12:06:17.000000 dataextractoroeg-0.3.5/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2552 2024-04-29 12:47:23.000000 dataextractoroeg-0.3.5/doiExtractor/main.py
--rw-rw-rw-   0        0        0     4086 2024-04-29 11:57:15.000000 dataextractoroeg-0.3.5/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-04-29 12:48:23.007582 dataextractoroeg-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      560 2024-04-29 12:48:18.000000 dataextractoroeg-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:59.960645 dataextractoroeg-0.3.6/
+-rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.3.6/.gitignore
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:59.954148 dataextractoroeg-0.3.6/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     3046 2024-04-29 12:53:59.000000 dataextractoroeg-0.3.6/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2024-04-29 12:53:59.000000 dataextractoroeg-0.3.6/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:53:59.000000 dataextractoroeg-0.3.6/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-29 12:53:59.000000 dataextractoroeg-0.3.6/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-29 12:53:59.000000 dataextractoroeg-0.3.6/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-29 12:53:59.000000 dataextractoroeg-0.3.6/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.3.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     3046 2024-04-29 12:53:59.954148 dataextractoroeg-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:59.938717 dataextractoroeg-0.3.6/doiExtractor/
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:59.946900 dataextractoroeg-0.3.6/doiExtractor/ExistingPapers/
+-rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.3.6/doiExtractor/ExistingPapers/Papers.csv
+-rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.3.6/doiExtractor/ExistingPapers/name_doi_papers.csv
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:59.954148 dataextractoroeg-0.3.6/doiExtractor/Outputs/
+-rw-rw-rw-   0        0        0    14166 2024-04-26 10:27:22.000000 dataextractoroeg-0.3.6/doiExtractor/Outputs/dois.txt
+-rw-rw-rw-   0        0        0    77928 2024-04-25 14:42:00.000000 dataextractoroeg-0.3.6/doiExtractor/Outputs/results.csv
+-rw-rw-rw-   0        0        0   123715 2024-04-29 12:01:52.000000 dataextractoroeg-0.3.6/doiExtractor/Outputs/results.json
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.3.6/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     8046 2024-04-29 12:06:17.000000 dataextractoroeg-0.3.6/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2343 2024-04-29 12:52:36.000000 dataextractoroeg-0.3.6/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     4086 2024-04-29 11:57:15.000000 dataextractoroeg-0.3.6/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-04-29 12:53:59.960645 dataextractoroeg-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      560 2024-04-29 12:53:17.000000 dataextractoroeg-0.3.6/setup.py
```

### Comparing `dataextractoroeg-0.3.5/DataExtractorOEG.egg-info/PKG-INFO` & `dataextractoroeg-0.3.6/DataExtractorOEG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.3.5
+Version: 0.3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.3.5/DataExtractorOEG.egg-info/SOURCES.txt` & `dataextractoroeg-0.3.6/DataExtractorOEG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.5/LICENSE.txt` & `dataextractoroeg-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.5/PKG-INFO` & `dataextractoroeg-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.3.5
+Version: 0.3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.3.5/README.md` & `dataextractoroeg-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.5/doiExtractor/ExistingPapers/Papers.csv` & `dataextractoroeg-0.3.6/doiExtractor/ExistingPapers/Papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.5/doiExtractor/ExistingPapers/name_doi_papers.csv` & `dataextractoroeg-0.3.6/doiExtractor/ExistingPapers/name_doi_papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.5/doiExtractor/Outputs/dois.txt` & `dataextractoroeg-0.3.6/doiExtractor/Outputs/dois.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.5/doiExtractor/Outputs/results.csv` & `dataextractoroeg-0.3.6/doiExtractor/Outputs/results.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.5/doiExtractor/Outputs/results.json` & `dataextractoroeg-0.3.6/doiExtractor/Outputs/results.json`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.5/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.3.6/doiExtractor/doiExtractor.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.5/doiExtractor/main.py` & `dataextractoroeg-0.3.6/doiExtractor/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from doiExtractor.doiExtractor import search_papers, merge_csv, remove_duplicates, csv_to_json, create_txt
 from doiExtractor.openAlex import add_primary_location_to_csv
-from doiExtractor import search_papers, merge_csv, remove_duplicates, create_txt, csv_to_json
-from openAlex import add_primary_location_to_csv
 import argparse
 import logging
 import os
-from doiExtractor.doiExtractor import search_papers, merge_csv
 
 logging.basicConfig(level=logging.INFO)
 
 def cli():
     parser = argparse.ArgumentParser(description="DOI Extractor Tool")
     parser.add_argument("--start", action="store_true", help="Start the extraction process")
     parser.add_argument("--url", default="https://portalcientifico.upm.es/es/ipublic/entity/16247", help="URL to extract DOIs from")
```

### Comparing `dataextractoroeg-0.3.5/doiExtractor/openAlex.py` & `dataextractoroeg-0.3.6/doiExtractor/openAlex.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.5/setup.py` & `dataextractoroeg-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.3.5",
+    version="0.3.6",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
         "pandas"
     ],
```

