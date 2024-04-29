# Comparing `tmp/connectedpapersextractor-0.1.2.tar.gz` & `tmp/connectedpapersextractor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectedpapersextractor-0.1.2.tar", max compression
+gzip compressed data, was "connectedpapersextractor-0.1.3.tar", max compression
```

## Comparing `connectedpapersextractor-0.1.2.tar` & `connectedpapersextractor-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1070 2024-04-23 21:01:05.479303 connectedpapersextractor-0.1.2/LICENSE
--rw-r--r--   0        0        0      644 2024-04-28 17:33:23.514920 connectedpapersextractor-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-27 22:23:56.499918 connectedpapersextractor-0.1.2/src/connectedpapersextractor/ArticleFilter.py
--rw-r--r--   0        0        0      183 2024-04-28 11:36:25.108943 connectedpapersextractor-0.1.2/src/connectedpapersextractor/Config.py
--rw-r--r--   0        0        0      374 2024-04-28 13:45:00.686988 connectedpapersextractor-0.1.2/src/connectedpapersextractor/MainPartsExtractor.py
--rw-r--r--   0        0        0     2127 2024-04-28 15:05:13.309963 connectedpapersextractor-0.1.2/src/connectedpapersextractor/PdfSummary.py
--rw-r--r--   0        0        0     2486 2024-04-28 13:45:00.750987 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_AIExtractor.py
--rw-r--r--   0        0        0      344 2024-04-28 13:39:32.895971 connectedpapersextractor-0.1.2/src/connectedpapersextractor/__init__.py
--rw-r--r--   0        0        0      724 2024-04-28 13:43:53.635611 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_add_docs.py
--rw-r--r--   0        0        0      872 2024-04-28 11:53:43.189003 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_combine_summaries.py
--rw-r--r--   0        0        0     2668 2024-04-28 15:05:13.301962 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_get_pdf_summaries.py
--rw-r--r--   0        0        0     1170 2024-04-28 16:50:24.953804 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_refine_documents.py
--rw-r--r--   0        0        0      768 2024-04-28 17:10:03.753179 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_stuff_documents.py
--rw-r--r--   0        0        0     1744 2024-04-28 17:26:44.686560 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_summarize_documents.py
--rw-r--r--   0        0        0     1530 2024-04-28 17:17:26.421933 connectedpapersextractor-0.1.2/src/connectedpapersextractor/create_related_work.py
--rw-r--r--   0        0        0     1450 2024-04-28 13:47:45.376986 connectedpapersextractor-0.1.2/src/connectedpapersextractor/get_summaries.py
--rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 connectedpapersextractor-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-23 21:01:05.479303 connectedpapersextractor-0.1.3/LICENSE
+-rw-r--r--   0        0        0      616 2024-04-29 13:13:20.196732 connectedpapersextractor-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-27 22:23:56.499918 connectedpapersextractor-0.1.3/src/connectedpapersextractor/ArticleFilter.py
+-rw-r--r--   0        0        0      183 2024-04-28 11:36:25.108943 connectedpapersextractor-0.1.3/src/connectedpapersextractor/Config.py
+-rw-r--r--   0        0        0      374 2024-04-28 13:45:00.686988 connectedpapersextractor-0.1.3/src/connectedpapersextractor/MainPartsExtractor.py
+-rw-r--r--   0        0        0     2157 2024-04-29 13:12:12.624547 connectedpapersextractor-0.1.3/src/connectedpapersextractor/PdfSummary.py
+-rw-r--r--   0        0        0     2486 2024-04-28 13:45:00.750987 connectedpapersextractor-0.1.3/src/connectedpapersextractor/_AIExtractor.py
+-rw-r--r--   0        0        0      344 2024-04-28 13:39:32.895971 connectedpapersextractor-0.1.3/src/connectedpapersextractor/__init__.py
+-rw-r--r--   0        0        0      704 2024-04-29 13:14:31.644921 connectedpapersextractor-0.1.3/src/connectedpapersextractor/_add_docs.py
+-rw-r--r--   0        0        0      872 2024-04-28 11:53:43.189003 connectedpapersextractor-0.1.3/src/connectedpapersextractor/_combine_summaries.py
+-rw-r--r--   0        0        0     2668 2024-04-28 15:05:13.301962 connectedpapersextractor-0.1.3/src/connectedpapersextractor/_get_pdf_summaries.py
+-rw-r--r--   0        0        0     1170 2024-04-28 16:50:24.953804 connectedpapersextractor-0.1.3/src/connectedpapersextractor/_refine_documents.py
+-rw-r--r--   0        0        0      768 2024-04-28 17:10:03.753179 connectedpapersextractor-0.1.3/src/connectedpapersextractor/_stuff_documents.py
+-rw-r--r--   0        0        0     1744 2024-04-28 17:26:44.686560 connectedpapersextractor-0.1.3/src/connectedpapersextractor/_summarize_documents.py
+-rw-r--r--   0        0        0     1530 2024-04-28 17:17:26.421933 connectedpapersextractor-0.1.3/src/connectedpapersextractor/create_related_work.py
+-rw-r--r--   0        0        0     1450 2024-04-28 13:47:45.376986 connectedpapersextractor-0.1.3/src/connectedpapersextractor/get_summaries.py
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 connectedpapersextractor-0.1.3/PKG-INFO
```

### Comparing `connectedpapersextractor-0.1.2/LICENSE` & `connectedpapersextractor-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.2/pyproject.toml` & `connectedpapersextractor-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tool.poetry]
 name = "ConnectedPapersExtractor"
-version = "0.1.2"
+version = "0.1.3"
 description = "A package for creating summaries based on https://www.connectedpapers.com/."
 authors = ["Tesla2000 <fratajczak124@gmail.com>"]
 license = "MIT License"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 langchain = "^0.1.16"
-langchain-openai = "^0.1.3"
 undetected-chromedriver = "^3.5.5"
 pypdf = "^4.2.0"
 download = "^0.3.5"
 chromedriver-autoinstaller = "^0.6.4"
 langchain-experimental = "^0.0.57"
 PyPDF2 = "^3.0.1"
 EnhancedWebdriver = "^0.1.6"
```

### Comparing `connectedpapersextractor-0.1.2/src/connectedpapersextractor/PdfSummary.py` & `connectedpapersextractor-0.1.3/src/connectedpapersextractor/PdfSummary.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     text_summary: list[Document] = field(init=False, default=None)
 
     def extract_documents(self) -> list[Document]:
         loader = PyPDFLoader(str(self.file_path))
         documents = loader.load()
         for document in documents:
             document.metadata["source"] = str(self.file_path)
+        self.docs = documents
         return documents
 
     def is_valid(self) -> bool:
         if not self.file_path.exists():
             return False
         io = self.file_path.open("rb")
         try:
```

### Comparing `connectedpapersextractor-0.1.2/src/connectedpapersextractor/_AIExtractor.py` & `connectedpapersextractor-0.1.3/src/connectedpapersextractor/_AIExtractor.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.2/src/connectedpapersextractor/_combine_summaries.py` & `connectedpapersextractor-0.1.3/src/connectedpapersextractor/_combine_summaries.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.2/src/connectedpapersextractor/_get_pdf_summaries.py` & `connectedpapersextractor-0.1.3/src/connectedpapersextractor/_get_pdf_summaries.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.2/src/connectedpapersextractor/_refine_documents.py` & `connectedpapersextractor-0.1.3/src/connectedpapersextractor/_refine_documents.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.2/src/connectedpapersextractor/_stuff_documents.py` & `connectedpapersextractor-0.1.3/src/connectedpapersextractor/_stuff_documents.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.2/src/connectedpapersextractor/_summarize_documents.py` & `connectedpapersextractor-0.1.3/src/connectedpapersextractor/_summarize_documents.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.2/src/connectedpapersextractor/create_related_work.py` & `connectedpapersextractor-0.1.3/src/connectedpapersextractor/create_related_work.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.2/src/connectedpapersextractor/get_summaries.py` & `connectedpapersextractor-0.1.3/src/connectedpapersextractor/get_summaries.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.2/PKG-INFO` & `connectedpapersextractor-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConnectedPapersExtractor
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for creating summaries based on https://www.connectedpapers.com/.
 License: MIT
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,10 +14,9 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: EnhancedWebdriver (>=0.1.6,<0.2.0)
 Requires-Dist: PyPDF2 (>=3.0.1,<4.0.0)
 Requires-Dist: chromedriver-autoinstaller (>=0.6.4,<0.7.0)
 Requires-Dist: download (>=0.3.5,<0.4.0)
 Requires-Dist: langchain (>=0.1.16,<0.2.0)
 Requires-Dist: langchain-experimental (>=0.0.57,<0.0.58)
-Requires-Dist: langchain-openai (>=0.1.3,<0.2.0)
 Requires-Dist: pypdf (>=4.2.0,<5.0.0)
 Requires-Dist: undetected-chromedriver (>=3.5.5,<4.0.0)
```

