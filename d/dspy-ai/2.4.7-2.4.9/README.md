# Comparing `tmp/dspy-ai-2.4.7.tar.gz` & `tmp/dspy-ai-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dspy-ai-2.4.7.tar", last modified: Mon Apr  8 20:57:43 2024, max compression
+gzip compressed data, was "dspy-ai-2.4.9.tar", last modified: Mon Apr 29 20:58:33 2024, max compression
```

## Comparing `dspy-ai-2.4.7.tar` & `dspy-ai-2.4.9.tar`

### file list

```diff
@@ -1,159 +1,167 @@
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/
--rw-r--r--   0 okhattab (19845) future   (20099)     1085 2024-04-08 16:37:16.000000 dspy-ai-2.4.7/LICENSE
--rw-r--r--   0 okhattab (19845) future   (20099)    35318 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/PKG-INFO
--rw-r--r--   0 okhattab (19845) future   (20099)    34442 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/README.md
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/
--rw-r--r--   0 okhattab (19845) future   (20099)     1532 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/evaluation/
--rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/evaluation/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2586 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/evaluation/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/modules/
--rw-r--r--   0 okhattab (19845) future   (20099)      446 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4547 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dsp/modules/anthropic.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6551 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/aws_lm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9196 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/azure_openai.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2688 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/azurecognitivesearch.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3102 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/bedrock.py
--rw-r--r--   0 okhattab (19845) future   (20099)      964 2024-04-08 20:57:18.000000 dspy-ai-2.4.7/dsp/modules/cache_utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3008 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/clarifai.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4346 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/cohere.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2156 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/colbertv2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5459 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/databricks.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/modules/finetuning/
--rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/finetuning/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    15071 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/finetuning/finetune_hf.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4552 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/google.py
--rw-r--r--   0 okhattab (19845) future   (20099)     8519 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/gpt3.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7705 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/hf.py
--rw-r--r--   0 okhattab (19845) future   (20099)    15089 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/hf_client.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2087 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/hf_server.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3258 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/modules/lm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6751 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/ollama.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3152 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/pyserini.py
--rw-r--r--   0 okhattab (19845) future   (20099)      693 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/sbert.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7787 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/modules/sentence_vectorizer.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/primitives/
--rw-r--r--   0 okhattab (19845) future   (20099)      145 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/primitives/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5185 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/primitives/compiler.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5789 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/primitives/demonstrate.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2471 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/primitives/inspect.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7948 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dsp/primitives/predict.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1439 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/primitives/primitives.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2681 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dsp/primitives/search.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/templates/
--rw-r--r--   0 okhattab (19845) future   (20099)       76 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/templates/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10226 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/templates/template_v2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2334 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/templates/template_v3.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1900 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/templates/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dsp/utils/
--rw-r--r--   0 okhattab (19845) future   (20099)      123 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/utils/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4903 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/utils/ann_utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7110 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/utils/dpr.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5933 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/utils/metrics.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3287 2024-04-08 17:29:25.000000 dspy-ai-2.4.7/dsp/utils/settings.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2828 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/utils/settings_v2.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5623 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dsp/utils/utils.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/
--rw-r--r--   0 okhattab (19845) future   (20099)      786 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/adapters/
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/adapters/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/adapters/basic_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/adapters/chatml_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/adapters/llamachat_adapter.py
--rw-r--r--   0 okhattab (19845) future   (20099)        0 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/adapters/vicuna_adapter.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/datasets/
--rw-r--r--   0 okhattab (19845) future   (20099)      122 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/datasets/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2986 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/datasets/colors.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4572 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/datasets/dataloader.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4098 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/datasets/dataset.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2618 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/datasets/gsm8k.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3286 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/datasets/hotpotqa.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/evaluate/
--rw-r--r--   0 okhattab (19845) future   (20099)      127 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/evaluate/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1421 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/evaluate/auto_evaluation.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10273 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/evaluate/evaluate.py
--rw-r--r--   0 okhattab (19845) future   (20099)      882 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/evaluate/metrics.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/experimental/
--rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/experimental/__init__.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/
--rw-r--r--   0 okhattab (19845) future   (20099)       26 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)      834 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/config.py
--rw-r--r--   0 okhattab (19845) future   (20099)      527 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/instruction_suffixes.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5543 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/signatures.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9542 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/synthesizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)      599 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/experimental/synthesizer/utils.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3292 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/experimental/synthetic_data.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/functional/
--rw-r--r--   0 okhattab (19845) future   (20099)       94 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/functional/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    15805 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/functional/functional.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/predict/
--rw-r--r--   0 okhattab (19845) future   (20099)      348 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1842 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/aggregation.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3589 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/chain_of_thought.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1527 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/chain_of_thought_with_hint.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1017 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/knn.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6117 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/langchain.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1659 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/multi_chain_comparison.py
--rw-r--r--   0 okhattab (19845) future   (20099)       58 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/parameter.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5276 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/predict/predict.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7397 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/predict/program_of_thought.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4415 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/predict/react.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2515 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/predict/retry.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/primitives/
--rw-r--r--   0 okhattab (19845) future   (20099)      132 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)    11870 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/assertions.py
--rw-r--r--   0 okhattab (19845) future   (20099)     7779 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/box.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3440 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/example.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2647 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/primitives/module.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2807 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/prediction.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3366 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/program.py
--rw-r--r--   0 okhattab (19845) future   (20099)    25710 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/primitives/python_interpreter.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/retrieve/
--rw-r--r--   0 okhattab (19845) future   (20099)       30 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4793 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/chromadb_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3257 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/clarifai_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6489 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/databricks_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3879 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/deeplake_rm.py
--rwxr-xr-x   0 okhattab (19845) future   (20099)     6530 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/faiss_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3459 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/retrieve/marqo_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3774 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/mongodb_atlas_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6213 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/neo4j_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     4211 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/pgvector_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)    10476 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/pinecone_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3246 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/qdrant_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1424 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/retrieve.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5659 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/vectara_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3331 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/retrieve/weaviate_rm.py
--rw-r--r--   0 okhattab (19845) future   (20099)      438 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/weaviate_rm_test.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1678 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/retrieve/you_rm.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/signatures/
--rw-r--r--   0 okhattab (19845) future   (20099)       46 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/signatures/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2758 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/signatures/field.py
--rw-r--r--   0 okhattab (19845) future   (20099)    14169 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/signatures/signature.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/teleprompt/
--rw-r--r--   0 okhattab (19845) future   (20099)      390 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/teleprompt/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     9525 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/bootstrap.py
--rw-r--r--   0 okhattab (19845) future   (20099)    18254 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/copro_optimizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)     1359 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/ensemble.py
--rw-r--r--   0 okhattab (19845) future   (20099)     6292 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/finetune.py
--rw-r--r--   0 okhattab (19845) future   (20099)      879 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/knn_fewshot.py
--rw-r--r--   0 okhattab (19845) future   (20099)    31087 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/mipro_optimizer.py
--rw-r--r--   0 okhattab (19845) future   (20099)     8107 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/random_search.py
--rw-r--r--   0 okhattab (19845) future   (20099)     2673 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/signature_opt.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3878 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/signature_opt_bayesian.py
--rw-r--r--   0 okhattab (19845) future   (20099)    11876 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/signature_opt_typed.py
--rw-r--r--   0 okhattab (19845) future   (20099)       57 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/teleprompt.py
--rw-r--r--   0 okhattab (19845) future   (20099)     3208 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/teleprompt_optuna.py
--rw-r--r--   0 okhattab (19845) future   (20099)      948 2024-04-08 19:45:10.000000 dspy-ai-2.4.7/dspy/teleprompt/vanilla.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy/utils/
--rw-r--r--   0 okhattab (19845) future   (20099)       23 2024-04-08 17:11:57.000000 dspy-ai-2.4.7/dspy/utils/__init__.py
--rw-r--r--   0 okhattab (19845) future   (20099)     5643 2024-04-08 16:37:23.000000 dspy-ai-2.4.7/dspy/utils/dummies.py
-drwxr-sr-x   0 okhattab (19845) future   (20099)        0 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy_ai.egg-info/
--rw-r--r--   0 okhattab (19845) future   (20099)    35318 2024-04-08 20:57:42.000000 dspy-ai-2.4.7/dspy_ai.egg-info/PKG-INFO
--rw-r--r--   0 okhattab (19845) future   (20099)     3752 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/dspy_ai.egg-info/SOURCES.txt
--rw-r--r--   0 okhattab (19845) future   (20099)        1 2024-04-08 20:57:42.000000 dspy-ai-2.4.7/dspy_ai.egg-info/dependency_links.txt
--rw-r--r--   0 okhattab (19845) future   (20099)      635 2024-04-08 20:57:42.000000 dspy-ai-2.4.7/dspy_ai.egg-info/requires.txt
--rw-r--r--   0 okhattab (19845) future   (20099)        9 2024-04-08 20:57:42.000000 dspy-ai-2.4.7/dspy_ai.egg-info/top_level.txt
--rw-r--r--   0 okhattab (19845) future   (20099)     6888 2024-04-08 20:57:27.000000 dspy-ai-2.4.7/pyproject.toml
--rw-r--r--   0 okhattab (19845) future   (20099)       38 2024-04-08 20:57:43.000000 dspy-ai-2.4.7/setup.cfg
--rw-r--r--   0 okhattab (19845) future   (20099)     1495 2024-04-08 20:57:37.000000 dspy-ai-2.4.7/setup.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.829986 dspy-ai-2.4.9/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1085 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/LICENSE
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    36243 2024-04-29 20:58:33.829986 dspy-ai-2.4.9/PKG-INFO
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    35291 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/README.md
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.805975 dspy-ai-2.4.9/dsp/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1532 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/__init__.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.805975 dspy-ai-2.4.9/dsp/evaluation/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        1 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/evaluation/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2586 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/evaluation/utils.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dsp/modules/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      760 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4439 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/anthropic.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    10296 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/aws_models.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4525 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/aws_providers.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     9756 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/azure_openai.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3135 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/azurecognitivesearch.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1018 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/cache_utils.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3008 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/clarifai.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3313 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/cohere.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2156 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/colbertv2.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5278 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/databricks.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3788 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/dummy_lm.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dsp/modules/finetuning/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       26 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/finetuning/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    15071 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/finetuning/finetune_hf.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4552 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/google.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5992 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/googlevertexai.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     8562 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/gpt3.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4859 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/groq_client.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     8119 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/hf.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    17704 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/hf_client.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2087 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/hf_server.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3721 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/lm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3655 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/mistral.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     6751 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/ollama.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3152 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/pyserini.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      693 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/sbert.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     7787 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/modules/sentence_vectorizer.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dsp/primitives/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      145 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5185 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/compiler.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5789 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/demonstrate.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2471 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/inspect.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     8432 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/predict.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1439 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/primitives.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2727 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/primitives/search.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dsp/templates/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       76 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/templates/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    10226 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/templates/template_v2.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2334 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/templates/template_v3.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1900 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/templates/utils.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dsp/utils/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      123 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4903 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/ann_utils.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     7110 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/dpr.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5933 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/metrics.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3215 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/settings.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2828 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/settings_v2.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5623 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dsp/utils/utils.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dspy/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1059 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/__init__.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.813979 dspy-ai-2.4.9/dspy/adapters/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/adapters/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/adapters/basic_adapter.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/adapters/chatml_adapter.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/adapters/llamachat_adapter.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/adapters/vicuna_adapter.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.817980 dspy-ai-2.4.9/dspy/datasets/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      122 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/datasets/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2986 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/datasets/colors.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4949 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/datasets/dataloader.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4098 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/datasets/dataset.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2618 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/datasets/gsm8k.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3286 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/datasets/hotpotqa.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.817980 dspy-ai-2.4.9/dspy/evaluate/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      127 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/evaluate/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1421 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/evaluate/auto_evaluation.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    10081 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/evaluate/evaluate.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      882 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/evaluate/metrics.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.817980 dspy-ai-2.4.9/dspy/experimental/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       57 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/__init__.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.817980 dspy-ai-2.4.9/dspy/experimental/synthesizer/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       26 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthesizer/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      834 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthesizer/config.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      527 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthesizer/instruction_suffixes.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5543 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthesizer/signatures.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     9723 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthesizer/synthesizer.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      599 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthesizer/utils.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4237 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/experimental/synthetic_data.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.817980 dspy-ai-2.4.9/dspy/functional/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       94 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/functional/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    19499 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/functional/functional.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.817980 dspy-ai-2.4.9/dspy/predict/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      348 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1842 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/aggregation.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3589 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/chain_of_thought.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1527 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/chain_of_thought_with_hint.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1017 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/knn.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     6117 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/langchain.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1659 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/multi_chain_comparison.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       58 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/parameter.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5580 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/predict.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     7603 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/program_of_thought.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4458 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/react.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2827 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/predict/retry.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.821982 dspy-ai-2.4.9/dspy/primitives/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      132 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    11407 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/assertions.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     7779 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/box.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3471 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/example.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3831 2024-04-29 20:58:28.000000 dspy-ai-2.4.9/dspy/primitives/module.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2807 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/prediction.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3366 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/program.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    25710 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/primitives/python_interpreter.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.825984 dspy-ai-2.4.9/dspy/retrieve/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       30 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    17405 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/azureaisearch_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5719 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/chromadb_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3275 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/clarifai_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     6604 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/databricks_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3897 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/deeplake_rm.py
+-rwxrwxr-x   0 okhattab  (1000) okhattab  (1000)     6605 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/faiss_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3459 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/marqo_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3998 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/milvus_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3774 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/mongodb_atlas_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     6213 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/neo4j_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5930 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/pgvector_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    10476 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/pinecone_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3271 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/qdrant_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2425 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/ragatouille_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1442 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/retrieve.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5659 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/vectara_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     4491 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/weaviate_rm.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      438 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/weaviate_rm_test.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1678 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/retrieve/you_rm.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.825984 dspy-ai-2.4.9/dspy/signatures/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       46 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/signatures/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2758 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/signatures/field.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    14464 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/signatures/signature.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.825984 dspy-ai-2.4.9/dspy/teleprompt/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      390 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     9532 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/bootstrap.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    17739 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/copro_optimizer.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1359 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/ensemble.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     6292 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/finetune.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      879 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/knn_fewshot.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    31087 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/mipro_optimizer.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     8130 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/random_search.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     2673 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/signature_opt.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3878 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/signature_opt_bayesian.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    11876 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/signature_opt_typed.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       57 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/teleprompt.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3208 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/teleprompt_optuna.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      948 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/teleprompt/vanilla.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.825984 dspy-ai-2.4.9/dspy/utils/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       46 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/utils/__init__.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     5643 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/utils/dummies.py
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3193 2024-04-29 20:37:23.000000 dspy-ai-2.4.9/dspy/utils/logging.py
+drwxrwxr-x   0 okhattab  (1000) okhattab  (1000)        0 2024-04-29 20:58:33.829986 dspy-ai-2.4.9/dspy_ai.egg-info/
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)    36243 2024-04-29 20:58:33.000000 dspy-ai-2.4.9/dspy_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     3981 2024-04-29 20:58:33.000000 dspy-ai-2.4.9/dspy_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        1 2024-04-29 20:58:33.000000 dspy-ai-2.4.9/dspy_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)      766 2024-04-29 20:58:33.000000 dspy-ai-2.4.9/dspy_ai.egg-info/requires.txt
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)        9 2024-04-29 20:58:33.000000 dspy-ai-2.4.9/dspy_ai.egg-info/top_level.txt
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     7322 2024-04-29 20:58:28.000000 dspy-ai-2.4.9/pyproject.toml
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)       38 2024-04-29 20:58:33.829986 dspy-ai-2.4.9/setup.cfg
+-rw-rw-r--   0 okhattab  (1000) okhattab  (1000)     1599 2024-04-29 20:58:28.000000 dspy-ai-2.4.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dspy-ai-2.4.7/LICENSE` & `dspy-ai-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/PKG-INFO` & `dspy-ai-2.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspy-ai
-Version: 2.4.7
+Version: 2.4.9
 Summary: DSPy
 Home-page: https://github.com/stanfordnlp/dsp
 Author: Omar Khattab
 Author-email: Omar Khattab <okhattab@stanford.edu>
 License: MIT License
 Project-URL: homepage, https://github.com/stanfordnlp/dspy
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,18 @@
 Provides-Extra: chromadb
 Provides-Extra: qdrant
 Provides-Extra: marqo
 Provides-Extra: mongodb
 Provides-Extra: pinecone
 Provides-Extra: weaviate
 Provides-Extra: faiss-cpu
+Provides-Extra: milvus
+Provides-Extra: google-vertex-ai
 Provides-Extra: anthropic
+Provides-Extra: aws
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
   <img align="center" src="docs/images/DSPy8.png" width="460px" />
 </p>
@@ -83,26 +86,33 @@
 
 **What does DSPy stand for?** It's a long story but the backronym now is **D**eclarative **S**elf-improving Language **P**rograms, p**y**thonically.
 
 ## 1) Installation
 
 All you need is:
 
-```
+```bash
 pip install dspy-ai
 ```
 
+To install the very latest from `main`:
+
+```bash
+pip install git+https://github.com/stanfordnlp/dspy.git
+````
+
 Or open our intro notebook in Google Colab: [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/github/stanfordnlp/dspy/blob/main/intro.ipynb)
 
 By default, DSPy installs the latest `openai` from pip. However, if you install old version before OpenAI changed their API `openai~=0.28.1`, the library will use that just fine. Both are supported.
 
-For the optional (alphabetically sorted) [Chromadb](https://github.com/chroma-core/chroma), [Qdrant](https://github.com/qdrant/qdrant), [Marqo](https://github.com/marqo-ai/marqo), Pinecone, or [Weaviate](https://github.com/weaviate/weaviate) retrieval integration(s), include the extra(s) below:
+For the optional (alphabetically sorted) [Chromadb](https://github.com/chroma-core/chroma), [Qdrant](https://github.com/qdrant/qdrant), [Marqo](https://github.com/marqo-ai/marqo), Pinecone, [Weaviate](https://github.com/weaviate/weaviate),
+or [Milvus](https://github.com/milvus-io/milvus) retrieval integration(s), include the extra(s) below:
 
 ```
-pip install dspy-ai[chromadb]  # or [qdrant] or [marqo] or [mongodb] or [pinecone] or [weaviate]
+pip install dspy-ai[chromadb]  # or [qdrant] or [marqo] or [mongodb] or [pinecone] or [weaviate] or [milvus]
 ```
 
 ## 2) Documentation
 
 The DSPy documentation is divided into **tutorials** (step-by-step illustration of solving a task in DSPy), **guides** (how to use specific parts of the API), and **examples** (self-contained programs that illustrate usage).
 
 ### A) Tutorials
@@ -119,17 +129,18 @@
 | Advanced | [**Information Extraction**](https://twitter.com/KarelDoostrlnck/status/1724991014207930696) | [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1CpsOiLiLYKeGrhmq579_FmtGsD5uZ3Qe) | Tackles extracting information from long articles (biomedical research papers). Combines in-context learning and retrieval to set SOTA on BioDEX. Contributed by [Karel D’Oosterlinck](https://twitter.com/KarelDoostrlnck/status/1724991014207930696).  |
 
 
 **Other resources people find useful**:
 
 - [DSPy talk at ScaleByTheBay Nov 2023](https://www.youtube.com/watch?v=Dt3H2ninoeY).
 - [DSPy webinar with MLOps Learners](https://www.youtube.com/watch?v=im7bCLW2aM4), a bit longer with Q&A.
-- Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck)
+- Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck), [DSPy Crash Course by AI Bites](https://youtu.be/5-zgASQKkKQ?si=3gnmVouT5_rpk_nu)
 - Interviews: [Weaviate Podcast in-person](https://www.youtube.com/watch?v=CDung1LnLbY), and you can find 6-7 other remote podcasts on YouTube from a few different perspectives/audiences.
 - **Tracing in DSPy** with Arize Phoenix: [Tutorial for tracing your prompts and the steps of your DSPy programs](https://colab.research.google.com/github/Arize-ai/phoenix/blob/main/tutorials/tracing/dspy_tracing_tutorial.ipynb)
+- [DSPy: Not Your Average Prompt Engineering](https://jina.ai/news/dspy-not-your-average-prompt-engineering), why it's crucial for future prompt engineering, and yet why it is challenging for prompt engineers to learn.
 
 ### B) Guides
 
 If you're new to DSPy, it's probably best to go in sequential order. You will probably refer to these guides frequently after that, e.g. to copy/paste snippets that you can edit for your own DSPy programs.
 
 
 1. **[Language Models](https://dspy-docs.vercel.app/docs/building-blocks/language_models)**
@@ -165,18 +176,21 @@
 - [AI feedback, or writing LM-based metrics in DSPy](https://github.com/stanfordnlp/dspy/blob/main/examples/tweets/tweet_metric.py)
 - [DSPy Optimizers Benchmark on a bunch of different tasks, by Michael Ryan](https://github.com/stanfordnlp/dspy/tree/main/testing/tasks)
 - [Indian Languages NLI with gains due to compiling by Saiful Haq](https://github.com/saifulhaq95/DSPy-Indic/blob/main/indicxlni.ipynb)
 - [Sophisticated Extreme Multi-Class Classification, IReRa, by Karel D’Oosterlinck](https://github.com/KarelDO/xmc.dspy)
 - [DSPy on BIG-Bench Hard Example, by Chris Levy](https://drchrislevy.github.io/posts/dspy/dspy.html)
 - [Using Ollama with DSPy for Mistral (quantized) by @jrknox1977](https://gist.github.com/jrknox1977/78c17e492b5a75ee5bbaf9673aee4641)
 - [Using DSPy, "The Unreasonable Effectiveness of Eccentric Automatic Prompts" (paper) by VMware's Rick Battle & Teja Gollapudi, and interview at TheRegister](https://www.theregister.com/2024/02/22/prompt_engineering_ai_models/)
+- [Optimizing Performance of Open Source LM for Text-to-SQL using DSPy and vLLM, by Juan Ovalle](https://github.com/jjovalle99/DSPy-Text2SQL)
 - Typed DSPy (contributed by [@normal-computing](https://github.com/normal-computing))
   - [Using DSPy to train Gpt 3.5 on HumanEval by Thomas Ahle](https://github.com/stanfordnlp/dspy/blob/main/examples/functional/functional.ipynb)
   - [Building a chess playing agent using DSPy by Franck SN](https://medium.com/thoughts-on-machine-learning/building-a-chess-playing-agent-using-dspy-9b87c868f71e)
 
+TODO: Add links to the state-of-the-art results on Theory of Mind (ToM) by Plastic Labs, the results by Haize Labs for Red Teaming with DSPy, and the DSPy pipeline from Replit.
+
 There are also recent cool examples at [Weaviate's DSPy cookbook](https://github.com/weaviate/recipes/tree/main/integrations/dspy) by Connor Shorten. [See tutorial on YouTube](https://www.youtube.com/watch?v=CEuUG4Umfxs).
 
 ## 3) Syntax: You're in charge of the workflow—it's free-form Python code!
 
 **DSPy** hides tedious prompt engineering, but it cleanly exposes the important decisions you need to make: **[1]** what's your system design going to look like? **[2]** what are the important constraints on the behavior of your program?
 
 You express your system as free-form Pythonic modules. **DSPy** will tune the quality of your program _in whatever way_ you use foundation models: you can code with loops, `if` statements, or exceptions, and use **DSPy** modules within any Python control flow you think works for your task.
@@ -435,15 +449,15 @@
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) for a quickstart guide to contributing to DSPy.
 
 ## Contributors & Acknowledgements
 
 **DSPy** is led by **Omar Khattab** at Stanford NLP with **Chris Potts** and **Matei Zaharia**.
 
-Key contributors and team members include **Arnav Singhvi**, **Krista Opsahl-Ong**, **Michael Ryan**, **Karel D'Oosterlinck**, **Shangyin Tan**, **Manish Shetty**, **Paridhi Maheshwari**, **Keshav Santhanam**, **Sri Vardhamanan**, **Eric Zhang**, **Hanna Moazam**, **Thomas Joshi**, **Saiful Haq**, **Ashutosh Sharma**, and **Herumb Shandilya**.
+Key contributors and team members include **Arnav Singhvi**, **Krista Opsahl-Ong**, **Michael Ryan**, **Cyrus Nouroozi**, **Kyle Caverly**, **Amir Mehr**, **Karel D'Oosterlinck**, **Shangyin Tan**, **Manish Shetty**, **Herumb Shandilya**, **Paridhi Maheshwari**, **Keshav Santhanam**, **Sri Vardhamanan**, **Eric Zhang**, **Hanna Moazam**, **Thomas Joshi**, **Saiful Haq**, and **Ashutosh Sharma**.
 
 **DSPy** includes important contributions from **Rick Battle** and **Igor Kotenkov**. It reflects discussions with **Peter Zhong**, **Haoze He**, **Lisa Li**, **David Hall**, **Ashwin Paranjape**, **Heather Miller**, **Chris Manning**, **Percy Liang**, and many others.
 
 The **DSPy** logo is designed by **Chuyi Zhang**.
 
 
 ## 📜 Citation & Reading More
```

### Comparing `dspy-ai-2.4.7/README.md` & `dspy-ai-2.4.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,26 +54,33 @@
 
 **What does DSPy stand for?** It's a long story but the backronym now is **D**eclarative **S**elf-improving Language **P**rograms, p**y**thonically.
 
 ## 1) Installation
 
 All you need is:
 
-```
+```bash
 pip install dspy-ai
 ```
 
+To install the very latest from `main`:
+
+```bash
+pip install git+https://github.com/stanfordnlp/dspy.git
+````
+
 Or open our intro notebook in Google Colab: [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/github/stanfordnlp/dspy/blob/main/intro.ipynb)
 
 By default, DSPy installs the latest `openai` from pip. However, if you install old version before OpenAI changed their API `openai~=0.28.1`, the library will use that just fine. Both are supported.
 
-For the optional (alphabetically sorted) [Chromadb](https://github.com/chroma-core/chroma), [Qdrant](https://github.com/qdrant/qdrant), [Marqo](https://github.com/marqo-ai/marqo), Pinecone, or [Weaviate](https://github.com/weaviate/weaviate) retrieval integration(s), include the extra(s) below:
+For the optional (alphabetically sorted) [Chromadb](https://github.com/chroma-core/chroma), [Qdrant](https://github.com/qdrant/qdrant), [Marqo](https://github.com/marqo-ai/marqo), Pinecone, [Weaviate](https://github.com/weaviate/weaviate),
+or [Milvus](https://github.com/milvus-io/milvus) retrieval integration(s), include the extra(s) below:
 
 ```
-pip install dspy-ai[chromadb]  # or [qdrant] or [marqo] or [mongodb] or [pinecone] or [weaviate]
+pip install dspy-ai[chromadb]  # or [qdrant] or [marqo] or [mongodb] or [pinecone] or [weaviate] or [milvus]
 ```
 
 ## 2) Documentation
 
 The DSPy documentation is divided into **tutorials** (step-by-step illustration of solving a task in DSPy), **guides** (how to use specific parts of the API), and **examples** (self-contained programs that illustrate usage).
 
 ### A) Tutorials
@@ -90,17 +97,18 @@
 | Advanced | [**Information Extraction**](https://twitter.com/KarelDoostrlnck/status/1724991014207930696) | [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1CpsOiLiLYKeGrhmq579_FmtGsD5uZ3Qe) | Tackles extracting information from long articles (biomedical research papers). Combines in-context learning and retrieval to set SOTA on BioDEX. Contributed by [Karel D’Oosterlinck](https://twitter.com/KarelDoostrlnck/status/1724991014207930696).  |
 
 
 **Other resources people find useful**:
 
 - [DSPy talk at ScaleByTheBay Nov 2023](https://www.youtube.com/watch?v=Dt3H2ninoeY).
 - [DSPy webinar with MLOps Learners](https://www.youtube.com/watch?v=im7bCLW2aM4), a bit longer with Q&A.
-- Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck)
+- Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck), [DSPy Crash Course by AI Bites](https://youtu.be/5-zgASQKkKQ?si=3gnmVouT5_rpk_nu)
 - Interviews: [Weaviate Podcast in-person](https://www.youtube.com/watch?v=CDung1LnLbY), and you can find 6-7 other remote podcasts on YouTube from a few different perspectives/audiences.
 - **Tracing in DSPy** with Arize Phoenix: [Tutorial for tracing your prompts and the steps of your DSPy programs](https://colab.research.google.com/github/Arize-ai/phoenix/blob/main/tutorials/tracing/dspy_tracing_tutorial.ipynb)
+- [DSPy: Not Your Average Prompt Engineering](https://jina.ai/news/dspy-not-your-average-prompt-engineering), why it's crucial for future prompt engineering, and yet why it is challenging for prompt engineers to learn.
 
 ### B) Guides
 
 If you're new to DSPy, it's probably best to go in sequential order. You will probably refer to these guides frequently after that, e.g. to copy/paste snippets that you can edit for your own DSPy programs.
 
 
 1. **[Language Models](https://dspy-docs.vercel.app/docs/building-blocks/language_models)**
@@ -136,18 +144,21 @@
 - [AI feedback, or writing LM-based metrics in DSPy](https://github.com/stanfordnlp/dspy/blob/main/examples/tweets/tweet_metric.py)
 - [DSPy Optimizers Benchmark on a bunch of different tasks, by Michael Ryan](https://github.com/stanfordnlp/dspy/tree/main/testing/tasks)
 - [Indian Languages NLI with gains due to compiling by Saiful Haq](https://github.com/saifulhaq95/DSPy-Indic/blob/main/indicxlni.ipynb)
 - [Sophisticated Extreme Multi-Class Classification, IReRa, by Karel D’Oosterlinck](https://github.com/KarelDO/xmc.dspy)
 - [DSPy on BIG-Bench Hard Example, by Chris Levy](https://drchrislevy.github.io/posts/dspy/dspy.html)
 - [Using Ollama with DSPy for Mistral (quantized) by @jrknox1977](https://gist.github.com/jrknox1977/78c17e492b5a75ee5bbaf9673aee4641)
 - [Using DSPy, "The Unreasonable Effectiveness of Eccentric Automatic Prompts" (paper) by VMware's Rick Battle & Teja Gollapudi, and interview at TheRegister](https://www.theregister.com/2024/02/22/prompt_engineering_ai_models/)
+- [Optimizing Performance of Open Source LM for Text-to-SQL using DSPy and vLLM, by Juan Ovalle](https://github.com/jjovalle99/DSPy-Text2SQL)
 - Typed DSPy (contributed by [@normal-computing](https://github.com/normal-computing))
   - [Using DSPy to train Gpt 3.5 on HumanEval by Thomas Ahle](https://github.com/stanfordnlp/dspy/blob/main/examples/functional/functional.ipynb)
   - [Building a chess playing agent using DSPy by Franck SN](https://medium.com/thoughts-on-machine-learning/building-a-chess-playing-agent-using-dspy-9b87c868f71e)
 
+TODO: Add links to the state-of-the-art results on Theory of Mind (ToM) by Plastic Labs, the results by Haize Labs for Red Teaming with DSPy, and the DSPy pipeline from Replit.
+
 There are also recent cool examples at [Weaviate's DSPy cookbook](https://github.com/weaviate/recipes/tree/main/integrations/dspy) by Connor Shorten. [See tutorial on YouTube](https://www.youtube.com/watch?v=CEuUG4Umfxs).
 
 ## 3) Syntax: You're in charge of the workflow—it's free-form Python code!
 
 **DSPy** hides tedious prompt engineering, but it cleanly exposes the important decisions you need to make: **[1]** what's your system design going to look like? **[2]** what are the important constraints on the behavior of your program?
 
 You express your system as free-form Pythonic modules. **DSPy** will tune the quality of your program _in whatever way_ you use foundation models: you can code with loops, `if` statements, or exceptions, and use **DSPy** modules within any Python control flow you think works for your task.
@@ -406,15 +417,15 @@
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) for a quickstart guide to contributing to DSPy.
 
 ## Contributors & Acknowledgements
 
 **DSPy** is led by **Omar Khattab** at Stanford NLP with **Chris Potts** and **Matei Zaharia**.
 
-Key contributors and team members include **Arnav Singhvi**, **Krista Opsahl-Ong**, **Michael Ryan**, **Karel D'Oosterlinck**, **Shangyin Tan**, **Manish Shetty**, **Paridhi Maheshwari**, **Keshav Santhanam**, **Sri Vardhamanan**, **Eric Zhang**, **Hanna Moazam**, **Thomas Joshi**, **Saiful Haq**, **Ashutosh Sharma**, and **Herumb Shandilya**.
+Key contributors and team members include **Arnav Singhvi**, **Krista Opsahl-Ong**, **Michael Ryan**, **Cyrus Nouroozi**, **Kyle Caverly**, **Amir Mehr**, **Karel D'Oosterlinck**, **Shangyin Tan**, **Manish Shetty**, **Herumb Shandilya**, **Paridhi Maheshwari**, **Keshav Santhanam**, **Sri Vardhamanan**, **Eric Zhang**, **Hanna Moazam**, **Thomas Joshi**, **Saiful Haq**, and **Ashutosh Sharma**.
 
 **DSPy** includes important contributions from **Rick Battle** and **Igor Kotenkov**. It reflects discussions with **Peter Zhong**, **Haoze He**, **Lisa Li**, **David Hall**, **Ashwin Paranjape**, **Heather Miller**, **Chris Manning**, **Percy Liang**, and many others.
 
 The **DSPy** logo is designed by **Chuyi Zhang**.
 
 
 ## 📜 Citation & Reading More
```

### Comparing `dspy-ai-2.4.7/dsp/__init__.py` & `dspy-ai-2.4.9/dsp/__init__.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/evaluation/utils.py` & `dspy-ai-2.4.9/dsp/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/modules/anthropic.py` & `dspy-ai-2.4.9/dsp/modules/anthropic.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 
 import backoff
 
 from dsp.modules.lm import LM
 
 try:
     import anthropic
+
     anthropic_rate_limit = anthropic.RateLimitError
 except ImportError:
     anthropic_rate_limit = Exception
 
-
 logger = logging.getLogger(__name__)
-
 BASE_URL = "https://api.anthropic.com/v1/messages"
 
 
 def backoff_hdlr(details):
     """Handler from https://pypi.org/project/backoff/."""
     print(
         "Backing off {wait:0.1f} seconds after {tries} tries "
@@ -32,32 +31,31 @@
     if "rate limits" in details.message:
         return False
     return True
 
 
 class Claude(LM):
     """Wrapper around anthropic's API. Supports both the Anthropic and Azure APIs."""
+
     def __init__(
-            self,
-            model: str = "claude-instant-1.2",
-            api_key: Optional[str] = None,
-            api_base: Optional[str] = None,
-            **kwargs,
+        self,
+        model: str = "claude-3-opus-20240229",
+        api_key: Optional[str] = None,
+        api_base: Optional[str] = None,
+        **kwargs,
     ):
         super().__init__(model)
-
         try:
             from anthropic import Anthropic
         except ImportError as err:
             raise ImportError("Claude requires `pip install anthropic`.") from err
 
         self.provider = "anthropic"
         self.api_key = api_key = os.environ.get("ANTHROPIC_API_KEY") if api_key is None else api_key
         self.api_base = BASE_URL if api_base is None else api_base
-
         self.kwargs = {
             "temperature": kwargs.get("temperature", 0.0),
             "max_tokens": min(kwargs.get("max_tokens", 4096), 4096),
             "top_p": kwargs.get("top_p", 1.0),
             "top_k": kwargs.get("top_k", 1),
             "n": kwargs.pop("n", kwargs.pop("num_generations", 1)),
             **kwargs,
@@ -67,33 +65,30 @@
         self.client = Anthropic(api_key=api_key)
 
     def log_usage(self, response):
         """Log the total tokens from the Anthropic API response."""
         usage_data = response.usage
         if usage_data:
             total_tokens = usage_data.input_tokens + usage_data.output_tokens
-            logger.info(f'{total_tokens}')
+            logger.debug(f"Anthropic Total Token Response Usage: {total_tokens}")
 
     def basic_request(self, prompt: str, **kwargs):
         raw_kwargs = kwargs
-
         kwargs = {**self.kwargs, **kwargs}
         # caching mechanism requires hashable kwargs
         kwargs["messages"] = [{"role": "user", "content": prompt}]
         kwargs.pop("n")
         response = self.client.messages.create(**kwargs)
-
         history = {
             "prompt": prompt,
             "response": response,
             "kwargs": kwargs,
             "raw_kwargs": raw_kwargs,
         }
         self.history.append(history)
-
         return response
 
     @backoff.on_exception(
         backoff.expo,
         (anthropic_rate_limit),
         max_time=1000,
         max_tries=8,
@@ -111,27 +106,21 @@
             prompt (str): prompt to send to Anthropic
             only_completed (bool, optional): return only completed responses and ignores completion due to length. Defaults to True.
             return_sorted (bool, optional): sort the completion choices using the returned probabilities. Defaults to False.
 
         Returns:
             list[str]: list of completion choices
         """
-
         assert only_completed, "for now"
         assert return_sorted is False, "for now"
-
-
         # per eg here: https://docs.anthropic.com/claude/reference/messages-examples
         # max tokens can be used as a proxy to return smaller responses
         # so this cannot be a proper indicator for incomplete response unless it isnt the user-intent.
-
         n = kwargs.pop("n", 1)
         completions = []
         for _ in range(n):
             response = self.request(prompt, **kwargs)
-            # TODO: Log llm usage instead of hardcoded openai usage
-            # if dsp.settings.log_openai_usage:
-            #     self.log_usage(response)
+            self.log_usage(response)
             if only_completed and response.stop_reason == "max_tokens":
                 continue
             completions = [c.text for c in response.content]
         return completions
```

### Comparing `dspy-ai-2.4.7/dsp/modules/aws_lm.py` & `dspy-ai-2.4.9/dsp/modules/googlevertexai.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,180 +1,177 @@
-"""
-A generalized AWS LLM.
-"""
-
-from __future__ import annotations
-
-import json
-import logging
-from abc import abstractmethod
-from typing import Any, Literal
+"""Module for interacting with Google Vertex AI."""
+from typing import Any, Dict
+
+import backoff
+from pydantic_core import PydanticCustomError
 
 from dsp.modules.lm import LM
 
-# Heuristic translating number of chars to tokens
-# ~4 chars = 1 token
-CHARS2TOKENS: int = 4
+try:
+    import vertexai  # type: ignore[import-untyped]
+    from vertexai.language_models import CodeGenerationModel, TextGenerationModel
+    from vertexai.preview.generative_models import GenerativeModel
+except ImportError:
+    pass
+
+
+def backoff_hdlr(details):
+    """Handler from https://pypi.org/project/backoff/"""
+    print(f"Backing off {details['wait']:0.1f} seconds after {details['tries']} tries "
+          f"calling function {details['target']} with kwargs "
+          f"{details['kwargs']}")
+
+
+def giveup_hdlr(details):
+    """wrapper function that decides when to give up on retry"""
+    if "rate limits" in details.message:
+        return False
+    return True
 
+class GoogleVertexAI(LM):
+    """Wrapper around GoogleVertexAI's API.
 
-class AWSLM(LM):
-    """
-    This class adds support for an AWS model
+    Currently supported models include `gemini-pro-1.0`.
     """
 
     def __init__(
-        self,
-        model: str,
-        region_name: str,
-        service_name: str,
-        max_new_tokens: int,
-        truncate_long_prompts: bool = False,
-        input_output_ratio: int = 3,
-        batch_n: bool = True,
-    ) -> None:
-        """_summary_
-
-        Args:
-
-            service_name (str): Used in context of invoking the boto3 API.
-            region_name (str, optional): The AWS region where this LM is hosted.
-            model (str, optional): An LM name, e.g., a bedrock name or an AWS endpoint.
-            max_new_tokens (int, optional): The maximum number of tokens to be sampled from the LM.
-            input_output_ratio (int, optional): The rough size of the number of input tokens to output tokens in the worst case. Defaults to 3.
-            temperature (float, optional): _description_. Defaults to 0.0.
-            truncate_long_prompts (bool, optional): If True, remove extremely long inputs to context. Defaults to False.
-            batch_n (bool, False): If False, call the LM N times rather than batching. Not all AWS models support the n parameter.
+        self, model: str = "text-bison@002", **kwargs,
+    ):
         """
-        super().__init__(model=model)
-        # AWS doesn't have an equivalent of max_tokens so let's clarify
-        # that the expected input is going to be about 2x as long as the output
-        self.kwargs["max_tokens"] = max_new_tokens * input_output_ratio
-        self._max_new_tokens: int = max_new_tokens
-        self._model_name: str = model
-        self._truncate_long_prompt_prompts: bool = truncate_long_prompts
-        self._batch_n: bool = batch_n
-
-        import boto3
-
-        self.predictor = boto3.client(service_name, region_name=region_name)
-
-    @abstractmethod
-    def _create_body(self, prompt: str, **kwargs):
-        pass
-
-    def _sanitize_kwargs(self, query_kwargs: dict[str, Any]) -> dict[str, Any]:
-        """Ensure that input kwargs can be used by Bedrock or Sagemaker."""
-        base_args: dict[str, Any] = {"temperature": self.kwargs["temperature"]}
-
-        for k, v in base_args.items():
-            if k not in query_kwargs:
-                query_kwargs[k] = v
-        if query_kwargs["temperature"] > 1.0:
-            query_kwargs["temperature"] = 0.99
-        if query_kwargs["temperature"] < 0.01:
-            query_kwargs["temperature"] = 0.01
-
-        return query_kwargs
-
-    @abstractmethod
-    def _call_model(self, body: str) -> str | list[str]:
-        """Call model, get generated input without the formatted prompt"""
-        pass
-
-    @abstractmethod
-    def _extract_input_parameters(
-        self, body: dict[Any, Any],
-    ) -> dict[str, str | float | int]:
-        pass
-
-    def _simple_api_call(self, formatted_prompt: str, **kwargs) -> str | list[str]:
-        body = self._create_body(formatted_prompt, **kwargs)
-        json_body = json.dumps(body)
-        llm_out: str | list[str] = self._call_model(json_body)
-        if isinstance(llm_out, str):
-            llm_out = llm_out.replace(formatted_prompt, "")
-        else:
-            llm_out = [generated.replace(formatted_prompt, "") for generated in llm_out]
-        self.history.append(
-            {"prompt": formatted_prompt, "response": llm_out, "kwargs": body},
-        )
-        return llm_out
-
-    def basic_request(self, prompt, **kwargs) -> str | list[str]:
-        """Query the endpoint."""
-
-        # Remove any texts that are too long
-        formatted_prompt: str
-        if self._truncate_long_prompt_prompts:
-            truncated_prompt: str = self._truncate_prompt(prompt)
-            formatted_prompt = self._format_prompt(truncated_prompt)
+        Parameters
+        ----------
+        model : str
+            Which pre-trained model from Google to use?
+            Choices are ['gemini-1.0-pro-001', 'gemini-1.0-pro',
+            'claude-3-sonnet@20240229', 'claude-3-sonnet@20240229', 'claude-3-haiku@20240307',
+            'text-bison@002', 'text-bison-32k@002', 'text-bison',]
+            full list at https://console.cloud.google.com/vertex-ai/model-garden
+        **kwargs: dict
+            Additional arguments to pass to the API provider.
+        """
+        super().__init__(model)
+        self._is_gemini = "gemini" in model
+        self._init_vertexai(kwargs)
+        if "code" in model:
+            model_cls = CodeGenerationModel
+            self.available_args = {
+                'suffix',
+                'max_output_tokens',
+                'temperature',
+                'stop_sequences',
+                'candidate_count',
+            }
+        elif "gemini" in model:
+            model_cls = GenerativeModel
+            self.available_args = {
+                'max_output_tokens',
+                'temperature',
+                'top_k',
+                'top_p',
+                'stop_sequences',
+                'candidate_count',
+            }
+        elif 'text' in model:
+            model_cls = TextGenerationModel
+            self.available_args = {
+                'max_output_tokens',
+                'temperature',
+                'top_k',
+                'top_p',
+                'stop_sequences',
+                'candidate_count',
+            }
         else:
-            formatted_prompt = self._format_prompt(prompt)
-
-        llm_out: str | list[str]
-        if "n" in kwargs.keys():
-            if self._batch_n:
-                llm_out = self._simple_api_call(
-                    formatted_prompt=formatted_prompt, **kwargs,
-                )
-            else:
-                del kwargs["n"]
-                llm_out = []
-                for _ in range(0, kwargs["n"]):
-                    generated: str | list[str] = self._simple_api_call(
-                        formatted_prompt=formatted_prompt, **kwargs,
-                    )
-                    if isinstance(generated, str):
-                        llm_out.append(generated)
-                    else:
-                        raise TypeError("Error, list type was returned from LM call")
+            raise PydanticCustomError(
+                'model',
+                'model name is not valid, got "{model_name}"',
+                dict(wrong_value=model),
+            )
+        if self._is_gemini:
+            self.client = model_cls(model_name=model, safety_settings=kwargs.get('safety_settings')) # pylint: disable=unexpected-keyword-arg,no-value-for-parameter
         else:
-            llm_out = self._simple_api_call(formatted_prompt=formatted_prompt, **kwargs)
-
-        return llm_out
-
-    def _estimate_tokens(self, text: str) -> int:
-        return len(text) * CHARS2TOKENS
-
-    @abstractmethod
-    def _format_prompt(self, raw_prompt: str) -> str:
-        pass
+            self.client = model_cls.from_pretrained(model)
+        self.provider = "googlevertexai"
+        self.kwargs = {
+            **self.kwargs,
+            "temperature": 0.7,
+            "max_output_tokens": 1024,
+            "top_p": 1.0,
+            "top_k": 1,
+            **kwargs,
+        }
+
+    @classmethod
+    def _init_vertexai(cls, values: Dict) -> None:
+        vertexai.init(
+            project=values.get("project"),
+            location=values.get("location"),
+            credentials=values.get("credentials"),
+        )
+        return
 
-    def _truncate_prompt(
+    def _prepare_params(
         self,
-        input_text: str,
-        remove_beginning_or_ending: Literal["beginning", "ending"] = "beginning",
-        max_input_tokens: int = 2500,
-    ) -> str:
-        """Reformat inputs such that they do not overflow context size limitation."""
-        token_count = self._estimate_tokens(input_text)
-        if token_count > self.kwargs["max_tokens"]:
-            logging.info("Excessive prompt found in llm input")
-            logging.info("Truncating texts to avoid error")
-            max_chars: int = CHARS2TOKENS * max_input_tokens
-            truncated_text: str
-            if remove_beginning_or_ending == "ending":
-                truncated_text = input_text[0:max_chars]
-            else:
-                truncated_text = input_text[-max_chars:]
-                return truncated_text
-        return input_text
+        parameters: Any,
+    ) -> dict:
+        stop_sequences = parameters.get('stop')
+        params_mapping = {"n": "candidate_count", 'max_tokens':'max_output_tokens'}
+        params = {params_mapping.get(k, k): v for k, v in parameters.items()}
+        params = {**self.kwargs, "stop_sequences": stop_sequences, **params}
+        return {k: params[k] for k in set(params.keys()) & self.available_args}
+
+    def basic_request(self, prompt: str, **kwargs):
+        raw_kwargs = kwargs
+        kwargs = self._prepare_params(raw_kwargs)
+        if self._is_gemini:
+            response = self.client.generate_content(
+                [prompt],
+                generation_config=kwargs,
+            )
+            history = {
+                "prompt": prompt,
+                "response": {
+                    "prompt": prompt,
+                    "choices": [{
+                        "text": '\n'.join(v.text for v in c.content.parts),
+                        'safetyAttributes': {v.category: v.probability for v in c.safety_ratings},
+                        }
+                        for c in response.candidates],
+                },
+                "kwargs": kwargs,
+                "raw_kwargs": raw_kwargs,
+            }
+        else:
+            response = self.client.predict(prompt, **kwargs).raw_prediction_response
+            history = {
+                "prompt": prompt,
+                "response": {
+                    "prompt": prompt,
+                    "choices": [{"text": c["content"], 'safetyAttributes': c['safetyAttributes']}
+                                for c in response.predictions],
+                },
+                "kwargs": kwargs,
+                "raw_kwargs": raw_kwargs,
+            }
+        self.history.append(history)
+
+        return [i['text'] for i in history['response']['choices']]
+
+    @backoff.on_exception(
+        backoff.expo,
+        (Exception),
+        max_time=1000,
+        on_backoff=backoff_hdlr,
+        giveup=giveup_hdlr,
+    )
+    def request(self, prompt: str, **kwargs):
+        """Handles retrieval of completions from Google whilst handling API errors"""
+        return self.basic_request(prompt, **kwargs)
 
     def __call__(
         self,
         prompt: str,
         only_completed: bool = True,
         return_sorted: bool = False,
         **kwargs,
-    ) -> list[str]:
-        """
-        Query the AWS LLM.
-
-        There is only support for only_completed=True and return_sorted=False
-        right now.
-        """
-        if not only_completed:
-            raise NotImplementedError("Error, only_completed not yet supported!")
-        if return_sorted:
-            raise NotImplementedError("Error, return_sorted not yet supported!")
-        generated = self.basic_request(prompt, **kwargs)
-        return [generated]
+    ):
+        return self.request(prompt, **kwargs)
```

### Comparing `dspy-ai-2.4.7/dsp/modules/azure_openai.py` & `dspy-ai-2.4.9/dsp/modules/azure_openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,15 @@
-import logging
-
-# Configure logging
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(message)s",
-    handlers=[logging.FileHandler("azure_openai_usage.log")],
-)
-
 import functools
 import json
+import logging
 from typing import Any, Literal, Optional, cast
 
 import backoff
 import openai
 
-import dsp
 from dsp.modules.cache_utils import CacheMemory, NotebookCacheMemory, cache_turn_on
 from dsp.modules.lm import LM
 
 try:
     OPENAI_LEGACY = int(openai.version.__version__[0]) == 0
 except Exception:
     OPENAI_LEGACY = True
@@ -48,32 +39,35 @@
 
 class AzureOpenAI(LM):
     """Wrapper around Azure's API for OpenAI.
 
     Args:
         api_base (str): Azure URL endpoint for model calling, often called 'azure_endpoint'.
         api_version (str): Version identifier for API.
-        model (str, optional): OpenAI or Azure supported LLM model to use. Defaults to "text-davinci-002".
+        model (str, optional): OpenAI or Azure supported LLM model to use. Defaults to "gpt-3.5-turbo-instruct".
         api_key (Optional[str], optional): API provider Authentication token. use Defaults to None.
         model_type (Literal["chat", "text"], optional): The type of model that was specified. Mainly to decide the optimal prompting strategy. Defaults to "chat".
         **kwargs: Additional arguments to pass to the API provider.
     """
 
     def __init__(
         self,
         api_base: str,
         api_version: str,
         model: str = "gpt-3.5-turbo-instruct",
         api_key: Optional[str] = None,
         model_type: Literal["chat", "text"] = "chat",
+        system_prompt: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(model)
         self.provider = "openai"
 
+        self.system_prompt = system_prompt
+
         # Define Client
         if OPENAI_LEGACY:
             # Assert that all variables are available
             assert (
                 "engine" in kwargs or "deployment_id" in kwargs
             ), "Must specify engine or deployment_id for Azure API instead of model."
 
@@ -112,36 +106,44 @@
             "top_p": 1,
             "frequency_penalty": 0,
             "presence_penalty": 0,
             "n": 1,
             **kwargs,
         }  # TODO: add kwargs above for </s>
 
+        self.api_base = api_base
+        self.api_version = api_version
+        self.api_key = api_key
+
         self.history: list[dict[str, Any]] = []
 
     def _openai_client(self):
         if OPENAI_LEGACY:
             return openai
 
         return self.client
 
     def log_usage(self, response):
         """Log the total tokens from the Azure OpenAI API response."""
         usage_data = response.get("usage")
         if usage_data:
             total_tokens = usage_data.get("total_tokens")
-            logging.info(f"{total_tokens}")
+            logging.debug(f"Azure OpenAI Total Token Usage: {total_tokens}")
 
     def basic_request(self, prompt: str, **kwargs):
         raw_kwargs = kwargs
 
         kwargs = {**self.kwargs, **kwargs}
         if self.model_type == "chat":
             # caching mechanism requires hashable kwargs
-            kwargs["messages"] = [{"role": "user", "content": prompt}]
+            messages = [{"role": "user", "content": prompt}]
+            if self.system_prompt:
+                messages.insert(0, {"role": "system", "content": self.system_prompt})
+
+            kwargs["messages"] = messages
             kwargs = {"stringify_request": json.dumps(kwargs)}
             response = chat_request(self.client, **kwargs)
 
         else:
             kwargs["prompt"] = prompt
             response = completions_request(self.client, **kwargs)
 
@@ -192,16 +194,15 @@
         """
 
         assert only_completed, "for now"
         assert return_sorted is False, "for now"
 
         response = self.request(prompt, **kwargs)
 
-        if dsp.settings.log_openai_usage:
-            self.log_usage(response)
+        self.log_usage(response)
 
         choices = response["choices"]
 
         completed_choices = [c for c in choices if c["finish_reason"] != "length"]
 
         if only_completed and len(completed_choices):
             choices = completed_choices
@@ -224,14 +225,27 @@
                 scored_completions.append((avglog, self._get_choice_text(c)))
 
             scored_completions = sorted(scored_completions, reverse=True)
             completions = [c for _, c in scored_completions]
 
         return completions
 
+    def copy(self, **kwargs):
+        """Returns a copy of the language model with the same parameters."""
+        kwargs = {**self.kwargs, **kwargs}
+        model = kwargs.pop("model")
+
+        return self.__class__(
+            model=model,
+            api_key=self.api_key,
+            api_version=self.api_version,
+            api_base=self.api_base,
+            **kwargs,
+        )
+
 
 @CacheMemory.cache
 def cached_gpt3_request_v2(**kwargs):
     return openai.Completion.create(**kwargs)
 
 
 @functools.lru_cache(maxsize=None if cache_turn_on else 0)
```

### Comparing `dspy-ai-2.4.7/dsp/modules/azurecognitivesearch.py` & `dspy-ai-2.4.9/dsp/modules/azurecognitivesearch.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,18 @@
     from azure.search.documents._paging import SearchItemPaged
 except ImportError:
     raise ImportError(
         "You need to install azure-search-documents library"
         "Please use the command: pip install azure-search-documents",
     )
 
+# Deprecated: This module is scheduled for removal in future releases.
+# Please use the AzureAISearchRM class from dspy.retrieve.azureaisearch_rm instead.
+# For more information, refer to the updated documentation.
+
 class AzureCognitiveSearch:
     """Wrapper for the Azure Cognitive Search Retrieval."""
 
     def __init__(
         self,
         search_service_name: str,
         search_api_key: str,
@@ -33,17 +37,20 @@
         # Create a client
         self.credential = AzureKeyCredential(self.search_api_key)
         self.client = SearchClient(endpoint=self.endpoint,
                         index_name=self.search_index_name,
                         credential=self.credential)
 
     def __call__(self, query: str, k: int = 10) -> Union[list[str], list[dotdict]]:
-        
+        print("""# Deprecated: This module is scheduled for removal in future releases.
+                Please use the AzureAISearchRM class from dspy.retrieve.azureaisearch_rm instead.
+                For more information, refer to the updated documentation.""")
+
         topk: list[dict[str, Any]] = azure_search_request(self.field_text, self.field_score, self.client, query, k)
-        topk = [{**d, "long_text": d["text"]} for d in topk]            
+        topk = [{**d, "long_text": d["text"]} for d in topk]
 
         return [dotdict(psg) for psg in topk]
 
 def azure_search_request(key_content: str, key_score: str,  client: SearchClient, query: str, top: int =1):
     '''
     Search in Azure Cognitive Search Index
     '''
@@ -61,10 +68,10 @@
         tmp = {}
         for key, value in result.items():
             if(key == content_key):
                 tmp["text"] = value # assign content
             elif(key == content_score):
                 tmp["score"] = value
             else:
-                tmp[key] = value            
+                tmp[key] = value
         res.append(tmp)
-    return res 
+    return res
```

### Comparing `dspy-ai-2.4.7/dsp/modules/cache_utils.py` & `dspy-ai-2.4.9/dsp/modules/cache_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import wraps
 from pathlib import Path
 
 from joblib import Memory
 
 from dsp.utils import dotdict
 
-cache_turn_on = True
+cache_turn_on = os.environ.get('DSP_CACHEBOOL', 'True').lower() != 'false'
 
 
 def noop_decorator(arg=None, *noop_args, **noop_kwargs):
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
```

### Comparing `dspy-ai-2.4.7/dsp/modules/clarifai.py` & `dspy-ai-2.4.9/dsp/modules/clarifai.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/modules/cohere.py` & `dspy-ai-2.4.9/dsp/modules/groq_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,145 +1,158 @@
-import math
-from typing import Any, Optional
+import logging
+from typing import Any
 
 import backoff
 
-from dsp.modules.lm import LM
-
 try:
-    import cohere
-    cohere_api_error = cohere.CohereAPIError
+    import groq
+    from groq import Groq
+
+    groq_api_error = (groq.APIError, groq.RateLimitError)
 except ImportError:
-    cohere_api_error = Exception
-    # print("Not loading Cohere because it is not installed.")
+    groq_api_error = Exception
+
+
+from dsp.modules.lm import LM
 
 
 def backoff_hdlr(details):
     """Handler from https://pypi.org/project/backoff/"""
     print(
         "Backing off {wait:0.1f} seconds after {tries} tries "
         "calling function {target} with kwargs "
         "{kwargs}".format(**details),
     )
 
 
-def giveup_hdlr(details):
-    """wrapper function that decides when to give up on retry"""
-    if "rate limits" in details.message:
-        return False
-    return True
-
-
-class Cohere(LM):
-    """Wrapper around Cohere's API.
+class GroqLM(LM):
+    """Wrapper around groq's API.
 
-    Currently supported models include `command`, `command-nightly`, `command-light`, `command-light-nightly`.
+    Args:
+        model (str, optional): groq supported LLM model to use. Defaults to "mixtral-8x7b-32768".
+        api_key (Optional[str], optional): API provider Authentication token. use Defaults to None.
+        **kwargs: Additional arguments to pass to the API provider.
     """
 
     def __init__(
         self,
-        model: str = "command-nightly",
-        api_key: Optional[str] = None,
-        stop_sequences: list[str] = [],
+        api_key: str,
+        model: str = "mixtral-8x7b-32768",
         **kwargs,
     ):
-        """
-        Parameters
-        ----------
-        model : str
-            Which pre-trained model from Cohere to use?
-            Choices are [`command`, `command-nightly`, `command-light`, `command-light-nightly`]
-        api_key : str
-            The API key for Cohere.
-            It can be obtained from https://dashboard.cohere.ai/register.
-        stop_sequences : list of str
-            Additional stop tokens to end generation.
-        **kwargs: dict
-            Additional arguments to pass to the API provider.
-        """
         super().__init__(model)
-        self.co = cohere.Client(api_key)
-        self.provider = "cohere"
+        self.provider = "groq"
+        if api_key:
+            self.api_key = api_key
+            self.client = Groq(api_key=api_key)
+        else:
+            raise ValueError("api_key is required for groq")
+
         self.kwargs = {
-            "model": model,
             "temperature": 0.0,
             "max_tokens": 150,
-            "p": 1,
+            "top_p": 1,
             "frequency_penalty": 0,
             "presence_penalty": 0,
-            "num_generations": 1,
+            "n": 1,
             **kwargs,
         }
-        self.stop_sequences = stop_sequences
-        self.max_num_generations = 5
-
+        models = self.client.models.list().data
+        if models is not None:
+            if model in [m.id for m in models]:
+                self.kwargs["model"] = model
         self.history: list[dict[str, Any]] = []
 
+    def log_usage(self, response):
+        """Log the total tokens from the Groq API response."""
+        usage_data = response.usage  # Directly accessing the 'usage' attribute
+        if usage_data:
+            total_tokens = usage_data.total_tokens
+            logging.debug(f"Groq Total Tokens Response Usage: {total_tokens}")
+
     def basic_request(self, prompt: str, **kwargs):
         raw_kwargs = kwargs
-        kwargs = {
-            **self.kwargs,
-            "stop_sequences": self.stop_sequences,
-            "prompt": prompt,
-            **kwargs,
-        }
-        response = self.co.generate(**kwargs)
+
+        kwargs = {**self.kwargs, **kwargs}
+
+        kwargs["messages"] = [{"role": "user", "content": prompt}]
+        response = self.chat_request(**kwargs)
 
         history = {
             "prompt": prompt,
-            "response": response,
+            "response": response.choices[0].message.content,
             "kwargs": kwargs,
             "raw_kwargs": raw_kwargs,
         }
+
         self.history.append(history)
 
         return response
 
     @backoff.on_exception(
         backoff.expo,
-        (cohere_api_error),
+        groq_api_error,
         max_time=1000,
         on_backoff=backoff_hdlr,
-        giveup=giveup_hdlr,
     )
     def request(self, prompt: str, **kwargs):
-        """Handles retrieval of completions from Cohere whilst handling API errors"""
+        """Handles retreival of model completions whilst handling rate limiting and caching."""
+        if "model_type" in kwargs:
+            del kwargs["model_type"]
+
         return self.basic_request(prompt, **kwargs)
 
+    def _get_choice_text(self, choice) -> str:
+        return choice.message.content
+
+    def chat_request(self, **kwargs):
+        """Handles retreival of model completions whilst handling rate limiting and caching."""
+        response = self.client.chat.completions.create(**kwargs)
+        return response
+
     def __call__(
         self,
         prompt: str,
         only_completed: bool = True,
         return_sorted: bool = False,
         **kwargs,
-    ):
+    ) -> list[dict[str, Any]]:
+        """Retrieves completions from model.
+
+        Args:
+            prompt (str): prompt to send to model
+            only_completed (bool, optional): return only completed responses and ignores completion due to length. Defaults to True.
+            return_sorted (bool, optional): sort the completion choices using the returned probabilities. Defaults to False.
+
+        Returns:
+            list[dict[str, Any]]: list of completion choices
+        """
+
         assert only_completed, "for now"
         assert return_sorted is False, "for now"
+        response = self.request(prompt, **kwargs)
 
-        # Cohere uses 'num_generations' whereas dsp.generate() uses 'n'
-        n = kwargs.pop("n", 1)
+        self.log_usage(response)
 
-        # Cohere can generate upto self.max_num_generations completions at a time
-        choices = []
-        num_iters = math.ceil(n / self.max_num_generations)
-        remainder = n % self.max_num_generations
-        for i in range(num_iters):
-            if i == (num_iters - 1):
-                kwargs["num_generations"] = (
-                    remainder if remainder != 0 else self.max_num_generations
-                )
-            else:
-                kwargs["num_generations"] = self.max_num_generations
-            response = self.request(prompt, **kwargs)
-            choices.extend(response.generations)
-        completions = [c.text for c in choices]
+        choices = response.choices
 
-        if return_sorted and kwargs.get("num_generations", 1) > 1:
+        completions = [self._get_choice_text(c) for c in choices]
+        if return_sorted and kwargs.get("n", 1) > 1:
             scored_completions = []
 
             for c in choices:
-                scored_completions.append((c.likelihood, c.text))
+                tokens, logprobs = (
+                    c["logprobs"]["tokens"],
+                    c["logprobs"]["token_logprobs"],
+                )
+
+                if "<|endoftext|>" in tokens:
+                    index = tokens.index("<|endoftext|>") + 1
+                    tokens, logprobs = tokens[:index], logprobs[:index]
+
+                avglog = sum(logprobs) / len(logprobs)
+                scored_completions.append((avglog, self._get_choice_text(c)))
 
             scored_completions = sorted(scored_completions, reverse=True)
             completions = [c for _, c in scored_completions]
 
         return completions
```

### Comparing `dspy-ai-2.4.7/dsp/modules/colbertv2.py` & `dspy-ai-2.4.9/dsp/modules/colbertv2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/modules/databricks.py` & `dspy-ai-2.4.9/dsp/modules/databricks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-import logging
-
-# Configure logging
-logging.basicConfig(
-    level=logging.INFO,
-    format='%(message)s',
-    handlers=[
-        logging.FileHandler('openai_usage.log'),
-    ],
-)
-
 import functools
 import json
 from typing import Literal, Optional
 
 import openai
 
 from dsp.modules.cache_utils import CacheMemory, NotebookCacheMemory, cache_turn_on
```

### Comparing `dspy-ai-2.4.7/dsp/modules/finetuning/finetune_hf.py` & `dspy-ai-2.4.9/dsp/modules/finetuning/finetune_hf.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/modules/google.py` & `dspy-ai-2.4.9/dsp/modules/google.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/modules/gpt3.py` & `dspy-ai-2.4.9/dsp/modules/gpt3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,28 @@
-import logging
-
-# Configure logging
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(message)s",
-    handlers=[logging.FileHandler("openai_usage.log")],
-)
-
 import functools
 import json
+import logging
 from typing import Any, Literal, Optional, cast
 
 import backoff
 import openai
 
-import dsp
 from dsp.modules.cache_utils import CacheMemory, NotebookCacheMemory, cache_turn_on
 from dsp.modules.lm import LM
 
 try:
     OPENAI_LEGACY = int(openai.version.__version__[0]) == 0
 except Exception:
     OPENAI_LEGACY = True
 
 try:
     import openai.error
     from openai.openai_object import OpenAIObject
 
-    ERRORS = (
-        openai.error.RateLimitError,
-    )
+    ERRORS = (openai.error.RateLimitError,)
 except Exception:
     ERRORS = (openai.RateLimitError,)
     OpenAIObject = dict
 
 
 def backoff_hdlr(details):
     """Handler from https://pypi.org/project/backoff/"""
@@ -44,42 +33,44 @@
     )
 
 
 class GPT3(LM):
     """Wrapper around OpenAI's GPT API.
 
     Args:
-        model (str, optional): OpenAI supported LLM model to use. Defaults to "text-davinci-002".
+        model (str, optional): OpenAI supported LLM model to use. Defaults to "gpt-3.5-turbo-instruct".
         api_key (Optional[str], optional): API provider Authentication token. use Defaults to None.
         api_provider (Literal["openai"], optional): The API provider to use. Defaults to "openai".
         model_type (Literal["chat", "text"], optional): The type of model that was specified. Mainly to decide the optimal prompting strategy. Defaults to "text".
         **kwargs: Additional arguments to pass to the API provider.
     """
 
     def __init__(
         self,
         model: str = "gpt-3.5-turbo-instruct",
         api_key: Optional[str] = None,
         api_provider: Literal["openai"] = "openai",
         api_base: Optional[str] = None,
         model_type: Literal["chat", "text"] = None,
+        system_prompt: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(model)
         self.provider = "openai"
         openai.api_type = api_provider
 
+        self.system_prompt = system_prompt
+
         assert (
             api_provider != "azure"
         ), "Azure functionality with base OpenAI has been deprecated, please use dspy.AzureOpenAI instead."
 
         default_model_type = (
             "chat"
-            if ("gpt-3.5" in model or "turbo" in model or "gpt-4" in model)
-            and ("instruct" not in model)
+            if ("gpt-3.5" in model or "turbo" in model or "gpt-4" in model) and ("instruct" not in model)
             else "text"
         )
         self.model_type = model_type if model_type else default_model_type
 
         if api_key:
             openai.api_key = api_key
 
@@ -106,23 +97,26 @@
         return openai
 
     def log_usage(self, response):
         """Log the total tokens from the OpenAI API response."""
         usage_data = response.get("usage")
         if usage_data:
             total_tokens = usage_data.get("total_tokens")
-            logging.info(f"{total_tokens}")
+            logging.debug(f"OpenAI Response Token Usage: {total_tokens}")
 
     def basic_request(self, prompt: str, **kwargs):
         raw_kwargs = kwargs
 
         kwargs = {**self.kwargs, **kwargs}
         if self.model_type == "chat":
             # caching mechanism requires hashable kwargs
-            kwargs["messages"] = [{"role": "user", "content": prompt}]
+            messages = [{"role": "user", "content": prompt}]
+            if self.system_prompt:
+                messages.insert(0, {"role": "system", "content": self.system_prompt})
+            kwargs["messages"] = messages
             kwargs = {"stringify_request": json.dumps(kwargs)}
             response = chat_request(**kwargs)
 
         else:
             kwargs["prompt"] = prompt
             response = completions_request(**kwargs)
 
@@ -179,17 +173,15 @@
         #     if self.model_type == "chat":
         #         kwargs = {**kwargs}
         #     else:
         #         kwargs = {**kwargs, "logprobs": 5}
 
         response = self.request(prompt, **kwargs)
 
-        if dsp.settings.log_openai_usage:
-            self.log_usage(response)
-
+        self.log_usage(response)
         choices = response["choices"]
 
         completed_choices = [c for c in choices if c["finish_reason"] != "length"]
 
         if only_completed and len(completed_choices):
             choices = completed_choices
```

### Comparing `dspy-ai-2.4.7/dsp/modules/hf.py` & `dspy-ai-2.4.9/dsp/modules/hf.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,33 +36,40 @@
         hf_device_map: Literal[
             "auto",
             "balanced",
             "balanced_low_0",
             "sequential",
         ] = "auto",
         token: Optional[str] = None,
+        model_kwargs: Optional[dict] = {},
     ):
         """wrapper for Hugging Face models
 
         Args:
             model (str): HF model identifier to load and use
             checkpoint (str, optional): load specific checkpoints of the model. Defaults to None.
             is_client (bool, optional): whether to access models via client. Defaults to False.
             hf_device_map (str, optional): HF config strategy to load the model.
                 Recommeded to use "auto", which will help loading large models using accelerate. Defaults to "auto".
+            model_kwargs (dict, optional): additional kwargs to pass to the model constructor. Defaults to empty dict.
         """
 
         super().__init__(model)
         self.provider = "hf"
         self.is_client = is_client
         self.device_map = hf_device_map
 
         hf_autoconfig_kwargs = dict(token=token or os.environ.get("HF_TOKEN"))
         hf_autotokenizer_kwargs = hf_autoconfig_kwargs.copy()
         hf_automodel_kwargs = hf_autoconfig_kwargs.copy()
+
+        # silently remove device_map from model_kwargs if it is present, as the option is provided in the constructor
+        if "device_map" in model_kwargs:
+            model_kwargs.pop("device_map")
+        hf_automodel_kwargs.update(model_kwargs)
         if not self.is_client:
             try:
                 import torch
                 from transformers import AutoConfig, AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoTokenizer
             except ImportError as exc:
                 raise ModuleNotFoundError(
                     "You need to install Hugging Face transformers library to use HF models.",
```

### Comparing `dspy-ai-2.4.7/dsp/modules/hf_client.py` & `dspy-ai-2.4.9/dsp/modules/hf_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import random
 import re
 import shutil
 import subprocess
+from typing import Literal
 
 # from dsp.modules.adapter import TurboAdapter, DavinciAdapter, LlamaAdapter
 import backoff
 import requests
 
 from dsp.modules.cache_utils import CacheMemory, NotebookCacheMemory
 from dsp.modules.hf import HFModel, openai_to_hf
@@ -28,14 +29,17 @@
         self.url = url
         self.ports = port if isinstance(port, list) else [port]
         self.http_request_kwargs = http_request_kwargs or {}
 
         self.headers = {"Content-Type": "application/json"}
 
         self.kwargs = {
+            "model": model,
+            "port": port,
+            "url": url,
             "temperature": 0.01,
             "max_tokens": 75,
             "top_p": 0.97,
             "n": 1,
             "stop": ["\n", "\n\n"],
             **kwargs,
         }
@@ -110,53 +114,120 @@
 
 @CacheMemory.cache
 def send_hftgi_request_v00(arg, **kwargs):
     return requests.post(arg, **kwargs)
 
 
 class HFClientVLLM(HFModel):
-    def __init__(self, model, port, url="http://localhost", **kwargs):
+    def __init__(self, model, port, model_type: Literal['chat', 'text'] = 'text', url="http://localhost", **kwargs):
         super().__init__(model=model, is_client=True)
-        self.url = f"{url}:{port}"
+
+        if isinstance(url, list):
+            self.urls = url
+        
+        elif isinstance(url, str):
+            self.urls = [f'{url}:{port}']
+        
+        else:
+            raise ValueError(f"The url provided to `HFClientVLLM` is neither a string nor a list of strings. It is of type {type(url)}.")
+        
+        self.urls_const = tuple(self.urls)
+        self.port = port
+        self.model_type = model_type
         self.headers = {"Content-Type": "application/json"}
+        self.kwargs |= kwargs
+        # kwargs needs to have model, port and url for the lm.copy() to work properly
+        self.kwargs.update({
+            'port': port,
+            'url': self.urls_const,
+        })
+
 
     def _generate(self, prompt, **kwargs):
         kwargs = {**self.kwargs, **kwargs}
-
-        payload = {
-            "model": kwargs["model"],
-            "prompt": prompt,
-            "max_tokens": kwargs["max_tokens"],
-            "temperature": kwargs["temperature"],
-        }
-
-        response = send_hfvllm_request_v00(
-            f"{self.url}/v1/completions",
-            json=payload,
-            headers=self.headers,
-        )
-
-        try:
-            json_response = response.json()
-            completions = json_response["choices"]
-            response = {
+        
+        # Round robin the urls.
+        url = self.urls.pop(0)
+        self.urls.append(url)
+        
+        if self.model_type == "chat":
+            system_prompt = kwargs.get("system_prompt",None)
+            messages = [{"role": "user", "content": prompt}]
+            if system_prompt:
+                messages.insert(0, {"role": "system", "content": system_prompt})
+            payload = {
+                "model": self.kwargs["model"],
+                "messages": messages,
+                **kwargs,
+            }
+            response = send_hfvllm_request_v01_wrapped(
+                f"{url}/v1/chat/completions",
+                url=self.urls_const,
+                port=self.port,
+                json=payload,
+                headers=self.headers,
+            )
+
+            try:
+                json_response = response.json()
+                completions = json_response["choices"]
+                response = {
+                    "prompt": prompt,
+                    "choices": [{"text": c["message"]['content']} for c in completions],
+                }
+                return response
+
+            except Exception:
+                print("Failed to parse JSON response:", response.text)
+                raise Exception("Received invalid JSON response from server")
+        else:
+            payload = {
+                "model": self.kwargs["model"],
                 "prompt": prompt,
-                "choices": [{"text": c["text"]} for c in completions],
+                **kwargs,
             }
-            return response
 
-        except Exception:
-            print("Failed to parse JSON response:", response.text)
-            raise Exception("Received invalid JSON response from server")
+            response = send_hfvllm_request_v01_wrapped(
+                f"{url}/v1/completions",
+                url=self.urls_const,
+                port=self.port,
+                json=payload,
+                headers=self.headers,
+            )
+
+            try:
+                json_response = response.json()
+                completions = json_response["choices"]
+                response = {
+                    "prompt": prompt,
+                    "choices": [{"text": c["text"]} for c in completions],
+                }
+                return response
+
+            except Exception:
+                print("Failed to parse JSON response:", response.text)
+                raise Exception("Received invalid JSON response from server")
+
+@CacheMemory.cache(ignore=['arg'])
+def send_hfvllm_request_v01(arg, url, port, **kwargs):
+    return requests.post(arg, **kwargs)
 
+# @functools.lru_cache(maxsize=None if cache_turn_on else 0)
+@NotebookCacheMemory.cache(ignore=['arg'])
+def send_hfvllm_request_v01_wrapped(arg, url, port, **kwargs):
+    return send_hftgi_request_v01(arg, url, port, **kwargs)
 
 @CacheMemory.cache
 def send_hfvllm_request_v00(arg, **kwargs):
     return requests.post(arg, **kwargs)
 
+@CacheMemory.cache
+def send_hfvllm_chat_request_v00(arg, **kwargs):
+    return requests.post(arg, **kwargs)
+
 
 class HFServerTGI:
     def __init__(self, user_dir):
         self.model_weights_dir = os.path.abspath(os.path.join(os.getcwd(), "text-generation-inference", user_dir))
         if not os.path.exists(self.model_weights_dir):
             os.makedirs(self.model_weights_dir)
```

### Comparing `dspy-ai-2.4.7/dsp/modules/hf_server.py` & `dspy-ai-2.4.9/dsp/modules/hf_server.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/modules/lm.py` & `dspy-ai-2.4.9/dsp/modules/lm.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,83 +22,87 @@
     def basic_request(self, prompt, **kwargs):
         pass
 
     def request(self, prompt, **kwargs):
         return self.basic_request(prompt, **kwargs)
 
     def print_green(self, text: str, end: str = "\n"):
-        print("\x1b[32m" + str(text) + "\x1b[0m", end=end)
+        return "\x1b[32m" + str(text) + "\x1b[0m" + end
 
     def print_red(self, text: str, end: str = "\n"):
-        print("\x1b[31m" + str(text) + "\x1b[0m", end=end)
+        return "\x1b[31m" + str(text) + "\x1b[0m" + end
 
     def inspect_history(self, n: int = 1, skip: int = 0):
         """Prints the last n prompts and their completions.
-        TODO: print the valid choice that contains filled output field instead of the first
+
+        TODO: print the valid choice that contains filled output field instead of the first.
         """
         provider: str = self.provider
 
         last_prompt = None
         printed = []
         n = n + skip
 
         for x in reversed(self.history[-100:]):
             prompt = x["prompt"]
 
             if prompt != last_prompt:
-
-                if provider == "clarifai" or provider == "google" or provider == "claude":
-                    printed.append(
-                        (
-                            prompt,
-                            x['response'],
-                        ),
-                    )
+                if provider == "clarifai" or provider == "google" or provider == "groq" or provider == "Bedrock" or provider == "Sagemaker":
+                    printed.append((prompt, x["response"]))
+                elif provider == "anthropic":
+                    blocks = [{"text": block.text} for block in x["response"].content if block.type == "text"]
+                    printed.append((prompt, blocks))
+                elif provider == "cohere":
+                    printed.append((prompt, x["response"].text))
+                elif provider == "mistral":
+                    printed.append((prompt, x['response'].choices))
                 else:
-                    printed.append(
-                        (
-                            prompt,
-                            x["response"].generations
-                            if provider == "cohere"
-                            else x["response"]["choices"],
-                        ),
-                    )
+                    printed.append((prompt, x["response"]["choices"]))
 
             last_prompt = prompt
 
             if len(printed) >= n:
                 break
 
+        printing_value = ""
         for idx, (prompt, choices) in enumerate(reversed(printed)):
             # skip the first `skip` prompts
             if (n - idx - 1) < skip:
                 continue
+            printing_value += "\n\n\n"
+            printing_value += prompt
 
-            print("\n\n\n")
-            print(prompt, end="")
             text = ""
-            if provider == "cohere":
-                text = choices[0].text
+            if provider == "cohere" or provider == "Bedrock" or provider == "Sagemaker":
+                text = choices
             elif provider == "openai" or provider == "ollama":
                 text = ' ' + self._get_choice_text(choices[0]).strip()
             elif provider == "clarifai" or provider == "claude" :
                 text=choices
+            elif provider == "groq":
+                text = ' ' + choices
             elif provider == "google":
                 text = choices[0].parts[0].text
+            elif provider == "mistral":
+                text = choices[0].message.content
             else:
                 text = choices[0]["text"]
-            self.print_green(text, end="")
+            printing_value += self.print_green(text, end="")
 
             if len(choices) > 1:
-                self.print_red(f" \t (and {len(choices)-1} other completions)", end="")
-            print("\n\n\n")
+                printing_value += self.print_red(f" \t (and {len(choices)-1} other completions)", end="")
+
+            printing_value += "\n\n\n"
+
+        print(printing_value)
+        return printing_value
 
     @abstractmethod
     def __call__(self, prompt, only_completed=True, return_sorted=False, **kwargs):
         pass
 
     def copy(self, **kwargs):
         """Returns a copy of the language model with the same parameters."""
         kwargs = {**self.kwargs, **kwargs}
-        model = kwargs.pop('model')
+        model = kwargs.pop("model")
 
         return self.__class__(model=model, **kwargs)
```

### Comparing `dspy-ai-2.4.7/dsp/modules/ollama.py` & `dspy-ai-2.4.9/dsp/modules/ollama.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/modules/pyserini.py` & `dspy-ai-2.4.9/dsp/modules/pyserini.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/modules/sbert.py` & `dspy-ai-2.4.9/dsp/modules/sbert.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/modules/sentence_vectorizer.py` & `dspy-ai-2.4.9/dsp/modules/sentence_vectorizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/primitives/compiler.py` & `dspy-ai-2.4.9/dsp/primitives/compiler.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/primitives/demonstrate.py` & `dspy-ai-2.4.9/dsp/primitives/demonstrate.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/primitives/inspect.py` & `dspy-ai-2.4.9/dsp/primitives/inspect.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/primitives/predict.py` & `dspy-ai-2.4.9/dsp/primitives/predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,19 +94,28 @@
         # If none of the completions is completed (i.e., none has the final field set).
         if last_field_idx < len(field_names):
             # Pick the first completion that has gone farthest.
             completion = completions[0]
             completion[field_names[last_field_idx]] = ""
 
             # Recurse with greedy decoding and a shorter length.
-            max_tokens = kwargs.get("max_tokens", dsp.settings.lm.kwargs["max_tokens"])
+            max_tokens = (kwargs.get("max_tokens") or 
+                        kwargs.get("max_output_tokens") or
+                        dsp.settings.lm.kwargs.get("max_tokens") or 
+                        dsp.settings.lm.kwargs.get('max_output_tokens'))
+
+
+            if max_tokens is None:
+                raise ValueError("Required 'max_tokens' or 'max_output_tokens' not specified in settings.")
             max_tokens = min(max(75, max_tokens // 2), max_tokens)
+            keys = list(kwargs.keys()) + list(dsp.settings.lm.kwargs.keys()) 
+            max_tokens_key = "max_tokens" if "max_tokens" in keys else "max_output_tokens"
             new_kwargs = {
                 **kwargs,
-                "max_tokens": max_tokens,
+                max_tokens_key: max_tokens,
                 "n": 1,
                 "temperature": 0.0,
             }
 
             assert max_depth > 0
             return generate(template, **new_kwargs)(
                 completion,
```

### Comparing `dspy-ai-2.4.7/dsp/primitives/primitives.py` & `dspy-ai-2.4.9/dsp/primitives/primitives.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/primitives/search.py` & `dspy-ai-2.4.9/dsp/primitives/search.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,49 +20,49 @@
         passages_cs_scores = dsp.settings.reranker(query, passages)
         passages_cs_scores_sorted = np.argsort(passages_cs_scores)[::-1]
         passages = [passages[idx] for idx in passages_cs_scores_sorted]
 
     return passages
 
 
-def retrieveRerankEnsemble(queries: list[str], k: int) -> list[str]:
+def retrieveRerankEnsemble(queries: list[str], k: int,**kwargs) -> list[str]:
     if not (dsp.settings.rm and dsp.settings.reranker):
         raise AssertionError("Both RM and Reranker are needed to retrieve & re-rank.")
     queries = [q for q in queries if q]
     passages = {}
     for query in queries:
-        retrieved_passages = dsp.settings.rm(query, k=k*3)
+        retrieved_passages = dsp.settings.rm(query, k=k*3,**kwargs)
         passages_cs_scores = dsp.settings.reranker(query, [psg.long_text for psg in retrieved_passages])
         for idx in np.argsort(passages_cs_scores)[::-1]:
             psg = retrieved_passages[idx]
             passages[psg.long_text] = passages.get(psg.long_text, []) + [
                 passages_cs_scores[idx],
             ]
 
     passages = [(np.average(score), text) for text, score in passages.items()]
     return [text for _, text in sorted(passages, reverse=True)[:k]]
 
 
-def retrieveEnsemble(queries: list[str], k: int, by_prob: bool = True) -> list[str]:
+def retrieveEnsemble(queries: list[str], k: int, by_prob: bool = True,**kwargs) -> list[str]:
     """Retrieves passages from the RM for each query in queries and returns the top k passages
     based on the probability or score.
     """
     if not dsp.settings.rm:
         raise AssertionError("No RM is loaded.")
     if dsp.settings.reranker:
         return retrieveRerankEnsemble(queries, k)
     
     queries = [q for q in queries if q]
 
     if len(queries) == 1:
-        return retrieve(queries[0], k)
+        return retrieve(queries[0], k, **kwargs)
 
     passages = {}
     for q in queries:
-        for psg in dsp.settings.rm(q, k=k * 3):
+        for psg in dsp.settings.rm(q, k=k * 3,**kwargs):
             if by_prob:
                 passages[psg.long_text] = passages.get(psg.long_text, 0.0) + psg.prob
             else:
                 passages[psg.long_text] = passages.get(psg.long_text, 0.0) + psg.score
 
     passages = [(score, text) for text, score in passages.items()]
     passages = sorted(passages, reverse=True)[:k]
```

### Comparing `dspy-ai-2.4.7/dsp/templates/template_v2.py` & `dspy-ai-2.4.9/dsp/templates/template_v2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/templates/template_v3.py` & `dspy-ai-2.4.9/dsp/templates/template_v3.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/templates/utils.py` & `dspy-ai-2.4.9/dsp/templates/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/utils/ann_utils.py` & `dspy-ai-2.4.9/dsp/utils/ann_utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/utils/dpr.py` & `dspy-ai-2.4.9/dsp/utils/dpr.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/utils/metrics.py` & `dspy-ai-2.4.9/dsp/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/utils/settings.py` & `dspy-ai-2.4.9/dsp/utils/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,33 +16,30 @@
 
         if cls._instance is None:
             cls._instance = super().__new__(cls)
             cls._instance.lock = threading.Lock()
             cls._instance.main_tid = threading.get_ident()
             cls._instance.main_stack = []
             cls._instance.stack_by_thread = {}
-            cls._instance.stack_by_thread[
-                threading.get_ident()
-            ] = cls._instance.main_stack
+            cls._instance.stack_by_thread[threading.get_ident()] = cls._instance.main_stack
 
             #  TODO: remove first-class support for re-ranker and potentially combine with RM to form a pipeline of sorts
             #  eg: RetrieveThenRerankPipeline(RetrievalModel, Reranker)
             #  downstream operations like dsp.retrieve would use configs from the defined pipeline.
             config = dotdict(
                 lm=None,
                 rm=None,
                 branch_idx=0,
                 reranker=None,
                 compiled_lm=None,
                 force_reuse_cached_compilation=False,
                 compiling=False,
                 skip_logprobs=False,
-                trace=None,
+                trace=[],
                 release=0,
-                log_openai_usage=False,
                 bypass_assert=False,
                 bypass_suggest=False,
                 assert_failures=0,
                 suggest_failures=0,
                 langchain_history=[],
             )
             cls._instance.__append(config)
```

### Comparing `dspy-ai-2.4.7/dsp/utils/settings_v2.py` & `dspy-ai-2.4.9/dsp/utils/settings_v2.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dsp/utils/utils.py` & `dspy-ai-2.4.9/dsp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/__init__.py` & `dspy-ai-2.4.9/dspy/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,31 +3,43 @@
 
 from .predict import *
 from .primitives import *
 from .retrieve import *
 from .signatures import *
 
 # Functional must be imported after primitives, predict and signatures
-from .functional import * # isort: skip
+from .functional import *  # isort: skip
+from .utils.logging import logger, set_log_output
 
 settings = dsp.settings
 
+LM = dsp.LM
+
 AzureOpenAI = dsp.AzureOpenAI
 OpenAI = dsp.GPT3
+Mistral = dsp.Mistral
 Databricks = dsp.Databricks
 Cohere = dsp.Cohere
 ColBERTv2 = dsp.ColBERTv2
 Pyserini = dsp.PyseriniRetriever
 Clarifai = dsp.ClarifaiLLM
 Google = dsp.Google
+GoogleVertexAI = dsp.GoogleVertexAI
+GROQ = dsp.GroqLM
 
 HFClientTGI = dsp.HFClientTGI
 HFClientVLLM = HFClientVLLM
 
 Anyscale = dsp.Anyscale
 Together = dsp.Together
 HFModel = dsp.HFModel
 OllamaLocal = dsp.OllamaLocal
+
 Bedrock = dsp.Bedrock
+Sagemaker = dsp.Sagemaker
+AWSModel = dsp.AWSModel
+AWSMistral = dsp.AWSMistral
+AWSAnthropic = dsp.AWSAnthropic
+AWSMeta = dsp.AWSMeta
 
 configure = settings.configure
 context = settings.context
```

### Comparing `dspy-ai-2.4.7/dspy/datasets/colors.py` & `dspy-ai-2.4.9/dspy/datasets/colors.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/datasets/dataloader.py` & `dspy-ai-2.4.9/dspy/datasets/dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,21 @@
         dataset = load_dataset("json", data_files=file_path)["train"]
         
         if not fields:
             fields = list(dataset.features)
         
         return [dspy.Example({field:row[field] for field in fields}).with_inputs(*input_keys) for row in dataset]
 
+    def from_parquet(self, file_path: str, fields: List[str] = None, input_keys: Tuple[str] = ()) -> List[dspy.Example]:
+        dataset = load_dataset("parquet", data_files=file_path)["train"]
+
+        if not fields:
+            fields = list(dataset.features)
+
+        return [dspy.Example({field: row[field] for field in fields}).with_inputs(input_keys) for row in dataset]
 
     def sample(
         self,
         dataset: List[dspy.Example],
         n: int,
         *args,
         **kwargs,
```

### Comparing `dspy-ai-2.4.7/dspy/datasets/dataset.py` & `dspy-ai-2.4.9/dspy/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/datasets/gsm8k.py` & `dspy-ai-2.4.9/dspy/datasets/gsm8k.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/datasets/hotpotqa.py` & `dspy-ai-2.4.9/dspy/datasets/hotpotqa.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/evaluate/auto_evaluation.py` & `dspy-ai-2.4.9/dspy/evaluate/auto_evaluation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/evaluate/evaluate.py` & `dspy-ai-2.4.9/dspy/evaluate/evaluate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import sys
 import threading
 import types
 
 import pandas as pd
 import tqdm
+from tqdm.contrib.logging import logging_redirect_tqdm
 
-import dsp
+import dspy
 
 try:
     from IPython.display import HTML
     from IPython.display import display as ipython_display
 except ImportError:
     ipython_display = print
 
@@ -31,172 +33,162 @@
         self,
         *,
         devset,
         metric=None,
         num_threads=1,
         display_progress=False,
         display_table=False,
-        display=True,
         max_errors=5,
         return_outputs=False,
+        **_kwargs,
     ):
         self.devset = devset
         self.metric = metric
         self.num_threads = num_threads
         self.display_progress = display_progress
         self.display_table = display_table
-        self.display = display
         self.max_errors = max_errors
         self.error_count = 0
         self.error_lock = threading.Lock()
         self.return_outputs = return_outputs
 
+        if "display" in _kwargs:
+            dspy.logger.warning(
+                "DeprecationWarning: 'display' has been deprecated. To see all information for debugging, use 'dspy.set_log_level('debug')'. In the future this will raise an error.",
+            )
+
     def _execute_single_thread(self, wrapped_program, devset, display_progress):
         ncorrect = 0
         ntotal = 0
         reordered_devset = []
 
-        pbar = tqdm.tqdm(total=len(devset), dynamic_ncols=True,
-                         disable=not display_progress)
+        pbar = tqdm.tqdm(total=len(devset), dynamic_ncols=True, disable=not display_progress, file=sys.stdout)
         for idx, arg in devset:
-            example_idx, example, prediction, score = wrapped_program(idx, arg)
-            reordered_devset.append((example_idx, example, prediction, score))
-            ncorrect += score
-            ntotal += 1
-            self._update_progress(pbar, ncorrect, ntotal)
+            with logging_redirect_tqdm():
+                example_idx, example, prediction, score = wrapped_program(idx, arg)
+                reordered_devset.append((example_idx, example, prediction, score))
+                ncorrect += score
+                ntotal += 1
+                self._update_progress(pbar, ncorrect, ntotal)
+
         pbar.close()
 
         return reordered_devset, ncorrect, ntotal
 
     def _execute_multi_thread(self, wrapped_program, devset, num_threads, display_progress):
         ncorrect = 0
         ntotal = 0
         reordered_devset = []
 
         with ThreadPoolExecutor(max_workers=num_threads) as executor:
-            futures = {executor.submit(wrapped_program, idx, arg)
-                       for idx, arg in devset}
-            pbar = tqdm.tqdm(total=len(devset), dynamic_ncols=True,
-                             disable=not display_progress)
+            futures = {executor.submit(wrapped_program, idx, arg) for idx, arg in devset}
+            pbar = tqdm.tqdm(total=len(devset), dynamic_ncols=True, disable=not display_progress)
 
             for future in as_completed(futures):
                 example_idx, example, prediction, score = future.result()
-                reordered_devset.append(
-                    (example_idx, example, prediction, score))
+                reordered_devset.append((example_idx, example, prediction, score))
                 ncorrect += score
                 ntotal += 1
                 self._update_progress(pbar, ncorrect, ntotal)
             pbar.close()
 
         return reordered_devset, ncorrect, ntotal
 
     def _update_progress(self, pbar, ncorrect, ntotal):
-        pbar.set_description(
-            f"Average Metric: {ncorrect} / {ntotal}  ({round(100 * ncorrect / ntotal, 1)})")
+        pbar.set_description(f"Average Metric: {ncorrect} / {ntotal}  ({round(100 * ncorrect / ntotal, 1)})")
         pbar.update()
 
     def __call__(
         self,
         program,
         metric=None,
         devset=None,
         num_threads=None,
         display_progress=None,
         display_table=None,
-        display=None,
         return_all_scores=False,
         return_outputs=False,
     ):
         metric = metric if metric is not None else self.metric
         devset = devset if devset is not None else self.devset
         num_threads = num_threads if num_threads is not None else self.num_threads
         display_progress = display_progress if display_progress is not None else self.display_progress
         display_table = display_table if display_table is not None else self.display_table
-
-        display = self.display if display is None else display
-        display_progress = display_progress and display
-        display_table = display_table if display else False
         return_outputs = return_outputs if return_outputs is not False else self.return_outputs
         results = []
 
         def wrapped_program(example_idx, example):
             # NOTE: TODO: Won't work if threads create threads!
-            creating_new_thread = threading.get_ident() not in dsp.settings.stack_by_thread
+            thread_stacks = dspy.settings.stack_by_thread
+            creating_new_thread = threading.get_ident() not in thread_stacks
             if creating_new_thread:
-                dsp.settings.stack_by_thread[threading.get_ident()] = list(
-                    dsp.settings.main_stack)
-                # print(threading.get_ident(), dsp.settings.stack_by_thread[threading.get_ident()])
-
-            # print(type(example), example)
+                thread_stacks[threading.get_ident()] = list(dspy.settings.main_stack)
 
             try:
                 prediction = program(**example.inputs())
                 score = metric(
                     example,
                     prediction,
                 )  # FIXME: TODO: What's the right order? Maybe force name-based kwargs!
 
                 # increment assert and suggest failures to program's attributes
                 if hasattr(program, "_assert_failures"):
-                    program._assert_failures += dsp.settings.assert_failures
+                    program._assert_failures += dspy.settings.get("assert_failures")
                 if hasattr(program, "_suggest_failures"):
-                    program._suggest_failures += dsp.settings.suggest_failures
+                    program._suggest_failures += dspy.settings.get("suggest_failures")
 
                 return example_idx, example, prediction, score
             except Exception as e:
                 with self.error_lock:
                     self.error_count += 1
                     current_error_count = self.error_count
                 if current_error_count >= self.max_errors:
                     raise e
-                print(f"Error for example in dev set: \t\t {e}")
-                return example_idx, example, dict(), 0.0
+
+                dspy.logger.error(f"Error for example in dev set: \t\t {e}")
+
+                return example_idx, example, {}, 0.0
             finally:
                 if creating_new_thread:
-                    del dsp.settings.stack_by_thread[threading.get_ident()]
+                    del thread_stacks[threading.get_ident()]
 
         devset = list(enumerate(devset))
+        tqdm.tqdm._instances.clear()
 
         if num_threads == 1:
-            reordered_devset, ncorrect, ntotal = self._execute_single_thread(
-                wrapped_program, devset, display_progress)
+            reordered_devset, ncorrect, ntotal = self._execute_single_thread(wrapped_program, devset, display_progress)
         else:
             reordered_devset, ncorrect, ntotal = self._execute_multi_thread(
                 wrapped_program,
                 devset,
                 num_threads,
                 display_progress,
             )
-        if return_outputs:  # Handle the return_outputs logic
-            results = [(example, prediction, score)
-                       for _, example, prediction, score in reordered_devset]
 
-        if display:
-            print(
-                f"Average Metric: {ncorrect} / {ntotal}  ({round(100 * ncorrect / ntotal, 1)}%)")
+        dspy.logger.info(f"Average Metric: {ncorrect} / {ntotal} ({round(100 * ncorrect / ntotal, 1)}%)")
 
         predicted_devset = sorted(reordered_devset)
 
-        # data = [{**example, **prediction, 'correct': score} for example, prediction, score in zip(reordered_devset, preds, scores)]
+        if return_outputs:  # Handle the return_outputs logic
+            results = [(example, prediction, score) for _, example, prediction, score in predicted_devset]
+
         data = [
             merge_dicts(example, prediction) | {"correct": score} for _, example, prediction, score in predicted_devset
         ]
 
         df = pd.DataFrame(data)
 
         # Truncate every cell in the DataFrame
         if hasattr(df, "map"):  # DataFrame.applymap was renamed to DataFrame.map in Pandas 2.1.0
             df = df.map(truncate_cell)
         else:
             df = df.applymap(truncate_cell)
 
         # Rename the 'correct' column to the name of the metric object
-        assert callable(metric)
-        metric_name = metric.__name__ if isinstance(
-            metric, types.FunctionType) else metric.__class__.__name__
+        metric_name = metric.__name__ if isinstance(metric, types.FunctionType) else metric.__class__.__name__
         df.rename(columns={"correct": metric_name}, inplace=True)
 
         if display_table:
             if isinstance(display_table, int):
                 df_to_display = df.head(display_table).copy()
                 truncated_rows = len(df) - display_table
             else:
@@ -218,17 +210,17 @@
                     margin: 10px 0;'>
                     ... {truncated_rows} more rows not displayed ...
                 </div>
                 """
                 ipython_display(HTML(message))
 
         if return_all_scores and return_outputs:
-            return round(100 * ncorrect / ntotal, 2), results, [score for *_, score in reordered_devset]
+            return round(100 * ncorrect / ntotal, 2), results, [score for *_, score in predicted_devset]
         elif return_all_scores:
-            return round(100 * ncorrect / ntotal, 2), [score for *_, score in reordered_devset]
+            return round(100 * ncorrect / ntotal, 2), [score for *_, score in predicted_devset]
         elif return_outputs:
             return round(100 * ncorrect / ntotal, 2), results
 
         return round(100 * ncorrect / ntotal, 2)
 
 
 def merge_dicts(d1, d2):
@@ -259,16 +251,17 @@
 def configure_dataframe_display(df, metric_name):
     """Set various pandas display options for DataFrame."""
     pd.options.display.max_colwidth = None
     pd.set_option("display.max_colwidth", 20)  # Adjust the number as needed
     pd.set_option("display.width", 400)  # Adjust
 
     # df[metric_name] = df[metric_name].apply(lambda x: f'✔️ [{x}]' if x is True else f'❌ [{x}]')
-    df.loc[:, metric_name] = df[metric_name].apply(
-        lambda x: f"✔️ [{x}]" if x is True else f"{x}")
+    # df.loc[:, metric_name] = df[metric_name].apply(lambda x: f"✔️ [{x}]" if x is True else f"{x}")
+    df[metric_name] = df[metric_name].apply(lambda x: f"✔️ [{x}]" if x else str(x))
+
 
     # Return styled DataFrame
     return df.style.set_table_styles(
         [
             {"selector": "th", "props": [("text-align", "left")]},
             {"selector": "td", "props": [("text-align", "left")]},
         ],
```

### Comparing `dspy-ai-2.4.7/dspy/evaluate/metrics.py` & `dspy-ai-2.4.9/dspy/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/experimental/synthesizer/config.py` & `dspy-ai-2.4.9/dspy/experimental/synthesizer/config.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/experimental/synthesizer/instruction_suffixes.py` & `dspy-ai-2.4.9/dspy/experimental/synthesizer/instruction_suffixes.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/experimental/synthesizer/signatures.py` & `dspy-ai-2.4.9/dspy/experimental/synthesizer/signatures.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/experimental/synthesizer/synthesizer.py` & `dspy-ai-2.4.9/dspy/experimental/synthesizer/synthesizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,17 @@
             kwargs = {
                 "task_description": task_description,
                 "knowledge_seed": iter_seed,
                 "config": dict(temperature=iter_temperature, n=batch_size),
             }
 
             if self.config.num_example_for_optim:
-                kwargs["ground_source"] = random.sample(ground_source, self.config.num_example_for_optim)
+                if not isinstance(ground_source, list):
+                    raise ValueError("Ground source must be a list of examples when `num_example_for_optim` is provided.")
+                kwargs["ground_source"] = random.sample(ground_source, k=self.config.num_example_for_optim)
             
             with dspy.context(lm=self.input_lm):
                 inputs = self.input_predictor(**kwargs)
 
             input_kwargs = [{
                 key: getattr(completions, key)
                 for key in input_keys
```

### Comparing `dspy-ai-2.4.7/dspy/experimental/synthesizer/utils.py` & `dspy-ai-2.4.9/dspy/experimental/synthesizer/utils.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/experimental/synthetic_data.py` & `dspy-ai-2.4.9/dspy/experimental/synthetic_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,89 @@
+import logging
 import random
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 import dspy
 
 
-class descriptionSignature(dspy.Signature):
-  field_name = dspy.InputField(desc="name of a field")
-  example = dspy.InputField(desc="an example value for the field")
-  description = dspy.OutputField(desc="a short text only description of what the field contains")
+class DescriptionSignature(dspy.Signature):
+    field_name = dspy.InputField(desc="name of a field")
+    example = dspy.InputField(desc="an example value for the field")
+    description = dspy.OutputField(desc="a short text only description of what the field contains")
+
 
 class SyntheticDataGenerator:
     def __init__(self, schema_class: Optional[BaseModel] = None, examples: Optional[List[dspy.Example]] = None):
         self.schema_class = schema_class
         self.examples = examples
 
     def generate(self, sample_size: int) -> List[dspy.Example]:
+        """Generate synthetic examples.
+
+        Args:
+            sample_size (int): number of examples to generate
+        Raises:
+            ValueError: either a schema_class or examples should be provided
+        Returns:
+            List[dspy.Example]: list of synthetic examples generated
+        """
         if not self.schema_class and not self.examples:
             raise ValueError("Either a schema_class or examples must be provided.")
         if self.examples and len(self.examples) >= sample_size:
-            print("No additional data generation needed.")
+            logging.info("No additional data generation needed.")
             return self.examples[:sample_size]
 
         additional_samples_needed = sample_size - (len(self.examples) if self.examples else 0)
         generated_examples = self._generate_additional_examples(additional_samples_needed)
 
         return self.examples + generated_examples if self.examples else generated_examples
 
     def _define_or_infer_fields(self):
+        """Define fields to generate if a schema class is provided.
+        Infer fields to generate if an inital sample of examples is provided.
+
+        Returns:
+            dict: dictionary of fields to generate
+        """  # noqa: D205
         if self.schema_class:
             data_schema = self.schema_class.model_json_schema()
             properties = data_schema['properties']
         elif self.examples:
             inferred_schema = self.examples[0].__dict__['_store']
-            descriptor = dspy.Predict(descriptionSignature)
+            descriptor = dspy.Predict(DescriptionSignature)
             properties = {field: {'description': str((descriptor(field_name=field, example=str(inferred_schema[field]))).description)}
                           for field in inferred_schema.keys()}
         else:
             properties = {}
         return properties
 
     def _generate_additional_examples(self, additional_samples_needed: int) -> List[dspy.Example]:
+        """Generate additional examples if needed.
+
+        Args:
+            additional_samples_needed (int): the difference between the desired
+            number of examples and the current number of examples
+        Returns:
+            List[dspy.Example]: list of synthetic examples
+        """
         properties = self._define_or_infer_fields()
         class_name = f"{self.schema_class.__name__ if self.schema_class else 'Inferred'}Signature"
         fields = self._prepare_fields(properties)
 
         signature_class = type(class_name, (dspy.Signature,), fields)
         generator = dspy.Predict(signature_class, n=additional_samples_needed)
         response = generator(sindex=str(random.randint(1, additional_samples_needed)))
 
         return [dspy.Example({field_name: getattr(completion, field_name) for field_name in properties.keys()})
                 for completion in response.completions]
 
     def _prepare_fields(self, properties) -> dict:
+        """Prepare fields to generate in an appropriate format."""
         return {
             '__doc__': f"Generates the following outputs: {{{', '.join(properties.keys())}}}.",
             'sindex': dspy.InputField(desc="a random string"),
             **{field_name: dspy.OutputField(desc=properties[field_name].get('description', 'No description'))
                for field_name in properties.keys()},
         }
```

### Comparing `dspy-ai-2.4.7/dspy/functional/functional.py` & `dspy-ai-2.4.9/dspy/functional/functional.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 import inspect
 import json
+import textwrap
 import typing
-from typing import Annotated, List, Tuple  # noqa: UP035
+from typing import Annotated, List, Tuple, Union  # noqa: UP035
 
 import pydantic
 import ujson
+from pydantic.fields import FieldInfo
 
 import dspy
 from dsp.templates import passages2text
 from dspy.primitives.prediction import Prediction
 from dspy.signatures.signature import ensure_signature, make_signature
 
 
-def predictor(func) -> dspy.Module:
-    """Decorator that creates a predictor module based on the provided function."""
-    signature = _func_to_signature(func)
-    *_, output_key = signature.output_fields.keys()
-    return _StripOutput(TypedPredictor(signature), output_key)
-
-
-def cot(func) -> dspy.Module:
-    """Decorator that creates a chain of thought module based on the provided function."""
-    signature = _func_to_signature(func)
-    *_, output_key = signature.output_fields.keys()
-    return _StripOutput(TypedChainOfThought(signature), output_key)
+def predictor(*args, **kwargs):
+    def _predictor(func) -> dspy.Module:
+        """Decorator that creates a predictor module based on the provided function."""
+        signature = _func_to_signature(func)
+        *_, output_key = signature.output_fields.keys()
+        return _StripOutput(TypedPredictor(signature, **kwargs), output_key)
+
+    # if we have only a single callable argument, the decorator was invoked with no key word arguments
+    #  so we just return the wrapped function 
+    if len(args) == 1 and callable(args[0]) and len(kwargs) == 0:
+        return _predictor(args[0])
+    return _predictor
+
+
+def cot(*args, **kwargs):
+    def _cot(func) -> dspy.Module:
+        """Decorator that creates a chain of thought module based on the provided function."""
+        signature = _func_to_signature(func)
+        *_, output_key = signature.output_fields.keys()
+        return _StripOutput(TypedChainOfThought(signature, **kwargs), output_key)
+
+    # if we have only a single callable argument, the decorator was invoked with no key word arguments
+    #  so we just return the wrapped function 
+    if len(args) == 1 and callable(args[0]) and len(kwargs) == 0:
+        return _cot(args[0])
+    return _cot
 
 
 class _StripOutput(dspy.Module):
     def __init__(self, predictor, output_key):
         super().__init__()
         self.predictor = predictor
         self.output_key = output_key
@@ -47,47 +63,57 @@
         super().__init__()
         for name in dir(self):
             attr = getattr(self, name)
             if isinstance(attr, dspy.Module):
                 self.__dict__[name] = attr.copy()
 
 
-def TypedChainOfThought(signature, max_retries=3) -> dspy.Module:  # noqa: N802
+def TypedChainOfThought(signature, instructions=None, reasoning=None, *, max_retries=3) -> dspy.Module:  # noqa: N802
     """Just like TypedPredictor, but adds a ChainOfThought OutputField."""
-    signature = ensure_signature(signature)
+    signature = ensure_signature(signature, instructions)
     output_keys = ", ".join(signature.output_fields.keys())
+
+    DEFAULT_RATIONALE = dspy.OutputField(
+        prefix="Reasoning: Let's think step by step in order to",
+        desc="${produce the " + output_keys + "}. We ...",
+    )
+    reasoning = reasoning or DEFAULT_RATIONALE
+
     return TypedPredictor(
         signature.prepend(
             "reasoning",
-            dspy.OutputField(
-                prefix="Reasoning: Let's think step by step in order to",
-                desc="${produce the " + output_keys + "}. We ...",
-            ),
+            reasoning,
         ),
         max_retries=max_retries,
     )
 
 
 class TypedPredictor(dspy.Module):
-    def __init__(self, signature, max_retries=3, wrap_json=False):
+    def __init__(self, signature, instructions=None, *, max_retries=3, wrap_json=False, explain_errors=False):
         """Like dspy.Predict, but enforces type annotations in the signature.
 
         Args:
             signature: The signature of the module. Can use type annotations.
             max_retries: The number of times to retry the prediction if the output is invalid.
             wrap_json: If True, json objects in the input will be wrapped in ```json ... ```
         """
         super().__init__()
-        self.signature = ensure_signature(signature)
+        self.signature = ensure_signature(signature, instructions)
         self.predictor = dspy.Predict(signature)
         self.max_retries = max_retries
         self.wrap_json = wrap_json
+        self.explain_errors = explain_errors
 
     def copy(self) -> "TypedPredictor":
-        return TypedPredictor(self.signature, self.max_retries, self.wrap_json)
+        return TypedPredictor(
+            self.signature,
+            max_retries=self.max_retries,
+            wrap_json=self.wrap_json,
+            explain_errors=self.explain_errors,
+        )
 
     def __repr__(self):
         """Return a string representation of the TypedPredictor object."""
         return f"TypedPredictor({self.signature})"
 
     def _make_example(self, type_) -> str:
         # Note: DSPy will cache this call so we only pay the first time TypedPredictor is called.
@@ -108,14 +134,71 @@
         return json_object
         # TODO: Another fun idea is to only (but automatically) do this if the output fails.
         # We could also have a more general "suggest solution" prompt that tries to fix the output
         # More directly.
         # TODO: Instead of using a language model to create the example, we can also just use a
         # library like https://pypi.org/project/polyfactory/ that's made exactly to do this.
 
+    def _format_error(
+        self,
+        error: Exception,
+        task_description: Union[str, FieldInfo],
+        model_output: str,
+        lm_explain: bool,
+    ) -> str:
+        if isinstance(error, pydantic.ValidationError):
+            errors = []
+            for e in error.errors():
+                fields = ", ".join(map(str, e["loc"]))
+                errors.append(f"{e['msg']}: {fields} (error type: {e['type']})")
+            error_text = "; ".join(errors)
+        else:
+            error_text = repr(error)
+
+        if self.explain_errors and lm_explain:
+            if isinstance(task_description, FieldInfo):
+                args = task_description.json_schema_extra
+                task_description = args["prefix"] + " " + args["desc"]
+            return (
+                error_text
+                + "\n"
+                + self._make_explanation(
+                    task_description=task_description,
+                    model_output=model_output,
+                    error=error_text,
+                )
+            )
+
+        return error_text
+
+    def _make_explanation(self, task_description: str, model_output: str, error: str) -> str:
+        class Signature(dspy.Signature):
+            __doc__ = textwrap.dedent(
+                """
+                I gave my language model a task, but it failed. Figure out what went wrong,
+                and write instructions to help it avoid the error next time.""",
+            )
+
+            task_description: str = dspy.InputField(desc="What I asked the model to do")
+            language_model_output: str = dspy.InputField(desc="The output of the model")
+            error: str = dspy.InputField(desc="The validation error trigged by the models output")
+            explanation: str = dspy.OutputField(desc="Explain what the model did wrong")
+            advice: str = dspy.OutputField(
+                desc="Instructions for the model to do better next time. A single paragraph.",
+            )
+
+        # TODO: We could also try repair the output here. For example, if the output is a float, but the
+        # model returned a "float + explanation", the repair could be to remove the explanation.
+
+        return dspy.Predict(Signature)(
+            task_description=task_description,
+            language_model_output=model_output,
+            error=error,
+        ).advice
+
     def _prepare_signature(self) -> dspy.Signature:
         """Add formats and parsers to the signature fields, based on the type annotations of the fields."""
         signature = self.signature
         for name, field in self.signature.fields.items():
             is_output = field.json_schema_extra["__dspy_field_type"] == "output"
             type_ = field.annotation
             if is_output:
@@ -217,15 +300,21 @@
                 parsed = {}
                 for name, field in signature.output_fields.items():
                     try:
                         value = completion[name]
                         parser = field.json_schema_extra.get("parser", lambda x: x)
                         parsed[name] = parser(value)
                     except (pydantic.ValidationError, ValueError) as e:
-                        errors[name] = _format_error(e)
+                        errors[name] = self._format_error(
+                            e,
+                            signature.fields[name],
+                            value,
+                            lm_explain=try_i + 1 < self.max_retries,
+                        )
+
                         # If we can, we add an example to the error message
                         current_desc = field.json_schema_extra.get("desc", "")
                         i = current_desc.find("JSON Schema: ")
                         if i == -1:
                             continue  # Only add examples to JSON objects
                         suffix, current_desc = current_desc[i:], current_desc[:i]
                         prefix = "You MUST use this format: "
@@ -243,15 +332,23 @@
                     break
                 # Instantiate the actual signature with the parsed values.
                 # This allow pydantic to validate the fields defined in the signature.
                 try:
                     _ = self.signature(**kwargs, **parsed)
                     parsed_results.append(parsed)
                 except pydantic.ValidationError as e:
-                    errors["general"] = _format_error(e)
+                    errors["general"] = self._format_error(
+                        e,
+                        signature.instructions,
+                        "\n\n".join(
+                            "> " + field.json_schema_extra["prefix"] + " " + completion[name]
+                            for name, field in signature.output_fields.items()
+                        ),
+                        lm_explain=try_i + 1 < self.max_retries,
+                    )
             if errors:
                 # Add new fields for each error
                 for name, error in errors.items():
                     modified_kwargs[f"error_{name}_{try_i}"] = error
                     if name == "general":
                         error_prefix = "General:"
                     else:
@@ -271,24 +368,14 @@
                 )
         raise ValueError(
             "Too many retries trying to get the correct output format. " + "Try simplifying the requirements.",
             errors,
         )
 
 
-def _format_error(error: Exception):
-    if isinstance(error, pydantic.ValidationError):
-        errors = []
-        for e in error.errors():
-            fields = ", ".join(map(str, e["loc"]))
-            errors.append(f"{e['msg']}: {fields} (error type: {e['type']})")
-        return "; ".join(errors)
-    return repr(error)
-
-
 def _func_to_signature(func):
     """Make a dspy.Signature based on a function definition."""
     sig = inspect.signature(func)
     annotations = typing.get_type_hints(func, include_extras=True)
     output_key = func.__name__
     instructions = func.__doc__
     fields = {}
```

### Comparing `dspy-ai-2.4.7/dspy/predict/aggregation.py` & `dspy-ai-2.4.9/dspy/predict/aggregation.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/predict/chain_of_thought.py` & `dspy-ai-2.4.9/dspy/predict/chain_of_thought.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/predict/chain_of_thought_with_hint.py` & `dspy-ai-2.4.9/dspy/predict/chain_of_thought_with_hint.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/predict/knn.py` & `dspy-ai-2.4.9/dspy/predict/knn.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/predict/langchain.py` & `dspy-ai-2.4.9/dspy/predict/langchain.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/predict/multi_chain_comparison.py` & `dspy-ai-2.4.9/dspy/predict/multi_chain_comparison.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/predict/predict.py` & `dspy-ai-2.4.9/dspy/predict/predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import random
 
+from pydantic import BaseModel
+
 import dsp
 from dspy.predict.parameter import Parameter
 from dspy.primitives.prediction import Prediction
 from dspy.signatures.signature import ensure_signature, signature_to_template
 
 
 class Predict(Parameter):
@@ -16,17 +18,27 @@
     def reset(self):
         self.lm = None
         self.traces = []
         self.train = []
         self.demos = []
 
     def dump_state(self):
-        state_keys = ["lm", "traces", "train", "demos"]
+        state_keys = ["lm", "traces", "train"]
         state = {k: getattr(self, k) for k in state_keys}
 
+        state["demos"] = []
+        for demo in self.demos:
+            demo = demo.copy()
+
+            for field in demo:
+                if isinstance(demo[field], BaseModel):
+                    demo[field] = demo[field].model_dump_json()
+
+            state["demos"].append(demo)
+
         # Cache the signature instructions and the last field's name.
         state["signature_instructions"] = self.signature.instructions
 
         *_, last_key = self.signature.fields.keys()
         state["signature_prefix"] = self.signature.fields[last_key].json_schema_extra["prefix"]
 
         return state
@@ -61,15 +73,15 @@
 
         # If temperature is 0.0 but its n > 1, set temperature to 0.7.
         temperature = config.get("temperature")
         temperature = lm.kwargs["temperature"] if temperature is None else temperature
 
         num_generations = config.get("n")
         if num_generations is None:
-            num_generations = lm.kwargs.get("n", lm.kwargs.get("num_generations", None))
+            num_generations = lm.kwargs.get("n", lm.kwargs.get("num_generations", 1))
 
         if (temperature is None or temperature <= 0.15) and num_generations > 1:
             config["temperature"] = 0.7
             # print(f"#> Setting temperature to 0.7 since n={num_generations} and prior temperature={temperature}.")
 
         # All of the other kwargs are presumed to fit a prefix of the signature.
         # That is, they are input variables for the bottom most generation, so
```

### Comparing `dspy-ai-2.4.7/dspy/predict/program_of_thought.py` & `dspy-ai-2.4.9/dspy/predict/program_of_thought.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 from dspy.signatures.signature import ensure_signature
 
 from ..primitives.program import Module
 from ..primitives.python_interpreter import CodePrompt, PythonInterpreter
 
 
 class ProgramOfThought(Module):
-    def __init__(self, signature, max_iters=3):
+    def __init__(self, signature, max_iters=3, import_white_list=None):
         super().__init__()
         self.signature = signature = ensure_signature(signature)
         self.max_iters = max_iters
+        self.import_white_list = import_white_list
 
         self.input_fields = signature.input_fields
         self.output_fields = signature.output_fields
 
+        assert len(self.output_fields) == 1, "PoT only supports one output field."
+
+        self.output_field_name = next(iter(self.output_fields))
         inputs_ = ", ".join(
             [f"`{field_name}`" for field_name in self.input_fields.keys()],
         )
-        outputs_ = ", ".join(
-            [f"`{field_name}`" for field_name in self.output_fields.keys()],
-        )
+        outputs_ = f"`{self.output_field_name}`"
 
         assert len(self.output_fields) == 1, "PoT only supports one output field."
 
         instr = []
         instr.append(
             f"You will be given {inputs_} and you will respond with {outputs_}.",
         )
@@ -51,15 +53,14 @@
         )
         self.generate_answer = dspy.ChainOfThought(
             dspy.Signature(
                 self._generate_signature("answer").fields,
                 self._generate_instruction("answer"),
             ),
         )
-
     def _generate_signature(self, mode):
         signature_dict = dict(self.input_fields)
         fields_for_mode = {
             "generate": {
                 "generated_code": dspy.OutputField(
                     prefix="Code:",
                     desc="python code that answers the question",
@@ -88,51 +89,47 @@
                     desc="python code that answers the question",
                     format=str,
                 ),
                 "code_output": dspy.InputField(
                     prefix="Code Output:",
                     desc="output of previously-generated python code",
                 ),
-                "answer": self.signature.fields["answer"],
+                self.output_field_name: self.signature.fields[self.output_field_name],
             },
         }
         signature_dict.update(fields_for_mode[mode])
         return dspy.Signature(signature_dict)
 
     def _generate_instruction(self, mode):
         mode_inputs = ", ".join(
             [
                 f"`{field_name}`"
                 for field_name in self._generate_signature(mode).input_fields
             ],
         )
-        mode_outputs = ", ".join(
-            [
-                f"`{field_name}`"
-                for field_name in self._generate_signature(mode).output_fields
-            ],
-        )
+        mode_outputs = f"`{self.output_field_name}`"
         if mode == "generate":
             instr = [
                 f"You will be given {mode_inputs} and you will respond with {mode_outputs}.",
                 f"Generating executable Python code that programmatically computes the correct {mode_outputs}.",
                 f"After you're done with the computation, make sure the last line in your code evaluates to the correct value for {mode_outputs}.",
             ]
         elif mode == "regenerate":
             instr = [
                 f"You are given {mode_inputs} due to an error in previous code.",
-                f"Your task is to correct the error and provide the new {mode_outputs}.",
+                "Your task is to correct the error and provide the new `generated_code`.",
             ]
         else:  # mode == 'answer'
             instr = [
                 f"Given the final code {mode_inputs}, provide the final {mode_outputs}.",
             ]
 
         return "\n".join(instr)
 
+
     def parse_code(self, code_data):
         code = (
             code_data.get("generated_code", "").split("---", 1)[0].split("\n\n\n", 1)[0]
         )
         code_match = re.search(r"```python[ \n](.*?)[ \n]```?", code, re.DOTALL)
         code_block = (code_match.group(1) if code_match else code).replace("\\n", "\n")
         if not code_block:
@@ -152,36 +149,37 @@
             )
         return code_block, None
 
     def execute_code(self, code):
         if not code:
             return code, None, "Error: Empty code before execution."
         code_prompt = CodePrompt(code, code_type="python")
-        interpreter = PythonInterpreter(action_space={"print": print})
+        interpreter = PythonInterpreter(action_space={"print": print}, import_white_list=self.import_white_list)
         try:
             output = str(code_prompt.execute(interpreter=interpreter)[0])
+            print
             return code, output, None
         except Exception as e:
             return code, None, str(e)
-
     def forward(self, **kwargs):
-        code_data = self.code_generate(question=kwargs["question"])
+        input_kwargs = {
+            field_name: kwargs[field_name] for field_name in self.input_fields
+        }
+        code_data = self.code_generate(**input_kwargs)
         parsed_code, error = self.parse_code(code_data)
         # FIXME: Don't try to execute the code if it didn't parse
         code, output, error = self.execute_code(parsed_code)
         hop = 0
         while hop < self.max_iters and error:
             print("Error in code execution")
-            code_data = self.code_regenerate(
-                question=kwargs["question"], previous_code=code, error=error,
-            )
+            input_kwargs.update({"previous_code": code, "error": error})
+            code_data = self.code_regenerate(**input_kwargs)
             parsed_code, error = self.parse_code(code_data)
             # FIXME: Don't try to execute the code if it didn't parse
             code, output, error = self.execute_code(parsed_code)
             hop += 1
             if hop == self.max_iters:
                 print("Max hops reached. Error persists.")
                 return None
-        answer_gen_result = self.generate_answer(
-            question=kwargs["question"], final_generated_code=code, code_output=output,
-        )
-        return answer_gen_result
+        input_kwargs.update({"final_generated_code": code, "code_output": output})
+        answer_gen_result = self.generate_answer(**input_kwargs)
+        return answer_gen_result
```

### Comparing `dspy-ai-2.4.7/dspy/predict/react.py` & `dspy-ai-2.4.9/dspy/predict/react.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from ..primitives.program import Module
 from .predict import Predict
 
 # TODO: Simplify a lot.
 # TODO: Divide Action and Action Input like langchain does for ReAct.
 
+# TODO: There's a lot of value in having a stopping condition in the LM calls at `\n\nObservation:`
+
 
 class ReAct(Module):
     def __init__(self, signature, max_iters=5, num_results=3, tools=None):
         super().__init__()
         self.signature = signature = ensure_signature(signature)
         self.max_iters = max_iters
 
@@ -87,33 +89,32 @@
             action = output[f"Action_{hop+1}"]
             action_name, action_val = action.strip().split("\n")[0].split("[", 1)
             action_val = action_val.rsplit("]", 1)[0]
 
             if action_name == "Finish":
                 return action_val
 
-            try:
-                output[f"Observation_{hop+1}"] = self.tools[action_name](action_val).passages
-            except AttributeError:
-                # Handle the case where 'passages' attribute is missing
-                # TODO: This is a hacky way to handle this. Need to fix this.
-                output[f"Observation_{hop+1}"] = self.tools[action_name](action_val)
+            result = self.tools[action_name](action_val)
+            # Handle the case where 'passages' attribute is missing
+            output[f"Observation_{hop+1}"] = getattr(result, "passages", result)
 
-        except Exception as e:
+        except Exception:
             output[f"Observation_{hop+1}"] = (
                 "Failed to parse action. Bad formatting or incorrect action name."
             )
-            raise e
+            # raise e
 
     def forward(self, **kwargs):
         args = {key: kwargs[key] for key in self.input_fields.keys() if key in kwargs}
 
         for hop in range(self.max_iters):
             # with dspy.settings.context(show_guidelines=(i <= 2)):
             output = self.react[hop](**args)
 
             if action_val := self.act(output, hop):
                 break
             args.update(output)
 
+        observations = [args[key] for key in args if key.startswith("Observation")]
+        
         # assumes only 1 output field for now - TODO: handling for multiple output fields
-        return dspy.Prediction(**{list(self.output_fields.keys())[0]: action_val or ""})
+        return dspy.Prediction(observations=observations, **{list(self.output_fields.keys())[0]: action_val or ""})
```

### Comparing `dspy-ai-2.4.7/dspy/predict/retry.py` & `dspy-ai-2.4.9/dspy/predict/retry.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,25 +28,31 @@
             desc="Some instructions you must satisfy",
             format=str,
         ))
 
         return signature
 
     def forward(self, *, past_outputs, **kwargs):
+        # Take into account the possible new signature, as in TypedPredictor
+        new_signature = kwargs.pop("new_signature", None)
+        if new_signature:
+            self.original_signature = new_signature
+            self.new_signature = self._create_new_signature(self.original_signature)
+
         # Convert the dict past_outputs={"answer": ...} to kwargs
         # {past_answer=..., ...}
         for key, value in past_outputs.items():
             past_key = f"past_{key}"
             if past_key in self.new_signature.input_fields:
                 kwargs[past_key] = value
         # Tell the wrapped module to use the new signature.
         # Note: This only works if the wrapped module is a Predict or ChainOfThought.
         kwargs["new_signature"] = self.new_signature
         return self.original_forward(**kwargs)
-    
+
     def __call__(self, **kwargs):
         cached_kwargs = copy.deepcopy(kwargs)
         kwargs["_trace"] = False
         kwargs.setdefault("demos", self.demos if self.demos is not None else [])
 
         # perform backtracking
         if dspy.settings.backtrack_to == self:
@@ -55,14 +61,14 @@
             pred = self.forward(**kwargs)
         else:
             pred = self.module(**kwargs)
 
         # now pop multiple reserved keys
         # NOTE(shangyin) past_outputs seems not useful to include in demos,
         # therefore dropped
-        for key in ["_trace", "demos", "signature", "config", "lm", "past_outputs"]:
+        for key in ["_trace", "demos", "signature", "new_signature", "config", "lm", "past_outputs"]:
             kwargs.pop(key, None)
 
         if dsp.settings.trace is not None:
             trace = dsp.settings.trace
             trace.append((self, {**kwargs}, pred))
         return pred
```

### Comparing `dspy-ai-2.4.7/dspy/primitives/assertions.py` & `dspy-ai-2.4.9/dspy/primitives/assertions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,17 @@
 import inspect
-import logging
 import uuid
 from typing import Any
 
 import dsp
 import dspy
 
 #################### Assertion Helpers ####################
 
 
-def setup_logger():
-    logger = logging.getLogger(__name__)
-    logger.setLevel(logging.DEBUG)
-
-    fileHandler = logging.FileHandler("assertion.log")
-    fileHandler.setLevel(logging.DEBUG)
-
-    formatter = logging.Formatter(
-        "%(asctime)s - %(name)s - %(levelname)s - %(message)s",
-    )
-    fileHandler.setFormatter(formatter)
-
-    logger.addHandler(fileHandler)
-
-    return logger
-
-
-logger = setup_logger()
-
-
 def _build_error_msg(feedback_msgs):
     """Build an error message from a list of feedback messages."""
     return "\n".join([msg for msg in feedback_msgs])
 
 
 #################### Assertion Exceptions ####################
 
@@ -75,17 +54,20 @@
         self.is_metric = is_metric
 
 
 #################### Assertion Primitives ####################
 
 
 class Constraint:
-
     def __init__(
-        self, result: bool, msg: str = "", target_module=None, is_metric: bool = False,
+        self,
+        result: bool,
+        msg: str = "",
+        target_module=None,
+        is_metric: bool = False,
     ):
         self.id = str(uuid.uuid4())
         self.result = result
         self.msg = msg
         self.target_module = target_module
         self.is_metric = is_metric
 
@@ -96,18 +78,18 @@
     """DSPy Assertion"""
 
     def __call__(self) -> bool:
         if isinstance(self.result, bool):
             if self.result:
                 return True
             elif dspy.settings.bypass_assert:
-                logger.error(f"AssertionError: {self.msg}")
+                dspy.logger.error(f"AssertionError: {self.msg}")
                 return True
             else:
-                logger.error(f"AssertionError: {self.msg}")
+                dspy.logger.error(f"AssertionError: {self.msg}")
                 raise DSPyAssertionError(
                     id=self.id,
                     msg=self.msg,
                     target_module=self.target_module,
                     state=dsp.settings.trace,
                     is_metric=self.is_metric,
                 )
@@ -119,18 +101,18 @@
     """DSPy Suggestion"""
 
     def __call__(self) -> Any:
         if isinstance(self.result, bool):
             if self.result:
                 return True
             elif dspy.settings.bypass_suggest:
-                logger.error(f"SuggestionFailed: {self.msg}")
+                dspy.logger.error(f"SuggestionFailed: {self.msg}")
                 return True
             else:
-                logger.error(f"SuggestionFailed: {self.msg}")
+                dspy.logger.error(f"SuggestionFailed: {self.msg}")
                 raise DSPySuggestionError(
                     id=self.id,
                     msg=self.msg,
                     target_module=self.target_module,
                     state=dsp.settings.trace,
                     is_metric=self.is_metric,
                 )
@@ -226,19 +208,15 @@
                     }
 
                 # if last backtrack: ignore suggestion errors
                 if i == max_backtracks:
                     if isinstance(current_error, DSPyAssertionError):
                         raise current_error
                     dsp.settings.trace.clear()
-                    result = (
-                        bypass_suggest_handler(func)(*args, **kwargs)
-                        if bypass_suggest
-                        else None
-                    )
+                    result = bypass_suggest_handler(func)(*args, **kwargs) if bypass_suggest else None
                     break
                 else:
                     try:
                         dsp.settings.trace.clear()
                         result = func(*args, **kwargs)
                         break
                     except (DSPySuggestionError, DSPyAssertionError) as e:
@@ -259,49 +237,48 @@
 
                         if dsp.settings.trace:
                             if error_target_module:
                                 for i in range(len(dsp.settings.trace) - 1, -1, -1):
                                     trace_element = dsp.settings.trace[i]
                                     mod = trace_element[0]
                                     if mod.signature == error_target_module:
+                                        error_state = e.state[i]
                                         dspy.settings.backtrack_to = mod
                                         break
                             else:
                                 dspy.settings.backtrack_to = dsp.settings.trace[-1][0]
 
                             if dspy.settings.backtrack_to is None:
-                                logger.error("Specified module not found in trace")
+                                dspy.logger.error("Specified module not found in trace")
 
                             # save unique feedback message for predictor
-                            if (
-                                error_msg
-                                not in dspy.settings.predictor_feedbacks.setdefault(
-                                    dspy.settings.backtrack_to, [],
-                                )
+                            if error_msg not in dspy.settings.predictor_feedbacks.setdefault(
+                                dspy.settings.backtrack_to,
+                                [],
                             ):
-                                dspy.settings.predictor_feedbacks[
-                                    dspy.settings.backtrack_to
-                                ].append(error_msg)
+                                dspy.settings.predictor_feedbacks[dspy.settings.backtrack_to].append(error_msg)
 
                             # assert isinstance(error_state[0].signature, dspy.Signature)
                             output_fields = error_state[0].signature.output_fields
                             past_outputs = {}
                             for field_name in output_fields.keys():
                                 past_outputs[field_name] = getattr(
-                                    error_state[2], field_name, None,
+                                    error_state[2],
+                                    field_name,
+                                    None,
                                 )
 
                             # save latest failure trace for predictor per suggestion
                             error_ip = error_state[1]
                             error_op = error_state[2].__dict__["_store"]
                             error_op.pop("_assert_feedback", None)
                             error_op.pop("_assert_traces", None)
 
                         else:
-                            logger.error(
+                            dspy.logger.error(
                                 "UNREACHABLE: No trace available, this should not happen. Is this run time?",
                             )
 
             return result
 
     return wrapper
 
@@ -320,25 +297,27 @@
     return forward
 
 
 default_assertion_handler = backtrack_handler
 
 
 def assert_transform_module(
-    module, assertion_handler=default_assertion_handler, **handler_args,
+    module,
+    assertion_handler=default_assertion_handler,
+    **handler_args,
 ):
     """
     Transform a module to handle assertions.
     """
     if not getattr(module, "forward", False):
         raise ValueError(
             "Module must have a forward method to have assertions handled.",
         )
     if getattr(module, "_forward", False):
-        logger.info(
+        dspy.logger.info(
             f"Module {module.__class__.__name__} already has a _forward method. Skipping...",
         )
         pass  # TODO warning: might be overwriting a previous _forward method
 
     module._forward = module.forward
     module.forward = handle_assert_forward(assertion_handler, **handler_args).__get__(
         module,
```

### Comparing `dspy-ai-2.4.7/dspy/primitives/box.py` & `dspy-ai-2.4.9/dspy/primitives/box.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/primitives/example.py` & `dspy-ai-2.4.9/dspy/primitives/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         d = {k: v for k, v in self._store.items() if not k.startswith('dspy_')}
         return f"Example({d})" + f" (input_keys={self._input_keys})"
     
     def __str__(self):
         return self.__repr__()
     
     def __eq__(self, other):
-        return self._store == other._store
+        return isinstance(other, Example) and self._store == other._store
     
     def __hash__(self):
         return hash(tuple(self._store.items()))
 
     def keys(self, include_dspy=False):
         return [k for k in self._store.keys() if not k.startswith('dspy_') or include_dspy]
```

### Comparing `dspy-ai-2.4.7/dspy/primitives/prediction.py` & `dspy-ai-2.4.9/dspy/primitives/prediction.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/primitives/program.py` & `dspy-ai-2.4.9/dspy/primitives/program.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/primitives/python_interpreter.py` & `dspy-ai-2.4.9/dspy/primitives/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/retrieve/chromadb_rm.py` & `dspy-ai-2.4.9/dspy/retrieve/chromadb_rm.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,17 +22,14 @@
     from chromadb.api.types import (
         Embeddable,
         EmbeddingFunction,
     )
     from chromadb.config import Settings
     from chromadb.utils import embedding_functions
 except ImportError:
-    chromadb = None
-
-if chromadb is None:
     raise ImportError(
         "The chromadb library is required to use ChromadbRM. Install it with `pip install dspy-ai[chromadb]`",
     )
 
 
 class ChromadbRM(dspy.Retrieve):
     """
@@ -42,68 +39,87 @@
         - documents: The text of the passage
 
     Args:
         collection_name (str): chromadb collection name
         persist_directory (str): chromadb persist directory
         embedding_function (Optional[EmbeddingFunction[Embeddable]]): Optional function to use to embed documents. Defaults to DefaultEmbeddingFunction.
         k (int, optional): The number of top passages to retrieve. Defaults to 7.
+        client(Optional[chromadb.Client]): Optional chromadb client provided by user, default to None
 
     Returns:
         dspy.Prediction: An object containing the retrieved passages.
 
     Examples:
         Below is a code snippet that shows how to use this as the default retriever:
         ```python
         llm = dspy.OpenAI(model="gpt-3.5-turbo")
+        # using default chromadb client
         retriever_model = ChromadbRM('collection_name', 'db_path')
         dspy.settings.configure(lm=llm, rm=retriever_model)
         # to test the retriever with "my query"
         retriever_model("my query")
         ```
 
+        Use provided chromadb client
+        ```python
+        import chromadb
+        llm = dspy.OpenAI(model="gpt-3.5-turbo")
+        # say you have a chromadb running on a different port
+        client = chromadb.HttpClient(host='localhost', port=8889)
+        retriever_model = ChromadbRM('collection_name', 'db_path', client=client)
+        dspy.settings.configure(lm=llm, rm=retriever_model)
+        # to test the retriever with "my query"
+        retriever_model("my query")
+        ```
+
         Below is a code snippet that shows how to use this in the forward() function of a module
         ```python
         self.retrieve = ChromadbRM('collection_name', 'db_path', k=num_passages)
         ```
     """
 
     def __init__(
         self,
         collection_name: str,
         persist_directory: str,
         embedding_function: Optional[
             EmbeddingFunction[Embeddable]
         ] = ef.DefaultEmbeddingFunction(),
+        client: Optional[chromadb.Client] = None,
         k: int = 7,
     ):
-        self._init_chromadb(collection_name, persist_directory)
+        self._init_chromadb(collection_name, persist_directory, client=client)
         self.ef = embedding_function
 
         super().__init__(k=k)
 
     def _init_chromadb(
         self,
         collection_name: str,
         persist_directory: str,
+        client: Optional[chromadb.Client] = None,
     ) -> chromadb.Collection:
         """Initialize chromadb and return the loaded index.
 
         Args:
             collection_name (str): chromadb collection name
             persist_directory (str): chromadb persist directory
+            client (chromadb.Client): chromadb client provided by user
 
-
-        Returns:
+        Returns: collection per collection_name
         """
 
-        self._chromadb_client = chromadb.Client(
-            Settings(
-                persist_directory=persist_directory,
-                is_persistent=True,
-            ),
+        if client:
+            self._chromadb_client = client
+        else:
+            self._chromadb_client = chromadb.Client(
+                Settings(
+                    persist_directory=persist_directory,
+                    is_persistent=True,
+                ),
         )
         self._chromadb_collection = self._chromadb_client.get_or_create_collection(
             name=collection_name,
         )
 
     @backoff.on_exception(
         backoff.expo,
@@ -118,15 +134,15 @@
 
         Returns:
             List[List[float]]: List of embeddings corresponding to each query.
         """
         return self.ef(queries)
 
     def forward(
-        self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,
+        self, query_or_queries: Union[str, List[str]], k: Optional[int] = None, **kwargs,
     ) -> dspy.Prediction:
         """Search with db for self.k top passages for query
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
 
         Returns:
@@ -138,15 +154,15 @@
             else query_or_queries
         )
         queries = [q for q in queries if q]  # Filter empty queries
         embeddings = self._get_embeddings(queries)
 
         k = self.k if k is None else k
         results = self._chromadb_collection.query(
-            query_embeddings=embeddings, n_results=k,
+            query_embeddings=embeddings, n_results=k,**kwargs,
         )
 
         zipped_results = zip(
             results["ids"][0], 
             results["distances"][0], 
             results["documents"][0], 
             results["metadatas"][0])
```

### Comparing `dspy-ai-2.4.7/dspy/retrieve/clarifai_rm.py` & `dspy-ai-2.4.9/dspy/retrieve/clarifai_rm.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         header = {"Authorization": f"Key {self.pat}"}
         request = requests.get(hits.input.data.text.url, headers=header)
         request.encoding = request.apparent_encoding
         requested_text = request.text
         return requested_text
 
     def forward(
-        self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,
+        self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,**kwargs,
     ) -> dspy.Prediction:
         """Uses clarifai-python SDK search function and retrieves top_k similar passages for given query,
         Args:
              query_or_queries : single query or list of queries
              k : Top K relevant documents to return
 
         Returns:
@@ -81,15 +81,15 @@
             if isinstance(query_or_queries, str)
             else query_or_queries
         )
         passages = []
         queries = [q for q in queries if q]
 
         for query in queries:
-            search_response = self.clarifai_search.query(ranks=[{"text_raw": query}])
+            search_response = self.clarifai_search.query(ranks=[{"text_raw": query}],**kwargs)
 
             # Retrieve hits
             hits = [hit for data in search_response for hit in data.hits]
             with ThreadPoolExecutor(max_workers=10) as executor:
                 results = list(executor.map(self.retrieve_hits, hits))
             passages.extend(dotdict({"long_text": d}) for d in results)
```

### Comparing `dspy-ai-2.4.7/dspy/retrieve/databricks_rm.py` & `dspy-ai-2.4.9/dspy/retrieve/databricks_rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         self.databricks_index_name = databricks_index_name
         self.columns = columns
         self.filters_json = filters_json
         self.k = k
         self.docs_id_column_name = docs_id_column_name
         self.text_column_name = text_column_name
 
-    def forward(self, query: Union[str, List[float]], query_type: str = 'vector') -> dspy.Prediction:
+    def forward(self, query: Union[str, List[float]], query_type: str = 'text', filters_json: str = None) -> dspy.Prediction:
         """Search with Databricks Vector Search Client for self.k top results for query
 
         Args:
             query (Union[str, List[float]]): query to search for.
             query_type (str): 'vector' for Direct Vector Access Index and Delta Sync Index using self-managed vectors or 'text' for Delta Sync Index using model endpoint.
 
         Returns:
@@ -111,16 +111,17 @@
             payload["query_vector"] = query
         elif query_type == 'text':
             if not isinstance(query, str):
                 raise ValueError("Query must be a string for query_text")
             payload["query_text"] = query
         else:
             raise ValueError("Invalid query type specified. Use 'vector' or 'text'.")
-        if self.filters_json:
-            payload["filters_json"] = self.filters_json     
+
+        payload["filters_json"] = filters_json if filters_json else self.filters_json
+
         response = requests.post(
             f"{self.databricks_endpoint}/api/2.0/vector-search/indexes/{self.databricks_index_name}/query",
             json=payload,
             headers=headers,
         )
         results = response.json()
 
@@ -132,13 +133,15 @@
                 if col["name"] == self.docs_id_column_name:
                     if self.docs_id_column_name == 'metadata':
                         docs_dict = json.loads(val)
                         doc_ids.append(str(docs_dict["document_id"]))
                     else:
                         doc_ids.append(str(val))
                     text = val
+                if col["name"] == self.text_column_name:   
+                    text = val   
                 if col["name"] == 'score':
                     score = val
             docs[text] += score
 
         sorted_docs = sorted(docs.items(), key=lambda x: x[1], reverse=True)[:self.k]
         return Prediction(docs=[doc for doc, _ in sorted_docs], doc_ids = doc_ids)
```

### Comparing `dspy-ai-2.4.7/dspy/retrieve/deeplake_rm.py` & `dspy-ai-2.4.9/dspy/retrieve/deeplake_rm.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         texts = [t.replace("\n", " ") for t in texts]
         return [
             data["embedding"]
             for data in openai.Embedding.create(input=texts, model=model)["data"]
         ]
 
     def forward(
-        self, query_or_queries: Union[str, List[str]], k: Optional[int],
+        self, query_or_queries: Union[str, List[str]], k: Optional[int],**kwargs,
     ) -> dspy.Prediction:
         
         """Search with DeepLake for self.k top passages for query
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
             k (Optional[int]): The number of top passages to retrieve. Defaults to self.k.
@@ -102,15 +102,15 @@
 
         passages = defaultdict(float)
         #deeplake doesn't support batch querying, manually querying each query and storing them
         for query in queries:
             results = self._deeplake_client(
             path=self._deeplake_vectorstore_name,
             embedding_function=self.embedding_function,
-            ).search(query, k=k)
+            ).search(query, k=k,**kwargs)
 
             for score,text in zip(results.get('score',0.0),results.get('text',"")):
                 passages[text] += score
 
         sorted_passages = sorted(
             passages.items(), key=lambda x: x[1], reverse=True)[:k]
```

### Comparing `dspy-ai-2.4.7/dspy/retrieve/faiss_rm.py` & `dspy-ai-2.4.9/dspy/retrieve/faiss_rm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Retriever model for faiss: https://github.com/facebookresearch/faiss.
 Author: Jagane Sundar: https://github.com/jagane.
 """
 
-import logging
 from typing import Optional, Union
 
 import numpy as np
 
 import dspy
 from dsp.modules.sentence_vectorizer import SentenceTransformersVectorizer
 from dsp.utils import dotdict
@@ -77,41 +76,41 @@
         if vectorizer:
             self._vectorizer = vectorizer
         else:
             self._vectorizer = SentenceTransformersVectorizer()
         embeddings = self._vectorizer(document_chunks)
         xb = np.array(embeddings)
         d = len(xb[0])
-        logging.info(f"FaissRM: embedding size={d}")
+        dspy.logger.info(f"FaissRM: embedding size={d}")
         if len(xb) < 100:
             self._faiss_index = faiss.IndexFlatL2(d)
             self._faiss_index.add(xb)
         else:
             # if we have at least 100 vectors, we use Voronoi cells
             nlist = 100
             quantizer = faiss.IndexFlatL2(d)
             self._faiss_index = faiss.IndexIVFFlat(quantizer, d, nlist)
             self._faiss_index.train(xb)
             self._faiss_index.add(xb)
 
-        logging.info(f"{self._faiss_index.ntotal} vectors in faiss index")
+        dspy.logger.info(f"{self._faiss_index.ntotal} vectors in faiss index")
         self._document_chunks = document_chunks  # save the input document chunks
 
         super().__init__(k=k)
 
     def _dump_raw_results(self, queries, index_list, distance_list) -> None:
         for i in range(len(queries)):
             indices = index_list[i]
             distances = distance_list[i]
-            logging.debug(f"Query: {queries[i]}")
+            dspy.logger.debug(f"Query: {queries[i]}")
             for j in range(len(indices)):
-                logging.debug(f"    Hit {j} = {indices[j]}/{distances[j]}: {self._document_chunks[indices[j]]}")
+                dspy.logger.debug(f"    Hit {j} = {indices[j]}/{distances[j]}: {self._document_chunks[indices[j]]}")
         return
 
-    def forward(self, query_or_queries: Union[str, list[str]], k: Optional[int] = None) -> dspy.Prediction:
+    def forward(self, query_or_queries: Union[str, list[str]], k: Optional[int] = None, **kwargs) -> dspy.Prediction:
         """Search the faiss index for k or self.k top passages for query.
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
 
         Returns:
             dspy.Prediction: An object containing the retrieved passages.
@@ -123,15 +122,15 @@
         # For single query, just look up the top k passages
         if len(queries) == 1:
             distance_list, index_list = self._faiss_index.search(emb_npa, k or self.k)
             # self._dump_raw_results(queries, index_list, distance_list)
             passages = [(self._document_chunks[ind], ind) for ind in index_list[0]]
             return [dotdict({"long_text": passage[0], "index": passage[1]}) for passage in passages]
 
-        distance_list, index_list = self._faiss_index.search(emb_npa, (k or self.k) * 3)
+        distance_list, index_list = self._faiss_index.search(emb_npa, (k or self.k) * 3, **kwargs)
         # self._dump_raw_results(queries, index_list, distance_list)
         passage_scores = {}
         for emb in range(len(embeddings)):
             indices = index_list[emb]  # indices of neighbors for embeddings[emb] - this is an array of k*3 integers
             distances = distance_list[
                 emb
             ]  # distances of neighbors for embeddings[emb] - this is an array of k*3 floating point numbers
@@ -142,9 +141,14 @@
                     passage_scores[neighbor].append(distance)
                 else:
                     passage_scores[neighbor] = [distance]
         # Note re. sorting:
         # first degree sort: number of queries that got a hit with any particular document chunk. More
         # is a better match. This is len(queries)-len(x[1])
         # second degree sort: sum of the distances of each hit returned by faiss. Smaller distance is a better match
-        sorted_passages = sorted(passage_scores.items(), key=lambda x: (len(queries) - len(x[1]), sum(x[1])))[: k or self.k]
-        return [ dotdict({"long_text": self._document_chunks[passage_index], "index": passage_index}) for passage_index, _ in sorted_passages ]
+        sorted_passages = sorted(passage_scores.items(), key=lambda x: (len(queries) - len(x[1]), sum(x[1])))[
+            : k or self.k
+        ]
+        return [
+            dotdict({"long_text": self._document_chunks[passage_index], "index": passage_index})
+            for passage_index, _ in sorted_passages
+        ]
```

### Comparing `dspy-ai-2.4.7/dspy/retrieve/marqo_rm.py` & `dspy-ai-2.4.9/dspy/retrieve/marqo_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/retrieve/mongodb_atlas_rm.py` & `dspy-ai-2.4.9/dspy/retrieve/mongodb_atlas_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/retrieve/neo4j_rm.py` & `dspy-ai-2.4.9/dspy/retrieve/neo4j_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/retrieve/pinecone_rm.py` & `dspy-ai-2.4.9/dspy/retrieve/pinecone_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/retrieve/qdrant_rm.py` & `dspy-ai-2.4.9/dspy/retrieve/qdrant_rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         k: int = 3,
     ):
         self._qdrant_collection_name = qdrant_collection_name
         self._qdrant_client = qdrant_client
 
         super().__init__(k=k)
 
-    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int]) -> dspy.Prediction:
+    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,**kwargs) -> dspy.Prediction:
         """Search with Qdrant for self.k top passages for query
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
             k (Optional[int]): The number of top passages to retrieve. Defaults to self.k.
         Returns:
             dspy.Prediction: An object containing the retrieved passages.
@@ -67,15 +67,15 @@
             if isinstance(query_or_queries, str)
             else query_or_queries
         )
         queries = [q for q in queries if q]  # Filter empty queries
 
         k = k if k is not None else self.k
         batch_results = self._qdrant_client.query_batch(
-            self._qdrant_collection_name, query_texts=queries, limit=k)
+            self._qdrant_collection_name, query_texts=queries, limit=k,**kwargs)
 
         passages_scores = defaultdict(float)
         for batch in batch_results:
             for result in batch:
                 # If a passage is returned multiple times, the score is accumulated.
                 passages_scores[result.document] += result.score
```

### Comparing `dspy-ai-2.4.7/dspy/retrieve/retrieve.py` & `dspy-ai-2.4.9/dspy/retrieve/retrieve.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     def load_state(self, state):
         for name, value in state.items():
             setattr(self, name, value)
 
     def __call__(self, *args, **kwargs):
         return self.forward(*args, **kwargs)
 
-    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int] = None) -> Prediction:
+    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int] = None,**kwargs) -> Prediction:
         queries = [query_or_queries] if isinstance(query_or_queries, str) else query_or_queries
         queries = [query.strip().split('\n')[0].strip() for query in queries]
 
         # print(queries)
         # TODO: Consider removing any quote-like markers that surround the query too.
         k = k if k is not None else self.k
-        passages = dsp.retrieveEnsemble(queries, k=k)
+        passages = dsp.retrieveEnsemble(queries, k=k,**kwargs)
         return Prediction(passages=passages)
 
 # TODO: Consider doing Prediction.from_completions with the individual sets of passages (per query) too.
```

### Comparing `dspy-ai-2.4.7/dspy/retrieve/vectara_rm.py` & `dspy-ai-2.4.9/dspy/retrieve/vectara_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/retrieve/weaviate_rm.py` & `dspy-ai-2.4.9/dspy/retrieve/weaviate_rm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import List, Optional, Union
 
 import dspy
 from dsp.utils import dotdict
 
 try:
     import weaviate
+    import weaviate.classes as wvc
+    from weaviate.collections.classes.grpc import HybridFusion
 except ImportError:
     raise ImportError(
         "The 'weaviate' extra is required to use WeaviateRM. Install it with `pip install dspy-ai[weaviate]`",
     )
 
 
 class WeaviateRM(dspy.Retrieve):
@@ -18,14 +20,17 @@
     Assumes that a Weaviate collection has been created and populated with the following payload:
         - content: The text of the passage
 
     Args:
         weaviate_collection_name (str): The name of the Weaviate collection.
         weaviate_client (WeaviateClient): An instance of the Weaviate client.
         k (int, optional): The default number of top passages to retrieve. Defaults to 3.
+        weaviate_collection_text_key (str, optional): The key in the collection with the content. Defaults to content.
+        weaviate_alpha (float, optional): The alpha value for the hybrid query. Defaults to 0.5.
+        weaviate_fusion_type (wvc.HybridFusion, optional): The fusion type for the query. Defaults to RELATIVE_SCORE.
 
     Examples:
         Below is a code snippet that shows how to use Weaviate as the default retriver:
         ```python
         import weaviate
 
         llm = dspy.OpenAI(model="gpt-3.5-turbo")
@@ -40,24 +45,28 @@
         ```python
         self.retrieve = WeaviateRM("my_collection_name", weaviate_client=weaviate_client, k=num_passages)
         ```
     """
 
     def __init__(self, 
                  weaviate_collection_name: str, 
-                 weaviate_client: weaviate.Client, 
+                 weaviate_client: weaviate.WeaviateClient,
                  k: int = 3,
                  weaviate_collection_text_key: Optional[str] = "content",
+                 weaviate_alpha: Optional[float] = 0.5,
+                 weaviate_fusion_type: Optional[HybridFusion] = HybridFusion.RELATIVE_SCORE,
         ):
         self._weaviate_collection_name = weaviate_collection_name
         self._weaviate_client = weaviate_client
         self._weaviate_collection_text_key = weaviate_collection_text_key
+        self._weaviate_alpha = weaviate_alpha
+        self._weaviate_fusion_type = weaviate_fusion_type
         super().__init__(k=k)
 
-    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int]) -> dspy.Prediction:
+    def forward(self, query_or_queries: Union[str, List[str]], k: Optional[int] = None, **kwargs) -> dspy.Prediction:
         """Search with Weaviate for self.k top passages for query
 
         Args:
             query_or_queries (Union[str, List[str]]): The query or queries to search for.
             k (Optional[int]): The number of top passages to retrieve. Defaults to self.k.
         Returns:
             dspy.Prediction: An object containing the retrieved passages.
@@ -68,18 +77,22 @@
             [query_or_queries]
             if isinstance(query_or_queries, str)
             else query_or_queries
         )
         queries = [q for q in queries if q]
         passages = []
         for query in queries:
-            results = self._weaviate_client.query\
-                .get(self._weaviate_collection_name, [self._weaviate_collection_text_key])\
-                .with_hybrid(query=query)\
-                .with_limit(k)\
-                .do()
+            collection = self._weaviate_client.collections.get(self._weaviate_collection_name)
+            results = collection.query.hybrid(query=query,
+                                              limit=k,
+                                              alpha=self._weaviate_alpha,
+                                              fusion_type=self._weaviate_fusion_type,
+                                              return_metadata=wvc.query.MetadataQuery(
+                                                  distance=True, score=True),
+                                              **kwargs,
+                                              )
 
-            results = results["data"]["Get"][self._weaviate_collection_name]
-            parsed_results = [result[self._weaviate_collection_text_key] for result in results]
+            parsed_results = [result.properties[self._weaviate_collection_text_key] for result in results.objects]
             passages.extend(dotdict({"long_text": d}) for d in parsed_results)
 
+        # Return type not changed, needs to be a Prediction object. But other code will break if we change it.
         return passages
```

### Comparing `dspy-ai-2.4.7/dspy/retrieve/you_rm.py` & `dspy-ai-2.4.9/dspy/retrieve/you_rm.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/signatures/field.py` & `dspy-ai-2.4.9/dspy/signatures/field.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/signatures/signature.py` & `dspy-ai-2.4.9/dspy/signatures/signature.py`

 * *Files 7% similar despite different names*

```diff
@@ -202,19 +202,21 @@
     ""  # noqa: D419
 
     # Note: Don't put a docstring here, as it will become the default instructions
     # for any signature that doesn't define it's own instructions.
     pass
 
 
-def ensure_signature(signature: Union[str, Type[Signature]]) -> Signature:
+def ensure_signature(signature: Union[str, Type[Signature]], instructions=None) -> Signature:
     if signature is None:
         return None
     if isinstance(signature, str):
-        return Signature(signature)
+        return Signature(signature, instructions)
+    if instructions is not None:
+        raise ValueError("Don't specify instructions when initializing with a Signature")
     return signature
 
 
 def make_signature(
     signature: Union[str, Dict[str, Tuple[type, FieldInfo]]],
     instructions: str = None,
     signature_name: str = "StringSignature",
@@ -273,44 +275,39 @@
     )
 
 
 def _parse_signature(signature: str) -> Tuple[Type, Field]:
     if signature.count("->") != 1:
         raise ValueError(f"Invalid signature format: '{signature}', must contain exactly one '->'.")
 
+    inputs_str, outputs_str = signature.split("->")
+
     fields = {}
-    inputs_str, outputs_str = map(str.strip, signature.split("->"))
-    inputs = [v.strip() for v in inputs_str.split(",") if v.strip()]
-    outputs = [v.strip() for v in outputs_str.split(",") if v.strip()]
-    for name_type in inputs:
-        name, type_ = _parse_named_type_node(name_type)
+    for name, type_ in _parse_arg_string(inputs_str):
         fields[name] = (type_, InputField())
-    for name_type in outputs:
-        name, type_ = _parse_named_type_node(name_type)
+    for name, type_ in _parse_arg_string(outputs_str):
         fields[name] = (type_, OutputField())
 
     return fields
 
 
-def _parse_named_type_node(node, names=None) -> Any:
-    parts = node.split(":")
-    if len(parts) == 1:
-        return parts[0], str
-    name, type_str = parts
-    type_ = _parse_type_node(ast.parse(type_str), names)
-    return name, type_
+def _parse_arg_string(string: str, names=None) -> Dict[str, str]:
+    args = ast.parse("def f(" + string + "): pass").body[0].args.args
+    names = [arg.arg for arg in args]
+    types = [str if arg.annotation is None else _parse_type_node(arg.annotation) for arg in args]
+    return zip(names, types)
 
 
 def _parse_type_node(node, names=None) -> Any:
     """Recursively parse an AST node representing a type annotation.
 
     without using structural pattern matching introduced in Python 3.10.
     """
     if names is None:
-        names = {}
+        names = typing.__dict__
 
     if isinstance(node, ast.Module):
         body = node.body
         if len(body) != 1:
             raise ValueError(f"Code is not syntactically valid: {node}")
         return _parse_type_node(body[0], names)
 
@@ -321,24 +318,31 @@
     if isinstance(node, ast.Name):
         id_ = node.id
         if id_ in names:
             return names[id_]
         for type_ in [int, str, float, bool, list, tuple, dict]:
             if type_.__name__ == id_:
                 return type_
+        raise ValueError(f"Unknown name: {id_}")
 
-    elif isinstance(node, ast.Subscript):
+    if isinstance(node, ast.Subscript):
         base_type = _parse_type_node(node.value, names)
         arg_type = _parse_type_node(node.slice, names)
         return base_type[arg_type]
 
-    elif isinstance(node, ast.Tuple):
+    if isinstance(node, ast.Tuple):
         elts = node.elts
         return tuple(_parse_type_node(elt, names) for elt in elts)
 
+    if isinstance(node, ast.Call):
+        if node.func.id == "Field":
+            keys = [kw.arg for kw in node.keywords]
+            values = [kw.value.value for kw in node.keywords]
+            return Field(**dict(zip(keys, values)))
+
     raise ValueError(f"Code is not syntactically valid: {node}")
 
 
 def infer_prefix(attribute_name: str) -> str:
     """Infer a prefix from an attribute name."""
     # Convert camelCase to snake_case, but handle sequences of capital letters properly
     s1 = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", attribute_name)
```

### Comparing `dspy-ai-2.4.7/dspy/teleprompt/bootstrap.py` & `dspy-ai-2.4.9/dspy/teleprompt/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,17 @@
 
                 if example_idx not in bootstrapped:
                     success = self._bootstrap_one_example(example, round_idx)
 
                     if success:
                         bootstrapped[example_idx] = True
 
-        print(f"Bootstrapped {len(bootstrapped)} full traces after {example_idx+1} examples in round {round_idx}.")
+        dspy.logger.info(
+            f"Bootstrapped {len(bootstrapped)} full traces after {example_idx + 1} examples in round {round_idx}.",
+        )
 
         # Unbootstrapped training examples
 
         self.validation = [x for idx, x in enumerate(self.trainset) if idx not in bootstrapped]
         random.Random(0).shuffle(self.validation)
 
         self.validation = self.valset or self.validation
@@ -163,48 +165,47 @@
                     metric_val = self.metric(example, prediction, trace)
                     if self.metric_threshold:
                         success = metric_val >= self.metric_threshold
                     else:
                         success = metric_val
                 else:
                     success = True
-                # print(success, example, prediction)
         except Exception as e:
             success = False
             with self.error_lock:
                 self.error_count += 1
                 current_error_count = self.error_count
             if current_error_count >= self.max_errors:
                 raise e
-            print(f"Failed to run or to evaluate example {example} with {self.metric} due to {e}.")
+            dspy.logger.error(f"Failed to run or to evaluate example {example} with {self.metric} due to {e}.")
 
         if success:
             for step in trace:
                 predictor, inputs, outputs = step
 
                 if "dspy_uuid" in example:
                     demo = Example(augmented=True, dspy_uuid=example.dspy_uuid, **inputs, **outputs)
                 else:
                     # TODO: FIXME: This is a hack. RandomSearch will complain for now in this edge case.
                     demo = Example(augmented=True, **inputs, **outputs)
 
                 try:
                     predictor_name = self.predictor2name[id(predictor)]
-                except KeyError as e:
+                except KeyError:
                     continue  # FIXME: !
 
-                    # TODO: Look closer into this. It's a bit tricky to reproduce.
-                    print(f"Failed to find predictor {predictor} in {self.predictor2name}.")
-                    print(
-                        "Are you doing this in a notebook (Jupyter)? This might be caused by redefining values by rerunning cells.",
-                    )
-                    print("Try restarting the notebook, or open an issue.")
-                    raise KeyError(
-                        f"Failed to find predictor {id(predictor)} {predictor} in {self.predictor2name}.",
-                    ) from e
+                    # # TODO: Look closer into this. It's a bit tricky to reproduce.
+                    # print(f"Failed to find predictor {predictor} in {self.predictor2name}.")
+                    # print(
+                    #     "Are you doing this in a notebook (Jupyter)? This might be caused by redefining values by rerunning cells.",
+                    # )
+                    # print("Try restarting the notebook, or open an issue.")
+                    # raise KeyError(
+                    #     f"Failed to find predictor {id(predictor)} {predictor} in {self.predictor2name}.",
+                    # ) from e
 
                 name2traces[predictor_name].append(demo)
 
         return success
 
     def _train(self):
         rng = random.Random(0)
```

### Comparing `dspy-ai-2.4.7/dspy/teleprompt/copro_optimizer.py` & `dspy-ai-2.4.9/dspy/teleprompt/copro_optimizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 Note that this teleprompter takes in the following parameters:
 
 * prompt_model: The model used for prompt generation. When unspecified, defaults to the model set in settings (ie. dspy.settings.configure(lm=task_model)).
 * metric: The task metric used for optimization.
 * breadth: The number of new prompts to generate at each iteration. Default=10.
 * depth: The number of times we should ask our prompt model to generate new prompts, with the history of the past prompts as input. Default=3.
 * init_temperature: The temperature used to generate new prompts. Higher roughly equals more creative. Default=1.4.
-* verbose: Tells the method whether or not to print intermediate steps.
 * track_stats: Tells the method whether or not to track statistics about the optimization process.
                 If True, the method will track the following statistics:
                     * results_best: The min,max,avg,stddev of top 10 scores for each predictor at each depth.
                     * results_latest: The min,max,avg,stddev of newest prompt scores for each predictor at each depth.
                     * total_calls: The total number of calls to the task metric.
                 These statistics will be returned as attributes of the best program.
 """
@@ -59,27 +58,29 @@
     def __init__(
         self,
         prompt_model=None,
         metric=None,
         breadth=10,
         depth=3,
         init_temperature=1.4,
-        verbose=False,
         track_stats=False,
+        **_kwargs,
     ):
         if breadth <= 1:
             raise ValueError("Breadth must be greater than 1")
         self.metric = metric
         self.breadth = breadth
         self.depth = depth
         self.init_temperature = init_temperature
         self.prompt_model = prompt_model
-        self.verbose = verbose
         self.track_stats = track_stats
 
+        if "verbose" in _kwargs:
+            dspy.logger.warning("DeprecationWarning: 'verbose' has been deprecated. To see all information for debugging, use 'dspy.set_log_level('debug')'. In the future this will raise an error.")
+
     def _check_candidates_equal(self, candidate1, candidate2):
         for p1, p2 in zip(candidate1["program"].predictors(), candidate2["program"].predictors()):
             if self._get_signature(p1).instructions != self._get_signature(p2).instructions:
                 return False
             *_, p1_last_field = self._get_signature(p1).fields.values()
             *_, p2_last_field = self._get_signature(p2).fields.values()
             if p1_last_field != p2_last_field:
@@ -103,19 +104,18 @@
                 last_batch = [c]
                 last_batch_score = c["score"]
             if not repeat:
                 final_candidates.append(c)
         return final_candidates
 
     def _print_signature(self, predictor):
-        if self.verbose:
-            signature = self._get_signature(predictor)
-            print(f"i: {signature.instructions}")
-            print(f"p: {list(signature.fields.values())[-1].json_schema_extra['prefix']}")
-            print()
+        signature = self._get_signature(predictor)
+
+        dspy.logger.debug(f"i: {signature.instructions}")
+        dspy.logger.debug(f"p: {list(signature.fields.values())[-1].json_schema_extra['prefix']}")
 
     def _get_signature(self, predictor):
         if hasattr(predictor, "extended_signature"):
             return predictor.extended_signature
         elif hasattr(predictor, "signature"):
             return predictor.signature
 
@@ -165,27 +165,27 @@
                 )(basic_instruction=basic_instruction)
             # Add in our initial prompt as a candidate as well
             instruct.completions.proposed_instruction.append(basic_instruction)
             instruct.completions.proposed_prefix_for_output_field.append(basic_prefix)
             candidates[id(predictor)] = instruct.completions
             evaluated_candidates[id(predictor)] = {}
 
-        if self.verbose and self.prompt_model:
-            print(f"{self.prompt_model.inspect_history(n=1)}")
+        if self.prompt_model:
+            dspy.logger.debug(f"{self.prompt_model.inspect_history(n=1)}")
 
         latest_candidates = candidates
         all_candidates = candidates
 
         module_clone = module.deepcopy()
 
         # For each iteration in depth...
         for d in range(
             self.depth,
         ):  # TODO: fix this so that we eval the new batch of predictors with the new best followoing predictors
-            print(f"Iteration Depth: {d+1}/{self.depth}.")
+            dspy.logger.info(f"Iteration Depth: {d+1}/{self.depth}.")
 
             latest_scores = []
 
             # Go through our module's predictors
             for p_i, (p_old, p_new) in enumerate(zip(module.predictors(), module_clone.predictors())):
                 candidates_ = latest_candidates[id(p_old)]  # Use the most recently generated candidates for evaluation
                 if len(module.predictors()) > 1:
@@ -207,36 +207,28 @@
                         self._get_signature(p_new)
                         .with_instructions(instruction)
                         .with_updated_fields(last_key, prefix=prefix)
                     )
                     self._set_signature(p_new, updated_signature)
 
                     # Score the instruction / prefix
-                    if self.verbose:
-                        print("----------------")
                     for i, predictor in enumerate(module_clone.predictors()):
-                        if self.verbose:
-                            print(f"Predictor {i+1}")
+                        dspy.logger.debug(f"Predictor {i+1}")
                         self._print_signature(predictor)
-                    print(
+                    dspy.logger.info(
                         f"At Depth {d+1}/{self.depth}, Evaluating Prompt Candidate #{c_i+1}/{len(candidates_)} for Predictor {p_i+1} of {len(module.predictors())}.",
                     )
                     score = evaluate(module_clone, devset=trainset, **eval_kwargs)
-                    if self.verbose and self.prompt_model:
-                        print(f"prompt_model.inspect_history(n=1) {self.prompt_model.inspect_history(n=1)}")
+                    if self.prompt_model:
+                        dspy.logger.debug(f"prompt_model.inspect_history(n=1) {self.prompt_model.inspect_history(n=1)}")
                     total_calls += 1
-                    if self.verbose:
-                        print("----------------")
 
                     replace_entry = True
-                    if self.verbose:
-                        print(f"(instruction, prefix) {(instruction, prefix)}")
-                    # if verbose: print(f"evaluated_candidates[id(p_old)] {evaluated_candidates[id(p_old)]}")
+                    dspy.logger.debug(f"(instruction, prefix) {(instruction, prefix)}")
                     if (instruction, prefix) in evaluated_candidates[id(p_old)]:
-                        # if verbose: print(f"if evaluated_candidates[id(p_old)][(instruction, prefix)] {evaluated_candidates[id(p_old)][(instruction, prefix)]}")
                         if evaluated_candidates[id(p_old)][(instruction, prefix)]["score"] >= score:
                             replace_entry = False
 
                     if replace_entry:
                         # Add it to our evaluated candidates list
                         evaluated_candidates[id(p_old)][(instruction, prefix)] = {
                             "score": score,
@@ -262,23 +254,21 @@
                 *_, last_key = self._get_signature(p_old).fields.keys()
                 updated_signature = (
                     self._get_signature(p_new)
                     .with_instructions(best_candidate["instruction"])
                     .with_updated_fields(last_key, prefix=best_candidate["prefix"])
                 )
                 self._set_signature(p_new, updated_signature)
-                if self.verbose:
-                    print(
-                        f"Updating Predictor {id(p_old)} to:\ni: {best_candidate['instruction']}\np: {best_candidate['prefix']}",
-                    )
-                if self.verbose:
-                    print("Full predictor with update: ")
+
+                dspy.logger.debug(
+                    f"Updating Predictor {id(p_old)} to:\ni: {best_candidate['instruction']}\np: {best_candidate['prefix']}",
+                )
+                dspy.logger.debug("Full predictor with update: ")
                 for i, predictor in enumerate(module_clone.predictors()):
-                    if self.verbose:
-                        print(f"Predictor {i}")
+                    dspy.logger.debug(f"Predictor {i}")
                     self._print_signature(predictor)
 
             if d == self.depth - 1:
                 break
 
             new_candidates = {}
             for p_base in module.predictors():
@@ -316,25 +306,25 @@
                 else:
                     instr = dspy.Predict(
                         GenerateInstructionGivenAttempts,
                         n=self.breadth,
                         temperature=self.init_temperature,
                     )(attempted_instructions=attempts)
 
-                if self.verbose and self.prompt_model:
-                    print(f"{self.prompt_model.inspect_history(n=1)}")
+                if self.prompt_model:
+                    dspy.logger.debug(f"(self.prompt_model.inspect_history(n=1)) {self.prompt_model.inspect_history(n=1)}")
                 # Get candidates for each predictor
                 new_candidates[id(p_base)] = instr.completions
                 all_candidates[id(p_base)].proposed_instruction.extend(instr.completions.proposed_instruction)
                 all_candidates[id(p_base)].proposed_prefix_for_output_field.extend(
                     instr.completions.proposed_prefix_for_output_field,
                 )
 
-            if self.verbose and self.prompt_model:
-                print(f"{self.prompt_model.inspect_history(n=1)}")
+            if self.prompt_model:
+                dspy.logger.debug(f"{self.prompt_model.inspect_history(n=1)}")
             latest_candidates = new_candidates
 
         candidates = []
         for predictor in module.predictors():
             candidates.extend(list(evaluated_candidates[id(predictor)].values()))
 
             if self.track_stats:
@@ -344,15 +334,14 @@
                 scores = [x["score"] for x in best_predictors][:10]
                 results_best[id(predictor)]["depth"].append(d)
                 results_best[id(predictor)]["max"].append(max(scores))
                 results_best[id(predictor)]["average"].append(sum(scores) / len(scores))
                 results_best[id(predictor)]["min"].append(min(scores))
                 results_best[id(predictor)]["std"].append(np.std(scores))
 
-        # if verbose: print(f"candidates: {candidates}")
         candidates.sort(key=lambda x: x["score"], reverse=True)
 
         candidates = self._drop_duplicates(candidates)
 
         best_program = candidates[0]["program"]
         best_program.candidate_programs = candidates
         best_program.total_calls = total_calls
```

### Comparing `dspy-ai-2.4.7/dspy/teleprompt/ensemble.py` & `dspy-ai-2.4.9/dspy/teleprompt/ensemble.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/teleprompt/finetune.py` & `dspy-ai-2.4.9/dspy/teleprompt/finetune.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/teleprompt/knn_fewshot.py` & `dspy-ai-2.4.9/dspy/teleprompt/knn_fewshot.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/teleprompt/mipro_optimizer.py` & `dspy-ai-2.4.9/dspy/teleprompt/mipro_optimizer.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/teleprompt/random_search.py` & `dspy-ai-2.4.9/dspy/teleprompt/random_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import random
 
+import dspy
 from dspy.evaluate.evaluate import Evaluate
 from dspy.teleprompt.teleprompt import Teleprompter
 
 from .bootstrap import BootstrapFewShot
 from .vanilla import LabeledFewShot
 
 # TODO: Don't forget dealing with the raw demos.
@@ -50,29 +51,29 @@
         self.num_candidate_sets = num_candidate_programs
         # self.max_num_traces = 1 + int(max_bootstrapped_demos / 2.0 * self.num_candidate_sets)
 
         # Semi-hacky way to get the parent class's _bootstrap function to stop early.
         # self.max_bootstrapped_demos = self.max_num_traces
         self.max_labeled_demos = max_labeled_demos
 
-        print("Going to sample between", self.min_num_samples, "and", self.max_num_samples, "traces per predictor.")
-        # print("Going to sample", self.max_num_traces, "traces in total.")
-        print("Will attempt to train", self.num_candidate_sets, "candidate sets.")
+        dspy.logger.info(
+            "Going to sample between", self.min_num_samples, "and", self.max_num_samples, "traces per predictor.",
+        )
+        dspy.logger.info("Will attempt to train", self.num_candidate_sets, "candidate sets.")
 
     def compile(self, student, *, teacher=None, trainset, valset=None, restrict=None, labeled_sample=True):
         self.trainset = trainset
         self.valset = valset or trainset  # TODO: FIXME: Note this choice.
 
         scores = []
         all_subscores = []
         score_data = []
 
         for seed in range(-3, self.num_candidate_sets):
             if (restrict is not None) and (seed not in restrict):
-                print(seed, restrict)
                 continue
 
             trainset2 = list(self.trainset)
 
             if seed == -3:
                 # zero-shot
                 program2 = student.reset_copy()
@@ -127,46 +128,46 @@
             ############ Assertion-aware Optimization ############
             if hasattr(program2, "_suggest_failures"):
                 score = score - program2._suggest_failures * 0.2
             if hasattr(program2, "_assert_failures"):
                 score = 0 if program2._assert_failures > 0 else score
             ######################################################
 
-            print("Score:", score, "for set:", [len(predictor.demos) for predictor in program2.predictors()])
+            dspy.logger.info("Score:", score, "for set:", [len(predictor.demos) for predictor in program2.predictors()])
 
             if len(scores) == 0 or score > max(scores):
-                print("New best score:", score, "for seed", seed)
+                dspy.logger.info("New best sscore:", score, "for seed", seed)
                 best_program = program2
 
             scores.append(score)
-            print(f"Scores so far: {scores}")
+            dspy.logger.info(f"Scores so far: {scores}")
 
-            print("Best score:", max(scores))
+            dspy.logger.info("Best score:", max(scores))
 
             score_data.append((score, subscores, seed, program2))
 
             if len(score_data) > 2:  # We check if there are at least 3 scores to consider
                 for k in [1, 2, 3, 5, 8, 9999]:
                     top_3_scores = sorted(score_data, key=lambda x: x[0], reverse=True)[:k]
 
                     # Transpose the subscores to get max per entry and then calculate their average
                     transposed_subscores = zip(*[subscores for _, subscores, *_ in top_3_scores if subscores])
                     avg_of_max_per_entry = sum(max(entry) for entry in transposed_subscores) / len(top_3_scores[0][1])
 
-                    print(f"Average of max per entry across top {k} scores: {avg_of_max_per_entry}")
+                    dspy.logger.info(f"Average of max per entry across top {k} scores: {avg_of_max_per_entry}")
 
             if self.stop_at_score is not None and score >= self.stop_at_score:
-                print(f"Stopping early because score {score} is >= stop_at_score {self.stop_at_score}")
+                dspy.logger.info(f"Stopping early because score {score} is >= stop_at_score {self.stop_at_score}")
                 break
 
         # To best program, attach all program candidates in decreasing average score
         best_program.candidate_programs = score_data
         best_program.candidate_programs = sorted(best_program.candidate_programs, key=lambda x: x[0], reverse=True)
 
-        print(len(best_program.candidate_programs), "candidate programs found.")
+        dspy.logger.info(f"{len(best_program.candidate_programs)} candidate programs found.")
 
         return best_program
 
 
 # sample between 4 and 10 examples from traces
 # TODO: FIXME: The max number of demos should be determined in part by the LM's tokenizer + max_length.
 # This does require executing the program, or at least the predictor.
```

### Comparing `dspy-ai-2.4.7/dspy/teleprompt/signature_opt.py` & `dspy-ai-2.4.9/dspy/teleprompt/signature_opt.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/teleprompt/signature_opt_bayesian.py` & `dspy-ai-2.4.9/dspy/teleprompt/signature_opt_bayesian.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/teleprompt/signature_opt_typed.py` & `dspy-ai-2.4.9/dspy/teleprompt/signature_opt_typed.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/teleprompt/teleprompt_optuna.py` & `dspy-ai-2.4.9/dspy/teleprompt/teleprompt_optuna.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/teleprompt/vanilla.py` & `dspy-ai-2.4.9/dspy/teleprompt/vanilla.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy/utils/dummies.py` & `dspy-ai-2.4.9/dspy/utils/dummies.py`

 * *Files identical despite different names*

### Comparing `dspy-ai-2.4.7/dspy_ai.egg-info/PKG-INFO` & `dspy-ai-2.4.9/dspy_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspy-ai
-Version: 2.4.7
+Version: 2.4.9
 Summary: DSPy
 Home-page: https://github.com/stanfordnlp/dsp
 Author: Omar Khattab
 Author-email: Omar Khattab <okhattab@stanford.edu>
 License: MIT License
 Project-URL: homepage, https://github.com/stanfordnlp/dspy
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,18 @@
 Provides-Extra: chromadb
 Provides-Extra: qdrant
 Provides-Extra: marqo
 Provides-Extra: mongodb
 Provides-Extra: pinecone
 Provides-Extra: weaviate
 Provides-Extra: faiss-cpu
+Provides-Extra: milvus
+Provides-Extra: google-vertex-ai
 Provides-Extra: anthropic
+Provides-Extra: aws
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
   <img align="center" src="docs/images/DSPy8.png" width="460px" />
 </p>
@@ -83,26 +86,33 @@
 
 **What does DSPy stand for?** It's a long story but the backronym now is **D**eclarative **S**elf-improving Language **P**rograms, p**y**thonically.
 
 ## 1) Installation
 
 All you need is:
 
-```
+```bash
 pip install dspy-ai
 ```
 
+To install the very latest from `main`:
+
+```bash
+pip install git+https://github.com/stanfordnlp/dspy.git
+````
+
 Or open our intro notebook in Google Colab: [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/github/stanfordnlp/dspy/blob/main/intro.ipynb)
 
 By default, DSPy installs the latest `openai` from pip. However, if you install old version before OpenAI changed their API `openai~=0.28.1`, the library will use that just fine. Both are supported.
 
-For the optional (alphabetically sorted) [Chromadb](https://github.com/chroma-core/chroma), [Qdrant](https://github.com/qdrant/qdrant), [Marqo](https://github.com/marqo-ai/marqo), Pinecone, or [Weaviate](https://github.com/weaviate/weaviate) retrieval integration(s), include the extra(s) below:
+For the optional (alphabetically sorted) [Chromadb](https://github.com/chroma-core/chroma), [Qdrant](https://github.com/qdrant/qdrant), [Marqo](https://github.com/marqo-ai/marqo), Pinecone, [Weaviate](https://github.com/weaviate/weaviate),
+or [Milvus](https://github.com/milvus-io/milvus) retrieval integration(s), include the extra(s) below:
 
 ```
-pip install dspy-ai[chromadb]  # or [qdrant] or [marqo] or [mongodb] or [pinecone] or [weaviate]
+pip install dspy-ai[chromadb]  # or [qdrant] or [marqo] or [mongodb] or [pinecone] or [weaviate] or [milvus]
 ```
 
 ## 2) Documentation
 
 The DSPy documentation is divided into **tutorials** (step-by-step illustration of solving a task in DSPy), **guides** (how to use specific parts of the API), and **examples** (self-contained programs that illustrate usage).
 
 ### A) Tutorials
@@ -119,17 +129,18 @@
 | Advanced | [**Information Extraction**](https://twitter.com/KarelDoostrlnck/status/1724991014207930696) | [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1CpsOiLiLYKeGrhmq579_FmtGsD5uZ3Qe) | Tackles extracting information from long articles (biomedical research papers). Combines in-context learning and retrieval to set SOTA on BioDEX. Contributed by [Karel D’Oosterlinck](https://twitter.com/KarelDoostrlnck/status/1724991014207930696).  |
 
 
 **Other resources people find useful**:
 
 - [DSPy talk at ScaleByTheBay Nov 2023](https://www.youtube.com/watch?v=Dt3H2ninoeY).
 - [DSPy webinar with MLOps Learners](https://www.youtube.com/watch?v=im7bCLW2aM4), a bit longer with Q&A.
-- Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck)
+- Hands-on Overviews of DSPy by the community: [DSPy Explained! by Connor Shorten](https://www.youtube.com/watch?v=41EfOY0Ldkc), [DSPy explained by code_your_own_ai](https://www.youtube.com/watch?v=ycfnKPxBMck), [DSPy Crash Course by AI Bites](https://youtu.be/5-zgASQKkKQ?si=3gnmVouT5_rpk_nu)
 - Interviews: [Weaviate Podcast in-person](https://www.youtube.com/watch?v=CDung1LnLbY), and you can find 6-7 other remote podcasts on YouTube from a few different perspectives/audiences.
 - **Tracing in DSPy** with Arize Phoenix: [Tutorial for tracing your prompts and the steps of your DSPy programs](https://colab.research.google.com/github/Arize-ai/phoenix/blob/main/tutorials/tracing/dspy_tracing_tutorial.ipynb)
+- [DSPy: Not Your Average Prompt Engineering](https://jina.ai/news/dspy-not-your-average-prompt-engineering), why it's crucial for future prompt engineering, and yet why it is challenging for prompt engineers to learn.
 
 ### B) Guides
 
 If you're new to DSPy, it's probably best to go in sequential order. You will probably refer to these guides frequently after that, e.g. to copy/paste snippets that you can edit for your own DSPy programs.
 
 
 1. **[Language Models](https://dspy-docs.vercel.app/docs/building-blocks/language_models)**
@@ -165,18 +176,21 @@
 - [AI feedback, or writing LM-based metrics in DSPy](https://github.com/stanfordnlp/dspy/blob/main/examples/tweets/tweet_metric.py)
 - [DSPy Optimizers Benchmark on a bunch of different tasks, by Michael Ryan](https://github.com/stanfordnlp/dspy/tree/main/testing/tasks)
 - [Indian Languages NLI with gains due to compiling by Saiful Haq](https://github.com/saifulhaq95/DSPy-Indic/blob/main/indicxlni.ipynb)
 - [Sophisticated Extreme Multi-Class Classification, IReRa, by Karel D’Oosterlinck](https://github.com/KarelDO/xmc.dspy)
 - [DSPy on BIG-Bench Hard Example, by Chris Levy](https://drchrislevy.github.io/posts/dspy/dspy.html)
 - [Using Ollama with DSPy for Mistral (quantized) by @jrknox1977](https://gist.github.com/jrknox1977/78c17e492b5a75ee5bbaf9673aee4641)
 - [Using DSPy, "The Unreasonable Effectiveness of Eccentric Automatic Prompts" (paper) by VMware's Rick Battle & Teja Gollapudi, and interview at TheRegister](https://www.theregister.com/2024/02/22/prompt_engineering_ai_models/)
+- [Optimizing Performance of Open Source LM for Text-to-SQL using DSPy and vLLM, by Juan Ovalle](https://github.com/jjovalle99/DSPy-Text2SQL)
 - Typed DSPy (contributed by [@normal-computing](https://github.com/normal-computing))
   - [Using DSPy to train Gpt 3.5 on HumanEval by Thomas Ahle](https://github.com/stanfordnlp/dspy/blob/main/examples/functional/functional.ipynb)
   - [Building a chess playing agent using DSPy by Franck SN](https://medium.com/thoughts-on-machine-learning/building-a-chess-playing-agent-using-dspy-9b87c868f71e)
 
+TODO: Add links to the state-of-the-art results on Theory of Mind (ToM) by Plastic Labs, the results by Haize Labs for Red Teaming with DSPy, and the DSPy pipeline from Replit.
+
 There are also recent cool examples at [Weaviate's DSPy cookbook](https://github.com/weaviate/recipes/tree/main/integrations/dspy) by Connor Shorten. [See tutorial on YouTube](https://www.youtube.com/watch?v=CEuUG4Umfxs).
 
 ## 3) Syntax: You're in charge of the workflow—it's free-form Python code!
 
 **DSPy** hides tedious prompt engineering, but it cleanly exposes the important decisions you need to make: **[1]** what's your system design going to look like? **[2]** what are the important constraints on the behavior of your program?
 
 You express your system as free-form Pythonic modules. **DSPy** will tune the quality of your program _in whatever way_ you use foundation models: you can code with loops, `if` statements, or exceptions, and use **DSPy** modules within any Python control flow you think works for your task.
@@ -435,15 +449,15 @@
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) for a quickstart guide to contributing to DSPy.
 
 ## Contributors & Acknowledgements
 
 **DSPy** is led by **Omar Khattab** at Stanford NLP with **Chris Potts** and **Matei Zaharia**.
 
-Key contributors and team members include **Arnav Singhvi**, **Krista Opsahl-Ong**, **Michael Ryan**, **Karel D'Oosterlinck**, **Shangyin Tan**, **Manish Shetty**, **Paridhi Maheshwari**, **Keshav Santhanam**, **Sri Vardhamanan**, **Eric Zhang**, **Hanna Moazam**, **Thomas Joshi**, **Saiful Haq**, **Ashutosh Sharma**, and **Herumb Shandilya**.
+Key contributors and team members include **Arnav Singhvi**, **Krista Opsahl-Ong**, **Michael Ryan**, **Cyrus Nouroozi**, **Kyle Caverly**, **Amir Mehr**, **Karel D'Oosterlinck**, **Shangyin Tan**, **Manish Shetty**, **Herumb Shandilya**, **Paridhi Maheshwari**, **Keshav Santhanam**, **Sri Vardhamanan**, **Eric Zhang**, **Hanna Moazam**, **Thomas Joshi**, **Saiful Haq**, and **Ashutosh Sharma**.
 
 **DSPy** includes important contributions from **Rick Battle** and **Igor Kotenkov**. It reflects discussions with **Peter Zhong**, **Haoze He**, **Lisa Li**, **David Hall**, **Ashwin Paranjape**, **Heather Miller**, **Chris Manning**, **Percy Liang**, and many others.
 
 The **DSPy** logo is designed by **Chuyi Zhang**.
 
 
 ## 📜 Citation & Reading More
```

### Comparing `dspy-ai-2.4.7/dspy_ai.egg-info/SOURCES.txt` & `dspy-ai-2.4.9/dspy_ai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 pyproject.toml
 setup.py
 dsp/__init__.py
 dsp/evaluation/__init__.py
 dsp/evaluation/utils.py
 dsp/modules/__init__.py
 dsp/modules/anthropic.py
-dsp/modules/aws_lm.py
+dsp/modules/aws_models.py
+dsp/modules/aws_providers.py
 dsp/modules/azure_openai.py
 dsp/modules/azurecognitivesearch.py
-dsp/modules/bedrock.py
 dsp/modules/cache_utils.py
 dsp/modules/clarifai.py
 dsp/modules/cohere.py
 dsp/modules/colbertv2.py
 dsp/modules/databricks.py
+dsp/modules/dummy_lm.py
 dsp/modules/google.py
+dsp/modules/googlevertexai.py
 dsp/modules/gpt3.py
+dsp/modules/groq_client.py
 dsp/modules/hf.py
 dsp/modules/hf_client.py
 dsp/modules/hf_server.py
 dsp/modules/lm.py
+dsp/modules/mistral.py
 dsp/modules/ollama.py
 dsp/modules/pyserini.py
 dsp/modules/sbert.py
 dsp/modules/sentence_vectorizer.py
 dsp/modules/finetuning/__init__.py
 dsp/modules/finetuning/finetune_hf.py
 dsp/primitives/__init__.py
@@ -89,25 +93,28 @@
 dspy/primitives/box.py
 dspy/primitives/example.py
 dspy/primitives/module.py
 dspy/primitives/prediction.py
 dspy/primitives/program.py
 dspy/primitives/python_interpreter.py
 dspy/retrieve/__init__.py
+dspy/retrieve/azureaisearch_rm.py
 dspy/retrieve/chromadb_rm.py
 dspy/retrieve/clarifai_rm.py
 dspy/retrieve/databricks_rm.py
 dspy/retrieve/deeplake_rm.py
 dspy/retrieve/faiss_rm.py
 dspy/retrieve/marqo_rm.py
+dspy/retrieve/milvus_rm.py
 dspy/retrieve/mongodb_atlas_rm.py
 dspy/retrieve/neo4j_rm.py
 dspy/retrieve/pgvector_rm.py
 dspy/retrieve/pinecone_rm.py
 dspy/retrieve/qdrant_rm.py
+dspy/retrieve/ragatouille_rm.py
 dspy/retrieve/retrieve.py
 dspy/retrieve/vectara_rm.py
 dspy/retrieve/weaviate_rm.py
 dspy/retrieve/weaviate_rm_test.py
 dspy/retrieve/you_rm.py
 dspy/signatures/__init__.py
 dspy/signatures/field.py
@@ -124,12 +131,13 @@
 dspy/teleprompt/signature_opt_bayesian.py
 dspy/teleprompt/signature_opt_typed.py
 dspy/teleprompt/teleprompt.py
 dspy/teleprompt/teleprompt_optuna.py
 dspy/teleprompt/vanilla.py
 dspy/utils/__init__.py
 dspy/utils/dummies.py
+dspy/utils/logging.py
 dspy_ai.egg-info/PKG-INFO
 dspy_ai.egg-info/SOURCES.txt
 dspy_ai.egg-info/dependency_links.txt
 dspy_ai.egg-info/requires.txt
 dspy_ai.egg-info/top_level.txt
```

### Comparing `dspy-ai-2.4.7/dspy_ai.egg-info/requires.txt` & `dspy-ai-2.4.9/dspy_ai.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 pandas
 regex
 ujson
 tqdm
 datasets<3.0.0,~=2.14.6
 requests
 optuna
-pydantic==2.5.0
+pydantic~=2.0
+structlog
 
 [anthropic]
 anthropic~=0.18.0
 
+[aws]
+boto3~=1.34.78
+
 [chromadb]
 chromadb~=0.4.14
 
 [dev]
 pytest>=6.2.5
 
 [docs]
@@ -32,25 +36,32 @@
 sphinx-reredirects>=0.1.2
 sphinx-automodapi==0.16.0
 
 [faiss-cpu]
 sentence_transformers
 faiss-cpu
 
+[google-vertex-ai]
+google-cloud-aiplatform==1.43.0
+
 [marqo]
 marqo~=3.1.0
 marqo
 
+[milvus]
+pymilvus~=2.3.7
+
 [mongodb]
 pymongo~=3.12.0
 
 [pinecone]
 pinecone-client~=2.2.4
 
 [qdrant]
 qdrant-client
 fastembed
-qdrant-client~=1.6.2
-fastembed~=0.1.0
+qdrant-client>=1.6.2
+fastembed>=0.1.0
 
 [weaviate]
 weaviate-client~=3.26.1
+weaviate-client~=4.5.4
```

### Comparing `dspy-ai-2.4.7/pyproject.toml` & `dspy-ai-2.4.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dspy-ai"
-version = "2.4.7"
+version = "2.4.9"
 description = "DSPy"
 readme = "README.md"
 authors = [{ name = "Omar Khattab", email = "okhattab@stanford.edu" }]
 license = { text = "MIT License" }
 requires-python = ">=3.9, <3.12"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -31,24 +31,27 @@
     "pandas",
     "regex",
     "ujson",
     "tqdm",
     "datasets~=2.14.6,<3.0.0",
     "requests",
     "optuna",
-    "pydantic==2.5.0",
+    "pydantic~=2.0",
+    "structlog",
 ]
 
 [project.optional-dependencies]
 anthropic = ["anthropic~=0.18.0"]
 chromadb = ["chromadb~=0.4.14"]
-qdrant = ["qdrant-client~=1.6.2", "fastembed~=0.1.0"]
+qdrant = ["qdrant-client>=1.6.2", "fastembed>=0.1.0"]
 marqo = ["marqo"]
 pinecone = ["pinecone-client~=2.2.4"]
-weaviate = ["weaviate-client~=3.26.1"]
+weaviate = ["weaviate-client~=4.5.4"]
+milvus = ["pymilvus~=2.3.7"]
+aws = ["boto3~=1.34.78"]
 docs = [
     "sphinx>=4.3.0",
     "furo>=2023.3.27",
     "docutils<0.17",
     "m2r2",
     "myst-parser",
     "myst-nb",
@@ -75,15 +78,15 @@
 # documentation = "https://dspy-ai.readthedocs.io"
 keywords = ["dspy", "ai", "language models", "llm", "openai"]
 # may be a bit much
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-pydantic = "2.5.0"
+pydantic = "^2.0"
 backoff = "^2.2.1"
 joblib = "^1.3.2"
 openai = ">=0.28.1,<2.0.0"
 pandas = "^2.1.1"
 regex = "^2023.10.3"
 ujson = "^5.8.0"
 tqdm = "^4.66.1"
@@ -92,43 +95,53 @@
 optuna = "^3.4.0"
 anthropic = { version = "^0.18.0", optional = true }
 chromadb = { version = "^0.4.14", optional = true }
 fastembed = { version = "^0.1.0", optional = true }
 marqo = { version = "*", optional = true }
 qdrant-client = { version = "^1.6.2", optional = true }
 pinecone-client = { version = "^2.2.4", optional = true }
-weaviate-client = { version = "^3.26.1", optional = true }
+weaviate-client = { version = "^4.5.4", optional = true }
+pymilvus = { version = "^2.3.6", optional = true }
+boto3 = { version = "^1.34.78", optional = true }
 sphinx = { version = ">=4.3.0", optional = true }
 furo = { version = ">=2023.3.27", optional = true }
 docutils = { version = "<0.17", optional = true }
 m2r2 = { version = "*", optional = true }
 myst-parser = { version = "*", optional = true }
 myst-nb = { version = "*", optional = true }
 sphinx-autobuild = { version = "*", optional = true }
 sphinx_rtd_theme = { version = "*", optional = true }
 autodoc_pydantic = { version = "*", optional = true }
 sphinx-reredirects = { version = "^0.1.2", optional = true }
 sphinx-automodapi = { version = "0.16.0", optional = true }
+groq = { version = "^0.4.2", optional = true }
 rich = "^13.7.1"
+psycopg2 = { version = "^2.9.9", optional = true }
+pgvector = { version = "^0.2.5", optional = true }
+structlog = "^24.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.5"
 transformers = "^4.38.2"
 torch = "^2.2.1"
 pytest-mock = "^3.12.0"
 ruff = "^0.3.0"
 black = "^24.2.0"
+pre-commit = "^3.7.0"
 
 [tool.poetry.extras]
 chromadb = ["chromadb"]
 qdrant = ["qdrant-client", "fastembed"]
 marqo = ["marqo"]
 pinecone = ["pinecone-client"]
 weaviate = ["weaviate-client"]
+milvus = ["pymilvus"]
+aws = ["boto3"]
+postgres = ["psycopg2", "pgvector"]
 docs = [
     "sphinx",
     "furo",
     "docutils",
     "m2r2",
     "myst-parser",
     "myst-nb",
```

### Comparing `dspy-ai-2.4.7/setup.py` & `dspy-ai-2.4.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the content of the requirements.txt file	
 with open('requirements.txt', encoding='utf-8') as f:	
     requirements = f.read().splitlines()	
 
 setup(	
     name="dspy-ai",	
-    version="2.4.7",	
+    version="2.4.9",	
     description="DSPy",	
     long_description=long_description,	
     long_description_content_type='text/markdown',	
     url="https://github.com/stanfordnlp/dsp",	
     author="Omar Khattab",	
     author_email="okhattab@stanford.edu",	
     license="MIT License",	
@@ -25,14 +25,16 @@
         "chromadb": ["chromadb~=0.4.14"],
         "qdrant": ["qdrant-client", "fastembed"],
         "marqo": ["marqo~=3.1.0"],
         "mongodb": ["pymongo~=3.12.0"],			
         "pinecone": ["pinecone-client~=2.2.4"],	
         "weaviate": ["weaviate-client~=3.26.1"],	
         "faiss-cpu": ["sentence_transformers", "faiss-cpu"],
+        "milvus": ["pymilvus~=2.3.7"],
+        "google-vertex-ai": ["google-cloud-aiplatform==1.43.0"],
     },	
     classifiers=[	
         "Development Status :: 3 - Alpha",	
         "Intended Audience :: Science/Research",	
         "License :: OSI Approved :: MIT License",	
         "Operating System :: POSIX :: Linux",	
         "Programming Language :: Python :: 3",
```

