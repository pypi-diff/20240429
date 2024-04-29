# Comparing `tmp/connectedpapersextractor-0.1.1.tar.gz` & `tmp/connectedpapersextractor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectedpapersextractor-0.1.1.tar", max compression
+gzip compressed data, was "connectedpapersextractor-0.1.2.tar", max compression
```

## Comparing `connectedpapersextractor-0.1.1.tar` & `connectedpapersextractor-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     1070 2024-04-23 21:01:05.479303 connectedpapersextractor-0.1.1/LICENSE
--rw-r--r--   0        0        0      644 2024-04-28 14:10:16.375106 connectedpapersextractor-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-27 22:23:56.499918 connectedpapersextractor-0.1.1/src/connectedpapersextractor/ArticleFilter.py
--rw-r--r--   0        0        0      183 2024-04-28 11:36:25.108943 connectedpapersextractor-0.1.1/src/connectedpapersextractor/Config.py
--rw-r--r--   0        0        0      374 2024-04-28 13:45:00.686988 connectedpapersextractor-0.1.1/src/connectedpapersextractor/MainPartsExtractor.py
--rw-r--r--   0        0        0     2062 2024-04-28 13:45:00.742987 connectedpapersextractor-0.1.1/src/connectedpapersextractor/PdfSummary.py
--rw-r--r--   0        0        0     2486 2024-04-28 13:45:00.750987 connectedpapersextractor-0.1.1/src/connectedpapersextractor/_AIExtractor.py
--rw-r--r--   0        0        0      344 2024-04-28 13:39:32.895971 connectedpapersextractor-0.1.1/src/connectedpapersextractor/__init__.py
--rw-r--r--   0        0        0      724 2024-04-28 13:43:53.635611 connectedpapersextractor-0.1.1/src/connectedpapersextractor/_add_docs.py
--rw-r--r--   0        0        0      872 2024-04-28 11:53:43.189003 connectedpapersextractor-0.1.1/src/connectedpapersextractor/_combine_summaries.py
--rw-r--r--   0        0        0     2526 2024-04-28 13:41:29.892333 connectedpapersextractor-0.1.1/src/connectedpapersextractor/_get_pdf_summaries.py
--rw-r--r--   0        0        0     2052 2024-04-28 13:39:32.907971 connectedpapersextractor-0.1.1/src/connectedpapersextractor/_summarize_documents_piecemeal.py
--rw-r--r--   0        0        0     1529 2024-04-28 13:39:32.871971 connectedpapersextractor-0.1.1/src/connectedpapersextractor/create_related_work.py
--rw-r--r--   0        0        0     1450 2024-04-28 13:47:45.376986 connectedpapersextractor-0.1.1/src/connectedpapersextractor/get_summaries.py
--rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 connectedpapersextractor-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-23 21:01:05.479303 connectedpapersextractor-0.1.2/LICENSE
+-rw-r--r--   0        0        0      644 2024-04-28 17:33:23.514920 connectedpapersextractor-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-27 22:23:56.499918 connectedpapersextractor-0.1.2/src/connectedpapersextractor/ArticleFilter.py
+-rw-r--r--   0        0        0      183 2024-04-28 11:36:25.108943 connectedpapersextractor-0.1.2/src/connectedpapersextractor/Config.py
+-rw-r--r--   0        0        0      374 2024-04-28 13:45:00.686988 connectedpapersextractor-0.1.2/src/connectedpapersextractor/MainPartsExtractor.py
+-rw-r--r--   0        0        0     2127 2024-04-28 15:05:13.309963 connectedpapersextractor-0.1.2/src/connectedpapersextractor/PdfSummary.py
+-rw-r--r--   0        0        0     2486 2024-04-28 13:45:00.750987 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_AIExtractor.py
+-rw-r--r--   0        0        0      344 2024-04-28 13:39:32.895971 connectedpapersextractor-0.1.2/src/connectedpapersextractor/__init__.py
+-rw-r--r--   0        0        0      724 2024-04-28 13:43:53.635611 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_add_docs.py
+-rw-r--r--   0        0        0      872 2024-04-28 11:53:43.189003 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_combine_summaries.py
+-rw-r--r--   0        0        0     2668 2024-04-28 15:05:13.301962 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_get_pdf_summaries.py
+-rw-r--r--   0        0        0     1170 2024-04-28 16:50:24.953804 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_refine_documents.py
+-rw-r--r--   0        0        0      768 2024-04-28 17:10:03.753179 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_stuff_documents.py
+-rw-r--r--   0        0        0     1744 2024-04-28 17:26:44.686560 connectedpapersextractor-0.1.2/src/connectedpapersextractor/_summarize_documents.py
+-rw-r--r--   0        0        0     1530 2024-04-28 17:17:26.421933 connectedpapersextractor-0.1.2/src/connectedpapersextractor/create_related_work.py
+-rw-r--r--   0        0        0     1450 2024-04-28 13:47:45.376986 connectedpapersextractor-0.1.2/src/connectedpapersextractor/get_summaries.py
+-rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 connectedpapersextractor-0.1.2/PKG-INFO
```

### Comparing `connectedpapersextractor-0.1.1/LICENSE` & `connectedpapersextractor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.1/pyproject.toml` & `connectedpapersextractor-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ConnectedPapersExtractor"
-version = "0.1.1"
+version = "0.1.2"
 description = "A package for creating summaries based on https://www.connectedpapers.com/."
 authors = ["Tesla2000 <fratajczak124@gmail.com>"]
 license = "MIT License"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 langchain = "^0.1.16"
```

### Comparing `connectedpapersextractor-0.1.1/src/connectedpapersextractor/PdfSummary.py` & `connectedpapersextractor-0.1.2/src/connectedpapersextractor/PdfSummary.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         loader = PyPDFLoader(str(self.file_path))
         documents = loader.load()
         for document in documents:
             document.metadata["source"] = str(self.file_path)
         return documents
 
     def is_valid(self) -> bool:
+        if not self.file_path.exists():
+            return False
         io = self.file_path.open("rb")
         try:
             PdfReader(io)
         except PdfReadError:
             io.close()
             os.remove(str(self.file_path.absolute()))
             return False
```

### Comparing `connectedpapersextractor-0.1.1/src/connectedpapersextractor/_AIExtractor.py` & `connectedpapersextractor-0.1.2/src/connectedpapersextractor/_AIExtractor.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.1/src/connectedpapersextractor/_add_docs.py` & `connectedpapersextractor-0.1.2/src/connectedpapersextractor/_add_docs.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.1/src/connectedpapersextractor/_combine_summaries.py` & `connectedpapersextractor-0.1.2/src/connectedpapersextractor/_combine_summaries.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.1/src/connectedpapersextractor/_get_pdf_summaries.py` & `connectedpapersextractor-0.1.2/src/connectedpapersextractor/_get_pdf_summaries.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,17 +60,22 @@
         downloads.append(
             (
                 link,
                 str(file_path),
             )
         )
     driver.quit()
+    failed_download = set()
     for link, file_path in downloads:
-        download(link, file_path)
-    summaries = list(filter(PdfSummary.is_valid, summaries))
+        try:
+            download(link, file_path)
+        except RuntimeError:
+            failed_download.add(file_path)
+    summaries = list(
+        summary for summary in summaries if summary.is_valid())
     dir_path.joinpath(Config.metadate_file_name).write_text(
         json.dumps(
             dict(
                 (str(summary_dict.pop("file_path")), summary_dict)
                 for summary_dict in map(asdict, summaries)
             ),
             indent=2,
```

### Comparing `connectedpapersextractor-0.1.1/src/connectedpapersextractor/_summarize_documents_piecemeal.py` & `connectedpapersextractor-0.1.2/src/connectedpapersextractor/create_related_work.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,42 @@
-import json
-from dataclasses import asdict
+from operator import attrgetter
 from typing import Union, Optional
 
-from langchain.chains.combine_documents.stuff import StuffDocumentsChain
-from langchain.chains.llm import LLMChain
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models import LanguageModelInput
 from langchain_core.messages import BaseMessage
-from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.runnables import Runnable
-from openai import BadRequestError
+from langchain_openai import ChatOpenAI
 
-from . import Config
-from .MainPartsExtractor import MainPartsExtractor
+from . import MainPartsExtractor
+from .MainPartsExtractor import _DefaultExtractor
 from .PdfSummary import PdfSummaries
-from ._add_docs import _add_docs
+from ._combine_summaries import _combine_summaries
+from ._summarize_documents import _summarize_documents
 
 
-def _summarize_documents_piecemeal(
+def create_related_work(
     summaries: PdfSummaries,
-    main_parts_extractor: MainPartsExtractor,
     llm: Union[
         Runnable[LanguageModelInput, str],
         Optional[Runnable[LanguageModelInput, BaseMessage]],
     ] = None,
     embeddings: Optional[Embeddings] = None,
-) -> PdfSummaries:
-    prompt = ChatPromptTemplate.from_template(
-        """
-    Write a concise summary of the following:
-    "{text}"
-    CONCISE SUMMARY:
-    """
+    main_parts_extractor: Optional[MainPartsExtractor] = None,
+    refine: bool = True,
+) -> str:
+    if not summaries:
+        raise ValueError("Summaries must be provided")
+    if main_parts_extractor is None:
+        main_parts_extractor = _DefaultExtractor()
+    if llm is None:
+        llm = ChatOpenAI(temperature=0, model_name="gpt-3.5-turbo-16k")
+        llm.max_tokens = 16385
+    summaries_with_text = _summarize_documents(
+        summaries, main_parts_extractor, llm, embeddings
     )
-    llm_chain = LLMChain(llm=llm, prompt=prompt)
-    stuff_chain = StuffDocumentsChain(
-        llm_chain=llm_chain, document_variable_name="text"
+    combined_summaries = "\n\n".join(
+        map(": ".join, map(attrgetter("title", "text_summary"), summaries_with_text))
     )
-    metadata_path = summaries[0].file_path.parent.joinpath(Config.metadate_file_name)
-    for summary in summaries:
-        if summary.text_summary is not None:
-            continue
-        _add_docs(summary, embeddings)
-        docs = main_parts_extractor.extract(summary)
-        try:
-            text_summary = stuff_chain.run(docs)
-        except BadRequestError as e:
-            e.message += "\nConsider changing  value of article_filter"
-            raise e
-        summary.text_summary = text_summary
-        summary_as_dict = asdict(summary)
-        summary_as_dict.pop("docs")
-        metadata = json.loads(metadata_path.read_text())
-        metadata[str(summary_as_dict.pop("file_path"))] = summary_as_dict
-        metadata_path.write_text(json.dumps(metadata, indent=2))
-    return summaries
+    if refine and len(summaries) != 1:
+        return _combine_summaries(combined_summaries, llm)
+    return combined_summaries
```

### Comparing `connectedpapersextractor-0.1.1/src/connectedpapersextractor/get_summaries.py` & `connectedpapersextractor-0.1.2/src/connectedpapersextractor/get_summaries.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.1/PKG-INFO` & `connectedpapersextractor-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConnectedPapersExtractor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for creating summaries based on https://www.connectedpapers.com/.
 License: MIT
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```
