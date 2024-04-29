# Comparing `tmp/research-framework-0.1.9.tar.gz` & `tmp/research_framework-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "research-framework-0.1.9.tar", last modified: Wed Sep  6 14:58:45 2023, max compression
+gzip compressed data, was "research_framework-0.2.1.tar", last modified: Mon Apr 29 17:52:41 2024, max compression
```

## Comparing `research-framework-0.1.9.tar` & `research_framework-0.2.1.tar`

### file list

```diff
@@ -1,73 +1,122 @@
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.684437 research-framework-0.1.9/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    35149 2023-09-01 08:34:48.000000 research-framework-0.1.9/LICENSE
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       24 2023-09-01 08:34:48.000000 research-framework-0.1.9/MANIFEST.in
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      624 2023-09-06 14:58:45.684437 research-framework-0.1.9/PKG-INFO
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      196 2023-09-06 13:45:32.000000 research-framework-0.1.9/requirements.txt
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       40 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/__init__.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/base/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/base/__init__.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/base/container/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/base/container/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      428 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/base/container/base_container.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/base/container/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/base/container/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      509 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/base/container/model/bind_model.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/base/flyweight/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/base/flyweight/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      736 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/base/flyweight/base_flyweight.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/base/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/base/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2443 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/base/model/base_dao.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      567 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/base/model/base_utils.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/base/plugin/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/base/plugin/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      177 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/base/plugin/base_plugin.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/base/storage/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/base/storage/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4637 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/base/storage/google_storage.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/base/wrappers/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/base/wrappers/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      221 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/base/wrappers/filter_wrapper.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/container/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/container/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1712 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/container/container.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/lightweight/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/lightweight/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3788 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/lightweight/lightweight.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/lightweight/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/lightweight/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1011 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/lightweight/model/item_dao.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      536 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/lightweight/model/item_model.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/pipeline/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       48 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/pipeline/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      491 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/pipeline/inputs.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/pipeline/model/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/pipeline/model/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      818 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/pipeline/model/pipeline_model.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2144 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/pipeline/pipeline.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     5607 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/pipeline/wrappers.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework/plugins/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      121 2023-09-01 08:34:48.000000 research-framework-0.1.9/research_framework/plugins/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      826 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/plugins/data_ingestion_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1545 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/plugins/text_mod_plugins.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1518 2023-09-06 13:45:32.000000 research-framework-0.1.9/research_framework/plugins/text_rep_plugins.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/research_framework.egg-info/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      624 2023-09-06 14:58:45.000000 research-framework-0.1.9/research_framework.egg-info/PKG-INFO
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1985 2023-09-06 14:58:45.000000 research-framework-0.1.9/research_framework.egg-info/SOURCES.txt
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        1 2023-09-06 14:58:45.000000 research-framework-0.1.9/research_framework.egg-info/dependency_links.txt
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      195 2023-09-06 14:58:45.000000 research-framework-0.1.9/research_framework.egg-info/requires.txt
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       32 2023-09-06 14:58:45.000000 research-framework-0.1.9/research_framework.egg-info/top_level.txt
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/scripts/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research-framework-0.1.9/scripts/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      183 2023-09-06 13:45:32.000000 research-framework-0.1.9/scripts/clean_storage.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       38 2023-09-06 14:58:45.684437 research-framework-0.1.9/setup.cfg
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1058 2023-09-06 14:58:20.000000 research-framework-0.1.9/setup.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.680437 research-framework-0.1.9/test/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research-framework-0.1.9/test/__init__.py
-drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 14:58:45.684437 research-framework-0.1.9/test/plugins/
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research-framework-0.1.9/test/plugins/__init__.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      652 2023-09-06 13:45:32.000000 research-framework-0.1.9/test/plugins/test_plugin.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      837 2023-09-06 13:45:32.000000 research-framework-0.1.9/test/test_container_bindings.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2069 2023-09-06 13:45:32.000000 research-framework-0.1.9/test/test_flyweight.py
--rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1929 2023-09-06 13:45:32.000000 research-framework-0.1.9/test/test_pipeline.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.150113 research_framework-0.2.1/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    35149 2023-09-01 08:34:48.000000 research_framework-0.2.1/LICENSE
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       24 2023-09-01 08:34:48.000000 research_framework-0.2.1/MANIFEST.in
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1310 2024-04-29 17:52:41.150113 research_framework-0.2.1/PKG-INFO
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      393 2024-04-10 15:04:36.000000 research_framework-0.2.1/requirements.txt
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       91 2023-11-07 13:43:38.000000 research_framework-0.2.1/research_framework/__init__.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/base/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.1/research_framework/base/__init__.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/base/container/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.1/research_framework/base/container/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1990 2023-11-09 16:51:42.000000 research_framework-0.2.1/research_framework/base/container/base_container.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/base/container/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.1/research_framework/base/container/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      722 2023-09-19 17:54:13.000000 research_framework-0.2.1/research_framework/base/container/model/bind_model.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/base/flyweight/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.1/research_framework/base/flyweight/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1074 2023-11-08 13:26:10.000000 research_framework-0.2.1/research_framework/base/flyweight/base_flyweight.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      800 2024-04-25 16:51:06.000000 research_framework-0.2.1/research_framework/base/flyweight/base_flyweight_manager.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/base/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.1/research_framework/base/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2550 2024-03-02 14:06:30.000000 research_framework-0.2.1/research_framework/base/model/base_dao.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      567 2023-09-01 08:34:48.000000 research_framework-0.2.1/research_framework/base/model/base_utils.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/base/pipeline/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-11-06 20:33:03.000000 research_framework-0.2.1/research_framework/base/pipeline/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      227 2023-12-29 14:25:32.000000 research_framework-0.2.1/research_framework/base/pipeline/base_pipeline.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/base/plugin/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.1/research_framework/base/plugin/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1029 2023-10-15 10:47:16.000000 research_framework-0.2.1/research_framework/base/plugin/base_plugin.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      337 2024-04-25 10:02:49.000000 research_framework-0.2.1/research_framework/base/plugin/base_wrapper.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/base/singleton/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-25 16:03:32.000000 research_framework-0.2.1/research_framework/base/singleton/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      262 2024-04-25 16:34:16.000000 research_framework-0.2.1/research_framework/base/singleton/base_singleton.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/base/storage/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.1/research_framework/base/storage/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      545 2024-04-25 16:34:46.000000 research_framework-0.2.1/research_framework/base/storage/base_storage.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/base/utils/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-21 13:26:13.000000 research_framework-0.2.1/research_framework/base/utils/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1503 2023-11-08 11:20:29.000000 research_framework-0.2.1/research_framework/base/utils/grid_seach.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      308 2023-09-19 18:09:27.000000 research_framework-0.2.1/research_framework/base/utils/method_overload.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/container/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.1/research_framework/container/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     5051 2024-04-25 18:49:10.000000 research_framework-0.2.1/research_framework/container/container.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/container/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-17 21:22:31.000000 research_framework-0.2.1/research_framework/container/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      472 2023-12-29 13:57:37.000000 research_framework-0.2.1/research_framework/container/model/global_config.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/dataset/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-15 10:07:36.000000 research_framework-0.2.1/research_framework/dataset/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      872 2023-09-20 22:03:33.000000 research_framework-0.2.1/research_framework/dataset/basic_dataset.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1071 2023-11-07 10:26:41.000000 research_framework-0.2.1/research_framework/dataset/standard_dataset.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.142112 research_framework-0.2.1/research_framework/flyweight/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.1/research_framework/flyweight/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     8026 2024-04-24 16:58:20.000000 research_framework-0.2.1/research_framework/flyweight/flyweight.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    14387 2024-04-25 17:28:03.000000 research_framework-0.2.1/research_framework/flyweight/flyweight_manager.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3581 2024-04-29 11:35:05.000000 research_framework-0.2.1/research_framework/flyweight/mem_manager.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.146113 research_framework-0.2.1/research_framework/flyweight/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.1/research_framework/flyweight/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1011 2023-09-06 13:45:32.000000 research_framework-0.2.1/research_framework/flyweight/model/item_dao.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      659 2023-11-08 13:27:58.000000 research_framework-0.2.1/research_framework/flyweight/model/item_model.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      497 2024-04-10 01:30:54.000000 research_framework-0.2.1/research_framework/flyweight/model/item_simple_model.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.146113 research_framework-0.2.1/research_framework/neural_models/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-15 10:13:05.000000 research_framework-0.2.1/research_framework/neural_models/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      379 2023-09-13 12:58:06.000000 research_framework-0.2.1/research_framework/neural_models/doomy_model.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.146113 research_framework-0.2.1/research_framework/pipeline/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       48 2023-11-07 13:43:32.000000 research_framework-0.2.1/research_framework/pipeline/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      491 2023-09-06 13:45:32.000000 research_framework-0.2.1/research_framework/pipeline/inputs.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.146113 research_framework-0.2.1/research_framework/pipeline/model/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.1/research_framework/pipeline/model/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3233 2024-04-25 16:57:27.000000 research_framework-0.2.1/research_framework/pipeline/model/pipeline_model.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     9541 2024-04-29 11:56:38.000000 research_framework-0.2.1/research_framework/pipeline/pipeline.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2607 2024-04-25 18:49:05.000000 research_framework-0.2.1/research_framework/pipeline/pipeline_manager.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.146113 research_framework-0.2.1/research_framework/plugins/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      416 2023-09-17 16:58:56.000000 research_framework-0.2.1/research_framework/plugins/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     5755 2024-04-29 17:32:18.000000 research_framework-0.2.1/research_framework/plugins/cv_strategies_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1626 2024-04-10 02:28:58.000000 research_framework-0.2.1/research_framework/plugins/data_ingestion_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4391 2023-09-21 10:17:00.000000 research_framework-0.2.1/research_framework/plugins/doomy_predictor.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)    11586 2024-04-10 00:55:18.000000 research_framework-0.2.1/research_framework/plugins/grid_search_cross_val.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2911 2024-04-29 12:02:49.000000 research_framework-0.2.1/research_framework/plugins/metrics_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1526 2023-09-20 20:59:39.000000 research_framework-0.2.1/research_framework/plugins/text_mod_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4267 2023-09-20 22:03:53.000000 research_framework-0.2.1/research_framework/plugins/text_rep_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6845 2024-04-29 12:14:04.000000 research_framework-0.2.1/research_framework/plugins/unsupervised_predictor.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1096 2023-09-19 18:12:57.000000 research_framework-0.2.1/research_framework/plugins/vector_red_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2764 2024-04-29 17:26:12.000000 research_framework-0.2.1/research_framework/plugins/wandb_sweep_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4460 2024-04-24 20:06:57.000000 research_framework-0.2.1/research_framework/plugins/wrappers.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.146113 research_framework-0.2.1/research_framework/storage/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-11-02 20:07:06.000000 research_framework-0.2.1/research_framework/storage/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4770 2024-04-25 16:30:23.000000 research_framework-0.2.1/research_framework/storage/google_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1732 2024-04-25 16:33:38.000000 research_framework-0.2.1/research_framework/storage/local_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     2893 2024-04-25 16:30:12.000000 research_framework-0.2.1/research_framework/storage/s3_storage.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.150113 research_framework-0.2.1/research_framework.egg-info/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1310 2024-04-29 17:52:41.000000 research_framework-0.2.1/research_framework.egg-info/PKG-INFO
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3817 2024-04-29 17:52:41.000000 research_framework-0.2.1/research_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        1 2024-04-29 17:52:41.000000 research_framework-0.2.1/research_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      386 2024-04-29 17:52:41.000000 research_framework-0.2.1/research_framework.egg-info/requires.txt
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       32 2024-04-29 17:52:41.000000 research_framework-0.2.1/research_framework.egg-info/top_level.txt
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.146113 research_framework-0.2.1/scripts/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.1/scripts/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      507 2023-09-19 19:10:14.000000 research_framework-0.2.1/scripts/clean.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      183 2023-09-06 13:45:32.000000 research_framework-0.2.1/scripts/clean_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)       38 2024-04-29 17:52:41.150113 research_framework-0.2.1/setup.cfg
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1059 2024-04-23 10:14:50.000000 research_framework-0.2.1/setup.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.146113 research_framework-0.2.1/test/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-01 08:34:48.000000 research_framework-0.2.1/test/__init__.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.146113 research_framework-0.2.1/test/metrics/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-25 16:39:11.000000 research_framework-0.2.1/test/metrics/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      757 2024-04-25 18:51:45.000000 research_framework-0.2.1/test/metrics/test_metrics.py
+drwxr-xr-x   0 manuel.couto.pintos  (4125) citius    (2000)        0 2024-04-29 17:52:41.150113 research_framework-0.2.1/test/plugins/
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)        0 2023-09-06 13:45:32.000000 research_framework-0.2.1/test/plugins/__init__.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      644 2024-04-25 18:08:47.000000 research_framework-0.2.1/test/plugins/test_mem_plugins.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     1796 2023-09-20 12:11:32.000000 research_framework-0.2.1/test/plugins/test_plugin.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)      956 2023-11-07 13:40:25.000000 research_framework-0.2.1/test/test_container_bindings.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3554 2023-11-07 12:38:53.000000 research_framework-0.2.1/test/test_flyweight_with_google_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3581 2023-11-06 20:17:48.000000 research_framework-0.2.1/test/test_flyweight_with_local_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     3555 2024-01-14 01:08:22.000000 research_framework-0.2.1/test/test_flyweight_with_s3_storage.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6278 2024-04-26 12:01:06.000000 research_framework-0.2.1/test/test_mem_module.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     7174 2023-12-29 14:28:04.000000 research_framework-0.2.1/test/test_pipeline.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6881 2023-12-29 14:27:46.000000 research_framework-0.2.1/test/test_pipeline_grid_search.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6934 2024-04-25 16:54:39.000000 research_framework-0.2.1/test/test_simple_pipeline.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     6510 2024-04-10 01:52:30.000000 research_framework-0.2.1/test/test_simple_pipeline_manager.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     8532 2024-04-29 17:18:12.000000 research_framework-0.2.1/test/test_simple_pipeline_with_sweep_supervised.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     8449 2024-04-29 12:25:07.000000 research_framework-0.2.1/test/test_simple_pipeline_with_sweep_unsupervised.py
+-rw-r--r--   0 manuel.couto.pintos  (4125) citius    (2000)     4580 2023-09-20 12:16:43.000000 research_framework-0.2.1/test/test_wrappers_type_validation.py
```

### Comparing `research-framework-0.1.9/LICENSE` & `research_framework-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `research-framework-0.1.9/research_framework/base/model/base_dao.py` & `research_framework-0.2.1/research_framework/base/model/base_dao.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,15 +38,18 @@
             cls.database.drop()
         else:
             raise Exception("Dao Not propertly initialized")
             
     @classmethod
     def create(cls, entity:Any, *args, **kwargs) -> Any:
         if cls.database != None:
-            del entity.id
+            if hasattr(entity,'id'):
+                del entity.id
+            elif 'id' in entity:
+                del entity['id']
             entity = entity.model_dump()
             new_entity = cls.database.insert_one(entity, *args, **kwargs)
             return new_entity
         else:
             raise Exception("Dao Not propertly initialized")
     
     @classmethod
```

### Comparing `research-framework-0.1.9/research_framework/base/model/base_utils.py` & `research_framework-0.2.1/research_framework/base/model/base_utils.py`

 * *Files identical despite different names*

### Comparing `research-framework-0.1.9/research_framework/base/storage/google_storage.py` & `research_framework-0.2.1/research_framework/storage/google_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from googleapiclient.http import MediaInMemoryUpload, MediaIoBaseDownload
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 from google.oauth2 import service_account
 from google.cloud.storage import Client
 from requests.exceptions import ConnectionError
+from research_framework.base.storage.base_storage import BaseStorage
 import io
 import os
 import json 
 import pickle
 
-class BucketStorage:
-    def __init__(self, service='drive'):
+class BucketStorage(BaseStorage):
+    def __init__(self):
+        print("Se está instanciando el Bucket Storage")
         creds = service_account.Credentials.from_service_account_file(os.environ["GOOGLE_APPLICATION_CREDENTIALS"], scopes=list(json.loads(os.environ["ACCOUNT_SCOPES"])))
         if os.environ['DELEGATE_TO'] is not None:
             creds = creds.with_subject(os.environ['DELEGATE_TO'])
         self.creds = creds
         self.session = Client(project='tfm-project', credentials=self.creds)
         self.bucket = self.session.bucket(os.environ['BUCKET_NAME'])
         
@@ -64,15 +66,15 @@
         blob = self.bucket.blob(file_id)
         if blob.exists():
             blob.delete()
         else:
             raise FileExistsError("No existe en el bucket")
     
 
-class DriveStrage():
+class DriveStrage(BaseStorage):
     def __init__(self, delegate=False):
         creds = service_account.Credentials.from_service_account_file(os.environ["GOOGLE_APPLICATION_CREDENTIALS"], scopes=list(json.loads(os.environ["ACCOUNT_SCOPES"])))
         if os.environ['DELEGATE_TO'] is not None and delegate:
             creds = creds.with_subject(os.environ['DELEGATE_TO'])
         self.creds = creds
         self.session = build('drive', 'v3', credentials=self.creds)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `research-framework-0.1.9/research_framework/lightweight/model/item_dao.py` & `research_framework-0.2.1/research_framework/flyweight/model/item_dao.py`

 * *Files identical despite different names*

### Comparing `research-framework-0.1.9/research_framework/lightweight/model/item_model.py` & `research_framework-0.2.1/research_framework/flyweight/model/item_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from typing import Optional, Dict, Any
 from pydantic import BaseModel, Field, ConfigDict
 from research_framework.base.model.base_utils import PyObjectId
+from typing import ForwardRef
 
 
+ItemModel = ForwardRef('ItemModel')
+
 class ItemTypeModel(BaseModel):
     name: str
     clazz: str
-
+    
 class ItemModel(BaseModel):
     id: Optional[PyObjectId] = Field(alias="_id", default=None)
     name: str
     hash_code: str
+    prev_model: Optional[ItemModel] = None
     clazz: str
     params: Dict[str, Any]
-    type: Optional[ItemTypeModel] = None
+    stored: bool = False
 
     model_config = ConfigDict(
         arbitrary_types_allowed = True,
         populate_by_name = True
     )
 
+ItemModel.model_rebuild()
```

### Comparing `research-framework-0.1.9/setup.py` & `research_framework-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         str(requirement)
         for requirement
         in parse_requirements(requirements_txt)
     ]
 
 setup(
     name="research-framework",
-    version='0.1.9',
+    version='0.2.1',
     description="framework base para investigación",
     url="https://github.com/manucouto1/research_framework",
     author="Manuel Couto Pintos",
     author_email="manuel.couto.pintos@usc.es",
     license="Apache License",
     packages=find_packages(),
     install_requires=install_requires,
@@ -27,8 +27,8 @@
         'License :: OSI Approved :: BSD License',  
         'Operating System :: POSIX :: Linux',        
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
     ],
 
-)
+)
```

