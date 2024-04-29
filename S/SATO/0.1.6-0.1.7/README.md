# Comparing `tmp/SATO-0.1.6.tar.gz` & `tmp/SATO-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SATO-0.1.6.tar", last modified: Sun Apr 28 13:55:14 2024, max compression
+gzip compressed data, was "SATO-0.1.7.tar", last modified: Mon Apr 29 18:46:57 2024, max compression
```

## Comparing `SATO-0.1.6.tar` & `SATO-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 cwekesa   (1000) cwekesa   (1000)        0 2024-04-28 13:55:14.025518 SATO-0.1.6/
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     1069 2024-03-13 17:18:07.000000 SATO-0.1.6/LICENSE
--rw-r--r--   0 cwekesa   (1000) cwekesa   (1000)     6809 2024-04-28 13:55:14.025518 SATO-0.1.6/PKG-INFO
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     5669 2024-03-15 06:12:30.000000 SATO-0.1.6/README.md
-drwxrwxr-x   0 cwekesa   (1000) cwekesa   (1000)        0 2024-04-28 13:55:14.025518 SATO-0.1.6/SATO/
--rw-r--r--   0 cwekesa   (1000) cwekesa   (1000)    33330 2024-04-28 13:48:12.000000 SATO-0.1.6/SATO/SATO.py
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       43 2024-04-28 13:20:29.000000 SATO-0.1.6/SATO/__init__.py
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     2352 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/about_intro.txt
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     3197 2024-03-15 06:13:15.000000 SATO-0.1.6/SATO/help.txt
-drwxrwxr-x   0 cwekesa   (1000) cwekesa   (1000)        0 2024-04-28 13:55:14.025518 SATO-0.1.6/SATO/icons/
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)    22650 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/icons/download.png
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)   216311 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/icons/fasta.png
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     1354 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/icons/file.png
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)    53857 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/icons/logo-no-background.png
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)    67297 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/icons/sato.png
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)      512 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/stylesheet.css
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     3298 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/validation.py
-drwxrwxr-x   0 cwekesa   (1000) cwekesa   (1000)        0 2024-04-28 13:55:14.025518 SATO-0.1.6/SATO.egg-info/
--rw-r--r--   0 cwekesa   (1000) cwekesa   (1000)     6809 2024-04-28 13:55:13.000000 SATO-0.1.6/SATO.egg-info/PKG-INFO
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)      436 2024-04-28 13:55:14.000000 SATO-0.1.6/SATO.egg-info/SOURCES.txt
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)        1 2024-04-28 13:55:13.000000 SATO-0.1.6/SATO.egg-info/dependency_links.txt
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       40 2024-04-28 13:55:13.000000 SATO-0.1.6/SATO.egg-info/entry_points.txt
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       16 2024-04-28 13:55:13.000000 SATO-0.1.6/SATO.egg-info/requires.txt
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)        5 2024-04-28 13:55:13.000000 SATO-0.1.6/SATO.egg-info/top_level.txt
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       70 2024-03-13 17:18:07.000000 SATO-0.1.6/run.py
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       38 2024-04-28 13:55:14.029518 SATO-0.1.6/setup.cfg
--rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     1729 2024-04-28 13:20:15.000000 SATO-0.1.6/setup.py
+drwxrwxr-x   0 cwekesa   (1000) cwekesa   (1000)        0 2024-04-29 18:46:57.716704 SATO-0.1.7/
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     1069 2024-03-13 17:18:07.000000 SATO-0.1.7/LICENSE
+-rw-r--r--   0 cwekesa   (1000) cwekesa   (1000)     6809 2024-04-29 18:46:57.716704 SATO-0.1.7/PKG-INFO
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     5669 2024-03-15 06:12:30.000000 SATO-0.1.7/README.md
+drwxrwxr-x   0 cwekesa   (1000) cwekesa   (1000)        0 2024-04-29 18:46:57.716704 SATO-0.1.7/SATO/
+-rw-r--r--   0 cwekesa   (1000) cwekesa   (1000)    33331 2024-04-29 18:12:03.000000 SATO-0.1.7/SATO/SATO.py
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       43 2024-04-29 18:46:15.000000 SATO-0.1.7/SATO/__init__.py
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     2352 2024-03-13 17:18:07.000000 SATO-0.1.7/SATO/about_intro.txt
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     3197 2024-03-15 06:13:15.000000 SATO-0.1.7/SATO/help.txt
+drwxrwxr-x   0 cwekesa   (1000) cwekesa   (1000)        0 2024-04-29 18:46:57.716704 SATO-0.1.7/SATO/icons/
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)    22650 2024-03-13 17:18:07.000000 SATO-0.1.7/SATO/icons/download.png
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)   216311 2024-03-13 17:18:07.000000 SATO-0.1.7/SATO/icons/fasta.png
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     1354 2024-03-13 17:18:07.000000 SATO-0.1.7/SATO/icons/file.png
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)    53857 2024-03-13 17:18:07.000000 SATO-0.1.7/SATO/icons/logo-no-background.png
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)    67297 2024-03-13 17:18:07.000000 SATO-0.1.7/SATO/icons/sato.png
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)      512 2024-03-13 17:18:07.000000 SATO-0.1.7/SATO/stylesheet.css
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     3298 2024-03-13 17:18:07.000000 SATO-0.1.7/SATO/validation.py
+drwxrwxr-x   0 cwekesa   (1000) cwekesa   (1000)        0 2024-04-29 18:46:57.716704 SATO-0.1.7/SATO.egg-info/
+-rw-r--r--   0 cwekesa   (1000) cwekesa   (1000)     6809 2024-04-29 18:46:57.000000 SATO-0.1.7/SATO.egg-info/PKG-INFO
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)      436 2024-04-29 18:46:57.000000 SATO-0.1.7/SATO.egg-info/SOURCES.txt
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)        1 2024-04-29 18:46:57.000000 SATO-0.1.7/SATO.egg-info/dependency_links.txt
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       40 2024-04-29 18:46:57.000000 SATO-0.1.7/SATO.egg-info/entry_points.txt
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       16 2024-04-29 18:46:57.000000 SATO-0.1.7/SATO.egg-info/requires.txt
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)        5 2024-04-29 18:46:57.000000 SATO-0.1.7/SATO.egg-info/top_level.txt
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       70 2024-03-13 17:18:07.000000 SATO-0.1.7/run.py
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       38 2024-04-29 18:46:57.716704 SATO-0.1.7/setup.cfg
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     1729 2024-04-29 18:45:21.000000 SATO-0.1.7/setup.py
```

### Comparing `SATO-0.1.6/LICENSE` & `SATO-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `SATO-0.1.6/PKG-INFO` & `SATO-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SATO
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package that generates consensus sequence from the forward and reverse sequences, performs multiple sequence alignment of the fasta sequences, and generates phylogenetic trees using Bayesian and Maximum Likelihood Methods
 Home-page: https://github.com/clabe-wekesa/SATO
 Author: Clabe Wekesa
 Author-email: simiyu86wekesa@gmail.com
 License: MIT
 Keywords: consensus,alignment,phylogenetics,bioinformatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SATO-0.1.6/README.md` & `SATO-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `SATO-0.1.6/SATO/SATO.py` & `SATO-0.1.7/SATO/SATO.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from PyQt6.QtCore import Qt, QFile, QTextStream, QIODevice
 from Bio import SeqIO
 from Bio.Seq import Seq
 from Bio import AlignIO
 from io import StringIO
 import subprocess
 import shutil
-from validation import (
+from .validation import (
     is_protein_alignment, text_formatting,is_valid_fasta,
     is_fasta_aligned, is_valid_fasta
 )
 
 # Define a custom exception for your application
 class CustomError(Exception):
     def __init__(self, message):
```

### Comparing `SATO-0.1.6/SATO/about_intro.txt` & `SATO-0.1.7/SATO/about_intro.txt`

 * *Files identical despite different names*

### Comparing `SATO-0.1.6/SATO/help.txt` & `SATO-0.1.7/SATO/help.txt`

 * *Files identical despite different names*

### Comparing `SATO-0.1.6/SATO/icons/download.png` & `SATO-0.1.7/SATO/icons/download.png`

 * *Files identical despite different names*

### Comparing `SATO-0.1.6/SATO/icons/fasta.png` & `SATO-0.1.7/SATO/icons/fasta.png`

 * *Files identical despite different names*

### Comparing `SATO-0.1.6/SATO/icons/file.png` & `SATO-0.1.7/SATO/icons/file.png`

 * *Files identical despite different names*

### Comparing `SATO-0.1.6/SATO/icons/logo-no-background.png` & `SATO-0.1.7/SATO/icons/logo-no-background.png`

 * *Files identical despite different names*

### Comparing `SATO-0.1.6/SATO/icons/sato.png` & `SATO-0.1.7/SATO/icons/sato.png`

 * *Files identical despite different names*

### Comparing `SATO-0.1.6/SATO/stylesheet.css` & `SATO-0.1.7/SATO/stylesheet.css`

 * *Files identical despite different names*

### Comparing `SATO-0.1.6/SATO/validation.py` & `SATO-0.1.7/SATO/validation.py`

 * *Files identical despite different names*

### Comparing `SATO-0.1.6/SATO.egg-info/PKG-INFO` & `SATO-0.1.7/SATO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SATO
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package that generates consensus sequence from the forward and reverse sequences, performs multiple sequence alignment of the fasta sequences, and generates phylogenetic trees using Bayesian and Maximum Likelihood Methods
 Home-page: https://github.com/clabe-wekesa/SATO
 Author: Clabe Wekesa
 Author-email: simiyu86wekesa@gmail.com
 License: MIT
 Keywords: consensus,alignment,phylogenetics,bioinformatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SATO-0.1.6/setup.py` & `SATO-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for long description
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     LONG_DESCRIPTION = readme_file.read()
 
 setuptools.setup(
     name="SATO",
-    version="0.1.6",
+    version="0.1.7",
     description='Python package that generates consensus sequence from the forward and reverse sequences, performs multiple sequence alignment of the fasta sequences, and generates phylogenetic trees using Bayesian and Maximum Likelihood Methods',
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     license="MIT",
     author='Clabe Wekesa',
     author_email='simiyu86wekesa@gmail.com',
     url="https://github.com/clabe-wekesa/SATO",
```

