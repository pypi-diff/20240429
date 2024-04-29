# Comparing `tmp/sibila-0.4.0.tar.gz` & `tmp/sibila-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sibila-0.4.0.tar", last modified: Tue Apr  9 16:07:32 2024, max compression
+gzip compressed data, was "sibila-0.4.1.tar", last modified: Mon Apr 29 17:49:51 2024, max compression
```

## Comparing `sibila-0.4.0.tar` & `sibila-0.4.1.tar`

### file list

```diff
@@ -1,49 +1,55 @@
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-09 16:07:32.290619 sibila-0.4.0/
--rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1078 2024-01-30 10:27:20.000000 sibila-0.4.0/LICENSE
--rw-r--r--   0 jorge     (1000) jorge     (1000)     4497 2024-04-09 16:07:32.290619 sibila-0.4.0/PKG-INFO
--rwxrwxr-x   0 jorge     (1000) jorge     (1000)     3299 2024-04-09 15:35:13.000000 sibila-0.4.0/README.md
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1560 2024-04-08 14:27:47.000000 sibila-0.4.0/pyproject.toml
--rw-rw-r--   0 jorge     (1000) jorge     (1000)       38 2024-04-09 16:07:32.290619 sibila-0.4.0/setup.cfg
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-09 16:07:32.286619 sibila-0.4.0/sibila/
--rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1249 2024-04-09 16:03:20.000000 sibila-0.4.0/sibila/__init__.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    29858 2024-03-09 11:56:55.000000 sibila-0.4.0/sibila/cli.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     5366 2024-03-13 19:10:42.000000 sibila-0.4.0/sibila/context.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    10254 2024-04-08 09:50:19.000000 sibila-0.4.0/sibila/gen.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     8577 2024-03-06 10:11:40.000000 sibila-0.4.0/sibila/json_grammar.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    24842 2024-02-29 16:28:12.000000 sibila-0.4.0/sibila/json_schema.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    23851 2024-04-08 14:31:59.000000 sibila-0.4.0/sibila/llamacpp.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    16156 2024-04-09 11:12:16.000000 sibila-0.4.0/sibila/mistral.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    73925 2024-04-09 11:29:20.000000 sibila-0.4.0/sibila/model.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    47337 2024-04-07 11:35:48.000000 sibila-0.4.0/sibila/models.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    17408 2024-02-29 10:46:02.000000 sibila-0.4.0/sibila/multigen.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     2280 2024-04-08 14:52:24.000000 sibila-0.4.0/sibila/null.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    21650 2024-04-09 11:16:34.000000 sibila-0.4.0/sibila/openai.py
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-09 16:07:32.286619 sibila-0.4.0/sibila/res/
--rwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-03-07 18:25:20.000000 sibila-0.4.0/sibila/res/__init__.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    12204 2024-04-08 15:05:04.000000 sibila-0.4.0/sibila/res/base_formats.json
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1620 2024-04-07 11:16:28.000000 sibila-0.4.0/sibila/res/base_models.json
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    15392 2024-04-09 11:17:44.000000 sibila-0.4.0/sibila/schema_format_openai.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4628 2024-02-26 20:11:39.000000 sibila-0.4.0/sibila/text_splitter.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    20173 2024-03-16 18:23:26.000000 sibila-0.4.0/sibila/thread.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    13103 2024-04-08 14:37:15.000000 sibila-0.4.0/sibila/tools.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1236 2024-03-14 11:27:35.000000 sibila-0.4.0/sibila/utils.py
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-09 16:07:32.290619 sibila-0.4.0/sibila.egg-info/
--rw-r--r--   0 jorge     (1000) jorge     (1000)     4497 2024-04-09 16:07:32.000000 sibila-0.4.0/sibila.egg-info/PKG-INFO
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      962 2024-04-09 16:07:32.000000 sibila-0.4.0/sibila.egg-info/SOURCES.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)        1 2024-04-09 16:07:32.000000 sibila-0.4.0/sibila.egg-info/dependency_links.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)       43 2024-04-09 16:07:32.000000 sibila-0.4.0/sibila.egg-info/entry_points.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      113 2024-04-09 16:07:32.000000 sibila-0.4.0/sibila.egg-info/requires.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)        7 2024-04-09 16:07:32.000000 sibila-0.4.0/sibila.egg-info/top_level.txt
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-09 16:07:32.290619 sibila-0.4.0/tests/
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    11688 2024-03-11 10:47:12.000000 sibila-0.4.0/tests/test_cli.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    20550 2024-04-08 16:10:27.000000 sibila-0.4.0/tests/test_examples_tinyllama.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     6696 2024-04-08 11:31:34.000000 sibila-0.4.0/tests/test_fireworks_mixtral.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     2347 2024-03-16 12:05:44.000000 sibila-0.4.0/tests/test_formats.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    14927 2024-02-29 16:31:57.000000 sibila-0.4.0/tests/test_json_schema.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1375 2024-03-16 19:37:51.000000 sibila-0.4.0/tests/test_llamacpp_models.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     7566 2024-04-08 16:12:48.000000 sibila-0.4.0/tests/test_llamacpp_tinyllama.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     6369 2024-04-08 11:08:30.000000 sibila-0.4.0/tests/test_mistral_small.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4613 2024-04-04 18:27:52.000000 sibila-0.4.0/tests/test_null_extract.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     6298 2024-04-08 11:15:51.000000 sibila-0.4.0/tests/test_openai_gpt35.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     6287 2024-04-08 11:16:00.000000 sibila-0.4.0/tests/test_openai_gpt4.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     6576 2024-04-08 11:28:50.000000 sibila-0.4.0/tests/test_together_mixtral.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-29 17:49:51.330298 sibila-0.4.1/
+-rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1078 2024-01-30 10:27:20.000000 sibila-0.4.1/LICENSE
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     4746 2024-04-29 17:49:51.330298 sibila-0.4.1/PKG-INFO
+-rwxrwxr-x   0 jorge     (1000) jorge     (1000)     3487 2024-04-29 17:34:57.000000 sibila-0.4.1/README.md
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1629 2024-04-29 16:44:20.000000 sibila-0.4.1/pyproject.toml
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)       38 2024-04-29 17:49:51.330298 sibila-0.4.1/setup.cfg
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-29 17:49:51.326298 sibila-0.4.1/sibila/
+-rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1312 2024-04-26 15:56:50.000000 sibila-0.4.1/sibila/__init__.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    14965 2024-04-29 14:31:30.000000 sibila-0.4.1/sibila/anthropic.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    29858 2024-03-09 11:56:55.000000 sibila-0.4.1/sibila/cli.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     5366 2024-03-13 19:10:42.000000 sibila-0.4.1/sibila/context.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    10272 2024-04-27 10:05:28.000000 sibila-0.4.1/sibila/gen.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     8577 2024-03-06 10:11:40.000000 sibila-0.4.1/sibila/json_grammar.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    24981 2024-04-27 09:42:38.000000 sibila-0.4.1/sibila/json_schema.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    23826 2024-04-26 15:02:47.000000 sibila-0.4.1/sibila/llamacpp.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    16238 2024-04-29 14:31:34.000000 sibila-0.4.1/sibila/mistral.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    74638 2024-04-27 10:40:15.000000 sibila-0.4.1/sibila/model.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    47729 2024-04-29 16:00:26.000000 sibila-0.4.1/sibila/models.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    17408 2024-02-29 10:46:02.000000 sibila-0.4.1/sibila/multigen.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2489 2024-04-29 14:30:36.000000 sibila-0.4.1/sibila/null.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    21545 2024-04-27 10:52:11.000000 sibila-0.4.1/sibila/openai.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-29 17:49:51.326298 sibila-0.4.1/sibila/res/
+-rwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-03-07 18:25:20.000000 sibila-0.4.1/sibila/res/__init__.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    14777 2024-04-27 19:34:06.000000 sibila-0.4.1/sibila/res/base_formats.json
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1869 2024-04-27 17:03:26.000000 sibila-0.4.1/sibila/res/base_models.json
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    15043 2024-04-27 10:51:43.000000 sibila-0.4.1/sibila/schema_format_openai.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4628 2024-02-26 20:11:39.000000 sibila-0.4.1/sibila/text_splitter.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    20235 2024-04-26 15:07:47.000000 sibila-0.4.1/sibila/thread.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    13103 2024-04-08 14:37:15.000000 sibila-0.4.1/sibila/tools.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1245 2024-04-29 15:26:33.000000 sibila-0.4.1/sibila/utils.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-29 17:49:51.330298 sibila-0.4.1/sibila.egg-info/
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     4746 2024-04-29 17:49:51.000000 sibila-0.4.1/sibila.egg-info/PKG-INFO
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1167 2024-04-29 17:49:51.000000 sibila-0.4.1/sibila.egg-info/SOURCES.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)        1 2024-04-29 17:49:51.000000 sibila-0.4.1/sibila.egg-info/dependency_links.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)       43 2024-04-29 17:49:51.000000 sibila-0.4.1/sibila.egg-info/entry_points.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      144 2024-04-29 17:49:51.000000 sibila-0.4.1/sibila.egg-info/requires.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)        7 2024-04-29 17:49:51.000000 sibila-0.4.1/sibila.egg-info/top_level.txt
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-29 17:49:51.330298 sibila-0.4.1/tests/
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4037 2024-04-29 16:15:42.000000 sibila-0.4.1/tests/test_anthropic_claude-3-haiku.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    11685 2024-04-29 16:05:39.000000 sibila-0.4.1/tests/test_cli.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4515 2024-04-29 16:05:46.000000 sibila-0.4.1/tests/test_common_llamacpp.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     8266 2024-04-29 15:07:11.000000 sibila-0.4.1/tests/test_common_llamacpp_examples.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     3780 2024-04-27 19:04:48.000000 sibila-0.4.1/tests/test_common_remote.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     7624 2024-04-27 20:12:25.000000 sibila-0.4.1/tests/test_common_remote_examples.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    20543 2024-04-26 18:26:18.000000 sibila-0.4.1/tests/test_examples_tinyllama.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4369 2024-04-26 10:26:46.000000 sibila-0.4.1/tests/test_fireworks_mixtral.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2347 2024-03-16 12:05:44.000000 sibila-0.4.1/tests/test_formats.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    14927 2024-02-29 16:31:57.000000 sibila-0.4.1/tests/test_json_schema.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1664 2024-04-27 17:53:16.000000 sibila-0.4.1/tests/test_llamacpp_models_dir.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     7957 2024-04-26 10:32:15.000000 sibila-0.4.1/tests/test_llamacpp_tinyllama.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4090 2024-04-26 10:27:01.000000 sibila-0.4.1/tests/test_mixtral_mistral_small.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4613 2024-04-04 18:27:52.000000 sibila-0.4.1/tests/test_null_extract.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4099 2024-04-29 16:16:00.000000 sibila-0.4.1/tests/test_openai_gpt35.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4086 2024-04-29 16:15:54.000000 sibila-0.4.1/tests/test_openai_gpt4.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4338 2024-04-26 10:27:29.000000 sibila-0.4.1/tests/test_together_mixtral.py
```

### Comparing `sibila-0.4.0/LICENSE` & `sibila-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sibila-0.4.0/PKG-INFO` & `sibila-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sibila
-Version: 0.4.0
+Version: 0.4.1
 Summary: Structured queries from local or online LLM models
 Author-email: Jorge Diogo <jndiogo@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jndiogo/sibila
 Project-URL: Documentation, https://jndiogo.github.io/sibila
 Project-URL: Issues, https://github.com/jndiogo/sibila/issues
 Keywords: llama.cpp,AI,Transformers,GPT,LLM
@@ -19,29 +19,32 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: llama-cpp-python>=0.2
 Requires-Dist: openai>=1.1
 Requires-Dist: tiktoken
+Requires-Dist: anthropic
 Requires-Dist: mistralai
 Requires-Dist: jinja2>=3.0
 Requires-Dist: jsonschema
 Requires-Dist: pydantic>=2.0
 Requires-Dist: typing_extensions
 Requires-Dist: tqdm
+Requires-Dist: pytest-asyncio>=0.17
 
 # Sibila
 
-Extract structured data from remote or local LLM models. Predictable output is essential for any serious use of LLMs.
+Extract structured data from remote or local LLM models. Predictable output is important for serious use of LLMs.
 
-- Extract data into Pydantic objects, dataclasses or simple types.
-- Same API for local file models and remote OpenAI, Mistral AI and other models.
+- Query structured data into Pydantic objects, dataclasses or simple types.
+- Access remote models from OpenAI, Anthropic, Mistral AI and other providers.
+- Use local models like Llama-3, Phi-3, OpenChat or any other GGUF file model.
+- Besides structured extraction, Sibila is also a general purpose model access library, to generate plain text or free JSON results, with the same API for local and remote models.
 - Model management: download models, manage configuration, quickly switch between models.
-- Tools for evaluating output across local/remote models, for chat-like interaction and more.
 
 No matter how well you craft a prompt begging a model for the output you need, it can always respond something else. Extracting structured data can be a big step into getting predictable behavior from your models.
 
 See [What can you do with Sibila?](https://jndiogo.github.io/sibila/what/)
 
 To extract structured data from a local model:
 
@@ -67,15 +70,15 @@
 Info(event_year=1969,
      first_name='Neil',
      last_name='Armstrong',
      age_at_the_time=38,
      nationality='American')
 ```
 
-Or to use OpenAI's GPT-4, we would simply replace the model's name:
+Or to use a remote model like OpenAI's GPT-4, we would simply replace the model's name:
 
 ``` python
 model = Models.create("openai:gpt-4")
 
 model.extract(Info, "Who was the first man in the moon?")
 ```
```

### Comparing `sibila-0.4.0/README.md` & `sibila-0.4.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Sibila
 
-Extract structured data from remote or local LLM models. Predictable output is essential for any serious use of LLMs.
+Extract structured data from remote or local LLM models. Predictable output is important for serious use of LLMs.
 
-- Extract data into Pydantic objects, dataclasses or simple types.
-- Same API for local file models and remote OpenAI, Mistral AI and other models.
+- Query structured data into Pydantic objects, dataclasses or simple types.
+- Access remote models from OpenAI, Anthropic, Mistral AI and other providers.
+- Use local models like Llama-3, Phi-3, OpenChat or any other GGUF file model.
+- Besides structured extraction, Sibila is also a general purpose model access library, to generate plain text or free JSON results, with the same API for local and remote models.
 - Model management: download models, manage configuration, quickly switch between models.
-- Tools for evaluating output across local/remote models, for chat-like interaction and more.
 
 No matter how well you craft a prompt begging a model for the output you need, it can always respond something else. Extracting structured data can be a big step into getting predictable behavior from your models.
 
 See [What can you do with Sibila?](https://jndiogo.github.io/sibila/what/)
 
 To extract structured data from a local model:
 
@@ -35,15 +36,15 @@
 Info(event_year=1969,
      first_name='Neil',
      last_name='Armstrong',
      age_at_the_time=38,
      nationality='American')
 ```
 
-Or to use OpenAI's GPT-4, we would simply replace the model's name:
+Or to use a remote model like OpenAI's GPT-4, we would simply replace the model's name:
 
 ``` python
 model = Models.create("openai:gpt-4")
 
 model.extract(Info, "Who was the first man in the moon?")
 ```
```

### Comparing `sibila-0.4.0/pyproject.toml` & `sibila-0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -30,20 +30,22 @@
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "llama-cpp-python >= 0.2",
     "openai >= 1.1",
     "tiktoken",
+    "anthropic",
     "mistralai",
     "jinja2 >= 3.0",
     "jsonschema",
     "pydantic >= 2.0",
     "typing_extensions",
     "tqdm",
+    "pytest-asyncio >= 0.17",
 ]
 dynamic = ["version"]
 
 
 [tool.setuptools.dynamic]
 version = {attr = "sibila.__version__"}
 
@@ -62,9 +64,10 @@
 Documentation = "https://jndiogo.github.io/sibila"
 Issues = "https://github.com/jndiogo/sibila/issues"
 
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
+asyncio_mode = "auto"
 # addopts = "-ra -q"
 # testpaths = ["tests"]
```

### Comparing `sibila-0.4.0/sibila/__init__.py` & `sibila-0.4.1/sibila/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Structured data from local or remote LLM models."""
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 __all__ = [
     "Models",
     "Model", "TextModel", "MessagesModel", "Tokenizer",
     "GenConf", "GenRes", "GenError", "GenOut",
+    "AnthropicModel",
+    "FireworksModel",
     "LlamaCppModel", "LlamaCppTokenizer",
-    "OpenAIModel", "OpenAITokenizer",
-    "TogetherModel", "FireworksModel",
     "MistralModel",
+    "OpenAIModel", "OpenAITokenizer",
+    "TogetherModel",
     "Thread", "MsgKind",
     "Context", "Trim",
     "JSchemaConf",
     "TDesc"
 ]
 
 __author__ = "Jorge Diogo"
@@ -35,32 +37,34 @@
     Model,
     TextModel,
     FormattedTextModel,
     MessagesModel,
     Tokenizer
 )
 
+
+from .anthropic import AnthropicModel
+
 from .llamacpp import (
     LlamaCppModel,
     LlamaCppTokenizer
 )
 
+from .mistral import MistralModel
+
 from .openai import (
     OpenAIModel,
     OpenAITokenizer
 )
 
 from .schema_format_openai import (
     TogetherModel,
     FireworksModel
 )
 
-from .mistral import (
-    MistralModel
-)
 
 from .context import (
     Context,
     Trim
 )
 
 from .models import Models
```

### Comparing `sibila-0.4.0/sibila/cli.py` & `sibila-0.4.1/sibila/cli.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.0/sibila/context.py` & `sibila-0.4.1/sibila/context.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.0/sibila/gen.py` & `sibila-0.4.1/sibila/gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         return asdict(self)
 
 
     @staticmethod
     def from_dict(dic: dict) -> Any: # Any = GenConf
         return GenConf(**dic)
 
+
     def resolve_max_tokens(self,
                            ctx_len: int,
                            max_tokens_limit: Optional[int] = None) -> int:
         """Calculate actual max_tokens value for cases where it's zero or a percentage of model's ctx_len)
 
         Args:
             ctx_len: Model's context length.
@@ -121,14 +122,15 @@
         if max_tokens <= 0:
             if max_tokens == 0:
                 max_tokens = ctx_len
             else:
                 max_tokens = min(-max_tokens, 100)
                 max_tokens = int(max_tokens / 100.0 * ctx_len)
                 max_tokens = max(1,max_tokens)
+                
         if max_tokens_limit is not None:
             max_tokens = min(max_tokens, max_tokens_limit)
 
         return max_tokens
 
 
     def resolve_special(self,
```

### Comparing `sibila-0.4.0/sibila/json_grammar.py` & `sibila-0.4.1/sibila/json_grammar.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.0/sibila/json_schema.py` & `sibila-0.4.1/sibila/json_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -662,14 +662,16 @@
 
 
 
 def build_dataclass_object_json_schema(type_: Any) -> dict:
     """Build a JSON schema for a dataclass type."""
 
     desc = type_.__doc__
+    if desc.startswith(type_.__name__ + "(") and desc[-1] == ")": # ignore automatic doc from dataclass params
+        desc = None        
 
     props = {}
     required = []
 
     flds = fields(type_)
     for fl in flds:
         name = fl.name
```

### Comparing `sibila-0.4.0/sibila/llamacpp.py` & `sibila-0.4.1/sibila/llamacpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,18 +54,14 @@
 
 
 
 class LlamaCppModel(FormattedTextModel):
     """Use local GGUF format models via llama.cpp engine.
     
     Supports grammar-constrained JSON output following a JSON schema.
-
-    Attributes:
-        ctx_len: Maximum context length, shared for input + output.
-        desc: Model information.
     """
 
     PROVIDER_NAME:str = "llamacpp"
     """Provider prefix that this class handles."""
 
     _llama: Llama
     """LlamaCpp instance"""
@@ -334,17 +330,22 @@
             Tuple of strings: generated_text, finish_reason.
         """
 
         return self._gen_text(text, genconf)
 
 
 
+   
+    def name(self) -> str:
+        """Model (short) name."""
+        return os.path.basename(self._model_path)
 
-
-
+    def desc(self) -> str:
+        """Model description."""
+        return f"{type(self).__name__}: {self._model_path} - '{self._llama._model.desc()}'"
 
         
     @classmethod
     def provider_version(_) -> str:
         """Provider library version: provider x.y.z
         Ex. llama-cpp-python 0.2.44
         """
@@ -352,20 +353,18 @@
             import llama_cpp
             ver = llama_cpp.__version__
         except Exception:
             raise ImportError("Please install llama-cpp-python by running: pip install llama-cpp-python")
             
         return f"llama-cpp-python {ver}"
 
-    
-    @property
-    def desc(self) -> str:
-        """Model description."""
-        return f"{type(self).__name__}: {self._model_path} - '{self._llama._model.desc()}'"
-    
+
+
+
+
     @property
     def n_embd(self) -> int:
         """Embedding size of model."""
         return self._llama.n_embd()
 
     @property
     def n_params(self) -> int:
```

### Comparing `sibila-0.4.0/sibila/mistral.py` & `sibila-0.4.1/sibila/mistral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Mistral remote model access.
 
 - MistralModel: Access Mistral AI models.
 """
 
 
 from typing import Any, Optional, Union
-import sys, json
+import os, sys, json
 from time import time 
 from copy import copy
 
 import logging
 logger = logging.getLogger(__name__)
 
 
@@ -42,18 +42,14 @@
 
 class MistralModel(MessagesModel):
     """Access a Mistral AI model.
     Supports constrained JSON output, via the Mistral API function calling mechanism.
 
     Ref:
         https://docs.mistral.ai/guides/function-calling/
-
-    Attributes:
-        ctx_len: Maximum context length, shared for input + output.
-        desc: Model information.
     """
 
     PROVIDER_NAME:str = "mistral"
     """Provider prefix that this class handles."""
 
     _token_estimation_factor: float
     """Multiplication factor to estimate token usage: multiplies text length to obtain token length."""
@@ -153,20 +149,25 @@
         self.max_tokens_limit = max_tokens_limit or default_max_tokens_limit
 
         self.max_tokens_limit = min(self.max_tokens_limit, self.ctx_len)
 
         self._token_estimation_factor = token_estimation_factor or default_token_estimation_factor
 
 
-        # only check for "json" text presence as json schema is requested with the tools facility.
+        # only check for "json" text presence as json schema (including field descriptions) is requested with the tools facility.
         self.json_format_instructors["json_schema"] = self.json_format_instructors["json"]
 
         self._client_init_kwargs = mistral_init_kwargs
+
         if api_key is not None:
-            self._client_init_kwargs["api_key"] = api_key
+            self._client_init_kwargs["api_key"] = api_key    
+        elif "api_key" not in self._client_init_kwargs and "MISTRAL_API_KEY" in os.environ:
+            # "MISTRAL_API_KEY" env key is ignored in pytest?
+            self._client_init_kwargs["api_key"] = os.environ["MISTRAL_API_KEY"]
+
 
 
 
 
 
 
     def _ensure_client(self,
@@ -213,15 +214,14 @@
 
         Instead we allow all available output length. This is only possible because endpoint
         doesn't error when max_tokens is larger than possible:"""
         resolved_max_tokens = self.resolve_genconf_max_tokens(0, genconf)
 
 
         # https://docs.mistral.ai/api/#operation/createChatCompletion
-        fn_name = "json_out"
 
         json_kwargs: dict = {}
         format = genconf.format
         if format == "json":
             
             if genconf.json_schema is None:
                 json_kwargs["response_format"] = {"type": "json_object"}
@@ -233,15 +233,15 @@
                 else:
                     params = genconf.json_schema
                 
                 json_kwargs["tools"] = [
                     {
                         "type": "function",
                         "function": {
-                            "name": fn_name,
+                            "name": self.output_fn_name,
                             "parameters": params
                         }
                     }
                 ]
 
                 json_kwargs["tool_choice"] = "any"
 
@@ -263,23 +263,20 @@
                   "top_p": 1. if genconf.temperature == 0 else genconf.top_p,
                   # "random_seed": seed,
                   **json_kwargs}
 
         # inject model-specific args, if any
         kwargs.update(genconf.resolve_special(self.PROVIDER_NAME))
 
-        return (kwargs,
-                fn_name,
-                genconf)
+        return (kwargs, genconf)
         
 
     def _gen_post(self, 
                   response: Any,
                   pre_kwargs: dict,
-                  fn_name: str,
                   genconf: GenConf
                   ) -> GenOut:
             
         logger.debug(f"Mistral response: {response}")
 
         choice = response.choices[0]
         
@@ -293,16 +290,16 @@
             
             # json schema generation via the tools API:
             if message.tool_calls is not None:
                 if len(message.tool_calls) != 1:
                     logger.warn(f"Mistral: expecting single message.tool_calls, but received {len(message.tool_calls)} - using first.")
 
                 fn = message.tool_calls[0].function
-                if fn.name != fn_name:
-                    logger.warn(f"Mistral: expecting '{fn_name}' function name, received ({fn.name})")
+                if fn.name != self.output_fn_name:
+                    logger.warn(f"Mistral: expecting '{self.output_fn_name}' function name, received ({fn.name})")
 
                 text = fn.arguments
 
             else: # use content instead
                 logger.warn("Mistral: expecting message.tool_calls, but none received - using text content")
                 text = message.content # type: ignore[assignment]
         
@@ -336,28 +333,27 @@
         Returns:
             A GenOut object with result, generated text, etc.
             The output text is in GenOut.text.
         """
 
 
         genconf2: GenConf
-        kwargs, fn_name, genconf2 = self._gen_pre(thread, genconf)
+        kwargs, genconf2 = self._gen_pre(thread, genconf)
 
         self._ensure_client(False)
 
         try:
             response = self._client.chat(**kwargs) # type: ignore[attr-defined]
 
         except Exception as e:
             raise RuntimeError(f"Cannot generate. Internal error: {e}")
 
 
         return self._gen_post(response,
                               kwargs,
-                              fn_name,
                               genconf2)
     
 
 
 
     async def gen_async(self, 
                         thread: Thread,
@@ -375,27 +371,26 @@
 
         Returns:
             A GenOut object with result, generated text, etc.
             The output text is in GenOut.text.
         """
 
         genconf2: GenConf
-        kwargs, fn_name, genconf2 = self._gen_pre(thread, genconf)
+        kwargs, genconf2 = self._gen_pre(thread, genconf)
 
         self._ensure_client(True)
 
         try:
             response = await self._client_async.chat(**kwargs) # type: ignore[attr-defined]
 
         except Exception as e:
             raise RuntimeError(f"Cannot generate. Internal error: {e}")
 
         return self._gen_post(response,
                               kwargs,
-                              fn_name,
                               genconf2)
     
 
    
 
 
 
@@ -435,34 +430,14 @@
             tools_num_tokens = len(js_str) * self._token_estimation_factor
             num_tokens += int(tools_num_tokens)
             # print("tools_num_tokens", tools_num_tokens)
         
         # print(num_tokens)
         return num_tokens
 
-
-
-    
-    @property
-    def desc(self) -> str:
-        """Model description."""
-        return f"MistralModel: {self._model_name}"
-
-
-    @classmethod
-    def provider_version(_) -> str:
-        """Provider library version: provider x.y.z
-        Ex. mistralai 0.1.8
-        """
-        try:
-            ver = MistralClient()._version
-        except Exception:
-            raise ImportError("Please install mistralai by running: pip install mistralai")
-            
-        return f"mistralai {ver}"
     
     @classmethod
     def known_models(cls,
                      api_key: Optional[str] = None) -> Union[list[str], None]:
         """If the model can only use a fixed set of models, return their names. Otherwise, return None.
 
         Args:
@@ -485,7 +460,29 @@
             out.append(mod.id)
 
         return sorted(out)
 
 
 
 
+
+    def name(self) -> str:
+        """Model (short) name."""
+        return self._model_name
+        
+    def desc(self) -> str:
+        """Model description."""
+        return f"MistralModel: {self._model_name}"
+
+
+    @classmethod
+    def provider_version(_) -> str:
+        """Provider library version: provider x.y.z
+        Ex. mistralai 0.1.8
+        """
+        try:
+            ver = MistralClient()._version
+        except Exception:
+            raise ImportError("Please install mistralai by running: pip install mistralai")
+            
+        return f"mistralai {ver}"
+
```

### Comparing `sibila-0.4.0/sibila/model.py` & `sibila-0.4.1/sibila/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,22 +178,25 @@
     json_format_instructors: dict
     """If GenConf.json / GenConf.json_schema is used, these strings are appended to first thread msg of either instructions or IN kind. See initialization below."""
 
     json_in_dumps_kwargs: dict
     """Object to string formatting options for json.dumps() calls. See initialization below."""
 
     ctx_len: int
-    """Maximum context token length that can be passed to model as input. There can be a limit for output tokens in the max_tokens_limit."""
+    """Maximum context token length, including input and model output. There can be a limit for output tokens in the max_tokens_limit."""
 
     max_tokens_limit: int
-    """Some models limit the size of emitted output tokens, which is stored in this property."""
+    """Some models limit the size of emitted output tokens."""
 
     output_key_name: str
     """Name used when an output key needs to be created for JSON output."""
 
+    output_fn_name: str
+    """Function name for models that return JSON with a Tools/Functions-style API."""
+    
     PROVIDER_NAME: str = NotImplemented
     """Provider prefix that this class handles."""
 
     
     def __init__(self,
                  is_local_model: bool,
                  genconf: Union[GenConf, None],
@@ -209,14 +212,15 @@
         """
         
         self.is_local_model = is_local_model
         
         self.ctx_len = 0
         self.max_tokens_limit = sys.maxsize
         self.output_key_name = "output"
+        self.output_fn_name = "json_out"
 
         self.tokenizer = tokenizer # type: ignore[assignment]
 
         if genconf is None:
             self.genconf = GenConf()
         else:
             self.genconf = genconf.clone()
@@ -637,15 +641,14 @@
                          thread: Thread,
                          genconf: Union[GenConf, None],
                          schemaconf: Union[JSchemaConf, None]
                          ) -> Any:
 
         schema, created_output_key = build_root_json_schema(target, 
                                                             self.output_key_name)
-        
         final_type, is_list = get_final_type(target)
 
         if schemaconf is None:
             schemaconf = JSchemaConf()
 
         return (thread,
                 schema,
@@ -1569,45 +1572,55 @@
             api_key: If the model provider requires an API key, pass it here or set it in the respective env variable.
 
         Returns:
             Returns a list of known models or None if unable to fetch it.
         """
         return None
 
-    @classmethod
-    def version(cls) -> str:
-        """Sibila version + provider version
-        Ex: sibila='0.2.3' provider='llama-cpp-python 0.2.44'        
-        """        
-        from .__init__ import __version__ as version  # type: ignore[import-not-found]
-        return f"sibila='{version}' provider='{cls.provider_version()}'"
-        
-    @classmethod
+
+
+
+
     @abstractmethod
-    def provider_version(cls) -> str:
-        """Provider library version: provider x.y.z
-        Ex. llama-cpp-python 0.2.44
-        """
+    def name(self) -> str:
+        """Model (short) name."""
         ...
 
-
-    @property
+    @abstractmethod
     def desc(self) -> str:
         """Model description."""
-        return "Unknown model desc"
+        ...
     
     def info(self) -> str:
-        """Model object information."""
-        return f"desc='{self.desc}',\n" \
+        """Model description and config information."""
+        return f"desc='{self.desc()}',\n" \
                f"ctx_len={self.ctx_len}, max_tokens_limit={self.max_tokens_limit},\n" \
                f"genconf={self.genconf}"
                
-    
+
+    @classmethod
+    @abstractmethod
+    def provider_version(cls) -> str:
+        """Provider library version: provider x.y.z
+        Ex. llama-cpp-python 0.2.44
+        """
+        ...
+
+    @classmethod
+    def version(cls) -> str:
+        """Sibila version + provider version
+        Ex: sibila='0.2.3' provider='llama-cpp-python 0.2.44'        
+        """        
+        from .__init__ import __version__ as version  # type: ignore[import-not-found]
+        return f"sibila='{version}' provider='{cls.provider_version()}'"
+        
+
+
     def __str__(self):
-        return self.info()
+        return self.desc_info()
 
 
 
 
 
     
     
@@ -1669,82 +1682,91 @@
         
         return thread
 
 
     
     
     def _prepare_gen_out(self,
-                         text: str, 
+                         response: Union[str,dict, None],
                          finish: str,
                          genconf: GenConf) -> GenOut:
         """Perform common operations over the generated model response.
 
         Args:
-            text: Text obtained from model.
+            response: Text or a JSON object obtained from model.
             finish: Model finish reason - only "stop", "length" are used, others will map as GenRes.ERROR_MODEL.
 
         Returns:
             A GenOut object with result, generated text, etc. 
         """
 
-        logger.debug(f"Response finish='{finish}': █{text}█")
+        logger.debug(f"Response finish='{finish}': █{response}█")
         
-        if text is None:
-            text = ''
-        else:
-            text = text.strip()
+        if response is None:
+            response = ''
 
         if genconf.format == "json":
-            if "\\u" in text:
-                # dumps(with default ensure_ascii=False) -> ascii (subset of utf-8) -> text.encode("latin1") -> latin1 ->
-                #   decode("unicode-escape") -> utf-8
-                text = text.encode("latin1").decode("unicode-escape")
-
-            # some troubled remote models may include chit-chat after the JSON
-            begin = text.find("{")
-            if begin > 0:
-                text = text[begin:]
-            end = text.rfind("}")
-            if end > 0:
-                text = text[:end + 1]
-                
+            if isinstance(response, str):
+                response = response.strip()
+
+                if "\\u" in response:
+                    # dumps(with default ensure_ascii=False) -> ascii (subset of utf-8) -> text.encode("latin1") -> latin1 ->
+                    #   decode("unicode-escape") -> utf-8
+                    response = response.encode("latin1").decode("unicode-escape")
+
+                # some troubled remote models may include chit-chat after the JSON
+                begin = response.find("{")
+                if begin > 0:
+                    response = response[begin:]
+                end = response.rfind("}")
+                if end > 0:
+                    response = response[:end + 1]
+
             try:
-                dic = json.loads(text)
+                if isinstance(response, str):
+                    dic = json.loads(response)
+                else:
+                    dic = response
 
                 if genconf.json_schema is not None:
                     if isinstance(genconf.json_schema, str):
                         schema_dic = json.loads(genconf.json_schema)
                     else:
                         schema_dic = genconf.json_schema
                         
                     json_schema_validate(dic, schema_dic)
 
                 out = GenOut(res=GenRes.from_finish_reason(finish),
-                             text=text,
+                             text=str(response),
                              dic=dic)
             
-            except json.JSONDecodeError:
+            except json.JSONDecodeError as err:
                 out = GenOut(res=GenRes.from_finish_reason("!json"),
-                             text=text)
+                             text=f"'{err}' {response}")
                 
             except json_schema_ValidationError as err:
                 logger.info(f"JSON schema validation error: {err.message}")
                 out = GenOut(res=GenRes.from_finish_reason("!json_schema_val"),
-                             text=text,
+                             text=f"'{err.message}' {response}",
                              dic=dic)
                 
             except json_schema_SchemaError as err:
                 logger.info(f"JSON schema error: {err.message}")
                 out = GenOut(res=GenRes.from_finish_reason("!json_schema_error"),
-                             text=text,
+                             text=f"'{err.message}' {response}",
                              dic=dic)
 
         else:
+            if isinstance(response, str):
+                response = response.strip()
+            else:
+                response = str(response)
+
             out = GenOut(res=GenRes.from_finish_reason(finish),
-                         text=text)
+                         text=response)
             
        
         return out
```

### Comparing `sibila-0.4.0/sibila/models.py` & `sibila-0.4.1/sibila/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,45 +160,50 @@
 
     genconf: Union[GenConf,None] = None
     """Default GenConf for created models."""
 
     ENV_VAR_NAME = "SIBILA_MODELS"
 
     PROVIDER_CONF = {
-        "llamacpp": {
-            "mandatory": ["name"],
-            "flags": ["name_passthrough", "local"]
+        "anthropic": {
+            "mandatory": [],
+            "flags": ["name_passthrough"]
         },
-        "openai": {
+        "fireworks": {
             "mandatory": [],
             "flags": ["name_passthrough"]
         },
-        "together": {
+        "llamacpp": {
+            "mandatory": ["name"],
+            "flags": ["name_passthrough", "local"]
+        },
+        "mistral": {
             "mandatory": [],
             "flags": ["name_passthrough"]
         },
-        "fireworks": {
+        "openai": {
             "mandatory": [],
             "flags": ["name_passthrough"]
         },
-        "mistral": {
+        "together": {
             "mandatory": [],
             "flags": ["name_passthrough"]
         },
     }
     ALL_PROVIDER_NAMES = list(PROVIDER_CONF.keys()) + ["alias"] # providers + "alias"
 
     @classmethod
     def EMPTY_MODELS_DIR(_) -> dict:
         return {
+            "anthropic": {},
+            "fireworks": {},
             "llamacpp": {},
+            "mistral": {},
             "openai": {},
             "together": {},
-            "fireworks": {},
-            "mistral": {},
             "alias": {},
         }
 
     MODELS_CONF_FILENAME = "models.json"
     MODELS_BASE_CONF_FILENAME = "base_" + MODELS_CONF_FILENAME
 
     DEFAULT_ENTRY_NAME = "_default"
@@ -362,15 +367,25 @@
             args["ctx_len"] = ctx_len
 
 
         logger.debug(f"Resolved '{res_name}' to '{provider}:{name}' with args: {args}")
 
 
         model: Model
-        if provider == "llamacpp":
+        if provider == "anthropic":
+
+            from .anthropic import AnthropicModel
+            model = AnthropicModel(**args)
+            
+        elif provider == "fireworks":
+
+            from .schema_format_openai import FireworksModel
+            model = FireworksModel(**args)
+            
+        elif provider == "llamacpp":
 
             # resolve filename -> path
             path = cls._locate_file(args["name"])
             if path is None:
                 path = args["name"] # LlamaCppModel should raise the exception, not us
             else:
                 logger.debug(f"Resolved llamacpp model '{args['name']}' to '{path}'")
@@ -378,40 +393,30 @@
             # rename "name" -> "path" which LlamaCppModel is expecting
             del args["name"]
             args["path"] = path
                         
             from .llamacpp import LlamaCppModel
 
             model = LlamaCppModel(**args)
-
         
+        elif provider == "mistral":
+
+            from .mistral import MistralModel
+            model = MistralModel(**args)
+            
         elif provider == "openai":
 
             from .openai import OpenAIModel
-                    
             model = OpenAIModel(**args)
             
         elif provider == "together":
 
             from .schema_format_openai import TogetherModel
-                    
             model = TogetherModel(**args)
             
-        elif provider == "fireworks":
-
-            from .schema_format_openai import FireworksModel
-                    
-            model = FireworksModel(**args)
-            
-        elif provider == "mistral":
-
-            from .mistral import MistralModel
-                    
-            model = MistralModel(**args)
-            
         """
         elif provider == "hf":
             from .hf import HFModel
             
             model = HFModel(**args)
         """
            
@@ -1207,17 +1212,21 @@
             return
             
         # model and format dirs
         cls.models_dir = cls.EMPTY_MODELS_DIR()
         cls.formats_dir = cls.EMPTY_FORMATS_DIR()
 
         if add_cwd:
-            # add "." to search path, so that paths relative paths work
-            cls.add_models_search_path(".")
-
+            # add CWD to search path, so that relative paths work
+            try: # try but don't add a deleted dir
+                cwd_path = os.getcwd()
+                if os.path.isdir(cwd_path):
+                    cls.add_models_search_path(cwd_path)
+            except FileNotFoundError:
+                ...
 
         path: Union[str, None]
 
         cls.base_models_dir = cls.EMPTY_MODELS_DIR()
         cls.base_formats_dir = cls.EMPTY_FORMATS_DIR()
 
         # read base_models.json from res folder
```

### Comparing `sibila-0.4.0/sibila/multigen.py` & `sibila-0.4.1/sibila/multigen.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.0/sibila/null.py` & `sibila-0.4.1/sibila/null.py`

 * *Files 18% similar despite different names*

```diff
@@ -94,13 +94,22 @@
 
     def token_len(self,
                   thread_or_text: Union[Thread,str],
                   _: Optional[GenConf] = None) -> int:
         assert False, "NullModel won't use tokens"
 
 
+
+    def name(self) -> str:
+        """Model (short) name."""
+        return 'null_model'
+    
+    def desc(self) -> str:
+        """Model description."""
+        return f"{type(self).__name__}: {self.name}"
+
     @classmethod
     def provider_version(_) -> str:
         """Provider library version: provider x.y.z
         Ex. openai 1.3.6
         """
         return "NullModel 0.0.0"
```

### Comparing `sibila-0.4.0/sibila/openai.py` & `sibila-0.4.1/sibila/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,14 @@
 class OpenAIModel(MessagesModel):
     """Access an OpenAI model.
 
     Supports constrained JSON output, via the OpenAI API tools mechanism.
 
     Ref:
         https://platform.openai.com/docs/api-reference/chat/create
-
-    Attributes:
-        ctx_len: Maximum context length.
-        desc: Model information.
     """
 
     PROVIDER_NAME:str = "openai"
     """Provider prefix that this class handles."""
 
     _token_estimation_factor: float
     """Multiplication factor to estimate token usage: multiplies text length to obtain token length."""
@@ -181,15 +177,15 @@
         self.max_tokens_limit = min(self.max_tokens_limit, self.ctx_len)
 
         self._overhead_per_msg = overhead_per_msg or default_overhead_per_msg
 
         self._token_estimation_factor = token_estimation_factor or default_token_estimation_factor
 
 
-        # only check for "json" text presence as json schema is requested with the tools facility.
+        # only check for "json" text presence as json schema (including field descriptions) is requested with the tools facility.
         self.json_format_instructors["json_schema"] = self.json_format_instructors["json"]
 
 
         if self.tokenizer is None and create_tokenizer:
             try:
                 self.tokenizer = OpenAITokenizer(self._model_name)
             except Exception as e:
@@ -246,41 +242,39 @@
             genconf = self.genconf
 
         thread = self._prepare_gen_thread(thread, genconf)
 
         token_len = self.token_len(thread, genconf)
         resolved_max_tokens = self.resolve_genconf_max_tokens(token_len, genconf)
 
-        # for reference: this is a bad idea as endpoint will error on larger than possible max_tokens:
+        # for reference: next commented-out line is a bad idea, as endpoint will error if max_tokens is greater than limit:
         # resolved_max_tokens = self.resolve_genconf_max_tokens(0, genconf)
 
-        fn_name = "json_out"
-
         json_kwargs: dict = {}
         if genconf.format == "json":
             
             json_kwargs["response_format"] = {"type": "json_object"}
 
             if genconf.json_schema is not None:
                 # use json_schema in OpenAi's tool API
                 json_kwargs["tool_choice"] = {
                     "type": "function",
-                    "function": {"name": fn_name},
+                    "function": {"name": self.output_fn_name},
                 }
 
                 if isinstance(genconf.json_schema, str):
                     params = json.loads(genconf.json_schema)
                 else:
                     params = genconf.json_schema
                 
                 json_kwargs["tools"] = [
                     {
                         "type": "function",
                         "function": {
-                            "name": fn_name,
+                            "name": self.output_fn_name,
                             "parameters": params
                         }
                     }
                 ]
 
         # seed config is disabled, remote models and some hardware accelerated local models don't support it.
         # seed = genconf.seed
@@ -302,23 +296,20 @@
                   **json_kwargs}
 
         # inject model-specific args, if any
         kwargs.update(genconf.resolve_special(self.PROVIDER_NAME))
 
         logger.debug(f"{type(self).__name__} gen args: {kwargs}")
 
-        return (kwargs,
-                fn_name,
-                genconf)
+        return (kwargs, genconf)
         
 
     def _gen_post(self, 
                   response: Any,
                   pre_kwargs: dict,
-                  fn_name: str,
                   genconf: GenConf
                   ) -> GenOut:
             
         logger.debug(f"OpenAI response: {response}")
 
         choice = response.choices[0]
         finish = choice.finish_reason
@@ -330,16 +321,16 @@
             
             # json schema generation via the tools API:
             if message.tool_calls is not None:
                 if len(message.tool_calls) != 1:
                     logger.warn(f"OpenAIModel: expecting single message.tool_calls, but received {len(message.tool_calls)} - using first.")
 
                 fn = message.tool_calls[0].function
-                if fn.name != fn_name:
-                    logger.warn(f"OpenAIModel: expecting '{fn_name}' function name, received ({fn.name})")
+                if fn.name != self.output_fn_name:
+                    logger.warn(f"OpenAIModel: expecting '{self.output_fn_name}' function name, received ({fn.name})")
 
                 text = fn.arguments
 
             else: # use content instead
                 logger.warn("OpenAIModel: expecting message.tool_calls, but none received - using text content")
                 text = message.content # type: ignore[assignment]
         
@@ -372,29 +363,28 @@
 
         Returns:
             A GenOut object with result, generated text, etc.
             The output text is in GenOut.text.
         """
 
         genconf2: GenConf
-        kwargs, fn_name, genconf2 = self._gen_pre(thread, genconf)
+        kwargs, genconf2 = self._gen_pre(thread, genconf)
 
         self._ensure_client(False)
 
         try:
             # https://platform.openai.com/docs/api-reference/chat/create
             response = self._client.chat.completions.create(**kwargs) # type: ignore[attr-defined]
 
         except Exception as e:
             raise RuntimeError(f"Cannot generate. Internal error: {e}")
 
 
         return self._gen_post(response,
                               kwargs,
-                              fn_name,
                               genconf2)
     
 
 
 
     async def gen_async(self, 
                         thread: Thread,
@@ -412,28 +402,27 @@
 
         Returns:
             A GenOut object with result, generated text, etc.
             The output text is in GenOut.text.
         """
 
         genconf2: GenConf
-        kwargs, fn_name, genconf2 = self._gen_pre(thread, genconf)
+        kwargs, genconf2 = self._gen_pre(thread, genconf)
 
         self._ensure_client(True)
 
         try:
             # https://platform.openai.com/docs/api-reference/chat/create
             response = await self._client_async.chat.completions.create(**kwargs) # type: ignore[attr-defined]
 
         except Exception as e:
             raise RuntimeError(f"Cannot generate. Internal error: {e}")
 
         return self._gen_post(response,
                               kwargs,
-                              fn_name,
                               genconf2)
     
 
    
 
 
 
@@ -482,15 +471,14 @@
                 else:
                     js_str = json.dumps(genconf.json_schema)
 
                 tools_num_tokens = len(js_str) * self._token_estimation_factor
                 num_tokens += int(tools_num_tokens)
                 # print("tools_num_tokens", tools_num_tokens)
 
-
         else: # do an "informed" token estimation from what is known of the OpenAI model's tokenization
             
             for index in range(-1, len(thread)): # -1 for system message
                 message = thread.msg_as_chatml(index)
                 # print(message)
                 num_tokens += self._overhead_per_msg
                 for key, value in message.items():
@@ -518,16 +506,43 @@
                 num_tokens += tools_num_tokens
 
         
         return num_tokens
 
 
 
+    @classmethod
+    def known_models(cls,
+                     api_key: Optional[str] = None) -> Union[list[str], None]:
+        """List of model names that can be used. Some of the models are not chat models and cannot be used,
+        for example embedding models.
+        
+        Args:
+            api_key: Requires OpenAI API key, passed as this arg or set in env variable OPENAI_API_KEY.
+
+        Returns:
+            Returns a list of known models.
+        """
+ 
+        client = openai.OpenAI(api_key=api_key)
+        model_list = client.models.list()
+
+        out = []
+        for model in model_list.data:
+            out.append(model.id)
+        return sorted(out)
+
+
+
+
+
+    def name(self) -> str:
+        """Model (short) name."""
+        return self._model_name
     
-    @property
     def desc(self) -> str:
         """Model description."""
         return f"{type(self).__name__}: '{self._model_name}'"
 
 
     @classmethod
     def provider_version(_) -> str:
@@ -539,34 +554,16 @@
             ver = openai.__version__
         except Exception:
             raise ImportError("Please install openai by running: pip install openai")
             
         return f"openai {ver}"
     
     
-    @classmethod
-    def known_models(cls,
-                     api_key: Optional[str] = None) -> Union[list[str], None]:
-        """List of model names that can be used. Some of the models are not chat models and cannot be used,
-        for example embedding models.
-        
-        Args:
-            api_key: Requires OpenAI API key, passed as this arg or set in env variable OPENAI_API_KEY.
 
-        Returns:
-            Returns a list of known models.
-        """
- 
-        client = openai.OpenAI(api_key=api_key)
-        model_list = client.models.list()
 
-        out = []
-        for model in model_list.data:
-            out.append(model.id)
-        return sorted(out)
 
 
 
 
 
 
 class OpenAITokenizer(Tokenizer):
```

### Comparing `sibila-0.4.0/sibila/res/base_formats.json` & `sibila-0.4.1/sibila/res/base_formats.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.825%*

 * *Differences: {"'command-r'": 'OrderedDict([(\'match\', \'c4ai-command-r\'), (\'template\', "{{ bos_token }}{% '*

 * *                "if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set "*

 * *                "system_message = messages[0]['content'] %}{% else %}{% set loop_messages = "*

 * *                'messages %}{% set system_message = false %}{% endif %}{% if system_message != '*

 * *                "false %}{{ '<|START_OF_TURN_TOKEN|><|SYSTEM_TOKEN|>' + system_message + "*

 * *                "'<|END_OF_TUR […]*

```diff
@@ -5,14 +5,18 @@
     "amber": {
         "match": "amberchat",
         "template": "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'].strip() + '\n' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if loop.index0 == 0 %}{{ bos_token + system_message }}{% endif %}{% if message['role'] == 'user' %}{{ '### Human: ' + message['content'].strip() + '\n' }}{% elif message['role'] == 'assistant' %}{{ '### Assistant: ' + message['content'].strip() + '\n' }}{% endif %}{% endfor %}{% if add_generation_prompt %}{{ '### Assistant:' }}{% endif %}"
     },
     "chatml": {
         "template": "{% for message in messages %}{{'<|im_start|>' + message['role'] + '\n' + message['content'].strip() + '<|im_end|>' + '\n'}}{% endfor %}{% if add_generation_prompt %}{{ '<|im_start|>assistant\n' }}{% endif %}"
     },
+    "command-r": {
+        "match": "c4ai-command-r",
+        "template": "{{ bos_token }}{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'] %}{% else %}{% set loop_messages = messages %}{% set system_message = false %}{% endif %}{% if system_message != false %}{{ '<|START_OF_TURN_TOKEN|><|SYSTEM_TOKEN|>' + system_message + '<|END_OF_TURN_TOKEN|>' }}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant...') }}{% endif %}{% set content = message['content'] %}{% if message['role'] == 'user' %}{{ '<|START_OF_TURN_TOKEN|><|USER_TOKEN|>' + content.strip() + '<|END_OF_TURN_TOKEN|>' }}{% elif message['role'] == 'assistant' %}{{ '<|START_OF_TURN_TOKEN|><|CHATBOT_TOKEN|>'  + content.strip() + '<|END_OF_TURN_TOKEN|>' }}{% endif %}{% endfor %}{% if add_generation_prompt %}{{ '<|START_OF_TURN_TOKEN|><|CHATBOT_TOKEN|>' }}{% endif %}"
+    },
     "dolphin": {
         "match": "dolphin-2",
         "template": "chatml"
     },
     "dolphin-phi2": {
         "match": "dolphin.+phi-2",
         "template": "chatml"
@@ -33,19 +37,22 @@
         "match": "hermes-",
         "template": "alpaca"
     },
     "hermes2": {
         "match": "hermes-[^1]",
         "template": "chatml"
     },
-    "llama": "llama2",
     "llama2": {
-        "match": "llama.+chat",
+        "match": "llama-2.+chat",
         "template": "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = '<<SYS>>\n' + messages[0]['content'].strip() + '\n<</SYS>>\n\n' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if loop.index0 == 0 %}{% set content = system_message + message['content'] %}{% else %}{% set content = message['content'] %}{% endif %}{% if message['role'] == 'user' %}{{ bos_token + '[INST] ' + content.strip() + ' [/INST]' }}{% elif message['role'] == 'assistant' %}{{ ' '  + content.strip() + ' ' + eos_token }}{% endif %}{% endfor %}"
     },
+    "llama3": {
+        "match": "llama-3.+instruct",
+        "template": "{{ bos_token }}{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = '<|start_header_id|>' + 'system' + '<|end_header_id|>\n\n' + messages[0]['content'].strip() + '<|eot_id|>' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if loop.index0 == 0 %}{{ system_message }}{% endif %}{{ '<|start_header_id|>' + message['role'] + '<|end_header_id|>\n\n' + message['content'].strip() + '<|eot_id|>' }}{% if loop.last and message['role'] == 'user' and add_generation_prompt %}{{ '<|start_header_id|>' + 'assistant' + '<|end_header_id|>\n\n' }}{% endif %}{% endfor %}"
+    },
     "mistral": {
         "match": "mistral.+instruct",
         "template": "{{ bos_token }}{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'].strip() + '\n\n' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if loop.index0 == 0 %}{% set content = system_message + message['content'] %}{% else %}{% set content = message['content'] %}{% endif %}{% if message['role'] == 'user' %}{{ '[INST] ' + content.strip() + ' [/INST]' }}{% elif message['role'] == 'assistant' %}{{ content.strip() + eos_token}}{% endif %}{% endfor %}"
     },
     "mixtral": {
         "match": "mixtral.+instruct",
         "template": "mistral"
@@ -62,22 +69,34 @@
         "match": "orca.2",
         "template": "chatml"
     },
     "phi2": {
         "match": "phi-2",
         "template": "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'].strip() + '\n\n' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if loop.index0 == 0 %}{% set content = system_message + message['content'] %}{% else %}{% set content = message['content'] %}{% endif %}{% if message['role'] == 'user' %}{{ 'Instruct: ' + content.strip() + '\n' }}{% elif message['role'] == 'assistant' %}{{ 'Output: '  + content.strip() + '\n' }}{% endif %}{% endfor %}{% if add_generation_prompt %}{{ 'Output:' }}{% endif %}"
     },
+    "phi3": {
+        "match": "phi-3.+instruct",
+        "template": "{{ bos_token }}{% for message in messages %}{% if (message['role'] == 'system') %}{{'<|system|>' + '\n' + message['content'] + '<|end|>' + '\n'}}{% elif (message['role'] == 'user') %}{{'<|user|>' + '\n' + message['content'] + '<|end|>' + '\n' + '<|assistant|>' + '\n'}}{% elif message['role'] == 'assistant' %}{{message['content'] + '<|end|>' + '\n'}}{% endif %}{% endfor %}"
+    },
     "qwen": {
         "match": "qwen.+chat",
         "template": "{% for message in messages %}{% if loop.first and messages[0]['role'] != 'system' %}{{ '<|im_start|>system\nYou are a helpful assistant<|im_end|>\n' }}{% endif %}{{'<|im_start|>' + message['role'] + '\n' + message['content'].strip() }}{% if (loop.last and add_generation_prompt) or not loop.last %}{{ '<|im_end|>' + '\n'}}{% endif %}{% endfor %}{% if add_generation_prompt and messages[-1]['role'] != 'assistant' %}{{ '<|im_start|>assistant\n' }}{% endif %}"
     },
+    "rocket": {
+        "match": "rocket.3b",
+        "template": "chatml"
+    },
     "solar-instruct": {
         "match": "solar.+instruct",
         "template": "{% for message in messages %}{% if message['role'] == 'system' %}{% if message['content']%}{{'### System:\n' + message['content'].strip() +'\n\n'}}{% endif %}{% elif message['role'] == 'user' %}{{'### User:\n' + message['content'].strip() +'\n\n'}}{% elif message['role'] == 'assistant' %}{{'### Assistant:\n'  + message['content'].strip() +'\n\n' }}{% endif %}{% if loop.last and add_generation_prompt %}{{ '### Assistant:\n' }}{% endif %}{% endfor %}"
     },
+    "stablelm2": {
+        "match": "stablelm-2.+chat",
+        "template": "chatml"
+    },
     "starling": {
         "match": "starling.lm",
         "template": "openchat"
     },
     "tinydolphin": {
         "match": "tinydolphin",
         "template": "chatml"
```

### Comparing `sibila-0.4.0/sibila/res/base_models.json` & `sibila-0.4.1/sibila/res/base_models.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8253968253968255%*

 * *Differences: {"'anthropic'": "OrderedDict([('_default', OrderedDict([('ctx_len', 200000), ('max_tokens_limit', "*

 * *                "4096), ('token_estimation_factor', 0.4)]))])",*

 * * "'openai'": "{'gpt-4-turbo-2024-04-09': OrderedDict([('ctx_len', 128000)]), 'gpt-4-turbo': "*

 * *             "'gpt-4-turbo-2024-04-09'}"}*

```diff
@@ -1,8 +1,15 @@
 {
+    "anthropic": {
+        "_default": {
+            "ctx_len": 200000,
+            "max_tokens_limit": 4096,
+            "token_estimation_factor": 0.4
+        }
+    },
     "fireworks": {
         "_default": {
             "ctx_len": 4096,
             "token_estimation_factor": 0.4
         }
     },
     "llamacpp": {
@@ -62,14 +69,18 @@
         "gpt-4-32k": "gpt-4-32k-0613",
         "gpt-4-32k-0314": {
             "ctx_len": 32768
         },
         "gpt-4-32k-0613": {
             "ctx_len": 32768
         },
+        "gpt-4-turbo": "gpt-4-turbo-2024-04-09",
+        "gpt-4-turbo-2024-04-09": {
+            "ctx_len": 128000
+        },
         "gpt-4-turbo-preview": "gpt-4-0125-preview"
     },
     "together": {
         "_default": {
             "ctx_len": 4096,
             "token_estimation_factor": 0.4
         }
```

### Comparing `sibila-0.4.0/sibila/schema_format_openai.py` & `sibila-0.4.1/sibila/schema_format_openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,18 +43,14 @@
     has_openai = False
     
 
 
 
 class SchemaFormatOpenAIModel(OpenAIModel):
     """Access a model that allows JSON Schema passed in response_format.
-
-    Attributes:
-        ctx_len: Maximum context length.
-        desc: Model information.
     """
 
     PROVIDER_NAME:str = "to be set by derived class"
     """Provider prefix that this class handles."""
 
     _token_estimation_factor: float
     """Multiplication factor to estimate token usage: multiplies text length to obtain token length."""
@@ -175,23 +171,20 @@
                   **json_kwargs}
 
         # inject model-specific args, if any
         kwargs.update(genconf.resolve_special(self.PROVIDER_NAME))
 
         logger.debug(f"{type(self).__name__} gen args: {kwargs}")
 
-        return (kwargs,
-                "__unused",
-                genconf)
+        return (kwargs, genconf)
         
 
     def _gen_post(self, 
                   response: Any,
                   pre_kwargs: dict,
-                  fn_name: str,
                   genconf: GenConf
                   ) -> GenOut:
             
         logger.debug(f"SchemaFormatOpenAIModel response: {response}")
 
         choice = response.choices[0]
         finish = choice.finish_reason
@@ -231,18 +224,14 @@
     """Access a together.ai model with the OpenAI API.
     Supports constrained JSON output, via the response_format JSON Schema mechanism.
 
     Ref:
         https://docs.together.ai/docs/json-mode
         
         https://docs.together.ai/reference/chat-completions
-
-    Attributes:
-        ctx_len: Maximum context length.
-        desc: Model information.
     """
 
     PROVIDER_NAME:str = "together"
     """Provider prefix that this class handles."""
 
     DEFAULT_BASE_URL: str = "https://api.together.xyz/v1"
     """Default API access URL"""
@@ -328,18 +317,14 @@
     """Access a Fireworks AI model with the OpenAI API.
     Supports constrained JSON output, via the response_format JSON Schema mechanism.
 
     Ref:
         https://readme.fireworks.ai/docs/structured-response-formatting
 
         https://readme.fireworks.ai/reference/createchatcompletion
-
-    Attributes:
-        ctx_len: Maximum context length.
-        desc: Model information.
     """
 
     PROVIDER_NAME:str = "fireworks"
     """Provider prefix that this class handles."""
 
     DEFAULT_BASE_URL: str = "https://api.fireworks.ai/inference/v1"
     """Default API access URL"""
```

### Comparing `sibila-0.4.0/sibila/text_splitter.py` & `sibila-0.4.1/sibila/text_splitter.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.0/sibila/thread.py` & `sibila-0.4.1/sibila/thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,24 +464,25 @@
 
         kind = Thread._kind_from_pos(index)
         role = MsgKind.chatml_role_from_kind(kind)
         text = self._msgs[index] if index >= 0 else self.inst
         return {"role": role, "content": text}
     
 
-    def as_chatml(self) -> list[dict]:
+    def as_chatml(self,
+                  include_INST: bool = True) -> list[dict]:
         """Returns Thread as a list of ChatML messages.
 
         Returns:
             A list of ChatML dict elements with "role" and "content" keys.
         """
         msgs = []
 
         for index,msg in enumerate(self._msgs):
-            if index == 0 and self.inst:
+            if index == 0 and self.inst and include_INST:
                 msgs.append(self.msg_as_chatml(-1))
             msgs.append(self.msg_as_chatml(index))
             
         return msgs
 
 
     def has_text_lower(self,
```

### Comparing `sibila-0.4.0/sibila/tools.py` & `sibila-0.4.1/sibila/tools.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.0/sibila/utils.py` & `sibila-0.4.1/sibila/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,13 +35,13 @@
         name = name.replace("_", " ").capitalize()
 
     return name
 
 
 
 def expand_path(path: str) -> str:
-    if '~' in path:
+    if path.startswith("~"):
         path = os.path.expanduser(path)
 
     path = os.path.abspath(path)
     path = os.path.normpath(path) # normalize absolute path
     return path
```

### Comparing `sibila-0.4.0/sibila.egg-info/PKG-INFO` & `sibila-0.4.1/sibila.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sibila
-Version: 0.4.0
+Version: 0.4.1
 Summary: Structured queries from local or online LLM models
 Author-email: Jorge Diogo <jndiogo@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jndiogo/sibila
 Project-URL: Documentation, https://jndiogo.github.io/sibila
 Project-URL: Issues, https://github.com/jndiogo/sibila/issues
 Keywords: llama.cpp,AI,Transformers,GPT,LLM
@@ -19,29 +19,32 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: llama-cpp-python>=0.2
 Requires-Dist: openai>=1.1
 Requires-Dist: tiktoken
+Requires-Dist: anthropic
 Requires-Dist: mistralai
 Requires-Dist: jinja2>=3.0
 Requires-Dist: jsonschema
 Requires-Dist: pydantic>=2.0
 Requires-Dist: typing_extensions
 Requires-Dist: tqdm
+Requires-Dist: pytest-asyncio>=0.17
 
 # Sibila
 
-Extract structured data from remote or local LLM models. Predictable output is essential for any serious use of LLMs.
+Extract structured data from remote or local LLM models. Predictable output is important for serious use of LLMs.
 
-- Extract data into Pydantic objects, dataclasses or simple types.
-- Same API for local file models and remote OpenAI, Mistral AI and other models.
+- Query structured data into Pydantic objects, dataclasses or simple types.
+- Access remote models from OpenAI, Anthropic, Mistral AI and other providers.
+- Use local models like Llama-3, Phi-3, OpenChat or any other GGUF file model.
+- Besides structured extraction, Sibila is also a general purpose model access library, to generate plain text or free JSON results, with the same API for local and remote models.
 - Model management: download models, manage configuration, quickly switch between models.
-- Tools for evaluating output across local/remote models, for chat-like interaction and more.
 
 No matter how well you craft a prompt begging a model for the output you need, it can always respond something else. Extracting structured data can be a big step into getting predictable behavior from your models.
 
 See [What can you do with Sibila?](https://jndiogo.github.io/sibila/what/)
 
 To extract structured data from a local model:
 
@@ -67,15 +70,15 @@
 Info(event_year=1969,
      first_name='Neil',
      last_name='Armstrong',
      age_at_the_time=38,
      nationality='American')
 ```
 
-Or to use OpenAI's GPT-4, we would simply replace the model's name:
+Or to use a remote model like OpenAI's GPT-4, we would simply replace the model's name:
 
 ``` python
 model = Models.create("openai:gpt-4")
 
 model.extract(Info, "Who was the first man in the moon?")
 ```
```

### Comparing `sibila-0.4.0/sibila.egg-info/SOURCES.txt` & `sibila-0.4.1/sibila.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 sibila/__init__.py
+sibila/anthropic.py
 sibila/cli.py
 sibila/context.py
 sibila/gen.py
 sibila/json_grammar.py
 sibila/json_schema.py
 sibila/llamacpp.py
 sibila/mistral.py
@@ -24,19 +25,24 @@
 sibila.egg-info/dependency_links.txt
 sibila.egg-info/entry_points.txt
 sibila.egg-info/requires.txt
 sibila.egg-info/top_level.txt
 sibila/res/__init__.py
 sibila/res/base_formats.json
 sibila/res/base_models.json
+tests/test_anthropic_claude-3-haiku.py
 tests/test_cli.py
+tests/test_common_llamacpp.py
+tests/test_common_llamacpp_examples.py
+tests/test_common_remote.py
+tests/test_common_remote_examples.py
 tests/test_examples_tinyllama.py
 tests/test_fireworks_mixtral.py
 tests/test_formats.py
 tests/test_json_schema.py
-tests/test_llamacpp_models.py
+tests/test_llamacpp_models_dir.py
 tests/test_llamacpp_tinyllama.py
-tests/test_mistral_small.py
+tests/test_mixtral_mistral_small.py
 tests/test_null_extract.py
 tests/test_openai_gpt35.py
 tests/test_openai_gpt4.py
 tests/test_together_mixtral.py
```

### Comparing `sibila-0.4.0/tests/test_cli.py` & `sibila-0.4.1/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,14 @@
 
     teardown_env_models(base_dir)
     
 
 
 
 
-
-
 def test_models(env):
 
     models_path = os.path.join(env[1], Models.MODELS_CONF_FILENAME)
 
     cmd = "sibila models -m models/ -s llamacpp:local-model local-model.gguf"
     run_json(cmd, 
              path=models_path,
@@ -156,15 +154,14 @@
     run_json(cmd, 
              path=models_path,
              expected_json={})
 
 
 
 
-
 def test_formats(env):
 
     formats_path = os.path.join(env[1], Models.FORMATS_CONF_FILENAME)
 
     cmd = """sibila formats -m models -s test-format "{% for message in messages %}{{'<|im_start|>' + message['role'] + '\n' + message['content'] + '<|im_end|>' + '\n'}}{% endfor %}{% if add_generation_prompt %}{{ '<|im_start|>assistant \n' }}{% endif %}" """
     run_json(cmd, 
              path=formats_path,
```

### Comparing `sibila-0.4.0/tests/test_examples_tinyllama.py` & `sibila-0.4.1/tests/test_examples_tinyllama.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,21 +302,21 @@
 def test_tag(env_model):
 
     model = env_model[2]
 
     queries = """\
 1. Do you offer a trial period for your software before purchasing?
 2. I'm experiencing a glitch with your app, it keeps freezing after the latest update.
-3. What are the different pricing plans available for your subscription service?"
-4. Can you provide instructions on how to reset my account password?"
-5. I'm unsure about the compatibility of your product with my device, can you advise?"
-6. How can I track my recent order and estimate its delivery date?"
-7. Is there a customer loyalty program or rewards system for frequent buyers?"
-8. I'm interested in your online courses, but do you offer refunds if I'm not satisfied?"
-9. Could you clarify the coverage and limitations of your product warranty?"
+3. What are the different pricing plans available for your subscription service?
+4. Can you provide instructions on how to reset my account password?
+5. I'm unsure about the compatibility of your product with my device, can you advise?
+6. How can I track my recent order and estimate its delivery date?
+7. Is there a customer loyalty program or rewards system for frequent buyers?
+8. I'm interested in your online courses, but do you offer refunds if I'm not satisfied?
+9. Could you clarify the coverage and limitations of your product warranty?
 10. What are your customer support hours and how can I reach your team in case of emergencies?
 """
 
 
     from enum import Enum
     from dataclasses import dataclass
```

### Comparing `sibila-0.4.0/tests/test_fireworks_mixtral.py` & `sibila-0.4.1/tests/test_fireworks_mixtral.py`

 * *Files 27% similar despite different names*

```diff
@@ -177,123 +177,7 @@
     assert model.resolve_genconf_max_tokens(1900, genconf) == OUT_MAX_TOKENS - 1900
     
     with pytest.raises(ValueError):
         assert model.resolve_genconf_max_tokens(160*1000, genconf)
 
     del model
 
-
-
-
-
-
-def test_prompt(env_model):
-
-    PROMPT = "Tell me briefly about oranges"
-    HAS = "orange"
-
-    model = create_model()
-    text = model(PROMPT)
-    print(text)
-    assert HAS in text.lower()
-    del model
-
-
-
-
-
-
-INT_PROMPT = "extract the number from the following text: there are twelve bananas"
-TRUE_PROMPT = "extract True/False from the following text: Yes I got it!"
-CTX_LEN = 200
-
-
-def test_extract(env_model):
-
-    model = create_model(ctx_len=CTX_LEN)
-
-    res = model.extract(int, INT_PROMPT)
-    assert res == 12
-
-    res = model.extract(bool, TRUE_PROMPT)
-    assert res == True
-
-    del model
-
-
-
-
-
-def test_extract_async1(env_model):
-
-    model = create_model(ctx_len=CTX_LEN)
-
-    async def run_async():
-        print("run_async begin")
-
-        res = await model.extract_async(int, INT_PROMPT)
-        assert res == 12
-
-        res = await model.extract_async(bool, TRUE_PROMPT)
-        assert res == True
-        print("run_async done")
-        
-    asyncio.run(run_async())
-
-
-
-
-def test_extract_async2(env_model):
-
-    model = create_model(ctx_len=CTX_LEN)
-
-    async def run1_async():        
-        print("run1 begin")
-        res = await model.extract_async(int, INT_PROMPT)
-        assert res == 12
-        print("run1 done")
-
-    async def run2_async():
-        print("run2 begin")
-        res = await model.extract_async(bool, TRUE_PROMPT)
-        assert res == True
-        print("run2 done")
-
-
-    async def gather():
-        print("gather begin")
-        tasks = [run1_async(), run2_async()]
-        await asyncio.gather(*tasks)
-        print("gather done")
-            
-    asyncio.run(gather())    
-
-
-
-def test_extract_async3(env_model):
-
-    model = create_model(ctx_len=CTX_LEN)
-
-    async def run1_async():        
-        print("run1 begin")
-        res = await model.extract_async(int, INT_PROMPT)
-        assert res == 12
-        print("run1 done")
-
-    async def run2_async():
-        print("run2 begin")
-        res = await model.extract_async(bool, TRUE_PROMPT)
-        assert res == True
-        print("run2 done")
-
-
-    async def as_completed():
-        print("as_complete begin")
-        tasks = [run1_async(), run2_async()]
-        for task in asyncio.as_completed(tasks):
-            await task
-        print("as_complete done")
-            
-    asyncio.run(as_completed())    
-
-
-
```

### Comparing `sibila-0.4.0/tests/test_formats.py` & `sibila-0.4.1/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.0/tests/test_json_schema.py` & `sibila-0.4.1/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.0/tests/test_llamacpp_models.py` & `sibila-0.4.1/tests/test_llamacpp_models_dir.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,39 +16,50 @@
 clear; pytest -s test_llamacpp_models.py --models_dir ../../models/
 """
 
 LIMIT = 9999
 
 @pytest.fixture(scope="module")
 def models_list(pytestconfig):
+
     models_dir = pytestconfig.getoption("models_dir")
+    if not models_dir:
+        models_dir = "res"
 
     if not os.path.isabs(models_dir):
         base_dir = os.path.dirname(__file__)
         models_dir = os.path.normpath(os.path.join(base_dir, models_dir))
 
-    print (models_dir)
-
-    file_list = os.listdir(models_dir)
-    # print(file_list)
+    print("models_dir:", models_dir)
 
     filenames = []
-    for filename in file_list:
-        if not filename.endswith(".gguf"):
-            continue
-        if filename.startswith("--"):
-            continue
-
-        path = os.path.join(models_dir, filename)
-        if not os.path.isfile(path):
-            continue
-        filenames.append(path)
 
-    # print(filenames)
-    return sorted(filenames[:LIMIT])
+    if os.path.isdir(models_dir):
+        file_list = os.listdir(models_dir)
+        # print(file_list)
+
+        for filename in file_list:
+            if not filename.endswith(".gguf"):
+                continue
+            if filename.startswith("--"):
+                continue
+
+            path = os.path.join(models_dir, filename)
+            if not os.path.isfile(path):
+                continue
+            filenames.append(path)
+
+        filenames = sorted(filenames[:LIMIT])
+
+    if not filenames:
+        print("No models found")
+    else:
+        print("Found models:", "\n".join(filenames), sep="\n")
+        
+    return filenames
 
 
 def test_extract(models_list):
     # print(models_list)
 
     IN = "The 7 seas"
     INST = "Extract the number from the text"
```

### Comparing `sibila-0.4.0/tests/test_llamacpp_tinyllama.py` & `sibila-0.4.1/tests/test_llamacpp_tinyllama.py`

 * *Files 6% similar despite different names*

```diff
@@ -259,15 +259,15 @@
 
 
 
 
 
 
 
-def test_extract_async(env_model):
+def test_extract_async1(env_model):
 
     rel_model_path = os.path.join("models", MODEL_FILENAME)
 
     model = LlamaCppModel(rel_model_path, format="zephyr")
 
     async def run_async():
         print("run_async begin")
@@ -311,7 +311,28 @@
         await asyncio.gather(*tasks)
         print("gather done")
             
     asyncio.run(gather())    
 
 
     del model
+
+
+
+
+
+
+async def test_extract_async2(env_model):
+
+    rel_model_path = os.path.join("models", MODEL_FILENAME)
+
+    model = LlamaCppModel(rel_model_path, format="zephyr")
+
+    print("run_async begin")
+
+    res = await model.extract_async(int, INT_PROMPT)
+    assert res == 12
+
+    res = await model.extract_async(bool, TRUE_PROMPT)
+    assert res == True
+    print("run_async done")
+
```

### Comparing `sibila-0.4.0/tests/test_null_extract.py` & `sibila-0.4.1/tests/test_null_extract.py`

 * *Files identical despite different names*

