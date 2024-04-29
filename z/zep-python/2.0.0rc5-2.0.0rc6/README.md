# Comparing `tmp/zep_python-2.0.0rc5.tar.gz` & `tmp/zep_python-2.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-2.0.0rc5.tar", max compression
+gzip compressed data, was "zep_python-2.0.0rc6.tar", max compression
```

## Comparing `zep_python-2.0.0rc5.tar` & `zep_python-2.0.0rc6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-03-20 20:55:29.147904 zep_python-2.0.0rc5/LICENSE
--rw-r--r--   0        0        0     4123 2024-03-20 20:55:29.147904 zep_python-2.0.0rc5/README.md
--rw-r--r--   0        0        0      962 2024-03-20 20:55:29.155904 zep_python-2.0.0rc5/pyproject.toml
--rw-r--r--   0        0        0      195 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/__init__.py
--rw-r--r--   0        0        0      168 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/document/__init__.py
--rw-r--r--   0        0        0    12449 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/document/client.py
--rw-r--r--   0        0        0    19391 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/document/collections.py
--rw-r--r--   0        0        0     4440 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/document/models.py
--rw-r--r--   0        0        0     2658 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/exceptions.py
--rw-r--r--   0        0        0      189 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/langchain/__init__.py
--rw-r--r--   0        0        0     6534 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/langchain/history.py
--rw-r--r--   0        0        0    19401 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/langchain/vectorstore.py
--rw-r--r--   0        0        0      268 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/memory/__init__.py
--rw-r--r--   0        0        0    30120 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/memory/client.py
--rw-r--r--   0        0        0     7171 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/memory/models.py
--rw-r--r--   0        0        0       85 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/message/__init__.py
--rw-r--r--   0        0        0     8998 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/message/client.py
--rw-r--r--   0        0        0     2725 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/message/models.py
--rw-r--r--   0        0        0        0 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/py.typed
--rw-r--r--   0        0        0      157 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/user/__init__.py
--rw-r--r--   0        0        0    13681 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/user/client.py
--rw-r--r--   0        0        0     2793 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/user/models.py
--rw-r--r--   0        0        0      474 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/utils.py
--rw-r--r--   0        0        0     7163 2024-03-20 20:55:29.159904 zep_python-2.0.0rc5/zep_python/zep_client.py
--rw-r--r--   0        0        0     4729 1970-01-01 00:00:00.000000 zep_python-2.0.0rc5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-29 18:28:40.236403 zep_python-2.0.0rc6/LICENSE
+-rw-r--r--   0        0        0     5367 2024-04-29 18:28:40.236403 zep_python-2.0.0rc6/README.md
+-rw-r--r--   0        0        0      962 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/__init__.py
+-rw-r--r--   0        0        0      168 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/document/__init__.py
+-rw-r--r--   0        0        0    12669 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/document/client.py
+-rw-r--r--   0        0        0    19711 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/document/collections.py
+-rw-r--r--   0        0        0     4440 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/document/models.py
+-rw-r--r--   0        0        0     2658 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/exceptions.py
+-rw-r--r--   0        0        0      189 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/langchain/__init__.py
+-rw-r--r--   0        0        0     6813 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/langchain/history.py
+-rw-r--r--   0        0        0    19401 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/langchain/vectorstore.py
+-rw-r--r--   0        0        0      268 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/memory/__init__.py
+-rw-r--r--   0        0        0    30746 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/memory/client.py
+-rw-r--r--   0        0        0     7331 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/memory/models.py
+-rw-r--r--   0        0        0       85 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/message/__init__.py
+-rw-r--r--   0        0        0     9651 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/message/client.py
+-rw-r--r--   0        0        0     2803 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/message/models.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/py.typed
+-rw-r--r--   0        0        0      157 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/user/__init__.py
+-rw-r--r--   0        0        0    14021 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/user/client.py
+-rw-r--r--   0        0        0     2793 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/user/models.py
+-rw-r--r--   0        0        0      474 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/utils.py
+-rw-r--r--   0        0        0     7163 2024-04-29 18:28:40.248403 zep_python-2.0.0rc6/zep_python/zep_client.py
+-rw-r--r--   0        0        0     5973 1970-01-01 00:00:00.000000 zep_python-2.0.0rc6/PKG-INFO
```

### Comparing `zep_python-2.0.0rc5/LICENSE` & `zep_python-2.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-2.0.0rc5/README.md` & `zep_python-2.0.0rc6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,53 @@
-[![Tests](https://github.com/getzep/zep-python/actions/workflows/test.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/test.yml) [![lint](https://github.com/getzep/zep-python/actions/workflows/lint.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/lint.yml) [![Release to PyPI](https://github.com/getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/release.yml) ![GitHub](https://img.shields.io/github/license/getzep/zep-python?color=blue)
 
+[![Tests](https://github.com/getzep/zep-python/actions/workflows/test.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/test.yml) [![lint](https://github.com/getzep/zep-python/actions/workflows/lint.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/lint.yml) [![Release to PyPI](https://github.com/getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/release.yml) ![GitHub](https://img.shields.io/github/license/getzep/zep-python?color=blue)
 
 <p align="center">
-  <a href="https://squidfunk.github.io/mkdocs-material/">
-    <img src="https://github.com/getzep/zep/blob/main/assets/zep-bot-square-200x200.png?raw=true" width="150" alt="Zep Logo">
+  <a href="https://www.getzep.com/">
+    <img src="https://raw.githubusercontent.com/getzep/zep/main/assets/zep-logo-icon-gradient-rgb.svg" width="150" alt="Zep Logo">
   </a>
 </p>
 
 <h1 align="center">
-Zep: Fast, scalable building blocks for LLM apps
+Zep: Long-Term Memory for ‍AI Assistants.
 </h1>
-<h2 align="center">Chat history memory, embedding, vector search, data enrichment, and more.</h2>
+<h2 align="center">Recall, understand, and extract data from chat histories. Power personalized AI experiences.</h2>
+<br />
 
 <p align="center">
 <a href="https://docs.getzep.com/deployment/quickstart/">Quick Start</a> | 
 <a href="https://docs.getzep.com/">Documentation</a> | 
 <a href="https://docs.getzep.com/sdk/langchain/">LangChain</a> and 
 <a href="https://docs.getzep.com/sdk/langchain/">LlamaIndex</a> Support | 
 <a href="https://discord.gg/W8Kw6bsgXQ">Discord</a><br />
 <a href="https://www.getzep.com">www.getzep.com</a>
 </p>
 
-## What is Zep?
-Zep is an open source platform for productionizing LLM apps. Zep summarizes, embeds, and enriches chat histories and documents asynchronously, ensuring these operations don't impact your user's chat experience. Data is persisted to database, allowing you to scale out when growth demands. As drop-in replacements for popular LangChain components, you can get to production in minutes without rewriting code.
+## What is Zep? 💬 
+Zep is a long-term memory service for AI Assistant apps. With Zep, you can provide AI assistants with the ability to recall past conversations, no matter how distant, while also reducing hallucinations, latency, and cost. 
+
+### How Zep works
+
+Zep does all of this asynchronously, ensuring these operations don't impact your user's chat experience. Data is persisted to database, allowing you to scale out when growth demands.
+
+Zep also provides a simple, easy to use abstraction for document vector search called Document Collections. This is designed to complement Zep's core memory features, but is not designed to be a general purpose vector database.
+
+Zep allows you to be more intentional about constructing your prompt: 
+1. automatically adding a few recent messages, with the number customized for your app;
+2. a summary of recent conversations prior to the messages above;
+3. and/or contextually relevant summaries or messages surfaced from the entire chat session.
+4. and/or relevant Business data from Zep Document Collections.
+
+## What is Zep Cloud? ⚡️ 
+
+[Zep Cloud](https://www.getzep.com/) is a managed service with Zep Open Source at its core. In addition to Zep Open Source's memory management features, Zep Cloud offers:
+- **Fact Extraction:** Automatically build fact tables from conversations, without having to define a data schema upfront.
+- **Dialog Classification:** Instantly and accurately classify chat dialog. Understand user intent and emotion, segment users, and more. Route chains based on semantic context, and trigger events. 
+- **Structured Data Extraction:** Quickly extract business data from chat conversations using a schema you define. Understand what your Assistant should ask for next in order to complete its task.
 
-[![Zep Demo Video](https://img.youtube.com/vi/d6ryNEvMXno/maxresdefault.jpg)](https://vimeo.com/865785086?share=copy)
 
 ## Zep Python Client
 
 This is the Python client package for the Zep service. For more information about Zep, see https://github.com/getzep/zep.
 
 Zep QuickStart Guide: https://docs.getzep.com/deployment/quickstart
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -3,47 +3,65 @@
 [lint](https://github.com/getzep/zep-python/actions/workflows/lint.yml/
 badge.svg)](https://github.com/getzep/zep-python/actions/workflows/lint.yml) [!
 [Release to PyPI](https://github.com/getzep/zep-python/actions/workflows/
 release.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/
 release.yml) ![GitHub](https://img.shields.io/github/license/getzep/zep-
 python?color=blue)
                                   _[_Z_e_p_ _L_o_g_o_]
-        ************ ZZeepp:: FFaasstt,, ssccaallaabbllee bbuuiillddiinngg bblloocckkss ffoorr LLLLMM aappppss ************
-********** CChhaatt hhiissttoorryy mmeemmoorryy,, eemmbbeeddddiinngg,, vveeccttoorr sseeaarrcchh,, ddaattaa eennrriicchhmmeenntt,, aanndd mmoorree..
-                                     **********
+           ************ ZZeepp:: LLoonngg--TTeerrmm MMeemmoorryy ffoorr ?â??AAII AAssssiissttaannttss.. ************
+     ********** RReeccaallll,, uunnddeerrssttaanndd,, aanndd eexxttrraacctt ddaattaa ffrroomm cchhaatt hhiissttoorriieess.. PPoowweerr
+                      ppeerrssoonnaalliizzeedd AAII eexxppeerriieenncceess.. **********
+
    _Q_u_i_c_k_ _S_t_a_r_t | _D_o_c_u_m_e_n_t_a_t_i_o_n | _L_a_n_g_C_h_a_i_n and _L_l_a_m_a_I_n_d_e_x Support | _D_i_s_c_o_r_d
                                 _w_w_w_._g_e_t_z_e_p_._c_o_m
-## What is Zep? Zep is an open source platform for productionizing LLM apps.
-Zep summarizes, embeds, and enriches chat histories and documents
-asynchronously, ensuring these operations don't impact your user's chat
-experience. Data is persisted to database, allowing you to scale out when
-growth demands. As drop-in replacements for popular LangChain components, you
-can get to production in minutes without rewriting code. [![Zep Demo Video]
-(https://img.youtube.com/vi/d6ryNEvMXno/maxresdefault.jpg)](https://vimeo.com/
-865785086?share=copy) ## Zep Python Client This is the Python client package
-for the Zep service. For more information about Zep, see https://github.com/
-getzep/zep. Zep QuickStart Guide: https://docs.getzep.com/deployment/quickstart
-Zep Documentation: [https://docs.getzep.com](https://docs.getzep.com/) ##
-Installation ```bash pip install zep-python ``` -- OR -- ```bash poetry add
-zep-python ``` ## Zep Cloud Installation In order to install Zep Python SDK
-with Zep Cloud support, you will need to install a release candidate version.
-```bash pip install --pre zep-python ``` -- OR -- ```bash poetry add zep-
-python@^2.0.0rc ``` You will also need to provide a Zep Project API key to your
-zep client for cloud support. You can find out about Zep Projects in our [cloud
-docs](https://help.getzep.com/projects.html) ### Using LangChain Zep Classes
-with `zep-python` (Currently only available on release candidate versions) In
-the pre-release version `zep-python` sdk comes with `ZepChatMessageHistory` and
-`ZepVectorStore` classes that are compatible with [LangChain's Python
-expression language](https://python.langchain.com/docs/expression_language/) In
-order to use these classes in your application, you need to make sure that you
-have `langchain_core` package installed, please refer to [Langchain's docs
-installation section](https://python.langchain.com/docs/get_started/
-installation#langchain-core). We support `langchain_core@>=0.1.3<0.2.0` You can
-import these classes in the following way: ```python from zep_python.langchain
-import ZepChatMessageHistory, ZepVectorStore ``` ### Running Examples You will
-need to set the following environment variables to run examples in the
-`examples` directory: ```dotenv # Please use examples/.env.example as a
-template for .env file # Required ZEP_API_KEY=# Your Zep Project API Key
-ZEP_COLLECTION=# used in ingestion script and in vector store examples
-OPENAI_API_KEY=# Your OpenAI API Key # Optional (If you want to use langsmith
-with LangServe Sample App) LANGCHAIN_TRACING_V2=true LANGCHAIN_API_KEY=
-LANGCHAIN_PROJECT=# If not specified, defaults to "default" ```
+## What is Zep? ð¬ Zep is a long-term memory service for AI Assistant apps.
+With Zep, you can provide AI assistants with the ability to recall past
+conversations, no matter how distant, while also reducing hallucinations,
+latency, and cost. ### How Zep works Zep does all of this asynchronously,
+ensuring these operations don't impact your user's chat experience. Data is
+persisted to database, allowing you to scale out when growth demands. Zep also
+provides a simple, easy to use abstraction for document vector search called
+Document Collections. This is designed to complement Zep's core memory
+features, but is not designed to be a general purpose vector database. Zep
+allows you to be more intentional about constructing your prompt: 1.
+automatically adding a few recent messages, with the number customized for your
+app; 2. a summary of recent conversations prior to the messages above; 3. and/
+or contextually relevant summaries or messages surfaced from the entire chat
+session. 4. and/or relevant Business data from Zep Document Collections. ##
+What is Zep Cloud? â¡ï¸ [Zep Cloud](https://www.getzep.com/) is a managed
+service with Zep Open Source at its core. In addition to Zep Open Source's
+memory management features, Zep Cloud offers: - **Fact Extraction:**
+Automatically build fact tables from conversations, without having to define a
+data schema upfront. - **Dialog Classification:** Instantly and accurately
+classify chat dialog. Understand user intent and emotion, segment users, and
+more. Route chains based on semantic context, and trigger events. -
+**Structured Data Extraction:** Quickly extract business data from chat
+conversations using a schema you define. Understand what your Assistant should
+ask for next in order to complete its task. ## Zep Python Client This is the
+Python client package for the Zep service. For more information about Zep, see
+https://github.com/getzep/zep. Zep QuickStart Guide: https://docs.getzep.com/
+deployment/quickstart Zep Documentation: [https://docs.getzep.com](https://
+docs.getzep.com/) ## Installation ```bash pip install zep-python ``` -- OR -
+- ```bash poetry add zep-python ``` ## Zep Cloud Installation In order to
+install Zep Python SDK with Zep Cloud support, you will need to install a
+release candidate version. ```bash pip install --pre zep-python ``` -- OR -
+- ```bash poetry add zep-python@^2.0.0rc ``` You will also need to provide a
+Zep Project API key to your zep client for cloud support. You can find out
+about Zep Projects in our [cloud docs](https://help.getzep.com/projects.html)
+### Using LangChain Zep Classes with `zep-python` (Currently only available on
+release candidate versions) In the pre-release version `zep-python` sdk comes
+with `ZepChatMessageHistory` and `ZepVectorStore` classes that are compatible
+with [LangChain's Python expression language](https://python.langchain.com/
+docs/expression_language/) In order to use these classes in your application,
+you need to make sure that you have `langchain_core` package installed, please
+refer to [Langchain's docs installation section](https://python.langchain.com/
+docs/get_started/installation#langchain-core). We support
+`langchain_core@>=0.1.3<0.2.0` You can import these classes in the following
+way: ```python from zep_python.langchain import ZepChatMessageHistory,
+ZepVectorStore ``` ### Running Examples You will need to set the following
+environment variables to run examples in the `examples` directory: ```dotenv #
+Please use examples/.env.example as a template for .env file # Required
+ZEP_API_KEY=# Your Zep Project API Key ZEP_COLLECTION=# used in ingestion
+script and in vector store examples OPENAI_API_KEY=# Your OpenAI API Key #
+Optional (If you want to use langsmith with LangServe Sample App)
+LANGCHAIN_TRACING_V2=true LANGCHAIN_API_KEY= LANGCHAIN_PROJECT=# If not
+specified, defaults to "default" ```
```

### Comparing `zep_python-2.0.0rc5/pyproject.toml` & `zep_python-2.0.0rc6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zep-python"
-version = "2.0.0-rc.5"
+version = "2.0.0-rc.6"
 description = "Long-Term Memory for AI Assistants. This is the Python client for the Zep service."
 authors = ["Daniel Chalef <daniel.chalef@private.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9.0,<4"
 httpx = ">=0.24.0,<0.29.0"
```

### Comparing `zep_python-2.0.0rc5/zep_python/document/client.py` & `zep_python-2.0.0rc6/zep_python/document/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import urllib.parse
 from typing import Any, Dict, List, Optional
 
 import httpx
 
 from zep_python.exceptions import handle_response
 from zep_python.utils import filter_dict
 
@@ -101,15 +102,15 @@
             description=description,
             embedding_dimensions=DEFAULT_EMBEDDING_DIMENSIONS,
             metadata=metadata,
             is_auto_embedded=True,
         )
 
         response = await self.aclient.post(
-            f"/collections/{name}",
+            f"/collections/{urllib.parse.quote_plus(name)}",
             json=collection.model_dump(exclude_none=True, exclude_unset=True),
         )
 
         handle_response(response)
 
         return await self.aget_collection(collection.name)
 
@@ -150,15 +151,15 @@
             description=description,
             embedding_dimensions=DEFAULT_EMBEDDING_DIMENSIONS,
             metadata=metadata,
             is_auto_embedded=True,
         )
 
         response = self.client.post(
-            f"/collections/{name}",
+            f"/collections/{urllib.parse.quote_plus(name)}",
             json=collection.model_dump(exclude_none=True, exclude_unset=True),
         )
 
         handle_response(response)
 
         return self.get_collection(collection.name)
 
@@ -187,15 +188,15 @@
             If API response is unexpected.
         AuthError
             If the API key is invalid.
         """
         if name is None or name.strip() == "":
             raise ValueError("collection name must be provided")
         response = await self.aclient.get(
-            f"/collections/{name}",
+            f"/collections/{urllib.parse.quote_plus(name)}",
         )
 
         handle_response(response)
 
         filtered_response = filter_dict(response.json())
 
         return DocumentCollection(
@@ -226,15 +227,15 @@
             If API response is unexpected.
         AuthError
             If the API key is invalid.
         """
         if name is None or name.strip() == "":
             raise ValueError("collection name must be provided")
         response = self.client.get(
-            f"/collections/{name}",
+            f"/collections/{urllib.parse.quote_plus(name)}",
         )
 
         handle_response(response)
 
         filtered_response = filter_dict(response.json())
 
         return DocumentCollection(
@@ -277,15 +278,15 @@
         collection = DocumentCollection(
             name=name,
             description=description,
             metadata=metadata,
         )
 
         response = await self.aclient.patch(
-            f"/collections/{collection.name}",
+            f"/collections/{urllib.parse.quote_plus(collection.name)}",
             json=collection.model_dump(exclude_none=True, exclude_unset=True),
         )
 
         handle_response(response)
 
         return await self.aget_collection(collection.name)
 
@@ -325,15 +326,15 @@
         collection = DocumentCollection(
             name=name,
             description=description,
             metadata=metadata,
         )
 
         response = self.client.patch(
-            f"/collections/{collection.name}",
+            f"/collections/{urllib.parse.quote_plus(collection.name)}",
             json=collection.model_dump(exclude_none=True, exclude_unset=True),
         )
 
         handle_response(response)
 
         return self.get_collection(collection.name)
 
@@ -405,15 +406,15 @@
         AuthError
             If the API key is invalid.
         """
         if collection_name is None or collection_name.strip() == "":
             raise ValueError("collection name must be provided")
 
         response = await self.aclient.delete(
-            f"/collections/{collection_name}",
+            f"/collections/{urllib.parse.quote_plus(collection_name)}",
         )
 
         handle_response(response)
 
     def delete_collection(self, collection_name: str) -> None:
         """
         Deletes a collection.
@@ -436,11 +437,11 @@
         AuthError
             If the API key is invalid.
         """
         if collection_name is None or collection_name.strip() == "":
             raise ValueError("collection name must be provided")
 
         response = self.client.delete(
-            f"/collections/{collection_name}",
+            f"/collections/{urllib.parse.quote_plus(collection_name)}",
         )
 
         handle_response(response)
```

### Comparing `zep_python-2.0.0rc5/zep_python/document/collections.py` & `zep_python-2.0.0rc6/zep_python/document/collections.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import urllib.parse
 import warnings
 from typing import Any, Dict, Generator, List, Optional, Tuple
 
 import httpx
 from pydantic import PrivateAttr
 
 from zep_python.exceptions import handle_response
@@ -106,15 +107,15 @@
 
         if documents is None:
             raise ValueError("document list must be provided")
 
         uuids: List[str] = []
         for batch in generate_batches(documents, batch_size):
             response = await self._aclient.post(
-                f"/collections/{self.name}/documents",
+                f"/collections/{urllib.parse.quote_plus(self.name)}/documents",
                 json=batch,
             )
 
             handle_response(response)
 
             uuids.extend(response.json())
 
@@ -151,15 +152,15 @@
 
         if documents is None:
             raise ValueError("document list must be provided")
 
         uuids: List[str] = []
         for batch in generate_batches(documents, batch_size):
             response = self._client.post(
-                f"/collections/{self.name}/documents",
+                f"/collections/{urllib.parse.quote_plus(self.name)}/documents",
                 json=batch,
             )
 
             handle_response(response)
 
             uuids.extend(response.json())
 
@@ -206,15 +207,15 @@
 
         if document_id is None and metadata is None:
             raise ValueError("document_id or metadata must be provided")
 
         payload = filter_dict({"document_id": document_id, "metadata": metadata})
 
         response = await self._aclient.patch(
-            f"/collections/{self.name}/documents/uuid/{uuid}",
+            f"/collections/{urllib.parse.quote_plus(self.name)}/documents/uuid/{uuid}",
             json=payload,
         )
 
         handle_response(response)
 
     def update_document(
         self,
@@ -257,15 +258,15 @@
 
         if document_id is None and metadata is None:
             raise ValueError("document_id or metadata must be provided")
 
         payload = filter_dict({"document_id": document_id, "metadata": metadata})
 
         response = self._client.patch(
-            f"/collections/{self.name}/documents/uuid/{uuid}",
+            f"/collections/{urllib.parse.quote_plus(self.name)}/documents/uuid/{uuid}",
             json=payload,
         )
 
         handle_response(response)
 
     async def adelete_document(self, uuid: str) -> None:
         """
@@ -293,15 +294,15 @@
                 "Can only delete a document once a collection has been retrieved"
             )
 
         if uuid is None or uuid.strip() == "":
             raise ValueError("document uuid must be provided")
 
         response = await self._aclient.delete(
-            f"/collections/{self.name}/documents/uuid/{uuid}",
+            f"/collections/{urllib.parse.quote_plus(self.name)}/documents/uuid/{uuid}",
         )
 
         handle_response(response)
 
     def delete_document(self, uuid: str) -> None:
         """
         Delete document.
@@ -328,15 +329,15 @@
                 "Can only delete a document once a collection has been retrieved"
             )
 
         if uuid is None or uuid.strip() == "":
             raise ValueError("document uuid must be provided")
 
         response = self._client.delete(
-            f"/collections/{self.name}/documents/uuid/{uuid}",
+            f"/collections/{urllib.parse.quote_plus(self.name)}/documents/uuid/{uuid}",
         )
 
         handle_response(response)
 
     async def aget_document(self, uuid: str) -> Document:
         """
         Asynchronously gets a document.
@@ -364,15 +365,15 @@
                 "Can only get a document once a collection has been retrieved"
             )
 
         if uuid is None or uuid.strip() == "":
             raise ValueError("document uuid must be provided")
 
         response = await self._aclient.get(
-            f"/collections/{self.name}/documents/uuid/{uuid}",
+            f"/collections/{urllib.parse.quote_plus(self.name)}/documents/uuid/{uuid}",
         )
 
         handle_response(response)
 
         return Document(**response.json())
 
     def get_document(self, uuid: str) -> Document:
@@ -402,15 +403,15 @@
                 "Can only get a document once a collection has been retrieved"
             )
 
         if uuid is None or uuid.strip() == "":
             raise ValueError("document uuid must be provided")
 
         response = self._client.get(
-            f"/collections/{self.name}/documents/uuid/{uuid}",
+            f"/collections/{urllib.parse.quote_plus(self.name)}/documents/uuid/{uuid}",
         )
 
         handle_response(response)
 
         return Document(**response.json())
 
     async def aget_documents(self, uuids: List[str]) -> List[Document]:
@@ -440,15 +441,15 @@
         if not uuids or len(uuids) == 0:
             raise ValueError("document uuids must be provided")
 
         if len(uuids) > LARGE_BATCH_WARNING_LIMIT:
             warnings.warn(LARGE_BATCH_WARNING, stacklevel=2)
 
         response = await self._aclient.post(
-            f"/collections/{self.name}/documents/list/get",
+            f"/collections/{urllib.parse.quote_plus(self.name)}/documents/list/get",
             json={"uuids": uuids},
         )
 
         handle_response(response)
 
         return [Document(**document) for document in response.json()]
 
@@ -479,15 +480,15 @@
         if not uuids or len(uuids) == 0:
             raise ValueError("document uuids must be provided")
 
         if len(uuids) > LARGE_BATCH_WARNING_LIMIT:
             warnings.warn(LARGE_BATCH_WARNING, stacklevel=2)
 
         response = self._client.post(
-            f"/collections/{self.name}/documents/list/get",
+            f"/collections/{urllib.parse.quote_plus(self.name)}/documents/list/get",
             json={"uuids": uuids},
         )
 
         handle_response(response)
 
         return [Document(**document) for document in response.json()]
 
@@ -515,15 +516,15 @@
         payload = DocumentSearchPayload(
             text=text,
             metadata=metadata,
             search_type=search_type_value,
             mmr_lambda=mmr_lambda,
         )
 
-        url = f"/collections/{self.name}/search"
+        url = f"/collections/{urllib.parse.quote_plus(self.name)}/search"
         params = {"limit": limit} if limit is not None and limit > 0 else {}
 
         response = await self._aclient.post(
             url,
             params=params,
             json=payload.model_dump(exclude_none=True, exclude_unset=True),
         )
@@ -613,15 +614,15 @@
         payload = DocumentSearchPayload(
             text=text,
             metadata=metadata,
             search_type=search_type_value,
             mmr_lambda=mmr_lambda,
         )
 
-        url = f"/collections/{self.name}/search"
+        url = f"/collections/{urllib.parse.quote_plus(self.name)}/search"
         params = {"limit": limit} if limit is not None and limit > 0 else {}
 
         response = self._client.post(
             url,
             params=params,
             json=payload.model_dump(exclude_none=True, exclude_unset=True),
         )
```

### Comparing `zep_python-2.0.0rc5/zep_python/document/models.py` & `zep_python-2.0.0rc6/zep_python/document/models.py`

 * *Files identical despite different names*

### Comparing `zep_python-2.0.0rc5/zep_python/exceptions.py` & `zep_python-2.0.0rc6/zep_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `zep_python-2.0.0rc5/zep_python/langchain/history.py` & `zep_python-2.0.0rc6/zep_python/langchain/history.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,36 +38,40 @@
     api_url : str
         The Zep API service URL. Not required if using Zep Cloud.
     api_key : str
         The Zep API key. Not required if using Zep Open Source.
     memory_type : str
         The type of memory to use. Can be "perpetual", "summary_retrieval",
         or "message_window". Defaults to "perpetual".
+    summary_instruction : Optional[str]
+        Additional instructions for generating dialog summaries.
     """
 
     def __init__(
         self,
         session_id: str,
         zep_client: Optional[ZepClient] = None,
         api_url: Optional[str] = API_URL,
         api_key: Optional[str] = None,
         memory_type: Optional[str] = None,
         ai_prefix: Optional[str] = None,
         human_prefix: Optional[str] = None,
+        summary_instruction: Optional[str] = None,
     ) -> None:
         if zep_client is None:
             self._client = ZepClient(api_url=api_url, api_key=api_key)
         else:
             self._client = zep_client
 
         self.session_id = session_id
         self.memory_type = memory_type or "perpetual"
 
         self.ai_prefix = ai_prefix or "ai"
         self.human_prefix = human_prefix or "human"
+        self.summary_instruction = summary_instruction
 
     @property
     def messages(self) -> List[BaseMessage]:  # type: ignore
         """Retrieve messages from Zep memory"""
 
         zep_memory: Optional[Memory] = self._get_memory()
         if not zep_memory:
@@ -173,15 +177,17 @@
         zep_message = Message(
             content=message.content,
             # If name is not set, use type as role
             role=message.name or message.type,
             role_type=get_zep_message_role_type(message.type),
             metadata=metadata,
         )
-        zep_memory = Memory(messages=[zep_message])
+        zep_memory = Memory(
+            messages=[zep_message], summary_instruction=self.summary_instruction
+        )
 
         self._client.memory.add_memory(self.session_id, zep_memory)
 
     def clear(self) -> None:
         """Clear session memory from Zep. Note that Zep is long-term storage for memory
         and this is not advised unless you have specific data retention requirements.
         """
```

### Comparing `zep_python-2.0.0rc5/zep_python/langchain/vectorstore.py` & `zep_python-2.0.0rc6/zep_python/langchain/vectorstore.py`

 * *Files identical despite different names*

### Comparing `zep_python-2.0.0rc5/zep_python/memory/client.py` & `zep_python-2.0.0rc6/zep_python/memory/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import urllib.parse
 from typing import Any, AsyncGenerator, Dict, Generator, List, Optional
 
 import httpx
 
 from zep_python.exceptions import handle_response
 from zep_python.memory.models import (
     ClassifySessionRequest,
@@ -78,15 +79,15 @@
             If the API response format is unexpected.
         ConnectionError
             If the connection to the server fails.
         """
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
-        url = f"/sessions/{session_id}"
+        url = f"/sessions/{urllib.parse.quote_plus(session_id)}"
 
         try:
             response = self.client.get(url)
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
 
         handle_response(response, f"No session found for session {session_id}")
@@ -120,15 +121,15 @@
             If the API response format is unexpected.
         ConnectionError
             If the connection to the server fails.
         """
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
-        url = f"/sessions/{session_id}"
+        url = f"/sessions/{urllib.parse.quote_plus(session_id)}"
 
         try:
             response = await self.aclient.get(url)
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
 
         handle_response(response, f"No session found for session {session_id}")
@@ -247,15 +248,15 @@
         """
         if session is None:
             raise ValueError("session must be provided")
         if session.session_id is None or session.session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
         response = self.client.patch(
-            f"/sessions/{session.session_id}",
+            f"/sessions/{urllib.parse.quote(session.session_id)}",
             json=session.model_dump(exclude_none=True, exclude_unset=True),
         )
 
         handle_response(response, f"Failed to update session {session.session_id}")
 
         return Session.model_validate(response.json())
 
@@ -285,15 +286,15 @@
         """
         if session is None:
             raise ValueError("session must be provided")
         if session.session_id is None or session.session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
         response = await self.aclient.patch(
-            f"/sessions/{session.session_id}",
+            f"/sessions/{urllib.parse.quote(session.session_id)}",
             json=session.model_dump(exclude_none=True, exclude_unset=True),
         )
 
         handle_response(response, f"Failed to update session {session.session_id}")
 
         return Session.model_validate(response.json())
 
@@ -356,15 +357,15 @@
             classes=classes,
             last_n=last_n,
             persist=persist,
             instruction=instruction,
         )
 
         response = await self.aclient.post(
-            f"/sessions/{session_id}/classify",
+            f"/sessions/{urllib.parse.quote_plus(session_id)}/classify",
             json=request.model_dump(exclude_none=True, exclude_unset=True),
         )
         handle_response(response)
 
         return ClassifySessionResponse(**response.json())
 
     def classify_session(
@@ -426,15 +427,15 @@
             classes=classes,
             last_n=last_n,
             persist=persist,
             instruction=instruction,
         )
 
         response = self.client.post(
-            f"/sessions/{session_id}/classify",
+            f"/sessions/{urllib.parse.quote_plus(session_id)}/classify",
             json=request.model_dump(exclude_none=True, exclude_unset=True),
         )
         handle_response(response)
 
         return ClassifySessionResponse(**response.json())
 
     # Memory APIs : Get a List of Sessions
@@ -633,16 +634,16 @@
         APIError
             If the API response format is unexpected.
         """
 
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
-        url = f"/sessions/{session_id}/memory"
-        params = self._gen_get_params(lastn, memory_type)
+        url = f"/sessions/{urllib.parse.quote_plus(session_id)}/memory"
+        params = self._gen_get_params(lastn, memory_type or MemoryType.perpetual.value)
         response = self.client.get(url, params=params)
 
         handle_response(response, f"No memory found for session {session_id}")
 
         response_data = response.json()
 
         return Memory.model_validate(response_data)
@@ -679,16 +680,16 @@
             If the session ID is None or empty.
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
-        url = f"/sessions/{session_id}/memory"
-        params = self._gen_get_params(lastn, memory_type)
+        url = f"/sessions/{urllib.parse.quote_plus(session_id)}/memory"
+        params = self._gen_get_params(lastn, memory_type or MemoryType.perpetual.value)
         response = await self.aclient.get(url, params=params)
 
         handle_response(response, f"No memory found for session {session_id}")
 
         response_data = response.json()
 
         return Memory.model_validate(response_data)
@@ -717,15 +718,15 @@
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
         response = self.client.post(
-            f"/sessions/{session_id}/memory",
+            f"/sessions/{urllib.parse.quote_plus(session_id)}/memory",
             json=memory_messages.model_dump(exclude_none=True, exclude_unset=True),
         )
 
         handle_response(response)
 
         return response.text
 
@@ -753,15 +754,15 @@
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
         response = await self.aclient.post(
-            f"/sessions/{session_id}/memory",
+            f"/sessions/{urllib.parse.quote_plus(session_id)}/memory",
             json=memory_messages.model_dump(exclude_none=True, exclude_unset=True),
         )
 
         handle_response(response)
 
         return response.text
 
@@ -786,15 +787,17 @@
             If the session ID is None or empty.
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
-        response = self.client.delete(f"/sessions/{session_id}/memory")
+        response = self.client.delete(
+            f"/sessions/{urllib.parse.quote_plus(session_id)}/memory"
+        )
         handle_response(response)
         return response.text
 
     # Memory APIs : Delete Memory Asynchronously
     async def adelete_memory(self, session_id: str) -> str:
         """
         Asynchronously delete memory for the specified session.
@@ -815,15 +818,17 @@
             If the session ID is None or empty.
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
-        response = await self.aclient.delete(f"/sessions/{session_id}/memory")
+        response = await self.aclient.delete(
+            f"/sessions/{urllib.parse.quote_plus(session_id)}/memory"
+        )
         handle_response(response)
         return response.text
 
     def _validate_search_payload(self, search_payload: MemorySearchPayload) -> None:
         if search_payload is None:
             raise ValueError("search_payload must be provided")
 
@@ -867,15 +872,15 @@
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
         self._validate_search_payload(search_payload)
 
         params = {"limit": limit} if limit is not None else {}
         response = self.client.post(
-            f"/sessions/{session_id}/search",
+            f"/sessions/{urllib.parse.quote_plus(session_id)}/search",
             json=search_payload.model_dump(exclude_unset=True, exclude_none=True),
             params=params,
         )
         handle_response(response)
         return [
             MemorySearchResult(**search_result) for search_result in response.json()
         ]
@@ -914,15 +919,15 @@
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
         self._validate_search_payload(search_payload)
 
         params = {"limit": limit} if limit is not None else {}
         response = await self.aclient.post(
-            f"/sessions/{session_id}/search",
+            f"/sessions/{urllib.parse.quote_plus(session_id)}/search",
             json=search_payload.model_dump(exclude_unset=True, exclude_none=True),
             params=params,
         )
         handle_response(response)
         return [
             MemorySearchResult(**search_result) for search_result in response.json()
         ]
@@ -948,16 +953,18 @@
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
         params = {"lastNMessages": last_n}
+        print(f"/sessions/{urllib.parse.quote_plus(session_id)}/synthesize_question")
         response = self.client.get(
-            f"/sessions/{session_id}/synthesize_question", params=params
+            f"/sessions/{urllib.parse.quote_plus(session_id)}/synthesize_question",
+            params=params,
         )
 
         handle_response(response)
 
         question = Question(**response.json())
 
         return question.question
@@ -984,15 +991,16 @@
             If the API response format is unexpected.
         """
         if session_id is None or session_id.strip() == "":
             raise ValueError("session_id must be provided")
 
         params = {"lastNMessages": last_n}
         response = await self.aclient.get(
-            f"/sessions/{session_id}/synthesize_question", params=params
+            f"/sessions/{urllib.parse.quote_plus(session_id)}/synthesize_question",
+            params=params,
         )
 
         handle_response(response)
 
         question = Question(**response.json())
 
         return question.question
```

### Comparing `zep_python-2.0.0rc5/zep_python/memory/models.py` & `zep_python-2.0.0rc6/zep_python/memory/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,16 @@
     created_at : Optional[str]
         The timestamp when the memory was created.
     token_count : Optional[int]
         The token count of the memory.
     facts : Optional[List[str]]
         Most recent list of facts derived from the session. Included only with
         perpetual memory type.
+    summary_instruction : Optional[str]
+        Additional instruction for generating the summary.
 
     Methods
     -------
     to_dict() -> Dict[str, Any]:
         Returns a dictionary representation of the message.
     """
 
@@ -132,14 +134,15 @@
     )
     metadata: Optional[Dict[str, Any]] = Field(default=None)
     summary: Optional[Summary] = Field(default=None)
     uuid: Optional[str] = Field(default=None)
     created_at: Optional[str] = Field(default=None)
     token_count: Optional[int] = Field(default=None)
     facts: Optional[List[str]] = Field(default=None)
+    summary_instruction: Optional[str] = Field(default=None)
 
     def to_dict(self) -> Dict[str, Any]:
         return self.model_dump(exclude_unset=True, exclude_none=True)
 
 
 class MemorySearchPayload(BaseModel):
     """
```

### Comparing `zep_python-2.0.0rc5/zep_python/message/client.py` & `zep_python-2.0.0rc6/zep_python/message/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import urllib.parse
 from typing import Any, Dict, List, Optional
 
 import httpx
 
 from zep_python.exceptions import handle_response
 
 from .models import Message
@@ -93,15 +94,15 @@
         """
 
         if session_id is None or session_id.strip() == "":
             raise ValueError("Session ID cannot be empty.")
 
         params = self._validate_cursor_limit(limit, cursor)
 
-        url = f"/sessions/{session_id}/messages"
+        url = f"/sessions/{urllib.parse.quote_plus(session_id)}/messages"
 
         try:
             response = self.client.get(url=url, params=params)
         except httpx.NetworkError:
             raise ConnectionError("Unable to connect to server.")
 
         handle_response(response, f"Unable to get messages for session {session_id}.")
@@ -143,15 +144,15 @@
         """
 
         if session_id is None or session_id.strip() == "":
             raise ValueError("Session ID cannot be empty.")
 
         params = self._validate_cursor_limit(limit, cursor)
 
-        url = f"/sessions/{session_id}/messages"
+        url = f"/sessions/{urllib.parse.quote_plus(session_id)}/messages"
 
         try:
             response = await self.aclient.get(url=url, params=params)
         except httpx.NetworkError:
             raise ConnectionError("Unable to connect to server.")
 
         handle_response(response, f"Unable to get messages for session {session_id}.")
@@ -178,16 +179,17 @@
         """
 
         if session_id is None or session_id.strip() == "":
             raise ValueError("Session ID cannot be empty.")
 
         if message_id is None or message_id.strip() == "":
             raise ValueError("Message ID cannot be empty.")
-
-        url = f"/sessions/{session_id}/messages/{message_id}"
+        encoded_message_id = urllib.parse.quote_plus(message_id)
+        encoded_session_id = urllib.parse.quote_plus(session_id)
+        url = f"/sessions/{encoded_session_id}/messages/{encoded_message_id}"
 
         try:
             response = self.client.get(url=url)
         except httpx.NetworkError:
             raise ConnectionError("Unable to connect to server.")
 
         handle_response(
@@ -215,15 +217,17 @@
 
         if session_id is None or session_id.strip() == "":
             raise ValueError("Session ID cannot be empty.")
 
         if message_id is None or message_id.strip() == "":
             raise ValueError("Message ID cannot be empty.")
 
-        url = f"/sessions/{session_id}/messages/{message_id}"
+        encoded_message_id = urllib.parse.quote_plus(message_id)
+        encoded_session_id = urllib.parse.quote_plus(session_id)
+        url = f"/sessions/{encoded_session_id}/messages/{encoded_message_id}"
 
         try:
             response = await self.aclient.get(url=url)
         except httpx.NetworkError:
             raise ConnectionError("Unable to connect to server.")
 
         handle_response(
@@ -255,15 +259,17 @@
 
         if session_id is None or session_id.strip() == "":
             raise ValueError("Session ID cannot be empty.")
 
         if message_id is None or message_id.strip() == "":
             raise ValueError("Message ID cannot be empty.")
 
-        url = f"/sessions/{session_id}/messages/{message_id}"
+        encoded_message_id = urllib.parse.quote_plus(message_id)
+        encoded_session_id = urllib.parse.quote_plus(session_id)
+        url = f"/sessions/{encoded_session_id}/messages/{encoded_message_id}"
 
         try:
             response = self.client.patch(url=url, json=metadata)
         except httpx.NetworkError:
             raise ConnectionError("Unable to connect to server.")
 
         handle_response(
@@ -297,15 +303,17 @@
 
         if session_id is None or session_id.strip() == "":
             raise ValueError("Session ID cannot be empty.")
 
         if message_id is None or message_id.strip() == "":
             raise ValueError("Message ID cannot be empty.")
 
-        url = f"/sessions/{session_id}/messages/{message_id}"
+        encoded_message_id = urllib.parse.quote_plus(message_id)
+        encoded_session_id = urllib.parse.quote_plus(session_id)
+        url = f"/sessions/{encoded_session_id}/messages/{encoded_message_id}"
 
         try:
             response = await self.aclient.patch(url=url, json=metadata)
         except httpx.NetworkError:
             raise ConnectionError("Unable to connect to server.")
 
         handle_response(
```

### Comparing `zep_python-2.0.0rc5/zep_python/message/models.py` & `zep_python-2.0.0rc6/zep_python/message/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,32 @@
 
 class RoleType(str, Enum):
     USER_ROLE = "user"
     ASSISTANT_ROLE = "assistant"
     SYSTEM_ROLE = "system"
     FUNCTION_ROLE = "function"
     TOOL_ROLE = "tool"
+    NO_ROLE = "norole"
 
 
 def get_zep_message_role_type(role):
     if role == "human":
         return RoleType.USER_ROLE
     elif role == "ai":
         return RoleType.ASSISTANT_ROLE
     elif role == "system":
         return RoleType.SYSTEM_ROLE
     elif role == "function":
         return RoleType.FUNCTION_ROLE
     elif role == "tool":
         return RoleType.TOOL_ROLE
+    elif role == "norole":
+        return RoleType.NO_ROLE
     else:
-        return RoleType.SYSTEM_ROLE
+        return RoleType.NO_ROLE
 
 
 class Message(BaseModel):
     """
     Represents a message in a conversation.
 
     Attributes
```

### Comparing `zep_python-2.0.0rc5/zep_python/user/client.py` & `zep_python-2.0.0rc6/zep_python/user/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import urllib.parse
 from typing import AsyncGenerator, Generator, List, Optional
 
 import httpx
 from httpx import AsyncClient, Client
 
 from zep_python.exceptions import handle_response
 
@@ -120,15 +121,15 @@
             If the client fails to connect to the server.
         APIError
             If the server returns an error.
         NotFoundError
             If the user does not exist.
         """
         try:
-            response = self.client.get(f"/users/{user_id}")
+            response = self.client.get(f"/users/{urllib.parse.quote_plus(user_id)}")
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
 
         handle_response(response)
         return User.model_validate(response.json())
 
     async def aget(self, user_id: str) -> User:
@@ -153,15 +154,17 @@
             If the server returns an error.
         NotFoundError
             If the user does not exist.
         """
         if user_id is None:
             raise ValueError("user_id must be provided")
         try:
-            response = await self.aclient.get(f"/users/{user_id}")
+            response = await self.aclient.get(
+                f"/users/{urllib.parse.quote_plus(user_id)}"
+            )
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
 
         handle_response(response)
         return User.model_validate(response.json())
 
     def update(self, user: UpdateUserRequest) -> User:
@@ -188,15 +191,15 @@
             If the user does not exist
         """
         if user.user_id is None:
             raise ValueError("user_id must be provided")
 
         try:
             response = self.client.patch(
-                f"/users/{user.user_id}",
+                f"/users/{urllib.parse.quote_plus(user.user_id)}",
                 json=user.model_dump(exclude_none=True, exclude_unset=True),
             )
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
         handle_response(response)
 
         return User.model_validate(response.json())
@@ -224,15 +227,15 @@
         NotFoundError
             If the user does not exist.
         """
         if user.user_id is None:
             raise ValueError("user_id must be provided")
         try:
             response = await self.aclient.patch(
-                f"/users/{user.user_id}",
+                f"/users/{urllib.parse.quote_plus(user.user_id)}",
                 json=user.model_dump(exclude_none=True, exclude_unset=True),
             )
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
 
         handle_response(response)
 
@@ -257,15 +260,15 @@
             If the client fails to connect to the server.
         APIError
             If the server returns an error.
         NotFoundError
             If the user does not exist.
         """
         try:
-            response = self.client.delete(f"/users/{user_id}")
+            response = self.client.delete(f"/users/{urllib.parse.quote_plus(user_id)}")
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
 
         handle_response(response)
 
     async def adelete(self, user_id: str) -> None:
         """
@@ -286,15 +289,17 @@
             If the client fails to connect to the server.
         APIError
             If the server returns an error.
         NotFoundError
             If the user does not exist.
         """
         try:
-            response = await self.aclient.delete(f"/users/{user_id}")
+            response = await self.aclient.delete(
+                f"/users/{urllib.parse.quote_plus(user_id)}"
+            )
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
 
         handle_response(response)
 
     def list(
         self, limit: Optional[int] = None, cursor: Optional[int] = None
@@ -461,15 +466,17 @@
         ------
         ConnectionError
             If the client fails to connect to the server.
         APIError
             If the server returns an error.
         """
         try:
-            response = self.client.get(f"/users/{user_id}/sessions")
+            response = self.client.get(
+                f"/users/{urllib.parse.quote_plus(user_id)}/sessions"
+            )
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
 
         handle_response(response)
         return [Session.model_validate(session) for session in response.json()]
 
     async def aget_sessions(self, user_id: str) -> List[Session]:
@@ -490,13 +497,15 @@
         ------
         ConnectionError
             If the client fails to connect to the server.
         APIError
             If the server returns an error.
         """
         try:
-            response = await self.aclient.get(f"/users/{user_id}/sessions")
+            response = await self.aclient.get(
+                f"/users/{urllib.parse.quote_plus(user_id)}/sessions"
+            )
         except httpx.NetworkError as e:
             raise ConnectionError("Failed to connect to server") from e
 
         handle_response(response)
         return [Session.model_validate(session) for session in response.json()]
```

### Comparing `zep_python-2.0.0rc5/zep_python/user/models.py` & `zep_python-2.0.0rc6/zep_python/user/models.py`

 * *Files identical despite different names*

### Comparing `zep_python-2.0.0rc5/zep_python/zep_client.py` & `zep_python-2.0.0rc6/zep_python/zep_client.py`

 * *Files identical despite different names*

### Comparing `zep_python-2.0.0rc5/PKG-INFO` & `zep_python-2.0.0rc6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,69 @@
 Metadata-Version: 2.1
 Name: zep-python
-Version: 2.0.0rc5
+Version: 2.0.0rc6
 Summary: Long-Term Memory for AI Assistants. This is the Python client for the Zep service.
 Author: Daniel Chalef
 Author-email: daniel.chalef@private.org
 Requires-Python: >=3.9.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.24.0,<0.29.0)
 Requires-Dist: pydantic (>=2.0.0)
 Description-Content-Type: text/markdown
 
-[![Tests](https://github.com/getzep/zep-python/actions/workflows/test.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/test.yml) [![lint](https://github.com/getzep/zep-python/actions/workflows/lint.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/lint.yml) [![Release to PyPI](https://github.com/getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/release.yml) ![GitHub](https://img.shields.io/github/license/getzep/zep-python?color=blue)
 
+[![Tests](https://github.com/getzep/zep-python/actions/workflows/test.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/test.yml) [![lint](https://github.com/getzep/zep-python/actions/workflows/lint.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/lint.yml) [![Release to PyPI](https://github.com/getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/release.yml) ![GitHub](https://img.shields.io/github/license/getzep/zep-python?color=blue)
 
 <p align="center">
-  <a href="https://squidfunk.github.io/mkdocs-material/">
-    <img src="https://github.com/getzep/zep/blob/main/assets/zep-bot-square-200x200.png?raw=true" width="150" alt="Zep Logo">
+  <a href="https://www.getzep.com/">
+    <img src="https://raw.githubusercontent.com/getzep/zep/main/assets/zep-logo-icon-gradient-rgb.svg" width="150" alt="Zep Logo">
   </a>
 </p>
 
 <h1 align="center">
-Zep: Fast, scalable building blocks for LLM apps
+Zep: Long-Term Memory for ‍AI Assistants.
 </h1>
-<h2 align="center">Chat history memory, embedding, vector search, data enrichment, and more.</h2>
+<h2 align="center">Recall, understand, and extract data from chat histories. Power personalized AI experiences.</h2>
+<br />
 
 <p align="center">
 <a href="https://docs.getzep.com/deployment/quickstart/">Quick Start</a> | 
 <a href="https://docs.getzep.com/">Documentation</a> | 
 <a href="https://docs.getzep.com/sdk/langchain/">LangChain</a> and 
 <a href="https://docs.getzep.com/sdk/langchain/">LlamaIndex</a> Support | 
 <a href="https://discord.gg/W8Kw6bsgXQ">Discord</a><br />
 <a href="https://www.getzep.com">www.getzep.com</a>
 </p>
 
-## What is Zep?
-Zep is an open source platform for productionizing LLM apps. Zep summarizes, embeds, and enriches chat histories and documents asynchronously, ensuring these operations don't impact your user's chat experience. Data is persisted to database, allowing you to scale out when growth demands. As drop-in replacements for popular LangChain components, you can get to production in minutes without rewriting code.
+## What is Zep? 💬 
+Zep is a long-term memory service for AI Assistant apps. With Zep, you can provide AI assistants with the ability to recall past conversations, no matter how distant, while also reducing hallucinations, latency, and cost. 
+
+### How Zep works
+
+Zep does all of this asynchronously, ensuring these operations don't impact your user's chat experience. Data is persisted to database, allowing you to scale out when growth demands.
+
+Zep also provides a simple, easy to use abstraction for document vector search called Document Collections. This is designed to complement Zep's core memory features, but is not designed to be a general purpose vector database.
+
+Zep allows you to be more intentional about constructing your prompt: 
+1. automatically adding a few recent messages, with the number customized for your app;
+2. a summary of recent conversations prior to the messages above;
+3. and/or contextually relevant summaries or messages surfaced from the entire chat session.
+4. and/or relevant Business data from Zep Document Collections.
+
+## What is Zep Cloud? ⚡️ 
+
+[Zep Cloud](https://www.getzep.com/) is a managed service with Zep Open Source at its core. In addition to Zep Open Source's memory management features, Zep Cloud offers:
+- **Fact Extraction:** Automatically build fact tables from conversations, without having to define a data schema upfront.
+- **Dialog Classification:** Instantly and accurately classify chat dialog. Understand user intent and emotion, segment users, and more. Route chains based on semantic context, and trigger events. 
+- **Structured Data Extraction:** Quickly extract business data from chat conversations using a schema you define. Understand what your Assistant should ask for next in order to complete its task.
 
-[![Zep Demo Video](https://img.youtube.com/vi/d6ryNEvMXno/maxresdefault.jpg)](https://vimeo.com/865785086?share=copy)
 
 ## Zep Python Client
 
 This is the Python client package for the Zep service. For more information about Zep, see https://github.com/getzep/zep.
 
 Zep QuickStart Guide: https://docs.getzep.com/deployment/quickstart
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zep-python Version: 2.0.0rc5 Summary: Long-Term
+Metadata-Version: 2.1 Name: zep-python Version: 2.0.0rc6 Summary: Long-Term
 Memory for AI Assistants. This is the Python client for the Zep service.
 Author: Daniel Chalef Author-email: daniel.chalef@private.org Requires-Python:
 >=3.9.0,<4 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: httpx (>=0.24.0,<0.29.0)
 Requires-Dist: pydantic (>=2.0.0) Description-Content-Type: text/markdown [!
@@ -11,47 +11,65 @@
 [lint](https://github.com/getzep/zep-python/actions/workflows/lint.yml/
 badge.svg)](https://github.com/getzep/zep-python/actions/workflows/lint.yml) [!
 [Release to PyPI](https://github.com/getzep/zep-python/actions/workflows/
 release.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/
 release.yml) ![GitHub](https://img.shields.io/github/license/getzep/zep-
 python?color=blue)
                                   _[_Z_e_p_ _L_o_g_o_]
-        ************ ZZeepp:: FFaasstt,, ssccaallaabbllee bbuuiillddiinngg bblloocckkss ffoorr LLLLMM aappppss ************
-********** CChhaatt hhiissttoorryy mmeemmoorryy,, eemmbbeeddddiinngg,, vveeccttoorr sseeaarrcchh,, ddaattaa eennrriicchhmmeenntt,, aanndd mmoorree..
-                                     **********
+           ************ ZZeepp:: LLoonngg--TTeerrmm MMeemmoorryy ffoorr ?â??AAII AAssssiissttaannttss.. ************
+     ********** RReeccaallll,, uunnddeerrssttaanndd,, aanndd eexxttrraacctt ddaattaa ffrroomm cchhaatt hhiissttoorriieess.. PPoowweerr
+                      ppeerrssoonnaalliizzeedd AAII eexxppeerriieenncceess.. **********
+
    _Q_u_i_c_k_ _S_t_a_r_t | _D_o_c_u_m_e_n_t_a_t_i_o_n | _L_a_n_g_C_h_a_i_n and _L_l_a_m_a_I_n_d_e_x Support | _D_i_s_c_o_r_d
                                 _w_w_w_._g_e_t_z_e_p_._c_o_m
-## What is Zep? Zep is an open source platform for productionizing LLM apps.
-Zep summarizes, embeds, and enriches chat histories and documents
-asynchronously, ensuring these operations don't impact your user's chat
-experience. Data is persisted to database, allowing you to scale out when
-growth demands. As drop-in replacements for popular LangChain components, you
-can get to production in minutes without rewriting code. [![Zep Demo Video]
-(https://img.youtube.com/vi/d6ryNEvMXno/maxresdefault.jpg)](https://vimeo.com/
-865785086?share=copy) ## Zep Python Client This is the Python client package
-for the Zep service. For more information about Zep, see https://github.com/
-getzep/zep. Zep QuickStart Guide: https://docs.getzep.com/deployment/quickstart
-Zep Documentation: [https://docs.getzep.com](https://docs.getzep.com/) ##
-Installation ```bash pip install zep-python ``` -- OR -- ```bash poetry add
-zep-python ``` ## Zep Cloud Installation In order to install Zep Python SDK
-with Zep Cloud support, you will need to install a release candidate version.
-```bash pip install --pre zep-python ``` -- OR -- ```bash poetry add zep-
-python@^2.0.0rc ``` You will also need to provide a Zep Project API key to your
-zep client for cloud support. You can find out about Zep Projects in our [cloud
-docs](https://help.getzep.com/projects.html) ### Using LangChain Zep Classes
-with `zep-python` (Currently only available on release candidate versions) In
-the pre-release version `zep-python` sdk comes with `ZepChatMessageHistory` and
-`ZepVectorStore` classes that are compatible with [LangChain's Python
-expression language](https://python.langchain.com/docs/expression_language/) In
-order to use these classes in your application, you need to make sure that you
-have `langchain_core` package installed, please refer to [Langchain's docs
-installation section](https://python.langchain.com/docs/get_started/
-installation#langchain-core). We support `langchain_core@>=0.1.3<0.2.0` You can
-import these classes in the following way: ```python from zep_python.langchain
-import ZepChatMessageHistory, ZepVectorStore ``` ### Running Examples You will
-need to set the following environment variables to run examples in the
-`examples` directory: ```dotenv # Please use examples/.env.example as a
-template for .env file # Required ZEP_API_KEY=# Your Zep Project API Key
-ZEP_COLLECTION=# used in ingestion script and in vector store examples
-OPENAI_API_KEY=# Your OpenAI API Key # Optional (If you want to use langsmith
-with LangServe Sample App) LANGCHAIN_TRACING_V2=true LANGCHAIN_API_KEY=
-LANGCHAIN_PROJECT=# If not specified, defaults to "default" ```
+## What is Zep? ð¬ Zep is a long-term memory service for AI Assistant apps.
+With Zep, you can provide AI assistants with the ability to recall past
+conversations, no matter how distant, while also reducing hallucinations,
+latency, and cost. ### How Zep works Zep does all of this asynchronously,
+ensuring these operations don't impact your user's chat experience. Data is
+persisted to database, allowing you to scale out when growth demands. Zep also
+provides a simple, easy to use abstraction for document vector search called
+Document Collections. This is designed to complement Zep's core memory
+features, but is not designed to be a general purpose vector database. Zep
+allows you to be more intentional about constructing your prompt: 1.
+automatically adding a few recent messages, with the number customized for your
+app; 2. a summary of recent conversations prior to the messages above; 3. and/
+or contextually relevant summaries or messages surfaced from the entire chat
+session. 4. and/or relevant Business data from Zep Document Collections. ##
+What is Zep Cloud? â¡ï¸ [Zep Cloud](https://www.getzep.com/) is a managed
+service with Zep Open Source at its core. In addition to Zep Open Source's
+memory management features, Zep Cloud offers: - **Fact Extraction:**
+Automatically build fact tables from conversations, without having to define a
+data schema upfront. - **Dialog Classification:** Instantly and accurately
+classify chat dialog. Understand user intent and emotion, segment users, and
+more. Route chains based on semantic context, and trigger events. -
+**Structured Data Extraction:** Quickly extract business data from chat
+conversations using a schema you define. Understand what your Assistant should
+ask for next in order to complete its task. ## Zep Python Client This is the
+Python client package for the Zep service. For more information about Zep, see
+https://github.com/getzep/zep. Zep QuickStart Guide: https://docs.getzep.com/
+deployment/quickstart Zep Documentation: [https://docs.getzep.com](https://
+docs.getzep.com/) ## Installation ```bash pip install zep-python ``` -- OR -
+- ```bash poetry add zep-python ``` ## Zep Cloud Installation In order to
+install Zep Python SDK with Zep Cloud support, you will need to install a
+release candidate version. ```bash pip install --pre zep-python ``` -- OR -
+- ```bash poetry add zep-python@^2.0.0rc ``` You will also need to provide a
+Zep Project API key to your zep client for cloud support. You can find out
+about Zep Projects in our [cloud docs](https://help.getzep.com/projects.html)
+### Using LangChain Zep Classes with `zep-python` (Currently only available on
+release candidate versions) In the pre-release version `zep-python` sdk comes
+with `ZepChatMessageHistory` and `ZepVectorStore` classes that are compatible
+with [LangChain's Python expression language](https://python.langchain.com/
+docs/expression_language/) In order to use these classes in your application,
+you need to make sure that you have `langchain_core` package installed, please
+refer to [Langchain's docs installation section](https://python.langchain.com/
+docs/get_started/installation#langchain-core). We support
+`langchain_core@>=0.1.3<0.2.0` You can import these classes in the following
+way: ```python from zep_python.langchain import ZepChatMessageHistory,
+ZepVectorStore ``` ### Running Examples You will need to set the following
+environment variables to run examples in the `examples` directory: ```dotenv #
+Please use examples/.env.example as a template for .env file # Required
+ZEP_API_KEY=# Your Zep Project API Key ZEP_COLLECTION=# used in ingestion
+script and in vector store examples OPENAI_API_KEY=# Your OpenAI API Key #
+Optional (If you want to use langsmith with LangServe Sample App)
+LANGCHAIN_TRACING_V2=true LANGCHAIN_API_KEY= LANGCHAIN_PROJECT=# If not
+specified, defaults to "default" ```
```

