# Comparing `tmp/bpm_ai-1.6.2.tar.gz` & `tmp/bpm_ai-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai-1.6.2.tar", max compression
+gzip compressed data, was "bpm_ai-1.7.0.tar", max compression
```

## Comparing `bpm_ai-1.6.2.tar` & `bpm_ai-1.7.0.tar`

### file list

```diff
@@ -1,31 +1,36 @@
--rw-r--r--   0        0        0      726 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/README.md
--rw-r--r--   0        0        0        0 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/common/__init__.py
--rw-r--r--   0        0        0      195 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/common/errors.py
--rw-r--r--   0        0        0     1668 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/common/multimodal.py
--rw-r--r--   0        0        0        0 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/compose/__init__.py
--rw-r--r--   0        0        0     1595 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/compose/compose.anthropic.prompt
--rw-r--r--   0        0        0     1369 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/compose/compose.openai.prompt
--rw-r--r--   0        0        0     3577 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/compose/compose.py
--rw-r--r--   0        0        0      950 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/compose/util.py
--rw-r--r--   0        0        0        0 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/decide/__init__.py
--rw-r--r--   0        0        0     8786 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/decide/decide.anthropic.prompt
--rw-r--r--   0        0        0     8181 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/decide/decide.openai.prompt
--rw-r--r--   0        0        0     4862 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/decide/decide.py
--rw-r--r--   0        0        0     3044 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/decide/schema.py
--rw-r--r--   0        0        0        0 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/extract/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/extract/extract.anthropic.prompt
--rw-r--r--   0        0        0     1286 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/extract/extract.openai.prompt
--rw-r--r--   0        0        0     7530 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/extract/extract.py
--rw-r--r--   0        0        0     2578 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/extract/util.py
--rw-r--r--   0        0        0        0 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/generic/__init__.py
--rw-r--r--   0        0        0      690 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/generic/generic.anthropic.prompt
--rw-r--r--   0        0        0      544 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/generic/generic.openai.prompt
--rw-r--r--   0        0        0     1631 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/generic/generic.py
--rw-r--r--   0        0        0        0 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/translate/__init__.py
--rw-r--r--   0        0        0      632 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/translate/translate.anthropic.prompt
--rw-r--r--   0        0        0      611 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/translate/translate.openai.prompt
--rw-r--r--   0        0        0     3138 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/translate/translate.py
--rw-r--r--   0        0        0      680 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/bpm_ai/translate/util.py
--rw-r--r--   0        0        0      900 2024-04-18 13:20:47.266463 bpm_ai-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 bpm_ai-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0      726 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/common/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/common/errors.py
+-rw-r--r--   0        0        0     1668 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/common/multimodal.py
+-rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/compose/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/compose/compose.anthropic.prompt
+-rw-r--r--   0        0        0     1369 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/compose/compose.openai.prompt
+-rw-r--r--   0        0        0     1699 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/compose/compose.prompt
+-rw-r--r--   0        0        0     3644 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/compose/compose.py
+-rw-r--r--   0        0        0      950 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/compose/util.py
+-rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/decide/__init__.py
+-rw-r--r--   0        0        0     8786 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/decide/decide.anthropic.prompt
+-rw-r--r--   0        0        0     8181 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/decide/decide.openai.prompt
+-rw-r--r--   0        0        0     8459 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/decide/decide.prompt
+-rw-r--r--   0        0        0     6170 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/decide/decide.py
+-rw-r--r--   0        0        0     3044 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/decide/schema.py
+-rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/extract/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/extract/extract.anthropic.prompt
+-rw-r--r--   0        0        0     1286 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/extract/extract.openai.prompt
+-rw-r--r--   0        0        0     1466 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/extract/extract.prompt
+-rw-r--r--   0        0        0     7495 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/extract/extract.py
+-rw-r--r--   0        0        0     2578 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/extract/util.py
+-rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/generic/__init__.py
+-rw-r--r--   0        0        0      690 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/generic/generic.anthropic.prompt
+-rw-r--r--   0        0        0      544 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/generic/generic.openai.prompt
+-rw-r--r--   0        0        0      738 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/generic/generic.prompt
+-rw-r--r--   0        0        0     1631 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/generic/generic.py
+-rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/translate/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/translate/translate.anthropic.prompt
+-rw-r--r--   0        0        0      611 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/translate/translate.openai.prompt
+-rw-r--r--   0        0        0      688 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/translate/translate.prompt
+-rw-r--r--   0        0        0     3138 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/translate/translate.py
+-rw-r--r--   0        0        0      680 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/translate/util.py
+-rw-r--r--   0        0        0      900 2024-04-29 16:12:29.958361 bpm_ai-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 bpm_ai-1.7.0/PKG-INFO
```

### Comparing `bpm_ai-1.6.2/README.md` & `bpm_ai-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/common/multimodal.py` & `bpm_ai-1.7.0/bpm_ai/common/multimodal.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/compose/compose.anthropic.prompt` & `bpm_ai-1.7.0/bpm_ai/compose/compose.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/compose/compose.openai.prompt` & `bpm_ai-1.7.0/bpm_ai/compose/compose.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/compose/compose.py` & `bpm_ai-1.7.0/bpm_ai/compose/compose.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import json
 import re
 from typing import TypedDict, Callable
 
 from bpm_ai_core.llm.common.llm import LLM
+from bpm_ai_core.llm.common.message import UserMessage
 from bpm_ai_core.ocr.ocr import OCR
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.speech_recognition.asr import ASRModel
 from bpm_ai_core.tracing.decorators import trace
 
 from bpm_ai.common.errors import MissingParameterError
 from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents, prepare_text_blobs, \
```

### Comparing `bpm_ai-1.6.2/bpm_ai/compose/util.py` & `bpm_ai-1.7.0/bpm_ai/compose/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/decide/decide.anthropic.prompt` & `bpm_ai-1.7.0/bpm_ai/decide/decide.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/decide/decide.openai.prompt` & `bpm_ai-1.7.0/bpm_ai/decide/decide.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/decide/decide.py` & `bpm_ai-1.7.0/bpm_ai/decide/decide.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import Any
 
-from bpm_ai_core.classification.zero_shot_classifier import ZeroShotClassifier
+from bpm_ai_core.image_classification.image_classifier import ImageClassifier
 from bpm_ai_core.llm.common.llm import LLM
 from bpm_ai_core.ocr.ocr import OCR
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.speech_recognition.asr import ASRModel
+from bpm_ai_core.text_classification.text_classifier import TextClassifier
 from bpm_ai_core.tracing.decorators import trace
+from bpm_ai_core.util.file import is_supported_img_file
 from bpm_ai_core.util.markdown import dict_to_md
 
 from bpm_ai.common.errors import MissingParameterError
 from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents, prepare_text_blobs, \
     assert_all_files_processed
 from bpm_ai.decide.schema import get_cot_decision_output_schema, get_decision_output_schema, remove_order_prefix_from_keys
 
@@ -67,55 +69,78 @@
     message = await llm.generate_message(prompt, output_schema=decide_schema)
 
     return remove_order_prefix_from_keys(message.content) if message.content else {}
 
 
 @trace("bpm-ai-decide", ["classifier"])
 async def decide_classifier(
-    classifier: ZeroShotClassifier,
     input_data: dict[str, str | dict | None],
     output_type: str,
+    classifier: TextClassifier = None,
+    image_classifier: ImageClassifier = None,
     question: str | None = None,
     possible_values: list[Any] | None = None,
     multiple_decision_values: bool = False,
     ocr: OCR | None = None,
     asr: ASRModel | None = None
 ) -> dict:
+    if (classifier and image_classifier) or not (classifier or image_classifier):
+        raise ValueError("Must provide either a TextClassifier or an ImageClassifier")
+    if image_classifier and multiple_decision_values:
+        raise ValueError("ImageClassifier does not support multiple decision values")
+
+    zero_shot = (possible_values is not None) or output_type == "boolean"
+
     if not output_type or output_type.isspace():
         raise MissingParameterError("output type is required")
-    if not possible_values and output_type != "boolean":
-        raise MissingParameterError("List of possible values must be specified for classifier (except boolean)")
-    if output_type == "boolean":
+    if zero_shot and output_type == "boolean":
         possible_values = ["yes", "no"]
-    possible_values = [str(v) for v in possible_values]
+    if zero_shot:
+        possible_values = [str(v) for v in possible_values]
 
     if all(value is None for value in input_data.values()):
         return {"decision": None, "reasoning": "No input values present."}
 
-    input_data = await ocr_documents(input_data, ocr)
-    input_data = await transcribe_audio(input_data, asr)
-    input_data = prepare_text_blobs(input_data)
-    assert_all_files_processed(input_data)
+    if image_classifier and not classifier:
+        image_path_or_url = list(input_data.values())[0]
+        if len(input_data) > 1 or not isinstance(image_path_or_url, str) or not is_supported_img_file(image_path_or_url):
+            raise ValueError("Must provide exactly one image file path variable as input when using an Image Classifier.")
+
+        hypothesis_template = "Based on this image, the question '" + question + "' should be answered with '{}'" \
+            if question else "This is an image of {}."
+
+        classification = await image_classifier.classify(
+            blob_or_path=image_path_or_url,
+            classes=possible_values,
+            hypothesis_template=hypothesis_template,
+            confidence_threshold=0.1,
+        )
 
-    input_md = dict_to_md(input_data).strip()
-
-    hypothesis_template = "In this example the question '" + question + "' should be answered with '{}'" \
-        if question else "This example is {}."
-
-    classification = await classifier.classify(
-        input_md,
-        possible_values,
-        hypothesis_template=hypothesis_template,
-        confidence_threshold=0.1,
-        multi_label=multiple_decision_values
-    )
+    else:  # text classifier
+        input_data = await ocr_documents(input_data, ocr)
+        input_data = await transcribe_audio(input_data, asr)
+        input_data = prepare_text_blobs(input_data)
+        assert_all_files_processed(input_data)
+
+        input_md = dict_to_md(input_data).strip()
+
+        hypothesis_template = "In this example the question '" + question + "' should be answered with '{}'" \
+            if question else "This example is {}."
+
+        classification = await classifier.classify(
+            input_md,
+            possible_values,
+            hypothesis_template=hypothesis_template,
+            confidence_threshold=0.1,
+            multi_label=multiple_decision_values
+        )
 
     def raw_to_output_type(raw: str) -> Any:
         if output_type == "boolean":
-            return (raw == 'yes') if raw else None
+            return (raw.lower() == 'yes' or raw.lower() == "true") if raw else None
         elif output_type == "integer":
             return int(raw) if raw else None
         elif output_type == "number":
             return float(raw) if raw else None
         else:
             return raw
```

### Comparing `bpm_ai-1.6.2/bpm_ai/decide/schema.py` & `bpm_ai-1.7.0/bpm_ai/decide/schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/extract/extract.anthropic.prompt` & `bpm_ai-1.7.0/bpm_ai/extract/extract.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/extract/extract.openai.prompt` & `bpm_ai-1.7.0/bpm_ai/extract/extract.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/extract/extract.py` & `bpm_ai-1.7.0/bpm_ai/extract/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import itertools
 import re
-from typing import Callable, Any
+from typing import Any
 
-from bpm_ai_core.classification.zero_shot_classifier import ZeroShotClassifier
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.question_answering.question_answering import QuestionAnswering
 from bpm_ai_core.llm.common.llm import LLM
 from bpm_ai_core.ocr.ocr import OCR
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.speech_recognition.asr import ASRModel
+from bpm_ai_core.text_classification.text_classifier import TextClassifier
 from bpm_ai_core.token_classification.zero_shot_token_classifier import ZeroShotTokenClassifier
 from bpm_ai_core.tracing.decorators import trace
 from bpm_ai_core.util.file import is_supported_img_file
 from bpm_ai_core.util.json_schema import expand_simplified_json_schema
 from bpm_ai_core.util.markdown import dict_to_md
 
 from bpm_ai.common.errors import MissingParameterError
@@ -72,15 +71,15 @@
 
     return transform_result(message.content or {})
 
 
 @trace("bpm-ai-extract", ["extractive-qa"])
 async def extract_qa(
     qa: QuestionAnswering,
-    classifier: ZeroShotClassifier,
+    classifier: TextClassifier,
     input_data: dict[str, str | dict | None],
     output_schema: dict[str, str | dict],
     multiple: bool = False,
     multiple_description: str = "",
     ocr: OCR | None = None,
     vqa: QuestionAnswering | None = None,
     token_classifier: ZeroShotTokenClassifier | None = None,
```

### Comparing `bpm_ai-1.6.2/bpm_ai/extract/util.py` & `bpm_ai-1.7.0/bpm_ai/extract/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/generic/generic.anthropic.prompt` & `bpm_ai-1.7.0/bpm_ai/generic/generic.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/generic/generic.openai.prompt` & `bpm_ai-1.7.0/bpm_ai/generic/generic.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/generic/generic.py` & `bpm_ai-1.7.0/bpm_ai/generic/generic.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/translate/translate.anthropic.prompt` & `bpm_ai-1.7.0/bpm_ai/translate/translate.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/translate/translate.openai.prompt` & `bpm_ai-1.7.0/bpm_ai/translate/translate.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/translate/translate.py` & `bpm_ai-1.7.0/bpm_ai/translate/translate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/bpm_ai/translate/util.py` & `bpm_ai-1.7.0/bpm_ai/translate/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.2/pyproject.toml` & `bpm_ai-1.7.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "bpm-ai"
-version = "1.6.2"
+version = "1.7.0"
 description = "AI task automation for BPM engines."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.11"
-bpm-ai-core = "2.4.2"
-openai = "^1.11.0"
-anthropic = "^0.25.2"
-langfuse = "^2.25.0"
+bpm-ai-core = "2.6.2"
+openai = "^1.22.0"
+anthropic = "^0.25.6"
+langfuse = "^2.27.2"
 amazon-textract-prettyprinter = "^0.1.9"
 aiobotocore = "^2.12.3"
 azure-storage-blob = "^12.19.1"
 azure-ai-translation-text = "^1.0.0b1"
 azure-ai-documentintelligence = "^1.0.0b2"
 av = "^11.0.0"
 
 [tool.poetry.group.dev.dependencies]
-bpm-ai-inference = "0.2.6"
+bpm-ai-inference = "0.3.0"
 ctranslate2 = "4.1.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.2"
 pytest-asyncio = "^0.23.5"
 pytest-dotenv = "^0.5.2"
```

### Comparing `bpm_ai-1.6.2/PKG-INFO` & `bpm_ai-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: bpm-ai
-Version: 1.6.2
+Version: 1.7.0
 Summary: AI task automation for BPM engines.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiobotocore (>=2.12.3,<3.0.0)
 Requires-Dist: amazon-textract-prettyprinter (>=0.1.9,<0.2.0)
-Requires-Dist: anthropic (>=0.25.2,<0.26.0)
+Requires-Dist: anthropic (>=0.25.6,<0.26.0)
 Requires-Dist: av (>=11.0.0,<12.0.0)
 Requires-Dist: azure-ai-documentintelligence (>=1.0.0b2,<2.0.0)
 Requires-Dist: azure-ai-translation-text (>=1.0.0b1,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0)
-Requires-Dist: bpm-ai-core (==2.4.2)
-Requires-Dist: langfuse (>=2.25.0,<3.0.0)
-Requires-Dist: openai (>=1.11.0,<2.0.0)
+Requires-Dist: bpm-ai-core (==2.6.2)
+Requires-Dist: langfuse (>=2.27.2,<3.0.0)
+Requires-Dist: openai (>=1.22.0,<2.0.0)
 Project-URL: Repository, https://github.com/holunda-io/bpm-ai
 Description-Content-Type: text/markdown
 
 # bpm-ai
 _AI task automation for BPM engines._
 
 See [bpm-ai-connectors-camunda-8](https://github.com/holunda-io/bpm-ai-connectors-camunda-8) for actual integration with the Camunda Platform 8 BPM engine using custom BPMN elements (Connectors).
```

