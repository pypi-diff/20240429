# Comparing `tmp/autorag-0.1.7.tar.gz` & `tmp/autorag-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autorag-0.1.7.tar", last modified: Sun Apr 28 11:59:17 2024, max compression
+gzip compressed data, was "autorag-0.1.8.tar", last modified: Mon Apr 29 14:33:49 2024, max compression
```

## Comparing `autorag-0.1.7.tar` & `autorag-0.1.8.tar`

### file list

```diff
@@ -1,515 +1,515 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.515210 autorag-0.1.7/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.395358 autorag-0.1.7/.github/
--rw-r--r--   0 jeffrey    (501) staff       (20)      501 2024-01-13 07:55:28.000000 autorag-0.1.7/.github/dependabot.yml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.395939 autorag-0.1.7/.github/workflows/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1486 2024-04-28 11:59:07.000000 autorag-0.1.7/.github/workflows/publish.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-03-25 06:37:01.000000 autorag-0.1.7/.github/workflows/sphinx.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)      927 2024-04-27 01:36:13.000000 autorag-0.1.7/.github/workflows/test.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)     3088 2024-01-13 07:55:28.000000 autorag-0.1.7/.gitignore
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.514309 autorag-0.1.7/AutoRAG.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)    24187 2024-04-28 11:59:17.000000 autorag-0.1.7/AutoRAG.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)    19840 2024-04-28 11:59:17.000000 autorag-0.1.7/AutoRAG.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2024-04-28 11:59:17.000000 autorag-0.1.7/AutoRAG.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       44 2024-04-28 11:59:17.000000 autorag-0.1.7/AutoRAG.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      523 2024-04-28 11:59:17.000000 autorag-0.1.7/AutoRAG.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        8 2024-04-28 11:59:17.000000 autorag-0.1.7/AutoRAG.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     2936 2024-04-27 01:36:13.000000 autorag-0.1.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     6374 2024-04-27 01:36:13.000000 autorag-0.1.7/CONTRIBUTING.md
--rw-r--r--   0 jeffrey    (501) staff       (20)    11357 2024-01-13 07:55:28.000000 autorag-0.1.7/LICENSE
--rw-r--r--   0 jeffrey    (501) staff       (20)    24187 2024-04-28 11:59:17.514924 autorag-0.1.7/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     9161 2024-04-15 08:09:03.000000 autorag-0.1.7/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.399209 autorag-0.1.7/autorag/
--rw-r--r--   0 jeffrey    (501) staff       (20)        5 2024-04-28 09:01:51.000000 autorag-0.1.7/autorag/VERSION
--rw-r--r--   0 jeffrey    (501) staff       (20)     2686 2024-04-27 14:09:04.000000 autorag-0.1.7/autorag/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4400 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/cli.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.399448 autorag-0.1.7/autorag/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-04-01 09:28:42.000000 autorag-0.1.7/autorag/data/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.400100 autorag-0.1.7/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      134 2024-03-22 04:27:08.000000 autorag-0.1.7/autorag/data/corpus/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1538 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/data/corpus/langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3645 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/data/corpus/llama_index.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.401971 autorag-0.1.7/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-04-11 07:54:19.000000 autorag-0.1.7/autorag/data/qacreation/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3123 2024-04-15 08:09:03.000000 autorag-0.1.7/autorag/data/qacreation/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7473 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/data/qacreation/llama_index.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3190 2024-03-23 03:44:06.000000 autorag-0.1.7/autorag/data/qacreation/llama_index_default_prompt.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     2924 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/data/qacreation/ragas.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3289 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/data/qacreation/simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.402377 autorag-0.1.7/autorag/data/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/data/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1496 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/data/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8871 2024-03-06 00:03:36.000000 autorag-0.1.7/autorag/deploy.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.403838 autorag-0.1.7/autorag/evaluate/
--rw-r--r--   0 jeffrey    (501) staff       (20)      146 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/evaluate/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2603 2024-04-05 14:53:42.000000 autorag-0.1.7/autorag/evaluate/generation.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.405407 autorag-0.1.7/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)      252 2024-04-05 14:53:42.000000 autorag-0.1.7/autorag/evaluate/metric/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.406447 autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-02-23 11:07:36.000000 autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1015 2024-02-23 11:07:40.000000 autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-02-23 11:07:43.000000 autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1005 2024-02-23 11:07:46.000000 autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)    12720 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/evaluate/metric/generation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1671 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/evaluate/metric/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2310 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/evaluate/metric/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      224 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/evaluate/metric/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2052 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/evaluate/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2099 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/evaluate/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1290 2024-02-18 20:58:37.000000 autorag-0.1.7/autorag/evaluate/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    17379 2024-04-27 15:42:07.000000 autorag-0.1.7/autorag/evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/node_line.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.406684 autorag-0.1.7/autorag/nodes/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/nodes/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.407779 autorag-0.1.7/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)       68 2024-03-07 23:12:39.000000 autorag-0.1.7/autorag/nodes/generator/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2215 2024-03-07 22:31:53.000000 autorag-0.1.7/autorag/nodes/generator/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1641 2024-03-30 16:26:48.000000 autorag-0.1.7/autorag/nodes/generator/llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4532 2024-03-31 04:56:43.000000 autorag-0.1.7/autorag/nodes/generator/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2810 2024-03-08 18:01:40.000000 autorag-0.1.7/autorag/nodes/generator/vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.408670 autorag-0.1.7/autorag/nodes/passageaugmenter/
--rw-r--r--   0 jeffrey    (501) staff       (20)      112 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passageaugmenter/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4688 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passageaugmenter/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      388 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passageaugmenter/prev_next_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3555 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/nodes/passageaugmenter/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.410248 autorag-0.1.7/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)      115 2024-04-15 08:09:03.000000 autorag-0.1.7/autorag/nodes/passagecompressor/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2445 2024-04-15 08:09:03.000000 autorag-0.1.7/autorag/nodes/passagecompressor/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      242 2024-02-22 15:32:30.000000 autorag-0.1.7/autorag/nodes/passagecompressor/pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2857 2024-04-15 08:09:03.000000 autorag-0.1.7/autorag/nodes/passagecompressor/refine.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6075 2024-02-15 17:28:32.000000 autorag-0.1.7/autorag/nodes/passagecompressor/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3028 2024-02-14 10:09:21.000000 autorag-0.1.7/autorag/nodes/passagecompressor/tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.411861 autorag-0.1.7/autorag/nodes/passagefilter/
--rw-r--r--   0 jeffrey    (501) staff       (20)      207 2024-04-15 08:09:03.000000 autorag-0.1.7/autorag/nodes/passagefilter/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2242 2024-04-15 08:09:03.000000 autorag-0.1.7/autorag/nodes/passagefilter/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      417 2024-04-11 14:32:56.000000 autorag-0.1.7/autorag/nodes/passagefilter/pass_passage_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3922 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/nodes/passagefilter/percentile_cutoff.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2399 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passagefilter/recency.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4119 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/nodes/passagefilter/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4022 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/nodes/passagefilter/threshold_cutoff.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.416033 autorag-0.1.7/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      504 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/nodes/passagereranker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2236 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/nodes/passagereranker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3979 2024-03-17 04:13:16.000000 autorag-0.1.7/autorag/nodes/passagereranker/cohere.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5376 2024-04-27 15:42:07.000000 autorag-0.1.7/autorag/nodes/passagereranker/colbert.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2722 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passagereranker/flag_embedding.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2397 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passagereranker/flag_embedding_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3713 2024-04-06 14:23:40.000000 autorag-0.1.7/autorag/nodes/passagereranker/jina.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4186 2024-03-06 19:44:35.000000 autorag-0.1.7/autorag/nodes/passagereranker/koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5697 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passagereranker/monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      618 2024-04-10 15:52:33.000000 autorag-0.1.7/autorag/nodes/passagereranker/pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4712 2024-04-05 03:16:26.000000 autorag-0.1.7/autorag/nodes/passagereranker/rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4335 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/nodes/passagereranker/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2884 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passagereranker/sentence_transformer.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.416836 autorag-0.1.7/autorag/nodes/passagereranker/tart/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/nodes/passagereranker/tart/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4983 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3832 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passagereranker/tart/tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4201 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/nodes/passagereranker/time_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5867 2024-04-27 15:32:19.000000 autorag-0.1.7/autorag/nodes/passagereranker/upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.418124 autorag-0.1.7/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)       84 2024-04-09 15:31:49.000000 autorag-0.1.7/autorag/nodes/promptmaker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1379 2024-04-09 15:31:49.000000 autorag-0.1.7/autorag/nodes/promptmaker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1162 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/nodes/promptmaker/fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2290 2024-04-09 15:31:49.000000 autorag-0.1.7/autorag/nodes/promptmaker/long_context_reorder.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8925 2024-03-31 10:20:41.000000 autorag-0.1.7/autorag/nodes/promptmaker/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.419532 autorag-0.1.7/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      123 2024-02-22 15:32:30.000000 autorag-0.1.7/autorag/nodes/queryexpansion/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1663 2024-03-06 19:11:31.000000 autorag-0.1.7/autorag/nodes/queryexpansion/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1572 2024-02-14 10:09:21.000000 autorag-0.1.7/autorag/nodes/queryexpansion/hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-22 15:32:30.000000 autorag-0.1.7/autorag/nodes/queryexpansion/pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3491 2024-02-14 10:09:21.000000 autorag-0.1.7/autorag/nodes/queryexpansion/query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7932 2024-02-15 17:29:26.000000 autorag-0.1.7/autorag/nodes/queryexpansion/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.421741 autorag-0.1.7/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      227 2024-04-11 14:29:33.000000 autorag-0.1.7/autorag/nodes/retrieval/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6444 2024-04-11 14:29:33.000000 autorag-0.1.7/autorag/nodes/retrieval/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5637 2024-03-25 04:14:52.000000 autorag-0.1.7/autorag/nodes/retrieval/bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3122 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/nodes/retrieval/hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3221 2024-04-11 14:29:33.000000 autorag-0.1.7/autorag/nodes/retrieval/hybrid_dbsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2957 2024-02-13 22:39:30.000000 autorag-0.1.7/autorag/nodes/retrieval/hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4148 2024-04-11 14:29:33.000000 autorag-0.1.7/autorag/nodes/retrieval/hybrid_rsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    10949 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/nodes/retrieval/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4907 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/nodes/retrieval/vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.422437 autorag-0.1.7/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)       50 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/schema/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      722 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/schema/module.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4158 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/schema/node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3996 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4202 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/support.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.423221 autorag-0.1.7/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)      237 2024-04-27 15:42:07.000000 autorag-0.1.7/autorag/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4020 2024-04-27 15:42:07.000000 autorag-0.1.7/autorag/utils/preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    12038 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2563 2024-03-06 00:03:36.000000 autorag-0.1.7/autorag/web.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       73 2024-04-27 01:36:13.000000 autorag-0.1.7/dev_requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.424160 autorag-0.1.7/docs/
--rw-r--r--   0 jeffrey    (501) staff       (20)      638 2024-01-17 16:38:11.000000 autorag-0.1.7/docs/Makefile
--rw-r--r--   0 jeffrey    (501) staff       (20)      804 2024-01-17 11:55:21.000000 autorag-0.1.7/docs/make.bat
--rw-r--r--   0 jeffrey    (501) staff       (20)      125 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.426113 autorag-0.1.7/docs/source/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.434500 autorag-0.1.7/docs/source/_static/
--rw-r--r--   0 jeffrey    (501) staff       (20)    57124 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/data_creation.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    30770 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/data_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    31538 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/node_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    18941 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/node_line_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    42589 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/node_line_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    92939 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/node_lines.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    95669 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/node_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    36728 2024-02-07 10:54:42.000000 autorag-0.1.7/docs/source/_static/project_folder_example.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    19853 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/project_folders.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    22432 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/resources_folder.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.438167 autorag-0.1.7/docs/source/_static/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)   159068 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/_static/roadmap/RAG_paradigms.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    38568 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/_static/roadmap/advanced_RAG.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    62853 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/_static/roadmap/cycle.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    75826 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/_static/roadmap/merger.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    82200 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/_static/roadmap/node_line_modular.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    69999 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/_static/roadmap/policy.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   567356 2024-02-07 10:54:42.000000 autorag-0.1.7/docs/source/_static/samsung_sundae.jpeg
--rw-r--r--   0 jeffrey    (501) staff       (20)    37348 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/trial_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    25499 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/trial_json.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   177107 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/trial_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   269046 2024-03-06 00:03:36.000000 autorag-0.1.7/docs/source/_static/web_interface.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.443566 autorag-0.1.7/docs/source/api_spec/
--rw-r--r--   0 jeffrey    (501) staff       (20)      563 2024-03-22 04:34:21.000000 autorag-0.1.7/docs/source/api_spec/autorag.data.corpus.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      939 2024-04-14 04:49:44.000000 autorag-0.1.7/docs/source/api_spec/autorag.data.qacreation.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      287 2024-03-22 04:34:21.000000 autorag-0.1.7/docs/source/api_spec/autorag.data.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      358 2024-03-22 04:34:21.000000 autorag-0.1.7/docs/source/api_spec/autorag.data.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      984 2024-02-10 14:23:30.000000 autorag-0.1.7/docs/source/api_spec/autorag.evaluate.metric.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      962 2024-02-10 14:23:30.000000 autorag-0.1.7/docs/source/api_spec/autorag.evaluate.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      941 2024-03-17 04:13:16.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.generator.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      864 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1294 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagecompressor.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1471 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagefilter.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     3434 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagereranker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      952 2024-02-01 16:32:39.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      995 2024-04-09 15:31:49.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.promptmaker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1254 2024-02-22 15:32:30.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.queryexpansion.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1896 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.retrieval.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      466 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1239 2024-03-07 15:58:42.000000 autorag-0.1.7/docs/source/api_spec/autorag.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      486 2024-01-17 15:59:52.000000 autorag-0.1.7/docs/source/api_spec/autorag.schema.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      489 2024-01-17 15:59:52.000000 autorag-0.1.7/docs/source/api_spec/autorag.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-01-17 15:59:52.000000 autorag-0.1.7/docs/source/api_spec/modules.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1454 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/conf.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.444432 autorag-0.1.7/docs/source/data_creation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     5072 2024-02-18 20:58:37.000000 autorag-0.1.7/docs/source/data_creation/data_format.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2206 2024-04-12 13:21:50.000000 autorag-0.1.7/docs/source/data_creation/ragas.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     5543 2024-03-25 11:47:15.000000 autorag-0.1.7/docs/source/data_creation/tutorial.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.444902 autorag-0.1.7/docs/source/deploy/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1473 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/deploy/api_endpoint.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      912 2024-03-06 00:03:36.000000 autorag-0.1.7/docs/source/deploy/web.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4124 2024-04-12 13:21:50.000000 autorag-0.1.7/docs/source/index.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1891 2024-02-15 09:50:25.000000 autorag-0.1.7/docs/source/install.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     6153 2024-04-12 13:21:50.000000 autorag-0.1.7/docs/source/local_model.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.445102 autorag-0.1.7/docs/source/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.445737 autorag-0.1.7/docs/source/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2703 2024-04-05 14:53:42.000000 autorag-0.1.7/docs/source/nodes/generator/generator.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1306 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/generator/llama_index_llm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1358 2024-03-14 09:00:38.000000 autorag-0.1.7/docs/source/nodes/generator/vllm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      172 2024-04-11 14:29:33.000000 autorag-0.1.7/docs/source/nodes/index.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.446169 autorag-0.1.7/docs/source/nodes/passage_augmenter/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1591 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/nodes/passage_augmenter/passage_augmenter.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      727 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.446653 autorag-0.1.7/docs/source/nodes/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3046 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/nodes/passage_compressor/passage_compressor.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1182 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/nodes/passage_compressor/refine.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1252 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/passage_compressor/tree_summarize.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.447345 autorag-0.1.7/docs/source/nodes/passage_filter/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1765 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/nodes/passage_filter/passage_filter.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1127 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/nodes/passage_filter/recency_filter.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1028 2024-04-12 13:21:50.000000 autorag-0.1.7/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1085 2024-04-10 13:46:46.000000 autorag-0.1.7/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.450206 autorag-0.1.7/docs/source/nodes/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1151 2024-03-17 04:13:16.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/cohere.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      521 2024-04-08 12:04:54.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/colbert.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      675 2024-04-11 14:29:33.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      654 2024-04-11 14:29:33.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1232 2024-04-06 14:23:40.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/jina_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      366 2024-02-22 16:33:58.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/koreranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1567 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/monot5.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2372 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/passage_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-04-05 03:16:26.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/rankgpt.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      645 2024-04-08 08:26:20.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      515 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/tart.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      561 2024-04-12 13:21:50.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/time_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1491 2024-04-28 04:56:07.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/upr.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.450868 autorag-0.1.7/docs/source/nodes/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      585 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/prompt_maker/fstring.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      815 2024-04-09 15:31:49.000000 autorag-0.1.7/docs/source/nodes/prompt_maker/long_context_reorder.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2689 2024-04-09 15:31:49.000000 autorag-0.1.7/docs/source/nodes/prompt_maker/prompt_maker.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.451481 autorag-0.1.7/docs/source/nodes/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1178 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/query_expansion/hyde.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1330 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/query_expansion/query_decompose.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3272 2024-02-22 15:32:30.000000 autorag-0.1.7/docs/source/nodes/query_expansion/query_expansion.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.453053 autorag-0.1.7/docs/source/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      625 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/retrieval/bm25.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-10 06:33:52.000000 autorag-0.1.7/docs/source/nodes/retrieval/hybrid_cc.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2294 2024-04-11 14:29:33.000000 autorag-0.1.7/docs/source/nodes/retrieval/hybrid_dbsf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2053 2024-04-10 06:33:52.000000 autorag-0.1.7/docs/source/nodes/retrieval/hybrid_rrf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2304 2024-04-10 06:33:52.000000 autorag-0.1.7/docs/source/nodes/retrieval/hybrid_rsf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1910 2024-04-11 14:29:33.000000 autorag-0.1.7/docs/source/nodes/retrieval/retrieval.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1223 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/retrieval/vectordb.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.454033 autorag-0.1.7/docs/source/optimization/
--rw-r--r--   0 jeffrey    (501) staff       (20)     4160 2024-02-15 10:23:20.000000 autorag-0.1.7/docs/source/optimization/custom_config.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3779 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/optimization/folder_structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4596 2024-02-07 21:46:19.000000 autorag-0.1.7/docs/source/optimization/optimization.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2580 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/optimization/sample_full_config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.454241 autorag-0.1.7/docs/source/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)     6735 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/roadmap/modular_rag.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3032 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3121 2024-02-18 20:58:37.000000 autorag-0.1.7/docs/source/troubleshooting.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     8338 2024-03-29 05:05:10.000000 autorag-0.1.7/docs/source/tutorial.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1529 2024-04-26 05:39:23.000000 autorag-0.1.7/pyproject.toml
--rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-04-27 07:55:59.000000 autorag-0.1.7/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.455947 autorag-0.1.7/sample_config/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2101 2024-03-14 09:00:38.000000 autorag-0.1.7/sample_config/compact_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2420 2024-03-17 04:13:16.000000 autorag-0.1.7/sample_config/compact_openai.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     1222 2024-03-17 04:13:16.000000 autorag-0.1.7/sample_config/config_korean.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      976 2024-03-06 00:03:36.000000 autorag-0.1.7/sample_config/extracted_sample.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     4769 2024-04-27 01:36:13.000000 autorag-0.1.7/sample_config/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      896 2024-03-14 09:00:38.000000 autorag-0.1.7/sample_config/simple_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      863 2024-02-08 11:27:02.000000 autorag-0.1.7/sample_config/simple_openai.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.456149 autorag-0.1.7/sample_dataset/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1404 2024-02-05 20:46:09.000000 autorag-0.1.7/sample_dataset/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.456375 autorag-0.1.7/sample_dataset/eli5/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1109 2024-02-05 20:46:09.000000 autorag-0.1.7/sample_dataset/eli5/load_eli5_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.456541 autorag-0.1.7/sample_dataset/msmarco/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1167 2024-02-05 20:46:09.000000 autorag-0.1.7/sample_dataset/msmarco/load_msmarco_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.456807 autorag-0.1.7/sample_dataset/triviaqa/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1171 2024-02-07 10:54:45.000000 autorag-0.1.7/sample_dataset/triviaqa/load_triviaqa_dataset.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2024-04-28 11:59:17.515262 autorag-0.1.7/setup.cfg
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.457702 autorag-0.1.7/tests/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.459267 autorag-0.1.7/tests/autorag/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.389040 autorag-0.1.7/tests/autorag/data/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.460016 autorag-0.1.7/tests/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      620 2024-03-22 04:29:06.000000 autorag-0.1.7/tests/autorag/data/corpus/test_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      646 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/data/corpus/test_langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1317 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/data/corpus/test_llama_index_corpus.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.461164 autorag-0.1.7/tests/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/data/qacreation/test_base_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3129 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/data/qacreation/test_llama_index_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      897 2024-04-12 13:21:50.000000 autorag-0.1.7/tests/autorag/data/qacreation/test_ragas_qa_creation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2097 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/data/qacreation/test_simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.462139 autorag-0.1.7/tests/autorag/evaluate/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.462939 autorag-0.1.7/tests/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3551 2024-04-05 14:53:42.000000 autorag-0.1.7/tests/autorag/evaluate/metric/test_generation_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1731 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1634 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/evaluate/metric/test_retrieval_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1263 2024-03-08 17:59:53.000000 autorag-0.1.7/tests/autorag/evaluate/test_evaluate_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4701 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/evaluate/test_generation_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1460 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2007 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/evaluate/test_retrieval_evaluate.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.389819 autorag-0.1.7/tests/autorag/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.463813 autorag-0.1.7/tests/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)      687 2024-03-08 18:01:40.000000 autorag-0.1.7/tests/autorag/nodes/generator/test_generator_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1372 2024-03-08 17:13:58.000000 autorag-0.1.7/tests/autorag/nodes/generator/test_llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3263 2024-03-31 05:05:12.000000 autorag-0.1.7/tests/autorag/nodes/generator/test_run_generator_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1004 2024-03-08 18:15:21.000000 autorag-0.1.7/tests/autorag/nodes/generator/test_vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.464417 autorag-0.1.7/tests/autorag/nodes/passageaugmenter/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1159 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      751 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2594 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3080 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.465423 autorag-0.1.7/tests/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-04-15 08:09:03.000000 autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      820 2024-02-22 15:32:30.000000 autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1852 2024-04-15 08:09:03.000000 autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_refine.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5073 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1933 2024-04-15 08:09:03.000000 autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.466823 autorag-0.1.7/tests/autorag/nodes/passagefilter/
--rw-r--r--   0 jeffrey    (501) staff       (20)      710 2024-04-11 14:32:56.000000 autorag-0.1.7/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3615 2024-04-15 08:09:03.000000 autorag-0.1.7/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2999 2024-04-10 13:46:46.000000 autorag-0.1.7/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      981 2024-04-12 13:21:50.000000 autorag-0.1.7/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4380 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagefilter/test_recency_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      860 2024-04-10 13:46:46.000000 autorag-0.1.7/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.470557 autorag-0.1.7/tests/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1160 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3283 2024-04-27 15:42:07.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1994 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_flag_embedding.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2213 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1881 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_jina_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-02-22 16:33:58.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1407 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-02-22 15:32:30.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4580 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4830 2024-02-18 20:58:37.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2230 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1604 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1371 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1210 2024-04-12 13:21:50.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_time_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      992 2024-04-27 15:25:25.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.471377 autorag-0.1.7/tests/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1373 2024-04-09 15:31:49.000000 autorag-0.1.7/tests/autorag/nodes/promptmaker/test_fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1798 2024-04-09 15:31:49.000000 autorag-0.1.7/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      580 2024-04-09 15:31:49.000000 autorag-0.1.7/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8310 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.472893 autorag-0.1.7/tests/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      813 2024-02-22 15:48:12.000000 autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      544 2024-02-22 15:32:30.000000 autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-22 15:56:28.000000 autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1586 2024-02-15 09:47:24.000000 autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6880 2024-02-22 16:17:25.000000 autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.475144 autorag-0.1.7/tests/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2906 2024-03-25 03:54:12.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4013 2024-04-11 14:29:33.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1525 2024-04-11 14:29:33.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      879 2024-04-11 14:29:33.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2989 2024-04-10 06:33:52.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      780 2024-04-11 14:29:33.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2976 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_retrieval_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    11185 2024-03-23 14:00:14.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4692 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.475678 autorag-0.1.7/tests/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1033 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/schema/test_module_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5515 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/schema/test_node_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3118 2024-03-29 05:05:10.000000 autorag-0.1.7/tests/autorag/test_cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6869 2024-04-10 13:46:46.000000 autorag-0.1.7/tests/autorag/test_deploy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    14669 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/test_evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2081 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/test_strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      306 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/test_support.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      878 2024-03-06 00:03:36.000000 autorag-0.1.7/tests/autorag/test_web.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.476276 autorag-0.1.7/tests/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3773 2024-04-27 15:42:07.000000 autorag-0.1.7/tests/autorag/utils/test_preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     9970 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/utils/test_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-23 03:44:06.000000 autorag-0.1.7/tests/conftest.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      672 2024-02-18 20:58:37.000000 autorag-0.1.7/tests/delete_tests.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2641 2024-02-22 16:04:39.000000 autorag-0.1.7/tests/mock.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.478582 autorag-0.1.7/tests/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-03-23 03:44:06.000000 autorag-0.1.7/tests/resources/README.md
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.7/tests/resources/corpus_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.390192 autorag-0.1.7/tests/resources/data_creation/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.479388 autorag-0.1.7/tests/resources/data_creation/raw_dir/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3379 2024-02-08 11:27:05.000000 autorag-0.1.7/tests/resources/data_creation/raw_dir/sample1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3243 2024-02-08 11:27:05.000000 autorag-0.1.7/tests/resources/data_creation/raw_dir/sample2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     4563 2024-02-08 11:27:05.000000 autorag-0.1.7/tests/resources/data_creation/raw_dir/sample3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3235 2024-04-12 16:43:24.000000 autorag-0.1.7/tests/resources/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.7/tests/resources/qa_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.480070 autorag-0.1.7/tests/resources/qa_gen_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)      198 2024-04-17 01:53:11.000000 autorag-0.1.7/tests/resources/qa_gen_prompts/prompt1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      186 2024-03-23 03:44:06.000000 autorag-0.1.7/tests/resources/qa_gen_prompts/prompt2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      202 2024-03-23 03:44:06.000000 autorag-0.1.7/tests/resources/qa_gen_prompts/prompt3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     5910 2024-02-07 10:54:45.000000 autorag-0.1.7/tests/resources/qa_test_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.480642 autorag-0.1.7/tests/resources/result_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.481080 autorag-0.1.7/tests/resources/result_project/0/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2297 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.481286 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.484147 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)    23516 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    26448 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    33716 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14618 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14683 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    13278 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    54234 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     1155 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.485087 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     8443 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    41557 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      513 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.485346 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.486803 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.486956 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.488121 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.489822 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.491320 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      845 2024-02-18 14:46:34.000000 autorag-0.1.7/tests/resources/result_project/0/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.491535 autorag-0.1.7/tests/resources/result_project/1/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.491746 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.493290 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.391872 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.493446 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.494530 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.496375 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.496757 autorag-0.1.7/tests/resources/result_project/2/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.392087 autorag-0.1.7/tests/resources/result_project/2/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.497053 autorag-0.1.7/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.497572 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.499282 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.499423 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.500005 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.501822 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.503556 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.503776 autorag-0.1.7/tests/resources/result_project/3/
--rw-r--r--   0 jeffrey    (501) staff       (20)      682 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/3/config.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2307 2024-03-29 05:05:10.000000 autorag-0.1.7/tests/resources/result_project/best.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.504771 autorag-0.1.7/tests/resources/result_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.505019 autorag-0.1.7/tests/resources/result_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/resources/bm25.pkl
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.505282 autorag-0.1.7/tests/resources/result_project/resources/chroma/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.511817 autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
--rw-r--r--   0 jeffrey    (501) staff       (20)  6284000 2024-02-18 14:41:41.000000 autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)      100 2024-02-18 14:41:00.000000 autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)     4000 2024-02-18 14:41:41.000000 autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-18 14:41:00.000000 autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)   352256 2024-02-18 14:41:41.000000 autorag-0.1.7/tests/resources/result_project/resources/chroma/chroma.sqlite3
--rw-r--r--   0 jeffrey    (501) staff       (20)      338 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/trial.json
--rw-r--r--   0 jeffrey    (501) staff       (20)     8439 2024-03-23 03:44:06.000000 autorag-0.1.7/tests/resources/sample_contents_nqa.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.393226 autorag-0.1.7/tests/resources/sample_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.512727 autorag-0.1.7/tests/resources/sample_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   115302 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/resources/sample_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.7/tests/resources/sample_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.513445 autorag-0.1.7/tests/resources/sample_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-01-13 07:56:04.000000 autorag-0.1.7/tests/resources/sample_project/resources/bm25.pkl
--rw-r--r--   0 jeffrey    (501) staff       (20)      893 2024-04-10 13:46:46.000000 autorag-0.1.7/tests/resources/simple.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)    26773 2024-01-13 07:56:04.000000 autorag-0.1.7/tests/resources/test_bm25_retrieval.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.267387 autorag-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.175387 autorag-0.1.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-29 14:33:32.000000 autorag-0.1.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.175387 autorag-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-29 14:33:32.000000 autorag-0.1.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-29 14:33:32.000000 autorag-0.1.8/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-29 14:33:32.000000 autorag-0.1.8/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-29 14:33:32.000000 autorag-0.1.8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.263387 autorag-0.1.8/AutoRAG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24187 2024-04-29 14:33:49.000000 autorag-0.1.8/AutoRAG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19840 2024-04-29 14:33:49.000000 autorag-0.1.8/AutoRAG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:33:49.000000 autorag-0.1.8/AutoRAG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 14:33:49.000000 autorag-0.1.8/AutoRAG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-29 14:33:49.000000 autorag-0.1.8/AutoRAG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 14:33:49.000000 autorag-0.1.8/AutoRAG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-29 14:33:32.000000 autorag-0.1.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-04-29 14:33:32.000000 autorag-0.1.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 14:33:32.000000 autorag-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24187 2024-04-29 14:33:49.263387 autorag-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-29 14:33:32.000000 autorag-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.175387 autorag-0.1.8/autorag/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.179386 autorag-0.1.8/autorag/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.179386 autorag-0.1.8/autorag/data/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/corpus/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/corpus/llama_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.179386 autorag-0.1.8/autorag/data/qacreation/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/qacreation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/qacreation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/qacreation/llama_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/qacreation/llama_index_default_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/qacreation/ragas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/qacreation/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.179386 autorag-0.1.8/autorag/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.179386 autorag-0.1.8/autorag/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.179386 autorag-0.1.8/autorag/evaluate/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.183386 autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/retrieval_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/retrieval_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17379 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/node_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.183386 autorag-0.1.8/autorag/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.183386 autorag-0.1.8/autorag/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/generator/llama_index_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/generator/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/generator/vllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.183386 autorag-0.1.8/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passageaugmenter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passageaugmenter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passageaugmenter/prev_next_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passageaugmenter/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.183386 autorag-0.1.8/autorag/nodes/passagecompressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagecompressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagecompressor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagecompressor/pass_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagecompressor/refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagecompressor/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagecompressor/tree_summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.187387 autorag-0.1.8/autorag/nodes/passagefilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/pass_passage_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/recency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/threshold_cutoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.187387 autorag-0.1.8/autorag/nodes/passagereranker/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/colbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/flag_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/flag_embedding_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/jina.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/koreranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/monot5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/pass_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/rankgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/sentence_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.187387 autorag-0.1.8/autorag/nodes/passagereranker/tart/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/tart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/tart/tart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/time_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/upr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.191387 autorag-0.1.8/autorag/nodes/promptmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/promptmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/promptmaker/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/promptmaker/fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/promptmaker/long_context_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/promptmaker/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.191387 autorag-0.1.8/autorag/nodes/queryexpansion/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/queryexpansion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/queryexpansion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/queryexpansion/hyde.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/queryexpansion/pass_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/queryexpansion/query_decompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/queryexpansion/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.191387 autorag-0.1.8/autorag/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/hybrid_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/hybrid_dbsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/hybrid_rrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/hybrid_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.191387 autorag-0.1.8/autorag/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/schema/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/schema/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.195387 autorag-0.1.8/autorag/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-29 14:33:32.000000 autorag-0.1.8/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.195387 autorag-0.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.195387 autorag-0.1.8/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.199386 autorag-0.1.8/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    57124 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/data_creation.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30770 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/data_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31538 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/node_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18941 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/node_line_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42589 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/node_line_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92939 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/node_lines.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95669 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/node_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36728 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/project_folder_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19853 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/project_folders.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/resources_folder.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.203387 autorag-0.1.8/docs/source/_static/roadmap/
+-rw-r--r--   0 runner    (1001) docker     (127)   159068 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/roadmap/RAG_paradigms.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38568 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/roadmap/advanced_RAG.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62853 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/roadmap/cycle.png
+-rw-r--r--   0 runner    (1001) docker     (127)    75826 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/roadmap/merger.png
+-rw-r--r--   0 runner    (1001) docker     (127)    82200 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/roadmap/node_line_modular.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69999 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/roadmap/policy.png
+-rw-r--r--   0 runner    (1001) docker     (127)   567356 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/samsung_sundae.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)    37348 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/trial_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25499 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/trial_json.png
+-rw-r--r--   0 runner    (1001) docker     (127)   177107 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/trial_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)   269046 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/web_interface.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/api_spec/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.data.corpus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.data.qacreation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.data.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.evaluate.metric.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.evaluate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.generator.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagecompressor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagefilter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagereranker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.promptmaker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.queryexpansion.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.retrieval.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/data_creation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/data_creation/data_format.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/data_creation/ragas.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/data_creation/tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/deploy/api_endpoint.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/deploy/web.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/local_model.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/generator/generator.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/generator/llama_index_llm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/generator/vllm.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/nodes/passage_augmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_augmenter/passage_augmenter.md
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/nodes/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_compressor/passage_compressor.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_compressor/refine.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_compressor/tree_summarize.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.211387 autorag-0.1.8/docs/source/nodes/passage_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_filter/passage_filter.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_filter/recency_filter.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.211387 autorag-0.1.8/docs/source/nodes/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/cohere.md
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/colbert.md
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/jina_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/koreranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/monot5.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/passage_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/rankgpt.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/tart.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/time_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/upr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.211387 autorag-0.1.8/docs/source/nodes/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/prompt_maker/fstring.md
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/prompt_maker/long_context_reorder.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/prompt_maker/prompt_maker.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.211387 autorag-0.1.8/docs/source/nodes/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/query_expansion/hyde.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/query_expansion/query_decompose.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/query_expansion/query_expansion.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.215386 autorag-0.1.8/docs/source/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/bm25.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/hybrid_cc.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/hybrid_dbsf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/hybrid_rrf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/hybrid_rsf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/retrieval.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/vectordb.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.215386 autorag-0.1.8/docs/source/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/optimization/custom_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/optimization/folder_structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/optimization/optimization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/optimization/sample_full_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.215386 autorag-0.1.8/docs/source/roadmap/
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/roadmap/modular_rag.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/troubleshooting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-29 14:33:32.000000 autorag-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-29 14:33:32.000000 autorag-0.1.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.215386 autorag-0.1.8/sample_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/compact_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/compact_openai.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/config_korean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/extracted_sample.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/full.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/simple_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/simple_openai.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.215386 autorag-0.1.8/sample_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_dataset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.215386 autorag-0.1.8/sample_dataset/eli5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_dataset/eli5/load_eli5_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/sample_dataset/msmarco/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_dataset/msmarco/load_msmarco_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/sample_dataset/triviaqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_dataset/triviaqa/load_triviaqa_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:33:49.267387 autorag-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/tests/autorag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.163386 autorag-0.1.8/tests/autorag/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/tests/autorag/data/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/corpus/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/corpus/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/corpus/test_llama_index_corpus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/tests/autorag/data/qacreation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/qacreation/test_base_qacreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/qacreation/test_llama_index_qacreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/qacreation/test_ragas_qa_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/qacreation/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/tests/autorag/evaluate/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.223387 autorag-0.1.8/tests/autorag/evaluate/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/metric/test_generation_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/metric/test_retrieval_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/test_evaluate_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/test_generation_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/test_retrieval_evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.167386 autorag-0.1.8/tests/autorag/nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.223387 autorag-0.1.8/tests/autorag/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/generator/test_generator_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/generator/test_llama_index_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/generator/test_run_generator_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/generator/test_vllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.223387 autorag-0.1.8/tests/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.223387 autorag-0.1.8/tests/autorag/nodes/passagecompressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.227387 autorag-0.1.8/tests/autorag/nodes/passagefilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagefilter/test_recency_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.227387 autorag-0.1.8/tests/autorag/nodes/passagereranker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_flag_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_jina_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_koreranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_monot5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_pass_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_rankgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_tart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_time_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_upr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.227387 autorag-0.1.8/tests/autorag/nodes/promptmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/promptmaker/test_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.231387 autorag-0.1.8/tests/autorag/nodes/queryexpansion/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_hyde.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_query_decompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.231387 autorag-0.1.8/tests/autorag/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_retrieval_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.231387 autorag-0.1.8/tests/autorag/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/schema/test_module_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/schema/test_node_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.231387 autorag-0.1.8/tests/autorag/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/utils/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/utils/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/delete_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.235387 autorag-0.1.8/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/corpus_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.167386 autorag-0.1.8/tests/resources/data_creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.235387 autorag-0.1.8/tests/resources/data_creation/raw_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/data_creation/raw_dir/sample1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/data_creation/raw_dir/sample2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/data_creation/raw_dir/sample3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/full.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/qa_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.235387 autorag-0.1.8/tests/resources/qa_gen_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/qa_gen_prompts/prompt1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/qa_gen_prompts/prompt2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/qa_gen_prompts/prompt3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/qa_test_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.235387 autorag-0.1.8/tests/resources/result_project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.235387 autorag-0.1.8/tests/resources/result_project/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.235387 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.239387 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    26448 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    33716 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54234 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.239387 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    41557 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.239387 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.239387 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.239387 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.239387 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.243387 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.243387 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.243387 autorag-0.1.8/tests/resources/result_project/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.243387 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.243387 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.171387 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.243387 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.171387 autorag-0.1.8/tests/resources/result_project/2/post_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/3/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/3/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/best.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/data/corpus.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/data/qa.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   109454 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/resources/bm25.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/resources/chroma/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.263387 autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
+-rw-r--r--   0 runner    (1001) docker     (127)  6284000 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
+-rw-r--r--   0 runner    (1001) docker     (127)   352256 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/resources/chroma/chroma.sqlite3
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/trial.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/sample_contents_nqa.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.171387 autorag-0.1.8/tests/resources/sample_project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.263387 autorag-0.1.8/tests/resources/sample_project/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   115302 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/sample_project/data/corpus.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/sample_project/data/qa.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.263387 autorag-0.1.8/tests/resources/sample_project/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   109454 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/sample_project/resources/bm25.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26773 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/test_bm25_retrieval.pkl
```

### Comparing `autorag-0.1.7/.github/workflows/publish.yml` & `autorag-0.1.8/.github/workflows/publish.yml`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: '3.10'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install setuptools wheel twine
+          python -m pip install setuptools wheel twine build setuptools-scm
       - name: Get changed files
         id: changed-files
         uses: tj-actions/changed-files@v44
       - name: Check for VERSION file change
         id: version_changed
         env:
           ALL_CHANGED_FILES: ${{ steps.changed-files.outputs.all_changed_files }}
```

### Comparing `autorag-0.1.7/.github/workflows/sphinx.yml` & `autorag-0.1.8/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/.github/workflows/test.yml` & `autorag-0.1.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/.gitignore` & `autorag-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/AutoRAG.egg-info/PKG-INFO` & `autorag-0.1.8/AutoRAG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.7
+Version: 0.1.8
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `autorag-0.1.7/AutoRAG.egg-info/SOURCES.txt` & `autorag-0.1.8/AutoRAG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/AutoRAG.egg-info/requires.txt` & `autorag-0.1.8/AutoRAG.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/CODE_OF_CONDUCT.md` & `autorag-0.1.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/CONTRIBUTING.md` & `autorag-0.1.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/LICENSE` & `autorag-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/PKG-INFO` & `autorag-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.7
+Version: 0.1.8
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `autorag-0.1.7/README.md` & `autorag-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/__init__.py` & `autorag-0.1.8/autorag/__init__.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/cli.py` & `autorag-0.1.8/autorag/cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/data/corpus/langchain.py` & `autorag-0.1.8/autorag/data/corpus/langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/data/corpus/llama_index.py` & `autorag-0.1.8/autorag/data/corpus/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/data/qacreation/base.py` & `autorag-0.1.8/autorag/data/qacreation/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/data/qacreation/llama_index.py` & `autorag-0.1.8/autorag/data/qacreation/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/data/qacreation/llama_index_default_prompt.txt` & `autorag-0.1.8/autorag/data/qacreation/llama_index_default_prompt.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/data/qacreation/ragas.py` & `autorag-0.1.8/autorag/data/qacreation/ragas.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/data/qacreation/simple.py` & `autorag-0.1.8/autorag/data/qacreation/simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/data/utils/util.py` & `autorag-0.1.8/autorag/data/utils/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/deploy.py` & `autorag-0.1.8/autorag/deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/evaluate/generation.py` & `autorag-0.1.8/autorag/evaluate/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt` & `autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-You will be given one summary written for a news article.
-
-Your task is to rate the summary on one metric.
-
-Please make sure you read and understand these instructions carefully. Please keep this document open while reviewing, and refer to it as needed.
-
-Evaluation Criteria:
-
-Coherence (1-5) - the collective quality of all sentences. We align this dimension with the DUC quality question of structure and coherence whereby "the summary should be well-structured and well-organized. The summary should not just be a heap of related information, but should build from sentence to a coherent body of information about a topic."
-
-Evaluation Steps:
-
-1. Read the news article carefully and identify the main topic and key points.
-2. Read the summary and compare it to the news article. Check if the summary covers the main topic and key points of the news article, and if it presents them in a clear and logical order.
-3. Assign a score for coherence on a scale of 1 to 5, where 1 is the lowest and 5 is the highest based on the Evaluation Criteria.
-
-
-Example:
-
-
-Source Text:
-
-{{Document}}
-
-Summary:
-
-{{Summary}}
-
-
-Evaluation Form (scores ONLY):
-
+You will be given one summary written for a news article.
+
+Your task is to rate the summary on one metric.
+
+Please make sure you read and understand these instructions carefully. Please keep this document open while reviewing, and refer to it as needed.
+
+Evaluation Criteria:
+
+Coherence (1-5) - the collective quality of all sentences. We align this dimension with the DUC quality question of structure and coherence whereby "the summary should be well-structured and well-organized. The summary should not just be a heap of related information, but should build from sentence to a coherent body of information about a topic."
+
+Evaluation Steps:
+
+1. Read the news article carefully and identify the main topic and key points.
+2. Read the summary and compare it to the news article. Check if the summary covers the main topic and key points of the news article, and if it presents them in a clear and logical order.
+3. Assign a score for coherence on a scale of 1 to 5, where 1 is the lowest and 5 is the highest based on the Evaluation Criteria.
+
+
+Example:
+
+
+Source Text:
+
+{{Document}}
+
+Summary:
+
+{{Summary}}
+
+
+Evaluation Form (scores ONLY):
+
 - Coherence:
```

### Comparing `autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt` & `autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt` & `autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-You will be given one summary written for a news article.
-
-Your task is to rate the summary on one metric.
-
-Please make sure you read and understand these instructions carefully. Please keep this document open while reviewing, and refer to it as needed.
-
-
-Evaluation Criteria:
-
-Fluency (1-3): the quality of the summary in terms of grammar, spelling, punctuation, word choice, and sentence structure.
-
-- 1: Poor. The summary has many errors that make it hard to understand or sound unnatural.
-- 2: Fair. The summary has some errors that affect the clarity or smoothness of the text, but the main points are still comprehensible.
-- 3: Good. The summary has few or no errors and is easy to read and follow.
-
-
-Example:
-
-Summary:
-
-{{Summary}}
-
-
-Evaluation Form (scores ONLY):
-
+You will be given one summary written for a news article.
+
+Your task is to rate the summary on one metric.
+
+Please make sure you read and understand these instructions carefully. Please keep this document open while reviewing, and refer to it as needed.
+
+
+Evaluation Criteria:
+
+Fluency (1-3): the quality of the summary in terms of grammar, spelling, punctuation, word choice, and sentence structure.
+
+- 1: Poor. The summary has many errors that make it hard to understand or sound unnatural.
+- 2: Fair. The summary has some errors that affect the clarity or smoothness of the text, but the main points are still comprehensible.
+- 3: Good. The summary has few or no errors and is easy to read and follow.
+
+
+Example:
+
+Summary:
+
+{{Summary}}
+
+
+Evaluation Form (scores ONLY):
+
 - Fluency (1-3):
```

### Comparing `autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt` & `autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-You will be given one summary written for a news article.
-
-Your task is to rate the summary on one metric.
-
-Please make sure you read and understand these instructions carefully. Please keep this document open while reviewing, and refer to it as needed.
-
-Evaluation Criteria:
-
-Relevance (1-5) - selection of important content from the source. The summary should include only important information from the source document. Annotators were instructed to penalize summaries which contained redundancies and excess information.
-
-Evaluation Steps:
-
-1. Read the summary and the source document carefully.
-2. Compare the summary to the source document and identify the main points of the article.
-3. Assess how well the summary covers the main points of the article, and how much irrelevant or redundant information it contains.
-4. Assign a relevance score from 1 to 5.
-
-
-Example:
-
-
-Source Text:
-
-{{Document}}
-
-Summary:
-
-{{Summary}}
-
-
-Evaluation Form (scores ONLY):
-
+You will be given one summary written for a news article.
+
+Your task is to rate the summary on one metric.
+
+Please make sure you read and understand these instructions carefully. Please keep this document open while reviewing, and refer to it as needed.
+
+Evaluation Criteria:
+
+Relevance (1-5) - selection of important content from the source. The summary should include only important information from the source document. Annotators were instructed to penalize summaries which contained redundancies and excess information.
+
+Evaluation Steps:
+
+1. Read the summary and the source document carefully.
+2. Compare the summary to the source document and identify the main points of the article.
+3. Assess how well the summary covers the main points of the article, and how much irrelevant or redundant information it contains.
+4. Assign a relevance score from 1 to 5.
+
+
+Example:
+
+
+Source Text:
+
+{{Document}}
+
+Summary:
+
+{{Summary}}
+
+
+Evaluation Form (scores ONLY):
+
 - Relevance:
```

### Comparing `autorag-0.1.7/autorag/evaluate/metric/generation.py` & `autorag-0.1.8/autorag/evaluate/metric/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/evaluate/metric/retrieval.py` & `autorag-0.1.8/autorag/evaluate/metric/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/evaluate/metric/retrieval_contents.py` & `autorag-0.1.8/autorag/evaluate/metric/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/evaluate/retrieval.py` & `autorag-0.1.8/autorag/evaluate/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/evaluate/retrieval_contents.py` & `autorag-0.1.8/autorag/evaluate/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/evaluate/util.py` & `autorag-0.1.8/autorag/evaluate/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/evaluator.py` & `autorag-0.1.8/autorag/evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/node_line.py` & `autorag-0.1.8/autorag/node_line.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/generator/base.py` & `autorag-0.1.8/autorag/nodes/generator/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import functools
+import logging
 from pathlib import Path
 from typing import Union, Tuple, List
 
 import pandas as pd
 
 from autorag import generator_models
 from autorag.utils import result_to_dataframe
 
+logger = logging.getLogger("AutoRAG")
+
 
 def generator_node(func):
     @functools.wraps(func)
     @result_to_dataframe(["generated_texts", "generated_tokens", "generated_log_probs"])
     def wrapper(
             project_dir: Union[str, Path],
             previous_result: pd.DataFrame,
@@ -24,14 +27,15 @@
         :param project_dir: The project directory.
         :param previous_result: The previous result that contains prompts,
         :param llm: The llm name that you want to use.
         :param kwargs: The extra parameters for initializing the llm instance.
         :return: Pandas dataframe that contains generated texts, generated tokens, and generated log probs.
             Each column is "generated_texts", "generated_tokens", and "generated_log_probs".
         """
+        logger.info(f"Running generator node - {func.__name__} module...")
         assert 'prompts' in previous_result.columns, "previous_result must contain prompts column."
         prompts = previous_result['prompts'].tolist()
         if func.__name__ == 'llama_index_llm':
             if llm not in generator_models:
                 raise ValueError(f"{llm} is not a valid llm name. Please check the llm name."
                                  "You can check valid llm names from autorag.generator_models.")
             batch = kwargs.pop('batch', 16)
```

### Comparing `autorag-0.1.7/autorag/nodes/generator/llama_index_llm.py` & `autorag-0.1.8/autorag/nodes/generator/llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/generator/run.py` & `autorag-0.1.8/autorag/nodes/generator/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/generator/vllm.py` & `autorag-0.1.8/autorag/nodes/generator/vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passageaugmenter/base.py` & `autorag-0.1.8/autorag/nodes/passageaugmenter/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 def passage_augmenter_node(func):
     @functools.wraps(func)
     @result_to_dataframe(["retrieved_contents", "retrieved_ids", "retrieve_scores"])
     def wrapper(
             project_dir: Union[str, Path],
             previous_result: pd.DataFrame,
             *args, **kwargs) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
+        logger.info(f"Running passage augmenter node - {func.__name__} module...")
         validate_qa_dataset(previous_result)
         data_dir = os.path.join(project_dir, "data")
 
         # find queries columns
         assert "query" in previous_result.columns, "previous_result must have query column."
         queries = previous_result["query"].tolist()
```

### Comparing `autorag-0.1.7/autorag/nodes/passageaugmenter/prev_next_augmenter.py` & `autorag-0.1.8/autorag/nodes/passageaugmenter/prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passageaugmenter/run.py` & `autorag-0.1.8/autorag/nodes/passageaugmenter/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagecompressor/base.py` & `autorag-0.1.8/autorag/nodes/passagecompressor/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import functools
+import logging
 from pathlib import Path
 from typing import List, Union, Dict
 
 import pandas as pd
 from llama_index.core.service_context_elements.llm_predictor import LLMPredictorType
 
 from autorag import generator_models
 from autorag.utils import result_to_dataframe
 
+logger = logging.getLogger("AutoRAG")
+
 
 def passage_compressor_node(func):
     @functools.wraps(func)
     @result_to_dataframe(['retrieved_contents'])
     def wrapper(
             project_dir: Union[str, Path],
             previous_result: pd.DataFrame,
             *args, **kwargs) -> List[List[str]]:
+        logger.info(f"Running generator node - {func.__name__} module...")
         assert all([column in previous_result.columns for column in
                     ['query', 'retrieved_contents', 'retrieved_ids', 'retrieve_scores']]), \
             "previous_result must have retrieved_contents, retrieved_ids, and retrieve_scores columns."
         assert len(previous_result) > 0, "previous_result must have at least one row."
 
         queries = previous_result['query'].tolist()
         retrieved_contents = previous_result['retrieved_contents'].tolist()
```

### Comparing `autorag-0.1.7/autorag/nodes/passagecompressor/refine.py` & `autorag-0.1.8/autorag/nodes/passagecompressor/refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagecompressor/run.py` & `autorag-0.1.8/autorag/nodes/passagecompressor/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagecompressor/tree_summarize.py` & `autorag-0.1.8/autorag/nodes/passagecompressor/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagefilter/base.py` & `autorag-0.1.8/autorag/nodes/passagefilter/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import functools
+import logging
 import os
 from pathlib import Path
 from typing import Union, Tuple, List
 
 import pandas as pd
 
 from autorag.utils import result_to_dataframe, validate_qa_dataset, fetch_contents
 
+logger = logging.getLogger("AutoRAG")
+
 
 # same with passage filter from now
 def passage_filter_node(func):
     @functools.wraps(func)
     @result_to_dataframe(['retrieved_contents', 'retrieved_ids', 'retrieve_scores'])
     def wrapper(
             project_dir: Union[str, Path],
             previous_result: pd.DataFrame,
             *args, **kwargs) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
+        logger.info(f"Running passage filter node - {func.__name__} module...")
         validate_qa_dataset(previous_result)
 
         # find queries columns
         assert "query" in previous_result.columns, "previous_result must have query column."
         queries = previous_result["query"].tolist()
 
         # find contents_list columns
```

### Comparing `autorag-0.1.7/autorag/nodes/passagefilter/percentile_cutoff.py` & `autorag-0.1.8/autorag/nodes/passagefilter/percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagefilter/recency.py` & `autorag-0.1.8/autorag/nodes/passagefilter/recency.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagefilter/run.py` & `autorag-0.1.8/autorag/nodes/passagefilter/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagefilter/threshold_cutoff.py` & `autorag-0.1.8/autorag/nodes/passagefilter/threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/base.py` & `autorag-0.1.8/autorag/nodes/passagereranker/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 def passage_reranker_node(func):
     @functools.wraps(func)
     @result_to_dataframe(["retrieved_contents", "retrieved_ids", "retrieve_scores"])
     def wrapper(
             project_dir: Union[str, Path],
             previous_result: pd.DataFrame,
             *args, **kwargs) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
+        logger.info(f"Running passage reranker node - {func.__name__} module...")
         validate_qa_dataset(previous_result)
 
         # find queries columns
         assert "query" in previous_result.columns, "previous_result must have query column."
         queries = previous_result["query"].tolist()
 
         # find contents_list columns
```

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/cohere.py` & `autorag-0.1.8/autorag/nodes/passagereranker/cohere.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/colbert.py` & `autorag-0.1.8/autorag/nodes/passagereranker/colbert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Tuple
 
 import numpy as np
 import pandas as pd
 import torch
+from tqdm import tqdm
 from transformers import AutoModel, AutoTokenizer
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
 from autorag.utils.util import flatten_apply, sort_by_scores, select_top_k
 
 
 @passage_reranker_node
@@ -64,16 +65,16 @@
                                 model, tokenizer, batch_size: int) -> List[np.array]:
 
     encoding = tokenizer(input_strings, return_tensors="pt", padding=True, truncation=True,
                          max_length=model.config.max_position_embeddings)
 
     input_batches = slice_tokenizer_result(encoding, batch_size)
     result_embedding = []
-    for encoding in input_batches:
-        result_embedding.append(model(**encoding).last_hidden_state)
+    for encoding_batch in tqdm(input_batches):
+        result_embedding.append(model(**encoding_batch).last_hidden_state)
     total_tensor = torch.cat(result_embedding, dim=0)  # shape [batch_size, token_length, embedding_dim]
     tensor_results = list(total_tensor.chunk(total_tensor.size()[0]))
 
     if torch.cuda.is_available():
         return list(map(lambda x: x.detach().cpu().numpy(), tensor_results))
     else:
         return list(map(lambda x: x.detach().numpy(), tensor_results))
```

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/flag_embedding.py` & `autorag-0.1.8/autorag/nodes/passagereranker/flag_embedding.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Tuple
 
 import pandas as pd
 import torch
 from FlagEmbedding import FlagReranker
+from tqdm import tqdm
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
 from autorag.utils.util import make_batch, sort_by_scores, flatten_apply, select_top_k
 
 
 @passage_reranker_node
 def flag_embedding_reranker(queries: List[str], contents_list: List[List[str]],
@@ -50,15 +51,15 @@
 
     return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
 
 
 def flag_embedding_run_model(input_texts, model, batch_size: int):
     batch_input_texts = make_batch(input_texts, batch_size)
     results = []
-    for batch_texts in batch_input_texts:
+    for batch_texts in tqdm(batch_input_texts):
         with torch.no_grad():
             pred_scores = model.compute_score(sentence_pairs=batch_texts)
         if batch_size == 1:
             results.append(pred_scores)
         else:
             results.extend(pred_scores)
     return results
```

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/flag_embedding_llm.py` & `autorag-0.1.8/autorag/nodes/passagereranker/flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/jina.py` & `autorag-0.1.8/autorag/nodes/passagereranker/jina.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/koreranker.py` & `autorag-0.1.8/autorag/nodes/passagereranker/koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/monot5.py` & `autorag-0.1.8/autorag/nodes/passagereranker/monot5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from itertools import chain
 from typing import List, Tuple
 
 import pandas as pd
 import torch
+from tqdm import tqdm
 from transformers import T5Tokenizer, T5ForConditionalGeneration
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
 from autorag.utils.util import make_batch, sort_by_scores, flatten_apply, select_top_k
 
 prediction_tokens = {
     'castorini/monot5-base-msmarco': ['▁false', '▁true'],
@@ -88,15 +89,15 @@
 
     return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
 
 
 def monot5_run_model(input_texts, model, batch_size: int, tokenizer, device, token_false_id, token_true_id):
     batch_input_texts = make_batch(input_texts, batch_size)
     results = []
-    for batch_texts in batch_input_texts:
+    for batch_texts in tqdm(batch_input_texts):
         flattened_batch_texts = list(chain.from_iterable(batch_texts))
         input_encodings = tokenizer(flattened_batch_texts, padding=True, truncation=True, max_length=512,
                                     return_tensors='pt').to(
             device)
         with torch.no_grad():
             outputs = model.generate(input_ids=input_encodings['input_ids'],
                                      attention_mask=input_encodings['attention_mask'],
```

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/pass_reranker.py` & `autorag-0.1.8/autorag/nodes/passagereranker/pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/rankgpt.py` & `autorag-0.1.8/autorag/nodes/passagereranker/rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/run.py` & `autorag-0.1.8/autorag/nodes/passagereranker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/sentence_transformer.py` & `autorag-0.1.8/autorag/nodes/passagereranker/sentence_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Tuple
 
 import pandas as pd
 import torch
 from sentence_transformers import CrossEncoder
+from tqdm import tqdm
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
 from autorag.utils.util import flatten_apply, make_batch, select_top_k, sort_by_scores
 
 
 @passage_reranker_node
 def sentence_transformer_reranker(queries: List[str], contents_list: List[List[str]],
@@ -50,12 +51,12 @@
 
     return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
 
 
 def sentence_transformer_run_model(input_texts, model, batch_size: int):
     batch_input_texts = make_batch(input_texts, batch_size)
     results = []
-    for batch_texts in batch_input_texts:
+    for batch_texts in tqdm(batch_input_texts):
         with torch.no_grad():
             pred_scores = model.predict(sentences=batch_texts, apply_softmax=True)
         results.extend(pred_scores.tolist())
     return results
```

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/tart/modeling_enc_t5.py` & `autorag-0.1.8/autorag/nodes/passagereranker/tart/modeling_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/tart/tart.py` & `autorag-0.1.8/autorag/nodes/passagereranker/tart/tart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from itertools import chain
 from typing import List, Tuple
 
 import pandas as pd
 import torch
 import torch.nn.functional as F
+from tqdm import tqdm
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
 from autorag.nodes.passagereranker.tart.modeling_enc_t5 import EncT5ForSequenceClassification
 from autorag.nodes.passagereranker.tart.tokenization_enc_t5 import EncT5Tokenizer
 from autorag.utils.util import make_batch, sort_by_scores, flatten_apply, select_top_k
 
 
@@ -64,15 +65,15 @@
 
 def tart_run_model(input_texts, contents_list, model, batch_size: int, tokenizer, device):
     flattened_texts = list(chain.from_iterable(input_texts))
     flattened_contents = list(chain.from_iterable(contents_list))
     batch_input_texts = make_batch(flattened_texts, batch_size)
     batch_contents_list = make_batch(flattened_contents, batch_size)
     results = []
-    for batch_texts, batch_contents in zip(batch_input_texts, batch_contents_list):
+    for batch_texts, batch_contents in tqdm(zip(batch_input_texts, batch_contents_list)):
         feature = tokenizer(batch_texts, batch_contents, padding=True, truncation=True,
                             return_tensors="pt").to(device)
         with torch.no_grad():
             pred_scores = model(**feature).logits
             normalized_scores = [float(score[1]) for score in F.softmax(pred_scores, dim=1)]
         results.extend(normalized_scores)
     return results
```

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py` & `autorag-0.1.8/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/time_reranker.py` & `autorag-0.1.8/autorag/nodes/passagereranker/time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/passagereranker/upr.py` & `autorag-0.1.8/autorag/nodes/passagereranker/upr.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,25 +49,27 @@
     df = pd.DataFrame({
         'query': queries,
         'contents': contents_list,
         'ids': ids_list,
     })
     ds = ray.data.from_pandas(df)
 
+    scorer = UPRScorer(suffix_prompt=suffix_prompt, prefix_prompt=prefix_prompt, use_bf16=use_bf16)
+
     if torch.cuda.is_available():
-        score_batch = ds.map_batches(UPRScorer(suffix_prompt=suffix_prompt,
-                                               prefix_prompt=prefix_prompt, use_bf16=use_bf16), batch_size=1,
+        score_batch = ds.map_batches(scorer, batch_size=1,
                                      concurrency=num_gpus, num_gpus=1)
     else:
-        score_batch = ds.map_batches(UPRScorer(suffix_prompt=suffix_prompt,
-                                               prefix_prompt=prefix_prompt, use_bf16=use_bf16),
+        score_batch = ds.map_batches(scorer,
                                      batch_size=1,
                                      concurrency=min(len(df), os.cpu_count()), num_cpus=os.cpu_count())
     scores = score_batch.to_pandas()['output'].tolist()  # converted to a flatten list of scores
 
+    del scorer
+
     explode_df = df.explode('contents')
     explode_df['scores'] = scores
     df['scores'] = explode_df.groupby(level=0, sort=False)['scores'].apply(list).tolist()
     df[['contents', 'ids', 'scores']] = df.apply(lambda x: sort_by_scores(x, reverse=False), axis=1,
                                                  result_type='expand')
     results = select_top_k(df, ['contents', 'ids', 'scores'], top_k)
     return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
@@ -104,9 +106,10 @@
         log_softmax = torch.nn.functional.log_softmax(logits, dim=-1)
         nll = -log_softmax.gather(2, query_input_ids.unsqueeze(2)).squeeze(2)
         avg_nll = torch.sum(nll, dim=1)
         return {"output": avg_nll.tolist()}
 
     def __del__(self):
         del self.model
+        del self.tokenizer
         if torch.cuda.is_available():
             torch.cuda.empty_cache()
```

### Comparing `autorag-0.1.7/autorag/nodes/promptmaker/base.py` & `autorag-0.1.8/autorag/nodes/promptmaker/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import functools
+import logging
 from pathlib import Path
 from typing import List, Union
 
 import pandas as pd
 
 from autorag.utils import result_to_dataframe
 
+logger = logging.getLogger("AutoRAG")
+
 
 def prompt_maker_node(func):
     @functools.wraps(func)
     @result_to_dataframe(["prompts"])
     def wrapper(
             project_dir: Union[str, Path],
             previous_result: pd.DataFrame,
             *args, **kwargs) -> List[str]:
+        logger.info(f"Running prompt maker node - {func.__name__} module...")
         # get query and retrieved contents from previous_result
         assert "query" in previous_result.columns, "previous_result must have query column."
         assert "retrieved_contents" in previous_result.columns, "previous_result must have retrieved_contents column."
         query = previous_result["query"].tolist()
         retrieved_contents = previous_result["retrieved_contents"].tolist()
         prompt = kwargs.pop("prompt")
```

### Comparing `autorag-0.1.7/autorag/nodes/promptmaker/fstring.py` & `autorag-0.1.8/autorag/nodes/promptmaker/fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/promptmaker/long_context_reorder.py` & `autorag-0.1.8/autorag/nodes/promptmaker/long_context_reorder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
 from typing import List
 
+import numpy as np
+
 from autorag.nodes.promptmaker.base import prompt_maker_node
 
 logger = logging.getLogger("AutoRAG")
 
 
 @prompt_maker_node
 def long_context_reorder(prompt: str, queries: List[str], retrieved_contents: List[List[str]],
@@ -31,14 +33,16 @@
     :param retrieved_contents: List of retrieved contents.
     :param retrieve_scores: List of retrieve scores.
     :return: Prompts that made by long context reorder.
     """
 
     def long_context_reorder_row(_prompt: str, _query: str, _retrieved_contents: List[str],
                                  _retrieve_scores: List[float]) -> str:
+        if isinstance(_retrieved_contents, np.ndarray):
+            _retrieved_contents = _retrieved_contents.tolist()
         if not len(_retrieved_contents) == len(_retrieve_scores):
             logger.info("If you use a summarizer, the reorder will not proceed.")
             return _prompt.format(query=_query, retrieved_contents="\n\n".join(_retrieved_contents))
         content_scores = list(zip(_retrieved_contents, _retrieve_scores))
         sorted_content_scores = sorted(content_scores, key=lambda x: x[1], reverse=True)
         content_result, score_result = zip(*sorted_content_scores)
         _retrieved_contents.append(content_result[0])
```

### Comparing `autorag-0.1.7/autorag/nodes/promptmaker/run.py` & `autorag-0.1.8/autorag/nodes/promptmaker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/queryexpansion/base.py` & `autorag-0.1.8/autorag/nodes/queryexpansion/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 def query_expansion_node(func):
     @functools.wraps(func)
     @result_to_dataframe(["queries"])
     def wrapper(
             project_dir: Union[str, Path],
             previous_result: pd.DataFrame,
             *args, **kwargs) -> List[List[str]]:
+        logger.info(f"Running query expansion node - {func.__name__} module...")
         validate_qa_dataset(previous_result)
 
         # find queries columns
         assert "query" in previous_result.columns, "previous_result must have query column."
         queries = previous_result["query"].tolist()
 
         if func.__name__ == "pass_query_expansion":
```

### Comparing `autorag-0.1.7/autorag/nodes/queryexpansion/hyde.py` & `autorag-0.1.8/autorag/nodes/queryexpansion/hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/queryexpansion/query_decompose.py` & `autorag-0.1.8/autorag/nodes/queryexpansion/query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/queryexpansion/run.py` & `autorag-0.1.8/autorag/nodes/queryexpansion/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/retrieval/base.py` & `autorag-0.1.8/autorag/nodes/retrieval/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
     @functools.wraps(func)
     @result_to_dataframe(["retrieved_contents", "retrieved_ids", "retrieve_scores"])
     def wrapper(
             project_dir: Union[str, Path],
             previous_result: pd.DataFrame,
             **kwargs) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
+        logger.info(f"Running retrieval node - {func.__name__} module...")
         validate_qa_dataset(previous_result)
         resources_dir = os.path.join(project_dir, "resources")
         data_dir = os.path.join(project_dir, "data")
 
         if func.__name__ == "bm25":
             # check if bm25_path and file exists
             bm25_path = os.path.join(resources_dir, 'bm25.pkl')
```

### Comparing `autorag-0.1.7/autorag/nodes/retrieval/bm25.py` & `autorag-0.1.8/autorag/nodes/retrieval/bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/retrieval/hybrid_cc.py` & `autorag-0.1.8/autorag/nodes/retrieval/hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/retrieval/hybrid_dbsf.py` & `autorag-0.1.8/autorag/nodes/retrieval/hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/retrieval/hybrid_rrf.py` & `autorag-0.1.8/autorag/nodes/retrieval/hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/retrieval/hybrid_rsf.py` & `autorag-0.1.8/autorag/nodes/retrieval/hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/retrieval/run.py` & `autorag-0.1.8/autorag/nodes/retrieval/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/nodes/retrieval/vectordb.py` & `autorag-0.1.8/autorag/nodes/retrieval/vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/schema/module.py` & `autorag-0.1.8/autorag/schema/module.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/schema/node.py` & `autorag-0.1.8/autorag/schema/node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/strategy.py` & `autorag-0.1.8/autorag/strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/support.py` & `autorag-0.1.8/autorag/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         'vectordb': ('autorag.nodes.retrieval', 'vectordb'),
         'hybrid_rrf': ('autorag.nodes.retrieval', 'hybrid_rrf'),
         'hybrid_cc': ('autorag.nodes.retrieval', 'hybrid_cc'),
         'hybrid_rsf': ('autorag.nodes.retrieval', 'hybrid_rsf'),
         'hybrid_dbsf': ('autorag.nodes.retrieval', 'hybrid_dbsf'),
         # passage_augmenter
         'prev_next_augmenter': ('autorag.nodes.passageaugmenter', 'prev_next_augmenter'),
+        'pass_passage_augmenter': ('autorag.nodes.passageaugmenter', 'pass_passage_augmenter'),
         # passage_reranker
         'monot5': ('autorag.nodes.passagereranker', 'monot5'),
         'tart': ('autorag.nodes.passagereranker', 'tart'),
         'upr': ('autorag.nodes.passagereranker', 'upr'),
         'koreranker': ('autorag.nodes.passagereranker', 'koreranker'),
         'pass_reranker': ('autorag.nodes.passagereranker', 'pass_reranker'),
         'cohere_reranker': ('autorag.nodes.passagereranker', 'cohere_reranker'),
```

### Comparing `autorag-0.1.7/autorag/utils/preprocess.py` & `autorag-0.1.8/autorag/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/autorag/utils/util.py` & `autorag-0.1.8/autorag/utils/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import ast
 import asyncio
+import datetime
 import functools
 import itertools
 import logging
 import os
 import re
 import string
 from copy import deepcopy
@@ -76,20 +77,39 @@
     if dict_columns is None:
         dict_columns = ['module_params']
 
     if any([col not in summary_df.columns for col in dict_columns]):
         raise ValueError(f"{dict_columns} must be in summary_df.columns.")
 
     def convert_dict(elem):
-        return ast.literal_eval(elem)
+        try:
+            return ast.literal_eval(elem)
+        except:
+            # convert datetime or date to its object (recency filter)
+            date_object = convert_datetime_string(elem)
+            if date_object is None:
+                raise ValueError(f"Malformed dict received : {elem}\nCan't convert to dict properly")
+            return {'threshold': date_object}
 
     summary_df[dict_columns] = summary_df[dict_columns].applymap(convert_dict)
     return summary_df
 
 
+def convert_datetime_string(s):
+    # Regex to extract datetime arguments from the string
+    m = re.search(r"(datetime|date)(\((\d+)(,\s*\d+)*\))", s)
+    if m:
+        args = ast.literal_eval(m.group(2))
+        if m.group(1) == 'datetime':
+            return datetime.datetime(*args)
+        elif m.group(1) == 'date':
+            return datetime.date(*args)
+    return None
+
+
 def make_combinations(target_dict: Dict[str, Any]) -> List[Dict[str, Any]]:
     """
     Make combinations from target_dict.
     The target_dict key value must be a string,
     and the value can be list of values or single value.
     If generates all combinations of values from target_dict,
     which means generated dictionaries that contain only one value for each key,
```

### Comparing `autorag-0.1.7/autorag/web.py` & `autorag-0.1.8/autorag/web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/Makefile` & `autorag-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/make.bat` & `autorag-0.1.8/docs/make.bat`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-@ECHO OFF
-
-pushd %~dp0
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=sphinx-build
-)
-set SOURCEDIR=source
-set BUILDDIR=build
-
-%SPHINXBUILD% >NUL 2>NUL
-if errorlevel 9009 (
-	echo.
-	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
-	echo.installed, then set the SPHINXBUILD environment variable to point
-	echo.to the full path of the 'sphinx-build' executable. Alternatively you
-	echo.may add the Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.https://www.sphinx-doc.org/
-	exit /b 1
-)
-
-if "%1" == "" goto help
-
-%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-goto end
-
-:help
-%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-
-:end
-popd
+@ECHO OFF
+
+pushd %~dp0
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=sphinx-build
+)
+set SOURCEDIR=source
+set BUILDDIR=build
+
+%SPHINXBUILD% >NUL 2>NUL
+if errorlevel 9009 (
+	echo.
+	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+	echo.installed, then set the SPHINXBUILD environment variable to point
+	echo.to the full path of the 'sphinx-build' executable. Alternatively you
+	echo.may add the Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.https://www.sphinx-doc.org/
+	exit /b 1
+)
+
+if "%1" == "" goto help
+
+%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+goto end
+
+:help
+%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+
+:end
+popd
```

### Comparing `autorag-0.1.7/docs/source/_static/data_creation.png` & `autorag-0.1.8/docs/source/_static/data_creation.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/data_folder.png` & `autorag-0.1.8/docs/source/_static/data_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/node_folder.png` & `autorag-0.1.8/docs/source/_static/node_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/node_line_folder.png` & `autorag-0.1.8/docs/source/_static/node_line_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/node_line_summary.png` & `autorag-0.1.8/docs/source/_static/node_line_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/node_lines.png` & `autorag-0.1.8/docs/source/_static/node_lines.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/node_summary.png` & `autorag-0.1.8/docs/source/_static/node_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/project_folder_example.png` & `autorag-0.1.8/docs/source/_static/project_folder_example.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/project_folders.png` & `autorag-0.1.8/docs/source/_static/project_folders.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/resources_folder.png` & `autorag-0.1.8/docs/source/_static/resources_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/roadmap/RAG_paradigms.png` & `autorag-0.1.8/docs/source/_static/roadmap/RAG_paradigms.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/roadmap/advanced_RAG.png` & `autorag-0.1.8/docs/source/_static/roadmap/advanced_RAG.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/roadmap/cycle.png` & `autorag-0.1.8/docs/source/_static/roadmap/cycle.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/roadmap/merger.png` & `autorag-0.1.8/docs/source/_static/roadmap/merger.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/roadmap/node_line_modular.png` & `autorag-0.1.8/docs/source/_static/roadmap/node_line_modular.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/roadmap/policy.png` & `autorag-0.1.8/docs/source/_static/roadmap/policy.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/samsung_sundae.jpeg` & `autorag-0.1.8/docs/source/_static/samsung_sundae.jpeg`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/trial_folder.png` & `autorag-0.1.8/docs/source/_static/trial_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/trial_json.png` & `autorag-0.1.8/docs/source/_static/trial_json.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/trial_summary.png` & `autorag-0.1.8/docs/source/_static/trial_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/_static/web_interface.png` & `autorag-0.1.8/docs/source/_static/web_interface.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.data.corpus.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.data.corpus.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.data.qacreation.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.data.qacreation.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.evaluate.metric.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.evaluate.metric.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.evaluate.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.evaluate.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.nodes.generator.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.nodes.generator.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.nodes.passageaugmenter.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.nodes.passageaugmenter.rst`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 ------------------------------------------
 
 .. automodule:: autorag.nodes.passageaugmenter.base
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.passageaugmenter.pass\_passage\_augmenter module
+--------------------------------------------------------------
+
+.. automodule:: autorag.nodes.passageaugmenter.pass_passage_augmenter
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.passageaugmenter.prev\_next\_augmenter module
 -----------------------------------------------------------
 
 .. automodule:: autorag.nodes.passageaugmenter.prev_next_augmenter
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagecompressor.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagecompressor.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagefilter.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagefilter.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagereranker.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagereranker.rst`

 * *Files 1% similar despite different names*

```diff
@@ -56,22 +56,14 @@
 -----------------------------------------
 
 .. automodule:: autorag.nodes.passagereranker.jina
    :members:
    :undoc-members:
    :show-inheritance:
 
-autorag.nodes.passagereranker.just\_lab module
-----------------------------------------------
-
-.. automodule:: autorag.nodes.passagereranker.just_lab
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
 autorag.nodes.passagereranker.koreranker module
 -----------------------------------------------
 
 .. automodule:: autorag.nodes.passagereranker.koreranker
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.nodes.promptmaker.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.nodes.promptmaker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.nodes.queryexpansion.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.nodes.queryexpansion.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.nodes.retrieval.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.nodes.retrieval.rst`

 * *Files 2% similar despite different names*

```diff
@@ -48,22 +48,14 @@
 ------------------------------------------
 
 .. automodule:: autorag.nodes.retrieval.hybrid_rsf
    :members:
    :undoc-members:
    :show-inheritance:
 
-autorag.nodes.retrieval.recursive\_chunk module
------------------------------------------------
-
-.. automodule:: autorag.nodes.retrieval.recursive_chunk
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
 autorag.nodes.retrieval.run module
 ----------------------------------
 
 .. automodule:: autorag.nodes.retrieval.run
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `autorag-0.1.7/docs/source/api_spec/autorag.rst` & `autorag-0.1.8/docs/source/api_spec/autorag.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/conf.py` & `autorag-0.1.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/data_creation/data_format.md` & `autorag-0.1.8/docs/source/data_creation/data_format.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/data_creation/ragas.md` & `autorag-0.1.8/docs/source/data_creation/ragas.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/data_creation/tutorial.md` & `autorag-0.1.8/docs/source/data_creation/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/deploy/api_endpoint.md` & `autorag-0.1.8/docs/source/deploy/api_endpoint.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/deploy/web.md` & `autorag-0.1.8/docs/source/deploy/web.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/index.rst` & `autorag-0.1.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/install.md` & `autorag-0.1.8/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/local_model.md` & `autorag-0.1.8/docs/source/local_model.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/generator/generator.md` & `autorag-0.1.8/docs/source/nodes/generator/generator.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/generator/llama_index_llm.md` & `autorag-0.1.8/docs/source/nodes/generator/llama_index_llm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/generator/vllm.md` & `autorag-0.1.8/docs/source/nodes/generator/vllm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_augmenter/passage_augmenter.md` & `autorag-0.1.8/docs/source/nodes/passage_augmenter/passage_augmenter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_augmenter/prev_next_augmenter.md` & `autorag-0.1.8/docs/source/nodes/passage_augmenter/prev_next_augmenter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_compressor/passage_compressor.md` & `autorag-0.1.8/docs/source/nodes/passage_compressor/passage_compressor.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_compressor/refine.md` & `autorag-0.1.8/docs/source/nodes/passage_compressor/refine.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_compressor/tree_summarize.md` & `autorag-0.1.8/docs/source/nodes/passage_compressor/tree_summarize.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_filter/passage_filter.md` & `autorag-0.1.8/docs/source/nodes/passage_filter/passage_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_filter/recency_filter.md` & `autorag-0.1.8/docs/source/nodes/passage_filter/recency_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md` & `autorag-0.1.8/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md` & `autorag-0.1.8/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_reranker/cohere.md` & `autorag-0.1.8/docs/source/nodes/passage_reranker/cohere.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_reranker/colbert.md` & `autorag-0.1.8/docs/source/nodes/passage_reranker/colbert.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md` & `autorag-0.1.8/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_reranker/flag_embedding_reranker.md` & `autorag-0.1.8/docs/source/nodes/passage_reranker/flag_embedding_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_reranker/jina_reranker.md` & `autorag-0.1.8/docs/source/nodes/passage_reranker/jina_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_reranker/monot5.md` & `autorag-0.1.8/docs/source/nodes/passage_reranker/monot5.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_reranker/passage_reranker.md` & `autorag-0.1.8/docs/source/nodes/passage_reranker/passage_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_reranker/rankgpt.md` & `autorag-0.1.8/docs/source/nodes/passage_reranker/rankgpt.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md` & `autorag-0.1.8/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_reranker/tart.md` & `autorag-0.1.8/docs/source/nodes/passage_reranker/tart.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_reranker/time_reranker.md` & `autorag-0.1.8/docs/source/nodes/passage_reranker/time_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/passage_reranker/upr.md` & `autorag-0.1.8/docs/source/nodes/passage_reranker/upr.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/prompt_maker/fstring.md` & `autorag-0.1.8/docs/source/nodes/prompt_maker/fstring.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/prompt_maker/long_context_reorder.md` & `autorag-0.1.8/docs/source/nodes/prompt_maker/long_context_reorder.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/prompt_maker/prompt_maker.md` & `autorag-0.1.8/docs/source/nodes/prompt_maker/prompt_maker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/query_expansion/hyde.md` & `autorag-0.1.8/docs/source/nodes/query_expansion/hyde.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/query_expansion/query_decompose.md` & `autorag-0.1.8/docs/source/nodes/query_expansion/query_decompose.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/query_expansion/query_expansion.md` & `autorag-0.1.8/docs/source/nodes/query_expansion/query_expansion.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/retrieval/bm25.md` & `autorag-0.1.8/docs/source/nodes/retrieval/bm25.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/retrieval/hybrid_cc.md` & `autorag-0.1.8/docs/source/nodes/retrieval/hybrid_cc.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/retrieval/hybrid_dbsf.md` & `autorag-0.1.8/docs/source/nodes/retrieval/hybrid_dbsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/retrieval/hybrid_rrf.md` & `autorag-0.1.8/docs/source/nodes/retrieval/hybrid_rrf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/retrieval/hybrid_rsf.md` & `autorag-0.1.8/docs/source/nodes/retrieval/hybrid_rsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/retrieval/retrieval.md` & `autorag-0.1.8/docs/source/nodes/retrieval/retrieval.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/nodes/retrieval/vectordb.md` & `autorag-0.1.8/docs/source/nodes/retrieval/vectordb.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/optimization/custom_config.md` & `autorag-0.1.8/docs/source/optimization/custom_config.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/optimization/folder_structure.md` & `autorag-0.1.8/docs/source/optimization/folder_structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/optimization/optimization.md` & `autorag-0.1.8/docs/source/optimization/optimization.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/optimization/sample_full_config.yaml` & `autorag-0.1.8/docs/source/optimization/sample_full_config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/roadmap/modular_rag.md` & `autorag-0.1.8/docs/source/roadmap/modular_rag.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/structure.md` & `autorag-0.1.8/docs/source/structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/troubleshooting.md` & `autorag-0.1.8/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/docs/source/tutorial.md` & `autorag-0.1.8/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/pyproject.toml` & `autorag-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/requirements.txt` & `autorag-0.1.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/sample_config/compact_local.yaml` & `autorag-0.1.8/sample_config/compact_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/sample_config/compact_openai.yaml` & `autorag-0.1.8/sample_config/compact_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/sample_config/config_korean.yaml` & `autorag-0.1.8/sample_config/config_korean.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/sample_config/extracted_sample.yaml` & `autorag-0.1.8/sample_config/extracted_sample.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/sample_config/full.yaml` & `autorag-0.1.8/sample_config/full.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/sample_config/simple_local.yaml` & `autorag-0.1.8/sample_config/simple_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/sample_config/simple_openai.yaml` & `autorag-0.1.8/sample_config/simple_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/sample_dataset/README.md` & `autorag-0.1.8/sample_dataset/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/sample_dataset/eli5/load_eli5_dataset.py` & `autorag-0.1.8/sample_dataset/eli5/load_eli5_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/sample_dataset/msmarco/load_msmarco_dataset.py` & `autorag-0.1.8/sample_dataset/msmarco/load_msmarco_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/sample_dataset/triviaqa/load_triviaqa_dataset.py` & `autorag-0.1.8/sample_dataset/triviaqa/load_triviaqa_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/data/corpus/test_base.py` & `autorag-0.1.8/tests/autorag/data/corpus/test_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/data/corpus/test_langchain.py` & `autorag-0.1.8/tests/autorag/data/corpus/test_langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/data/corpus/test_llama_index_corpus.py` & `autorag-0.1.8/tests/autorag/data/corpus/test_llama_index_corpus.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/data/qacreation/test_base_qacreation.py` & `autorag-0.1.8/tests/autorag/data/qacreation/test_base_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/data/qacreation/test_llama_index_qacreation.py` & `autorag-0.1.8/tests/autorag/data/qacreation/test_llama_index_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/data/qacreation/test_ragas_qa_creation.py` & `autorag-0.1.8/tests/autorag/data/qacreation/test_ragas_qa_creation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/data/qacreation/test_simple.py` & `autorag-0.1.8/tests/autorag/data/qacreation/test_simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/evaluate/metric/test_generation_metric.py` & `autorag-0.1.8/tests/autorag/evaluate/metric/test_generation_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py` & `autorag-0.1.8/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/evaluate/metric/test_retrieval_metric.py` & `autorag-0.1.8/tests/autorag/evaluate/metric/test_retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/evaluate/test_evaluate_util.py` & `autorag-0.1.8/tests/autorag/evaluate/test_evaluate_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/evaluate/test_generation_evaluate.py` & `autorag-0.1.8/tests/autorag/evaluate/test_generation_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/evaluate/test_retrieval_contents_evaluate.py` & `autorag-0.1.8/tests/autorag/evaluate/test_retrieval_contents_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/evaluate/test_retrieval_evaluate.py` & `autorag-0.1.8/tests/autorag/evaluate/test_retrieval_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/generator/test_generator_base.py` & `autorag-0.1.8/tests/autorag/nodes/generator/test_generator_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/generator/test_llama_index_llm.py` & `autorag-0.1.8/tests/autorag/nodes/generator/test_llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/generator/test_run_generator_node.py` & `autorag-0.1.8/tests/autorag/nodes/generator/test_run_generator_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/generator/test_vllm.py` & `autorag-0.1.8/tests/autorag/nodes/generator/test_vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py` & `autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py` & `autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py` & `autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py` & `autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py` & `autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_pass_compressor.py` & `autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_pass_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_refine.py` & `autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py` & `autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_tree_summarize.py` & `autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py` & `autorag-0.1.8/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagefilter/test_passage_filter_base.py` & `autorag-0.1.8/tests/autorag/nodes/passagefilter/test_passage_filter_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagefilter/test_passage_filter_run.py` & `autorag-0.1.8/tests/autorag/nodes/passagefilter/test_passage_filter_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py` & `autorag-0.1.8/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagefilter/test_recency_filter.py` & `autorag-0.1.8/tests/autorag/nodes/passagefilter/test_recency_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py` & `autorag-0.1.8/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_cohere_reranker.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_cohere_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_colbert_reranker.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_flag_embedding.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_jina_reranker.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_jina_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_koreranker.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_monot5.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_pass_reranker.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_rankgpt.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_sentence_transformer.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_tart.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_tart.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_time_reranker.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_upr.py` & `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_upr.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/promptmaker/test_fstring.py` & `autorag-0.1.8/tests/autorag/nodes/promptmaker/test_fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/promptmaker/test_long_context_reorder.py` & `autorag-0.1.8/tests/autorag/nodes/promptmaker/test_long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py` & `autorag-0.1.8/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py` & `autorag-0.1.8/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_hyde.py` & `autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py` & `autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_query_decompose.py` & `autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py` & `autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py` & `autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/retrieval/test_bm25.py` & `autorag-0.1.8/tests/autorag/nodes/retrieval/test_bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_base.py` & `autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_cc.py` & `autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py` & `autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_rrf.py` & `autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_rsf.py` & `autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/retrieval/test_retrieval_base.py` & `autorag-0.1.8/tests/autorag/nodes/retrieval/test_retrieval_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/retrieval/test_run_retrieval_node.py` & `autorag-0.1.8/tests/autorag/nodes/retrieval/test_run_retrieval_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/nodes/retrieval/test_vectordb.py` & `autorag-0.1.8/tests/autorag/nodes/retrieval/test_vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/schema/test_module_schema.py` & `autorag-0.1.8/tests/autorag/schema/test_module_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/schema/test_node_schema.py` & `autorag-0.1.8/tests/autorag/schema/test_node_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/test_cli.py` & `autorag-0.1.8/tests/autorag/test_cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/test_deploy.py` & `autorag-0.1.8/tests/autorag/test_deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/test_evaluator.py` & `autorag-0.1.8/tests/autorag/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/test_strategy.py` & `autorag-0.1.8/tests/autorag/test_strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/test_web.py` & `autorag-0.1.8/tests/autorag/test_web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/utils/test_preprocess.py` & `autorag-0.1.8/tests/autorag/utils/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/autorag/utils/test_util.py` & `autorag-0.1.8/tests/autorag/utils/test_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import asyncio
 import itertools
 import os
 import pathlib
 import tempfile
-from datetime import datetime
+from datetime import datetime, date
 
 import pandas as pd
 import pytest
 import tiktoken
 from llama_index.core.llms import CompletionResponse
 
 from autorag.utils import fetch_contents
 from autorag.utils.util import load_summary_file, result_to_dataframe, \
     make_combinations, explode, replace_value_in_dict, normalize_string, convert_string_to_tuple_in_dict, process_batch, \
-    convert_env_in_dict, openai_truncate_by_token
+    convert_env_in_dict, openai_truncate_by_token, convert_datetime_string
 from tests.mock import MockLLM
 
 root_dir = pathlib.PurePath(os.path.dirname(os.path.realpath(__file__))).parent.parent
 
 summary_df = pd.DataFrame({
     'best_module_name': ['bm25', 'upr', 'gpt-4'],
     'best_module_params': [{'top_k': 50}, {'model': 'llama-2', 'havertz': 'chelsea'}, {'top_p': 0.9}],
@@ -82,14 +82,36 @@
 def test_load_summary_file(summary_path):
     with pytest.raises(ValueError):
         load_summary_file(summary_path)
     df = load_summary_file(summary_path, ['best_module_params'])
     assert df.equals(summary_df)
 
 
+def test_load_summary_file_recency_filter():
+    df = pd.DataFrame({
+        'module_name': ['havertz', 'recency_filter'],
+        'module_params': [{'jazz': 'eastsidegunn'},
+                          {'threshold': datetime(2022, 1, 3, 0, 1, 3)}],
+    })
+    with tempfile.NamedTemporaryFile(suffix='.csv') as csv_file:
+        df.to_csv(csv_file.name, index=False)
+        load_df = load_summary_file(csv_file.name)
+        assert load_df.equals(df)
+
+
+def test_convert_datetime_string():
+    datetime_dict = {'threshold': datetime(2022, 1, 3, 0, 0, 3)}
+    date_dict = {'threshold': date(2001, 7, 11)}
+    result1 = convert_datetime_string(str(datetime_dict))
+    result2 = convert_datetime_string(str(date_dict))
+
+    assert result1 == datetime_dict['threshold']
+    assert result2 == date_dict['threshold']
+
+
 def test_result_to_dataframe():
     @result_to_dataframe(['col_1', 'col_2'])
     def func1():
         return [1, 2], [3, 4]
 
     result1 = func1()
     assert isinstance(result1, pd.DataFrame)
```

### Comparing `autorag-0.1.7/tests/delete_tests.py` & `autorag-0.1.8/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/mock.py` & `autorag-0.1.8/tests/mock.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/README.md` & `autorag-0.1.8/tests/resources/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/corpus_data_sample.parquet` & `autorag-0.1.8/tests/resources/corpus_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/data_creation/raw_dir/sample1.txt` & `autorag-0.1.8/tests/resources/data_creation/raw_dir/sample1.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/data_creation/raw_dir/sample2.txt` & `autorag-0.1.8/tests/resources/data_creation/raw_dir/sample2.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/data_creation/raw_dir/sample3.txt` & `autorag-0.1.8/tests/resources/data_creation/raw_dir/sample3.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/full.yaml` & `autorag-0.1.8/tests/resources/full.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/qa_data_sample.parquet` & `autorag-0.1.8/tests/resources/qa_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/qa_test_data_sample.parquet` & `autorag-0.1.8/tests/resources/qa_test_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/config.yaml` & `autorag-0.1.8/tests/resources/result_project/0/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet` & `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet` & `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet` & `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet` & `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet` & `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet` & `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet` & `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv` & `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet` & `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet` & `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv` & `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/0/summary.csv` & `autorag-0.1.8/tests/resources/result_project/0/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/1/config.yaml` & `autorag-0.1.8/tests/resources/result_project/1/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/config.yaml` & `autorag-0.1.8/tests/resources/result_project/2/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.8/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/3/config.yaml` & `autorag-0.1.8/tests/resources/result_project/3/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/best.yaml` & `autorag-0.1.8/tests/resources/result_project/best.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/data/corpus.parquet` & `autorag-0.1.8/tests/resources/result_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/data/qa.parquet` & `autorag-0.1.8/tests/resources/result_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/resources/bm25.pkl` & `autorag-0.1.8/tests/resources/result_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin` & `autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin` & `autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/result_project/resources/chroma/chroma.sqlite3` & `autorag-0.1.8/tests/resources/result_project/resources/chroma/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/sample_contents_nqa.csv` & `autorag-0.1.8/tests/resources/sample_contents_nqa.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/sample_project/data/corpus.parquet` & `autorag-0.1.8/tests/resources/sample_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/sample_project/data/qa.parquet` & `autorag-0.1.8/tests/resources/sample_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/sample_project/resources/bm25.pkl` & `autorag-0.1.8/tests/resources/sample_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/simple.yaml` & `autorag-0.1.8/tests/resources/simple.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.7/tests/resources/test_bm25_retrieval.pkl` & `autorag-0.1.8/tests/resources/test_bm25_retrieval.pkl`

 * *Files identical despite different names*

