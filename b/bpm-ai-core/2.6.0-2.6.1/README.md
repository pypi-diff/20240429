# Comparing `tmp/bpm_ai_core-2.6.0.tar.gz` & `tmp/bpm_ai_core-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_core-2.6.0.tar", max compression
+gzip compressed data, was "bpm_ai_core-2.6.1.tar", max compression
```

## Comparing `bpm_ai_core-2.6.0.tar` & `bpm_ai_core-2.6.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0       13 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/README.md
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/image_classification/__init__.py
--rw-r--r--   0        0        0     1532 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/image_classification/image_classifier.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/__init__.py
--rw-r--r--   0        0        0      864 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/__init__.py
--rw-r--r--   0        0        0      306 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/_constants.py
--rw-r--r--   0        0        0     6753 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
--rw-r--r--   0        0        0      226 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
--rw-r--r--   0        0        0     4929 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/common/__init__.py
--rw-r--r--   0        0        0     6142 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/common/blob.py
--rw-r--r--   0        0        0     2674 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/common/llm.py
--rw-r--r--   0        0        0     2710 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/common/message.py
--rw-r--r--   0        0        0     2781 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/common/tool.py
--rw-r--r--   0        0        0     1459 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/__init__.py
--rw-r--r--   0        0        0      430 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/_constants.py
--rw-r--r--   0        0        0     8438 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/openai_chat.py
--rw-r--r--   0        0        0     3397 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/ocr/__init__.py
--rw-r--r--   0        0        0     5669 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/ocr/amazon_textract.py
--rw-r--r--   0        0        0     2789 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/ocr/azure_doc_intelligence.py
--rw-r--r--   0        0        0     1343 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/ocr/ocr.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/pos/__init__.py
--rw-r--r--   0        0        0      590 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/pos/pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/prompt/__init__.py
--rw-r--r--   0        0        0      372 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/prompt/filters.py
--rw-r--r--   0        0        0     6898 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/prompt/prompt.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/question_answering/__init__.py
--rw-r--r--   0        0        0     2047 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py
--rw-r--r--   0        0        0     3086 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
--rw-r--r--   0        0        0     1463 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/question_answering/question_answering.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/speech_recognition/__init__.py
--rw-r--r--   0        0        0     1200 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/speech_recognition/asr.py
--rw-r--r--   0        0        0     1486 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/speech_recognition/openai_whisper.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/testing/__init__.py
--rw-r--r--   0        0        0     2894 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/testing/fake_llm.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/text_classification/__init__.py
--rw-r--r--   0        0        0     1495 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/text_classification/text_classifier.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/token_classification/__init__.py
--rw-r--r--   0        0        0      968 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/__init__.py
--rw-r--r--   0        0        0     2434 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/decorators.py
--rw-r--r--   0        0        0     1597 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/delegate.py
--rw-r--r--   0        0        0     4381 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/langfuse.py
--rw-r--r--   0        0        0     2347 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/logging.py
--rw-r--r--   0        0        0     1097 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/tracer.py
--rw-r--r--   0        0        0      876 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/tracing.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/translation/__init__.py
--rw-r--r--   0        0        0     1360 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/translation/amazon_translate.py
--rw-r--r--   0        0        0     1630 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/translation/azure_translation.py
--rw-r--r--   0        0        0      593 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/translation/nmt.py
--rw-r--r--   0        0        0        0 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/__init__.py
--rw-r--r--   0        0        0     1154 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/audio.py
--rw-r--r--   0        0        0     4427 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/caching.py
--rw-r--r--   0        0        0     2290 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/file.py
--rw-r--r--   0        0        0     6130 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/image.py
--rw-r--r--   0        0        0     3135 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/json_schema.py
--rw-r--r--   0        0        0    22412 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/linguistics.py
--rw-r--r--   0        0        0     1130 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/markdown.py
--rw-r--r--   0        0        0     4278 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/rpc.py
--rw-r--r--   0        0        0     2596 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/storage.py
--rw-r--r--   0        0        0      670 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/text.py
--rw-r--r--   0        0        0      675 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/xml_convert.py
--rw-r--r--   0        0        0     1059 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 bpm_ai_core-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/image_classification/__init__.py
+-rw-r--r--   0        0        0     1532 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/image_classification/image_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/__init__.py
+-rw-r--r--   0        0        0      864 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/anthropic_chat/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/anthropic_chat/_constants.py
+-rw-r--r--   0        0        0     6753 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
+-rw-r--r--   0        0        0      226 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
+-rw-r--r--   0        0        0     4929 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/anthropic_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/common/__init__.py
+-rw-r--r--   0        0        0     6142 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/common/blob.py
+-rw-r--r--   0        0        0     2674 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/common/llm.py
+-rw-r--r--   0        0        0     2710 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/common/message.py
+-rw-r--r--   0        0        0     2781 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/common/tool.py
+-rw-r--r--   0        0        0     1459 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/openai_chat/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/openai_chat/_constants.py
+-rw-r--r--   0        0        0     8438 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/openai_chat/openai_chat.py
+-rw-r--r--   0        0        0     3397 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/llm/openai_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/ocr/__init__.py
+-rw-r--r--   0        0        0     5669 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/ocr/amazon_textract.py
+-rw-r--r--   0        0        0     2789 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/ocr/azure_doc_intelligence.py
+-rw-r--r--   0        0        0     1343 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/ocr/ocr.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/pos/__init__.py
+-rw-r--r--   0        0        0      590 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/pos/pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/prompt/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/prompt/filters.py
+-rw-r--r--   0        0        0     6898 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/prompt/prompt.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/question_answering/__init__.py
+-rw-r--r--   0        0        0     2047 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/question_answering/amazon_textract_docvqa.py
+-rw-r--r--   0        0        0     3086 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
+-rw-r--r--   0        0        0     1463 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/question_answering/question_answering.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/speech_recognition/__init__.py
+-rw-r--r--   0        0        0     1200 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/speech_recognition/asr.py
+-rw-r--r--   0        0        0     1486 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/speech_recognition/openai_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/testing/__init__.py
+-rw-r--r--   0        0        0     2894 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/testing/fake_llm.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/text_classification/__init__.py
+-rw-r--r--   0        0        0     1495 2024-04-29 09:52:56.535573 bpm_ai_core-2.6.1/bpm_ai_core/text_classification/text_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/token_classification/__init__.py
+-rw-r--r--   0        0        0      968 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/token_classification/zero_shot_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/tracing/__init__.py
+-rw-r--r--   0        0        0     2434 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/tracing/decorators.py
+-rw-r--r--   0        0        0     1597 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/tracing/delegate.py
+-rw-r--r--   0        0        0     4381 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/tracing/langfuse.py
+-rw-r--r--   0        0        0     2347 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/tracing/logging.py
+-rw-r--r--   0        0        0     1097 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/tracing/tracer.py
+-rw-r--r--   0        0        0      876 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/tracing/tracing.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/translation/__init__.py
+-rw-r--r--   0        0        0     1360 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/translation/amazon_translate.py
+-rw-r--r--   0        0        0     1630 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/translation/azure_translation.py
+-rw-r--r--   0        0        0      593 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/translation/nmt.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/util/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/util/audio.py
+-rw-r--r--   0        0        0     4423 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/util/caching.py
+-rw-r--r--   0        0        0     2290 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/util/file.py
+-rw-r--r--   0        0        0     6130 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/util/image.py
+-rw-r--r--   0        0        0     3135 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/util/json_schema.py
+-rw-r--r--   0        0        0    22412 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/util/linguistics.py
+-rw-r--r--   0        0        0     1130 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/util/markdown.py
+-rw-r--r--   0        0        0     4600 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/util/rpc.py
+-rw-r--r--   0        0        0     2596 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/util/storage.py
+-rw-r--r--   0        0        0      670 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/util/text.py
+-rw-r--r--   0        0        0      675 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/bpm_ai_core/util/xml_convert.py
+-rw-r--r--   0        0        0     1059 2024-04-29 09:52:56.539573 bpm_ai_core-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 bpm_ai_core-2.6.1/PKG-INFO
```

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/image_classification/image_classifier.py` & `bpm_ai_core-2.6.1/bpm_ai_core/image_classification/image_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/__init__.py` & `bpm_ai_core-2.6.1/bpm_ai_core/llm/anthropic_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py` & `bpm_ai_core-2.6.1/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/util.py` & `bpm_ai_core-2.6.1/bpm_ai_core/llm/anthropic_chat/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/llm/common/blob.py` & `bpm_ai_core-2.6.1/bpm_ai_core/llm/common/blob.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/llm/common/llm.py` & `bpm_ai_core-2.6.1/bpm_ai_core/llm/common/llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/llm/common/message.py` & `bpm_ai_core-2.6.1/bpm_ai_core/llm/common/message.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/llm/common/tool.py` & `bpm_ai_core-2.6.1/bpm_ai_core/llm/common/tool.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/__init__.py` & `bpm_ai_core-2.6.1/bpm_ai_core/llm/openai_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/openai_chat.py` & `bpm_ai_core-2.6.1/bpm_ai_core/llm/openai_chat/openai_chat.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/util.py` & `bpm_ai_core-2.6.1/bpm_ai_core/llm/openai_chat/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/ocr/amazon_textract.py` & `bpm_ai_core-2.6.1/bpm_ai_core/ocr/amazon_textract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/ocr/azure_doc_intelligence.py` & `bpm_ai_core-2.6.1/bpm_ai_core/ocr/azure_doc_intelligence.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/ocr/ocr.py` & `bpm_ai_core-2.6.1/bpm_ai_core/ocr/ocr.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/pos/pos_tagger.py` & `bpm_ai_core-2.6.1/bpm_ai_core/pos/pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/prompt/prompt.py` & `bpm_ai_core-2.6.1/bpm_ai_core/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py` & `bpm_ai_core-2.6.1/bpm_ai_core/question_answering/amazon_textract_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py` & `bpm_ai_core-2.6.1/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/question_answering/question_answering.py` & `bpm_ai_core-2.6.1/bpm_ai_core/question_answering/question_answering.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/speech_recognition/asr.py` & `bpm_ai_core-2.6.1/bpm_ai_core/speech_recognition/asr.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/speech_recognition/openai_whisper.py` & `bpm_ai_core-2.6.1/bpm_ai_core/speech_recognition/openai_whisper.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/testing/fake_llm.py` & `bpm_ai_core-2.6.1/bpm_ai_core/testing/fake_llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/text_classification/text_classifier.py` & `bpm_ai_core-2.6.1/bpm_ai_core/text_classification/text_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py` & `bpm_ai_core-2.6.1/bpm_ai_core/token_classification/zero_shot_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/tracing/decorators.py` & `bpm_ai_core-2.6.1/bpm_ai_core/tracing/decorators.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/tracing/delegate.py` & `bpm_ai_core-2.6.1/bpm_ai_core/tracing/delegate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/tracing/langfuse.py` & `bpm_ai_core-2.6.1/bpm_ai_core/tracing/langfuse.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/tracing/logging.py` & `bpm_ai_core-2.6.1/bpm_ai_core/tracing/logging.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/tracing/tracer.py` & `bpm_ai_core-2.6.1/bpm_ai_core/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/tracing/tracing.py` & `bpm_ai_core-2.6.1/bpm_ai_core/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/translation/amazon_translate.py` & `bpm_ai_core-2.6.1/bpm_ai_core/translation/amazon_translate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/translation/azure_translation.py` & `bpm_ai_core-2.6.1/bpm_ai_core/translation/azure_translation.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/translation/nmt.py` & `bpm_ai_core-2.6.1/bpm_ai_core/translation/nmt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/util/audio.py` & `bpm_ai_core-2.6.1/bpm_ai_core/util/audio.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/util/caching.py` & `bpm_ai_core-2.6.1/bpm_ai_core/util/caching.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
             # Include all function parameters, excluding the specified ones
             exclude_params = set(exclude) if exclude else set()
             sig = inspect.signature(func)
             bound_args = sig.bind_partial(self, *args, **kwargs)
             bound_args.apply_defaults()
             for param_name, param_value in bound_args.arguments.items():
-                if param_name not in exclude_params and param_name is not "self":
+                if param_name not in exclude_params and param_name != "self":
                     cache_key_components.append(f"{param_name}={param_value}")
 
             if key_func:
                 custom_key_part = await key_func(*args, **kwargs)
                 cache_key_components.append(custom_key_part)
 
             logger.debug(f"Cache key components: {cache_key_components}")
```

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/util/file.py` & `bpm_ai_core-2.6.1/bpm_ai_core/util/file.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/util/image.py` & `bpm_ai_core-2.6.1/bpm_ai_core/util/image.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/util/json_schema.py` & `bpm_ai_core-2.6.1/bpm_ai_core/util/json_schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/util/linguistics.py` & `bpm_ai_core-2.6.1/bpm_ai_core/util/linguistics.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/util/markdown.py` & `bpm_ai_core-2.6.1/bpm_ai_core/util/markdown.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/util/rpc.py` & `bpm_ai_core-2.6.1/bpm_ai_core/util/rpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,26 +71,33 @@
         self.class_name = class_name
         self.host = host
         self.port = port
         self.instance_args = instance_args or ()
         self.instance_kwargs = instance_kwargs or {}
 
     def __getattr__(self, name):
+        if name == '__slots__':
+            return ['class_name', 'host', 'port', 'instance_args', 'instance_kwargs']
+
         async def remote_method(*args, **kwargs):
             data = pickle.dumps((self.class_name, name, args, kwargs, self.instance_args, self.instance_kwargs))
             async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=600)) as session:
                 async with session.post(f'http://{self.host}:{self.port}/rpc', data=data) as response:
                     if response.status == 200:
                         result = await response.read()
                         return pickle.loads(result)
                     else:
                         error_message = await response.text()
                         raise Exception(f"Remote method call failed: {error_message}")
+
         return remote_method
 
+    def __str__(self):
+        return f"RemoteObjectProxy(class_name={self.class_name}, host={self.host}, port={self.port}, instance_args={self.instance_args}, instance_kwargs={self.instance_kwargs})"
+
 
 def create_remote_object_daemon(
         host='0.0.0.0',
         port=8008,
         instance_strategy='memory_limit',
         max_memory: int = 8 * 1024 * 1024 * 1024
 ):
```

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/util/storage.py` & `bpm_ai_core-2.6.1/bpm_ai_core/util/storage.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/util/text.py` & `bpm_ai_core-2.6.1/bpm_ai_core/util/text.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/bpm_ai_core/util/xml_convert.py` & `bpm_ai_core-2.6.1/bpm_ai_core/util/xml_convert.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.6.0/pyproject.toml` & `bpm_ai_core-2.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai-core"
-version = "2.6.0"
+version = "2.6.1"
 description = "Core AI abstractions and helpers."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `bpm_ai_core-2.6.0/PKG-INFO` & `bpm_ai_core-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai-core
-Version: 2.6.0
+Version: 2.6.1
 Summary: Core AI abstractions and helpers.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

