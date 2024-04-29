# Comparing `tmp/simple_generation-0.3.1.tar.gz` & `tmp/simple_generation-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_generation-0.3.1.tar", max compression
+gzip compressed data, was "simple_generation-0.4.0.tar", max compression
```

## Comparing `simple_generation-0.3.1.tar` & `simple_generation-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0      590 2024-02-20 17:50:37.322749 simple_generation-0.3.1/LICENSE
--rw-r--r--   0        0        0    14325 2024-02-21 10:27:36.018790 simple_generation-0.3.1/README.md
--rw-r--r--   0        0        0      652 2024-02-26 18:00:41.716239 simple_generation-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      225 2024-02-20 17:50:37.334749 simple_generation-0.3.1/simple_generation/__init__.py
--rw-r--r--   0        0        0    20322 2024-02-26 17:32:40.336043 simple_generation-0.3.1/simple_generation/simple_generation.py
--rw-r--r--   0        0        0     4459 2024-02-20 17:50:37.334749 simple_generation-0.3.1/simple_generation/utils.py
--rw-r--r--   0        0        0    15324 1970-01-01 00:00:00.000000 simple_generation-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      590 2024-04-17 15:47:25.745257 simple_generation-0.4.0/LICENSE
+-rw-r--r--   0        0        0    15034 2024-04-29 15:27:22.505854 simple_generation-0.4.0/README.md
+-rw-r--r--   0        0        0      879 2024-04-29 15:28:02.993927 simple_generation-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      225 2024-04-17 15:47:26.249259 simple_generation-0.4.0/simple_generation/__init__.py
+-rw-r--r--   0        0        0    20455 2024-04-29 15:27:22.529854 simple_generation-0.4.0/simple_generation/simple_generation.py
+-rw-r--r--   0        0        0     4459 2024-04-17 15:47:26.253259 simple_generation-0.4.0/simple_generation/utils.py
+-rw-r--r--   0        0        0       36 2024-04-29 15:27:22.537854 simple_generation-0.4.0/simple_generation/vlm/__init__.py
+-rw-r--r--   0        0        0      211 2024-04-29 15:27:22.541854 simple_generation-0.4.0/simple_generation/vlm/config.py
+-rw-r--r--   0        0        0    13403 2024-04-29 15:27:22.541854 simple_generation-0.4.0/simple_generation/vlm/vlm.py
+-rw-r--r--   0        0        0    16103 1970-01-01 00:00:00.000000 simple_generation-0.4.0/PKG-INFO
```

### Comparing `simple_generation-0.3.1/LICENSE` & `simple_generation-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_generation-0.3.1/README.md` & `simple_generation-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/simple-generation.svg)](https://pypi.python.org/pypi/simple-generation)
 [![Documentation Status](https://readthedocs.org/projects/simple-generation/badge/?version=latest)](https://simple-generation.readthedocs.io/en/latest/?version=latest)
 [![downloads badge](https://pepy.tech/badge/simple-generation/month)](https://pepy.tech/project/simple-generation)
 
 # Simple Generation
 
-Simple Generation offers a minimal interface to run text generation with HuggingFace checkpoint.
-The core idea is to ship many neat features out of the box and avoid boilerplate.
+Simple Generation offers a minimal interface to run text generation with HuggingFace checkpoints.
+The core idea is to ship many neat features out of the box, avoiding boilerplate.
 
-This is mainly for personal use and simple hardware setups (ideally, single-node single- or multi-gpu).
+*Simplegen is mainly for personal use and simple hardware setups (ideally, single-node single- or multi-gpu). If you are looking for production-ready inference engine consider looking elsewhere :) )*
 
 Moreover, please note that **the library will apply some (sensible) defaults (on where to place models, generation configuration, and so on) which might not suit your use case** and should be edited accordingly. Please head to [defaults](#defaults) to see a list of things you should be aware of.
 
 Install:
 ```bash
 pip install simple-generation
 ```
 
-Or, install it from source with:
+If you want to use inference with Vision Language Models (VLMs) run:
 ```bash
-pip install git+https://github.com/MilaNLProc/simple-generation.git
+pip install simple-generation[vlm]
 ```
 
 ## Features
 
 - generate with any model that can be loaded with `AutoModelForCausalLM` or `AutoModelForSeq2SeqLM`
 - batched inference for speed (`batch_size=256`)
 - auto find the largest batch size fitting in your accelerator (`batch_size="auto"`, `starting_batch_size=512`)
@@ -32,14 +32,18 @@
 - load and attach LoRA weights (`lora_weights=...`)
 - chat templates for modern chat models (`apply_chat_template=True` in `__call__`)
 - carbon emission estimates using [codecarbon](https://mlco2.github.io/codecarbon/)
 - sparsity and fused kernels for speed with [optimum](https://huggingface.co/docs/optimum/main/en/index) (`use_bettertransformer=True`)
 - DDP for single-node, multi-gpu setups using [accelerate](https://github.com/huggingface/accelerate). See [Distributed Inference](#distributed-inference)
 - GUI for quick interaction with models using Gradio's [ChatInterface](https://www.gradio.app/guides/creating-a-chatbot-fast#customizing-your-chatbot). See [Chat Interface](#chat-interface)
 
+**Vision-Language Models**
+
+- all of the above for [LLaVA](https://huggingface.co/docs/transformers/main/en/model_doc/llava#overview), [IDEFICS](https://huggingface.co/docs/transformers/main/en/model_doc/idefics#overview), and [BLIP](https://huggingface.co/docs/transformers/main/en/model_doc/blip#overview). For an example look into `./examples/vlm`.
+
 **Loading a Model**
 
 ```python
 from simple_generation import SimpleGenerator
 model_name = "meta-llama/Llama-2-7b-chat-hf"
 generator = SimpleGenerator(model_name, load_in_8bit=True)
 ```
@@ -271,15 +275,14 @@
 >> 219s
 
 # two GPUs, DDP
 CUDA_VISIBLE_DEVICES=0,1 accelerate launch --num_processes 2 examples/inference.py
 >> 105s
 ```
 
-
 ## Defaults
 
 If not specified we set some sensible defaults. **Please note that they might not fit your use case.**
 
 **Default Generation Configuration**
 
 - If not specified otherwise, the library will use the generation configs listed below, **overriding the default config loaded from the specified model**.
@@ -294,15 +297,15 @@
     do_sample: bool = True  # set to False for greedy decoding
     temperature: float = 0.7
     top_p: float = 1.0
     top_k: int = 50
     num_return_sequences: int = 1
 ```
 
-- We set the tokenizer to use left padding. This is required for batched inference with `AutoModelForCausalLM` but should also be fine with any other `AutoModelForSeq2SeqLM` since we use attention masks.
+- We set the tokenizer to use left padding. This is required for batched inference with `AutoModelForCausalLM` but should also be fine with any other `AutoModelForSeq2SeqLM` since we use attention masks. It is also recommended for VLM batch generations. See [this issue](https://github.com/huggingface/transformers/issues/3021#issuecomment-1454266627) and [usage tips](https://huggingface.co/docs/transformers/model_doc/llava_next#usage-tips) for more details.
 
 ## Warning
 
 There seem to be instabilities while using 4bit quantization (not related to this library). Use it only if strictly necessary.
 
 ## Acknowledgments
```

### Comparing `simple_generation-0.3.1/simple_generation/simple_generation.py` & `simple_generation-0.4.0/simple_generation/simple_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,15 @@
             tokenizer_name_or_path if tokenizer_name_or_path else model_name_or_path
         )
         self.tokenizer = AutoTokenizer.from_pretrained(
             tokenizer_name, config=config, padding_side="left"
         )
 
         # padding_size="left" is required for autoregressive models, and should not make a difference for every other model as we use attention_masks. See: https://github.com/huggingface/transformers/issues/3021#issuecomment-1454266627 for a discussion on why left padding is needed on batched inference
+        # This is also relevant for VLM batched generation: https://huggingface.co/docs/transformers/model_doc/llava_next#usage-tips
         self.tokenizer.padding_side = "left"
 
         logger.debug("Setting off the deprecation warning for padding")
         # see https://github.com/huggingface/transformers/issues/22638
         # and monitor https://github.com/huggingface/transformers/pull/23742
         self.tokenizer.deprecation_warnings["Asking-to-pad-a-fast-tokenizer"] = True
```

### Comparing `simple_generation-0.3.1/simple_generation/utils.py` & `simple_generation-0.4.0/simple_generation/utils.py`

 * *Files identical despite different names*

### Comparing `simple_generation-0.3.1/PKG-INFO` & `simple_generation-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 Metadata-Version: 2.1
 Name: simple-generation
-Version: 0.3.1
+Version: 0.4.0
 Summary: A python package to run inference with HuggingFace checkpoints wrapping many convenient features.
 License: Apache Software License 2.0
 Author: Giuseppe Attanasio
 Author-email: giuseppeattanasio6@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: vlm
 Requires-Dist: accelerate (>=0.20.3)
 Requires-Dist: bitsandbytes (>=0.39.1)
 Requires-Dist: codecarbon (>=2.1.4)
 Requires-Dist: datasets (>=2.12.0)
 Requires-Dist: optimum (>=1.9.0)
 Requires-Dist: peft (>=0.3.0)
+Requires-Dist: pillow (>=10.3.0) ; extra == "vlm"
 Requires-Dist: pyopenssl (>=23.2.0)
 Requires-Dist: scipy (>=1.10.1)
 Requires-Dist: tokenizers (>=0.13.3)
-Requires-Dist: transformers (>=4.30.2)
+Requires-Dist: transformers (>=4.39.3)
 Description-Content-Type: text/markdown
 
 ![Simple Generation Dining](/docs/_static/banner.png)
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/simple-generation.svg)](https://pypi.python.org/pypi/simple-generation)
 [![Documentation Status](https://readthedocs.org/projects/simple-generation/badge/?version=latest)](https://simple-generation.readthedocs.io/en/latest/?version=latest)
 [![downloads badge](https://pepy.tech/badge/simple-generation/month)](https://pepy.tech/project/simple-generation)
 
 # Simple Generation
 
-Simple Generation offers a minimal interface to run text generation with HuggingFace checkpoint.
-The core idea is to ship many neat features out of the box and avoid boilerplate.
+Simple Generation offers a minimal interface to run text generation with HuggingFace checkpoints.
+The core idea is to ship many neat features out of the box, avoiding boilerplate.
 
-This is mainly for personal use and simple hardware setups (ideally, single-node single- or multi-gpu).
+*Simplegen is mainly for personal use and simple hardware setups (ideally, single-node single- or multi-gpu). If you are looking for production-ready inference engine consider looking elsewhere :) )*
 
 Moreover, please note that **the library will apply some (sensible) defaults (on where to place models, generation configuration, and so on) which might not suit your use case** and should be edited accordingly. Please head to [defaults](#defaults) to see a list of things you should be aware of.
 
 Install:
 ```bash
 pip install simple-generation
 ```
 
-Or, install it from source with:
+If you want to use inference with Vision Language Models (VLMs) run:
 ```bash
-pip install git+https://github.com/MilaNLProc/simple-generation.git
+pip install simple-generation[vlm]
 ```
 
 ## Features
 
 - generate with any model that can be loaded with `AutoModelForCausalLM` or `AutoModelForSeq2SeqLM`
 - batched inference for speed (`batch_size=256`)
 - auto find the largest batch size fitting in your accelerator (`batch_size="auto"`, `starting_batch_size=512`)
@@ -58,14 +60,18 @@
 - load and attach LoRA weights (`lora_weights=...`)
 - chat templates for modern chat models (`apply_chat_template=True` in `__call__`)
 - carbon emission estimates using [codecarbon](https://mlco2.github.io/codecarbon/)
 - sparsity and fused kernels for speed with [optimum](https://huggingface.co/docs/optimum/main/en/index) (`use_bettertransformer=True`)
 - DDP for single-node, multi-gpu setups using [accelerate](https://github.com/huggingface/accelerate). See [Distributed Inference](#distributed-inference)
 - GUI for quick interaction with models using Gradio's [ChatInterface](https://www.gradio.app/guides/creating-a-chatbot-fast#customizing-your-chatbot). See [Chat Interface](#chat-interface)
 
+**Vision-Language Models**
+
+- all of the above for [LLaVA](https://huggingface.co/docs/transformers/main/en/model_doc/llava#overview), [IDEFICS](https://huggingface.co/docs/transformers/main/en/model_doc/idefics#overview), and [BLIP](https://huggingface.co/docs/transformers/main/en/model_doc/blip#overview). For an example look into `./examples/vlm`.
+
 **Loading a Model**
 
 ```python
 from simple_generation import SimpleGenerator
 model_name = "meta-llama/Llama-2-7b-chat-hf"
 generator = SimpleGenerator(model_name, load_in_8bit=True)
 ```
@@ -297,15 +303,14 @@
 >> 219s
 
 # two GPUs, DDP
 CUDA_VISIBLE_DEVICES=0,1 accelerate launch --num_processes 2 examples/inference.py
 >> 105s
 ```
 
-
 ## Defaults
 
 If not specified we set some sensible defaults. **Please note that they might not fit your use case.**
 
 **Default Generation Configuration**
 
 - If not specified otherwise, the library will use the generation configs listed below, **overriding the default config loaded from the specified model**.
@@ -320,15 +325,15 @@
     do_sample: bool = True  # set to False for greedy decoding
     temperature: float = 0.7
     top_p: float = 1.0
     top_k: int = 50
     num_return_sequences: int = 1
 ```
 
-- We set the tokenizer to use left padding. This is required for batched inference with `AutoModelForCausalLM` but should also be fine with any other `AutoModelForSeq2SeqLM` since we use attention masks.
+- We set the tokenizer to use left padding. This is required for batched inference with `AutoModelForCausalLM` but should also be fine with any other `AutoModelForSeq2SeqLM` since we use attention masks. It is also recommended for VLM batch generations. See [this issue](https://github.com/huggingface/transformers/issues/3021#issuecomment-1454266627) and [usage tips](https://huggingface.co/docs/transformers/model_doc/llava_next#usage-tips) for more details.
 
 ## Warning
 
 There seem to be instabilities while using 4bit quantization (not related to this library). Use it only if strictly necessary.
 
 ## Acknowledgments
```

