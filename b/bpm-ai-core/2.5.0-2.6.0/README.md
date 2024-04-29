# Comparing `tmp/bpm_ai_core-2.5.0.tar.gz` & `tmp/bpm_ai_core-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_core-2.5.0.tar", max compression
+gzip compressed data, was "bpm_ai_core-2.6.0.tar", max compression
```

## Comparing `bpm_ai_core-2.5.0.tar` & `bpm_ai_core-2.6.0.tar`

### file list

```diff
@@ -1,64 +1,66 @@
--rw-r--r--   0        0        0       13 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/README.md
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/classification/__init__.py
--rw-r--r--   0        0        0     1478 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/classification/zero_shot_classifier.py
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/__init__.py
--rw-r--r--   0        0        0      864 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/__init__.py
--rw-r--r--   0        0        0      306 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/_constants.py
--rw-r--r--   0        0        0     6753 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
--rw-r--r--   0        0        0      226 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
--rw-r--r--   0        0        0     4929 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/common/__init__.py
--rw-r--r--   0        0        0     6142 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/common/blob.py
--rw-r--r--   0        0        0     2674 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/common/llm.py
--rw-r--r--   0        0        0     2710 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/common/message.py
--rw-r--r--   0        0        0     2781 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/common/tool.py
--rw-r--r--   0        0        0     1459 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/__init__.py
--rw-r--r--   0        0        0      430 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/_constants.py
--rw-r--r--   0        0        0     8438 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/openai_chat.py
--rw-r--r--   0        0        0     3397 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/ocr/__init__.py
--rw-r--r--   0        0        0     5669 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/ocr/amazon_textract.py
--rw-r--r--   0        0        0     2789 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/ocr/azure_doc_intelligence.py
--rw-r--r--   0        0        0     1631 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/ocr/ocr.py
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/pos/__init__.py
--rw-r--r--   0        0        0      590 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/pos/pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/prompt/__init__.py
--rw-r--r--   0        0        0      372 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/prompt/filters.py
--rw-r--r--   0        0        0     6420 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/prompt/prompt.py
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/question_answering/__init__.py
--rw-r--r--   0        0        0     2047 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py
--rw-r--r--   0        0        0     3086 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
--rw-r--r--   0        0        0     1463 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/question_answering/question_answering.py
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/speech_recognition/__init__.py
--rw-r--r--   0        0        0     1188 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/speech_recognition/asr.py
--rw-r--r--   0        0        0     1486 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/speech_recognition/openai_whisper.py
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/testing/__init__.py
--rw-r--r--   0        0        0     2894 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/testing/fake_llm.py
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/token_classification/__init__.py
--rw-r--r--   0        0        0      968 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/__init__.py
--rw-r--r--   0        0        0     2434 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/decorators.py
--rw-r--r--   0        0        0     1597 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/delegate.py
--rw-r--r--   0        0        0     4381 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/langfuse.py
--rw-r--r--   0        0        0     2347 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/logging.py
--rw-r--r--   0        0        0     1097 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/tracer.py
--rw-r--r--   0        0        0      876 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/tracing/tracing.py
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/translation/__init__.py
--rw-r--r--   0        0        0     1360 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/translation/amazon_translate.py
--rw-r--r--   0        0        0     1630 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/translation/azure_translation.py
--rw-r--r--   0        0        0      593 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/translation/nmt.py
--rw-r--r--   0        0        0        0 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/__init__.py
--rw-r--r--   0        0        0     1154 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/audio.py
--rw-r--r--   0        0        0     4125 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/caching.py
--rw-r--r--   0        0        0     2290 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/file.py
--rw-r--r--   0        0        0     6130 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/image.py
--rw-r--r--   0        0        0     3135 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/json_schema.py
--rw-r--r--   0        0        0    22412 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/linguistics.py
--rw-r--r--   0        0        0     1130 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/markdown.py
--rw-r--r--   0        0        0     4278 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/rpc.py
--rw-r--r--   0        0        0     2596 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/storage.py
--rw-r--r--   0        0        0      670 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/text.py
--rw-r--r--   0        0        0      675 2024-04-24 14:39:08.472771 bpm_ai_core-2.5.0/bpm_ai_core/util/xml_convert.py
--rw-r--r--   0        0        0     1059 2024-04-24 14:39:08.476771 bpm_ai_core-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 bpm_ai_core-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/image_classification/__init__.py
+-rw-r--r--   0        0        0     1532 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/image_classification/image_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/__init__.py
+-rw-r--r--   0        0        0      864 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/_constants.py
+-rw-r--r--   0        0        0     6753 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
+-rw-r--r--   0        0        0      226 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
+-rw-r--r--   0        0        0     4929 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/common/__init__.py
+-rw-r--r--   0        0        0     6142 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/common/blob.py
+-rw-r--r--   0        0        0     2674 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/common/llm.py
+-rw-r--r--   0        0        0     2710 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/common/message.py
+-rw-r--r--   0        0        0     2781 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/common/tool.py
+-rw-r--r--   0        0        0     1459 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/_constants.py
+-rw-r--r--   0        0        0     8438 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/openai_chat.py
+-rw-r--r--   0        0        0     3397 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/ocr/__init__.py
+-rw-r--r--   0        0        0     5669 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/ocr/amazon_textract.py
+-rw-r--r--   0        0        0     2789 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/ocr/azure_doc_intelligence.py
+-rw-r--r--   0        0        0     1343 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/ocr/ocr.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/pos/__init__.py
+-rw-r--r--   0        0        0      590 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/pos/pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/prompt/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/prompt/filters.py
+-rw-r--r--   0        0        0     6898 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/prompt/prompt.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/question_answering/__init__.py
+-rw-r--r--   0        0        0     2047 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py
+-rw-r--r--   0        0        0     3086 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
+-rw-r--r--   0        0        0     1463 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/question_answering/question_answering.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.530877 bpm_ai_core-2.6.0/bpm_ai_core/speech_recognition/__init__.py
+-rw-r--r--   0        0        0     1200 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/speech_recognition/asr.py
+-rw-r--r--   0        0        0     1486 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/speech_recognition/openai_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/testing/__init__.py
+-rw-r--r--   0        0        0     2894 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/testing/fake_llm.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/text_classification/__init__.py
+-rw-r--r--   0        0        0     1495 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/text_classification/text_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/token_classification/__init__.py
+-rw-r--r--   0        0        0      968 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/__init__.py
+-rw-r--r--   0        0        0     2434 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/decorators.py
+-rw-r--r--   0        0        0     1597 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/delegate.py
+-rw-r--r--   0        0        0     4381 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/langfuse.py
+-rw-r--r--   0        0        0     2347 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/logging.py
+-rw-r--r--   0        0        0     1097 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/tracer.py
+-rw-r--r--   0        0        0      876 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/tracing/tracing.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/translation/__init__.py
+-rw-r--r--   0        0        0     1360 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/translation/amazon_translate.py
+-rw-r--r--   0        0        0     1630 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/translation/azure_translation.py
+-rw-r--r--   0        0        0      593 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/translation/nmt.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/audio.py
+-rw-r--r--   0        0        0     4427 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/caching.py
+-rw-r--r--   0        0        0     2290 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/file.py
+-rw-r--r--   0        0        0     6130 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/image.py
+-rw-r--r--   0        0        0     3135 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/json_schema.py
+-rw-r--r--   0        0        0    22412 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/linguistics.py
+-rw-r--r--   0        0        0     1130 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/markdown.py
+-rw-r--r--   0        0        0     4278 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/rpc.py
+-rw-r--r--   0        0        0     2596 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/storage.py
+-rw-r--r--   0        0        0      670 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/text.py
+-rw-r--r--   0        0        0      675 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/bpm_ai_core/util/xml_convert.py
+-rw-r--r--   0        0        0     1059 2024-04-29 06:59:14.534878 bpm_ai_core-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 bpm_ai_core-2.6.0/PKG-INFO
```

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/classification/zero_shot_classifier.py` & `bpm_ai_core-2.6.0/bpm_ai_core/text_classification/text_classifier.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,35 +9,35 @@
 
 class ClassificationResult(BaseModel):
     max_label: str
     max_score: float
     labels_scores: list[Tuple[str, float]]
 
 
-class ZeroShotClassifier(ABC):
+class TextClassifier(ABC):
     """
-    Zero Shot Classification Model
+    (Zero Shot) Text Classification Model
     """
 
     @abstractmethod
     async def _do_classify(
             self,
             text: str,
-            classes: list[str],
+            classes: list[str] = None,
             hypothesis_template: str | None = None,
             multi_label: bool = False
     ) -> ClassificationResult:
         pass
 
     @cached()
     @span(name="classifier")
     async def classify(
             self,
             text: str,
-            classes: list[str],
+            classes: list[str] = None,
             confidence_threshold: float | None = None,
             hypothesis_template: str | None = None,
             multi_label: bool = False
     ) -> ClassificationResult:
         result = await self._do_classify(
             text=text,
             classes=classes,
```

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/__init__.py` & `bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py` & `bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/llm/anthropic_chat/util.py` & `bpm_ai_core-2.6.0/bpm_ai_core/llm/anthropic_chat/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/llm/common/blob.py` & `bpm_ai_core-2.6.0/bpm_ai_core/llm/common/blob.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/llm/common/llm.py` & `bpm_ai_core-2.6.0/bpm_ai_core/llm/common/llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/llm/common/message.py` & `bpm_ai_core-2.6.0/bpm_ai_core/llm/common/message.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/llm/common/tool.py` & `bpm_ai_core-2.6.0/bpm_ai_core/llm/common/tool.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/__init__.py` & `bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/openai_chat.py` & `bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/openai_chat.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/llm/openai_chat/util.py` & `bpm_ai_core-2.6.0/bpm_ai_core/llm/openai_chat/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/ocr/amazon_textract.py` & `bpm_ai_core-2.6.0/bpm_ai_core/ocr/amazon_textract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/ocr/azure_doc_intelligence.py` & `bpm_ai_core-2.6.0/bpm_ai_core/ocr/azure_doc_intelligence.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/ocr/ocr.py` & `bpm_ai_core-2.6.0/bpm_ai_core/ocr/ocr.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import Tuple
 
 from pydantic import BaseModel, Field
 
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.tracing.decorators import span
-from bpm_ai_core.util.caching import cached, calculate_cache_key
+from bpm_ai_core.util.caching import cached, blob_cache_key
 
 
 class OCRPage(BaseModel):
     text: str
     words: list[str] = Field(..., exclude=True)
     bboxes: list[Tuple[float, float, float, float]] = Field(..., exclude=True)
     """Format: (x, y, x + w, y + h), normalized to 1"""
@@ -32,22 +32,15 @@
     async def _do_process(
             self,
             blob: Blob,
             language: str = None
     ) -> OCRResult:
         pass
 
-    async def _cache_key(self, blob_or_path: Blob | str, *args, **kwargs) -> str:
-        if isinstance(blob_or_path, str):
-            blob = Blob.from_path_or_url(blob_or_path)
-        else:  # Blob
-            blob = blob_or_path
-        return f"blob_bytes={await blob.as_bytes()}"
-
-    @cached(exclude=["blob_or_path"], key_func=_cache_key)
+    @cached(exclude=["blob_or_path"], key_func=blob_cache_key)
     @span(name="ocr")
     async def process(
             self,
             blob_or_path: Blob | str,
             language: str = None
     ) -> OCRResult:
         if isinstance(blob_or_path, str):
```

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/pos/pos_tagger.py` & `bpm_ai_core-2.6.0/bpm_ai_core/pos/pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/prompt/prompt.py` & `bpm_ai_core-2.6.0/bpm_ai_core/prompt/prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import glob
 import inspect
 import os
 import re
 from typing import List, Dict, Any
 
 from jinja2 import Template, environment
 
@@ -13,37 +14,47 @@
 environment.DEFAULT_FILTERS['markdown'] = dict_to_markdown
 environment.DEFAULT_FILTERS['json'] = dict_to_json
 environment.DEFAULT_FILTERS['xml'] = dict_to_xml
 
 
 class Prompt:
 
-    def __init__(self, kwargs: Dict[str, Any], path: str | None = None, template_str: str | None = None) -> None:
-        self.path = path
+    def __init__(self, kwargs: dict[str, Any], template_str: str = None, path: str = None, prompt_templates: dict = None) -> None:
         self.template_str = template_str
         self.template_vars = kwargs
+        self.path = path
+        self.prompt_templates = prompt_templates
 
     @classmethod
     def from_file(cls, path: str, **kwargs):
         # Get the frame of the caller of the function that called this function
         caller_frame = inspect.stack()[1]
         caller_filename = caller_frame.filename
 
         # Get the directory of the caller's file
         current_dir = os.path.dirname(os.path.abspath(caller_filename))
         file_path = os.path.join(current_dir, path)
 
-        return cls(kwargs, path=file_path)
+        prompt_templates = {}
+
+        default_file_path = f"{file_path}.prompt"
+        specific_file_path = f"{file_path}.*.prompt"
+        prompt_files = glob.glob(specific_file_path) + [default_file_path]
+        for prompt_file in prompt_files:
+            with open(prompt_file, 'r') as p:
+                prompt_templates[os.path.basename(prompt_file)] = p.read()
+
+        return cls(kwargs, path=path, prompt_templates=prompt_templates)
 
     @classmethod
     def from_string(cls, template: str, **kwargs):
         return cls(kwargs, template_str=template)
 
     def format(self, llm_name: str = "") -> List[ChatMessage]:
-        template = self.load_template(self.path, llm_name) if self.path else Template(self.template_str)
+        template = self.load_template(llm_name)
         full_prompt = template.render(self.template_vars)
 
         regex = r'\[#\s*(user|assistant|system|tool_result:.*|)\s*#\]'
         blob_regex = r'\[#\s*blob\s*(.*?)\s*#\]'
         tool_call_regex = r'\[#\s*tool_call:\s*(.*?)\s*#\]'
 
         # Check if the raw template contains message prompt sections
@@ -126,19 +137,20 @@
                 messages.append(message)
         else:
             # If the raw template doesn't contain any sections, treat whole file as 'user' message
             messages = [UserMessage(content=full_prompt)]
 
         return [m for m in messages if m]
 
-    @staticmethod
-    def load_template(path: str, llm_name: str) -> Template:
-        default_path = f"{path}.prompt"
-        llm_specific_path = f"{path}.{llm_name}.prompt"
-        filename = llm_specific_path if os.path.exists(llm_specific_path) else default_path
-        if not os.path.exists(filename):
-            raise FileNotFoundError(f"No prompt file found at {filename}")
-        with open(filename, 'r') as f:
-            return Template(f.read())
+    def load_template(self, llm_name: str) -> Template:
+        if self.path:
+            default_prompt = f"{self.path}.prompt"
+            llm_specific_prompt = f"{self.path}.{llm_name}.prompt"
+            prompt = self.prompt_templates.get(llm_specific_prompt, self.prompt_templates.get(default_prompt))
+            if not prompt:
+                raise FileNotFoundError(f"No prompt file {self.path} found for llm {llm_name}")
+        else:
+            prompt = self.template_str
+        return Template(prompt)
 
     def __repr__(self):
         return f"{self.__class__.__qualname__}(template_vars={self.template_vars}, path={self.path}, template_str={self.template_str})"
```

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py` & `bpm_ai_core-2.6.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py` & `bpm_ai_core-2.6.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/question_answering/question_answering.py` & `bpm_ai_core-2.6.0/bpm_ai_core/question_answering/question_answering.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/speech_recognition/openai_whisper.py` & `bpm_ai_core-2.6.0/bpm_ai_core/speech_recognition/openai_whisper.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/testing/fake_llm.py` & `bpm_ai_core-2.6.0/bpm_ai_core/testing/fake_llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py` & `bpm_ai_core-2.6.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/tracing/decorators.py` & `bpm_ai_core-2.6.0/bpm_ai_core/tracing/decorators.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/tracing/delegate.py` & `bpm_ai_core-2.6.0/bpm_ai_core/tracing/delegate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/tracing/langfuse.py` & `bpm_ai_core-2.6.0/bpm_ai_core/tracing/langfuse.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/tracing/logging.py` & `bpm_ai_core-2.6.0/bpm_ai_core/tracing/logging.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/tracing/tracer.py` & `bpm_ai_core-2.6.0/bpm_ai_core/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/tracing/tracing.py` & `bpm_ai_core-2.6.0/bpm_ai_core/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/translation/amazon_translate.py` & `bpm_ai_core-2.6.0/bpm_ai_core/translation/amazon_translate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/translation/azure_translation.py` & `bpm_ai_core-2.6.0/bpm_ai_core/translation/azure_translation.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/translation/nmt.py` & `bpm_ai_core-2.6.0/bpm_ai_core/translation/nmt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/util/audio.py` & `bpm_ai_core-2.6.0/bpm_ai_core/util/audio.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/util/caching.py` & `bpm_ai_core-2.6.0/bpm_ai_core/util/caching.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import hashlib
 import inspect
 import logging
 import os
 
 from diskcache import Cache
 
+from bpm_ai_core.llm.common.blob import Blob
+
 logger = logging.getLogger(__name__)
 
 
 _cache = Cache(directory=os.path.join(os.path.expanduser("~"), ".cache", "bpm-ai", "predictions"))
 
 
 def calculate_cache_key(data: tuple) -> str:
@@ -50,15 +52,15 @@
             bound_args = sig.bind_partial(self, *args, **kwargs)
             bound_args.apply_defaults()
             for param_name, param_value in bound_args.arguments.items():
                 if param_name not in exclude_params and param_name is not "self":
                     cache_key_components.append(f"{param_name}={param_value}")
 
             if key_func:
-                custom_key_part = await key_func(self, *args, **kwargs)
+                custom_key_part = await key_func(*args, **kwargs)
                 cache_key_components.append(custom_key_part)
 
             logger.debug(f"Cache key components: {cache_key_components}")
 
             cache_key = hashlib.sha256(":".join(cache_key_components).encode()).hexdigest()
             cache_key = f"{self.__class__.__module__}__{self.__class__.__qualname__}__{func.__name__}__" + cache_key
 
@@ -104,7 +106,15 @@
             original_init(self, *args, **kwargs)
 
         cls.__init__ = __init__
 
         return cls
 
     return decorator
+
+
+async def blob_cache_key(blob_or_path: Blob | str, *args, **kwargs) -> str:
+    if isinstance(blob_or_path, str):
+        blob = Blob.from_path_or_url(blob_or_path)
+    else:  # Blob
+        blob = blob_or_path
+    return f"blob_bytes={await blob.as_bytes()}"
```

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/util/file.py` & `bpm_ai_core-2.6.0/bpm_ai_core/util/file.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/util/image.py` & `bpm_ai_core-2.6.0/bpm_ai_core/util/image.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/util/json_schema.py` & `bpm_ai_core-2.6.0/bpm_ai_core/util/json_schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/util/linguistics.py` & `bpm_ai_core-2.6.0/bpm_ai_core/util/linguistics.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/util/markdown.py` & `bpm_ai_core-2.6.0/bpm_ai_core/util/markdown.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/util/rpc.py` & `bpm_ai_core-2.6.0/bpm_ai_core/util/rpc.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/util/storage.py` & `bpm_ai_core-2.6.0/bpm_ai_core/util/storage.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/util/text.py` & `bpm_ai_core-2.6.0/bpm_ai_core/util/text.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/bpm_ai_core/util/xml_convert.py` & `bpm_ai_core-2.6.0/bpm_ai_core/util/xml_convert.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.5.0/pyproject.toml` & `bpm_ai_core-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai-core"
-version = "2.5.0"
+version = "2.6.0"
 description = "Core AI abstractions and helpers."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `bpm_ai_core-2.5.0/PKG-INFO` & `bpm_ai_core-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai-core
-Version: 2.5.0
+Version: 2.6.0
 Summary: Core AI abstractions and helpers.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

