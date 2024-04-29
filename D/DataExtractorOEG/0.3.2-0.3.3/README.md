# Comparing `tmp/dataextractoroeg-0.3.2.tar.gz` & `tmp/dataextractoroeg-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.3.2.tar", last modified: Fri Apr 26 11:55:50 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.3.3.tar", last modified: Mon Apr 29 12:14:07 2024, max compression
```

## Comparing `dataextractoroeg-0.3.2.tar` & `dataextractoroeg-0.3.3.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 11:55:50.815449 dataextractoroeg-0.3.2/
--rw-rw-rw-   0        0        0       72 2024-04-25 13:36:35.000000 dataextractoroeg-0.3.2/.gitignore
-drwxrwxrwx   0        0        0        0 2024-04-26 11:55:50.811438 dataextractoroeg-0.3.2/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     2916 2024-04-26 11:55:50.000000 dataextractoroeg-0.3.2/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2024-04-26 11:55:50.000000 dataextractoroeg-0.3.2/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 11:55:50.000000 dataextractoroeg-0.3.2/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-26 11:55:50.000000 dataextractoroeg-0.3.2/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-26 11:55:50.000000 dataextractoroeg-0.3.2/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-26 11:55:50.000000 dataextractoroeg-0.3.2/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2916 2024-04-26 11:55:50.813448 dataextractoroeg-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2677 2024-04-26 10:19:16.000000 dataextractoroeg-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 11:55:50.791107 dataextractoroeg-0.3.2/dist/
--rw-rw-rw-   0        0        0     7779 2024-04-25 14:20:01.000000 dataextractoroeg-0.3.2/dist/DataExtractorOEG-0.3.1-py3-none-any.whl
--rw-rw-rw-   0        0        0     6548 2024-04-25 14:20:01.000000 dataextractoroeg-0.3.2/dist/dataextractoroeg-0.3.1.tar.gz
-drwxrwxrwx   0        0        0        0 2024-04-26 11:55:50.798411 dataextractoroeg-0.3.2/doiExtractor/
-drwxrwxrwx   0        0        0        0 2024-04-26 11:55:50.804424 dataextractoroeg-0.3.2/doiExtractor/ExistingPapers/
--rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.3.2/doiExtractor/ExistingPapers/Papers.csv
--rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.3.2/doiExtractor/ExistingPapers/name_doi_papers.csv
-drwxrwxrwx   0        0        0        0 2024-04-26 11:55:50.809172 dataextractoroeg-0.3.2/doiExtractor/Outputs/
--rw-rw-rw-   0        0        0    14166 2024-04-26 10:27:22.000000 dataextractoroeg-0.3.2/doiExtractor/Outputs/dois.txt
--rw-rw-rw-   0        0        0    77928 2024-04-25 14:42:00.000000 dataextractoroeg-0.3.2/doiExtractor/Outputs/name_doi.csv
--rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.3.2/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     5989 2024-04-22 09:37:48.000000 dataextractoroeg-0.3.2/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2183 2024-04-26 10:20:30.000000 dataextractoroeg-0.3.2/doiExtractor/main.py
--rw-rw-rw-   0        0        0     5998 2024-04-26 11:52:51.000000 dataextractoroeg-0.3.2/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-04-26 11:55:50.816460 dataextractoroeg-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      560 2024-04-26 10:20:45.000000 dataextractoroeg-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:14:07.396129 dataextractoroeg-0.3.3/
+-rw-rw-rw-   0        0        0       72 2024-04-29 12:10:47.000000 dataextractoroeg-0.3.3/.gitignore
+drwxrwxrwx   0        0        0        0 2024-04-29 12:14:07.391143 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     3046 2024-04-29 12:14:06.000000 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2024-04-29 12:14:06.000000 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:14:06.000000 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-29 12:14:06.000000 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-29 12:14:06.000000 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-29 12:14:06.000000 dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3046 2024-04-29 12:14:07.393274 dataextractoroeg-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 12:14:07.277847 dataextractoroeg-0.3.3/dist/
+-rw-rw-rw-   0        0        0     7779 2024-04-25 14:20:01.000000 dataextractoroeg-0.3.3/dist/DataExtractorOEG-0.3.1-py3-none-any.whl
+-rw-rw-rw-   0        0        0     6548 2024-04-25 14:20:01.000000 dataextractoroeg-0.3.3/dist/dataextractoroeg-0.3.1.tar.gz
+drwxrwxrwx   0        0        0        0 2024-04-29 12:14:07.341493 dataextractoroeg-0.3.3/doiExtractor/
+drwxrwxrwx   0        0        0        0 2024-04-29 12:14:07.382621 dataextractoroeg-0.3.3/doiExtractor/ExistingPapers/
+-rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.3.3/doiExtractor/ExistingPapers/Papers.csv
+-rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.3.3/doiExtractor/ExistingPapers/name_doi_papers.csv
+drwxrwxrwx   0        0        0        0 2024-04-29 12:14:07.387751 dataextractoroeg-0.3.3/doiExtractor/Outputs/
+-rw-rw-rw-   0        0        0    14166 2024-04-26 10:27:22.000000 dataextractoroeg-0.3.3/doiExtractor/Outputs/dois.txt
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.3.3/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     8046 2024-04-29 12:06:17.000000 dataextractoroeg-0.3.3/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2358 2024-04-29 12:09:22.000000 dataextractoroeg-0.3.3/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     4086 2024-04-29 11:57:15.000000 dataextractoroeg-0.3.3/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-04-29 12:14:07.397751 dataextractoroeg-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      560 2024-04-29 12:11:40.000000 dataextractoroeg-0.3.3/setup.py
```

### Comparing `dataextractoroeg-0.3.2/DataExtractorOEG.egg-info/PKG-INFO` & `dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.3.2
+Version: 0.3.3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
 
@@ -21,28 +21,31 @@
 1) https://portalcientifico.upm.es/es/ipublic/entity/16247 , corresponding to all papers from OEG. 
 
 2) ExistingPapers/ Papers.csv with already extracted data from some OEG papers.
 
 <br>
 The resulting information is placed in Outputs folder, which include:
 
-- A dois.txt containing, for each paper, the pdf if it was founded or if not the doi
+- A dois.txt containing, for each paper, the URL to the pdf if it was founded or if not the doi
 
-- A name-doi.csv, containing the title and the doi of every paper found, in addition to OpenAlex primary location attribute
+- A results.csv, containing the title and the doi of every paper found, in addition to OpenAlex primary location attribute
+
+- A results.json, containing the same information as results.csv but in a json formal
 
 ## Project Structure
 ```
 DOI-Extractor-OEG
 ├───doiExtractor
 |   ├───ExistingPapers
 |   |   ├───name_doi_papers.csv
 |   |   └───Papers.csv
 |   ├───Outputs
 |   |   ├───dois.csv
-|   |   └───name_doi.csv
+|   |   |───results.csv
+|   |   └───results.json
 |   ├───__init__.py
 |   ├───doiExtractor.py
 |   ├───main.py
 |   └───openAlex.py
 ├───.gitignore
 ├───LICENSE.txt
 ├───README.MD
```

### Comparing `dataextractoroeg-0.3.2/DataExtractorOEG.egg-info/SOURCES.txt` & `dataextractoroeg-0.3.3/DataExtractorOEG.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,9 +12,8 @@
 dist/dataextractoroeg-0.3.1.tar.gz
 doiExtractor/__init__.py
 doiExtractor/doiExtractor.py
 doiExtractor/main.py
 doiExtractor/openAlex.py
 doiExtractor/ExistingPapers/Papers.csv
 doiExtractor/ExistingPapers/name_doi_papers.csv
-doiExtractor/Outputs/dois.txt
-doiExtractor/Outputs/name_doi.csv
+doiExtractor/Outputs/dois.txt
```

### Comparing `dataextractoroeg-0.3.2/LICENSE.txt` & `dataextractoroeg-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.2/PKG-INFO` & `dataextractoroeg-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.3.2
+Version: 0.3.3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
 
@@ -21,28 +21,31 @@
 1) https://portalcientifico.upm.es/es/ipublic/entity/16247 , corresponding to all papers from OEG. 
 
 2) ExistingPapers/ Papers.csv with already extracted data from some OEG papers.
 
 <br>
 The resulting information is placed in Outputs folder, which include:
 
-- A dois.txt containing, for each paper, the pdf if it was founded or if not the doi
+- A dois.txt containing, for each paper, the URL to the pdf if it was founded or if not the doi
 
-- A name-doi.csv, containing the title and the doi of every paper found, in addition to OpenAlex primary location attribute
+- A results.csv, containing the title and the doi of every paper found, in addition to OpenAlex primary location attribute
+
+- A results.json, containing the same information as results.csv but in a json formal
 
 ## Project Structure
 ```
 DOI-Extractor-OEG
 ├───doiExtractor
 |   ├───ExistingPapers
 |   |   ├───name_doi_papers.csv
 |   |   └───Papers.csv
 |   ├───Outputs
 |   |   ├───dois.csv
-|   |   └───name_doi.csv
+|   |   |───results.csv
+|   |   └───results.json
 |   ├───__init__.py
 |   ├───doiExtractor.py
 |   ├───main.py
 |   └───openAlex.py
 ├───.gitignore
 ├───LICENSE.txt
 ├───README.MD
```

### Comparing `dataextractoroeg-0.3.2/README.md` & `dataextractoroeg-0.3.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,28 +11,31 @@
 1) https://portalcientifico.upm.es/es/ipublic/entity/16247 , corresponding to all papers from OEG. 
 
 2) ExistingPapers/ Papers.csv with already extracted data from some OEG papers.
 
 <br>
 The resulting information is placed in Outputs folder, which include:
 
-- A dois.txt containing, for each paper, the pdf if it was founded or if not the doi
+- A dois.txt containing, for each paper, the URL to the pdf if it was founded or if not the doi
 
-- A name-doi.csv, containing the title and the doi of every paper found, in addition to OpenAlex primary location attribute
+- A results.csv, containing the title and the doi of every paper found, in addition to OpenAlex primary location attribute
+
+- A results.json, containing the same information as results.csv but in a json formal
 
 ## Project Structure
 ```
 DOI-Extractor-OEG
 ├───doiExtractor
 |   ├───ExistingPapers
 |   |   ├───name_doi_papers.csv
 |   |   └───Papers.csv
 |   ├───Outputs
 |   |   ├───dois.csv
-|   |   └───name_doi.csv
+|   |   |───results.csv
+|   |   └───results.json
 |   ├───__init__.py
 |   ├───doiExtractor.py
 |   ├───main.py
 |   └───openAlex.py
 ├───.gitignore
 ├───LICENSE.txt
 ├───README.MD
```

### Comparing `dataextractoroeg-0.3.2/dist/DataExtractorOEG-0.3.1-py3-none-any.whl` & `dataextractoroeg-0.3.3/dist/DataExtractorOEG-0.3.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.2/dist/dataextractoroeg-0.3.1.tar.gz` & `dataextractoroeg-0.3.3/dist/dataextractoroeg-0.3.1.tar.gz`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.2/doiExtractor/ExistingPapers/Papers.csv` & `dataextractoroeg-0.3.3/doiExtractor/ExistingPapers/Papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.2/doiExtractor/ExistingPapers/name_doi_papers.csv` & `dataextractoroeg-0.3.3/doiExtractor/ExistingPapers/name_doi_papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.2/doiExtractor/Outputs/dois.txt` & `dataextractoroeg-0.3.3/doiExtractor/Outputs/dois.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.2/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.3.3/doiExtractor/doiExtractor.py`

 * *Files 23% similar despite different names*

```diff
@@ -147,8 +147,48 @@
         reader = csv.reader(papers_file)
         next(reader)  # Skip header row
         with open(csv1, 'a', newline='', encoding='utf-8') as existing_csv_file:
             csv_writer = csv.writer(existing_csv_file)
             for row in reader:
                 doi = row[1]
                 if doi not in existing_dois:
-                    csv_writer.writerow(row)
+                    csv_writer.writerow(row)
+
+
+def create_txt(csv_filename, txt_filename):
+    print("\nCreating the .txt with the .pdf or doi\n")
+    with open(csv_filename, mode='r', newline='', encoding='utf-8') as file:
+        reader = csv.DictReader(file)
+        with open(txt_filename, mode='w', encoding='utf-8') as output_file:
+            for row in reader:
+                name = row.get("NAME")
+                doi = row.get("DOI")
+                primary_location = row.get("PRIMARY_LOCATION")
+                if primary_location != "":
+                    try:
+                        response = requests.head(primary_location, allow_redirects=True)
+                        final_url = response.url
+                        parsed_url = urllib.parse.urlparse(final_url)
+                        if parsed_url.path.endswith('.pdf'):
+                            output_file.write(primary_location + "\n")
+                            print(f"Found pdf for {name}: {primary_location}")
+                            print("-----------------------------------------------------------------")
+                            continue
+                        else:
+                            if doi != "" and doi.startswith('10'):
+                                output_file.write(doi + "\n")
+                                print(f"No pdf found for {name}, wrote DOI instead: {doi}")
+                            else:
+                                print(f"No pdf or DOI found for {name}")
+                    except requests.RequestException:
+                        pass
+                elif doi != "" and doi.startswith('10'):
+                    output_file.write(doi + "\n")
+                    print(f"No pdf found for {name}, wrote DOI instead: {doi}")
+                else:
+                    print(f"No pdf or DOI found for {name}")
+                print("-----------------------------------------------------------------")
+
+
+def csv_to_json(csv_file, json_file):
+    df = pd.read_csv(csv_file)
+    df.to_json(json_file, orient='records', indent=4)
```

### Comparing `dataextractoroeg-0.3.2/doiExtractor/main.py` & `dataextractoroeg-0.3.3/doiExtractor/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from doiExtractor.doiExtractor import search_papers, merge_csv, remove_duplicates
-from doiExtractor.openAlex import add_primary_location_to_csv, create_txt
+from doiExtractor.doiExtractor import search_papers, merge_csv, remove_duplicates, create_txt, csv_to_json
+from doiExtractor.openAlex import add_primary_location_to_csv
 import argparse
 import logging
 import os
 
 from doiExtractor.doiExtractor import search_papers, merge_csv
 
 logging.basicConfig(level=logging.INFO)
@@ -16,16 +16,17 @@
     args = parser.parse_args()
 
     if args.start:
         url = args.url + "#14"
         url_docs = args.url
 
         # Files to write the output
-        csv_filename = args.output + "/name_doi.csv"
         txt_filename = args.output + "/dois.txt"
+        csv_filename = args.output + "/results.csv"
+        json_filename = args.output + "/results.json"
 
         # ExistingPapers
         papers = "doiExtractor/ExistingPapers/name_doi_papers.csv"
 
         logging.info("DOI Extractor Tool started")
         logging.info(f"Search in: {url}, Output csv: {csv_filename}, Output txt: {txt_filename}")
 
@@ -46,10 +47,13 @@
 
         # Add URLs from OpenAlex
         add_primary_location_to_csv(csv_filename)
 
         # After adding missing dois with OpenAlex, create the .txt file containing the .pdf if it was found or the DOI if it wasn't
         create_txt(csv_filename, txt_filename)
 
+        # Create a JSON with the information extracted
+        csv_to_json(csv_filename, json_filename)
+
         logging.info(f"Data saved to {csv_filename} and {txt_filename}")
     else:
         logging.info("Use --start flag to start the extraction process")
```

### Comparing `dataextractoroeg-0.3.2/doiExtractor/openAlex.py` & `dataextractoroeg-0.3.3/doiExtractor/openAlex.py`

 * *Files 20% similar despite different names*

```diff
@@ -93,41 +93,7 @@
         new_columns.append("PRIMARY_LOCATION")
 
     with open(csv_filename, mode='w', newline='', encoding='utf-8') as file:
         writer = csv.DictWriter(file, fieldnames=new_columns)
         writer.writeheader()
         writer.writerows(rows)
 
-
-def create_txt(csv_filename, txt_filename):
-    print("\nCreating the .txt with the .pdf or doi\n")
-    with open(csv_filename, mode='r', newline='', encoding='utf-8') as file:
-        reader = csv.DictReader(file)
-        with open(txt_filename, mode='w', encoding='utf-8') as output_file:
-            for row in reader:
-                name = row.get("NAME")
-                doi = row.get("DOI")
-                primary_location = row.get("PRIMARY_LOCATION")
-                if primary_location != "":
-                    try:
-                        response = requests.head(primary_location, allow_redirects=True)
-                        final_url = response.url
-                        parsed_url = urlparse(final_url)
-                        if parsed_url.path.endswith('.pdf'):
-                            output_file.write(primary_location + "\n")
-                            print(f"Found pdf for {name}: {primary_location}")
-                            print("-----------------------------------------------------------------")
-                            continue
-                        else:
-                            if doi != "" and doi.startswith('10'):
-                                output_file.write(doi + "\n")
-                                print(f"No pdf found for {name}, wrote DOI instead: {doi}")
-                            else:
-                                print(f"No pdf or DOI found for {name}")
-                    except requests.RequestException:
-                        pass
-                elif doi != "" and doi.startswith('10'):
-                    output_file.write(doi + "\n")
-                    print(f"No pdf found for {name}, wrote DOI instead: {doi}")
-                else:
-                    print(f"No pdf or DOI found for {name}")
-                print("-----------------------------------------------------------------")
```

### Comparing `dataextractoroeg-0.3.2/setup.py` & `dataextractoroeg-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.3.2",
+    version="0.3.3",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
         "pandas"
     ],
```

