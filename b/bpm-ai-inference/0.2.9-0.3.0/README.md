# Comparing `tmp/bpm_ai_inference-0.2.9.tar.gz` & `tmp/bpm_ai_inference-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_inference-0.2.9.tar", max compression
+gzip compressed data, was "bpm_ai_inference-0.3.0.tar", max compression
```

## Comparing `bpm_ai_inference-0.2.9.tar` & `bpm_ai_inference-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,40 @@
--rw-r--r--   0        0        0    35128 2024-04-18 14:13:26.670002 bpm_ai_inference-0.2.9/LICENSE
--rw-r--r--   0        0        0      743 2024-04-18 14:13:26.670002 bpm_ai_inference-0.2.9/README.md
--rw-r--r--   0        0        0        0 2024-04-18 14:13:26.670002 bpm_ai_inference-0.2.9/bpm_ai_inference/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 14:13:26.670002 bpm_ai_inference-0.2.9/bpm_ai_inference/classification/__init__.py
--rw-r--r--   0        0        0     2520 2024-04-18 14:13:26.670002 bpm_ai_inference-0.2.9/bpm_ai_inference/classification/transformers_classifier.py
--rw-r--r--   0        0        0     1519 2024-04-18 14:13:26.670002 bpm_ai_inference-0.2.9/bpm_ai_inference/daemon.py
--rw-r--r--   0        0        0        0 2024-04-18 14:13:26.670002 bpm_ai_inference-0.2.9/bpm_ai_inference/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 14:13:26.670002 bpm_ai_inference-0.2.9/bpm_ai_inference/ocr/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-18 14:13:26.670002 bpm_ai_inference-0.2.9/bpm_ai_inference/ocr/tesseract.py
--rw-r--r--   0        0        0        0 2024-04-18 14:13:26.670002 bpm_ai_inference-0.2.9/bpm_ai_inference/pos/__init__.py
--rw-r--r--   0        0        0     1848 2024-04-18 14:13:26.670002 bpm_ai_inference-0.2.9/bpm_ai_inference/pos/spacy_pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-18 14:13:26.670002 bpm_ai_inference-0.2.9/bpm_ai_inference/question_answering/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-18 14:13:26.670002 bpm_ai_inference-0.2.9/bpm_ai_inference/question_answering/pix2struct_vqa.py
--rw-r--r--   0        0        0     2013 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/question_answering/transformers_docvqa.py
--rw-r--r--   0        0        0     1882 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/question_answering/transformers_qa.py
--rw-r--r--   0        0        0        0 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/speech_recognition/__init__.py
--rw-r--r--   0        0        0     1176 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/speech_recognition/faster_whisper.py
--rw-r--r--   0        0        0        0 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/token_classification/__init__.py
--rw-r--r--   0        0        0     1344 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/token_classification/gliner_token_classifier.py
--rw-r--r--   0        0        0     3115 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/token_classification/transformers_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/translation/__init__.py
--rw-r--r--   0        0        0        2 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/translation/easy_nmt/__init__.py
--rw-r--r--   0        0        0    18637 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
--rw-r--r--   0        0        0     2423 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/translation/easy_nmt/opus_mt.py
--rw-r--r--   0        0        0     1784 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/translation/easy_nmt/util.py
--rw-r--r--   0        0        0        0 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/util/__init__.py
--rw-r--r--   0        0        0      828 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/util/language.py
--rw-r--r--   0        0        0     6718 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/bpm_ai_inference/util/optimum.py
--rw-r--r--   0        0        0      960 2024-04-18 14:13:26.674002 bpm_ai_inference-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 bpm_ai_inference-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/LICENSE
+-rw-r--r--   0        0        0      743 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/bpm_ai_inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/bpm_ai_inference/classification/__init__.py
+-rw-r--r--   0        0        0     2852 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/bpm_ai_inference/classification/transformers_text_classifier.py
+-rw-r--r--   0        0        0     1740 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/bpm_ai_inference/daemon.py
+-rw-r--r--   0        0        0        0 2024-04-29 08:28:08.741572 bpm_ai_inference-0.3.0/bpm_ai_inference/image_classification/__init__.py
+-rw-r--r--   0        0        0     2547 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/image_classification/transformers_image_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/__init__.py
+-rw-r--r--   0        0        0      219 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/_constants.py
+-rw-r--r--   0        0        0     8123 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/llama_chat.py
+-rw-r--r--   0        0        0      199 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/output_schema.prompt
+-rw-r--r--   0        0        0      981 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/tool_use.prompt
+-rw-r--r--   0        0        0     1082 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/llm/llama_cpp/util.py
+-rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/ocr/__init__.py
+-rw-r--r--   0        0        0     3256 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/ocr/tesseract.py
+-rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/pos/__init__.py
+-rw-r--r--   0        0        0     1833 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/pos/spacy_pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/__init__.py
+-rw-r--r--   0        0        0     2154 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/pix2struct_vqa.py
+-rw-r--r--   0        0        0     2056 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/transformers_docvqa.py
+-rw-r--r--   0        0        0     1940 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/transformers_qa.py
+-rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/speech_recognition/__init__.py
+-rw-r--r--   0        0        0     1219 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/speech_recognition/faster_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/token_classification/__init__.py
+-rw-r--r--   0        0        0     1402 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/token_classification/gliner_token_classifier.py
+-rw-r--r--   0        0        0     3178 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/token_classification/transformers_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/translation/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/__init__.py
+-rw-r--r--   0        0        0    18731 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
+-rw-r--r--   0        0        0     2423 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/opus_mt.py
+-rw-r--r--   0        0        0     1784 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/util.py
+-rw-r--r--   0        0        0       36 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/util/__init__.py
+-rw-r--r--   0        0        0      483 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/util/files.py
+-rw-r--r--   0        0        0      122 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/util/hf.py
+-rw-r--r--   0        0        0      828 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/util/language.py
+-rw-r--r--   0        0        0     7153 2024-04-29 08:28:08.745572 bpm_ai_inference-0.3.0/bpm_ai_inference/util/optimum.py
+-rw-r--r--   0        0        0     1014 2024-04-29 08:28:08.749572 bpm_ai_inference-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 bpm_ai_inference-0.3.0/PKG-INFO
```

### Comparing `bpm_ai_inference-0.2.9/LICENSE` & `bpm_ai_inference-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.9/README.md` & `bpm_ai_inference-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/classification/transformers_classifier.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/classification/transformers_text_classifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
-from bpm_ai_core.classification.zero_shot_classifier import ZeroShotClassifier, ClassificationResult
+from bpm_ai_core.text_classification.text_classifier import TextClassifier, ClassificationResult
+from bpm_ai_core.util.caching import cachable
 from typing_extensions import override
 
 from bpm_ai_inference.util.optimum import get_optimized_model
 
 try:
     from transformers import pipeline, AutoTokenizer, AutoModelForSequenceClassification
     from optimum.onnxruntime import ORTModelForSequenceClassification, ORTOptimizer, ORTQuantizer
@@ -15,57 +16,63 @@
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_MODEL_EN = "MoritzLaurer/deberta-v3-large-zeroshot-v2.0"
 DEFAULT_MODEL_MULTI = "MoritzLaurer/bge-m3-zeroshot-v2.0"
 
 
-class TransformersClassifier(ZeroShotClassifier):
+@cachable()
+class TransformersClassifier(TextClassifier):
     """
-    Local zero-shot classification model based on Huggingface transformers library.
+    Local (zero-shot) text classification model based on Huggingface transformers library.
 
     To use, you should have the ``transformers`` and ``optimum`` python packages installed.
     """
 
-    def __init__(self, model: str = DEFAULT_MODEL_EN):
+    def __init__(self, model: str = DEFAULT_MODEL_EN, zero_shot: bool = True):
         if not has_transformers:
             raise ImportError('transformers or optimum not installed')
 
-        model, self.tokenizer = get_optimized_model(model, "zero-shot-classification")
+        task = "zero-shot-classification" if zero_shot else "text-classification"
 
-        self.zeroshot_classifier = pipeline(
-            "zero-shot-classification",
+        model, self.tokenizer = get_optimized_model(model, task)
+
+        self.text_classifier = pipeline(
+            task,
             model=model,
             tokenizer=self.tokenizer
         )
 
     @override
     async def _do_classify(
             self,
             text: str,
-            classes: list[str],
+            classes: list[str] = None,
             hypothesis_template: str | None = None,
             multi_label: bool = False
     ) -> ClassificationResult:
         input_tokens = len(self.tokenizer.encode(text))
         max_tokens = self.tokenizer.model_max_length
         logger.debug(f"Input tokens: {input_tokens}")
         if input_tokens > max_tokens:
             logger.warning(
                 f"Input tokens exceed max model context size: {input_tokens} > {max_tokens}. Input will be truncated."
             )
 
-        prediction = self.zeroshot_classifier(
+        prediction = self.text_classifier(
             text,
-            candidate_labels=classes,
-            hypothesis_template=hypothesis_template or "This example is about {}",
-            multi_label=multi_label
+            **({"candidate_labels": classes} if classes else {}),
+            **({"hypothesis_template": hypothesis_template or "This example is about {}"} if classes else {}),
+            **({"multi_label": multi_label} if classes else {}),
         )
         # Zip the labels and scores together and find the label with the max score
-        labels_scores = list(zip(prediction['labels'], prediction['scores']))
+        if 'labels' in prediction:
+            labels_scores = list(zip(prediction['labels'], prediction['scores']))
+        else:
+            labels_scores = [(p['label'], p['score']) for p in prediction]
         max_label, max_score = max(labels_scores, key=lambda x: x[1])
 
         return ClassificationResult(
             max_label=max_label,
             max_score=max_score,
             labels_scores=labels_scores
         )
```

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/daemon.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/daemon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import logging
 import os
 
-from bpm_ai_core.util.remote_object import create_remote_object_daemon
+from bpm_ai_core.util.rpc import create_remote_object_daemon
 
-from bpm_ai_inference.classification.transformers_classifier import TransformersClassifier
+from bpm_ai_inference.classification.transformers_text_classifier import TransformersClassifier
+from bpm_ai_inference.image_classification.transformers_image_classifier import TransformersImageClassifier
+from bpm_ai_inference.llm.llama_cpp.llama_chat import ChatLlamaCpp
 from bpm_ai_inference.ocr.tesseract import TesseractOCR
 from bpm_ai_inference.pos.spacy_pos_tagger import SpacyPOSTagger
 from bpm_ai_inference.question_answering.pix2struct_vqa import Pix2StructVQA
 from bpm_ai_inference.question_answering.transformers_docvqa import TransformersDocVQA
 from bpm_ai_inference.question_answering.transformers_qa import TransformersExtractiveQA
 from bpm_ai_inference.speech_recognition.faster_whisper import FasterWhisperASR
 from bpm_ai_inference.token_classification.gliner_token_classifier import GlinerTokenClassifier
 from bpm_ai_inference.token_classification.transformers_token_classifier import TransformersTokenClassifier
 from bpm_ai_inference.translation.easy_nmt.easy_nmt import EasyNMT
 
 remote_classes = [
     TransformersClassifier,
+    TransformersImageClassifier,
     TransformersTokenClassifier,
     GlinerTokenClassifier,
     TesseractOCR,
     SpacyPOSTagger,
     Pix2StructVQA,
     TransformersDocVQA,
     TransformersExtractiveQA,
     FasterWhisperASR,
-    EasyNMT
+    EasyNMT,
+    ChatLlamaCpp
 ]
 
 if __name__ == "__main__":
     logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
 
     daemon = create_remote_object_daemon(
         host=os.environ.get('DAEMON_HOST', '0.0.0.0'),
```

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/ocr/tesseract.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/ocr/tesseract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import asyncio
 import logging
 import os
 import urllib
 
 from PIL import Image
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.ocr.ocr import OCR, OCRResult, OCRPage
+from bpm_ai_core.util.caching import cachable
 from bpm_ai_core.util.image import pdf_to_images
 from typing_extensions import override
 
 from bpm_ai_inference.util.language import indentify_language_iso_639_3
 
 try:
     import pytesseract
@@ -18,14 +18,15 @@
     has_pytesseract = False
 
 logger = logging.getLogger(__name__)
 
 TESSDATA_DIR = "~/.bpm.ai/tessdata/"
 
 
+@cachable()
 class TesseractOCR(OCR):
     """
     Local OCR model based on tesseract.
 
     To use, you should have the ``tesseract`` or ``tesseract-ocr`` package installed.
     """
     def __init__(self):
```

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/pos/spacy_pos_tagger.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/pos/spacy_pos_tagger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import logging
 
 from bpm_ai_core.pos.pos_tagger import POSTagger, POSResult
 from typing_extensions import override
 
 try:
     import spacy
```

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/question_answering/pix2struct_vqa.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/pix2struct_vqa.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import asyncio
 import logging
 
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.question_answering.question_answering import QuestionAnswering, QAResult
+from bpm_ai_core.util.caching import cachable
 from bpm_ai_core.util.image import blob_as_images
 from typing_extensions import override
 
 try:
     from transformers import pipeline, AutoTokenizer, DocumentQuestionAnsweringPipeline, \
     Pix2StructForConditionalGeneration, Pix2StructProcessor
     import torch
@@ -16,22 +16,23 @@
     has_transformers = False
 
 logger = logging.getLogger(__name__)
 
 IMAGE_FORMATS = ["png", "jpeg"]
 
 
+@cachable()
 class Pix2StructVQA(QuestionAnswering):
     """
     Local visual question answering model based on Pix2Struct and Huggingface transformers library.
 
     To use, you should have the ``transformers`` python package installed.
     """
 
-    def __init__(self,model: str = "google/pix2struct-docvqa-base"):
+    def __init__(self, model: str = "google/pix2struct-docvqa-base"):
         if not has_transformers:
             raise ImportError('transformers is not installed')
         self.model = model
 
     @override
     async def _do_answer(
             self,
```

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/question_answering/transformers_docvqa.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/transformers_docvqa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import asyncio
 import logging
 
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.question_answering.question_answering import QuestionAnswering, QAResult
+from bpm_ai_core.util.caching import cachable
 from bpm_ai_core.util.image import blob_as_images
 from typing_extensions import override
 
 try:
     from transformers import pipeline, AutoTokenizer, DocumentQuestionAnsweringPipeline
 
     has_transformers = True
@@ -14,14 +14,15 @@
     has_transformers = False
 
 logger = logging.getLogger(__name__)
 
 IMAGE_FORMATS = ["png", "jpeg"]
 
 
+@cachable()
 class TransformersDocVQA(QuestionAnswering):
     """
     Local visual document question answering model based on Huggingface transformers library.
 
     To use, you should have the ``transformers`` python package and the ``tesseract`` or ``tesseract-ocr`` package installed.
     """
```

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/question_answering/transformers_qa.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/question_answering/transformers_qa.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import logging
 
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.question_answering.question_answering import QuestionAnswering, QAResult
+from bpm_ai_core.util.caching import cachable
 from typing_extensions import override
 
 from bpm_ai_inference.util.optimum import get_optimized_model
 
 try:
     from transformers import pipeline, AutoTokenizer
     has_transformers = True
 except ImportError:
     has_transformers = False
 
 logger = logging.getLogger(__name__)
 
 
+@cachable()
 class TransformersExtractiveQA(QuestionAnswering):
     """
     Local extractive question answering model based on Huggingface transformers library.
 
     To use, you should have the ``transformers`` and ``optimum`` python packages installed.
     """
```

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/speech_recognition/faster_whisper.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/speech_recognition/faster_whisper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import asyncio
 import io
 
 from bpm_ai_core.speech_recognition.asr import ASRModel, ASRResult
+from bpm_ai_core.util.caching import cachable
 from typing_extensions import override
 
 try:
     from faster_whisper import WhisperModel
     has_faster_whisper = True
 except ImportError:
     has_faster_whisper = False
 
 
+@cachable()
 class FasterWhisperASR(ASRModel):
     """
     Local `OpenAI` Whisper Automatic Speech Recognition (ASR) model for transcribing audio.
 
     To use, you should have the ``faster_whisper`` python package installed.
     """
```

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/token_classification/gliner_token_classifier.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/token_classification/gliner_token_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import logging
 
 from bpm_ai_core.token_classification.zero_shot_token_classifier import ZeroShotTokenClassifier, \
     TokenClassificationResult, TokenSpan
+from bpm_ai_core.util.caching import cachable
 from typing_extensions import override
 
 try:
     from gliner import GLiNER
     has_gliner = True
 except ImportError:
     has_gliner = False
 
 logger = logging.getLogger(__name__)
 
 
+@cachable()
 class GlinerTokenClassifier(ZeroShotTokenClassifier):
     """
     Zero Shot Token Classifier based on GLiNER.
 
     To use, you should have the ``gliner`` python package installed.
     """
```

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/token_classification/transformers_token_classifier.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/token_classification/transformers_token_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import logging
 
 from bpm_ai_core.token_classification.zero_shot_token_classifier import ZeroShotTokenClassifier, \
     TokenClassificationResult, TokenSpan
+from bpm_ai_core.util.caching import cachable
 from typing_extensions import override
 
-from bpm_ai_inference.classification.transformers_classifier import TransformersClassifier, DEFAULT_MODEL_EN, \
+from bpm_ai_inference.classification.transformers_text_classifier import TransformersClassifier, DEFAULT_MODEL_EN, \
     DEFAULT_MODEL_MULTI
 from bpm_ai_inference.pos.spacy_pos_tagger import SpacyPOSTagger
 from bpm_ai_inference.util.language import indentify_language
 
 logger = logging.getLogger(__name__)
 
 
+@cachable()
 class TransformersTokenClassifier(ZeroShotTokenClassifier):
     """
     Zero Shot Token Classifier based on a POS tagger and a zero shot classifier.
 
     To use, you should have the ``spacy`` and ``transformers`` python packages installed.
     """
```

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/translation/easy_nmt/easy_nmt.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/easy_nmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import asyncio
 import json
 import logging
 import math
 import os
 import queue
 import re
 import time
 from typing import List, Union, Dict, FrozenSet, Iterable
 
+from bpm_ai_core.util.caching import cachable
 from typing_extensions import override
 
 try:
     import nltk
     import numpy as np
     import torch
     import torch.multiprocessing as mp
@@ -26,14 +26,17 @@
 from bpm_ai_inference.util.language import indentify_language
 
 logger = logging.getLogger(__name__)
 
 DOWNLOAD_URL = 'http://easynmt.net/models/v2'
 
 
+@cachable(
+    exclude_key_params=["cache_folder", "device"]
+)
 class EasyNMT(NMTModel):
     """
     See https://github.com/UKPLab/EasyNMT.
     Copied and modified to remove dependency to fasttext.
     """
 
     def __init__(
```

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/translation/easy_nmt/opus_mt.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/opus_mt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/translation/easy_nmt/util.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/translation/easy_nmt/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/util/language.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/util/language.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.9/bpm_ai_inference/util/optimum.py` & `bpm_ai_inference-0.3.0/bpm_ai_inference/util/optimum.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 import time
 from pathlib import Path
 from typing import Type
 
 import cpuinfo
 from huggingface_hub import HfFileSystem
 from optimum.onnxruntime import ORTModelForSequenceClassification, ORTOptimizer, ORTQuantizer, \
-    ORTModelForQuestionAnswering, ORTModel
-from optimum.onnxruntime.configuration import OptimizationConfig, AutoQuantizationConfig, AutoOptimizationConfig
+    ORTModelForQuestionAnswering, ORTModel, ORTModelForImageClassification
+from optimum.onnxruntime.configuration import AutoQuantizationConfig, AutoOptimizationConfig
 from transformers import AutoTokenizer
 
+from bpm_ai_inference.util.hf import hf_home
+
 logger = logging.getLogger(__name__)
 
 FILENAME_ONNX = "model.onnx"
 FILENAME_OPTIMIZED_ONNX = "model_optimized.onnx"
 FILENAME_QUANTIZED_ONNX = "model_quantized.onnx"
 
 
@@ -34,42 +36,41 @@
 
 def _holisticon_onnx_repository_id(model_name: str) -> str:
     return f"holisticon/{model_name.split('/')[1]}-onnx"
 
 
 def get_optimized_model(model: str, task: str, optimization_level: int = None, push_to_hub: bool = False):
     model_name = model
-    model_dir = _hf_home() + "/onnx/" + model.replace("/", "--")
+    model_dir = hf_home() + "/onnx/" + model.replace("/", "--")
     tokenizer = AutoTokenizer.from_pretrained(model)
 
     optimization_level = optimization_level or int(os.getenv("OPTIMIZATION_LEVEL", "2"))
 
     onnx = optimization_level >= 1
     optimize = optimization_level == 2
     quantize = optimization_level == 3
 
-    if onnx:
-        tokenizer.model_input_names = ['input_ids', 'attention_mask']
-        if optimize:
-            model = _optimize(model, model_dir, task, push_to_hub=push_to_hub)
-        elif quantize:
-            model = _quantize(model, model_dir, task, push_to_hub=push_to_hub)
-        else:
-            model = _export_to_onnx(model, model_dir, task)
+    try:
+        if onnx:
+            tokenizer.model_input_names = ['input_ids', 'attention_mask']
+            if optimize:
+                model = _optimize(model, model_dir, task, push_to_hub=push_to_hub)
+            elif quantize:
+                model = _quantize(model, model_dir, task, push_to_hub=push_to_hub)
+            else:
+                model = _export_to_onnx(model, model_dir, task)
+    except Exception as e:
+        logger.warning("Error while trying to optimize model, falling back to unoptimized model: %s", e)
 
     if push_to_hub:
         model.push_to_hub(model.model_save_dir, _holisticon_onnx_repository_id(model_name))
 
     return model, tokenizer
 
 
-def _hf_home():
-    return os.getenv('HF_HOME', os.path.join(os.path.expanduser("~"), ".cache", "huggingface"))
-
-
 def _check_exists_on_hub(repository_id: str, filename: str) -> str | None:
     fs = HfFileSystem()
     if not fs.exists(repository_id):
         return None
     hub_models = fs.glob(f"{repository_id}/**/{filename}", maxdepth=3)
     if len(hub_models) == 1:
         model_path = str(Path(hub_models[0].removeprefix(repository_id + "/")).parent)
@@ -93,14 +94,20 @@
     return None
 
 
 def _task_to_model(task: str):
     match task:
         case "zero-shot-classification":
             return ORTModelForSequenceClassification
+        case "text-classification":
+            return ORTModelForSequenceClassification
+        case "zero-shot-image-classification":
+            return ORTModelForImageClassification
+        case "image-classification":
+            return ORTModelForImageClassification
         case "question-answering":
             return ORTModelForQuestionAnswering
 
 
 @timer
 def _export_to_onnx(repository_id: str, model_dir, task):
     model_class = _task_to_model(task)
@@ -130,15 +137,16 @@
 
     # optimize
     model = _export_to_onnx(repository_id, model_dir, task)
     optimizer = ORTOptimizer.from_pretrained(model)
     if push_to_hub:
         config = AutoOptimizationConfig.O2()
     else:
-        config = OptimizationConfig(optimization_level=99)  # enable all optimizations
+        config = AutoOptimizationConfig.O2()
+        #config = OptimizationConfig(optimization_level=99)  # enable all optimizations
     optimizer.optimize(
         optimization_config=config,
         save_dir=model_dir
     )
     size = os.path.getsize(model_file) / (1024 * 1024)
     logger.debug(f"Optimized Onnx Model file size: {size:.2f} MB")
     return model_class.from_pretrained(model_dir, file_name=FILENAME_OPTIMIZED_ONNX)
```

### Comparing `bpm_ai_inference-0.2.9/pyproject.toml` & `bpm_ai_inference-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [tool.poetry]
 name = "bpm-ai-inference"
-version = "0.2.9"
+version = "0.3.0"
 description = "Inference and server for local AI implementations of bpm-ai-core abstractions."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai-inference"
 homepage = "https://www.holisticon.de/"
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
-bpm-ai-core = "^2.4.2"
+bpm-ai-core = "^2.6.0"
 langfuse = "^2.7.6"
 faster-whisper = "^0.10.0"
 lingua-language-detector = "^2.0.2"
 pytesseract = "^0.3.10"
-transformers = "^4.37.2"
+transformers = "^4.39.3"
 sacremoses = "^0.1.1"
 sentencepiece = "^0.2.0"
 nltk = "^3.8.0"
-pyro5 = "^5.15"
 optimum = {extras = ["onnxruntime"], version = "^1.18.0"}
 gliner = "^0.1.6"
 scipy = "1.10.1"
 py-cpuinfo = "^9.0.0"
+llama-cpp-python = "^0.2.65"
+#fast-fit = "^1.2.0"
+#jupyter = "^1.0.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.2"
 pytest-asyncio = "^0.23.5"
 pytest-dotenv = "^0.5.2"
```

### Comparing `bpm_ai_inference-0.2.9/PKG-INFO` & `bpm_ai_inference-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: bpm-ai-inference
-Version: 0.2.9
+Version: 0.3.0
 Summary: Inference and server for local AI implementations of bpm-ai-core abstractions.
 Home-page: https://www.holisticon.de/
 License: GPL-3.0-or-later
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bpm-ai-core (>=2.4.2,<3.0.0)
+Requires-Dist: bpm-ai-core (>=2.6.0,<3.0.0)
 Requires-Dist: faster-whisper (>=0.10.0,<0.11.0)
 Requires-Dist: gliner (>=0.1.6,<0.2.0)
 Requires-Dist: langfuse (>=2.7.6,<3.0.0)
 Requires-Dist: lingua-language-detector (>=2.0.2,<3.0.0)
+Requires-Dist: llama-cpp-python (>=0.2.65,<0.3.0)
 Requires-Dist: nltk (>=3.8.0,<4.0.0)
 Requires-Dist: optimum[onnxruntime] (>=1.18.0,<2.0.0)
 Requires-Dist: py-cpuinfo (>=9.0.0,<10.0.0)
-Requires-Dist: pyro5 (>=5.15,<6.0)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
 Requires-Dist: sacremoses (>=0.1.1,<0.2.0)
 Requires-Dist: scipy (==1.10.1)
 Requires-Dist: sentencepiece (>=0.2.0,<0.3.0)
-Requires-Dist: transformers (>=4.37.2,<5.0.0)
+Requires-Dist: transformers (>=4.39.3,<5.0.0)
 Project-URL: Repository, https://github.com/holunda-io/bpm-ai-inference
 Description-Content-Type: text/markdown
 
 # bpm-ai-inference
 
 Extension to bpm-ai project for local AI inference.
```

