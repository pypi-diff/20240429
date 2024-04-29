# Comparing `tmp/xagent-0.0.7.tar.gz` & `tmp/xagent-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xagent-0.0.7.tar", last modified: Mon Apr 22 05:37:01 2024, max compression
+gzip compressed data, was "xagent-0.0.8.tar", last modified: Mon Apr 29 03:01:01 2024, max compression
```

## Comparing `xagent-0.0.7.tar` & `xagent-0.0.8.tar`

### file list

```diff
@@ -1,58 +1,67 @@
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.480812 xagent-0.0.7/
--rw-r--r--   0 chenhao    (501) staff       (20)     1063 2024-03-14 09:35:14.000000 xagent-0.0.7/LICENSE
--rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-22 05:37:01.480610 xagent-0.0.7/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)     5501 2024-04-22 05:36:21.000000 xagent-0.0.7/README.md
--rw-r--r--   0 chenhao    (501) staff       (20)       38 2024-04-22 05:37:01.480900 xagent-0.0.7/setup.cfg
--rw-r--r--   0 chenhao    (501) staff       (20)     1207 2024-03-21 03:48:59.000000 xagent-0.0.7/setup.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.478470 xagent-0.0.7/tests/
--rw-r--r--   0 chenhao    (501) staff       (20)     2193 2024-04-19 07:38:46.000000 xagent-0.0.7/tests/test_job.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1830 2024-04-22 05:36:21.000000 xagent-0.0.7/tests/test_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2569 2024-04-15 04:02:55.000000 xagent-0.0.7/tests/test_local_model.py
--rw-r--r--   0 chenhao    (501) staff       (20)     6219 2024-04-19 08:20:14.000000 xagent-0.0.7/tests/test_xagent.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4747 2024-04-15 04:02:55.000000 xagent-0.0.7/tests/test_zhipu_api_model.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.480349 xagent-0.0.7/xagent.egg-info/
--rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-22 05:37:01.000000 xagent-0.0.7/xagent.egg-info/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)     1159 2024-04-22 05:37:01.000000 xagent-0.0.7/xagent.egg-info/SOURCES.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-22 05:37:01.000000 xagent-0.0.7/xagent.egg-info/dependency_links.txt
--rw-r--r--   0 chenhao    (501) staff       (20)      111 2024-04-22 05:37:01.000000 xagent-0.0.7/xagent.egg-info/requires.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        8 2024-04-22 05:37:01.000000 xagent-0.0.7/xagent.egg-info/top_level.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-22 05:37:01.000000 xagent-0.0.7/xagent.egg-info/zip-safe
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.467276 xagent-0.0.7/xagents/
--rw-r--r--   0 chenhao    (501) staff       (20)      667 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/__init__.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.468948 xagent-0.0.7/xagents/agent/
--rw-r--r--   0 chenhao    (501) staff       (20)      213 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/agent/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3426 2024-04-19 08:20:14.000000 xagent-0.0.7/xagents/agent/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2206 2024-04-19 08:20:14.000000 xagent-0.0.7/xagents/agent/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)      811 2024-04-08 07:28:32.000000 xagent-0.0.7/xagents/agent/memory.py
--rw-r--r--   0 chenhao    (501) staff       (20)     7784 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/agent/xagent.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1775 2024-04-19 08:20:14.000000 xagent-0.0.7/xagents/config.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.470966 xagent-0.0.7/xagents/kb/
--rw-r--r--   0 chenhao    (501) staff       (20)      178 2024-03-19 07:40:40.000000 xagent-0.0.7/xagents/kb/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     9629 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/kb/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     6559 2024-03-20 02:46:15.000000 xagent-0.0.7/xagents/kb/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)    11226 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/kb/kb.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2495 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/kb/kb_file.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4583 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/kb/vector_store.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.473122 xagent-0.0.7/xagents/loader/
--rw-r--r--   0 chenhao    (501) staff       (20)      152 2024-03-19 10:48:10.000000 xagent-0.0.7/xagents/loader/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4907 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/loader/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3874 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/loader/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)     5981 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/loader/docx_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)      863 2024-03-19 10:49:45.000000 xagent-0.0.7/xagents/loader/markdown.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3427 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/loader/pdf_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3365 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/loader/splitter.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1809 2024-04-08 07:28:32.000000 xagent-0.0.7/xagents/loader/structed.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.475114 xagent-0.0.7/xagents/model/
--rw-r--r--   0 chenhao    (501) staff       (20)      179 2024-03-20 06:50:45.000000 xagent-0.0.7/xagents/model/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2800 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/model/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2442 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/model/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2224 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/model/local.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1234 2024-03-21 07:20:01.000000 xagent-0.0.7/xagents/model/openai.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4064 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/model/zhipu.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.476762 xagent-0.0.7/xagents/tool/
--rw-r--r--   0 chenhao    (501) staff       (20)      226 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/tool/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1429 2024-04-19 08:20:14.000000 xagent-0.0.7/xagents/tool/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1641 2024-04-22 03:01:50.000000 xagent-0.0.7/xagents/tool/common_tool.py
--rw-r--r--   0 chenhao    (501) staff       (20)      463 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/tool/core.py
--rw-r--r--   0 chenhao    (501) staff       (20)     6766 2024-04-22 03:01:52.000000 xagent-0.0.7/xagents/tool/web_search.py
--rw-r--r--   0 chenhao    (501) staff       (20)      560 2024-04-19 07:38:46.000000 xagent-0.0.7/xagents/util.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.605608 xagent-0.0.8/
+-rw-r--r--   0 chenhao    (501) staff       (20)     1063 2024-03-14 09:35:14.000000 xagent-0.0.8/LICENSE
+-rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-29 03:01:01.605418 xagent-0.0.8/PKG-INFO
+-rw-r--r--   0 chenhao    (501) staff       (20)     5714 2024-04-29 02:59:57.000000 xagent-0.0.8/README.md
+-rw-r--r--   0 chenhao    (501) staff       (20)       38 2024-04-29 03:01:01.605661 xagent-0.0.8/setup.cfg
+-rw-r--r--   0 chenhao    (501) staff       (20)     1207 2024-03-21 03:48:59.000000 xagent-0.0.8/setup.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.603088 xagent-0.0.8/tests/
+-rw-r--r--   0 chenhao    (501) staff       (20)     2193 2024-04-19 07:38:46.000000 xagent-0.0.8/tests/test_job.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4058 2024-04-28 11:46:32.000000 xagent-0.0.8/tests/test_kb.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3422 2024-04-29 02:32:45.000000 xagent-0.0.8/tests/test_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2567 2024-04-29 02:35:16.000000 xagent-0.0.8/tests/test_local_model.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     8094 2024-04-25 05:55:07.000000 xagent-0.0.8/tests/test_xagent.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4747 2024-04-15 04:02:55.000000 xagent-0.0.8/tests/test_zhipu_api_model.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.605187 xagent-0.0.8/xagent.egg-info/
+-rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-29 03:01:01.000000 xagent-0.0.8/xagent.egg-info/PKG-INFO
+-rw-r--r--   0 chenhao    (501) staff       (20)     1432 2024-04-29 03:01:01.000000 xagent-0.0.8/xagent.egg-info/SOURCES.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-29 03:01:01.000000 xagent-0.0.8/xagent.egg-info/dependency_links.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)      210 2024-04-29 03:01:01.000000 xagent-0.0.8/xagent.egg-info/requires.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        8 2024-04-29 03:01:01.000000 xagent-0.0.8/xagent.egg-info/top_level.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-29 03:01:01.000000 xagent-0.0.8/xagent.egg-info/zip-safe
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.584305 xagent-0.0.8/xagents/
+-rw-r--r--   0 chenhao    (501) staff       (20)      667 2024-04-15 04:02:55.000000 xagent-0.0.8/xagents/__init__.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.586600 xagent-0.0.8/xagents/agent/
+-rw-r--r--   0 chenhao    (501) staff       (20)      213 2024-04-15 04:02:55.000000 xagent-0.0.8/xagents/agent/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3554 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/agent/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2206 2024-04-19 08:20:14.000000 xagent-0.0.8/xagents/agent/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      811 2024-04-08 07:28:32.000000 xagent-0.0.8/xagents/agent/memory.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     8093 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/agent/xagent.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1940 2024-04-25 06:21:58.000000 xagent-0.0.8/xagents/config.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.588957 xagent-0.0.8/xagents/kb/
+-rw-r--r--   0 chenhao    (501) staff       (20)      178 2024-03-19 07:40:40.000000 xagent-0.0.8/xagents/kb/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)    11768 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/kb/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     7948 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/kb/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)    13120 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/kb/kb.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3248 2024-04-25 02:50:51.000000 xagent-0.0.8/xagents/kb/kb_file.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     5516 2024-04-25 02:50:51.000000 xagent-0.0.8/xagents/kb/vector_store.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.595004 xagent-0.0.8/xagents/loader/
+-rw-r--r--   0 chenhao    (501) staff       (20)      152 2024-03-19 10:48:10.000000 xagent-0.0.8/xagents/loader/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     5379 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/loader/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4226 2024-04-25 06:23:17.000000 xagent-0.0.8/xagents/loader/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      945 2024-04-25 06:24:43.000000 xagent-0.0.8/xagents/loader/csv_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1388 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/loader/doc_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     6064 2024-04-29 02:27:35.000000 xagent-0.0.8/xagents/loader/docx_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1075 2024-04-25 06:24:55.000000 xagent-0.0.8/xagents/loader/excel_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1594 2024-04-25 02:50:51.000000 xagent-0.0.8/xagents/loader/json_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      842 2024-04-25 02:50:51.000000 xagent-0.0.8/xagents/loader/jsonl_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      961 2024-04-25 02:50:51.000000 xagent-0.0.8/xagents/loader/markdown_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3236 2024-04-29 02:27:35.000000 xagent-0.0.8/xagents/loader/pdf_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1328 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/loader/ppt_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2593 2024-04-29 02:27:35.000000 xagent-0.0.8/xagents/loader/pptx_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3374 2024-04-22 05:58:02.000000 xagent-0.0.8/xagents/loader/splitter.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1809 2024-04-08 07:28:32.000000 xagent-0.0.8/xagents/loader/structed.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1425 2024-04-29 02:27:35.000000 xagent-0.0.8/xagents/loader/utils.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.597709 xagent-0.0.8/xagents/model/
+-rw-r--r--   0 chenhao    (501) staff       (20)      179 2024-03-20 06:50:45.000000 xagent-0.0.8/xagents/model/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2800 2024-04-15 04:02:55.000000 xagent-0.0.8/xagents/model/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2426 2024-04-26 05:26:11.000000 xagent-0.0.8/xagents/model/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2243 2024-04-26 06:06:20.000000 xagent-0.0.8/xagents/model/local.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1234 2024-03-21 07:20:01.000000 xagent-0.0.8/xagents/model/openai.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4048 2024-04-26 05:26:29.000000 xagent-0.0.8/xagents/model/zhipu.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.600522 xagent-0.0.8/xagents/tool/
+-rw-r--r--   0 chenhao    (501) staff       (20)      226 2024-04-15 04:02:55.000000 xagent-0.0.8/xagents/tool/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1429 2024-04-19 08:20:14.000000 xagent-0.0.8/xagents/tool/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1641 2024-04-22 03:01:50.000000 xagent-0.0.8/xagents/tool/common_tool.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      463 2024-04-22 05:36:21.000000 xagent-0.0.8/xagents/tool/core.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     6639 2024-04-22 08:53:58.000000 xagent-0.0.8/xagents/tool/web_search.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      560 2024-04-19 07:38:46.000000 xagent-0.0.8/xagents/util.py
```

### Comparing `xagent-0.0.7/LICENSE` & `xagent-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xagent-0.0.7/README.md` & `xagent-0.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -130,14 +130,17 @@
 }
 ```
 
 - [支持csv格式、xlsx格式文件](https://dev.aminer.cn/solution-center-algorithm/XAgents/-/issues/26)
  - csv会load成一个表格
  - xlsx会load成多个表格，每个sheet一个表格
 
+- [支持json/jsonl格式文件上传](https://dev.aminer.cn/solution-center-algorithm/XAgents/-/issues/27)
+ - 支持json/jsonl格式，每个json-dict是一个chunk
+
 - [支持图片类型的chunk](https://dev.aminer.cn/solution-center-algorithm/XAgents/-/issues/24)
 示例chunk
 ```json
 {
   "content": "orc_result",
   "content_type": "IMAGE",
   "url":"http://cdn/file1-page1-image2.png",
@@ -190,7 +193,16 @@
   -H 'Content-Type: application/json' \
   -d '{
   "job_id": "job_id_xxx"
 }'
 ```
 
 
+
+
+
+## 20240429
+
+version: 0.0.8
+
+#### FEATURE
+
```

### Comparing `xagent-0.0.7/setup.py` & `xagent-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.7/tests/test_job.py` & `xagent-0.0.8/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.7/tests/test_loader.py` & `xagent-0.0.8/tests/test_loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,55 +5,103 @@
 @Author  :   ChenHao
 @Description  :   测试loader
 @Contact :   jerrychen1990@gmail.com
 '''
 from unittest import TestCase
 from loguru import logger
 from snippets import set_logger
-from xagents.loader.api import load_file
+from xagents.loader.api import load_file, parse_file
 from xagents.config import *
 from xagents.loader.common import *
 
 
 # unit test
-class TestEMBD(TestCase):
+class TestLoader(TestCase):
 
     @classmethod
     def setUpClass(cls):
         set_logger("dev", __name__)
         logger.info("start test embd")
 
     @classmethod
     def show_chunks(cls, chunks:Iterable[Chunk]):
         image_cnt = 0
         for chunk in chunks:
             logger.info(f"page={chunk.page_idx}, type={chunk.content_type}")
 
-            # logger.info(chunk.model_dump_json(indent=4, exclude_none=True, exclude={"data"}))
-            if isinstance(chunk, ImageChunk):
+            if chunk.content_type == ContentType.IMAGE:
                 image_cnt += 1
                 logger.info(f"image:{chunk.image_name}")
                 logger.info(f"content:{chunk.content}")
-            if isinstance(chunk, TextChunk):
+                logger.info(f"url:{chunk.url}")
+            if chunk.content_type == ContentType.TEXT:
                 logger.info(f"text:{chunk.content}")
     
-            if isinstance(chunk, TableChunk):
-                logger.info(f"table:\n{chunk.data}")
+            if chunk.content_type == ContentType.TABLE:
+                # logger.info(f"table:\n{chunk.data}")
                 logger.info(f"content:\n{chunk.content}")
             logger.info("*"*40+"\n")
         return image_cnt
 
     def test_load_pdf(self):
         file_path = os.path.join(DATA_DIR, "kb_file", "image_table.pdf")
-        chunks = load_file(file_path, end_page=5)
+        chunks = load_file(file_path, end_page=5, ocr=True)
         # image_cnt = 0
         image_cnt = self.show_chunks(chunks)
 
         self.assertEqual(image_cnt, 4)
 
 
     def test_load_docx(self):
         file_path = os.path.join(DATA_DIR, "kb_file", "Xagents中间件.docx")
+        chunks = load_file(file_path, ocr=True)
+        image_cnt = self.show_chunks(chunks)
+
+        self.assertEqual(image_cnt, 1)
+
+
+    # def test_load_doc(self):
+    #     file_path = os.path.join(DATA_DIR, "kb_file", "初步设计文件.doc")
+    #     chunks = load_file(file_path)
+    #     image_cnt = self.show_chunks(chunks)
+
+    #     self.assertEqual(image_cnt, 6)
+    
+    def test_load_pptx(self):
+        file_path = os.path.join(DATA_DIR, "kb_file", "时序数据预测.pptx")
+        chunks = load_file(file_path)
+        image_cnt = self.show_chunks(chunks)
+
+        self.assertEqual(image_cnt, 18)
+    
+    def test_load_json(self):
+        file_path = os.path.join(DATA_DIR, "kb_file", "alpaca_data-0-3252-中文.json")
+        chunks = list(load_file(file_path))
+        self.show_chunks(chunks)
+        self.assertEqual(len(chunks), 7)
+        
+    def test_load_jsonl(self):
+        file_path = os.path.join(DATA_DIR, "kb_file", "LICENSE.jsonl")
+        chunks = list(load_file(file_path))
+        self.show_chunks(chunks)
+        self.assertEqual(len(chunks), 17)
+
+
+    def test_load_excel(self):
+        file_path = os.path.join(DATA_DIR, "kb_file", "大学综合排名2022.xlsx")
+        chunks = list(load_file(file_path))
+        
+        self.show_chunks(chunks)
+
+        self.assertEqual(len(chunks), 3)
+        
+    def test_load_txt(self):
+        file_path = os.path.join(DATA_DIR, "kb_file", "requirements.txt")
         chunks = load_file(file_path)
         image_cnt = self.show_chunks(chunks)
+        self.assertEqual(image_cnt, 0)
+        chunks = parse_file(file_path = file_path)
+        logger.info(chunks)
+        self.show_chunks(chunks)
+                
 
-        self.assertEqual(image_cnt, 1)
+
```

### Comparing `xagent-0.0.7/tests/test_local_model.py` & `xagent-0.0.8/tests/test_local_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     @classmethod
     def setUpClass(cls):
         set_logger("dev", __name__)
         logger.info("start llm")
         cls.tgi_llm_model:LLM = get_llm_model(dict(cls="TGI_GLM", url="http://hz-model.bigmodel.cn/wind-130b"))
 
-    def test_zhipu_api(self):
+    def test_tgi_llm(self):
         # set_logger("dev", "")
         prompt = "你好呀，你是谁"
         _system = "请用英语回答我的问题，你的名字叫XAgent"
         
         # 测试zhipu api
         resp:LLMResp = self.tgi_llm_model.generate(prompt=prompt, system=_system, temperature=0.7, top_p=0.95, max_tokens=100, log_level="INFO", stream=False)
```

### Comparing `xagent-0.0.7/tests/test_xagent.py` & `xagent-0.0.8/tests/test_xagent.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 @Time    :   2024/04/11 17:17:19
 @Author  :   ChenHao
 @Description  :   测试xagent
 @Contact :   jerrychen1990@gmail.com
 '''
 
 from unittest import TestCase
-import sys
 # sys.path.append("../")
 from xagents.agent.api import *
 from xagents.kb.api import *
 from loguru import logger
 from snippets import set_logger
 
 
@@ -140,15 +139,57 @@
 
         self.assertIsNotNone(agent_resp.content)
         content = "".join(agent_resp.content)
         logger.info(f"agent resp:{content}")
 
         self.assertIsNotNone(agent_resp.references)
         for reference in agent_resp.references:
+            logger.info(f"reference_len:{reference.total_len}")
             logger.info(f"reference: {reference.to_plain_text()}")
 
         self.assertIsNotNone(agent_resp.usage)
 
         logger.info(f"agent resp: {agent_resp.model_dump(exclude={'content'})}")
 
+    def test_inverted_index(self):
+        # create kb
+        kb_name='test_inverted'
+        try:
+            kb = get_knowledge_base(kb_name)
+        except Exception as e:
+            kb = create_knowledge_base(kb_name)
+        file_name = "README.md"
 
+        # create kb_file
+        try:
+            kb_file = get_kb_file_info(kb_name=kb_name, file_name=file_name)
+        except Exception as e:
+            cur_dir = os.path.abspath(os.path.dirname(__file__))
+            file_path = os.path.join(os.path.dirname(cur_dir), file_name)
+            logger.debug(f"adding file:{file_path}")
+            kb_file = create_kb_file(kb_name=kb_name, file=file_path)
 
+        # delete kb_file
+        # cur_dir = os.path.abspath(os.path.dirname(__file__))
+        # file_path = os.path.join(os.path.dirname(cur_dir), file_name)
+        # delete_kb_file(kb_name=kb_name, file_name=file_name)
+
+        # reindex_kb_file
+        # reindex_kb_file(kb_name=kb_name, file_name=file_name, reindex=True)
+
+        agent_name = "unittest_agent"
+        kb_config = KBConfig(name=kb_name)
+        llm_config = dict(cls="GLM", version="glm-3-turbo")
+
+        # create agent
+        agent: XAgent = create_agent(name=agent_name, llm_config=llm_config, kb_config=kb_config)
+        logger.info(f"create Agent {agent.get_info()} success")
+
+        # chat with agent
+        message = "具体接口文档参考哪里？"
+        llm_gen_config = LLMGenConfig()
+        kb_search_config = KBSearchConfig(do_expand=True, expand_len=200)
+        agent_resp = chat_agent(name=agent.name, message=message, use_kb=True, stream=False, kb_search_config=kb_search_config, llm_gen_config=llm_gen_config)
+        self.assertIsNotNone(agent_resp.content)
+        content = "".join(agent_resp.content)
+        logger.info(f"agent resp:{content}")
+
```

### Comparing `xagent-0.0.7/tests/test_zhipu_api_model.py` & `xagent-0.0.8/tests/test_zhipu_api_model.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.7/xagents/__init__.py` & `xagent-0.0.8/xagents/__init__.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.7/xagents/agent/api.py` & `xagent-0.0.8/xagents/agent/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 '''
 from enum import Enum
 from typing import List
 from xagents.tool.api import get_tools
 from xagents.model.common import LLMGenConfig
 from xagents.kb.api import KBSearchConfig
 from xagents.config import AGENT_DIR, XAGENT_CACHE_NUM
-from xagents.agent.common import AgentResp, KBConfig, WebSearchConfig
+from xagents.agent.common import AgentResp, KBConfig
 from xagents.agent.xagent import XAgent
 from cachetools import LRUCache, cached
 from loguru import logger
 
 agent_cache = LRUCache(maxsize=XAGENT_CACHE_NUM)
 
 
@@ -84,7 +84,14 @@
 
     Args:
         name (str): agent的名称
     """
     logger.info(f"clear memory of {name}")
     agent = get_agent(name=name)
     agent.clear_memory()
+
+
+def delete_agent(name:str) ->None:
+    logger.info(f"clear memory of {name}")
+    agent = get_agent(name=name)
+    agent.delete(AGENT_DIR)
+
```

### Comparing `xagent-0.0.7/xagents/agent/common.py` & `xagent-0.0.8/xagents/agent/common.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.7/xagents/agent/memory.py` & `xagent-0.0.8/xagents/agent/memory.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.7/xagents/agent/xagent.py` & `xagent-0.0.8/xagents/agent/xagent.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 
 import os
 import copy
+import shutil
 from typing import Generator, List, Optional
 
 from pydantic import BaseModel, Field
 
 from agit.common import LLMResp
 from xagents.model.common import LLMGenConfig
 from xagents.agent.common import AbstractAgent, AgentResp, KBConfig, WebSearchResp
@@ -32,28 +33,28 @@
 
 class XAgentInfo(BaseModel):
     name: str = Field(description="agent的名称，唯一键")
     llm_config: dict = Field(description="llm的配置信息")
     memory_config: dict = Field(description="memory的配置信息")
     kb_config: Optional[KBConfig] = Field(description="kb的配置信息")
     # web_search_config: Optional[WebSearchConfig] = Field(description="web_search的配置信息")
-    tools_descs: List[ToolDesc] = Field(description="工具列表")
+    tools: List[ToolDesc] = Field(description="工具列表")
 
 
 class XAgent(AbstractAgent):
 
     def __init__(self, name: str,
                  llm_config: dict,
                  memory_config: dict,
                  kb_config:KBConfig,
                  # web_search_config: WebSearchConfig,
                  tools: List[BaseTool] = []) -> None:
         super().__init__(name=name)
         self.info = XAgentInfo(name=name,llm_config=llm_config, memory_config=memory_config,kb_config=kb_config,
-                               tools_descs=[ToolDesc(**e.model_dump(exclude={})) for e in tools])
+                               tools=[ToolDesc(**e.model_dump(exclude={})) for e in tools])
         self.llm_model = get_llm_model(llm_config)
         self.memory = BaseMemory(**memory_config)
         self._load_kb(kb_config)
         # print(f"web_search_config_0:{web_search_config}")
         # self._load_web_search(web_search_config)
         self.tools = tools
 
@@ -83,14 +84,21 @@
         return os.path.join(dir_path, agent_name+".json")
 
     def save(self, save_dir: str):
         save_path = self._get_agent_config_path(save_dir, self.name)
         logger.info(f"save agent:{self.name} to {save_path}")
         logger.debug(f"agent info:{self.get_info()}")
         dump(self.get_info().model_dump(), save_path)
+        
+    def delete(self, save_dir: str):
+        save_path = self._get_agent_config_path(save_dir, self.name)
+        if os.path.exists(save_path):
+            logger.info(f"deleting agent:{self.name} from save_path:{save_path}")
+            shutil.rmtree(save_path)
+
 
     @classmethod
     def load(cls, save_dir: str, name: str) -> "XAgent":
         config_path = cls._get_agent_config_path(save_dir, name)
         if not os.path.exists(config_path):
             raise FileExistsError(f"config file {config_path} not found")
 
@@ -100,15 +108,15 @@
         logger.debug(f"{kwargs=}")
 
         return XAgent(**kwargs)     
 
 
     def chat(self, message: str, do_remember=True, details=False, stream = False,
              use_kb=False, kb_search_config:KBSearchConfig=KBSearchConfig(),
-             fake_chat=False, llm_gen_config:LLMGenConfig=LLMGenConfig(), **kwargs) -> AgentResp:
+             fake_chat=False, llm_gen_config:LLMGenConfig=LLMGenConfig(), key_word=True, **kwargs) -> AgentResp:
 
         chunks = []
         if use_kb:
             if not self.kb or not self.kb_prompt_template:
                 logger.warning(f"agent:{self.name} has no related knowledge base, will not chat with kb! ")
                 prompt = message
                 chunks = None
@@ -126,15 +134,15 @@
         if fake_chat:
             fake_resp = "这是MOCK的回答信息,如果需要真实回答,请设置fake_chat=False"
             llm_resp = (e for e in fake_resp) if stream else fake_resp
             tool_call = None
         else:
             history = self.memory.to_llm_history()
             llm_resp: LLMResp = self.llm_model.generate(prompt=prompt, history=history, tools=self.tools, details=details, stream=stream,
-                                                        **llm_gen_config.model_dump(), **kwargs)
+                                                        **llm_gen_config.model_dump(), key_word=key_word, **kwargs)
 
             logger.debug(f"llm_resp_inner:{llm_resp}")
             # 调用tool
             tool_calls = copy.deepcopy(llm_resp.tool_calls)
             if tool_calls:
                 for tool_call in tool_calls:
                     logger.debug(f"calling tool:{tool_call.name}")
```

### Comparing `xagent-0.0.7/xagents/config.py` & `xagent-0.0.8/xagents/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,8 +57,15 @@
 ### 最大job数（job用来处理知识库index任务）
 MAX_JOB_NUM=10
 ### 用户鉴权配置
 USERNAME="zhipu"
 PASSWORD="zhipu"
 ### xagent缓存数目
 XAGENT_CACHE_NUM=1000
-XAGENT_CACHE_EXPIRE_SECONDS=3600
+XAGENT_CACHE_EXPIRE_SECONDS=3600
+
+
+
+### MinIO对象存储相关
+MINIO_URL = '10.50.130.151:9000'
+MINIO_ACCESS_KEY='l7RJ3QCGX6gt7M8zfN1v'
+MINIO_SECRET_KEY='smGpFhcz0hLOup8V2s6SMkzgzxzJFtSJiuAuKFqS'
```

### Comparing `xagent-0.0.7/xagents/kb/api.py` & `xagent-0.0.8/xagents/kb/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 @Contact :   jerrychen1990@gmail.com
 '''
 
 from typing import List
 from fastapi import UploadFile
 from loguru import logger
 from pydantic import BaseModel, Field
+from xagents.loader.common import Chunk
 from xagents.kb.kb_file import KnowledgeBaseFile
 from xagents.kb.kb import KnowledgeBase
 from xagents.config import *
-from xagents.kb.common import KnowledgeBaseInfo, KnowledgeBaseFileInfo, RecalledChunk, get_config_path, get_kb_dir, DistanceStrategy
-
+from xagents.kb.common import KnowledgeBaseInfo, KnowledgeBaseFileInfo, RecalledChunk, get_config_path, DistanceStrategy
 
 def list_knowledge_base_names() -> List[str]:
     """列出所有知识库名称
 
     Returns:
         str: 知识库名称列表
     """
@@ -62,16 +62,16 @@
     kb = get_knowledge_base(name=name)
     return kb.get_info()
 
 
 def create_knowledge_base(name: str,
                           desc: str = None,
                           embedding_config: dict = dict(cls="ZhipuEmbedding"),
-                          vecstore_config: dict = dict(cls='XFAISS', distance_strategy=DistanceStrategy.MAX_INNER_PRODUCT)
-                          ) -> KnowledgeBaseInfo:
+                          vecstore_config: dict|List[dict] = dict(cls='XFAISS', distance_strategy=DistanceStrategy.MAX_INNER_PRODUCT)
+                          )->KnowledgeBase:
     """创建知识库
 
     Raises:
         ValueError: 知识库已经存在的异常
 
     Returns:
         _type_: _description_
@@ -81,33 +81,37 @@
     kb_names = list_knowledge_base_names()
     if name in kb_names:
         msg = f"Knowledge base {name} already exists, can not create!"
         logger.warning(msg)
         raise ValueError(msg)
     if not desc:
         desc = f"知识库{name}"
+
     kb = KnowledgeBase(name=name, embedding_config=embedding_config,
                        desc=desc, vecstore_config=vecstore_config)
-    return kb.get_info()
+    return kb
 
 
 def delete_knowledge_base(name: str) -> str:
     """删除知识库
 
     Args:
         name (str): 知识库名称
 
     Returns:
         str: 删除消息
     """
     # delete knowledge base
-    kb_dir = get_kb_dir(kb_name=name)
-    if os.path.exists(kb_dir):
-        import shutil
-        shutil.rmtree(path=kb_dir)
+    kb = get_knowledge_base(name=name)
+    kb.delete()    
+
+    # kb_dir = get_kb_dir(kb_name=name)
+    # if os.path.exists(kb_dir):
+    #     import shutil
+    #     shutil.rmtree(path=kb_dir)
     msg = f'【{name}】deleted.'
     return msg
 
 
 def reindex_knowledge_base(name: str, reindex=True, batch_size=16) -> str:
     """重新构建知识库索引
 
@@ -139,14 +143,19 @@
                           do_expand=False, expand_len: int = 500, forward_rate: float = 0.5) -> List[RecalledChunk]:
     kb = get_knowledge_base(name=name)
     
     chunks = kb.search(query=query, top_k=top_k, score_threshold=score_threshold, do_split_query=do_split_query,
                        file_names=file_names, rerank_config=rerank_config, do_expand=do_expand, expand_len=expand_len, forward_rate=forward_rate)
     return chunks
 
+def list_kb_files(kb_name: str) -> List[KnowledgeBaseFile]:
+    kb = get_knowledge_base(kb_name)
+    kb_files = kb.list_kb_files()
+    return kb_files
+
 
 def list_kb_file_infos(kb_name: str) -> List[KnowledgeBaseFileInfo]:
     kb = get_knowledge_base(kb_name)
     kb_files = kb.list_kb_files()
     kb_file_infos = [kb_file.get_info() for kb_file in kb_files]
     return kb_file_infos
 
@@ -163,15 +172,15 @@
     return kb_file.get_info()
 
 
 def create_kb_file(kb_name: str, file: UploadFile | str, do_cut=True, do_index=True,
                    batch_size:int=16,
                    cut_config: dict = dict(separator='\n',
                                            max_len=200,
-                                           min_len=10)) -> KnowledgeBaseFileInfo:
+                                           min_len=10)) -> KnowledgeBaseFile:
     """创建知识库文件
     Args:
         kb_name (str): 知识库名称
         file (UploadFile | str): 知识库文件，UploadFile(fast_api)或者str(文件路径)
         do_cut (bool, optional): 是否切分文件. Defaults to True.
         do_index (bool, optional): 是否添加到索引. Defaults to True.
         cut_config (dict, optional): 切分文件的参数. Defaults to dict(separator='\n', max_len=200, min_len=10).
@@ -198,19 +207,16 @@
         content = file.file.read()
     with open(kb_file_path, "wb") as f:
         f.write(content)
     if do_cut:
         kb_file.cut(**cut_config)
     if do_index:
         kb = get_knowledge_base(name=kb_name)
-        index = kb.get_index()
-        # logger.debug(f"{index=}")
-        kb.add_kb_file2index(index, kb_file, reindex=True, do_save=True,batch_size=batch_size)
-    kb_file_info = kb_file.get_info()
-    return kb_file_info
+        kb.add_kb_file2index(kb_file=kb_file, reindex=True, do_save=True, batch_size=batch_size)
+    return kb_file
 
 
 def delete_kb_file(kb_name: str, file_name: str) -> str:
     """删除知识库文件
 
     Args:
         kb_name (str): 知识库名称
@@ -218,15 +224,15 @@
 
     Returns:
         str: 删除消息
     """
 
     kb = get_knowledge_base(kb_name)
     kb_file = get_kb_file(kb_name=kb_name, file_name=file_name)
-    kb.remove_file(kb_file=kb_file)
+    kb.remove_kb_file(kb_file=kb_file)
     return f"知识库文件【{file_name}】删除成功"
 
 
 def cut_kb_file(kb_name: str, file_name: str,
                 separator: str = '\n',
                 max_len: int = 200,
                 min_len: int = 10) -> int:
@@ -258,18 +264,69 @@
 
     Returns:
         str: 构建成功的消息
     """
 
     kb = get_knowledge_base(kb_name)
     kb_file = get_kb_file(kb_name=kb_name, file_name=file_name)
-    kb.add_kb_file2index(index=kb.get_index(), kb_file=kb_file, reindex=reindex, do_save=True, batch_size=batch_size)
+    indexes = kb.get_indexes()
+    kb.add_kb_file2index(indexes=indexes, kb_file=kb_file, reindex=reindex, do_save=True, batch_size=batch_size)
     return f"更新知识库文件【{file_name}】到索引成功"
 
 
+def list_chunks(kb_name: str, file_name: str) -> List[Chunk]:
+    """给定知识库文件，返回所有的chunk
+
+    Args:
+        kb_name (str): 知识库名称
+        file_name (str): 知识库文件名称
+
+    Returns:
+        List[Chunk]: chunk列表
+    """
+    kb_file:KnowledgeBaseFile= get_kb_file(kb_name=kb_name, file_name=file_name)
+    chunks =  kb_file.list_chunks()
+    return chunks   
+
+def add_chunks(kb_name: str, file_name: str, chunks: List[Chunk], idx:int=None) -> str:
+    """给定知识库文件，添加chunk
+
+    Args:
+        kb_name (str): 知识库名称
+        file_name (str): 知识库文件名称
+        chunk (Chunk): 待添加的chunk
+        idx (_type_, optional): chunk添加的位置，None的话添加在最后. Defaults to None.
+
+    Returns:
+        str: 添加成功的消息
+    """
+    kb_file:KnowledgeBaseFile= get_kb_file(kb_name=kb_name, file_name=file_name)
+    kb_file.add_chunks(chunks=chunks, idx=idx)
+    kb:KnowledgeBase = get_knowledge_base(name=kb_name)
+    kb.add_chunks2index(chunks=chunks, meta_info=dict(file_name=file_name), do_save=True)
+    message =f"添加{len(chunks)}chunk到知识库文件【{file_name}】成功" 
+    return message
+
+def delete_chunks(kb_name: str, file_name: str, chunk_ids: List[str]) -> str:
+
+    kb_file:KnowledgeBaseFile= get_kb_file(kb_name=kb_name, file_name=file_name)
+    kb_file.delete_chunks(ids=chunk_ids)
+    kb:KnowledgeBase = get_knowledge_base(name=kb_name)
+    kb.remove_chunks_from_index(chunk_ids=chunk_ids)
+    message =f"从【{file_name}】删除{len(chunk_ids)}chunk成功" 
+    return message
+
+def update_chunk(kb_name: str, file_name: str, chunk: Chunk) -> str:
+    kb_file:KnowledgeBaseFile= get_kb_file(kb_name=kb_name, file_name=file_name)
+    kb_file.update_chunk(chunk=chunk)
+    kb:KnowledgeBase = get_knowledge_base(name=kb_name)
+    logger.debug(f"{chunk=}")
+    kb.add_chunks2index(chunks=[chunk], meta_info=dict(file_name=file_name), do_save=True)
+    
+
 if __name__ == "__main__":
     # print(list_knowledge_base_names())
     # print(list_vecstores())
     # print(list_distance_strategy())
     # chunk_len = cut_kb_file(kb_name="new_kb", file_name="requirements.txt")
     # print(chunk_len)
```

### Comparing `xagent-0.0.7/xagents/kb/common.py` & `xagent-0.0.8/xagents/kb/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,93 +24,122 @@
 
 def get_chunk_dir(kb_name)->str:
     return os.path.join(get_kb_dir(kb_name), "chunk")
 def get_origin_dir(kb_name)->str:
     return os.path.join(get_kb_dir(kb_name), "origin")
 def get_id_dir(kb_name)->str:
     return os.path.join(get_kb_dir(kb_name), "id")
-def get_index_dir(kb_name)->str:
-    return os.path.join(get_kb_dir(kb_name), "index")
+def get_inverted_id_dir(kb_name)->str:
+    return os.path.join(get_kb_dir(kb_name), "inverted_id")
 
+def get_index_dir(kb_name, index_name="index")->str:
+    return os.path.join(get_kb_dir(kb_name), index_name)
+
+def get_inverted_index_dir(kb_name)->str:
+    return os.path.join(get_kb_dir(kb_name), "inverted_index")
 def get_config_path(kb_name)->str:
     return os.path.join(get_kb_dir(kb_name), "config.json")
 
 def get_chunk_path(kb_name, file_name) -> str:
     return os.path.join(get_chunk_dir(kb_name), file_name+".jsonl")
 
 def get_origin_path(kb_name, file_name) -> str:
     return os.path.join(get_origin_dir(kb_name), file_name)
 
 def get_id_path(kb_name, file_name) -> str:
     return os.path.join(get_id_dir(kb_name), file_name+".jsonl")
-
+def get_inverted_id_path(kb_name, file_name) -> str:
+    return os.path.join(get_inverted_id_dir(kb_name), file_name+".jsonl")
 
 class DistanceStrategy(str, enum.Enum):
     """Enumerator of the Distance strategies for calculating distances
     between vectors."""
 
     EUCLIDEAN_DISTANCE = "EUCLIDEAN_DISTANCE"
     MAX_INNER_PRODUCT = "MAX_INNER_PRODUCT"
 
 
-# 知识库中的切片
-class KBChunk(Chunk):
-    kb_name: str = Field(description="知识库名称")
-    file_name: str = Field(description="文件名称")
-    idx: int = Field(description="chunk在文档中的顺序,从0开始")
-
-    def to_dict(self):
-        return self.model_dump(mode="json", exclude_none=True, exclude={"kb_name", "file_name", "idx"})
 
-    def to_document(self) -> Document:
-        if self.search_content:
-            page_content, metadata = self.search_content, dict(content=self.content)
-        else:
-            page_content, metadata = self.content, dict()
-
-        metadata.update(chunk_type=self.content_type.value, idx=self.idx, page_idx=self.page_idx,
-                        kb_name=self.kb_name, file_name=self.file_name)
-        return Document(page_content=page_content, metadata=metadata)
+def chunk2document(chunk: Chunk, metadata: dict = dict()) -> Document:
+    _metadata = copy.copy(metadata)
+    if chunk.search_content:
+        page_content= chunk.search_content,
+        _metadata.update(content=chunk.content)
+    else:
+        page_content = chunk.content
+    _metadata.update(page_idx=chunk.page_idx, id=chunk.id)
+    return Document(page_content=page_content, metadata=_metadata)
+
+# # 知识库中的切片
+# class KBChunk(Chunk):
+#     kb_name: str = Field(description="知识库名称")
+#     file_name: str = Field(description="文件名称")
+#     idx: int = Field(description="chunk在文档中的顺序,从0开始")
+
+#     def to_dict(self):
+#         return self.model_dump(mode="json", exclude_none=True, exclude={"kb_name", "file_name", "idx"})
+
+#     def to_document(self) -> Document:
+#         if self.search_content:
+#             page_content, metadata = self.search_content, dict(content=self.content)
+#         else:
+#             page_content, metadata = self.content, dict()
+
+#         metadata.update(chunk_type=self.content_type.value, idx=self.idx, page_idx=self.page_idx,
+#                         kb_name=self.kb_name, file_name=self.file_name)
+#         return Document(page_content=page_content, metadata=metadata)
+
+    # @classmethod
+    # def from_document(cls, document: Document):
+    #     content = document.metadata.pop("content", None)
+    #     item = dict(content=content, search_content=document.page_content) if content else dict(content=document.page_content)
+    #     item.update(document.metadata)
+    #     return cls(**item)
 
-    @classmethod
-    def from_document(cls, document: Document):
-        content = document.metadata.pop("content", None)
-        item = dict(content=content, search_content=document.page_content) if content else dict(content=document.page_content)
-        item.update(document.metadata)
-        return cls(**item)
+    # def __hash__(self) -> int:
+    #     return hash((self.kb_name, self.file_name, self.idx))
 
-    def __hash__(self) -> int:
-        return hash((self.kb_name, self.file_name, self.idx))
-
-    def __eq__(self, __value: object) -> bool:
-        return hash(self) == hash(__value)
+    # def __eq__(self, __value: object) -> bool:
+    #     return hash(self) == hash(__value)
 
 
 # 召回的切片
-class RecalledChunk(KBChunk):
+class RecalledChunk(Chunk):
     query: str = Field(description="召回chunk的query")
     score: float = Field(description="召回chunk的分数")
+    file_name:str = Field(description="知识库文件名称")
     forwards: List[Chunk] = Field(description="chunk的下文扩展", default=[])
     backwards: List[Chunk] = Field(description="chunk的上文扩展", default=[])
+    index_cls: str = Field(description="索引类型", default=None)
 
     @classmethod
-    def from_document(cls, document: Document, query: str, score: float) -> "RecalledChunk":
+    def from_document(cls, document: Document, query: str, score: float, index_cls:str) -> "RecalledChunk":
         """从langchain的Document构造过来
 
         Args:
             document (Document): langchain的Document
             query (str): 相关问题
             score (float): 召回得分
 
         Returns:
             _type_: RecalledChunk
         """
-        chunk = cls.__bases__[0].from_document(document)
-        recalled_chunk = cls(**chunk.__dict__, query=query, score=score)
-        return recalled_chunk
+    
+        content = document.metadata.pop("content", None)
+        item = dict(content=content, search_content=document.page_content) if content else dict(content=document.page_content)
+        # logger.debug(f"meta:{document.metadata}")
+        item.update(document.metadata)
+        return cls(**item, query=query, score=score, index_cls=index_cls)
+    
+    def __hash__(self) -> int:
+        return hash((self.file_name, self.id))
+
+    def __eq__(self, __value: object) -> bool:
+        return hash(self) == hash(__value)
+
 
     def get_content(self):
         if self.search_content:
             return self.search_content + "\n" + self.content
 
         return self.content
 
@@ -153,26 +182,28 @@
         if forwards_len:
             forwards_str = "\n".join([f"{chunk.content}" for idx, chunk in enumerate(self.forwards)])
             if max_len:
                 forwards_str = forwards_str[:max_len]+"..."
             forwards_str = f"下文[{forwards_len}]字\n\n{forwards_str}"
 
         return backwards_str, forwards_str
+    @property
+    def total_len(self):
+        return sum(len(c.content) for c in self.backwards+[self]+self.forwards)
+
 
 
 class KnowledgeBaseInfo(BaseModel):
     name: str = Field(description="知识库名称")
     desc: str = Field(description="知识库描述")
     embedding_config: dict = Field(description="embedding模型配置")
-    vecstore_config: dict = Field(description="向量存储配置")
+    vecstore_config: dict|list[dict] = Field(description="向量存储配置")
     file_num:int = Field(description="知识库文件数量")
 
 
 
 # 知识库文件类
 class KnowledgeBaseFileInfo(BaseModel):
     kb_name: str = Field(description="知识库名称")
     file_name: str = Field(description="知识库文件名称")
     is_cut:bool = Field(description="是否已经切片")
-    is_indexed:bool = Field(description="是否已经索引")
-
```

### Comparing `xagent-0.0.7/xagents/kb/kb.py` & `xagent-0.0.8/xagents/kb/kb.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,36 +8,38 @@
 '''
 import copy
 import os
 import re
 from typing import List, Type
 from loguru import logger
 from xagents.kb.kb_file import KnowledgeBaseFile
-from xagents.kb.vector_store import LocalVecStore, XVecStore, get_vecstore_cls
-from xagents.loader.common import Chunk
+from xagents.kb.vector_store import XES, LocalVecStore, XVecStore, get_vecstore_cls
+from xagents.loader.common import Chunk, ContentType
 from xagents.model.api import get_embd_model, get_rerank_model
-from xagents.kb.common import KnowledgeBaseInfo, RecalledChunk, get_chunk_dir, get_chunk_path, get_config_path, get_id_dir, get_index_dir, get_kb_dir, get_origin_dir, DistanceStrategy
-from snippets import load, log_cost_time, dump
+from xagents.kb.common import KnowledgeBaseInfo, RecalledChunk, chunk2document, get_chunk_dir, get_chunk_path, get_config_path, get_index_dir, get_kb_dir, get_origin_dir
+from snippets import load, log_cost_time, dump, jload
 
 
 class KnowledgeBase():
 
-    def __init__(self, name: str, desc, embedding_config: dict, vecstore_config: dict):
+    def __init__(self, name: str, desc, embedding_config: dict, vecstore_config: dict|List[dict]):
         self.name = name
         self.desc = desc
         self.embedding_config = embedding_config
-        self.vecstore_config = vecstore_config
+        self.vecstore_config = vecstore_config if isinstance(vecstore_config, list) else [vecstore_config]
+        self.indexes = []
         self._build_dirs()
         self._save_config()
-        self.index=None
 
     @classmethod
     def from_config(cls, config: dict | str):
         if isinstance(config, str):
-            config = load(config)
+            # logger.info(f"{config=}")
+            config = jload(config)
+        logger.debug(f"{config=}")
         return cls(**config)
 
     def _get_config(self) -> dict:
         return dict(name=self.name, desc=self.desc, embedding_config=self.embedding_config, vecstore_config=self.vecstore_config)
 
     def get_info(self) -> KnowledgeBaseInfo:
         """返回知识库的信息
@@ -49,105 +51,127 @@
         return KnowledgeBaseInfo(**self._get_config(), file_num=file_num)
 
     def _build_dirs(self):
         self.kb_dir = get_kb_dir(self.name)
         self.origin_dir = get_origin_dir(self.name)
 
         self.chunk_dir = get_chunk_dir(self.name)
-        self.index_dir = get_index_dir(self.name)
-        self.id_dir = get_id_dir(self.name)
         self.config_path = get_config_path(self.name)
 
         os.makedirs(self.origin_dir, exist_ok=True)
         os.makedirs(self.chunk_dir, exist_ok=True)
-        os.makedirs(self.id_dir, exist_ok=True)
 
     def _save_config(self):
         dump(self._get_config(), self.config_path)
 
-    def get_index(self) -> XVecStore:
+    def get_indexes(self) -> List[XVecStore]:
         """
-        加载向量库
+        初始化向量存储、ES存储
         """
-        if not self.index:
-            config = copy.copy(self.vecstore_config)
-            vecstore_cls: Type[XVecStore] = get_vecstore_cls(config.pop("cls"))
-            embedding_model = get_embd_model(self.embedding_config)
-            config.update(embedding=embedding_model, local_dir=self.index_dir)
-            self.index = vecstore_cls.from_config(config)
-        return self.index
-
+        if not self.indexes:
+            for index_config in self.vecstore_config:
+                config = copy.copy(index_config)
+                vecstore_cls: Type[XVecStore] = get_vecstore_cls(config.pop("cls"))
+                if vecstore_cls.is_local():
+                    local_dir = get_index_dir(kb_name=self.name, index_name=f"{vecstore_cls.__name__}_index")
+                    config.update(local_dir=local_dir)
+
+                if vecstore_cls.need_embd():
+                    embedding_model = get_embd_model(self.embedding_config)
+                    config.update(embedding=embedding_model)
+                if vecstore_cls == XES:
+                    if "es_index" not in config:
+                        config.update(es_index=f"{self.name}")
+
+                    
+                logger.debug(f"creating index:{vecstore_cls} with config:{config}")
+                index = vecstore_cls.from_config(config)
+                self.indexes.append(index)
+        return self.indexes
+            
     def list_kb_files(self) -> List[KnowledgeBaseFile]:
         kb_files = []
         for file_name in os.listdir(self.origin_dir):
             kb_file = KnowledgeBaseFile(kb_name=self.name, file_name=file_name)
             kb_files.append(kb_file)
         return kb_files
 
-    def remove_file(self, kb_file: KnowledgeBaseFile):
+    def remove_kb_file(self, kb_file: KnowledgeBaseFile):
         """
         删除文档
         """
         assert kb_file.kb_name == self.name
-        kb_file.remove()
-        if kb_file.is_indexed:
-            index = self.get_index()
-            logger.debug(f"{index=}")
-            self.remove_kb_file_from_index(index, kb_file)
-
-    def remove_kb_file_from_index(self, index: XVecStore, kb_file: KnowledgeBaseFile):
-        if kb_file.is_indexed:
-            doc_ids = load(kb_file.id_path)
-            index.delete(doc_ids)
-            os.remove(kb_file.id_path)
+        ## 从索引中删除
+        self.remove_kb_file_from_index(kb_file=kb_file)
+        # 删除kb文件
+        kb_file.delete()
+
+    def remove_kb_file_from_index(self, kb_file: KnowledgeBaseFile):
+        ids = kb_file.get_chunk_ids()
+        self.remove_chunks_from_index(ids)      
+            
+    def remove_chunks_from_index(self, chunk_ids):
+        for index in self.get_indexes():
+            logger.info(f"deleting {len(chunk_ids)} chunks from index:{index}")
+            index.delete(chunk_ids) 
+            if index.is_local():
+                index.save()
+
+    def add_chunks2index(self, chunks:List[Chunk], meta_info:dict, reindex=False, do_save=False, batch_size=16):
+        indexes = self.get_indexes()
+        documents = [chunk2document(chunk, meta_info) for chunk in chunks if chunk.content]
+
+        ids = [chunk.id for chunk in chunks if chunk.content]
+        # 添加新的index        
+        for index in indexes:
+            embd_model = index.embeddings
+            if embd_model:
+                if hasattr(embd_model, "batch_size"):
+                    logger.debug(f"setting embedding model batch size to {batch_size}")
+                    setattr(embd_model, "batch_size", batch_size)
+                else:
+                    logger.warning(f"{embd_model.__class__} has no attribute batch_size, set to default value {batch_size}") 
+            logger.debug(f"updating {len(ids)} documents to index:{index}")
+            index.delete(ids=ids)
+            index.add_documents(documents=documents, ids=ids)
+
+            if index.is_local() and do_save:
+                
+            # TODO 为何isinstance判断不work？
+            # if isinstance(index, LocalVecStore) and do_save:
+                logger.info(f"saving to index dir:{index.local_dir}")
+                index.save()
+        
 
-    def add_kb_file2index(self, index: XVecStore, kb_file: KnowledgeBaseFile, reindex=False, do_save=False, batch_size=16):
+    def add_kb_file2index(self,  kb_file: KnowledgeBaseFile, reindex=False, do_save=False, batch_size=16):
         if not kb_file.is_cut:
             logger.warning(f"{kb_file.file_name} is not cut, please cut it first")
             return
-
-        if kb_file.is_indexed and not reindex:
-            logger.info(f"{kb_file.file_name} is already indexed, skip")
-        else:
-
-            embd_model = index.embeddings
-            if hasattr(embd_model, "batch_size"):
-                logger.debug(f"setting embedding model batch size to {batch_size}")
-                setattr(embd_model, "batch_size", batch_size)
-            else:
-                logger.warning(f"{embd_model.__class__} has no attribute batch_size, set to default value {batch_size}")  
-                
-            self.remove_kb_file_from_index(index, kb_file)
-            chunks = kb_file.get_chunks()
-            documents = [chunk.to_document() for chunk in chunks if chunk.content]
-
-            logger.info(f"reindexing {kb_file.file_name} with {len(chunks)}chunks and {len(documents)} documents")
-    
-            # logger.debug(f"sample document:{documents[0]}")
-            ids = index.add_documents(documents)
-            logger.debug(f"{len(ids)} documents add to index")
-            dump(ids, kb_file.id_path)
-        # logger.debug(f"{index=}")
-        if index.is_local() and do_save:
-        # TODO 为何isinstance判断不work？
-        # if isinstance(index, LocalVecStore) and do_save:
-            logger.info(f"saving {kb_file.file_name} to index dir:{index.local_dir}")
-            index.save()
+        chunks = kb_file.list_chunks()
+        return self.add_chunks2index(chunks=chunks, meta_info=dict(file_name=kb_file.file_name), reindex=reindex, do_save=do_save, batch_size=batch_size)
 
     @log_cost_time(name="rebuild_index")
     def rebuild_index(self, reindex:bool, batch_size:int):
         """
         重新构建向量知识库
         """
-        index = self.get_index()
+        indexes = self.get_indexes()
         kb_files = self.list_kb_files()
         for kb_file in kb_files:
-            self.add_kb_file2index(index, kb_file, reindex=reindex, do_save=False, batch_size=batch_size)
-        if isinstance(index, LocalVecStore):
-            index.save()
+            self.add_kb_file2index(kb_file=kb_file, reindex=reindex, do_save=False, batch_size=batch_size)
+        for index in indexes:
+            if isinstance(index, LocalVecStore):
+                index.save()
+                
+    def delete(self):
+        """删除知识库"""
+        for index in self.get_indexes():
+            index.delete_all()
+        import shutil
+        shutil.rmtree(path=self.kb_dir)
 
 
 
     @log_cost_time(name="kb_search")
     def search(self, query: str, top_k: int = 3, score_threshold: float = None,
                do_split_query=False, file_names: List[str] = None, rerank_config: dict = {},
                do_expand=False, expand_len: int = 500, forward_rate: float = 0.5) -> List[RecalledChunk]:
@@ -162,56 +186,51 @@
             do_expand (bool, optional): 返回的chunk是否做上下文扩展. Defaults to False.
             expand_len (int, optional): 上下文扩展后的chunk字符长度（do_expand=True时生效）. Defaults to 500.
             forward_rate (float, optional): 上下文扩展时向下文扩展的比率（do_expand=True时生效）. Defaults to 0.5.
 
         Returns:
             List[RecalledChunk]: 相关的切片，按照score降序
         """
-        index = self.get_index()
         recalled_chunks = []
         # 切分query
         queries = split_query(query, do_split_query)
 
-        # 将原始score归一化到0-1，越大越接近
-        def _get_score(s):
-            if self.vecstore_config["distance_strategy"] in [DistanceStrategy.EUCLIDEAN_DISTANCE]:
-                return 1.-s
-            return s
-
         # 过滤条件
         _filter = dict()
         if file_names:
             _filter = dict(file_name=file_names)
 
         # 每个子query做检索
+        indexes = self.get_indexes()
         for query in queries:
-            score_threshold = _get_score(score_threshold)
-            logger.debug(f"searching {query} with vecstore_cls: {index.__class__.__name__}, {_filter=}, {top_k=}, {score_threshold=}")
-
-            docs_with_score = index.similarity_search_with_score(query, k=top_k, score_threshold=score_threshold, filter=_filter)
-            logger.debug(f"{len(docs_with_score)} origin chunks found for {query}")
-            # logger.debug(f"{query}'s related docs{[d.page_content[:5] for d,s in docs_with_score]}")
-            # logger.debug(docs_with_score[0])
-
-            tmp_recalled_chunks = [RecalledChunk.from_document(d, score=_get_score(s), query=query) for d, s in docs_with_score]
-            recalled_chunks.extend(tmp_recalled_chunks)
+            
+            for index in indexes:
+                score_threshold = index.convert_score(score_threshold)
+                logger.debug(f"searching {query} with vecstore_cls: {index.__class__.__name__}, {_filter=}, {top_k=}, {score_threshold=}")
+                docs_with_score = index.similarity_search_with_score(query, k=top_k, score_threshold=score_threshold, filter=_filter)
+                logger.debug(f"{docs_with_score=}")
+                tmp_recalled_chunks = [RecalledChunk.from_document(d, score= index.convert_score(s), query=query, index_cls=index.__class__.__name__) for d, s in docs_with_score]
+                recalled_chunks.extend(tmp_recalled_chunks)
 
         # 去重，避免召回相同切片
-        recalled_chunks = list(set(recalled_chunks))
-        logger.info(f"{len(recalled_chunks)} chunks recalled")
-
-        #重排序
-        recalled_chunks = rerank(recalled_chunks, rerank_config)[:top_k]
+        origin_recall_num = len(recalled_chunks)
+        recalled_chunks = list(sorted(set(recalled_chunks), key=lambda x:x.score, reverse=True))
+        logger.info(f"{len(recalled_chunks)} distinct recalled from {len(queries)} queries and {len(indexes)} indexes, {origin_recall_num-len(recalled_chunks)} duplicated")
+
+        #精排
+        if rerank_config:
+            recalled_chunks = rerank(recalled_chunks, rerank_config)
+        recalled_chunks = recalled_chunks[:top_k]
         logger.info(f"get {len(recalled_chunks)} reranked chunks after sort")
 
         # 上下文扩展
         if do_expand:
             logger.info("expanding recalled chunks")
             for chunk in recalled_chunks:
-                expand_chunk(chunk, expand_len, forward_rate)
+                expand_chunk(chunk, self.name, expand_len, forward_rate)
 
         return recalled_chunks
 
 
 def rerank(recalled_chunks: List[RecalledChunk], rerank_config: dict) -> List[RecalledChunk]:
     """重排序
     Args:
@@ -241,50 +260,67 @@
     else:
         # 不需要切分也转成list形式，方便后续统一处理
         return [query]
 
 
 # 扩展上下文到给定的长度
 #TODO 扩展时，避免重复的chunk
-#TODO 扩展时，截断chunk以达到固定数目，Agent问答单测可以检验此问题
-def expand_chunk(chunk: RecalledChunk, expand_len: int, forward_rate=0.5) -> RecalledChunk:
+def expand_chunk(chunk: RecalledChunk, kb_name:str, expand_len: int, forward_rate=0.5) -> RecalledChunk:
     logger.debug(f"expanding chunk {chunk}")
-    chunk_path = get_chunk_path(chunk.kb_name, chunk.file_name)
-    chunks = []
-    for item in load(chunk_path):
-        tmp = Chunk(**item)
-        chunks.append(tmp)
-    chunk_idx = chunk.idx
+    chunk_path = get_chunk_path(kb_name, chunk.file_name)
+    chunk_dicts = load(chunk_path)
+    chunk_idx = None
+    
+    for idx, ele in enumerate(chunk_dicts):
+        if ele["id"] == chunk.id:
+            chunk_idx = idx
+            break
+        
+    if chunk_idx is None:
+        logger.warning(f"chunk {chunk} not found in {chunk_path}")
+        return chunk
 
     to_expand = expand_len - len(chunk.content)
     if to_expand <= 0:
         return chunk
 
     forward_len = int(to_expand * forward_rate)
     backward_len = to_expand - forward_len
-    logger.debug(f"expand chunk with :{forward_len=}, {backward_len=}")
+    logger.debug(f"expand chunk with :{forward_len=}, {backward_len=}, origin_len:{len(chunk.content)}")
     backwards, forwards = [], []
 
     # 查找前面的chunk
     idx = chunk_idx-1
     while idx >= 0:
-        tmp_chunk = chunks[idx]
-        backward_len -= len(tmp_chunk.content)
-        if backward_len < 0:
-            break
-        backwards.append(tmp_chunk)
+        if backward_len <= 0:
+            break        
+        tmp_chunk = copy.copy(chunk_dicts[idx])
+        if tmp_chunk["content_type"] ==ContentType.TEXT:
+            chunk_len = min (len(tmp_chunk["content"]), backward_len)
+            tmp_chunk["content"] = tmp_chunk["content"][-chunk_len:]
+            to_add:Chunk = Chunk(**tmp_chunk)
+            backwards.append(to_add)
+            backward_len -= chunk_len
         idx -= 1
+        
     backwards.reverse()
 
     idx = chunk_idx + 1
-    while idx < len(chunks):
-        tmp_chunk = chunks[idx]
-        forward_len -= len(tmp_chunk.content)
-        if forward_len < 0:
-            break
-        forwards.append(tmp_chunk)
+    # logger.debug(f"{idx=}, {len(chunk_dicts)=}, {forward_len=}") 
+    while idx < len(chunk_dicts):
+        if forward_len <= 0:
+            break        
+
+        tmp_chunk = copy.copy(chunk_dicts[idx])
+        if tmp_chunk["content_type"] ==ContentType.TEXT:
+            chunk_len = min (len(tmp_chunk["content"]), forward_len)
+            tmp_chunk["content"] = tmp_chunk["content"][:chunk_len]
+            to_add:Chunk = Chunk(**tmp_chunk)
+            forwards.append(to_add)
+            forward_len -= chunk_len
         idx += 1
 
-    logger.debug(f"expand with {len(backwards)} backward chunks and {len(forwards)} forward chunks")
     chunk.backwards = backwards
     chunk.forwards = forwards
+    logger.debug(f"expand done with {len(backwards)} backward chunks and {len(forwards)} forward chunks, total_len:{chunk.total_len}")
+
     return chunk
```

### Comparing `xagent-0.0.7/xagents/kb/kb_file.py` & `xagent-0.0.8/xagents/kb/kb_file.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,68 +8,98 @@
 '''
 
 
 # 知识库文件类
 import os
 from loguru import logger
 from typing import List
-from xagents.kb.common import KBChunk, KnowledgeBaseFileInfo, get_chunk_path, get_id_path, get_origin_path
+from xagents.kb.common import KnowledgeBaseFileInfo, get_chunk_path, get_origin_path
 from xagents.loader.api import parse_file
 from xagents.loader.common import Chunk
 from snippets import dump, load
 
 
 class KnowledgeBaseFile:
     def __init__(self, kb_name: str, file_name: str):
         self.kb_name = kb_name
         self.file_name = file_name
-
         self.chunk_path = get_chunk_path(self.kb_name, self.file_name)
         self.origin_path = get_origin_path(self.kb_name, self.file_name)
-        self.id_path = get_id_path(self.kb_name, self.file_name)
 
     @property
     def is_cut(self) -> bool:
         return os.path.exists(self.chunk_path)
 
-    @property
-    def is_indexed(self) -> bool:
-        return os.path.exists(self.id_path)
 
     @property
     def chunk_num(self) -> int:
         if not self.is_cut:
             return 0
         chunks = load(self.chunk_path)
         return len(chunks)
 
     def get_info(self):
-        return KnowledgeBaseFileInfo(kb_name=self.kb_name, file_name=self.file_name, is_cut=self.is_cut, is_indexed=self.is_indexed)
+        return KnowledgeBaseFileInfo(kb_name=self.kb_name, file_name=self.file_name, is_cut=self.is_cut)
 
-    def cut(self, *args, **kwargs):
+    def cut(self, *args, **kwargs) -> List[Chunk]:
         logger.info(f"start cut file: {self.file_name}")
         chunks: List[Chunk] = parse_file(file_path=self.origin_path, *args, **kwargs)
-        kb_chunks = [KBChunk(**chunk.to_json(), idx=idx, kb_name=self.kb_name, file_name=self.file_name)
-                     for idx, chunk in enumerate(chunks) if chunk.content]
-        kb_chunk_json = [chunk.to_dict() for chunk in kb_chunks]
-        dump(kb_chunk_json, self.chunk_path)
-        return len(kb_chunks)
+        self._save_chunks(chunks=chunks)
+    
+    def _save_chunks(self, chunks: List[Chunk]):
+        chunk_json = [chunk.to_json() for chunk in chunks]
+        dump(chunk_json, self.chunk_path)
+        return chunks
 
-    def get_chunks(self) -> List[KBChunk]:
+    def list_chunks(self) -> List[Chunk]:
         """
         从切片文件加载切片
         """
         if not self.is_cut:
             return []
 
         chunk_dicts = load(self.chunk_path)
         logger.debug(f"loaded {len(chunk_dicts)} chunks from {self.chunk_path}")
-        chunks: List[KBChunk] = [KBChunk(**c, idx=idx, kb_name=self.kb_name, file_name=self.file_name) for idx, c in enumerate(chunk_dicts)]
+        chunks = [Chunk.from_dict(ele) for ele in chunk_dicts]
         return chunks
 
-    def remove(self):
+    def get_chunk_ids(self) -> List[str]:
+        chunks = self.list_chunks()
+        chunk_ids = [c.id for c in chunks]
+        return chunk_ids
+    
+    def get_chunk(self, idx: int) -> Chunk:
+        chunks = self.list_chunks()
+        if idx < 0 or idx >= len(chunks):
+            raise Exception(f"chunk index out of range, idx: {idx}, len: {len(chunks)}")
+        return chunks[idx]  
+
+    def add_chunks(self, chunks: List[Chunk], idx:int= None):
+        origin_chunks = self.list_chunks()
+        if idx is None:
+            idx = len(chunks)
+        chunks = origin_chunks[:idx] + chunks + origin_chunks[idx:]
+        self._save_chunks(chunks)
+
+    def delete_chunks(self, ids:List[str]):
+        chunks = self.list_chunks()
+        remain_chunks = [c for c in chunks if c.id not in ids]
+        self._save_chunks(remain_chunks)
+
+    
+    def update_chunk(self, chunk:Chunk)->bool:
+        # do delete
+        
+        chunks = self.list_chunks()
+        for idx, c in enumerate(chunks):
+            if c.id == chunk.id:
+                chunks[idx] = chunk
+                break
+        self._save_chunks(chunks)
+    
+    def delete(self):
         """
         删除知识库文档
         """
         for path in [self.origin_path, self.chunk_path]:
             if os.path.exists(path):
                 os.remove(path)
```

### Comparing `xagent-0.0.7/xagents/kb/vector_store.py` & `xagent-0.0.8/xagents/kb/vector_store.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,40 +4,46 @@
 @Time    :   2023/12/08 16:57:23
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 import copy
 import os
+import shutil
 from typing import List, Type
 from langchain.vectorstores.faiss import FAISS
 import faiss
 from langchain.vectorstores import VectorStore
 from langchain.docstore.in_memory import InMemoryDocstore
-from langchain.vectorstores.elasticsearch import ElasticsearchStore
 from langchain.vectorstores import VectorStore as VectorStore
 
 from xagents.model.common import EMBD
 from xagents.kb.common import DistanceStrategy
-
+from langchain_elasticsearch import ElasticsearchStore
 from loguru import logger
 
 
 class XVecStore(VectorStore):
     @classmethod
     def is_local(cls) -> bool:
         raise NotImplementedError()
 
+    def convert_score(self, score: float) -> float:
+        return score
+
     @classmethod
     def need_embd(cls):
         raise NotImplementedError()
 
     @classmethod
     def from_config(cls, config: dict):
         raise NotImplementedError()
+    
+    def delete_all(self):
+        raise NotImplementedError()
 
 
 class LocalVecStore(VectorStore):
     def __init__(self, local_dir: str, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.local_dir = local_dir
 
@@ -47,24 +53,33 @@
 
     @classmethod
     def load_local(cls):
         pass
 
     def save(self, *args, **kwargs):
         pass
-
+    
+    def delete_all(self):
+        logger.info(f"deleting vecstore from :{self.local_dir}")
+        if os.path.exists(self.local_dir):
+            shutil.rmtree(self.local_dir)
+        else:
+            logger.warning(f"{self.local_dir} not exists")
 
 class XFAISS(LocalVecStore, FAISS):
     @classmethod
     def is_local(cls):
         return True
 
     @classmethod
     def need_embd(cls):
-        return False
+        return True
+    
+    def convert_score(self, score: float) -> float:
+        return 1-score if self.distance_strategy == DistanceStrategy.EUCLIDEAN_DISTANCE else score
 
     @classmethod
     def from_config(cls, config: dict) ->"XFAISS":
         local_dir: str = config["local_dir"]
         embedding: EMBD = config["embedding"]
         distance_strategy = config.get("distance_strategy", DistanceStrategy.MAX_INNER_PRODUCT)
 
@@ -111,24 +126,34 @@
 class XES(XVecStore, ElasticsearchStore):
     @classmethod
     def is_local(cls):
         return False
 
     @classmethod
     def need_embd(cls):
-        return True
+        return False
 
     @classmethod
-    def from_config(cls, config: dict):
+    def from_config(cls, config: dict) -> "XES":
+        es_url: str = config["es_url"]
+        es_index: str = config["es_index"]
+
         vecstore = cls(
-            **config
+            es_url=es_url,
+            index_name=es_index,
+            strategy=ElasticsearchStore.BM25RetrievalStrategy(),
         )
-        return vecstore
 
+        return vecstore
+    
+    def delete_all(self):
+        logger.info(f"deleting vecstore with es_index:{self.index_name}")
+        self.client.indices.delete(index=self.index_name, ignore=[400, 404])
 
+    
 _vecstores = [XFAISS, XES]
 _name2vecstores = {e.__name__: e for e in _vecstores}
 
 
 def list_vecstores():
     return [e.__name__ for e in _vecstores]
```

### Comparing `xagent-0.0.7/xagents/loader/api.py` & `xagent-0.0.8/xagents/loader/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,31 +8,41 @@
 '''
 
 import os
 from loguru import logger
 from typing import Iterable, List, Type
 from xagents.loader.pdf_loader import PDFLoader
 from xagents.loader.docx_loader import DOCXLoader
-
-from xagents.loader.markdown import MarkDownLoader
-from xagents.loader.structed import StructedLoader
+from xagents.loader.doc_loader import DOCLoader
+from xagents.loader.csv_loader import CSVLoader
+from xagents.loader.excel_loader import EXCELLoader
+from xagents.loader.pptx_loader import PPTXLoader
+from xagents.loader.ppt_loader import PPTLoader
+
+from xagents.loader.markdown_loader import MarkDownLoader
+from xagents.loader.json_loader import JSONLoader
+from xagents.loader.jsonl_loader import JSONLLoader
 from xagents.loader.common import Chunk, AbstractLoader
 
 from xagents.loader.splitter import BaseSplitter
 from snippets import flat, log_cost_time
 
 _EXT2LOADER = {
     "pdf": PDFLoader,
     "markdown": MarkDownLoader,
     "md": MarkDownLoader,
-    "json": StructedLoader,
-    "jsonl": StructedLoader,
-    "csv": StructedLoader,
+    "json": JSONLoader,
+    "jsonl": JSONLLoader,
+    "csv": CSVLoader,
+    "xlsx": EXCELLoader,
     "txt": MarkDownLoader,
     "docx": DOCXLoader,
+    "doc": DOCLoader,
+    "pptx": PPTXLoader,
+    "ppt": PPTLoader,
     "": MarkDownLoader
 }
 
 
 def get_loader_cls(file_path: str) -> Type[AbstractLoader]:
     """根据file路径后缀，加载对应的文档加载器
 
@@ -118,18 +128,20 @@
         min_len (int, optional): 最小切片长度. Defaults to 10.
 
     Returns:
         List[Chunk]: 切片列表
     """
 
     splitter = BaseSplitter(max_len=max_len, min_len=min_len, separator=separator)
+    # logger.debug(f"splitter: {splitter}")
     origin_chunks: Iterable[Chunk] = load_file(file_path=file_path, start_page=start_page,
                                                end_page=end_page, upload_image=upload_image, ocr=ocr)
     origin_chunks = list(origin_chunks)
     logger.debug(f"load {len(origin_chunks)} origin_chunks")
+    # logger.debug(f"{origin_chunks[0]=}")
     if do_cut:
         split_chunks = flat([splitter.split_chunk(origin_chunk) for origin_chunk in origin_chunks])
         logger.info(f"split {len(origin_chunks)} origin_chunks to {len(split_chunks)} chunks")
         return split_chunks
     else:
         return origin_chunks
```

### Comparing `xagent-0.0.7/xagents/loader/common.py` & `xagent-0.0.8/xagents/loader/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 
 from abc import abstractmethod
 import enum
-from loguru import logger
+import uuid
 from pathlib import Path
 from typing import Iterable, List, Optional, Tuple
 
 from pydantic import BaseModel, Field, ConfigDict, validator
 from pandas import DataFrame
 from numpy import ndarray
 from xagents.config import *
@@ -39,57 +39,70 @@
     y1: float
     @property
     def sort_key(self):
         return (self.y0, self.x0)
     
     def to_tuple(self):
         return (self.x0, self.y0, self.x1, self.y1)
+    
+
+
 
 class Chunk(BaseModel):
+    id:str = Field(description="chunk的id", default_factory=lambda:str(uuid.uuid4()))
     content: str = Field(description="chunk的内容")
     content_type: ContentType = Field(description="chunk类型", default=ContentType.TEXT)
     search_content: Optional[str] = Field(description="用来检索的内容", default=None)
-    page_idx: int = Field(description="chunk在文档中的页码,从1开始")
+    page_idx: int = Field(description="chunk在文档中的页码,从1开始", default=1)
     
     def to_json(self):
         return self.model_dump(exclude_none=True)
 
-
+    @classmethod
+    def from_dict(cls, data:dict) -> "Chunk":
+        content_type = data["content_type"]
+        cls:type[BaseModel] =_content_type2cls[content_type]
+        return cls.model_validate(data)
+        
 class TextChunk(Chunk):
     content_type:ContentType=ContentType.TEXT
     
 class ImageChunk(Chunk):
     content_type:ContentType=ContentType.IMAGE
     content: Optional[str] = Field(description="image的文字描述", default=None)
     url:Optional[str] = Field(description="图片的url", default=None)
     image_name:str = Field(description="图片的文件名")
 
 class TableChunk(Chunk):
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     content_type:ContentType=ContentType.TABLE
-    data: ndarray|DataFrame = Field(description="表格的数据, 二维数组或pandas的dataframe")
+    data: Optional[ndarray|DataFrame] = Field(description="表格的数据, 二维数组或pandas的dataframe", default=None)
     content: str = Field(description="表格的文字描述, markdown格式", default=None)
     
     def to_json(self):
         return self.model_dump(exclude_none=True, exclude={"data"})
 
-
-    
     @validator('data', pre=True, always=True)
     def set_content_based_on_data(cls, v, values, **kwargs):
-        logger.info(f"{values=}")
+        # logger.info(f"{values=}")
         # Check if description is already set
         if values.get("content") is None:
             content = data2markdown(v)
             values["content"] = content
             return v
         return v    
 
 
+_content_type2cls={
+    ContentType.TABLE: TableChunk,
+    ContentType.TEXT: TextChunk,
+    ContentType.IMAGE: ImageChunk,
+}
+
 class AbstractLoader:
     def __init__(self, **kwargs) -> None:
         pass
     @abstractmethod
     def load(self, file_path: str,  start_page:int=0, end_page:int=None, store_image=True, ocr=False, **kwargs) -> List[Chunk]:
         raise NotImplementedError
 
@@ -105,19 +118,15 @@
             if acc:
                 yield TextChunk(content=acc, page_idx=cur_page_idx)
                 acc = None
             yield chunk
     if acc:
         yield TextChunk(content=acc, page_idx=cur_page_idx)
             
-        
-
-def upload_image(local_path:str, remote_url:str)->str:
-    return f"{remote_url}/{local_path}"
-
+    
 
 def get_image_name_path(kf_file_name:str, page_idx:int, image_idx:int)->Tuple[str, str]:
     image_name =f"{Path(kf_file_name).stem}-page{page_idx}-image{image_idx}.png"
     file_path = os.path.join(TEMP_DIR, "extracted_images", image_name)
     os.makedirs(os.path.dirname(file_path), exist_ok=True)
     return image_name, file_path
```

### Comparing `xagent-0.0.7/xagents/loader/docx_loader.py` & `xagent-0.0.8/xagents/loader/docx_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 
 
 from typing import Iterable
 
 import docx.table
 
 
+from xagents.loader.utils import upload_to_minio, image2text
 from xagents.config import *
-from xagents.loader.common import Chunk, AbstractLoader, ImageChunk, TextChunk, TableChunk, get_image_name_path, merge_chunks, upload_image as do_upload_image
+from xagents.loader.common import Chunk, AbstractLoader, ImageChunk, TextChunk, TableChunk, get_image_name_path, merge_chunks
 
 import docx
 import pandas as pd
 
+from PIL import Image
 from docx.text.paragraph import Paragraph
 import xml.etree.ElementTree as ET
 from docx.document import Document as DOC
 from docx.oxml.table import CT_Tbl
 from docx.oxml.text.paragraph import CT_P
 from docx.table import _Cell
 from xml.etree import ElementTree
@@ -112,27 +114,27 @@
                         image_part = document_part.related_parts[embed_attr]
                         image_name, image_path =get_image_name_path(file_name, 0, image_idx)    
 
                         if upload_image:
                             with open(image_path, "wb") as f:
                                 f.write(image_part._blob)
                 
-                            url = do_upload_image(image_path, "http://cdn")
+                            url = upload_to_minio(image_path)
                         else:
-                            url=None,
-                        content = "" if ocr else None
+                            url=None
+                        content = image2text(Image.open(io.BytesIO(image_part._blob))) if ocr else None
                         # image_base64 = base64.b64encode(image_part._blob)
                         # image_base64 = image_base64.decode()        
                         yield ImageChunk(url=url, content=content,page_idx=page_index, image_name=image_name)
                     image_idx = image_idx + 1
                 
         elif 'table' in str(block):
             content = str(block)
             df:pd.DataFrame = read_docx_tables(document=document,tab_id=table_idx)
-            yield TableChunk(page_idx=page_index, data=df)            
+            yield TableChunk(page_idx=page_index, data=df)
             table_idx+=1
 
             
 class DOCXLoader(AbstractLoader):
     def __init__(self, max_page:int=None, **kwargs):
         """构建pdf加载器
 
@@ -140,15 +142,15 @@
             max_page (int, optional): 最大页数. Defaults to None：不限定页数
             extract_images (bool, optional): 是否使用ocr抽取其中的图片. Defaults to False.
         """
         super().__init__(**kwargs)
         self.max_page = max_page
 
 
-    def load(self, file_path: str, start_page=1, end_page=None, upload_image=True, ocr=False) -> Iterable[Chunk]:
+    def load(self, file_path: str, start_page=1, end_page=None, upload_image=True, ocr=False, **kwargs) -> Iterable[Chunk]:
         #TODO 缺少页码控制
         doc = docx.Document(file_path)
         chunks = analyse_page(doc, file_name=os.path.basename(file_path), upload_image=upload_image, ocr=ocr)
         chunks = merge_chunks(chunks)
         yield from chunks
```

### Comparing `xagent-0.0.7/xagents/loader/markdown.py` & `xagent-0.0.8/xagents/loader/markdown_loader.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 
 import os
 import re
-from typing import List
-from xagents.loader.common import AbstractLoader, Chunk
+from typing import Iterable
+from xagents.loader.common import AbstractLoader, Chunk, TextChunk
+from loguru import logger
 
 
 def extract_md_table(text):
     tables = re.findall("^\\|(.*)\\|$", text, re.MULTILINE | re.DOTALL)
     return tables
 
 
 class MarkDownLoader(AbstractLoader):
-    def load(self, file_path: str) -> List[Chunk]:
+    def load(self, file_path: str, **kwargs) -> Iterable[Chunk]:
         with open(file_path, "r") as f:
             content = f.read()
-            return [Chunk(content=content, page_idx=1)]
+            # logger.debug(f"{content=}")
+            yield TextChunk(content=content, page_idx=1)
 
 
 if __name__ == "__main__":
     from xagents.config import XAGENT_HOME
     loader = MarkDownLoader()
 
     file_path = os.path.join(XAGENT_HOME, "data/raw/贵州茅台2022年报-4.md")
```

### Comparing `xagent-0.0.7/xagents/loader/pdf_loader.py` & `xagent-0.0.8/xagents/loader/pdf_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,35 +7,30 @@
 '''
 
 import numpy as np
 from loguru import logger
 from typing import Iterable, List, Tuple
 
 
+from xagents.loader.utils import upload_to_minio, image2text
 from xagents.config import *
-from xagents.loader.common import BBox, Chunk, TableChunk, TextChunk, ImageChunk, get_image_name_path, merge_chunks, upload_image as do_upload_image, AbstractLoader
+from xagents.loader.common import BBox, Chunk, TableChunk, TextChunk, ImageChunk, get_image_name_path, merge_chunks, AbstractLoader
 from pdfplumber.page import Page
 
 
 
 
 def analyse_page(idx:int, page:Page, file_name:str, upload_image:bool, ocr:bool)->Iterable[Chunk]:
             
     chunks:List[Tuple[Chunk, BBox]] = []  # List to store all content with their position
 
     # 抽取文本
     for line in  page.extract_text_lines(x_tolerance=3, y_tolerance=3):
         chunks.append((TextChunk(content=line['text'], page_idx=idx), BBox(x0=line["x0"], y0=line["top"], x1=line["x1"], y1=line["bottom"])))
 
-    # Extract tables and add to content list
-    # tables = page.extract_tables({
-    #     "horizontal_strategy": "text",
-    #     "vertical_strategy": "text",
-    # })
-    # print(tables)
     tables = page.extract_tables()
     for table in tables:
         bbox = BBox(x0=0, x1=0, y0=0, y1=0)
         # logger.info(f"table: {table}")
 
         table = np.array(table)
         chunks.append((TableChunk(data=table, page_idx=idx), bbox))
@@ -48,20 +43,19 @@
         image = page_image.crop(bbox.to_tuple())
         
         
         image_name, image_path =get_image_name_path(file_name, idx, i)     
         if upload_image:
             os.makedirs(os.path.dirname(image_path), exist_ok=True)
             image.save(image_path, format="PNG")
-            url= do_upload_image(image_path, "http://cdn/")
+            url= upload_to_minio(image_path)
         else:
             url=None
         if ocr:
-            #TODO 调用ocr
-            content = ""
+            content = image2text(image)
         else:
             content = None
         chunks.append((ImageChunk(url=url, content=content, image_name=image_name, page_idx=idx), bbox))
         
     chunks.sort(key=lambda x: x[1].sort_key)  # Sort by top y coordinate, then by left x coordinate
     yield from (x[0] for x in chunks)
```

### Comparing `xagent-0.0.7/xagents/loader/splitter.py` & `xagent-0.0.8/xagents/loader/splitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     @abstractmethod
     def split(self, text: str) -> List[str]:
         raise NotImplementedError
 
     def split_chunk(self, chunk: Chunk) -> Iterable[Chunk]:
         if chunk.content_type == ContentType.TABLE or chunk.content_type==ContentType.IMAGE:
-            # 图片和表格暂时不做切割
+            # 图片、表格和 json 暂时不做切割
             yield chunk
         else:
 
             for content in self.split(chunk.content):
                 content = content.strip()
                 if content in self.invalid_chunks:
                     continue
```

### Comparing `xagent-0.0.7/xagents/loader/structed.py` & `xagent-0.0.8/xagents/loader/structed.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.7/xagents/model/api.py` & `xagent-0.0.8/xagents/model/api.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.7/xagents/model/common.py` & `xagent-0.0.8/xagents/model/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,16 +67,15 @@
         return f"[{self.name}]-{self.version}"
 
     def __repr__(self):
         return self.__str__()
 
 
 class EMBD(Embeddings):
-    @classmethod
-    def get_dim(cls) -> int:
+    def get_dim(self) -> int:
         raise NotImplementedError
 
 class Reranker:
     def __init__(self, name: str, version: str):
         self.name = name
         self.version = version
```

### Comparing `xagent-0.0.7/xagents/model/local.py` & `xagent-0.0.8/xagents/model/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,34 +25,34 @@
     resp = requests.post(url=url, json=dict(texts=contents, norm=norm))
     resp.raise_for_status()
     return resp.json()["data"]['embeddings']
 
 
 class LocalEmbedding(EMBD):
 
-    def __init__(self,  url="http://hz-model.bigmodel.cn/embedding-models/v2/embeddings", batch_size=16, norm=True):
+    def __init__(self,  url="http://hz-model.bigmodel.cn/embedding-models/v2/embeddings", batch_size=16, norm=True, dim=1024):
         self.batch_size = batch_size
         self.norm = norm
         self.url = url
+        self.dim=dim
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         logger.info(f"embedding {len(texts)} with {self.batch_size=}")
         embeddings = call_embedding(text=texts,model_or_url=self.url, embd_type=EMBD_TYPE.LOCAL,
                                     norm=self.norm, batch_size=self.batch_size)
         
         return embeddings
 
     def embed_query(self, text: str) -> List[float]:
         embedding = call_embedding(text=text,model_or_url=self.url, embd_type=EMBD_TYPE.LOCAL,
                                     norm=self.norm, batch_size=self.batch_size)
         return embedding
 
-    @classmethod
-    def get_dim(cls) -> int:
-        return 1024
+    def get_dim(self) -> int:
+        return self.dim
 
 
 class TGI_GLM(LLM):
     """
     本地调用LLM
     """
```

### Comparing `xagent-0.0.7/xagents/model/openai.py` & `xagent-0.0.8/xagents/model/openai.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.7/xagents/model/zhipu.py` & `xagent-0.0.8/xagents/model/zhipu.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,15 @@
         return embeddings
 
     def embed_query(self, text: str) -> List[float]:
         embedding = call_embedding(text=text, embd_type=EMBD_TYPE.ZHIPU_API, model_or_url="embedding-2",
                                    norm=self.norm, batch_size=self.batch_size)
         return embedding
 
-    @classmethod
-    def get_dim(cls) -> int:
+    def get_dim(self) -> int:
         return 1024
 
 
 class ZhipuReranker(Reranker):
     def __init__(self,  url: str, name="reranker", version="ZhipuReranker"):
         self.url = url
         super().__init__(name=name, version=version)
```

### Comparing `xagent-0.0.7/xagents/tool/api.py` & `xagent-0.0.8/xagents/tool/api.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.7/xagents/tool/common_tool.py` & `xagent-0.0.8/xagents/tool/common_tool.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.7/xagents/tool/web_search.py` & `xagent-0.0.8/xagents/tool/web_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,23 @@
+import re
+from fake_useragent import UserAgent
+from agit.common import Parameter
+from xagents.tool.core import BaseTool
 import requests
 from bs4 import BeautifulSoup
 import time
 import random
 
 import requests
 import chardet
-import sys
-sys.path.append("../../")
-from xagents.tool.core import BaseTool
-from agit.common import Parameter
-from typing import Any, Callable, Dict, List
-from pydantic import BaseModel, Field
 
-from fake_useragent import UserAgent
-import time
-import re
 
 def get_search_result(url):
     headers = {
-        "User-Agent": UserAgent().random,#Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36"
+        "User-Agent": UserAgent().random,  # Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36"
     }
     try:
         response = requests.get(url, headers=headers)
         # 使用 chardet 检测网页编码
         encoding = chardet.detect(response.content)['encoding']
         # 设置解码方式
         response.encoding = encoding
@@ -32,15 +27,14 @@
             # 解析搜索结果页面，这里以输出标题和链接为例
             soup_text = soup.text
             return soup_text
     except:
         return ""
 
 
-
 def sogou_search(query):
     url = f"https://www.sogou.com/web"
     # "http://www.so.com/s?q=keyword"
     # f"https://www.sogou.com/web"
     params = {"query": query}
 
     headers = {
@@ -59,24 +53,24 @@
         # 等待一段随机时间，模拟人类操作
         time.sleep(random.uniform(1, 2))
         sub_page_contents = []
         sub_page_links = []
         if response.status_code == 200:
             soup = BeautifulSoup(response.text, "html.parser")
             # 解析搜索结果页面，这里以输出标题和链接为例
-            soup_text = soup.text# str(soup)
+            soup_text = soup.text  # str(soup)
             pattern = r'data-url="(.*?)"'
             urls = re.findall(pattern, soup_text)
             if len(urls) >= 1:
                 for url_temp in urls:
                     sub_page_links.append(url_temp)
                     sub_page_contents.append(get_search_result(url_temp))
             else:
                 sub_page_links = []
-                sub_page_contents.append(soup_text.replace("\n\n",""))
+                sub_page_contents.append(soup_text.replace("\n\n", ""))
 
             return sub_page_links, sub_page_contents
         else:
             print(f"Error: Failed to fetch search results (status code {response.status_code})")
             return None, None
     except Exception as e:
         print(f"Error: {str(e)}")
@@ -174,24 +168,22 @@
     except requests.exceptions.RequestException as e:
         print(f"An error occurred: {e}")
 
     return None
 
 # print(fetch_baidu_search_results("江泽民生平"))
 
+
 web_search_sogou = BaseTool(name="联网查询", description="根据用户提供的输入，通过搜索引擎从网上去查询信息，尤其是实时的信息",
-                           parameters=[Parameter(name="query", description="搜索的语句", type="string", required=True)],
-                           callable=sogou_search)
+                            parameters=[Parameter(name="query", description="搜索的语句", type="string", required=True)],
+                            callable=sogou_search)
 
 
 # 测试搜索功能
 if __name__ == "__main__":
     keyword = "邓小平生平"
     # web_search = WebSearch()
     # search_results = web_search.sogou_search(keyword)
     search_links, search_contents = web_search_sogou.execute(query=keyword)
     print(f"Search results for '{search_links}':")
     print("text:", search_contents)
     # from snippets.logs import ChangeLogLevelContext
-
-
-
```

### Comparing `xagent-0.0.7/xagents/util.py` & `xagent-0.0.8/xagents/util.py`

 * *Files identical despite different names*

