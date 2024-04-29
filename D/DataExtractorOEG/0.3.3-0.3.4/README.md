# Comparing `tmp/dataextractoroeg-0.3.3.tar.gz` & `tmp/dataextractoroeg-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.3.3.tar", last modified: Mon Apr 29 12:14:07 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.3.4.tar", last modified: Mon Apr 29 12:41:27 2024, max compression
```

## Comparing `dataextractoroeg-0.3.3.tar` & `dataextractoroeg-0.3.4.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 12:14:07.396129 dataextractoroeg-0.3.3/
--rw-rw-rw-   0        0        0       72 2024-04-29 12:10:47.000000 dataextractoroeg-0.3.3/.gitignore
-drwxrwxrwx   0        0        0        0 2024-04-29 12:14:07.391143 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     3046 2024-04-29 12:14:06.000000 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      580 2024-04-29 12:14:06.000000 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 12:14:06.000000 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-29 12:14:06.000000 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-29 12:14:06.000000 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 12:14:06.000000 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3046 2024-04-29 12:14:07.393274 dataextractoroeg-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 12:14:07.277847 dataextractoroeg-0.3.3/dist/
--rw-rw-rw-   0        0        0     7779 2024-04-25 14:20:01.000000 dataextractoroeg-0.3.3/dist/DataExtractorOEG-0.3.1-py3-none-any.whl
--rw-rw-rw-   0        0        0     6548 2024-04-25 14:20:01.000000 dataextractoroeg-0.3.3/dist/dataextractoroeg-0.3.1.tar.gz
-drwxrwxrwx   0        0        0        0 2024-04-29 12:14:07.341493 dataextractoroeg-0.3.3/doiExtractor/
-drwxrwxrwx   0        0        0        0 2024-04-29 12:14:07.382621 dataextractoroeg-0.3.3/doiExtractor/ExistingPapers/
--rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.3.3/doiExtractor/ExistingPapers/Papers.csv
--rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.3.3/doiExtractor/ExistingPapers/name_doi_papers.csv
-drwxrwxrwx   0        0        0        0 2024-04-29 12:14:07.387751 dataextractoroeg-0.3.3/doiExtractor/Outputs/
--rw-rw-rw-   0        0        0    14166 2024-04-26 10:27:22.000000 dataextractoroeg-0.3.3/doiExtractor/Outputs/dois.txt
--rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.3.3/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     8046 2024-04-29 12:06:17.000000 dataextractoroeg-0.3.3/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2358 2024-04-29 12:09:22.000000 dataextractoroeg-0.3.3/doiExtractor/main.py
--rw-rw-rw-   0        0        0     4086 2024-04-29 11:57:15.000000 dataextractoroeg-0.3.3/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-04-29 12:14:07.397751 dataextractoroeg-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      560 2024-04-29 12:11:40.000000 dataextractoroeg-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:41:27.671634 dataextractoroeg-0.3.4/
+-rw-rw-rw-   0        0        0       72 2024-04-29 12:32:52.000000 dataextractoroeg-0.3.4/.gitignore
+drwxrwxrwx   0        0        0        0 2024-04-29 12:41:27.664742 dataextractoroeg-0.3.4/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     3046 2024-04-29 12:41:27.000000 dataextractoroeg-0.3.4/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2024-04-29 12:41:27.000000 dataextractoroeg-0.3.4/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:41:27.000000 dataextractoroeg-0.3.4/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-29 12:41:27.000000 dataextractoroeg-0.3.4/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-29 12:41:27.000000 dataextractoroeg-0.3.4/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-29 12:41:27.000000 dataextractoroeg-0.3.4/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3046 2024-04-29 12:41:27.666747 dataextractoroeg-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 12:41:27.641499 dataextractoroeg-0.3.4/doiExtractor/
+drwxrwxrwx   0        0        0        0 2024-04-29 12:41:27.649812 dataextractoroeg-0.3.4/doiExtractor/ExistingPapers/
+-rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.3.4/doiExtractor/ExistingPapers/Papers.csv
+-rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.3.4/doiExtractor/ExistingPapers/name_doi_papers.csv
+drwxrwxrwx   0        0        0        0 2024-04-29 12:41:27.660416 dataextractoroeg-0.3.4/doiExtractor/Outputs/
+-rw-rw-rw-   0        0        0    14166 2024-04-26 10:27:22.000000 dataextractoroeg-0.3.4/doiExtractor/Outputs/dois.txt
+-rw-rw-rw-   0        0        0    77928 2024-04-25 14:42:00.000000 dataextractoroeg-0.3.4/doiExtractor/Outputs/results.csv
+-rw-rw-rw-   0        0        0   123715 2024-04-29 12:01:52.000000 dataextractoroeg-0.3.4/doiExtractor/Outputs/results.json
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.3.4/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     8046 2024-04-29 12:06:17.000000 dataextractoroeg-0.3.4/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2317 2024-04-29 12:38:58.000000 dataextractoroeg-0.3.4/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     4086 2024-04-29 11:57:15.000000 dataextractoroeg-0.3.4/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-04-29 12:41:27.671920 dataextractoroeg-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      560 2024-04-29 12:31:13.000000 dataextractoroeg-0.3.4/setup.py
```

### Comparing `dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/PKG-INFO` & `dataextractoroeg-0.3.4/DataExtractorOEG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.3.3
+Version: 0.3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/SOURCES.txt` & `dataextractoroeg-0.3.4/DataExtractorOEG.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 setup.py
 DataExtractorOEG.egg-info/PKG-INFO
 DataExtractorOEG.egg-info/SOURCES.txt
 DataExtractorOEG.egg-info/dependency_links.txt
 DataExtractorOEG.egg-info/entry_points.txt
 DataExtractorOEG.egg-info/requires.txt
 DataExtractorOEG.egg-info/top_level.txt
-dist/DataExtractorOEG-0.3.1-py3-none-any.whl
-dist/dataextractoroeg-0.3.1.tar.gz
 doiExtractor/__init__.py
 doiExtractor/doiExtractor.py
 doiExtractor/main.py
 doiExtractor/openAlex.py
 doiExtractor/ExistingPapers/Papers.csv
 doiExtractor/ExistingPapers/name_doi_papers.csv
-doiExtractor/Outputs/dois.txt
+doiExtractor/Outputs/dois.txt
+doiExtractor/Outputs/results.csv
+doiExtractor/Outputs/results.json
```

### Comparing `dataextractoroeg-0.3.3/LICENSE.txt` & `dataextractoroeg-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.3/PKG-INFO` & `dataextractoroeg-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.3.3
+Version: 0.3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.3.3/README.md` & `dataextractoroeg-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.3/doiExtractor/ExistingPapers/Papers.csv` & `dataextractoroeg-0.3.4/doiExtractor/ExistingPapers/Papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.3/doiExtractor/ExistingPapers/name_doi_papers.csv` & `dataextractoroeg-0.3.4/doiExtractor/ExistingPapers/name_doi_papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.3/doiExtractor/Outputs/dois.txt` & `dataextractoroeg-0.3.4/doiExtractor/Outputs/dois.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.3/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.3.4/doiExtractor/doiExtractor.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.3/doiExtractor/main.py` & `dataextractoroeg-0.3.4/doiExtractor/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from doiExtractor.doiExtractor import search_papers, merge_csv, remove_duplicates, create_txt, csv_to_json
-from doiExtractor.openAlex import add_primary_location_to_csv
+from doiExtractor import search_papers, merge_csv, remove_duplicates, create_txt, csv_to_json
+from openAlex import add_primary_location_to_csv
 import argparse
 import logging
 import os
 
-from doiExtractor.doiExtractor import search_papers, merge_csv
-
 logging.basicConfig(level=logging.INFO)
 
 def cli():
     parser = argparse.ArgumentParser(description="DOI Extractor Tool")
     parser.add_argument("--start", action="store_true", help="Start the extraction process")
     parser.add_argument("--url", default="https://portalcientifico.upm.es/es/ipublic/entity/16247", help="URL to extract DOIs from")
     parser.add_argument("--output", default="doiExtractor/Outputs", help="File path for the outputs")
@@ -20,14 +18,16 @@
         url_docs = args.url
 
         # Files to write the output
         txt_filename = args.output + "/dois.txt"
         csv_filename = args.output + "/results.csv"
         json_filename = args.output + "/results.json"
 
+        os.makedirs(args.output, exist_ok=True)
+
         # ExistingPapers
         papers = "doiExtractor/ExistingPapers/name_doi_papers.csv"
 
         logging.info("DOI Extractor Tool started")
         logging.info(f"Search in: {url}, Output csv: {csv_filename}, Output txt: {txt_filename}")
 
         # Delete contents of the files if already created
```

### Comparing `dataextractoroeg-0.3.3/doiExtractor/openAlex.py` & `dataextractoroeg-0.3.4/doiExtractor/openAlex.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.3/setup.py` & `dataextractoroeg-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.3.3",
+    version="0.3.4",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
         "pandas"
     ],
```

