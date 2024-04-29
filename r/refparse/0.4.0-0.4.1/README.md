# Comparing `tmp/refparse-0.4.0.tar.gz` & `tmp/refparse-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refparse-0.4.0.tar", last modified: Sun Apr 28 04:39:03 2024, max compression
+gzip compressed data, was "refparse-0.4.1.tar", last modified: Mon Apr 29 14:50:01 2024, max compression
```

## Comparing `refparse-0.4.0.tar` & `refparse-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:39:03.654750 refparse-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-28 04:38:54.000000 refparse-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-28 04:39:03.654750 refparse-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-28 04:38:54.000000 refparse-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-28 04:38:54.000000 refparse-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:39:03.654750 refparse-0.4.0/refparse/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-28 04:38:54.000000 refparse-0.4.0/refparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-04-28 04:38:54.000000 refparse-0.4.0/refparse/cssci.py
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-28 04:38:54.000000 refparse-0.4.0/refparse/scopus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-28 04:38:54.000000 refparse-0.4.0/refparse/wos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:39:03.654750 refparse-0.4.0/refparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-28 04:39:03.000000 refparse-0.4.0/refparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-28 04:39:03.000000 refparse-0.4.0/refparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 04:39:03.000000 refparse-0.4.0/refparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 04:39:03.000000 refparse-0.4.0/refparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 04:39:03.654750 refparse-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:39:03.654750 refparse-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13114 2024-04-28 04:38:54.000000 refparse-0.4.0/tests/test_cssci.py
--rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-04-28 04:38:54.000000 refparse-0.4.0/tests/test_scopus.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-28 04:38:54.000000 refparse-0.4.0/tests/test_wos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:50:01.497932 refparse-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-29 14:49:57.000000 refparse-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-29 14:50:01.497932 refparse-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-29 14:49:57.000000 refparse-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-29 14:49:57.000000 refparse-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:50:01.497932 refparse-0.4.1/refparse/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-29 14:49:57.000000 refparse-0.4.1/refparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-04-29 14:49:57.000000 refparse-0.4.1/refparse/cssci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-29 14:49:57.000000 refparse-0.4.1/refparse/scopus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-29 14:49:57.000000 refparse-0.4.1/refparse/wos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:50:01.497932 refparse-0.4.1/refparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-29 14:50:01.000000 refparse-0.4.1/refparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-29 14:50:01.000000 refparse-0.4.1/refparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:50:01.000000 refparse-0.4.1/refparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 14:50:01.000000 refparse-0.4.1/refparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:50:01.497932 refparse-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:50:01.497932 refparse-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13114 2024-04-29 14:49:57.000000 refparse-0.4.1/tests/test_cssci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-04-29 14:49:57.000000 refparse-0.4.1/tests/test_scopus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-04-29 14:49:57.000000 refparse-0.4.1/tests/test_wos.py
```

### Comparing `refparse-0.4.0/LICENSE` & `refparse-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `refparse-0.4.0/PKG-INFO` & `refparse-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refparse
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python library to parse bibliographic references
 Author-email: WangK2 <kw221225@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/doublessay/refparse
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `refparse-0.4.0/README.md` & `refparse-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `refparse-0.4.0/pyproject.toml` & `refparse-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `refparse-0.4.0/refparse/__init__.py` & `refparse-0.4.1/refparse/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 from typing import Literal, Optional
 from .wos import ParseWos
 from .scopus import ParseScopus
 from .cssci import ParseCssci
```

### Comparing `refparse-0.4.0/refparse/cssci.py` & `refparse-0.4.1/refparse/cssci.py`

 * *Files identical despite different names*

### Comparing `refparse-0.4.0/refparse/scopus.py` & `refparse-0.4.1/refparse/scopus.py`

 * *Files identical despite different names*

### Comparing `refparse-0.4.0/refparse/wos.py` & `refparse-0.4.1/refparse/wos.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,38 +17,43 @@
         # e.g. Afshinmanesh F, 2005, EUROCON 2005: THE INTERNATIONAL CONFERENCE ON COMPUTER AS A TOOL, VOL 1 AND 2 , PROCEEDINGS, P217
         ref = re.sub(r" ,", ",", ref)
         return ref
 
     def parse(self):
         if self.ref.startswith("[Anonymous]"):
             return None
+        if self.ref.count(", ") == 0:
+            return None
         elif "Patent No." in self.ref:
             return None
         elif re.search(r"\d{4}, \[", self.ref):
             return self.parse_bilingual()
         else:
             return self.parse_general()
 
     @staticmethod
     def extract_doi(entry: str) -> Optional[str]:
         """Extract DOI from a reference entry."""
+        doi = None
         if ", DOI [" in entry:
             doi_part = re.split(r", DOI (?=\[)", entry, maxsplit=1)[1]
             doi_list = doi_part.strip("[]").split(", ")
             doi_set = set(doi.replace("DOI ", "").lower() for doi in doi_list)
             if len(doi_set) == 1:
                 doi = doi_set.pop()
             elif len(doi_set) > 1:
                 doi = "; ".join(doi_set)
         elif ", DOI " in entry:
             doi_match = re.search(r"DOI (10\..*)$", entry)
             if doi_match:
                 doi = doi_match.group(1).lower()
-        else:
-            doi = None
+            else:
+                doi_match = re.search(r"DOI (arXiv.*)$", entry)
+                if doi_match:
+                    doi = doi_match.group(1).lower()
         return doi
 
     @staticmethod
     def extract_page(entry: str) -> Optional[str]:
         """Extract page number from a reference entry."""
         page_match = re.search(r", p([A-Za-z\d]+)(?=, DOI|$)", entry, flags=re.I)
         page = page_match.group(1) if page_match else None
```

### Comparing `refparse-0.4.0/refparse.egg-info/PKG-INFO` & `refparse-0.4.1/refparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refparse
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python library to parse bibliographic references
 Author-email: WangK2 <kw221225@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/doublessay/refparse
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `refparse-0.4.0/tests/test_cssci.py` & `refparse-0.4.1/tests/test_cssci.py`

 * *Files identical despite different names*

### Comparing `refparse-0.4.0/tests/test_scopus.py` & `refparse-0.4.1/tests/test_scopus.py`

 * *Files identical despite different names*

### Comparing `refparse-0.4.0/tests/test_wos.py` & `refparse-0.4.1/tests/test_wos.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,18 @@
         "Jiang HM, 2017, NAT CHEM BIOL, V13, P994, DOI [10.1038/NCHEMBIO.2442, 10.1038/nchembio.2442]",
         "10.1038/nchembio.2442",
     ),
     (
         "Du K-K., 2013, J CHINA U POSTS TELE, V20, P96, DOI DOI 10.1016/S1005-8885(13)60240-X",
         "10.1016/s1005-8885(13)60240-x",
     ),
+    (
+        "Bahdanau D, 2016, Arxiv, DOI arXiv:1409.0473",
+        "arxiv:1409.0473",
+    ),
 ]
 
 test_page_data = [
     (
         "Habibi M, 2017, BIOINFORMATICS, V33, pI37, DOI 10.1093/bioinformatics/btx228",
         "I37",
     ),
@@ -203,14 +207,18 @@
 
 test_parse_data = [
     (
         "[Anonymous], 2017, NATURE, DOI DOI 10.1038/NATURE.2017.22094",
         None,
     ),
     (
+        "SILICON REPUBLIC NEW",
+        None,
+    ),
+    (
         "Dodd SK., 2013, Patent No. 2013/171639 A1",
         None,
     ),
     (
         "[张铁华 Zhang Tiehua], 2011, [吉林大学学报. 工学版, Journal of Jilin University. Engineering and Technology Edition], V41, P882",
         {
             "author": "Zhang Tiehua",
```

